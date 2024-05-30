# Comparing `tmp/fbgemm_gpu_nightly_cpu-2024.5.29-cp39-cp39-manylinux2014_x86_64.whl.zip` & `tmp/fbgemm_gpu_nightly_cpu-2024.5.30-cp38-cp38-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,62 +1,62 @@
-Zip file size: 3177887 bytes, number of entries: 60
--rw-r--r--  2.0 unx     1342 b- defN 24-May-29 13:06 fbgemm_gpu/__init__.py
--rw-r--r--  2.0 unx     3079 b- defN 24-May-29 13:06 fbgemm_gpu/batched_unary_embeddings_ops.py
--rw-r--r--  2.0 unx      789 b- defN 24-May-29 13:06 fbgemm_gpu/enums.py
--rwxr-xr-x  2.0 unx 10953528 b- defN 24-May-29 13:06 fbgemm_gpu/fbgemm_gpu_py.so
--rw-r--r--  2.0 unx     5663 b- defN 24-May-29 13:06 fbgemm_gpu/metrics.py
--rw-r--r--  2.0 unx     2362 b- defN 24-May-29 13:06 fbgemm_gpu/permute_pooled_embedding_modules.py
--rw-r--r--  2.0 unx     2752 b- defN 24-May-29 13:06 fbgemm_gpu/permute_pooled_embedding_modules_split.py
--rw-r--r--  2.0 unx     7885 b- defN 24-May-29 13:06 fbgemm_gpu/quantize_comm.py
--rw-r--r--  2.0 unx     4020 b- defN 24-May-29 13:06 fbgemm_gpu/quantize_utils.py
--rw-r--r--  2.0 unx     6947 b- defN 24-May-29 13:06 fbgemm_gpu/runtime_monitor.py
--rw-r--r--  2.0 unx    32634 b- defN 24-May-29 13:06 fbgemm_gpu/sparse_ops.py
--rw-r--r--  2.0 unx     5859 b- defN 24-May-29 13:06 fbgemm_gpu/split_embedding_configs.py
--rw-r--r--  2.0 unx     7058 b- defN 24-May-29 13:06 fbgemm_gpu/split_embedding_inference_converter.py
--rw-r--r--  2.0 unx      540 b- defN 24-May-29 13:06 fbgemm_gpu/split_embedding_optimizer_ops.py
--rw-r--r--  2.0 unx    26853 b- defN 24-May-29 13:06 fbgemm_gpu/split_embedding_utils.py
--rw-r--r--  2.0 unx     2339 b- defN 24-May-29 13:06 fbgemm_gpu/split_table_batched_embeddings_ops.py
--rw-r--r--  2.0 unx     4035 b- defN 24-May-29 13:06 fbgemm_gpu/split_table_batched_embeddings_ops_common.py
--rw-r--r--  2.0 unx    67230 b- defN 24-May-29 13:06 fbgemm_gpu/split_table_batched_embeddings_ops_inference.py
--rw-r--r--  2.0 unx   101933 b- defN 24-May-29 13:06 fbgemm_gpu/split_table_batched_embeddings_ops_training.py
--rw-r--r--  2.0 unx    44844 b- defN 24-May-29 13:06 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py
--rw-r--r--  2.0 unx      925 b- defN 24-May-29 13:06 fbgemm_gpu/uvm.py
--rw-r--r--  2.0 unx      419 b- defN 24-May-29 13:06 fbgemm_gpu/docs/__init__.py
--rw-r--r--  2.0 unx      273 b- defN 24-May-29 13:06 fbgemm_gpu/docs/common.py
--rw-r--r--  2.0 unx     2377 b- defN 24-May-29 13:06 fbgemm_gpu/docs/examples.py
--rw-r--r--  2.0 unx     7381 b- defN 24-May-29 13:06 fbgemm_gpu/docs/jagged_tensor_ops.py
--rw-r--r--  2.0 unx     7708 b- defN 24-May-29 13:06 fbgemm_gpu/docs/table_batched_embedding_ops.py
--rw-r--r--  2.0 unx      264 b- defN 24-May-29 13:06 fbgemm_gpu/docs/version.py
--rw-r--r--  2.0 unx     1964 b- defN 24-May-29 13:04 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py
--rw-r--r--  2.0 unx     4181 b- defN 24-May-29 13:04 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py
--rw-r--r--  2.0 unx     4181 b- defN 24-May-29 13:04 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad_pt2.py
--rw-r--r--  2.0 unx     3396 b- defN 24-May-29 13:04 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py
--rw-r--r--  2.0 unx     3396 b- defN 24-May-29 13:04 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam_pt2.py
--rw-r--r--  2.0 unx     2153 b- defN 24-May-29 13:04 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py
--rw-r--r--  2.0 unx     2194 b- defN 24-May-29 13:04 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args_ssd.py
--rw-r--r--  2.0 unx     3396 b- defN 24-May-29 13:04 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
--rw-r--r--  2.0 unx     3396 b- defN 24-May-29 13:04 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb_pt2.py
--rw-r--r--  2.0 unx     3145 b- defN 24-May-29 13:04 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
--rw-r--r--  2.0 unx     3145 b- defN 24-May-29 13:04 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd_pt2.py
--rw-r--r--  2.0 unx     2421 b- defN 24-May-29 13:04 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none.py
--rw-r--r--  2.0 unx     2421 b- defN 24-May-29 13:04 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none_pt2.py
--rw-r--r--  2.0 unx     3101 b- defN 24-May-29 13:04 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py
--rw-r--r--  2.0 unx     3101 b- defN 24-May-29 13:04 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam_pt2.py
--rw-r--r--  2.0 unx     3101 b- defN 24-May-29 13:04 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py
--rw-r--r--  2.0 unx     3101 b- defN 24-May-29 13:04 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb_pt2.py
--rw-r--r--  2.0 unx     4513 b- defN 24-May-29 13:04 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
--rw-r--r--  2.0 unx     4513 b- defN 24-May-29 13:04 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_pt2.py
--rw-r--r--  2.0 unx     3902 b- defN 24-May-29 13:04 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_ssd.py
--rw-r--r--  2.0 unx     3965 b- defN 24-May-29 13:04 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
--rw-r--r--  2.0 unx     3965 b- defN 24-May-29 13:04 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter_pt2.py
--rw-r--r--  2.0 unx     3763 b- defN 24-May-29 13:04 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
--rw-r--r--  2.0 unx     3763 b- defN 24-May-29 13:04 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd_pt2.py
--rw-r--r--  2.0 unx      649 b- defN 24-May-29 13:04 fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py
--rw-r--r--  2.0 unx     6162 b- defN 24-May-29 13:04 fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py
--rw-r--r--  2.0 unx      231 b- defN 24-May-29 13:06 fbgemm_gpu/tbe/__init__.py
--rw-r--r--  2.0 unx      308 b- defN 24-May-29 13:06 fbgemm_gpu/tbe/cache/__init__.py
--rw-r--r--  2.0 unx     1660 b- defN 24-May-29 13:06 fbgemm_gpu/tbe/cache/split_embeddings_cache_ops.py
--rw-r--r--  2.0 unx     2602 b- defN 24-May-29 13:06 fbgemm_gpu_nightly_cpu-2024.5.29.dist-info/METADATA
--rw-r--r--  2.0 unx      105 b- defN 24-May-29 13:06 fbgemm_gpu_nightly_cpu-2024.5.29.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-May-29 13:06 fbgemm_gpu_nightly_cpu-2024.5.29.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     6564 b- defN 24-May-29 13:06 fbgemm_gpu_nightly_cpu-2024.5.29.dist-info/RECORD
-60 files, 11399508 bytes uncompressed, 3166905 bytes compressed:  72.2%
+Zip file size: 3177885 bytes, number of entries: 60
+-rw-r--r--  2.0 unx     1342 b- defN 24-May-30 12:59 fbgemm_gpu/__init__.py
+-rw-r--r--  2.0 unx     3079 b- defN 24-May-30 12:59 fbgemm_gpu/batched_unary_embeddings_ops.py
+-rw-r--r--  2.0 unx      789 b- defN 24-May-30 12:59 fbgemm_gpu/enums.py
+-rwxr-xr-x  2.0 unx 10953528 b- defN 24-May-30 12:59 fbgemm_gpu/fbgemm_gpu_py.so
+-rw-r--r--  2.0 unx     5663 b- defN 24-May-30 12:59 fbgemm_gpu/metrics.py
+-rw-r--r--  2.0 unx     2362 b- defN 24-May-30 12:59 fbgemm_gpu/permute_pooled_embedding_modules.py
+-rw-r--r--  2.0 unx     2752 b- defN 24-May-30 12:59 fbgemm_gpu/permute_pooled_embedding_modules_split.py
+-rw-r--r--  2.0 unx     7885 b- defN 24-May-30 12:59 fbgemm_gpu/quantize_comm.py
+-rw-r--r--  2.0 unx     4020 b- defN 24-May-30 12:59 fbgemm_gpu/quantize_utils.py
+-rw-r--r--  2.0 unx     6947 b- defN 24-May-30 12:59 fbgemm_gpu/runtime_monitor.py
+-rw-r--r--  2.0 unx    32634 b- defN 24-May-30 12:59 fbgemm_gpu/sparse_ops.py
+-rw-r--r--  2.0 unx     5859 b- defN 24-May-30 12:59 fbgemm_gpu/split_embedding_configs.py
+-rw-r--r--  2.0 unx     7058 b- defN 24-May-30 12:59 fbgemm_gpu/split_embedding_inference_converter.py
+-rw-r--r--  2.0 unx      540 b- defN 24-May-30 12:59 fbgemm_gpu/split_embedding_optimizer_ops.py
+-rw-r--r--  2.0 unx    26853 b- defN 24-May-30 12:59 fbgemm_gpu/split_embedding_utils.py
+-rw-r--r--  2.0 unx     2339 b- defN 24-May-30 12:59 fbgemm_gpu/split_table_batched_embeddings_ops.py
+-rw-r--r--  2.0 unx     4035 b- defN 24-May-30 12:59 fbgemm_gpu/split_table_batched_embeddings_ops_common.py
+-rw-r--r--  2.0 unx    67230 b- defN 24-May-30 12:59 fbgemm_gpu/split_table_batched_embeddings_ops_inference.py
+-rw-r--r--  2.0 unx   101933 b- defN 24-May-30 12:59 fbgemm_gpu/split_table_batched_embeddings_ops_training.py
+-rw-r--r--  2.0 unx    44844 b- defN 24-May-30 12:59 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py
+-rw-r--r--  2.0 unx      925 b- defN 24-May-30 12:59 fbgemm_gpu/uvm.py
+-rw-r--r--  2.0 unx      419 b- defN 24-May-30 12:59 fbgemm_gpu/docs/__init__.py
+-rw-r--r--  2.0 unx      273 b- defN 24-May-30 12:59 fbgemm_gpu/docs/common.py
+-rw-r--r--  2.0 unx     2377 b- defN 24-May-30 12:59 fbgemm_gpu/docs/examples.py
+-rw-r--r--  2.0 unx     7381 b- defN 24-May-30 12:59 fbgemm_gpu/docs/jagged_tensor_ops.py
+-rw-r--r--  2.0 unx     7708 b- defN 24-May-30 12:59 fbgemm_gpu/docs/table_batched_embedding_ops.py
+-rw-r--r--  2.0 unx      264 b- defN 24-May-30 12:59 fbgemm_gpu/docs/version.py
+-rw-r--r--  2.0 unx     1964 b- defN 24-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py
+-rw-r--r--  2.0 unx     4181 b- defN 24-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py
+-rw-r--r--  2.0 unx     4181 b- defN 24-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad_pt2.py
+-rw-r--r--  2.0 unx     3396 b- defN 24-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py
+-rw-r--r--  2.0 unx     3396 b- defN 24-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam_pt2.py
+-rw-r--r--  2.0 unx     2153 b- defN 24-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py
+-rw-r--r--  2.0 unx     2194 b- defN 24-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args_ssd.py
+-rw-r--r--  2.0 unx     3396 b- defN 24-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
+-rw-r--r--  2.0 unx     3396 b- defN 24-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb_pt2.py
+-rw-r--r--  2.0 unx     3145 b- defN 24-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
+-rw-r--r--  2.0 unx     3145 b- defN 24-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd_pt2.py
+-rw-r--r--  2.0 unx     2421 b- defN 24-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none.py
+-rw-r--r--  2.0 unx     2421 b- defN 24-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none_pt2.py
+-rw-r--r--  2.0 unx     3101 b- defN 24-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py
+-rw-r--r--  2.0 unx     3101 b- defN 24-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam_pt2.py
+-rw-r--r--  2.0 unx     3101 b- defN 24-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py
+-rw-r--r--  2.0 unx     3101 b- defN 24-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb_pt2.py
+-rw-r--r--  2.0 unx     4513 b- defN 24-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
+-rw-r--r--  2.0 unx     4513 b- defN 24-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_pt2.py
+-rw-r--r--  2.0 unx     3902 b- defN 24-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_ssd.py
+-rw-r--r--  2.0 unx     3965 b- defN 24-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
+-rw-r--r--  2.0 unx     3965 b- defN 24-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter_pt2.py
+-rw-r--r--  2.0 unx     3763 b- defN 24-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
+-rw-r--r--  2.0 unx     3763 b- defN 24-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd_pt2.py
+-rw-r--r--  2.0 unx      649 b- defN 24-May-30 12:57 fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py
+-rw-r--r--  2.0 unx     6162 b- defN 24-May-30 12:57 fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py
+-rw-r--r--  2.0 unx      231 b- defN 24-May-30 12:59 fbgemm_gpu/tbe/__init__.py
+-rw-r--r--  2.0 unx      308 b- defN 24-May-30 12:59 fbgemm_gpu/tbe/cache/__init__.py
+-rw-r--r--  2.0 unx     1660 b- defN 24-May-30 12:59 fbgemm_gpu/tbe/cache/split_embeddings_cache_ops.py
+-rw-r--r--  2.0 unx     2602 b- defN 24-May-30 12:59 fbgemm_gpu_nightly_cpu-2024.5.30.dist-info/METADATA
+-rw-r--r--  2.0 unx      105 b- defN 24-May-30 12:59 fbgemm_gpu_nightly_cpu-2024.5.30.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-May-30 12:59 fbgemm_gpu_nightly_cpu-2024.5.30.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     6564 b- defN 24-May-30 12:59 fbgemm_gpu_nightly_cpu-2024.5.30.dist-info/RECORD
+60 files, 11399508 bytes uncompressed, 3166903 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -162,20 +162,20 @@
 
 Filename: fbgemm_gpu/tbe/cache/__init__.py
 Comment: 
 
 Filename: fbgemm_gpu/tbe/cache/split_embeddings_cache_ops.py
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2024.5.29.dist-info/METADATA
+Filename: fbgemm_gpu_nightly_cpu-2024.5.30.dist-info/METADATA
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2024.5.29.dist-info/WHEEL
+Filename: fbgemm_gpu_nightly_cpu-2024.5.30.dist-info/WHEEL
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2024.5.29.dist-info/top_level.txt
+Filename: fbgemm_gpu_nightly_cpu-2024.5.30.dist-info/top_level.txt
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2024.5.29.dist-info/RECORD
+Filename: fbgemm_gpu_nightly_cpu-2024.5.30.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fbgemm_gpu/fbgemm_gpu_py.so

### strings --all --bytes=8 {}

```diff
@@ -16161,53 +16161,53 @@
 SymFloat
 GenericList
 PyObject
 Uninitialized
 Quantizer
 Generator
 InvalidTag(
-extra_meta_ && extra_meta_->symbolic_shape_meta_ INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/TensorImpl.h":1723, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/TensorImpl.h
+extra_meta_ && extra_meta_->symbolic_shape_meta_ INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/TensorImpl.h":1723, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/TensorImpl.h
 /__w/FBGEMM/FBGEMM/fbgemm_gpu/codegen/training/forward/embedding_forward_split_cpu.cpp
 Expected !indice_weights.defined() || indice_weights.scalar_type() != at::kHalf to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 split_embedding_codegen_forward_cpu_meta
 split_embedding_codegen_forward_cpu(Tensor weights, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, Tensor hash_size_cumsum, Tensor indices, Tensor offsets, int pooling_mode, Tensor indice_weights, int output_dtype) -> Tensor
 Expected weights.is_contiguous() to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 split_embedding_forward_cpu_kernel
 split_embedding_grad_indice_weights_cpu_outer
 split_embedding_grad_indice_weights_cpu
 split_embedding_codegen_grad_indice_weights_cpu(Tensor grad_output, Tensor weights, Tensor weights_offsets, Tensor D_offsets, Tensor indices, Tensor offsets, Tensor feature_requires_grad) -> Tensor
 tensor does not have a device
 device_default
 There is an error in the layout calculation logic.
-is_mkldnn() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/TensorImpl.h":1290, please report a bug to PyTorch. 
+is_mkldnn() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/TensorImpl.h":1290, please report a bug to PyTorch. 
 Operators taking TensorOptions cannot take a TensorOptions with options.requires_grad set as true. This isn't implemented yet.
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/CheckMemoryFormat.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/CheckMemoryFormat.h
 check_tensor_options_and_extract_memory_format
 Cannot set memory_format both in TensorOptions and explicit argument; please delete the redundant setter.
 basic_string::_S_construct null not valid
 basic_string::append
 IntArrayRef contains an int that cannot be represented as a SymInt: 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/SymIntArrayRef.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/SymIntArrayRef.h
 fromIntArrayRefSlow
  dims but tensor has 
 TensorAccessor expected 
 accessor
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/TensorBase.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/TensorBase.h
  is out of bounds: 
 , range 
 report_embedding_error
 /__w/FBGEMM/FBGEMM/fbgemm_gpu/include/fbgemm_gpu/cpu_utils.h
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h
-0 INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h":652, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue.h
+0 INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue.h":652, please report a bug to PyTorch. 
 expected int
 vector::_M_realloc_insert
 Expected SymInt or int but got 
-isSymInt() || isInt() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":237, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h
+isSymInt() || isInt() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":237, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h
 toSymInt
 St19bad_optional_access
 N3c1020intrusive_ptr_targetE
 N3c1014OperatorKernelE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_S5_S5_S5_EXadL_Z47split_embedding_codegen_grad_indice_weights_cpuS5_S5_S5_S5_S5_S5_S5_EEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S5_S5_S5_EEEEE
 FN2at6TensorES0_S0_S0_S0_S0_S0_S0_E
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_NS_6SymIntES5_S5_S5_lS5_lEXadL_Z35split_embedding_codegen_forward_cpuS5_S5_S5_S6_S5_S5_S5_lS5_lEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S6_S5_S5_S5_lS5_lEEEEE
@@ -16236,136 +16236,136 @@
 __obj_flatten__
 Expected GenericDict but got 
 toGenericDict
 Unknown Exception Type
  devices
 getDeviceGuardImpl
 PyTorch is not linked with support for 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/impl/DeviceGuardImplInterface.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/impl/DeviceGuardImplInterface.h
 Event device type 
  does not match blocking stream's device type 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/impl/InlineEvent.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/impl/InlineEvent.h
 Expected !name.empty() to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/qualified_name.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/qualified_name.h
 Invalid name for qualified name: '
-!atom.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/qualified_name.h":24, please report a bug to PyTorch. 
-!finalAtom.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/qualified_name.h":32, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/util/ArrayRef.h
+!atom.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/qualified_name.h":24, please report a bug to PyTorch. 
+!finalAtom.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/qualified_name.h":32, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/util/ArrayRef.h
 QualifiedName
 basic_string::substr
 ArrayRef: invalid slice, N = 
 ; size = 
 Expected a 0-dim Tensor, but got Tensor with dimensions: 
-tensor.dim() == 0 INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":317, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h
+tensor.dim() == 0 INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":317, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h
  in its first dimension, but got Tensor with size 
-tensor.sizes()[0] == (int64_t)init_list_.size() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":324, please report a bug to PyTorch. 
+tensor.sizes()[0] == (int64_t)init_list_.size() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":324, please report a bug to PyTorch. 
 TensorDataContainer is already a Tensor type, `fill_tensor` should not be called
-false INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":338, please report a bug to PyTorch. 
+false INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":338, please report a bug to PyTorch. 
 Invalid TensorDataContainer type
-false INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":342, please report a bug to PyTorch. 
+false INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":342, please report a bug to PyTorch. 
 fill_tensor
 Expected a Tensor with size 
  in its first dimension
 can not do torch::tensor(complex, dtype=non-complex) because complex can not be casted to real number without loss of information
-false INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":272, please report a bug to PyTorch. 
+false INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":272, please report a bug to PyTorch. 
 convert_to_tensor
 /__w/FBGEMM/FBGEMM/fbgemm_gpu/codegen/inference/embedding_forward_quantized_host_cpu.cpp
 int_nbit_split_embedding_uvm_caching_codegen_lookup_function shouldn't be called for CPU; it is only for GPU.
-isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":1966, please report a bug to PyTorch. 
+isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":1966, please report a bug to PyTorch. 
 vector::_M_range_check: __n (which is %zu) >= this->size() (which is %zu)
 __getstate__ should take exactly one argument: self. Got: 
 self argument of __getstate__ must be the custom class type. Got 
 __getstate__ should return exactly one value for serialization. Got: 
 __getstate__'s return type should be a subtype of input argument of __setstate__. Got 
-isString() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":2355, please report a bug to PyTorch. 
+isString() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":2355, please report a bug to PyTorch. 
 //deeplearning/fbgemm/fbgemm_gpu:sparse_ops_py
 int_nbit_split_embedding_codegen_lookup_function(Tensor dev_weights, Tensor uvm_weights, Tensor weights_placements, Tensor weights_offsets, Tensor weights_tys, Tensor D_offsets, SymInt total_D, int max_int2_D, int max_int4_D, int max_int8_D, int max_float16_D, int max_float32_D, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, int output_dtype=1, Tensor? lxu_cache_weights=None, Tensor? lxu_cache_locations=None, int? row_alignment = None, int? max_float8_D=0, int? fp8_exponent_bits=-1, int? fp8_exponent_bias=-1) -> Tensor
 int_nbit_split_embedding_codegen_lookup_function
 int_nbit_split_embedding_uvm_caching_codegen_lookup_function(Tensor dev_weights, Tensor uvm_weights, Tensor weights_placements, Tensor weights_offsets, Tensor weights_tys, Tensor D_offsets, SymInt total_D, int max_int2_D, int max_int4_D, int max_int8_D, int max_float16_D, int max_float32_D, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights=None, int output_dtype=1, Tensor? lxu_cache_weights=None, Tensor? lxu_cache_locations=None, int? row_alignment=-1, int? max_float8_D=0, int? fp8_exponent_bits=-1, int? fp8_exponent_bias=-1, Tensor? cache_hash_size_cumsum=None, int? total_cache_hash_size=-1, Tensor? cache_index_table_map=None, Tensor? lxu_cache_state=None, Tensor? lxu_state=None) -> Tensor
 int_nbit_split_embedding_uvm_caching_codegen_lookup_function
 pruned_hashmap_insert(Tensor indices, Tensor dense_indices, Tensor offsets, Tensor(a!) hash_table, Tensor hash_table_offsets) -> ()
 pruned_hashmap_lookup(Tensor indices, Tensor offsets, Tensor hash_table, Tensor hash_table_offsets) -> Tensor
 pruned_array_lookup(Tensor indices, Tensor offsets, Tensor index_remappings, Tensor index_remappings_offsets) -> Tensor
-isGenericDict() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":2082, please report a bug to PyTorch. 
-self_impl INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/variable.h":305, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/variable.h
+isGenericDict() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":2082, please report a bug to PyTorch. 
+self_impl INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/variable.h":305, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/variable.h
 Only Tensors of floating point and complex dtype can require gradients
 AutogradMeta
 set_requires_grad
 Expected T > 0 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected B > 0 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected maps_.size() == T to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 , got one on device 
 getDevicesOfStorages
 Expected all data ptrs to be on a device of type 
 vector::reserve
 Expected map.size() == (table_offsets_acc[t + 1] - table_offsets_acc[t]) to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 serialize
 table_offsets
 vector::_M_fill_insert
-schema_.returns().size() == 1 INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/builtin_function.h":22, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/builtin_function.h
+schema_.returns().size() == 1 INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/builtin_function.h":22, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/builtin_function.h
 BuiltinOpFunction
 defineMethod
 Default values must be specified for none or all arguments
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/custom_class.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/custom_class.h
 TensorImpl with nullptr is not supported
 init_tensor
 vector::_M_default_append
 cannot create std::deque larger than max_size()
 *ZN5torch6class_I12PrunedMapCPUE12defineMethodIZNS2_10def_pickleINL20PrunedMapCPURegistryMUlRKN3c1013intrusive_ptrIS1_NS5_6detail34intrusive_target_default_null_typeIS1_EEEEE_ENL20PrunedMapCPURegistryMUlSsE0_EEERS2_OT_OT0_EUlNS5_14tagged_capsuleIS1_EEOSsE_EEPNS_3jit8FunctionESsSG_SsSt16initializer_listINS_3argEEEUlRSt6vectorINS5_6IValueESaISV_EEE_
 *ZN5torch6class_I13AtomicCounterE12defineMethodIZNS2_10def_pickleINL21AtomicCounterRegistryMUlRKN3c1013intrusive_ptrIS1_NS5_6detail34intrusive_target_default_null_typeIS1_EEEEE_ENL21AtomicCounterRegistryMUlSsE0_EEERS2_OT_OT0_EUlNS5_14tagged_capsuleIS1_EEOSsE_EEPNS_3jit8FunctionESsSG_SsSt16initializer_listINS_3argEEEUlRSt6vectorINS5_6IValueESaISV_EEE_
 *ZN5torch6class_I11TensorQueueE12defineMethodIZNS2_10def_pickleINL19TensorQueueRegistryMUlRKN3c1013intrusive_ptrIS1_NS5_6detail34intrusive_target_default_null_typeIS1_EEEEE_ENL19TensorQueueRegistryMUlNS5_4DictISsN2at6TensorEEEE0_EEERS2_OT_OT0_EUlNS5_14tagged_capsuleIS1_EEOSH_E_EEPNS_3jit8FunctionESsSK_SsSt16initializer_listINS_3argEEEUlRSt6vectorINS5_6IValueESaISZ_EEE_
 *ZN5torch6class_I12PrunedMapCPUE12defineMethodINL20PrunedMapCPURegistryMUlRKN3c1013intrusive_ptrIS1_NS4_6detail34intrusive_target_default_null_typeIS1_EEEEE_EEEPNS_3jit8FunctionESsT_SsSt16initializer_listINS_3argEEEUlRSt6vectorINS4_6IValueESaISL_EEE_
 *ZN5torch6class_I13AtomicCounterE12defineMethodINL21AtomicCounterRegistryMUlRKN3c1013intrusive_ptrIS1_NS4_6detail34intrusive_target_default_null_typeIS1_EEEEE_EEEPNS_3jit8FunctionESsT_SsSt16initializer_listINS_3argEEEUlRSt6vectorINS4_6IValueESaISL_EEE_
 *ZN5torch6class_I11TensorQueueE12defineMethodINL19TensorQueueRegistryMUlRKN3c1013intrusive_ptrIS1_NS4_6detail34intrusive_target_default_null_typeIS1_EEEEE_EEEPNS_3jit8FunctionESsT_SsSt16initializer_listINS_3argEEEUlRSt6vectorINS4_6IValueESaISL_EEE_
 Expected Object but got 
 toObject
-isObject() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":133, please report a bug to PyTorch. 
+isObject() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":133, please report a bug to PyTorch. 
 Argument passed to at() was not in the map.
 Streams have a mix of device types: stream 0 is on 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/impl/InlineStreamGuard.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/impl/InlineStreamGuard.h
  while stream 
  is on device 
 getDeviceTypeOfStreams
 , trying to set error: 
 setErrorInternal
 Error already set on this Future: 
 Future is already marked completed
-!completed() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":1215, please report a bug to PyTorch. 
+!completed() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":1215, please report a bug to PyTorch. 
  which are not among the expected device(s) 
 The result contained tensors residing on device(s) 
 Attempting to mark a completed Future as complete again. Note that a Future can only be marked completed once.
  does not match recording stream's device type 
 ensureIsSubsetOfDevices
 markCompleted
 constexpr c10::string_view c10::util::detail::fully_qualified_type_name_impl() [with T = c10::intrusive_ptr<TensorQueue>; c10::string_view = c10::basic_string_view<char>]
  could not be converted to any of the known types.
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/jit_type.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/jit_type.h
 constexpr c10::string_view c10::util::detail::fully_qualified_type_name_impl() [with T = c10::tagged_capsule<TensorQueue>; c10::string_view = c10::basic_string_view<char>]
 constexpr c10::string_view c10::util::detail::fully_qualified_type_name_impl() [with T = c10::intrusive_ptr<AtomicCounter>; c10::string_view = c10::basic_string_view<char>]
 constexpr c10::string_view c10::util::detail::fully_qualified_type_name_impl() [with T = c10::tagged_capsule<AtomicCounter>; c10::string_view = c10::basic_string_view<char>]
 constexpr c10::string_view c10::util::detail::fully_qualified_type_name_impl() [with T = c10::intrusive_ptr<PrunedMapCPU>; c10::string_view = c10::basic_string_view<char>]
 constexpr c10::string_view c10::util::detail::fully_qualified_type_name_impl() [with T = c10::tagged_capsule<PrunedMapCPU>; c10::string_view = c10::basic_string_view<char>]
 Tried to cast IValue to custom class but it did not contain a custom class!
-isCapsule() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":225, please report a bug to PyTorch. 
+isCapsule() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":225, please report a bug to PyTorch. 
 toCustomClass
 toCapsule
 Expected TensorList but got 
 toTensorList
-isTensorList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":2038, please report a bug to PyTorch. 
+isTensorList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":2038, please report a bug to PyTorch. 
 Tried to cast a Dict<
 > to a Dict<
 >. Key types mismatch.
 toTypedDict
 >. Value types mismatch.
-*getTypePtr<Key>() == *dict.impl_->elementTypes.keyType INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/Dict_inl.h":26, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/Dict_inl.h
-*getTypePtr<Value>() == *dict.impl_->elementTypes.valueType INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/Dict_inl.h":27, please report a bug to PyTorch. 
+*getTypePtr<Key>() == *dict.impl_->elementTypes.keyType INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/Dict_inl.h":26, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/Dict_inl.h
+*getTypePtr<Value>() == *dict.impl_->elementTypes.valueType INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/Dict_inl.h":27, please report a bug to PyTorch. 
 N3c1010ValueErrorE
 N3c1011StorageImplE
 N3c1015VariableVersion14VersionCounterE
 N3c104impl24DeviceGuardImplInterfaceE
 N3c106detail8ListImplE
 N5torch17CustomClassHolderE
 N3c106detail8DictImplE
@@ -16413,42 +16413,42 @@
 pooling_mode
 function 
 apply_with_saved
 missing before())
 vector<bool>::_M_insert_aux
 Please open a feature request on GitHub if you need this.
 jvp is not implemented for the c++ API of custom Function yet.
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/custom_function.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/custom_function.h
 compiled_args not implemented for non-traceable node: 
 dense_embedding_codegen_lookup_function(Tensor dev_weights, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, int output_dtype=0, Tensor? B_offsets=None, Tensor? vbe_output_offsets_feature_rank=None, Tensor? vbe_B_offsets_rank_per_feature=None, SymInt max_B=-1, SymInt max_B_feature_rank=-1, SymInt vbe_output_size=-1) -> Tensor
 dense_embedding_codegen_lookup_function
 Cannot update a node's topological_nr after it already has a parent. If we allow this, we can no longer guarantee that a parent's topo_nr is always greater than those of all its children
-!has_parent_ INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/function.h":262, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/function.h
+!has_parent_ INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/function.h":262, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/function.h
 /__w/FBGEMM/FBGEMM/fbgemm_gpu/codegen/training/backward/embedding_backward_dense_host_cpu.cpp
 Check failed: grad_outputs.size() == 1 (
  returned an incorrect number of gradients (expected 
  returned a gradient different that is defined at position 
 , but the corresponding forward input was not a Variable
-ctx_.non_differentiable_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/custom_function.h":221, please report a bug to PyTorch. 
-ctx_.dirty_inputs_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/custom_function.h":222, please report a bug to PyTorch. 
-it != _saved_variables.end() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h":138, please report a bug to PyTorch. 
-arg.proxy_tensor.defined() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h":561, please report a bug to PyTorch. 
-ctx_.to_save_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/custom_function.h":224, please report a bug to PyTorch. 
-it != this->end() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h":760, please report a bug to PyTorch. 
-ctx_.non_differentiable_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/custom_function.h":231, please report a bug to PyTorch. 
-ctx_.dirty_inputs_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/custom_function.h":232, please report a bug to PyTorch. 
-ctx_.to_save_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/custom_function.h":234, please report a bug to PyTorch. 
+ctx_.non_differentiable_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/custom_function.h":221, please report a bug to PyTorch. 
+ctx_.dirty_inputs_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/custom_function.h":222, please report a bug to PyTorch. 
+it != _saved_variables.end() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h":138, please report a bug to PyTorch. 
+arg.proxy_tensor.defined() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h":561, please report a bug to PyTorch. 
+ctx_.to_save_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/custom_function.h":224, please report a bug to PyTorch. 
+it != this->end() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h":760, please report a bug to PyTorch. 
+ctx_.non_differentiable_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/custom_function.h":231, please report a bug to PyTorch. 
+ctx_.dirty_inputs_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/custom_function.h":232, please report a bug to PyTorch. 
+ctx_.to_save_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/custom_function.h":234, please report a bug to PyTorch. 
 *N5torch8autograd7CppNodeIN12_GLOBAL__N_128SplitLookupFunction_Dense_OpEEE
 *ZN5torch8autograd8FunctionIN12_GLOBAL__N_128SplitLookupFunction_Dense_OpEE5applyIS3_JRKN2at6TensorES9_S9_RN3c106SymIntESC_S9_RKlS9_S9_SE_RKSt8optionalIS7_ESI_EEENSt9enable_ifIX9is_same_vIT_S3_EEDTclsrSK_7forwardLDnEspcl7declvalIT0_EEEEE4typeEDpOSL_EUlRKSt6vectorIS7_SaIS7_EESV_E_
 *ZN5torch8autograd8FunctionIN12_GLOBAL__N_128SplitLookupFunction_Dense_OpEE5applyIS3_JRKN2at6TensorES9_S9_RN3c106SymIntESC_S9_RKlS9_S9_SE_RKSt8optionalIS7_ESI_EEENSt9enable_ifIX9is_same_vIT_S3_EEDTclsrSK_7forwardLDnEspcl7declvalIT0_EEEEE4typeEDpOSL_EUlS9_E0_
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_NS_6SymIntES8_S7_lS7_S7_lRKSt8optionalIS5_ESC_lSC_SC_SC_S8_S8_S8_EXadL_ZN12_GLOBAL__N_145split_embedding_codegen_lookup_dense_functionES7_S7_S7_S8_S8_S7_lS7_S7_lSC_SC_lSC_SC_SC_S8_S8_S8_EEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S8_S8_S7_lS7_S7_lSC_SC_lSC_SC_SC_S8_S8_S8_EEEEE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN12_GLOBAL__N_128SplitLookupFunction_Dense_OpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
-sym_sizes_index < sym_sizes.size() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h":531, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h
+sym_sizes_index < sym_sizes.size() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h":531, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h
 next_sym_size
 PFvPN5torch8autograd4NodeEE
 FN2at6TensorERKS0_S2_S2_N3c106SymIntES4_S2_lS2_S2_lRKSt8optionalIS0_ES8_lS8_S8_S8_S4_S4_S4_E
 bounds_check_indices_cpu
 offsets size 
  is not equal to B (
 weights size 
@@ -16486,37 +16486,37 @@
 sum_reduce_to_one
 merge_pooled_embeddings
 t must be a CPU tensor; it is currently on device 
 /__w/FBGEMM/FBGEMM/fbgemm_gpu/src/merge_pooled_embedding_ops/merge_pooled_embedding_ops_cpu.cpp
 Expected input_tensors.size() > 0 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 input_0 must be a CPU tensor; it is currently on device 
 input_tensors[i] must be a CPU tensor; it is currently on device 
-isDevice() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h":931, please report a bug to PyTorch. 
-isTensorList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":2034, please report a bug to PyTorch. 
+isDevice() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue.h":931, please report a bug to PyTorch. 
+isTensorList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":2034, please report a bug to PyTorch. 
 toDevice
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorESt6vectorIS5_SaIS5_EElNS_6DeviceElEXadL_ZN10fbgemm_gpu27merge_pooled_embeddings_cpuES8_lS9_lEEEES5_NS_4guts8typelist8typelistIJS8_lS9_lEEEEE
 FN2at6TensorESt6vectorIS0_SaIS0_EElN3c106DeviceElE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorESt6vectorIS5_SaIS5_EENS_6DeviceEEXadL_ZN10fbgemm_gpu21sum_reduce_to_one_cpuES8_S9_EEEES5_NS_4guts8typelist8typelistIJS8_S9_EEEEE
 FN2at6TensorESt6vectorIS0_SaIS0_EEN3c106DeviceEE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFSt6vectorIN2at6TensorESaIS6_EES8_NS_6DeviceEEXadL_ZN10fbgemm_gpu21all_to_one_device_cpuES8_S9_EEEES8_NS_4guts8typelist8typelistIJS8_S9_EEEEE
 FSt6vectorIN2at6TensorESaIS1_EES3_N3c106DeviceEE
 merge_pooled_embeddings(Tensor[] pooled_embeddings, SymInt uncat_dim_size, Device target_device, SymInt cat_dim=all_to_one_device(Tensor[] input_tensors, Device target_device) sum_reduce_to_onfbgemm::permute_pooled_embs
 expected bool
 fbgemm::permute_duplicate_pooled_embs
 offset_dim_list needs to have long/int64 type
 /__w/FBGEMM/FBGEMM/fbgemm_gpu/src/permute_pooled_embedding_ops/permute_pooled_embedding_function.cpp
 permute_list needs to have long/int64 type
 Expected ptr_->is_bool() to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/SymBool.h
-0 INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h":676, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/SymBool.h
+0 INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue.h":676, please report a bug to PyTorch. 
 permute_pooled_embs does not support allow_duplicates in backward!
 Tried to access the schema for 
  which doesn't have a schema registered yet
-schema_.has_value() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/dispatch/OperatorEntry.h":80, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/dispatch/OperatorEntry.h
+schema_.has_value() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/dispatch/OperatorEntry.h":80, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/dispatch/OperatorEntry.h
 FN2at6TensorERKS0_S2_S2_S2_S2_E
 inv_offset_dim_linv_permute_listallow_duplicatespermute_pooled_embs_cpu_impl
 permute_pooled_embs_auto_grad
 permute_duplicate_pooled_embs
 /__w/FBGEMM/FBGEMM/fbgemm_gpu/src/permute_pooled_embedding_ops/permute_pooled_embedding_ops_cpu.cpp
 permute_duplicate_pooled_embs_auto_grad
 N5torch8autograd7CppNodeIN10fbgemm_gpu25PermutePooledEmbsFunctionEEE
@@ -16575,27 +16575,27 @@
 num_output_rows
 slice_length
 fbgemm::jagged_slice_forward
 lengths is currently on 
 start should be <= len
 jagged_dense_dense_elementwise_add_jagged_output
 batched_dense_vec_jagged_2d_mul
-isList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":2066, please report a bug to PyTorch. 
+isList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":2066, please report a bug to PyTorch. 
 /__w/FBGEMM/FBGEMM/fbgemm_gpu/src/jagged_tensor_ops/jagged_tensor_ops_autograd.cpp
 Expected grad_outputs.size() == 1 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected total_L >= 0 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 fbgemm::jagged_to_padded_dense_backward
 fbgemm::jagged_to_padded_dense_forward
 Expected values.dim() == 1 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected offsets.dim() == 1 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected max_L > 0 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected max_lengths.size() == x_offsets.size() to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected SymIntList or IntList but got 
-isSymIntList() || isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":1978, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/SymInt.h
+isSymIntList() || isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":1978, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/SymInt.h
 Expected dense_values_grad.sym_sizes() == dense_shape to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 fbgemm::jagged_dense_dense_elementwise_add_jagged_output_forward
 fbgemm::jagged_dense_elementwise_mul_backward
 fbgemm::jagged_dense_elementwise_mul_forward
 fbgemm::batched_dense_vec_jagged_2d_mul_backward
 fbgemm::batched_dense_vec_jagged_2d_mul_forward
 fbgemm::dense_to_jagged_forward
@@ -16615,15 +16615,15 @@
 fbgemm::jagged_index_select_2d_forward_v2
 output_lengths is currently on 
 grad must be on the same device as output_lengths! grad is currently on 
 Tensor 'values' must have 1 dimension(s). Found 
 values must be on the same device as lengths! values is currently on 
 start should be always be positive
 type with contained types did not overload createWithContained: 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/jit_type_base.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/jit_type_base.h
 createWithContained
 ; Length = 
 ArrayRef: invalid index Index = 
  with None type
 Can not create 
 : SymIntArrayRef expected to contain only concrete integers
 asIntArrayRefSlow
@@ -16669,24 +16669,24 @@
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN10fbgemm_gpu12_GLOBAL__N_115DenseToJaggedOpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN10fbgemm_gpu12_GLOBAL__N_136JaggedDenseElementwiseAddJaggedOutOpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN10fbgemm_gpu12_GLOBAL__N_115JaggedSoftmaxOpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN10fbgemm_gpu12_GLOBAL__N_117JaggedJaggedBmmOpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN10fbgemm_gpu12_GLOBAL__N_116JaggedDenseBmmOpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN10fbgemm_gpu12_GLOBAL__N_121JaggedIndexSelect2dOpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN10fbgemm_gpu12_GLOBAL__N_113JaggedSliceOpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
-isSymInt() || isInt() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":245, please report a bug to PyTorch. 
+isSymInt() || isInt() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":245, please report a bug to PyTorch. 
 Tried to cast a List<
 > to a List<
 >. Types mismatch.
 toTypedList
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/List_inl.h
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/boxing/KernelFunction_impl.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/List_inl.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/boxing/KernelFunction_impl.h
 Expected ptr_->is_float() to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/SymFloat.h
-0 INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h":540, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/SymFloat.h
+0 INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue.h":540, please report a bug to PyTorch. 
 expected double
 toDouble
 St23enable_shared_from_thisIN3c1010SharedTypeEE
 N3c1010SharedTypeE
 N3c1017SingleElementTypeILNS_8TypeKindE6ENS_8ListTypeEEE
 FN2at6TensorERKS0_RKSt6vectorIS0_SaIS0_EEN3c108ArrayRefINS8_6SymIntEEEdE
 FN2at6TensorERKS0_RKSt6vectorIS0_SaIS0_EEN3c108ArrayRefIlEEdE
@@ -16883,15 +16883,15 @@
 jagged_jagged_elementwise_dense_output_kernel_
 Expected !NO_INNER_DENSE || output.size(-1) == 1 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 unsupported number of jagged dim 
 jagged_2d_to_dense_forward_cpu
 jagged_2d_to_dense_backward_kernel
 fbgemm::jagged_index_select_2d_forward
 fbgemm::jagged_index_add_2d_forward
-isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":1962, please report a bug to PyTorch. 
+isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":1962, please report a bug to PyTorch. 
 FN2at6TensorERKS0_S2_S2_S2_lE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_RKSt6vectorIS5_SaIS5_EES7_EXadL_ZN10fbgemm_gpu28jagged_dense_elementwise_addES7_SC_S7_EEEES5_NS_4guts8typelist8typelistIJS7_SC_S7_EEEEE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFSt6vectorIN2at6TensorESaIS6_EES6_S6_RKS4_IlSaIlEESC_lEXadL_ZN10fbgemm_gpu30stacked_jagged_1d_to_dense_cpuES6_S6_SC_SC_lEEEES8_NS_4guts8typelist8typelistIJS6_S6_SC_SC_lEEEEE
 FSt6vectorIN2at6TensorESaIS1_EES1_S1_RKS_IlSaIlEES7_lE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFSt6vectorIN2at6TensorESaIS6_EES6_S6_RKS4_IlSaIlEESC_lEXadL_ZN10fbgemm_gpu30stacked_jagged_2d_to_dense_cpuES6_S6_SC_SC_lEEEES8_NS_4guts8typelist8typelistIJS6_S6_SC_SC_lEEEEE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_lEXadL_ZN10fbgemm_gpu34jagged_index_select_2d_forward_cpuES7_S7_S7_S7_lEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_lEEEEE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_llEXadL_ZN10fbgemm_gpu31jagged_index_add_2d_forward_cpuES7_S7_S7_S7_llEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_llEEEEE
@@ -17470,15 +17470,15 @@
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_S7_bEXadL_Z43batch_index_select_dim0_tensor_cpu_autogradS7_S7_S7_S7_S7_bEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_S7_bEEEEE
 FN2at6TensorERKS0_S2_S2_S2_S2_bE
 St19_Sp_counted_deleterIPN5torch8autograd7CppNodeI25BatchIndexSelectDim0CPUOpEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 St19_Sp_counted_deleterIPN5torch8autograd7CppNodeI31BatchIndexSelectDim0TensorCPUOpEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 Unsupported SparseType: 
 pruned_array_lookup_cpu
 Expected placement != PlacementType::DEVICE to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_forward_quantized_unweighted_codegen_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_forward_quantized_unweighted_codegen_cpu.cpp
 int8 output are only supported for int8 weights
 Expected offsets_nobag.numel() == index_size + 1 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected offsets_nobag_ptr[index_size] - offsets_nobag_ptr[0] == index_size to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 int_nbit_split_embedding_codegen_forward_unweighted_cpu
 Expected B >= 0 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected total_D > 0 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Enabling both CUDA and HIP in ATen is not supported, as HIP masquerades to be CUDA (e.g., when you say CUDA, on a HIP build of ATen, this actually means HIP.  Rebuild PyTorch with one or the other disabled.
@@ -17491,30 +17491,30 @@
 int_nbit_split_embedding_nobag_codegen_forward_
 "intn_split_embedding_nobag_codegen_forward_kernel"
 pruned_hashmap_lookup_unweighted_cpu
 hash_table must be a CPU tensor; it is currently on device 
 hash_table_offsets must be a CPU tensor; it is currently on device 
 pruned_hashmap_insert_unweighted_cpu
 dense_indices must be a CPU tensor; it is currently on device 
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_forward_quantized_weighted_codegen_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_forward_quantized_weighted_codegen_cpu.cpp
 pruned_hashmap_lookup_weighted_cpu
 pruned_hashmap_insert_weighted_cpu
 int_nbit_split_embedding_codegen_forward_weighted_cpu
 indice_weights must be empty or a CPU tensor; it is currently on device 
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_dense_split_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_dense_split_cpu.cpp
 Check failed: host_weights.dim() == 1 (
 split_embedding_backward_exact_cpu
 split_embedding_backward_codegen_dense_cpu(Tensor grad_output, Tensor(a!) host_weights, Tensor weights_offsets, Tensor D_offsets, int max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets,int pooling_mode, Tensor indice_weights, float unused = 0) -> Tensor
 split_embedding_backward_codegen_dense_cpu
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_lS5_lS5_S5_lS5_dEXadL_Z42split_embedding_backward_codegen_dense_cpuS5_S5_S5_S5_lS5_lS5_S5_lS5_dEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_lS5_lS5_S5_lS5_dEEEEE
 FN2at6TensorES0_S0_S0_S0_lS0_lS0_S0_lS0_dE
 split_embedding_codegen_grad_indice_weights_pt2_wrapper
 split_embedding_codegen_forward_weighted_pt2_wrapper
 split_embedding_codegen_forward_unweighted_pt2_wrapper
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_forward_split_pt2_cpu_wrapper.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_forward_split_pt2_cpu_wrapper.cpp
 fbgemm::split_embedding_codegen_grad_indice_weights_cpu
 fbgemm::split_embedding_codegen_forward_cpu
 FN2at6TensorES0_S0_S0_lS0_S0_S0_lS0_lE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_S7_S7_S7_S7_NS_6SymIntES7_S7_S7_S7_EXadL_Z59split_embedding_codegen_grad_indice_weights_pt2_cpu_wrapperS7_S7_S7_S7_S7_S7_S7_S7_S8_S7_S7_S7_S7_EEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_S7_S7_S7_S7_S8_S7_S7_S7_S7_EEEEE
 FN2at6TensorERKS0_S2_S2_S2_S2_S2_S2_S2_N3c106SymIntES2_S2_S2_S2_E
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_S7_S7_S7_NS_6SymIntES8_S7_S7_S7_lS7_S7_S7_blEXadL_Z56split_embedding_codegen_forward_weighted_pt2_cpu_wrapperS7_S7_S7_S7_S7_S7_S7_S8_S8_S7_S7_S7_lS7_S7_S7_blEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_S7_S7_S7_S8_S8_S7_S7_S7_lS7_S7_S7_blEEEEE
 FN2at6TensorERKS0_S2_S2_S2_S2_S2_S2_N3c106SymIntES4_S2_S2_S2_lS2_S2_S2_blE
@@ -17522,150 +17522,150 @@
 gradient_clipping
 max_gradient
 stochastic_rounding
 output_dtype
 learning_rate
 split_embedding_codegen_lookup_adagrad_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, float eps = 0, float learning_rate = 0, int output_dtype=0) -> Tensor
 split_embedding_codegen_lookup_adagrad_function_cpu
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_adagrad_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_adagrad_cpu.cpp
 fbgemm::split_embedding_backward_codegen_adagrad_cpu
 *N5torch8autograd7CppNodeIN12_GLOBAL__N_130SplitLookupFunction_adagrad_OpEEE
 *ZN5torch8autograd8FunctionIN12_GLOBAL__N_130SplitLookupFunction_adagrad_OpEE5applyIS3_JRN2at6TensorES8_S8_S8_RN3c106SymIntESB_S8_RlS8_S8_SC_RSt8optionalIS7_ESF_RbRdSG_S8_S8_S8_SH_SH_SC_EEENSt9enable_ifIX9is_same_vIT_S3_EEDTclsrSJ_7forwardLDnEspcl7declvalIT0_EEEEE4typeEDpOSK_EUlRKSt6vectorIS7_SaIS7_EESU_E_
 *ZN5torch8autograd8FunctionIN12_GLOBAL__N_130SplitLookupFunction_adagrad_OpEE5applyIS3_JRN2at6TensorES8_S8_S8_RN3c106SymIntESB_S8_RlS8_S8_SC_RSt8optionalIS7_ESF_RbRdSG_S8_S8_S8_SH_SH_SC_EEENSt9enable_ifIX9is_same_vIT_S3_EEDTclsrSJ_7forwardLDnEspcl7declvalIT0_EEEEE4typeEDpOSK_EUlRKS7_E0_
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_ddlEXadL_ZN12_GLOBAL__N_151split_embedding_codegen_lookup_adagrad_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_ddlEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_ddlEEEEE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN12_GLOBAL__N_130SplitLookupFunction_adagrad_OpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 FvN2at6TensorES0_S0_S0_S0_N3c106SymIntES0_lS0_S0_lS0_bS0_S0_S0_ddlE
 FvN2at6TensorES0_S0_S0_S0_lS0_lS0_S0_lS0_bS0_S0_S0_ddlE
 FN2at6TensorES0_S0_S0_S0_N3c106SymIntES2_S0_lS0_S0_lSt8optionalIS0_ES4_bdbS0_S0_S0_ddlE
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_adagrad_pt2_cpu_wrapper.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_adagrad_pt2_cpu_wrapper.cpp
 split_embedding_backward_codegen_adagrad_weighted_exact_pt2_wrapper
 split_embedding_backward_codegen_adagrad_unweighted_exact_pt2_wrapper
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_ddlEXadL_Z71split_embedding_backward_codegen_adagrad_weighted_exact_pt2_cpu_wrapperS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_ddlEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_ddlEEEEE
 FN2at6TensorERKS0_S2_S2_S2_S2_S2_S2_S2_lS2_lS2_S2_lS2_S2_llbllbbS0_S0_S0_S0_S0_ddlE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_ddlEXadL_Z73split_embedding_backward_codegen_adagrad_unweighted_exact_pt2_cpu_wrapperS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_ddlEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_ddlEEEEE
 weight_decay
 weight_decay_mode
 max_norm
 split_embedding_codegen_lookup_rowwise_adagrad_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, float eps = 0, float learning_rate = 0, float weight_decay = 0.0, int weight_decay_mode = 0, float max_norm = 0.0, int output_dtype=0) -> Tensor
 split_embedding_codegen_lookup_rowwise_adagrad_function_cpu
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_rowwise_adagrad_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_rowwise_adagrad_cpu.cpp
 fbgemm::split_embedding_backward_codegen_rowwise_adagrad_cpu
 *N5torch8autograd7CppNodeIN12_GLOBAL__N_138SplitLookupFunction_rowwise_adagrad_OpEEE
 *ZN5torch8autograd8FunctionIN12_GLOBAL__N_138SplitLookupFunction_rowwise_adagrad_OpEE5applyIS3_JRN2at6TensorES8_S8_S8_RN3c106SymIntESB_S8_RlS8_S8_SC_RSt8optionalIS7_ESF_RbRdSG_S8_S8_S8_SH_SH_SH_SC_SH_SC_EEENSt9enable_ifIX9is_same_vIT_S3_EEDTclsrSJ_7forwardLDnEspcl7declvalIT0_EEEEE4typeEDpOSK_EUlRKSt6vectorIS7_SaIS7_EESU_E_
 *ZN5torch8autograd8FunctionIN12_GLOBAL__N_138SplitLookupFunction_rowwise_adagrad_OpEE5applyIS3_JRN2at6TensorES8_S8_S8_RN3c106SymIntESB_S8_RlS8_S8_SC_RSt8optionalIS7_ESF_RbRdSG_S8_S8_S8_SH_SH_SH_SC_SH_SC_EEENSt9enable_ifIX9is_same_vIT_S3_EEDTclsrSJ_7forwardLDnEspcl7declvalIT0_EEEEE4typeEDpOSK_EUlRKS7_E0_
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_dddldlEXadL_ZN12_GLOBAL__N_159split_embedding_codegen_lookup_rowwise_adagrad_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddldlEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddldlEEEEE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN12_GLOBAL__N_138SplitLookupFunction_rowwise_adagrad_OpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 FvN2at6TensorES0_S0_S0_S0_N3c106SymIntES0_lS0_S0_lS0_bS0_S0_S0_dddldlE
 FvN2at6TensorES0_S0_S0_S0_lS0_lS0_S0_lS0_bS0_S0_S0_dddldlE
 FN2at6TensorES0_S0_S0_S0_N3c106SymIntES2_S0_lS0_S0_lSt8optionalIS0_ES4_bdbS0_S0_S0_dddldlE
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_rowwise_adagrad_pt2_cpu_wrapper.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_rowwise_adagrad_pt2_cpu_wrapper.cpp
 split_embedding_backward_codegen_rowwise_adagrad_weighted_exact_pt2_wrapper
 split_embedding_backward_codegen_rowwise_adagrad_unweighted_exact_pt2_wrapper
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_dddldlEXadL_Z79split_embedding_backward_codegen_rowwise_adagrad_weighted_exact_pt2_cpu_wrapperS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_dddldlEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_dddldlEEEEE
 FN2at6TensorERKS0_S2_S2_S2_S2_S2_S2_S2_lS2_lS2_S2_lS2_S2_llbllbbS0_S0_S0_S0_S0_dddldlE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_dddldlEXadL_Z81split_embedding_backward_codegen_rowwise_adagrad_unweighted_exact_pt2_cpu_wrapperS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_dddldlEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_dddldlEEEEE
 split_embedding_codegen_lookup_sgd_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, float learning_rate = 0, int output_dtype=0) -> Tensor
 split_embedding_codegen_lookup_sgd_function_cpu
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_sgd_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_sgd_cpu.cpp
 fbgemm::split_embedding_backward_codegen_sgd_cpu
 *N5torch8autograd7CppNodeIN12_GLOBAL__N_126SplitLookupFunction_sgd_OpEEE
 *ZN5torch8autograd8FunctionIN12_GLOBAL__N_126SplitLookupFunction_sgd_OpEE5applyIS3_JRN2at6TensorES8_S8_S8_RN3c106SymIntESB_S8_RlS8_S8_SC_RSt8optionalIS7_ESF_RbRdSG_SH_SC_EEENSt9enable_ifIX9is_same_vIT_S3_EEDTclsrSJ_7forwardLDnEspcl7declvalIT0_EEEEE4typeEDpOSK_EUlRKSt6vectorIS7_SaIS7_EESU_E_
 *ZN5torch8autograd8FunctionIN12_GLOBAL__N_126SplitLookupFunction_sgd_OpEE5applyIS3_JRN2at6TensorES8_S8_S8_RN3c106SymIntESB_S8_RlS8_S8_SC_RSt8optionalIS7_ESF_RbRdSG_SH_SC_EEENSt9enable_ifIX9is_same_vIT_S3_EEDTclsrSJ_7forwardLDnEspcl7declvalIT0_EEEEE4typeEDpOSK_EUlRKS7_E0_
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbdlEXadL_ZN12_GLOBAL__N_147split_embedding_codegen_lookup_sgd_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbdlEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbdlEEEEE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN12_GLOBAL__N_126SplitLookupFunction_sgd_OpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 FvN2at6TensorES0_S0_S0_S0_N3c106SymIntES0_lS0_S0_lS0_bdlE
 FvN2at6TensorES0_S0_S0_S0_lS0_lS0_S0_lS0_bdlE
 FN2at6TensorES0_S0_S0_S0_N3c106SymIntES2_S0_lS0_S0_lSt8optionalIS0_ES4_bdbdlE
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_sgd_pt2_cpu_wrapper.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_sgd_pt2_cpu_wrapper.cpp
 split_embedding_backward_codegen_sgd_weighted_exact_pt2_wrapper
 split_embedding_backward_codegen_sgd_unweighted_exact_pt2_wrapper
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbdlEXadL_Z67split_embedding_backward_codegen_sgd_weighted_exact_pt2_cpu_wrapperS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbdlEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbdlEEEEE
 FN2at6TensorERKS0_S2_S2_S2_S2_S2_S2_S2_lS2_lS2_S2_lS2_S2_llbllbbdlE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbdlEXadL_Z69split_embedding_backward_codegen_sgd_unweighted_exact_pt2_cpu_wrapperS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbdlEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbdlEEEEE
 split_embedding_codegen_lookup_adam_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_adam_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_adam_cpu.cpp
 split_embedding_codegen_lookup_adam_function_cpu
 split_embedding_codegen_lookup_adam_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, Tensor momentum2_host, Tensor momentum2_placements, Tensor momentum2_offsets, float learning_rate = 0, float eps = 0, float beta1 = 0, float beta2 = 0, float weight_decay = 0, int iter = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_S5_S5_S5_dddddllEXadL_ZN12_GLOBAL__N_148split_embedding_codegen_lookup_adam_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_dddddllEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_dddddllEEEEE
 FN2at6TensorES0_S0_S0_S0_N3c106SymIntES2_S0_lS0_S0_lSt8optionalIS0_ES4_bdbS0_S0_S0_S0_S0_S0_dddddllE
 split_embedding_codegen_lookup_lamb_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_lamb_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_lamb_cpu.cpp
 split_embedding_codegen_lookup_lamb_function_cpu
 split_embedding_codegen_lookup_lamb_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, Tensor momentum2_host, Tensor momentum2_placements, Tensor momentum2_offsets, float learning_rate = 0, float eps = 0, float beta1 = 0, float beta2 = 0, float weight_decay = 0, int iter = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_S5_S5_S5_dddddllEXadL_ZN12_GLOBAL__N_148split_embedding_codegen_lookup_lamb_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_dddddllEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_dddddllEEEEE
 split_embedding_codegen_lookup_partial_rowwise_adam_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_partial_rowwise_adam_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_partial_rowwise_adam_cpu.cpp
 split_embedding_codegen_lookup_partial_rowwise_adam_function_cpu
 split_embedding_codegen_lookup_partial_rowwise_adam_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, Tensor momentum2_host, Tensor momentum2_placements, Tensor momentum2_offsets, float learning_rate = 0, float eps = 0, float beta1 = 0, float beta2 = 0, float weight_decay = 0, int iter = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_S5_S5_S5_dddddllEXadL_ZN12_GLOBAL__N_164split_embedding_codegen_lookup_partial_rowwise_adam_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_dddddllEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_dddddllEEEEE
 split_embedding_codegen_lookup_partial_rowwise_lamb_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_partial_rowwise_lamb_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_partial_rowwise_lamb_cpu.cpp
 split_embedding_codegen_lookup_partial_rowwise_lamb_function_cpu
 split_embedding_codegen_lookup_partial_rowwise_lamb_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, Tensor momentum2_host, Tensor momentum2_placements, Tensor momentum2_offsets, float learning_rate = 0, float eps = 0, float beta1 = 0, float beta2 = 0, float weight_decay = 0, int iter = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_S5_S5_S5_dddddllEXadL_ZN12_GLOBAL__N_164split_embedding_codegen_lookup_partial_rowwise_lamb_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_dddddllEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_dddddllEEEEE
 split_embedding_codegen_lookup_lars_sgd_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_lars_sgd_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_lars_sgd_cpu.cpp
 split_embedding_codegen_lookup_lars_sgd_function_cpu
 split_embedding_codegen_lookup_lars_sgd_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, float learning_rate = 0, float eta = 0, float momentum = 0, float weight_decay = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_ddddlEXadL_ZN12_GLOBAL__N_152split_embedding_codegen_lookup_lars_sgd_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_ddddlEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_ddddlEEEEE
 FN2at6TensorES0_S0_S0_S0_N3c106SymIntES2_S0_lS0_S0_lSt8optionalIS0_ES4_bdbS0_S0_S0_ddddlE
 split_embedding_codegen_lookup_none_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_none_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_none_cpu.cpp
 split_embedding_codegen_lookup_none_function_cpu
 split_embedding_codegen_lookup_none_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, int total_hash_size = 0, SymInt total_unique_indices = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdblS6_lEXadL_ZN12_GLOBAL__N_148split_embedding_codegen_lookup_none_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdblS6_lEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdblS6_lEEEEE
 FN2at6TensorES0_S0_S0_S0_N3c106SymIntES2_S0_lS0_S0_lSt8optionalIS0_ES4_bdblS2_lE
 split_embedding_codegen_lookup_rowwise_adagrad_with_counter_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_rowwise_adagrad_with_counter_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_rowwise_adagrad_with_counter_cpu.cpp
 split_embedding_codegen_lookup_rowwise_adagrad_with_counter_function_cpu
 split_embedding_codegen_lookup_rowwise_adagrad_with_counter_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, Tensor prev_iter_host, Tensor prev_iter_placements, Tensor prev_iter_offsets, Tensor row_counter_host, Tensor row_counter_placements, Tensor row_counter_offsets, float eps = 0, float learning_rate = 0, float weight_decay = 0.0, int iter = 0, int counter_halflife = -1, int adjustment_iter = -1, float adjustment_ub = 1.0, int learning_rate_mode = -1, int weight_decay_mode = 1, int grad_sum_decay = -1, float max_counter = 0, float tail_id_threshold = 0.0, int is_tail_id_thresh_ratio = 0, int regularization_mode = 0, float weight_norm_coefficient = 0.0, float lower_bound = 0.0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_S5_S5_S5_S5_S5_S5_dddllldlllddllddlEXadL_ZN12_GLOBAL__N_172split_embedding_codegen_lookup_rowwise_adagrad_with_counter_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_S5_S5_S5_dddllldlllddllddlEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_S5_S5_S5_dddllldlllddllddlEEEEE
 FN2at6TensorES0_S0_S0_S0_N3c106SymIntES2_S0_lS0_S0_lSt8optionalIS0_ES4_bdbS0_S0_S0_S0_S0_S0_S0_S0_S0_dddllldlllddllddlE
 split_embedding_codegen_lookup_approx_sgd_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_approx_sgd_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_approx_sgd_cpu.cpp
 split_embedding_codegen_lookup_approx_sgd_function_cpu
 split_embedding_codegen_lookup_approx_sgd_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, float learning_rate = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbdlEXadL_ZN12_GLOBAL__N_154split_embedding_codegen_lookup_approx_sgd_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbdlEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbdlEEEEE
 split_embedding_codegen_lookup_approx_rowwise_adagrad_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_approx_rowwise_adagrad_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_approx_rowwise_adagrad_cpu.cpp
 split_embedding_codegen_lookup_approx_rowwise_adagrad_function_cpu
 split_embedding_codegen_lookup_approx_rowwise_adagrad_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, float eps = 0, float learning_rate = 0, float weight_decay = 0.0, int weight_decay_mode = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_dddllEXadL_ZN12_GLOBAL__N_166split_embedding_codegen_lookup_approx_rowwise_adagrad_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddllEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddllEEEEE
 FN2at6TensorES0_S0_S0_S0_N3c106SymIntES2_S0_lS0_S0_lSt8optionalIS0_ES4_bdbS0_S0_S0_dddllE
 split_embedding_codegen_lookup_approx_rowwise_adagrad_with_counter_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_approx_rowwise_adagrad_with_counter_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_approx_rowwise_adagrad_with_counter_cpu.cpp
 split_embedding_codegen_lookup_approx_rowwise_adagrad_with_counter_function_cpu
 split_embedding_codegen_lookup_approx_rowwise_adagrad_with_counter_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, Tensor prev_iter_host, Tensor prev_iter_placements, Tensor prev_iter_offsets, Tensor row_counter_host, Tensor row_counter_placements, Tensor row_counter_offsets, float eps = 0, float learning_rate = 0, float weight_decay = 0.0, int iter = 0, int counter_halflife = -1, int adjustment_iter = -1, float adjustment_ub = 1.0, int learning_rate_mode = -1, int weight_decay_mode = 1, int grad_sum_decay = -1, float max_counter = 0, float tail_id_threshold = 0.0, int is_tail_id_thresh_ratio = 0, int regularization_mode = 0, float weight_norm_coefficient = 0.0, float lower_bound = 0.0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_S5_S5_S5_S5_S5_S5_dddllldlllddllddlEXadL_ZN12_GLOBAL__N_179split_embedding_codegen_lookup_approx_rowwise_adagrad_with_counter_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_S5_S5_S5_dddllldlllddllddlEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_S5_S5_S5_dddllldlllddllddlEEEEE
 split_embedding_codegen_lookup_approx_rowwise_adagrad_with_weight_decay_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_approx_rowwise_adagrad_with_weight_decay_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_approx_rowwise_adagrad_with_weight_decay_cpu.cpp
 split_embedding_codegen_lookup_approx_rowwise_adagrad_with_weight_decay_function_cpu
 split_embedding_codegen_lookup_approx_rowwise_adagrad_with_weight_decay_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, float eps = 0, float learning_rate = 0, float weight_decay = 0.0, int weight_decay_mode = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_dddllEXadL_ZN12_GLOBAL__N_184split_embedding_codegen_lookup_approx_rowwise_adagrad_with_weight_decay_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddllEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddllEEEEE
 split_embedding_codegen_lookup_rowwise_adagrad_with_weight_decay_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_rowwise_adagrad_with_weight_decay_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_rowwise_adagrad_with_weight_decay_cpu.cpp
 split_embedding_codegen_lookup_rowwise_adagrad_with_weight_decay_function_cpu
 split_embedding_codegen_lookup_rowwise_adagrad_with_weight_decay_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, float eps = 0, float learning_rate = 0, float weight_decay = 0.0, int weight_decay_mode = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_dddllEXadL_ZN12_GLOBAL__N_177split_embedding_codegen_lookup_rowwise_adagrad_with_weight_decay_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddllEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddllEEEEE
 split_embedding_codegen_lookup_rowwise_weighted_adagrad_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_rowwise_weighted_adagrad_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_rowwise_weighted_adagrad_cpu.cpp
 split_embedding_codegen_lookup_rowwise_weighted_adagrad_function_cpu
 split_embedding_codegen_lookup_rowwise_weighted_adagrad_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, float eps = 0, float learning_rate = 0, float weight_decay = 0, int iter = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_dddllEXadL_ZN12_GLOBAL__N_168split_embedding_codegen_lookup_rowwise_weighted_adagrad_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddllEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddllEEEEE
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_adagrad_split_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_adagrad_split_cpu.cpp
 split_embedding_backward_exact_cpu_outer
 CPU exact rowwise adagrad currently doesn't support embedding tables with more than 2B rows
 split_embedding_backward_codegen_adagrad_cpu(Tensor grad_output, Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, int max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets,int pooling_mode, Tensor indice_weights, bool stochastic_rounding, Tensor(b!) momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, float eps = 0, float learning_rate = 0, int output_dtype = 0) -> ()
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFvN2at6TensorES5_S5_S5_S5_lS5_lS5_S5_lS5_bS5_S5_S5_ddlEXadL_Z44split_embedding_backward_codegen_adagrad_cpuS5_S5_S5_S5_S5_lS5_lS5_S5_lS5_bS5_S5_S5_ddlEEEEvNS_4guts8typelist8typelistIJS5_S5_S5_S5_S5_lS5_lS5_S5_lS5_bS5_S5_S5_ddlEEEEE
 does not match c_block size: 
 num of rows processed by adagrad: 
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_rowwise_adagrad_split_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_rowwise_adagrad_split_cpu.cpp
 split_embedding_backward_codegen_rowwise_adagrad_cpu(Tensor grad_output, Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, int max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets,int pooling_mode, Tensor indice_weights, bool stochastic_rounding, Tensor(b!) momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, float eps = 0, float learning_rate = 0, float weight_decay = 0.0, int weight_decay_mode = 0, float max_norm = 0.0, int output_dtype = 0) -> ()
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFvN2at6TensorES5_S5_S5_S5_lS5_lS5_S5_lS5_bS5_S5_S5_dddldlEXadL_Z52split_embedding_backward_codegen_rowwise_adagrad_cpuS5_S5_S5_S5_S5_lS5_lS5_S5_lS5_bS5_S5_S5_dddldlEEEEvNS_4guts8typelist8typelistIJS5_S5_S5_S5_S5_lS5_lS5_S5_lS5_bS5_S5_S5_dddldlEEEEE
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_sgd_split_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_sgd_split_cpu.cpp
 split_embedding_backward_codegen_sgd_cpu(Tensor grad_output, Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, int max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets,int pooling_mode, Tensor indice_weights, bool stochastic_rounding, float learning_rate = 0, int output_dtype = 0) -> ()
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFvN2at6TensorES5_S5_S5_S5_lS5_lS5_S5_lS5_bdlEXadL_Z40split_embedding_backward_codegen_sgd_cpuS5_S5_S5_S5_S5_lS5_lS5_S5_lS5_bdlEEEEvNS_4guts8typelist8typelistIJS5_S5_S5_S5_S5_lS5_lS5_S5_lS5_bdlEEEEE
 GCC: (conda-forge gcc 10.4.0-19) 10.4.0
 .shstrtab
 .gnu.hash
 .gnu.version
 .gnu.version_r
```

### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -10935,24 +10935,24 @@
   0x0098cb40 78747261 5f6d6574 615f2d3e 73796d62 xtra_meta_->symb
   0x0098cb50 6f6c6963 5f736861 70655f6d 6574615f olic_shape_meta_
   0x0098cb60 20494e54 45524e41 4c204153 53455254  INTERNAL ASSERT
   0x0098cb70 20464149 4c454420 61742022 2f676974  FAILED at "/git
   0x0098cb80 6875622f 686f6d65 2f6d696e 69636f6e hub/home/minicon
   0x0098cb90 64612f65 6e76732f 6275696c 645f6269 da/envs/build_bi
   0x0098cba0 6e617279 2f6c6962 2f707974 686f6e33 nary/lib/python3
-  0x0098cbb0 2e392f73 6974652d 7061636b 61676573 .9/site-packages
+  0x0098cbb0 2e382f73 6974652d 7061636b 61676573 .8/site-packages
   0x0098cbc0 2f746f72 63682f69 6e636c75 64652f63 /torch/include/c
   0x0098cbd0 31302f63 6f72652f 54656e73 6f72496d 10/core/TensorIm
   0x0098cbe0 706c2e68 223a3137 32332c20 706c6561 pl.h":1723, plea
   0x0098cbf0 73652072 65706f72 74206120 62756720 se report a bug 
   0x0098cc00 746f2050 79546f72 63682e20 00000000 to PyTorch. ....
   0x0098cc10 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x0098cc20 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x0098cc30 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x0098cc40 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x0098cc40 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x0098cc50 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x0098cc60 64652f63 31302f63 6f72652f 54656e73 de/c10/core/Tens
   0x0098cc70 6f72496d 706c2e68 00000000 00000000 orImpl.h........
   0x0098cc80 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x0098cc90 4d4d2f66 6267656d 6d5f6770 752f636f MM/fbgemm_gpu/co
   0x0098cca0 64656765 6e2f7472 61696e69 6e672f66 degen/training/f
   0x0098ccb0 6f727761 72642f65 6d626564 64696e67 orward/embedding
@@ -11027,15 +11027,15 @@
   0x0098d100 206c6179 6f757420 63616c63 756c6174  layout calculat
   0x0098d110 696f6e20 6c6f6769 632e0000 00000000 ion logic.......
   0x0098d120 69735f6d 6b6c646e 6e282920 494e5445 is_mkldnn() INTE
   0x0098d130 524e414c 20415353 45525420 4641494c RNAL ASSERT FAIL
   0x0098d140 45442061 7420222f 67697468 75622f68 ED at "/github/h
   0x0098d150 6f6d652f 6d696e69 636f6e64 612f656e ome/miniconda/en
   0x0098d160 76732f62 75696c64 5f62696e 6172792f vs/build_binary/
-  0x0098d170 6c69622f 70797468 6f6e332e 392f7369 lib/python3.9/si
+  0x0098d170 6c69622f 70797468 6f6e332e 382f7369 lib/python3.8/si
   0x0098d180 74652d70 61636b61 6765732f 746f7263 te-packages/torc
   0x0098d190 682f696e 636c7564 652f6331 302f636f h/include/c10/co
   0x0098d1a0 72652f54 656e736f 72496d70 6c2e6822 re/TensorImpl.h"
   0x0098d1b0 3a313239 302c2070 6c656173 65207265 :1290, please re
   0x0098d1c0 706f7274 20612062 75672074 6f205079 port a bug to Py
   0x0098d1d0 546f7263 682e2000 4f706572 61746f72 Torch. .Operator
   0x0098d1e0 73207461 6b696e67 2054656e 736f724f s taking TensorO
@@ -11044,15 +11044,15 @@
   0x0098d210 6e732077 69746820 6f707469 6f6e732e ns with options.
   0x0098d220 72657175 69726573 5f677261 64207365 requires_grad se
   0x0098d230 74206173 20747275 652e2054 68697320 t as true. This 
   0x0098d240 69736e27 7420696d 706c656d 656e7465 isn't implemente
   0x0098d250 64207965 742e0000 2f676974 6875622f d yet.../github/
   0x0098d260 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x0098d270 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x0098d280 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x0098d280 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x0098d290 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x0098d2a0 63682f69 6e636c75 64652f41 54656e2f ch/include/ATen/
   0x0098d2b0 636f7265 2f436865 636b4d65 6d6f7279 core/CheckMemory
   0x0098d2c0 466f726d 61742e68 00000000 00000000 Format.h........
   0x0098d2d0 63686563 6b5f7465 6e736f72 5f6f7074 check_tensor_opt
   0x0098d2e0 696f6e73 5f616e64 5f657874 72616374 ions_and_extract
   0x0098d2f0 5f6d656d 6f72795f 666f726d 61740000 _memory_format..
@@ -11070,51 +11070,51 @@
   0x0098d3b0 496e7441 72726179 52656620 636f6e74 IntArrayRef cont
   0x0098d3c0 61696e73 20616e20 696e7420 74686174 ains an int that
   0x0098d3d0 2063616e 6e6f7420 62652072 65707265  cannot be repre
   0x0098d3e0 73656e74 65642061 73206120 53796d49 sented as a SymI
   0x0098d3f0 6e743a20 00000000 2f676974 6875622f nt: ..../github/
   0x0098d400 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x0098d410 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x0098d420 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x0098d420 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x0098d430 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x0098d440 63682f69 6e636c75 64652f63 31302f63 ch/include/c10/c
   0x0098d450 6f72652f 53796d49 6e744172 72617952 ore/SymIntArrayR
   0x0098d460 65662e68 0066726f 6d496e74 41727261 ef.h.fromIntArra
   0x0098d470 79526566 536c6f77 00206469 6d732062 yRefSlow. dims b
   0x0098d480 75742074 656e736f 72206861 73200054 ut tensor has .T
   0x0098d490 656e736f 72416363 6573736f 72206578 ensorAccessor ex
   0x0098d4a0 70656374 65642000 61636365 73736f72 pected .accessor
   0x0098d4b0 00000000 00000000 2f676974 6875622f ......../github/
   0x0098d4c0 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x0098d4d0 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x0098d4e0 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x0098d4e0 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x0098d4f0 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x0098d500 63682f69 6e636c75 64652f41 54656e2f ch/include/ATen/
   0x0098d510 636f7265 2f54656e 736f7242 6173652e core/TensorBase.
   0x0098d520 68002d31 00496e64 65782000 20697320 h.-1.Index . is 
   0x0098d530 6f757420 6f662062 6f756e64 733a2000 out of bounds: .
   0x0098d540 2c207261 6e676520 0020746f 20007265 , range . to .re
   0x0098d550 706f7274 5f656d62 65646469 6e675f65 port_embedding_e
   0x0098d560 72726f72 00000000 2f5f5f77 2f464247 rror..../__w/FBG
   0x0098d570 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x0098d580 6d5f6770 752f696e 636c7564 652f6662 m_gpu/include/fb
   0x0098d590 67656d6d 5f677075 2f637075 5f757469 gemm_gpu/cpu_uti
   0x0098d5a0 6c732e68 00000000 2f676974 6875622f ls.h..../github/
   0x0098d5b0 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x0098d5c0 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x0098d5d0 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x0098d5d0 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x0098d5e0 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x0098d5f0 63682f69 6e636c75 64652f41 54656e2f ch/include/ATen/
   0x0098d600 636f7265 2f697661 6c75652e 68000000 core/ivalue.h...
   0x0098d610 3020494e 5445524e 414c2041 53534552 0 INTERNAL ASSER
   0x0098d620 54204641 494c4544 20617420 222f6769 T FAILED at "/gi
   0x0098d630 74687562 2f686f6d 652f6d69 6e69636f thub/home/minico
   0x0098d640 6e64612f 656e7673 2f627569 6c645f62 nda/envs/build_b
   0x0098d650 696e6172 792f6c69 622f7079 74686f6e inary/lib/python
-  0x0098d660 332e392f 73697465 2d706163 6b616765 3.9/site-package
+  0x0098d660 332e382f 73697465 2d706163 6b616765 3.8/site-package
   0x0098d670 732f746f 7263682f 696e636c 7564652f s/torch/include/
   0x0098d680 4154656e 2f636f72 652f6976 616c7565 ATen/core/ivalue
   0x0098d690 2e68223a 3635322c 20706c65 61736520 .h":652, please 
   0x0098d6a0 7265706f 72742061 20627567 20746f20 report a bug to 
   0x0098d6b0 5079546f 7263682e 20006578 70656374 PyTorch. .expect
   0x0098d6c0 65642069 6e740074 6f496e74 00766563 ed int.toInt.vec
   0x0098d6d0 746f723a 3a5f4d5f 7265616c 6c6f635f tor::_M_realloc_
@@ -11122,25 +11122,25 @@
   0x0098d6f0 2053796d 496e7420 6f722069 6e742062  SymInt or int b
   0x0098d700 75742067 6f742000 69735379 6d496e74 ut got .isSymInt
   0x0098d710 2829207c 7c206973 496e7428 2920494e () || isInt() IN
   0x0098d720 5445524e 414c2041 53534552 54204641 TERNAL ASSERT FA
   0x0098d730 494c4544 20617420 222f6769 74687562 ILED at "/github
   0x0098d740 2f686f6d 652f6d69 6e69636f 6e64612f /home/miniconda/
   0x0098d750 656e7673 2f627569 6c645f62 696e6172 envs/build_binar
-  0x0098d760 792f6c69 622f7079 74686f6e 332e392f y/lib/python3.9/
+  0x0098d760 792f6c69 622f7079 74686f6e 332e382f y/lib/python3.8/
   0x0098d770 73697465 2d706163 6b616765 732f746f site-packages/to
   0x0098d780 7263682f 696e636c 7564652f 4154656e rch/include/ATen
   0x0098d790 2f636f72 652f6976 616c7565 5f696e6c /core/ivalue_inl
   0x0098d7a0 2e68223a 3233372c 20706c65 61736520 .h":237, please 
   0x0098d7b0 7265706f 72742061 20627567 20746f20 report a bug to 
   0x0098d7c0 5079546f 7263682e 20000000 00000000 PyTorch. .......
   0x0098d7d0 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x0098d7e0 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x0098d7f0 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x0098d800 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x0098d800 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x0098d810 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x0098d820 64652f41 54656e2f 636f7265 2f697661 de/ATen/core/iva
   0x0098d830 6c75655f 696e6c2e 6800746f 53796d49 lue_inl.h.toSymI
   0x0098d840 6e740000 00000000 00000000 00000000 nt..............
   0x0098d850 53743139 6261645f 6f707469 6f6e616c St19bad_optional
   0x0098d860 5f616363 65737300 00000000 00000000 _access.........
   0x0098d870 4e336331 30323069 6e747275 73697665 N3c1020intrusive
@@ -11273,28 +11273,28 @@
   0x0098e060 6e642000 20646576 69636573 00676574 nd . devices.get
   0x0098e070 44657669 63654775 61726449 6d706c00 DeviceGuardImpl.
   0x0098e080 5079546f 72636820 6973206e 6f74206c PyTorch is not l
   0x0098e090 696e6b65 64207769 74682073 7570706f inked with suppo
   0x0098e0a0 72742066 6f722000 2f676974 6875622f rt for ./github/
   0x0098e0b0 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x0098e0c0 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x0098e0d0 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x0098e0d0 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x0098e0e0 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x0098e0f0 63682f69 6e636c75 64652f63 31302f63 ch/include/c10/c
   0x0098e100 6f72652f 696d706c 2f446576 69636547 ore/impl/DeviceG
   0x0098e110 75617264 496d706c 496e7465 72666163 uardImplInterfac
   0x0098e120 652e6800 4576656e 74206465 76696365 e.h.Event device
   0x0098e130 20747970 65200062 6c6f636b 00000000  type .block....
   0x0098e140 20646f65 73206e6f 74206d61 74636820  does not match 
   0x0098e150 626c6f63 6b696e67 20737472 65616d27 blocking stream'
   0x0098e160 73206465 76696365 20747970 65200000 s device type ..
   0x0098e170 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x0098e180 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x0098e190 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x0098e1a0 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x0098e1a0 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x0098e1b0 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x0098e1c0 64652f63 31302f63 6f72652f 696d706c de/c10/core/impl
   0x0098e1d0 2f496e6c 696e6545 76656e74 2e680000 /InlineEvent.h..
   0x0098e1e0 45787065 63746564 20216e61 6d652e65 Expected !name.e
   0x0098e1f0 6d707479 28292074 6f206265 20747275 mpty() to be tru
   0x0098e200 652c2062 75742067 6f742066 616c7365 e, but got false
   0x0098e210 2e202028 436f756c 64207468 69732065 .  (Could this e
@@ -11302,49 +11302,49 @@
   0x0098e230 696d7072 6f766564 3f202049 6620736f improved?  If so
   0x0098e240 2c20706c 65617365 20726570 6f727420 , please report 
   0x0098e250 616e2065 6e68616e 63656d65 6e742072 an enhancement r
   0x0098e260 65717565 73742074 6f205079 546f7263 equest to PyTorc
   0x0098e270 682e2900 00000000 2f676974 6875622f h.)...../github/
   0x0098e280 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x0098e290 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x0098e2a0 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x0098e2a0 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x0098e2b0 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x0098e2c0 63682f69 6e636c75 64652f41 54656e2f ch/include/ATen/
   0x0098e2d0 636f7265 2f717561 6c696669 65645f6e core/qualified_n
   0x0098e2e0 616d652e 68000000 496e7661 6c696420 ame.h...Invalid 
   0x0098e2f0 6e616d65 20666f72 20717561 6c696669 name for qualifi
   0x0098e300 6564206e 616d653a 20270000 00000000 ed name: '......
   0x0098e310 2161746f 6d2e656d 70747928 2920494e !atom.empty() IN
   0x0098e320 5445524e 414c2041 53534552 54204641 TERNAL ASSERT FA
   0x0098e330 494c4544 20617420 222f6769 74687562 ILED at "/github
   0x0098e340 2f686f6d 652f6d69 6e69636f 6e64612f /home/miniconda/
   0x0098e350 656e7673 2f627569 6c645f62 696e6172 envs/build_binar
-  0x0098e360 792f6c69 622f7079 74686f6e 332e392f y/lib/python3.9/
+  0x0098e360 792f6c69 622f7079 74686f6e 332e382f y/lib/python3.8/
   0x0098e370 73697465 2d706163 6b616765 732f746f site-packages/to
   0x0098e380 7263682f 696e636c 7564652f 4154656e rch/include/ATen
   0x0098e390 2f636f72 652f7175 616c6966 6965645f /core/qualified_
   0x0098e3a0 6e616d65 2e68223a 32342c20 706c6561 name.h":24, plea
   0x0098e3b0 73652072 65706f72 74206120 62756720 se report a bug 
   0x0098e3c0 746f2050 79546f72 63682e20 00000000 to PyTorch. ....
   0x0098e3d0 2166696e 616c4174 6f6d2e65 6d707479 !finalAtom.empty
   0x0098e3e0 28292049 4e544552 4e414c20 41535345 () INTERNAL ASSE
   0x0098e3f0 52542046 41494c45 44206174 20222f67 RT FAILED at "/g
   0x0098e400 69746875 622f686f 6d652f6d 696e6963 ithub/home/minic
   0x0098e410 6f6e6461 2f656e76 732f6275 696c645f onda/envs/build_
   0x0098e420 62696e61 72792f6c 69622f70 7974686f binary/lib/pytho
-  0x0098e430 6e332e39 2f736974 652d7061 636b6167 n3.9/site-packag
+  0x0098e430 6e332e38 2f736974 652d7061 636b6167 n3.8/site-packag
   0x0098e440 65732f74 6f726368 2f696e63 6c756465 es/torch/include
   0x0098e450 2f415465 6e2f636f 72652f71 75616c69 /ATen/core/quali
   0x0098e460 66696564 5f6e616d 652e6822 3a33322c fied_name.h":32,
   0x0098e470 20706c65 61736520 7265706f 72742061  please report a
   0x0098e480 20627567 20746f20 5079546f 7263682e  bug to PyTorch.
   0x0098e490 20000000 00000000 2f676974 6875622f  ......./github/
   0x0098e4a0 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x0098e4b0 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x0098e4c0 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x0098e4c0 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x0098e4d0 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x0098e4e0 63682f69 6e636c75 64652f63 31302f75 ch/include/c10/u
   0x0098e4f0 74696c2f 41727261 79526566 2e680051 til/ArrayRef.h.Q
   0x0098e500 75616c69 66696564 4e616d65 00626173 ualifiedName.bas
   0x0098e510 69635f73 7472696e 673a3a73 75627374 ic_string::subst
   0x0098e520 72004172 72617952 65663a20 696e7661 r.ArrayRef: inva
   0x0098e530 6c696420 736c6963 652c204e 203d2000 lid slice, N = .
@@ -11355,27 +11355,27 @@
   0x0098e580 77697468 2064696d 656e7369 6f6e733a with dimensions:
   0x0098e590 20000000 00000000 74656e73 6f722e64  .......tensor.d
   0x0098e5a0 696d2829 203d3d20 3020494e 5445524e im() == 0 INTERN
   0x0098e5b0 414c2041 53534552 54204641 494c4544 AL ASSERT FAILED
   0x0098e5c0 20617420 222f6769 74687562 2f686f6d  at "/github/hom
   0x0098e5d0 652f6d69 6e69636f 6e64612f 656e7673 e/miniconda/envs
   0x0098e5e0 2f627569 6c645f62 696e6172 792f6c69 /build_binary/li
-  0x0098e5f0 622f7079 74686f6e 332e392f 73697465 b/python3.9/site
+  0x0098e5f0 622f7079 74686f6e 332e382f 73697465 b/python3.8/site
   0x0098e600 2d706163 6b616765 732f746f 7263682f -packages/torch/
   0x0098e610 696e636c 7564652f 746f7263 682f6373 include/torch/cs
   0x0098e620 72632f61 70692f69 6e636c75 64652f74 rc/api/include/t
   0x0098e630 6f726368 2f646574 61696c2f 54656e73 orch/detail/Tens
   0x0098e640 6f724461 7461436f 6e746169 6e65722e orDataContainer.
   0x0098e650 68223a33 31372c20 706c6561 73652072 h":317, please r
   0x0098e660 65706f72 74206120 62756720 746f2050 eport a bug to P
   0x0098e670 79546f72 63682e20 00000000 00000000 yTorch. ........
   0x0098e680 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x0098e690 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x0098e6a0 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x0098e6b0 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x0098e6b0 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x0098e6c0 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x0098e6d0 64652f74 6f726368 2f637372 632f6170 de/torch/csrc/ap
   0x0098e6e0 692f696e 636c7564 652f746f 7263682f i/include/torch/
   0x0098e6f0 64657461 696c2f54 656e736f 72446174 detail/TensorDat
   0x0098e700 61436f6e 7461696e 65722e68 00000000 aContainer.h....
   0x0098e710 20696e20 69747320 66697273 74206469  in its first di
   0x0098e720 6d656e73 696f6e2c 20627574 20676f74 mension, but got
@@ -11384,15 +11384,15 @@
   0x0098e750 697a6573 28295b30 5d203d3d 2028696e izes()[0] == (in
   0x0098e760 7436345f 7429696e 69745f6c 6973745f t64_t)init_list_
   0x0098e770 2e73697a 65282920 494e5445 524e414c .size() INTERNAL
   0x0098e780 20415353 45525420 4641494c 45442061  ASSERT FAILED a
   0x0098e790 7420222f 67697468 75622f68 6f6d652f t "/github/home/
   0x0098e7a0 6d696e69 636f6e64 612f656e 76732f62 miniconda/envs/b
   0x0098e7b0 75696c64 5f62696e 6172792f 6c69622f uild_binary/lib/
-  0x0098e7c0 70797468 6f6e332e 392f7369 74652d70 python3.9/site-p
+  0x0098e7c0 70797468 6f6e332e 382f7369 74652d70 python3.8/site-p
   0x0098e7d0 61636b61 6765732f 746f7263 682f696e ackages/torch/in
   0x0098e7e0 636c7564 652f746f 7263682f 63737263 clude/torch/csrc
   0x0098e7f0 2f617069 2f696e63 6c756465 2f746f72 /api/include/tor
   0x0098e800 63682f64 65746169 6c2f5465 6e736f72 ch/detail/Tensor
   0x0098e810 44617461 436f6e74 61696e65 722e6822 DataContainer.h"
   0x0098e820 3a333234 2c20706c 65617365 20726570 :324, please rep
   0x0098e830 6f727420 61206275 6720746f 20507954 ort a bug to PyT
@@ -11403,15 +11403,15 @@
   0x0098e880 6f726020 73686f75 6c64206e 6f742062 or` should not b
   0x0098e890 65206361 6c6c6564 00000000 00000000 e called........
   0x0098e8a0 66616c73 6520494e 5445524e 414c2041 false INTERNAL A
   0x0098e8b0 53534552 54204641 494c4544 20617420 SSERT FAILED at 
   0x0098e8c0 222f6769 74687562 2f686f6d 652f6d69 "/github/home/mi
   0x0098e8d0 6e69636f 6e64612f 656e7673 2f627569 niconda/envs/bui
   0x0098e8e0 6c645f62 696e6172 792f6c69 622f7079 ld_binary/lib/py
-  0x0098e8f0 74686f6e 332e392f 73697465 2d706163 thon3.9/site-pac
+  0x0098e8f0 74686f6e 332e382f 73697465 2d706163 thon3.8/site-pac
   0x0098e900 6b616765 732f746f 7263682f 696e636c kages/torch/incl
   0x0098e910 7564652f 746f7263 682f6373 72632f61 ude/torch/csrc/a
   0x0098e920 70692f69 6e636c75 64652f74 6f726368 pi/include/torch
   0x0098e930 2f646574 61696c2f 54656e73 6f724461 /detail/TensorDa
   0x0098e940 7461436f 6e746169 6e65722e 68223a33 taContainer.h":3
   0x0098e950 33382c20 706c6561 73652072 65706f72 38, please repor
   0x0098e960 74206120 62756720 746f2050 79546f72 t a bug to PyTor
@@ -11419,15 +11419,15 @@
   0x0098e980 54656e73 6f724461 7461436f 6e746169 TensorDataContai
   0x0098e990 6e657220 74797065 00000000 00000000 ner type........
   0x0098e9a0 66616c73 6520494e 5445524e 414c2041 false INTERNAL A
   0x0098e9b0 53534552 54204641 494c4544 20617420 SSERT FAILED at 
   0x0098e9c0 222f6769 74687562 2f686f6d 652f6d69 "/github/home/mi
   0x0098e9d0 6e69636f 6e64612f 656e7673 2f627569 niconda/envs/bui
   0x0098e9e0 6c645f62 696e6172 792f6c69 622f7079 ld_binary/lib/py
-  0x0098e9f0 74686f6e 332e392f 73697465 2d706163 thon3.9/site-pac
+  0x0098e9f0 74686f6e 332e382f 73697465 2d706163 thon3.8/site-pac
   0x0098ea00 6b616765 732f746f 7263682f 696e636c kages/torch/incl
   0x0098ea10 7564652f 746f7263 682f6373 72632f61 ude/torch/csrc/a
   0x0098ea20 70692f69 6e636c75 64652f74 6f726368 pi/include/torch
   0x0098ea30 2f646574 61696c2f 54656e73 6f724461 /detail/TensorDa
   0x0098ea40 7461436f 6e746169 6e65722e 68223a33 taContainer.h":3
   0x0098ea50 34322c20 706c6561 73652072 65706f72 42, please repor
   0x0098ea60 74206120 62756720 746f2050 79546f72 t a bug to PyTor
@@ -11445,15 +11445,15 @@
   0x0098eb20 74686f75 74206c6f 7373206f 6620696e thout loss of in
   0x0098eb30 666f726d 6174696f 6e000000 00000000 formation.......
   0x0098eb40 66616c73 6520494e 5445524e 414c2041 false INTERNAL A
   0x0098eb50 53534552 54204641 494c4544 20617420 SSERT FAILED at 
   0x0098eb60 222f6769 74687562 2f686f6d 652f6d69 "/github/home/mi
   0x0098eb70 6e69636f 6e64612f 656e7673 2f627569 niconda/envs/bui
   0x0098eb80 6c645f62 696e6172 792f6c69 622f7079 ld_binary/lib/py
-  0x0098eb90 74686f6e 332e392f 73697465 2d706163 thon3.9/site-pac
+  0x0098eb90 74686f6e 332e382f 73697465 2d706163 thon3.8/site-pac
   0x0098eba0 6b616765 732f746f 7263682f 696e636c kages/torch/incl
   0x0098ebb0 7564652f 746f7263 682f6373 72632f61 ude/torch/csrc/a
   0x0098ebc0 70692f69 6e636c75 64652f74 6f726368 pi/include/torch
   0x0098ebd0 2f646574 61696c2f 54656e73 6f724461 /detail/TensorDa
   0x0098ebe0 7461436f 6e746169 6e65722e 68223a32 taContainer.h":2
   0x0098ebf0 37322c20 706c6561 73652072 65706f72 72, please repor
   0x0098ec00 74206120 62756720 746f2050 79546f72 t a bug to PyTor
@@ -11473,15 +11473,15 @@
   0x0098ece0 3b206974 20697320 6f6e6c79 20666f72 ; it is only for
   0x0098ecf0 20475055 2e000000 6973496e 744c6973  GPU....isIntLis
   0x0098ed00 74282920 494e5445 524e414c 20415353 t() INTERNAL ASS
   0x0098ed10 45525420 4641494c 45442061 7420222f ERT FAILED at "/
   0x0098ed20 67697468 75622f68 6f6d652f 6d696e69 github/home/mini
   0x0098ed30 636f6e64 612f656e 76732f62 75696c64 conda/envs/build
   0x0098ed40 5f62696e 6172792f 6c69622f 70797468 _binary/lib/pyth
-  0x0098ed50 6f6e332e 392f7369 74652d70 61636b61 on3.9/site-packa
+  0x0098ed50 6f6e332e 382f7369 74652d70 61636b61 on3.8/site-packa
   0x0098ed60 6765732f 746f7263 682f696e 636c7564 ges/torch/includ
   0x0098ed70 652f4154 656e2f63 6f72652f 6976616c e/ATen/core/ival
   0x0098ed80 75655f69 6e6c2e68 223a3139 36362c20 ue_inl.h":1966, 
   0x0098ed90 706c6561 73652072 65706f72 74206120 please report a 
   0x0098eda0 62756720 746f2050 79546f72 63682e20 bug to PyTorch. 
   0x0098edb0 00000000 00000000 76656374 6f723a3a ........vector::
   0x0098edc0 5f4d5f72 616e6765 5f636865 636b3a20 _M_range_check: 
@@ -11508,15 +11508,15 @@
   0x0098ef10 61726775 6d656e74 206f6620 5f5f7365 argument of __se
   0x0098ef20 74737461 74655f5f 2e20476f 74200000 tstate__. Got ..
   0x0098ef30 69735374 72696e67 28292049 4e544552 isString() INTER
   0x0098ef40 4e414c20 41535345 52542046 41494c45 NAL ASSERT FAILE
   0x0098ef50 44206174 20222f67 69746875 622f686f D at "/github/ho
   0x0098ef60 6d652f6d 696e6963 6f6e6461 2f656e76 me/miniconda/env
   0x0098ef70 732f6275 696c645f 62696e61 72792f6c s/build_binary/l
-  0x0098ef80 69622f70 7974686f 6e332e39 2f736974 ib/python3.9/sit
+  0x0098ef80 69622f70 7974686f 6e332e38 2f736974 ib/python3.8/sit
   0x0098ef90 652d7061 636b6167 65732f74 6f726368 e-packages/torch
   0x0098efa0 2f696e63 6c756465 2f415465 6e2f636f /include/ATen/co
   0x0098efb0 72652f69 76616c75 655f696e 6c2e6822 re/ivalue_inl.h"
   0x0098efc0 3a323335 352c2070 6c656173 65207265 :2355, please re
   0x0098efd0 706f7274 20612062 75672074 6f205079 port a bug to Py
   0x0098efe0 546f7263 682e2000 2f2f6465 65706c65 Torch. .//deeple
   0x0098eff0 61726e69 6e672f66 6267656d 6d2f6662 arning/fbgemm/fb
@@ -11634,36 +11634,36 @@
   0x0098f6f0 73657473 29202d3e 2054656e 736f7200 sets) -> Tensor.
   0x0098f700 69734765 6e657269 63446963 74282920 isGenericDict() 
   0x0098f710 494e5445 524e414c 20415353 45525420 INTERNAL ASSERT 
   0x0098f720 4641494c 45442061 7420222f 67697468 FAILED at "/gith
   0x0098f730 75622f68 6f6d652f 6d696e69 636f6e64 ub/home/minicond
   0x0098f740 612f656e 76732f62 75696c64 5f62696e a/envs/build_bin
   0x0098f750 6172792f 6c69622f 70797468 6f6e332e ary/lib/python3.
-  0x0098f760 392f7369 74652d70 61636b61 6765732f 9/site-packages/
+  0x0098f760 382f7369 74652d70 61636b61 6765732f 8/site-packages/
   0x0098f770 746f7263 682f696e 636c7564 652f4154 torch/include/AT
   0x0098f780 656e2f63 6f72652f 6976616c 75655f69 en/core/ivalue_i
   0x0098f790 6e6c2e68 223a3230 38322c20 706c6561 nl.h":2082, plea
   0x0098f7a0 73652072 65706f72 74206120 62756720 se report a bug 
   0x0098f7b0 746f2050 79546f72 63682e20 00000000 to PyTorch. ....
   0x0098f7c0 73656c66 5f696d70 6c20494e 5445524e self_impl INTERN
   0x0098f7d0 414c2041 53534552 54204641 494c4544 AL ASSERT FAILED
   0x0098f7e0 20617420 222f6769 74687562 2f686f6d  at "/github/hom
   0x0098f7f0 652f6d69 6e69636f 6e64612f 656e7673 e/miniconda/envs
   0x0098f800 2f627569 6c645f62 696e6172 792f6c69 /build_binary/li
-  0x0098f810 622f7079 74686f6e 332e392f 73697465 b/python3.9/site
+  0x0098f810 622f7079 74686f6e 332e382f 73697465 b/python3.8/site
   0x0098f820 2d706163 6b616765 732f746f 7263682f -packages/torch/
   0x0098f830 696e636c 7564652f 746f7263 682f6373 include/torch/cs
   0x0098f840 72632f61 75746f67 7261642f 76617269 rc/autograd/vari
   0x0098f850 61626c65 2e68223a 3330352c 20706c65 able.h":305, ple
   0x0098f860 61736520 7265706f 72742061 20627567 ase report a bug
   0x0098f870 20746f20 5079546f 7263682e 20000000  to PyTorch. ...
   0x0098f880 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x0098f890 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x0098f8a0 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x0098f8b0 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x0098f8b0 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x0098f8c0 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x0098f8d0 64652f74 6f726368 2f637372 632f6175 de/torch/csrc/au
   0x0098f8e0 746f6772 61642f76 61726961 626c652e tograd/variable.
   0x0098f8f0 68000000 00000000 4f6e6c79 2054656e h.......Only Ten
   0x0098f900 736f7273 206f6620 666c6f61 74696e67 sors of floating
   0x0098f910 20706f69 6e742061 6e642063 6f6d706c  point and compl
   0x0098f920 65782064 74797065 2063616e 20726571 ex dtype can req
@@ -11723,37 +11723,37 @@
   0x0098fc80 73657274 00000000 73636865 6d615f2e sert....schema_.
   0x0098fc90 72657475 726e7328 292e7369 7a652829 returns().size()
   0x0098fca0 203d3d20 3120494e 5445524e 414c2041  == 1 INTERNAL A
   0x0098fcb0 53534552 54204641 494c4544 20617420 SSERT FAILED at 
   0x0098fcc0 222f6769 74687562 2f686f6d 652f6d69 "/github/home/mi
   0x0098fcd0 6e69636f 6e64612f 656e7673 2f627569 niconda/envs/bui
   0x0098fce0 6c645f62 696e6172 792f6c69 622f7079 ld_binary/lib/py
-  0x0098fcf0 74686f6e 332e392f 73697465 2d706163 thon3.9/site-pac
+  0x0098fcf0 74686f6e 332e382f 73697465 2d706163 thon3.8/site-pac
   0x0098fd00 6b616765 732f746f 7263682f 696e636c kages/torch/incl
   0x0098fd10 7564652f 4154656e 2f636f72 652f6275 ude/ATen/core/bu
   0x0098fd20 696c7469 6e5f6675 6e637469 6f6e2e68 iltin_function.h
   0x0098fd30 223a3232 2c20706c 65617365 20726570 ":22, please rep
   0x0098fd40 6f727420 61206275 6720746f 20507954 ort a bug to PyT
   0x0098fd50 6f726368 2e200000 2f676974 6875622f orch. ../github/
   0x0098fd60 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x0098fd70 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x0098fd80 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x0098fd80 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x0098fd90 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x0098fda0 63682f69 6e636c75 64652f41 54656e2f ch/include/ATen/
   0x0098fdb0 636f7265 2f627569 6c74696e 5f66756e core/builtin_fun
   0x0098fdc0 6374696f 6e2e6800 4275696c 74696e4f ction.h.BuiltinO
   0x0098fdd0 7046756e 6374696f 6e006465 66696e65 pFunction.define
   0x0098fde0 4d657468 6f640000 44656661 756c7420 Method..Default 
   0x0098fdf0 76616c75 6573206d 75737420 62652073 values must be s
   0x0098fe00 70656369 66696564 20666f72 206e6f6e pecified for non
   0x0098fe10 65206f72 20616c6c 20617267 756d656e e or all argumen
   0x0098fe20 74730000 00000000 2f676974 6875622f ts....../github/
   0x0098fe30 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x0098fe40 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x0098fe50 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x0098fe50 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x0098fe60 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x0098fe70 63682f69 6e636c75 64652f74 6f726368 ch/include/torch
   0x0098fe80 2f637573 746f6d5f 636c6173 732e6800 /custom_class.h.
   0x0098fe90 54656e73 6f72496d 706c2077 69746820 TensorImpl with 
   0x0098fea0 6e756c6c 70747220 6973206e 6f742073 nullptr is not s
   0x0098feb0 7570706f 72746564 00717565 75650069 upported.queue.i
   0x0098fec0 6e69745f 74656e73 6f720076 6563746f nit_tensor.vecto
@@ -11892,15 +11892,15 @@
   0x00990710 204f626a 65637420 62757420 676f7420  Object but got 
   0x00990720 00746f4f 626a6563 74000000 00000000 .toObject.......
   0x00990730 69734f62 6a656374 28292049 4e544552 isObject() INTER
   0x00990740 4e414c20 41535345 52542046 41494c45 NAL ASSERT FAILE
   0x00990750 44206174 20222f67 69746875 622f686f D at "/github/ho
   0x00990760 6d652f6d 696e6963 6f6e6461 2f656e76 me/miniconda/env
   0x00990770 732f6275 696c645f 62696e61 72792f6c s/build_binary/l
-  0x00990780 69622f70 7974686f 6e332e39 2f736974 ib/python3.9/sit
+  0x00990780 69622f70 7974686f 6e332e38 2f736974 ib/python3.8/sit
   0x00990790 652d7061 636b6167 65732f74 6f726368 e-packages/torch
   0x009907a0 2f696e63 6c756465 2f415465 6e2f636f /include/ATen/co
   0x009907b0 72652f69 76616c75 655f696e 6c2e6822 re/ivalue_inl.h"
   0x009907c0 3a313333 2c20706c 65617365 20726570 :133, please rep
   0x009907d0 6f727420 61206275 6720746f 20507954 ort a bug to PyT
   0x009907e0 6f726368 2e200000 41726775 6d656e74 orch. ..Argument
   0x009907f0 20706173 73656420 746f2061 74282920  passed to at() 
@@ -11908,15 +11908,15 @@
   0x00990810 61702e00 2f73697a 65002f00 00000000 ap../size./.....
   0x00990820 53747265 616d7320 68617665 2061206d Streams have a m
   0x00990830 6978206f 66206465 76696365 20747970 ix of device typ
   0x00990840 65733a20 73747265 616d2030 20697320 es: stream 0 is 
   0x00990850 6f6e2000 00000000 2f676974 6875622f on ...../github/
   0x00990860 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x00990870 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x00990880 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x00990880 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x00990890 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x009908a0 63682f69 6e636c75 64652f63 31302f63 ch/include/c10/c
   0x009908b0 6f72652f 696d706c 2f496e6c 696e6553 ore/impl/InlineS
   0x009908c0 74726561 6d477561 72642e68 00207768 treamGuard.h. wh
   0x009908d0 696c6520 73747265 616d2000 20697320 ile stream . is 
   0x009908e0 6f6e2064 65766963 65200067 65744465 on device .getDe
   0x009908f0 76696365 54797065 4f665374 7265616d viceTypeOfStream
@@ -11929,15 +11929,15 @@
   0x00990960 7320616c 72656164 79206d61 726b6564 s already marked
   0x00990970 20636f6d 706c6574 65640000 00000000  completed......
   0x00990980 21636f6d 706c6574 65642829 20494e54 !completed() INT
   0x00990990 45524e41 4c204153 53455254 20464149 ERNAL ASSERT FAI
   0x009909a0 4c454420 61742022 2f676974 6875622f LED at "/github/
   0x009909b0 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x009909c0 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x009909d0 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x009909d0 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x009909e0 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x009909f0 63682f69 6e636c75 64652f41 54656e2f ch/include/ATen/
   0x00990a00 636f7265 2f697661 6c75655f 696e6c2e core/ivalue_inl.
   0x00990a10 68223a31 3231352c 20706c65 61736520 h":1215, please 
   0x00990a20 7265706f 72742061 20627567 20746f20 report a bug to 
   0x00990a30 5079546f 7263682e 20000000 00000000 PyTorch. .......
   0x00990a40 20776869 63682061 7265206e 6f742061  which are not a
@@ -11973,15 +11973,15 @@
   0x00990c20 6965773c 63686172 3e5d0000 00000000 iew<char>]......
   0x00990c30 20636f75 6c64206e 6f742062 6520636f  could not be co
   0x00990c40 6e766572 74656420 746f2061 6e79206f nverted to any o
   0x00990c50 66207468 65206b6e 6f776e20 74797065 f the known type
   0x00990c60 732e0000 00000000 2f676974 6875622f s......./github/
   0x00990c70 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x00990c80 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x00990c90 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x00990c90 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x00990ca0 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x00990cb0 63682f69 6e636c75 64652f41 54656e2f ch/include/ATen/
   0x00990cc0 636f7265 2f6a6974 5f747970 652e6800 core/jit_type.h.
   0x00990cd0 54797065 20000000 636f6e73 74657870 Type ...constexp
   0x00990ce0 72206331 303a3a73 7472696e 675f7669 r c10::string_vi
   0x00990cf0 65772063 31303a3a 7574696c 3a3a6465 ew c10::util::de
   0x00990d00 7461696c 3a3a6675 6c6c795f 7175616c tail::fully_qual
@@ -12043,15 +12043,15 @@
   0x00991080 61696e20 61206375 73746f6d 20636c61 ain a custom cla
   0x00991090 73732100 00000000 69734361 7073756c ss!.....isCapsul
   0x009910a0 65282920 494e5445 524e414c 20415353 e() INTERNAL ASS
   0x009910b0 45525420 4641494c 45442061 7420222f ERT FAILED at "/
   0x009910c0 67697468 75622f68 6f6d652f 6d696e69 github/home/mini
   0x009910d0 636f6e64 612f656e 76732f62 75696c64 conda/envs/build
   0x009910e0 5f62696e 6172792f 6c69622f 70797468 _binary/lib/pyth
-  0x009910f0 6f6e332e 392f7369 74652d70 61636b61 on3.9/site-packa
+  0x009910f0 6f6e332e 382f7369 74652d70 61636b61 on3.8/site-packa
   0x00991100 6765732f 746f7263 682f696e 636c7564 ges/torch/includ
   0x00991110 652f4154 656e2f63 6f72652f 6976616c e/ATen/core/ival
   0x00991120 75655f69 6e6c2e68 223a3232 352c2070 ue_inl.h":225, p
   0x00991130 6c656173 65207265 706f7274 20612062 lease report a b
   0x00991140 75672074 6f205079 546f7263 682e2000 ug to PyTorch. .
   0x00991150 746f4375 73746f6d 436c6173 7300746f toCustomClass.to
   0x00991160 43617073 756c6500 45787065 63746564 Capsule.Expected
@@ -12059,15 +12059,15 @@
   0x00991180 676f7420 00746f54 656e736f 724c6973 got .toTensorLis
   0x00991190 74000000 00000000 69735465 6e736f72 t.......isTensor
   0x009911a0 4c697374 28292049 4e544552 4e414c20 List() INTERNAL 
   0x009911b0 41535345 52542046 41494c45 44206174 ASSERT FAILED at
   0x009911c0 20222f67 69746875 622f686f 6d652f6d  "/github/home/m
   0x009911d0 696e6963 6f6e6461 2f656e76 732f6275 iniconda/envs/bu
   0x009911e0 696c645f 62696e61 72792f6c 69622f70 ild_binary/lib/p
-  0x009911f0 7974686f 6e332e39 2f736974 652d7061 ython3.9/site-pa
+  0x009911f0 7974686f 6e332e38 2f736974 652d7061 ython3.8/site-pa
   0x00991200 636b6167 65732f74 6f726368 2f696e63 ckages/torch/inc
   0x00991210 6c756465 2f415465 6e2f636f 72652f69 lude/ATen/core/i
   0x00991220 76616c75 655f696e 6c2e6822 3a323033 value_inl.h":203
   0x00991230 382c2070 6c656173 65207265 706f7274 8, please report
   0x00991240 20612062 75672074 6f205079 546f7263  a bug to PyTorc
   0x00991250 682e2000 54726965 6420746f 20636173 h. .Tried to cas
   0x00991260 74206120 44696374 3c003e20 746f2061 t a Dict<.> to a
@@ -12080,36 +12080,36 @@
   0x009912d0 6963742e 696d706c 5f2d3e65 6c656d65 ict.impl_->eleme
   0x009912e0 6e745479 7065732e 6b657954 79706520 ntTypes.keyType 
   0x009912f0 494e5445 524e414c 20415353 45525420 INTERNAL ASSERT 
   0x00991300 4641494c 45442061 7420222f 67697468 FAILED at "/gith
   0x00991310 75622f68 6f6d652f 6d696e69 636f6e64 ub/home/minicond
   0x00991320 612f656e 76732f62 75696c64 5f62696e a/envs/build_bin
   0x00991330 6172792f 6c69622f 70797468 6f6e332e ary/lib/python3.
-  0x00991340 392f7369 74652d70 61636b61 6765732f 9/site-packages/
+  0x00991340 382f7369 74652d70 61636b61 6765732f 8/site-packages/
   0x00991350 746f7263 682f696e 636c7564 652f4154 torch/include/AT
   0x00991360 656e2f63 6f72652f 44696374 5f696e6c en/core/Dict_inl
   0x00991370 2e68223a 32362c20 706c6561 73652072 .h":26, please r
   0x00991380 65706f72 74206120 62756720 746f2050 eport a bug to P
   0x00991390 79546f72 63682e20 00000000 00000000 yTorch. ........
   0x009913a0 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x009913b0 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x009913c0 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x009913d0 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x009913d0 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x009913e0 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x009913f0 64652f41 54656e2f 636f7265 2f446963 de/ATen/core/Dic
   0x00991400 745f696e 6c2e6800 2a676574 54797065 t_inl.h.*getType
   0x00991410 5074723c 56616c75 653e2829 203d3d20 Ptr<Value>() == 
   0x00991420 2a646963 742e696d 706c5f2d 3e656c65 *dict.impl_->ele
   0x00991430 6d656e74 54797065 732e7661 6c756554 mentTypes.valueT
   0x00991440 79706520 494e5445 524e414c 20415353 ype INTERNAL ASS
   0x00991450 45525420 4641494c 45442061 7420222f ERT FAILED at "/
   0x00991460 67697468 75622f68 6f6d652f 6d696e69 github/home/mini
   0x00991470 636f6e64 612f656e 76732f62 75696c64 conda/envs/build
   0x00991480 5f62696e 6172792f 6c69622f 70797468 _binary/lib/pyth
-  0x00991490 6f6e332e 392f7369 74652d70 61636b61 on3.9/site-packa
+  0x00991490 6f6e332e 382f7369 74652d70 61636b61 on3.8/site-packa
   0x009914a0 6765732f 746f7263 682f696e 636c7564 ges/torch/includ
   0x009914b0 652f4154 656e2f63 6f72652f 44696374 e/ATen/core/Dict
   0x009914c0 5f696e6c 2e68223a 32372c20 706c6561 _inl.h":27, plea
   0x009914d0 73652072 65706f72 74206120 62756720 se report a bug 
   0x009914e0 746f2050 79546f72 63682e20 00000000 to PyTorch. ....
   0x009914f0 4e336331 30313056 616c7565 4572726f N3c1010ValueErro
   0x00991500 72450000 00000000 00000000 00000000 rE..............
@@ -12492,15 +12492,15 @@
   0x00992c90 6a767020 6973206e 6f742069 6d706c65 jvp is not imple
   0x00992ca0 6d656e74 65642066 6f722074 68652063 mented for the c
   0x00992cb0 2b2b2041 5049206f 66206375 73746f6d ++ API of custom
   0x00992cc0 2046756e 6374696f 6e207965 742e0000  Function yet...
   0x00992cd0 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x00992ce0 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x00992cf0 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x00992d00 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x00992d00 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x00992d10 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x00992d20 64652f74 6f726368 2f637372 632f6175 de/torch/csrc/au
   0x00992d30 746f6772 61642f63 7573746f 6d5f6675 tograd/custom_fu
   0x00992d40 6e637469 6f6e2e68 00000000 00000000 nction.h........
   0x00992d50 636f6d70 696c6564 5f617267 73206e6f compiled_args no
   0x00992d60 7420696d 706c656d 656e7465 6420666f t implemented fo
   0x00992d70 72206e6f 6e2d7472 61636561 626c6520 r non-traceable 
@@ -12552,25 +12552,25 @@
   0x00993050 2074686f 7365206f 6620616c 6c206974  those of all it
   0x00993060 73206368 696c6472 656e0000 00000000 s children......
   0x00993070 21686173 5f706172 656e745f 20494e54 !has_parent_ INT
   0x00993080 45524e41 4c204153 53455254 20464149 ERNAL ASSERT FAI
   0x00993090 4c454420 61742022 2f676974 6875622f LED at "/github/
   0x009930a0 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x009930b0 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x009930c0 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x009930c0 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x009930d0 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x009930e0 63682f69 6e636c75 64652f74 6f726368 ch/include/torch
   0x009930f0 2f637372 632f6175 746f6772 61642f66 /csrc/autograd/f
   0x00993100 756e6374 696f6e2e 68223a32 36322c20 unction.h":262, 
   0x00993110 706c6561 73652072 65706f72 74206120 please report a 
   0x00993120 62756720 746f2050 79546f72 63682e20 bug to PyTorch. 
   0x00993130 00000000 00000000 2f676974 6875622f ......../github/
   0x00993140 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x00993150 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x00993160 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x00993160 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x00993170 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x00993180 63682f69 6e636c75 64652f74 6f726368 ch/include/torch
   0x00993190 2f637372 632f6175 746f6772 61642f66 /csrc/autograd/f
   0x009931a0 756e6374 696f6e2e 68000000 00000000 unction.h.......
   0x009931b0 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x009931c0 4d4d2f66 6267656d 6d5f6770 752f636f MM/fbgemm_gpu/co
   0x009931d0 64656765 6e2f7472 61696e69 6e672f62 degen/training/b
@@ -12594,123 +12594,123 @@
   0x009932f0 00000000 00000000 6374785f 2e6e6f6e ........ctx_.non
   0x00993300 5f646966 66657265 6e746961 626c655f _differentiable_
   0x00993310 2e656d70 74792829 20494e54 45524e41 .empty() INTERNA
   0x00993320 4c204153 53455254 20464149 4c454420 L ASSERT FAILED 
   0x00993330 61742022 2f676974 6875622f 686f6d65 at "/github/home
   0x00993340 2f6d696e 69636f6e 64612f65 6e76732f /miniconda/envs/
   0x00993350 6275696c 645f6269 6e617279 2f6c6962 build_binary/lib
-  0x00993360 2f707974 686f6e33 2e392f73 6974652d /python3.9/site-
+  0x00993360 2f707974 686f6e33 2e382f73 6974652d /python3.8/site-
   0x00993370 7061636b 61676573 2f746f72 63682f69 packages/torch/i
   0x00993380 6e636c75 64652f74 6f726368 2f637372 nclude/torch/csr
   0x00993390 632f6175 746f6772 61642f63 7573746f c/autograd/custo
   0x009933a0 6d5f6675 6e637469 6f6e2e68 223a3232 m_function.h":22
   0x009933b0 312c2070 6c656173 65207265 706f7274 1, please report
   0x009933c0 20612062 75672074 6f205079 546f7263  a bug to PyTorc
   0x009933d0 682e2000 00000000 6374785f 2e646972 h. .....ctx_.dir
   0x009933e0 74795f69 6e707574 735f2e65 6d707479 ty_inputs_.empty
   0x009933f0 28292049 4e544552 4e414c20 41535345 () INTERNAL ASSE
   0x00993400 52542046 41494c45 44206174 20222f67 RT FAILED at "/g
   0x00993410 69746875 622f686f 6d652f6d 696e6963 ithub/home/minic
   0x00993420 6f6e6461 2f656e76 732f6275 696c645f onda/envs/build_
   0x00993430 62696e61 72792f6c 69622f70 7974686f binary/lib/pytho
-  0x00993440 6e332e39 2f736974 652d7061 636b6167 n3.9/site-packag
+  0x00993440 6e332e38 2f736974 652d7061 636b6167 n3.8/site-packag
   0x00993450 65732f74 6f726368 2f696e63 6c756465 es/torch/include
   0x00993460 2f746f72 63682f63 7372632f 6175746f /torch/csrc/auto
   0x00993470 67726164 2f637573 746f6d5f 66756e63 grad/custom_func
   0x00993480 74696f6e 2e68223a 3232322c 20706c65 tion.h":222, ple
   0x00993490 61736520 7265706f 72742061 20627567 ase report a bug
   0x009934a0 20746f20 5079546f 7263682e 20000000  to PyTorch. ...
   0x009934b0 69742021 3d205f73 61766564 5f766172 it != _saved_var
   0x009934c0 6961626c 65732e65 6e642829 20494e54 iables.end() INT
   0x009934d0 45524e41 4c204153 53455254 20464149 ERNAL ASSERT FAI
   0x009934e0 4c454420 61742022 2f676974 6875622f LED at "/github/
   0x009934f0 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x00993500 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x00993510 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x00993510 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x00993520 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x00993530 63682f69 6e636c75 64652f74 6f726368 ch/include/torch
   0x00993540 2f637372 632f6479 6e616d6f 2f636f6d /csrc/dynamo/com
   0x00993550 70696c65 645f6175 746f6772 61642e68 piled_autograd.h
   0x00993560 223a3133 382c2070 6c656173 65207265 ":138, please re
   0x00993570 706f7274 20612062 75672074 6f205079 port a bug to Py
   0x00993580 546f7263 682e2000 6172672e 70726f78 Torch. .arg.prox
   0x00993590 795f7465 6e736f72 2e646566 696e6564 y_tensor.defined
   0x009935a0 28292049 4e544552 4e414c20 41535345 () INTERNAL ASSE
   0x009935b0 52542046 41494c45 44206174 20222f67 RT FAILED at "/g
   0x009935c0 69746875 622f686f 6d652f6d 696e6963 ithub/home/minic
   0x009935d0 6f6e6461 2f656e76 732f6275 696c645f onda/envs/build_
   0x009935e0 62696e61 72792f6c 69622f70 7974686f binary/lib/pytho
-  0x009935f0 6e332e39 2f736974 652d7061 636b6167 n3.9/site-packag
+  0x009935f0 6e332e38 2f736974 652d7061 636b6167 n3.8/site-packag
   0x00993600 65732f74 6f726368 2f696e63 6c756465 es/torch/include
   0x00993610 2f746f72 63682f63 7372632f 64796e61 /torch/csrc/dyna
   0x00993620 6d6f2f63 6f6d7069 6c65645f 6175746f mo/compiled_auto
   0x00993630 67726164 2e68223a 3536312c 20706c65 grad.h":561, ple
   0x00993640 61736520 7265706f 72742061 20627567 ase report a bug
   0x00993650 20746f20 5079546f 7263682e 20000000  to PyTorch. ...
   0x00993660 6374785f 2e746f5f 73617665 5f2e656d ctx_.to_save_.em
   0x00993670 70747928 2920494e 5445524e 414c2041 pty() INTERNAL A
   0x00993680 53534552 54204641 494c4544 20617420 SSERT FAILED at 
   0x00993690 222f6769 74687562 2f686f6d 652f6d69 "/github/home/mi
   0x009936a0 6e69636f 6e64612f 656e7673 2f627569 niconda/envs/bui
   0x009936b0 6c645f62 696e6172 792f6c69 622f7079 ld_binary/lib/py
-  0x009936c0 74686f6e 332e392f 73697465 2d706163 thon3.9/site-pac
+  0x009936c0 74686f6e 332e382f 73697465 2d706163 thon3.8/site-pac
   0x009936d0 6b616765 732f746f 7263682f 696e636c kages/torch/incl
   0x009936e0 7564652f 746f7263 682f6373 72632f61 ude/torch/csrc/a
   0x009936f0 75746f67 7261642f 63757374 6f6d5f66 utograd/custom_f
   0x00993700 756e6374 696f6e2e 68223a32 32342c20 unction.h":224, 
   0x00993710 706c6561 73652072 65706f72 74206120 please report a 
   0x00993720 62756720 746f2050 79546f72 63682e20 bug to PyTorch. 
   0x00993730 00000000 00000000 69742021 3d207468 ........it != th
   0x00993740 69732d3e 656e6428 2920494e 5445524e is->end() INTERN
   0x00993750 414c2041 53534552 54204641 494c4544 AL ASSERT FAILED
   0x00993760 20617420 222f6769 74687562 2f686f6d  at "/github/hom
   0x00993770 652f6d69 6e69636f 6e64612f 656e7673 e/miniconda/envs
   0x00993780 2f627569 6c645f62 696e6172 792f6c69 /build_binary/li
-  0x00993790 622f7079 74686f6e 332e392f 73697465 b/python3.9/site
+  0x00993790 622f7079 74686f6e 332e382f 73697465 b/python3.8/site
   0x009937a0 2d706163 6b616765 732f746f 7263682f -packages/torch/
   0x009937b0 696e636c 7564652f 746f7263 682f6373 include/torch/cs
   0x009937c0 72632f64 796e616d 6f2f636f 6d70696c rc/dynamo/compil
   0x009937d0 65645f61 75746f67 7261642e 68223a37 ed_autograd.h":7
   0x009937e0 36302c20 706c6561 73652072 65706f72 60, please repor
   0x009937f0 74206120 62756720 746f2050 79546f72 t a bug to PyTor
   0x00993800 63682e20 00000000 6374785f 2e6e6f6e ch. ....ctx_.non
   0x00993810 5f646966 66657265 6e746961 626c655f _differentiable_
   0x00993820 2e656d70 74792829 20494e54 45524e41 .empty() INTERNA
   0x00993830 4c204153 53455254 20464149 4c454420 L ASSERT FAILED 
   0x00993840 61742022 2f676974 6875622f 686f6d65 at "/github/home
   0x00993850 2f6d696e 69636f6e 64612f65 6e76732f /miniconda/envs/
   0x00993860 6275696c 645f6269 6e617279 2f6c6962 build_binary/lib
-  0x00993870 2f707974 686f6e33 2e392f73 6974652d /python3.9/site-
+  0x00993870 2f707974 686f6e33 2e382f73 6974652d /python3.8/site-
   0x00993880 7061636b 61676573 2f746f72 63682f69 packages/torch/i
   0x00993890 6e636c75 64652f74 6f726368 2f637372 nclude/torch/csr
   0x009938a0 632f6175 746f6772 61642f63 7573746f c/autograd/custo
   0x009938b0 6d5f6675 6e637469 6f6e2e68 223a3233 m_function.h":23
   0x009938c0 312c2070 6c656173 65207265 706f7274 1, please report
   0x009938d0 20612062 75672074 6f205079 546f7263  a bug to PyTorc
   0x009938e0 682e2000 00000000 6374785f 2e646972 h. .....ctx_.dir
   0x009938f0 74795f69 6e707574 735f2e65 6d707479 ty_inputs_.empty
   0x00993900 28292049 4e544552 4e414c20 41535345 () INTERNAL ASSE
   0x00993910 52542046 41494c45 44206174 20222f67 RT FAILED at "/g
   0x00993920 69746875 622f686f 6d652f6d 696e6963 ithub/home/minic
   0x00993930 6f6e6461 2f656e76 732f6275 696c645f onda/envs/build_
   0x00993940 62696e61 72792f6c 69622f70 7974686f binary/lib/pytho
-  0x00993950 6e332e39 2f736974 652d7061 636b6167 n3.9/site-packag
+  0x00993950 6e332e38 2f736974 652d7061 636b6167 n3.8/site-packag
   0x00993960 65732f74 6f726368 2f696e63 6c756465 es/torch/include
   0x00993970 2f746f72 63682f63 7372632f 6175746f /torch/csrc/auto
   0x00993980 67726164 2f637573 746f6d5f 66756e63 grad/custom_func
   0x00993990 74696f6e 2e68223a 3233322c 20706c65 tion.h":232, ple
   0x009939a0 61736520 7265706f 72742061 20627567 ase report a bug
   0x009939b0 20746f20 5079546f 7263682e 20000000  to PyTorch. ...
   0x009939c0 6374785f 2e746f5f 73617665 5f2e656d ctx_.to_save_.em
   0x009939d0 70747928 2920494e 5445524e 414c2041 pty() INTERNAL A
   0x009939e0 53534552 54204641 494c4544 20617420 SSERT FAILED at 
   0x009939f0 222f6769 74687562 2f686f6d 652f6d69 "/github/home/mi
   0x00993a00 6e69636f 6e64612f 656e7673 2f627569 niconda/envs/bui
   0x00993a10 6c645f62 696e6172 792f6c69 622f7079 ld_binary/lib/py
-  0x00993a20 74686f6e 332e392f 73697465 2d706163 thon3.9/site-pac
+  0x00993a20 74686f6e 332e382f 73697465 2d706163 thon3.8/site-pac
   0x00993a30 6b616765 732f746f 7263682f 696e636c kages/torch/incl
   0x00993a40 7564652f 746f7263 682f6373 72632f61 ude/torch/csrc/a
   0x00993a50 75746f67 7261642f 63757374 6f6d5f66 utograd/custom_f
   0x00993a60 756e6374 696f6e2e 68223a32 33342c20 unction.h":234, 
   0x00993a70 706c6561 73652072 65706f72 74206120 please report a 
   0x00993a80 62756720 746f2050 79546f72 63682e20 bug to PyTorch. 
   0x00993a90 00000000 00000000 00000000 00000000 ................
@@ -12800,25 +12800,25 @@
   0x00993fd0 79453245 45000000 73796d5f 73697a65 yE2EE...sym_size
   0x00993fe0 735f696e 64657820 3c207379 6d5f7369 s_index < sym_si
   0x00993ff0 7a65732e 73697a65 28292049 4e544552 zes.size() INTER
   0x00994000 4e414c20 41535345 52542046 41494c45 NAL ASSERT FAILE
   0x00994010 44206174 20222f67 69746875 622f686f D at "/github/ho
   0x00994020 6d652f6d 696e6963 6f6e6461 2f656e76 me/miniconda/env
   0x00994030 732f6275 696c645f 62696e61 72792f6c s/build_binary/l
-  0x00994040 69622f70 7974686f 6e332e39 2f736974 ib/python3.9/sit
+  0x00994040 69622f70 7974686f 6e332e38 2f736974 ib/python3.8/sit
   0x00994050 652d7061 636b6167 65732f74 6f726368 e-packages/torch
   0x00994060 2f696e63 6c756465 2f746f72 63682f63 /include/torch/c
   0x00994070 7372632f 64796e61 6d6f2f63 6f6d7069 src/dynamo/compi
   0x00994080 6c65645f 6175746f 67726164 2e68223a led_autograd.h":
   0x00994090 3533312c 20706c65 61736520 7265706f 531, please repo
   0x009940a0 72742061 20627567 20746f20 5079546f rt a bug to PyTo
   0x009940b0 7263682e 20000000 2f676974 6875622f rch. .../github/
   0x009940c0 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x009940d0 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x009940e0 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x009940e0 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x009940f0 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x00994100 63682f69 6e636c75 64652f74 6f726368 ch/include/torch
   0x00994110 2f637372 632f6479 6e616d6f 2f636f6d /csrc/dynamo/com
   0x00994120 70696c65 645f6175 746f6772 61642e68 piled_autograd.h
   0x00994130 006e6578 745f7379 6d5f7369 7a650000 .next_sym_size..
   0x00994140 50467650 4e35746f 72636838 6175746f PFvPN5torch8auto
   0x00994150 67726164 344e6f64 65454500 00000000 grad4NodeEE.....
@@ -13032,26 +13032,26 @@
   0x00994e50 84f5c9ff 34f5c9ff ecf4c9ff a4f4c9ff ....4...........
   0x00994e60 44f4c9ff b4fbc9ff 69734465 76696365 D.......isDevice
   0x00994e70 28292049 4e544552 4e414c20 41535345 () INTERNAL ASSE
   0x00994e80 52542046 41494c45 44206174 20222f67 RT FAILED at "/g
   0x00994e90 69746875 622f686f 6d652f6d 696e6963 ithub/home/minic
   0x00994ea0 6f6e6461 2f656e76 732f6275 696c645f onda/envs/build_
   0x00994eb0 62696e61 72792f6c 69622f70 7974686f binary/lib/pytho
-  0x00994ec0 6e332e39 2f736974 652d7061 636b6167 n3.9/site-packag
+  0x00994ec0 6e332e38 2f736974 652d7061 636b6167 n3.8/site-packag
   0x00994ed0 65732f74 6f726368 2f696e63 6c756465 es/torch/include
   0x00994ee0 2f415465 6e2f636f 72652f69 76616c75 /ATen/core/ivalu
   0x00994ef0 652e6822 3a393331 2c20706c 65617365 e.h":931, please
   0x00994f00 20726570 6f727420 61206275 6720746f  report a bug to
   0x00994f10 20507954 6f726368 2e200000 00000000  PyTorch. ......
   0x00994f20 69735465 6e736f72 4c697374 28292049 isTensorList() I
   0x00994f30 4e544552 4e414c20 41535345 52542046 NTERNAL ASSERT F
   0x00994f40 41494c45 44206174 20222f67 69746875 AILED at "/githu
   0x00994f50 622f686f 6d652f6d 696e6963 6f6e6461 b/home/miniconda
   0x00994f60 2f656e76 732f6275 696c645f 62696e61 /envs/build_bina
-  0x00994f70 72792f6c 69622f70 7974686f 6e332e39 ry/lib/python3.9
+  0x00994f70 72792f6c 69622f70 7974686f 6e332e38 ry/lib/python3.8
   0x00994f80 2f736974 652d7061 636b6167 65732f74 /site-packages/t
   0x00994f90 6f726368 2f696e63 6c756465 2f415465 orch/include/ATe
   0x00994fa0 6e2f636f 72652f69 76616c75 655f696e n/core/ivalue_in
   0x00994fb0 6c2e6822 3a323033 342c2070 6c656173 l.h":2034, pleas
   0x00994fc0 65207265 706f7274 20612062 75672074 e report a bug t
   0x00994fd0 6f205079 546f7263 682e2000 746f4465 o PyTorch. .toDe
   0x00994fe0 76696365 00000000 00000000 00000000 vice............
@@ -13151,23 +13151,23 @@
   0x009955c0 65643f20 20496620 736f2c20 706c6561 ed?  If so, plea
   0x009955d0 73652072 65706f72 7420616e 20656e68 se report an enh
   0x009955e0 616e6365 6d656e74 20726571 75657374 ancement request
   0x009955f0 20746f20 5079546f 7263682e 29000000  to PyTorch.)...
   0x00995600 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x00995610 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x00995620 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x00995630 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x00995630 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x00995640 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x00995650 64652f63 31302f63 6f72652f 53796d42 de/c10/core/SymB
   0x00995660 6f6f6c2e 68000000 3020494e 5445524e ool.h...0 INTERN
   0x00995670 414c2041 53534552 54204641 494c4544 AL ASSERT FAILED
   0x00995680 20617420 222f6769 74687562 2f686f6d  at "/github/hom
   0x00995690 652f6d69 6e69636f 6e64612f 656e7673 e/miniconda/envs
   0x009956a0 2f627569 6c645f62 696e6172 792f6c69 /build_binary/li
-  0x009956b0 622f7079 74686f6e 332e392f 73697465 b/python3.9/site
+  0x009956b0 622f7079 74686f6e 332e382f 73697465 b/python3.8/site
   0x009956c0 2d706163 6b616765 732f746f 7263682f -packages/torch/
   0x009956d0 696e636c 7564652f 4154656e 2f636f72 include/ATen/cor
   0x009956e0 652f6976 616c7565 2e68223a 3637362c e/ivalue.h":676,
   0x009956f0 20706c65 61736520 7265706f 72742061  please report a
   0x00995700 20627567 20746f20 5079546f 7263682e  bug to PyTorch.
   0x00995710 20000000 00000000 7065726d 7574655f  .......permute_
   0x00995720 706f6f6c 65645f65 6d627320 646f6573 pooled_embs does
@@ -13187,25 +13187,25 @@
   0x00995800 68656d61 20726567 69737465 72656420 hema registered 
   0x00995810 79657400 00000000 73636865 6d615f2e yet.....schema_.
   0x00995820 6861735f 76616c75 65282920 494e5445 has_value() INTE
   0x00995830 524e414c 20415353 45525420 4641494c RNAL ASSERT FAIL
   0x00995840 45442061 7420222f 67697468 75622f68 ED at "/github/h
   0x00995850 6f6d652f 6d696e69 636f6e64 612f656e ome/miniconda/en
   0x00995860 76732f62 75696c64 5f62696e 6172792f vs/build_binary/
-  0x00995870 6c69622f 70797468 6f6e332e 392f7369 lib/python3.9/si
+  0x00995870 6c69622f 70797468 6f6e332e 382f7369 lib/python3.8/si
   0x00995880 74652d70 61636b61 6765732f 746f7263 te-packages/torc
   0x00995890 682f696e 636c7564 652f4154 656e2f63 h/include/ATen/c
   0x009958a0 6f72652f 64697370 61746368 2f4f7065 ore/dispatch/Ope
   0x009958b0 7261746f 72456e74 72792e68 223a3830 ratorEntry.h":80
   0x009958c0 2c20706c 65617365 20726570 6f727420 , please report 
   0x009958d0 61206275 6720746f 20507954 6f726368 a bug to PyTorch
   0x009958e0 2e200000 00000000 2f676974 6875622f . ....../github/
   0x009958f0 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x00995900 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x00995910 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x00995910 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x00995920 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x00995930 63682f69 6e636c75 64652f41 54656e2f ch/include/ATen/
   0x00995940 636f7265 2f646973 70617463 682f4f70 core/dispatch/Op
   0x00995950 65726174 6f72456e 7472792e 68007363 eratorEntry.h.sc
   0x00995960 68656d61 00000000 00000000 00000000 hema............
   0x00995970 00000000 00000000 00000000 00000000 ................
   0x00995980 464e3261 74365465 6e736f72 45524b53 FN2at6TensorERKS
@@ -13713,15 +13713,15 @@
   0x009978e0 62617463 6865645f 64656e73 655f7665 batched_dense_ve
   0x009978f0 635f6a61 67676564 5f32645f 6d756c00 c_jagged_2d_mul.
   0x00997900 69734c69 73742829 20494e54 45524e41 isList() INTERNA
   0x00997910 4c204153 53455254 20464149 4c454420 L ASSERT FAILED 
   0x00997920 61742022 2f676974 6875622f 686f6d65 at "/github/home
   0x00997930 2f6d696e 69636f6e 64612f65 6e76732f /miniconda/envs/
   0x00997940 6275696c 645f6269 6e617279 2f6c6962 build_binary/lib
-  0x00997950 2f707974 686f6e33 2e392f73 6974652d /python3.9/site-
+  0x00997950 2f707974 686f6e33 2e382f73 6974652d /python3.8/site-
   0x00997960 7061636b 61676573 2f746f72 63682f69 packages/torch/i
   0x00997970 6e636c75 64652f41 54656e2f 636f7265 nclude/ATen/core
   0x00997980 2f697661 6c75655f 696e6c2e 68223a32 /ivalue_inl.h":2
   0x00997990 3036362c 20706c65 61736520 7265706f 066, please repo
   0x009979a0 72742061 20627567 20746f20 5079546f rt a bug to PyTo
   0x009979b0 7263682e 20000000 2f5f5f77 2f464247 rch. .../__w/FBG
   0x009979c0 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
@@ -13798,24 +13798,24 @@
   0x00997e30 75742067 6f742000 69735379 6d496e74 ut got .isSymInt
   0x00997e40 4c697374 2829207c 7c206973 496e744c List() || isIntL
   0x00997e50 69737428 2920494e 5445524e 414c2041 ist() INTERNAL A
   0x00997e60 53534552 54204641 494c4544 20617420 SSERT FAILED at 
   0x00997e70 222f6769 74687562 2f686f6d 652f6d69 "/github/home/mi
   0x00997e80 6e69636f 6e64612f 656e7673 2f627569 niconda/envs/bui
   0x00997e90 6c645f62 696e6172 792f6c69 622f7079 ld_binary/lib/py
-  0x00997ea0 74686f6e 332e392f 73697465 2d706163 thon3.9/site-pac
+  0x00997ea0 74686f6e 332e382f 73697465 2d706163 thon3.8/site-pac
   0x00997eb0 6b616765 732f746f 7263682f 696e636c kages/torch/incl
   0x00997ec0 7564652f 4154656e 2f636f72 652f6976 ude/ATen/core/iv
   0x00997ed0 616c7565 5f696e6c 2e68223a 31393738 alue_inl.h":1978
   0x00997ee0 2c20706c 65617365 20726570 6f727420 , please report 
   0x00997ef0 61206275 6720746f 20507954 6f726368 a bug to PyTorch
   0x00997f00 2e200000 00000000 2f676974 6875622f . ....../github/
   0x00997f10 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x00997f20 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x00997f30 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x00997f30 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x00997f40 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x00997f50 63682f69 6e636c75 64652f63 31302f63 ch/include/c10/c
   0x00997f60 6f72652f 53796d49 6e742e68 00000000 ore/SymInt.h....
   0x00997f70 45787065 63746564 2064656e 73655f76 Expected dense_v
   0x00997f80 616c7565 735f6772 61642e73 796d5f73 alues_grad.sym_s
   0x00997f90 697a6573 2829203d 3d206465 6e73655f izes() == dense_
   0x00997fa0 73686170 6520746f 20626520 74727565 shape to be true
@@ -13924,15 +13924,15 @@
   0x00998610 74797065 20776974 6820636f 6e746169 type with contai
   0x00998620 6e656420 74797065 73206469 64206e6f ned types did no
   0x00998630 74206f76 65726c6f 61642063 72656174 t overload creat
   0x00998640 65576974 68436f6e 7461696e 65643a20 eWithContained: 
   0x00998650 00000000 00000000 2f676974 6875622f ......../github/
   0x00998660 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x00998670 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x00998680 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x00998680 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x00998690 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x009986a0 63682f69 6e636c75 64652f41 54656e2f ch/include/ATen/
   0x009986b0 636f7265 2f6a6974 5f747970 655f6261 core/jit_type_ba
   0x009986c0 73652e68 00637265 61746557 69746843 se.h.createWithC
   0x009986d0 6f6e7461 696e6564 003b204c 656e6774 ontained.; Lengt
   0x009986e0 68203d20 00000000 41727261 79526566 h = ....ArrayRef
   0x009986f0 3a20696e 76616c69 6420696e 64657820 : invalid index 
@@ -14516,35 +14516,35 @@
   0x0099ab10 45450000 00000000 00000000 78000000 EE..........x...
   0x0099ab20 69735379 6d496e74 2829207c 7c206973 isSymInt() || is
   0x0099ab30 496e7428 2920494e 5445524e 414c2041 Int() INTERNAL A
   0x0099ab40 53534552 54204641 494c4544 20617420 SSERT FAILED at 
   0x0099ab50 222f6769 74687562 2f686f6d 652f6d69 "/github/home/mi
   0x0099ab60 6e69636f 6e64612f 656e7673 2f627569 niconda/envs/bui
   0x0099ab70 6c645f62 696e6172 792f6c69 622f7079 ld_binary/lib/py
-  0x0099ab80 74686f6e 332e392f 73697465 2d706163 thon3.9/site-pac
+  0x0099ab80 74686f6e 332e382f 73697465 2d706163 thon3.8/site-pac
   0x0099ab90 6b616765 732f746f 7263682f 696e636c kages/torch/incl
   0x0099aba0 7564652f 4154656e 2f636f72 652f6976 ude/ATen/core/iv
   0x0099abb0 616c7565 5f696e6c 2e68223a 3234352c alue_inl.h":245,
   0x0099abc0 20706c65 61736520 7265706f 72742061  please report a
   0x0099abd0 20627567 20746f20 5079546f 7263682e  bug to PyTorch.
   0x0099abe0 20005472 69656420 746f2063 61737420  .Tried to cast 
   0x0099abf0 61204c69 73743c00 3e20746f 2061204c a List<.> to a L
   0x0099ac00 6973743c 003e2e20 54797065 73206d69 ist<.>. Types mi
   0x0099ac10 736d6174 63682e00 746f5479 7065644c smatch..toTypedL
   0x0099ac20 69737400 00000000 2f676974 6875622f ist...../github/
   0x0099ac30 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x0099ac40 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x0099ac50 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x0099ac50 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x0099ac60 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x0099ac70 63682f69 6e636c75 64652f41 54656e2f ch/include/ATen/
   0x0099ac80 636f7265 2f4c6973 745f696e 6c2e6800 core/List_inl.h.
   0x0099ac90 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x0099aca0 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x0099acb0 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x0099acc0 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x0099acc0 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x0099acd0 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x0099ace0 64652f41 54656e2f 636f7265 2f626f78 de/ATen/core/box
   0x0099acf0 696e672f 4b65726e 656c4675 6e637469 ing/KernelFuncti
   0x0099ad00 6f6e5f69 6d706c2e 68000000 00000000 on_impl.h.......
   0x0099ad10 45787065 63746564 20707472 5f2d3e69 Expected ptr_->i
   0x0099ad20 735f666c 6f617428 2920746f 20626520 s_float() to be 
   0x0099ad30 74727565 2c206275 7420676f 74206661 true, but got fa
@@ -14553,24 +14553,24 @@
   0x0099ad60 62652069 6d70726f 7665643f 20204966 be improved?  If
   0x0099ad70 20736f2c 20706c65 61736520 7265706f  so, please repo
   0x0099ad80 72742061 6e20656e 68616e63 656d656e rt an enhancemen
   0x0099ad90 74207265 71756573 7420746f 20507954 t request to PyT
   0x0099ada0 6f726368 2e290000 2f676974 6875622f orch.)../github/
   0x0099adb0 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x0099adc0 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x0099add0 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x0099add0 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x0099ade0 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x0099adf0 63682f69 6e636c75 64652f63 31302f63 ch/include/c10/c
   0x0099ae00 6f72652f 53796d46 6c6f6174 2e680000 ore/SymFloat.h..
   0x0099ae10 3020494e 5445524e 414c2041 53534552 0 INTERNAL ASSER
   0x0099ae20 54204641 494c4544 20617420 222f6769 T FAILED at "/gi
   0x0099ae30 74687562 2f686f6d 652f6d69 6e69636f thub/home/minico
   0x0099ae40 6e64612f 656e7673 2f627569 6c645f62 nda/envs/build_b
   0x0099ae50 696e6172 792f6c69 622f7079 74686f6e inary/lib/python
-  0x0099ae60 332e392f 73697465 2d706163 6b616765 3.9/site-package
+  0x0099ae60 332e382f 73697465 2d706163 6b616765 3.8/site-package
   0x0099ae70 732f746f 7263682f 696e636c 7564652f s/torch/include/
   0x0099ae80 4154656e 2f636f72 652f6976 616c7565 ATen/core/ivalue
   0x0099ae90 2e68223a 3534302c 20706c65 61736520 .h":540, please 
   0x0099aea0 7265706f 72742061 20627567 20746f20 report a bug to 
   0x0099aeb0 5079546f 7263682e 20006578 70656374 PyTorch. .expect
   0x0099aec0 65642064 6f75626c 6500746f 446f7562 ed double.toDoub
   0x0099aed0 6c650000 00000000 00000000 00000000 le..............
@@ -16036,15 +16036,15 @@
   0x009a0a10 6a616767 65645f69 6e646578 5f616464 jagged_index_add
   0x009a0a20 5f32645f 666f7277 61726400 00000000 _2d_forward.....
   0x009a0a30 6973496e 744c6973 74282920 494e5445 isIntList() INTE
   0x009a0a40 524e414c 20415353 45525420 4641494c RNAL ASSERT FAIL
   0x009a0a50 45442061 7420222f 67697468 75622f68 ED at "/github/h
   0x009a0a60 6f6d652f 6d696e69 636f6e64 612f656e ome/miniconda/en
   0x009a0a70 76732f62 75696c64 5f62696e 6172792f vs/build_binary/
-  0x009a0a80 6c69622f 70797468 6f6e332e 392f7369 lib/python3.9/si
+  0x009a0a80 6c69622f 70797468 6f6e332e 382f7369 lib/python3.8/si
   0x009a0a90 74652d70 61636b61 6765732f 746f7263 te-packages/torc
   0x009a0aa0 682f696e 636c7564 652f4154 656e2f63 h/include/ATen/c
   0x009a0ab0 6f72652f 6976616c 75655f69 6e6c2e68 ore/ivalue_inl.h
   0x009a0ac0 223a3139 36322c20 706c6561 73652072 ":1962, please r
   0x009a0ad0 65706f72 74206120 62756720 746f2050 eport a bug to P
   0x009a0ae0 79546f72 63682e20 00000000 00000000 yTorch. ........
   0x009a0af0 464e3261 74365465 6e736f72 45524b53 FN2at6TensorERKS
@@ -20253,15 +20253,15 @@
   0x009b11a0 726f7665 643f2020 49662073 6f2c2070 roved?  If so, p
   0x009b11b0 6c656173 65207265 706f7274 20616e20 lease report an 
   0x009b11c0 656e6861 6e63656d 656e7420 72657175 enhancement requ
   0x009b11d0 65737420 746f2050 79546f72 63682e29 est to PyTorch.)
   0x009b11e0 00000000 00000000 2f5f5f77 2f464247 ......../__w/FBG
   0x009b11f0 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x009b1200 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x009b1210 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x009b1210 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x009b1220 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x009b1230 656d6265 6464696e 675f666f 72776172 embedding_forwar
   0x009b1240 645f7175 616e7469 7a65645f 756e7765 d_quantized_unwe
   0x009b1250 69676874 65645f63 6f646567 656e5f63 ighted_codegen_c
   0x009b1260 70752e63 70700000 696e7438 206f7574 pu.cpp..int8 out
   0x009b1270 70757420 61726520 6f6e6c79 20737570 put are only sup
   0x009b1280 706f7274 65642066 6f722069 6e743820 ported for int8 
@@ -20394,15 +20394,15 @@
   0x009b1a70 38c1f2ff 28c1f2ff 18c1f2ff 08c1f2ff 8...(...........
   0x009b1a80 78c2f2ff 68c2f2ff 58c2f2ff 48c2f2ff x...h...X...H...
   0x009b1a90 78c1f2ff 68c1f2ff 58c1f2ff 48c1f2ff x...h...X...H...
   0x009b1aa0 d8c0f2ff c8c0f2ff e8c0f2ff 06050010 ................
   0x009b1ab0 110f0000 00000000 2f5f5f77 2f464247 ......../__w/FBG
   0x009b1ac0 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x009b1ad0 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x009b1ae0 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x009b1ae0 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x009b1af0 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x009b1b00 656d6265 6464696e 675f666f 72776172 embedding_forwar
   0x009b1b10 645f7175 616e7469 7a65645f 77656967 d_quantized_weig
   0x009b1b20 68746564 5f636f64 6567656e 5f637075 hted_codegen_cpu
   0x009b1b30 2e637070 00000000 7072756e 65645f68 .cpp....pruned_h
   0x009b1b40 6173686d 61705f6c 6f6f6b75 705f7765 ashmap_lookup_we
   0x009b1b50 69676874 65645f63 70750000 00000000 ighted_cpu......
@@ -20416,15 +20416,15 @@
   0x009b1bd0 75737420 62652065 6d707479 206f7220 ust be empty or 
   0x009b1be0 61204350 55207465 6e736f72 3b206974 a CPU tensor; it
   0x009b1bf0 20697320 63757272 656e746c 79206f6e  is currently on
   0x009b1c00 20646576 69636520 00000000 00000000  device ........
   0x009b1c10 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x009b1c20 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x009b1c30 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x009b1c40 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x009b1c40 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x009b1c50 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x009b1c60 675f6261 636b7761 72645f64 656e7365 g_backward_dense
   0x009b1c70 5f73706c 69745f63 70752e63 70700000 _split_cpu.cpp..
   0x009b1c80 43686563 6b206661 696c6564 3a20686f Check failed: ho
   0x009b1c90 73745f77 65696768 74732e64 696d2829 st_weights.dim()
   0x009b1ca0 203d3d20 31202800 73706c69 745f656d  == 1 (.split_em
   0x009b1cb0 62656464 696e675f 6261636b 77617264 bedding_backward
@@ -20505,15 +20505,15 @@
   0x009b2160 70706572 00000000 73706c69 745f656d pper....split_em
   0x009b2170 62656464 696e675f 636f6465 67656e5f bedding_codegen_
   0x009b2180 666f7277 6172645f 756e7765 69676874 forward_unweight
   0x009b2190 65645f70 74325f77 72617070 65720000 ed_pt2_wrapper..
   0x009b21a0 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x009b21b0 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x009b21c0 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x009b21d0 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x009b21d0 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x009b21e0 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x009b21f0 675f666f 72776172 645f7370 6c69745f g_forward_split_
   0x009b2200 7074325f 6370755f 77726170 7065722e pt2_cpu_wrapper.
   0x009b2210 63707000 00000000 66626765 6d6d3a3a cpp.....fbgemm::
   0x009b2220 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009b2230 636f6465 67656e5f 67726164 5f696e64 codegen_grad_ind
   0x009b2240 6963655f 77656967 6874735f 63707500 ice_weights_cpu.
@@ -20644,15 +20644,15 @@
   0x009b2a10 3d302920 2d3e2054 656e736f 72000000 =0) -> Tensor...
   0x009b2a20 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009b2a30 636f6465 67656e5f 6c6f6f6b 75705f61 codegen_lookup_a
   0x009b2a40 64616772 61645f66 756e6374 696f6e5f dagrad_function_
   0x009b2a50 63707500 00000000 2f5f5f77 2f464247 cpu...../__w/FBG
   0x009b2a60 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x009b2a70 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x009b2a80 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x009b2a80 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x009b2a90 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x009b2aa0 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x009b2ab0 72645f73 706c6974 5f616461 67726164 rd_split_adagrad
   0x009b2ac0 5f637075 2e637070 00000000 00000000 _cpu.cpp........
   0x009b2ad0 66626765 6d6d3a3a 73706c69 745f656d fbgemm::split_em
   0x009b2ae0 62656464 696e675f 6261636b 77617264 bedding_backward
   0x009b2af0 5f636f64 6567656e 5f616461 67726164 _codegen_adagrad
@@ -20767,15 +20767,15 @@
   0x009b31c0 303af5ff 183af5ff 003af5ff e839f5ff 0:...:...:...9..
   0x009b31d0 d039f5ff b839f5ff a039f5ff 9039f5ff .9...9...9...9..
   0x009b31e0 8039f5ff 7039f5ff 6039f5ff 5039f5ff .9..p9..`9..P9..
   0x009b31f0 4039f5ff 1839f5ff 683bf5ff 00000000 @9...9..h;......
   0x009b3200 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x009b3210 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x009b3220 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x009b3230 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x009b3230 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x009b3240 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x009b3250 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x009b3260 5f616461 67726164 5f707432 5f637075 _adagrad_pt2_cpu
   0x009b3270 5f777261 70706572 2e637070 00000000 _wrapper.cpp....
   0x009b3280 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009b3290 6261636b 77617264 5f636f64 6567656e backward_codegen
   0x009b32a0 5f616461 67726164 5f776569 67687465 _adagrad_weighte
@@ -20889,15 +20889,15 @@
   0x009b3960 00000000 00000000 73706c69 745f656d ........split_em
   0x009b3970 62656464 696e675f 636f6465 67656e5f bedding_codegen_
   0x009b3980 6c6f6f6b 75705f72 6f777769 73655f61 lookup_rowwise_a
   0x009b3990 64616772 61645f66 756e6374 696f6e5f dagrad_function_
   0x009b39a0 63707500 00000000 2f5f5f77 2f464247 cpu...../__w/FBG
   0x009b39b0 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x009b39c0 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x009b39d0 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x009b39d0 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x009b39e0 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x009b39f0 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x009b3a00 72645f73 706c6974 5f726f77 77697365 rd_split_rowwise
   0x009b3a10 5f616461 67726164 5f637075 2e637070 _adagrad_cpu.cpp
   0x009b3a20 00000000 00000000 66626765 6d6d3a3a ........fbgemm::
   0x009b3a30 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009b3a40 6261636b 77617264 5f636f64 6567656e backward_codegen
@@ -21017,15 +21017,15 @@
   0x009b4160 ec89f6ff d489f6ff bc89f6ff a489f6ff ................
   0x009b4170 8c89f6ff 7489f6ff 5c89f6ff 4489f6ff ....t...\...D...
   0x009b4180 2c89f6ff 1489f6ff 0489f6ff f488f6ff ,...............
   0x009b4190 e488f6ff d488f6ff c488f6ff b488f6ff ................
   0x009b41a0 8c88f6ff dc8af6ff 2f5f5f77 2f464247 ......../__w/FBG
   0x009b41b0 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x009b41c0 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x009b41d0 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x009b41d0 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x009b41e0 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x009b41f0 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x009b4200 72645f73 706c6974 5f726f77 77697365 rd_split_rowwise
   0x009b4210 5f616461 67726164 5f707432 5f637075 _adagrad_pt2_cpu
   0x009b4220 5f777261 70706572 2e637070 00000000 _wrapper.cpp....
   0x009b4230 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009b4240 6261636b 77617264 5f636f64 6567656e backward_codegen
@@ -21129,15 +21129,15 @@
   0x009b4860 745f6474 7970653d 3029202d 3e205465 t_dtype=0) -> Te
   0x009b4870 6e736f72 00000000 73706c69 745f656d nsor....split_em
   0x009b4880 62656464 696e675f 636f6465 67656e5f bedding_codegen_
   0x009b4890 6c6f6f6b 75705f73 67645f66 756e6374 lookup_sgd_funct
   0x009b48a0 696f6e5f 63707500 2f5f5f77 2f464247 ion_cpu./__w/FBG
   0x009b48b0 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x009b48c0 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x009b48d0 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x009b48d0 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x009b48e0 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x009b48f0 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x009b4900 72645f73 706c6974 5f736764 5f637075 rd_split_sgd_cpu
   0x009b4910 2e637070 00000000 66626765 6d6d3a3a .cpp....fbgemm::
   0x009b4920 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009b4930 6261636b 77617264 5f636f64 6567656e backward_codegen
   0x009b4940 5f736764 5f637075 00000000 00000000 _sgd_cpu........
@@ -21245,15 +21245,15 @@
   0x009b4fa0 30b9f7ff 18b9f7ff 00b9f7ff e8b8f7ff 0...............
   0x009b4fb0 d0b8f7ff b8b8f7ff a0b8f7ff 90b8f7ff ................
   0x009b4fc0 80b8f7ff 70b8f7ff 60b8f7ff 50b8f7ff ....p...`...P...
   0x009b4fd0 40b8f7ff 18b8f7ff 68baf7ff 00000000 @.......h.......
   0x009b4fe0 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x009b4ff0 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x009b5000 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x009b5010 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x009b5010 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x009b5020 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x009b5030 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x009b5040 5f736764 5f707432 5f637075 5f777261 _sgd_pt2_cpu_wra
   0x009b5050 70706572 2e637070 00000000 00000000 pper.cpp........
   0x009b5060 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009b5070 6261636b 77617264 5f636f64 6567656e backward_codegen
   0x009b5080 5f736764 5f776569 67687465 645f6578 _sgd_weighted_ex
@@ -21325,15 +21325,15 @@
   0x009b54a0 3a2f2f67 69746875 622e636f 6d2f7079 ://github.com/py
   0x009b54b0 746f7263 682f4642 47454d4d 2f646973 torch/FBGEMM/dis
   0x009b54c0 63757373 696f6e73 2f313732 3720666f cussions/1727 fo
   0x009b54d0 72206d6f 72652064 65746169 6c2e0000 r more detail...
   0x009b54e0 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x009b54f0 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x009b5500 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x009b5510 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x009b5510 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x009b5520 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x009b5530 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x009b5540 5f616461 6d5f6370 752e6370 70000000 _adam_cpu.cpp...
   0x009b5550 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009b5560 636f6465 67656e5f 6c6f6f6b 75705f61 codegen_lookup_a
   0x009b5570 64616d5f 66756e63 74696f6e 5f637075 dam_function_cpu
   0x009b5580 00000000 00000000 73706c69 745f656d ........split_em
@@ -21430,15 +21430,15 @@
   0x009b5b30 65652068 74747073 3a2f2f67 69746875 ee https://githu
   0x009b5b40 622e636f 6d2f7079 746f7263 682f4642 b.com/pytorch/FB
   0x009b5b50 47454d4d 2f646973 63757373 696f6e73 GEMM/discussions
   0x009b5b60 2f313732 3720666f 72206d6f 72652064 /1727 for more d
   0x009b5b70 65746169 6c2e0000 2f5f5f77 2f464247 etail.../__w/FBG
   0x009b5b80 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x009b5b90 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x009b5ba0 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x009b5ba0 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x009b5bb0 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x009b5bc0 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x009b5bd0 72645f73 706c6974 5f6c616d 625f6370 rd_split_lamb_cp
   0x009b5be0 752e6370 70000000 73706c69 745f656d u.cpp...split_em
   0x009b5bf0 62656464 696e675f 636f6465 67656e5f bedding_codegen_
   0x009b5c00 6c6f6f6b 75705f6c 616d625f 66756e63 lookup_lamb_func
   0x009b5c10 74696f6e 5f637075 00000000 00000000 tion_cpu........
@@ -21529,15 +21529,15 @@
   0x009b6160 3a2f2f67 69746875 622e636f 6d2f7079 ://github.com/py
   0x009b6170 746f7263 682f4642 47454d4d 2f646973 torch/FBGEMM/dis
   0x009b6180 63757373 696f6e73 2f313732 3720666f cussions/1727 fo
   0x009b6190 72206d6f 72652064 65746169 6c2e0000 r more detail...
   0x009b61a0 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x009b61b0 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x009b61c0 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x009b61d0 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x009b61d0 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x009b61e0 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x009b61f0 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x009b6200 5f706172 7469616c 5f726f77 77697365 _partial_rowwise
   0x009b6210 5f616461 6d5f6370 752e6370 70000000 _adam_cpu.cpp...
   0x009b6220 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009b6230 636f6465 67656e5f 6c6f6f6b 75705f70 codegen_lookup_p
   0x009b6240 61727469 616c5f72 6f777769 73655f61 artial_rowwise_a
@@ -21632,15 +21632,15 @@
   0x009b67d0 3a2f2f67 69746875 622e636f 6d2f7079 ://github.com/py
   0x009b67e0 746f7263 682f4642 47454d4d 2f646973 torch/FBGEMM/dis
   0x009b67f0 63757373 696f6e73 2f313732 3720666f cussions/1727 fo
   0x009b6800 72206d6f 72652064 65746169 6c2e0000 r more detail...
   0x009b6810 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x009b6820 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x009b6830 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x009b6840 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x009b6840 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x009b6850 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x009b6860 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x009b6870 5f706172 7469616c 5f726f77 77697365 _partial_rowwise
   0x009b6880 5f6c616d 625f6370 752e6370 70000000 _lamb_cpu.cpp...
   0x009b6890 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009b68a0 636f6465 67656e5f 6c6f6f6b 75705f70 codegen_lookup_p
   0x009b68b0 61727469 616c5f72 6f777769 73655f6c artial_rowwise_l
@@ -21735,15 +21735,15 @@
   0x009b6e40 74747073 3a2f2f67 69746875 622e636f ttps://github.co
   0x009b6e50 6d2f7079 746f7263 682f4642 47454d4d m/pytorch/FBGEMM
   0x009b6e60 2f646973 63757373 696f6e73 2f313732 /discussions/172
   0x009b6e70 3720666f 72206d6f 72652064 65746169 7 for more detai
   0x009b6e80 6c2e0000 00000000 2f5f5f77 2f464247 l......./__w/FBG
   0x009b6e90 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x009b6ea0 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x009b6eb0 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x009b6eb0 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x009b6ec0 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x009b6ed0 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x009b6ee0 72645f73 706c6974 5f6c6172 735f7367 rd_split_lars_sg
   0x009b6ef0 645f6370 752e6370 70000000 00000000 d_cpu.cpp.......
   0x009b6f00 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009b6f10 636f6465 67656e5f 6c6f6f6b 75705f6c codegen_lookup_l
   0x009b6f20 6172735f 7367645f 66756e63 74696f6e ars_sgd_function
@@ -21834,15 +21834,15 @@
   0x009b7470 3a2f2f67 69746875 622e636f 6d2f7079 ://github.com/py
   0x009b7480 746f7263 682f4642 47454d4d 2f646973 torch/FBGEMM/dis
   0x009b7490 63757373 696f6e73 2f313732 3720666f cussions/1727 fo
   0x009b74a0 72206d6f 72652064 65746169 6c2e0000 r more detail...
   0x009b74b0 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x009b74c0 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x009b74d0 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x009b74e0 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x009b74e0 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x009b74f0 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x009b7500 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x009b7510 5f6e6f6e 655f6370 752e6370 70000000 _none_cpu.cpp...
   0x009b7520 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009b7530 636f6465 67656e5f 6c6f6f6b 75705f6e codegen_lookup_n
   0x009b7540 6f6e655f 66756e63 74696f6e 5f637075 one_function_cpu
   0x009b7550 00000000 00000000 73706c69 745f656d ........split_em
@@ -21923,15 +21923,15 @@
   0x009b7a00 3a2f2f67 69746875 622e636f 6d2f7079 ://github.com/py
   0x009b7a10 746f7263 682f4642 47454d4d 2f646973 torch/FBGEMM/dis
   0x009b7a20 63757373 696f6e73 2f313732 3720666f cussions/1727 fo
   0x009b7a30 72206d6f 72652064 65746169 6c2e0000 r more detail...
   0x009b7a40 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x009b7a50 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x009b7a60 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x009b7a70 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x009b7a70 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x009b7a80 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x009b7a90 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x009b7aa0 5f726f77 77697365 5f616461 67726164 _rowwise_adagrad
   0x009b7ab0 5f776974 685f636f 756e7465 725f6370 _with_counter_cp
   0x009b7ac0 752e6370 70000000 73706c69 745f656d u.cpp...split_em
   0x009b7ad0 62656464 696e675f 636f6465 67656e5f bedding_codegen_
   0x009b7ae0 6c6f6f6b 75705f72 6f777769 73655f61 lookup_rowwise_a
@@ -22064,15 +22064,15 @@
   0x009b82d0 2f676974 6875622e 636f6d2f 7079746f /github.com/pyto
   0x009b82e0 7263682f 46424745 4d4d2f64 69736375 rch/FBGEMM/discu
   0x009b82f0 7373696f 6e732f31 37323720 666f7220 ssions/1727 for 
   0x009b8300 6d6f7265 20646574 61696c2e 00000000 more detail.....
   0x009b8310 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x009b8320 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x009b8330 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x009b8340 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x009b8340 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x009b8350 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x009b8360 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x009b8370 5f617070 726f785f 7367645f 6370752e _approx_sgd_cpu.
   0x009b8380 63707000 00000000 73706c69 745f656d cpp.....split_em
   0x009b8390 62656464 696e675f 636f6465 67656e5f bedding_codegen_
   0x009b83a0 6c6f6f6b 75705f61 7070726f 785f7367 lookup_approx_sg
   0x009b83b0 645f6675 6e637469 6f6e5f63 70750000 d_function_cpu..
@@ -22145,15 +22145,15 @@
   0x009b87e0 70733a2f 2f676974 6875622e 636f6d2f ps://github.com/
   0x009b87f0 7079746f 7263682f 46424745 4d4d2f64 pytorch/FBGEMM/d
   0x009b8800 69736375 7373696f 6e732f31 37323720 iscussions/1727 
   0x009b8810 666f7220 6d6f7265 20646574 61696c2e for more detail.
   0x009b8820 00000000 00000000 2f5f5f77 2f464247 ......../__w/FBG
   0x009b8830 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x009b8840 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x009b8850 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x009b8850 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x009b8860 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x009b8870 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x009b8880 72645f73 706c6974 5f617070 726f785f rd_split_approx_
   0x009b8890 726f7777 6973655f 61646167 7261645f rowwise_adagrad_
   0x009b88a0 6370752e 63707000 73706c69 745f656d cpu.cpp.split_em
   0x009b88b0 62656464 696e675f 636f6465 67656e5f bedding_codegen_
   0x009b88c0 6c6f6f6b 75705f61 7070726f 785f726f lookup_approx_ro
@@ -22248,15 +22248,15 @@
   0x009b8e50 2f2f6769 74687562 2e636f6d 2f707974 //github.com/pyt
   0x009b8e60 6f726368 2f464247 454d4d2f 64697363 orch/FBGEMM/disc
   0x009b8e70 75737369 6f6e732f 31373237 20666f72 ussions/1727 for
   0x009b8e80 206d6f72 65206465 7461696c 2e000000  more detail....
   0x009b8e90 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x009b8ea0 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x009b8eb0 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x009b8ec0 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x009b8ec0 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x009b8ed0 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x009b8ee0 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x009b8ef0 5f617070 726f785f 726f7777 6973655f _approx_rowwise_
   0x009b8f00 61646167 7261645f 77697468 5f636f75 adagrad_with_cou
   0x009b8f10 6e746572 5f637075 2e637070 00000000 nter_cpu.cpp....
   0x009b8f20 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009b8f30 636f6465 67656e5f 6c6f6f6b 75705f61 codegen_lookup_a
@@ -22384,15 +22384,15 @@
   0x009b96d0 69746875 622e636f 6d2f7079 746f7263 ithub.com/pytorc
   0x009b96e0 682f4642 47454d4d 2f646973 63757373 h/FBGEMM/discuss
   0x009b96f0 696f6e73 2f313732 3720666f 72206d6f ions/1727 for mo
   0x009b9700 72652064 65746169 6c2e0000 00000000 re detail.......
   0x009b9710 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x009b9720 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x009b9730 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x009b9740 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x009b9740 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x009b9750 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x009b9760 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x009b9770 5f617070 726f785f 726f7777 6973655f _approx_rowwise_
   0x009b9780 61646167 7261645f 77697468 5f776569 adagrad_with_wei
   0x009b9790 6768745f 64656361 795f6370 752e6370 ght_decay_cpu.cp
   0x009b97a0 70000000 00000000 73706c69 745f656d p.......split_em
   0x009b97b0 62656464 696e675f 636f6465 67656e5f bedding_codegen_
@@ -22484,15 +22484,15 @@
   0x009b9d10 68747470 733a2f2f 67697468 75622e63 https://github.c
   0x009b9d20 6f6d2f70 79746f72 63682f46 4247454d om/pytorch/FBGEM
   0x009b9d30 4d2f6469 73637573 73696f6e 732f3137 M/discussions/17
   0x009b9d40 32372066 6f72206d 6f726520 64657461 27 for more deta
   0x009b9d50 696c2e00 00000000 2f5f5f77 2f464247 il....../__w/FBG
   0x009b9d60 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x009b9d70 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x009b9d80 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x009b9d80 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x009b9d90 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x009b9da0 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x009b9db0 72645f73 706c6974 5f726f77 77697365 rd_split_rowwise
   0x009b9dc0 5f616461 67726164 5f776974 685f7765 _adagrad_with_we
   0x009b9dd0 69676874 5f646563 61795f63 70752e63 ight_decay_cpu.c
   0x009b9de0 70700000 00000000 73706c69 745f656d pp......split_em
   0x009b9df0 62656464 696e675f 636f6465 67656e5f bedding_codegen_
@@ -22583,15 +22583,15 @@
   0x009ba340 74747073 3a2f2f67 69746875 622e636f ttps://github.co
   0x009ba350 6d2f7079 746f7263 682f4642 47454d4d m/pytorch/FBGEMM
   0x009ba360 2f646973 63757373 696f6e73 2f313732 /discussions/172
   0x009ba370 3720666f 72206d6f 72652064 65746169 7 for more detai
   0x009ba380 6c2e0000 00000000 2f5f5f77 2f464247 l......./__w/FBG
   0x009ba390 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x009ba3a0 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x009ba3b0 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x009ba3b0 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x009ba3c0 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x009ba3d0 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x009ba3e0 72645f73 706c6974 5f726f77 77697365 rd_split_rowwise
   0x009ba3f0 5f776569 67687465 645f6164 61677261 _weighted_adagra
   0x009ba400 645f6370 752e6370 70000000 00000000 d_cpu.cpp.......
   0x009ba410 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009ba420 636f6465 67656e5f 6c6f6f6b 75705f72 codegen_lookup_r
@@ -22684,15 +22684,15 @@
   0x009ba990 086df9ff f06cf9ff d86cf9ff c06cf9ff .m...l...l...l..
   0x009ba9a0 a86cf9ff 906cf9ff 786cf9ff 606cf9ff .l...l..xl..`l..
   0x009ba9b0 486cf9ff 386cf9ff 286cf9ff 186cf9ff Hl..8l..(l...l..
   0x009ba9c0 086cf9ff f86bf9ff e86bf9ff c06bf9ff .l...k...k...k..
   0x009ba9d0 106ef9ff 00000000 2f5f5f77 2f464247 .n....../__w/FBG
   0x009ba9e0 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x009ba9f0 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x009baa00 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x009baa00 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x009baa10 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x009baa20 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x009baa30 72645f61 64616772 61645f73 706c6974 rd_adagrad_split
   0x009baa40 5f637075 2e637070 00000000 00000000 _cpu.cpp........
   0x009baa50 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009baa60 6261636b 77617264 5f657861 63745f63 backward_exact_c
   0x009baa70 70755f6f 75746572 00000000 00000000 pu_outer........
@@ -22771,15 +22771,15 @@
   0x009baf00 28f1f9ff 18f1f9ff 08f1f9ff e0f0f9ff (...............
   0x009baf10 30f3f9ff 00000000 6e756d20 6f662072 0.......num of r
   0x009baf20 6f777320 70726f63 65737365 64206279 ows processed by
   0x009baf30 20616461 67726164 3a200000 00000000  adagrad: ......
   0x009baf40 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x009baf50 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x009baf60 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x009baf70 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x009baf70 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x009baf80 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x009baf90 675f6261 636b7761 72645f72 6f777769 g_backward_rowwi
   0x009bafa0 73655f61 64616772 61645f73 706c6974 se_adagrad_split
   0x009bafb0 5f637075 2e637070 00000000 00000000 _cpu.cpp........
   0x009bafc0 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009bafd0 6261636b 77617264 5f636f64 6567656e backward_codegen
   0x009bafe0 5f726f77 77697365 5f616461 67726164 _rowwise_adagrad
@@ -22851,15 +22851,15 @@
   0x009bb400 7c54faff 6454faff 4c54faff 3454faff |T..dT..LT..4T..
   0x009bb410 1c54faff 0454faff ec53faff d453faff .T...T...S...S..
   0x009bb420 bc53faff a453faff 9453faff 8453faff .S...S...S...S..
   0x009bb430 7453faff 6453faff 5453faff 4453faff tS..dS..TS..DS..
   0x009bb440 1c53faff 6c55faff 2f5f5f77 2f464247 .S..lU../__w/FBG
   0x009bb450 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x009bb460 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x009bb470 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x009bb470 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x009bb480 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x009bb490 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x009bb4a0 72645f73 67645f73 706c6974 5f637075 rd_sgd_split_cpu
   0x009bb4b0 2e637070 00000000 73706c69 745f656d .cpp....split_em
   0x009bb4c0 62656464 696e675f 6261636b 77617264 bedding_backward
   0x009bb4d0 5f636f64 6567656e 5f736764 5f637075 _codegen_sgd_cpu
   0x009bb4e0 2854656e 736f7220 67726164 5f6f7574 (Tensor grad_out
```

## fbgemm_gpu/docs/version.py

```diff
@@ -2,8 +2,8 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
-__version__: str = "2024.5.29"
+__version__: str = "2024.5.30"
```

## Comparing `fbgemm_gpu_nightly_cpu-2024.5.29.dist-info/METADATA` & `fbgemm_gpu_nightly_cpu-2024.5.30.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fbgemm_gpu_nightly-cpu
-Version: 2024.5.29
+Version: 2024.5.30
 Home-page: https://github.com/pytorch/fbgemm
 Author: FBGEMM Team
 Author-email: packages@pytorch.org
 License: BSD-3
 Keywords: PyTorch,Recommendation Models,High Performance Computing,GPU,CUDA
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

## Comparing `fbgemm_gpu_nightly_cpu-2024.5.29.dist-info/RECORD` & `fbgemm_gpu_nightly_cpu-2024.5.30.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 fbgemm_gpu/__init__.py,sha256=plInYJM4Eqp01xDgYvEdYAYLy9btsh6_mTqqmXysarc,1342
 fbgemm_gpu/batched_unary_embeddings_ops.py,sha256=dpxZAueNsadJVuK7Dwo8GbOlho9r67Lfh8kesqRKJNI,3079
 fbgemm_gpu/enums.py,sha256=GVuzF5cFTLzttkvlH1SdcGrxrppMhDSbQj_Vm_4zmEo,789
-fbgemm_gpu/fbgemm_gpu_py.so,sha256=GdIOLv63e42PxzcZ8aSF5PTn27C0kS3TgaViaJFqQM8,10953528
+fbgemm_gpu/fbgemm_gpu_py.so,sha256=Ebm_yNEy_gjndaEk1L05YONkWD8RWCi-iDTvLZ4G8yo,10953528
 fbgemm_gpu/metrics.py,sha256=TsurFLJf0nJvPDN7urWb4LMQlf5RgdWPTTTDO7S4wtI,5663
 fbgemm_gpu/permute_pooled_embedding_modules.py,sha256=4mHJ2fo3SeG25iSwdm2YsM8q_oWsF1LxRguYmxSnuDI,2362
 fbgemm_gpu/permute_pooled_embedding_modules_split.py,sha256=cUrEbRIvLFW_3Zmh07QkN4S1Cfvvge6TYO1VXBFCpz8,2752
 fbgemm_gpu/quantize_comm.py,sha256=UZcVSC2JQ0oSkwsJQnjaZ2k8mm2p3hvVzpyg7X5xFXM,7885
 fbgemm_gpu/quantize_utils.py,sha256=TmlA7g74cxhP0TEbrNOgpR2TOYmfMc_LiDMVCYa-Sw4,4020
 fbgemm_gpu/runtime_monitor.py,sha256=tIdxkJIWkJ8705btxs9NqzEXC7QprFh3sA8Q4LpvtJ8,6947
 fbgemm_gpu/sparse_ops.py,sha256=qT3oBNOgu3YDwerFWS9RdC0TW9Dvh8M_CrBC_YgNvUM,32634
@@ -20,15 +20,15 @@
 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py,sha256=A7GLMdnH19AxCK9bgPNcHhNYvtRQ9ty6EI7bL40pUs0,44844
 fbgemm_gpu/uvm.py,sha256=-cZunsuvnAKUEQptIwdYVar_3hUE99FbQUsyfBVeXPE,925
 fbgemm_gpu/docs/__init__.py,sha256=Rh8Kn4L7LJRqCFWILZD7wReoBy8ZD2R_TfEzWHVCoA0,419
 fbgemm_gpu/docs/common.py,sha256=8ipXTwVb222X-aZ71O6n8fhxHCHPNhJEHMFiO7epcIs,273
 fbgemm_gpu/docs/examples.py,sha256=ZMN_6sL74LH_hrp2bF_hmg8gi29GhcgvwV3kCMjxkoE,2377
 fbgemm_gpu/docs/jagged_tensor_ops.py,sha256=Bsx-ZxvvdMv5CaldSvuw9GPR-HRcLbRR2IEXCOCm9r0,7381
 fbgemm_gpu/docs/table_batched_embedding_ops.py,sha256=h_EQOIMsdVlr-Pygul-fDGxx7JqLRjaBMI_z0PFrGAE,7708
-fbgemm_gpu/docs/version.py,sha256=QjQAiyBnyVYyWE6MX7oW7hgBsqwB26Zg7UXUCNjLBJE,264
+fbgemm_gpu/docs/version.py,sha256=Viq7phulDE3MVhhW8zXUPeSjn9VxFDxlLQg6JADRH4c,264
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py,sha256=zjUGbYZIC0yGtsNCPoCbTZ0-_Nj0Pd_yqHiRWTKeuT8,1964
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py,sha256=eHXy3WvsqeDDAAG2IKQKW-TYKtkO7rwqqaa-ypPK19w,4181
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad_pt2.py,sha256=eHXy3WvsqeDDAAG2IKQKW-TYKtkO7rwqqaa-ypPK19w,4181
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py,sha256=npe6C60ZLb3oWCni9OCfNYty22Lrw4br_7x8hG4IEcw,3396
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam_pt2.py,sha256=npe6C60ZLb3oWCni9OCfNYty22Lrw4br_7x8hG4IEcw,3396
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py,sha256=iaVc4tedyUEfN-TDKYu2jgcUEgHcCA5O9gw2H4uNBBA,2153
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args_ssd.py,sha256=VVJhaeY78p2LYRWejF_CI17VWJ58vbNJBAPIrlrITdU,2194
@@ -50,11 +50,11 @@
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py,sha256=kmd4ezZHdWF7TWI4V_SUUv04prmu_Hq_CvzslCIEawc,3763
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd_pt2.py,sha256=kmd4ezZHdWF7TWI4V_SUUv04prmu_Hq_CvzslCIEawc,3763
 fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py,sha256=yiD3_bG5yT5VXLoGw4eeRKQ2Nj087DRq0qKCVPb52SY,649
 fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py,sha256=OFw5PM2YDiKvr6T9ZW7BKiq58gB7txcKfuJkBUROxdI,6162
 fbgemm_gpu/tbe/__init__.py,sha256=fE0IHi1JJpxsNVBNzWNee2thrNXFFRhY94c80RxNSIE,231
 fbgemm_gpu/tbe/cache/__init__.py,sha256=kueJp-xYnDflz4DYf7dh5_xtx5ItzrbQc_1neoe5XQc,308
 fbgemm_gpu/tbe/cache/split_embeddings_cache_ops.py,sha256=F2XIec8Kgcihy1vXJRp0tQErqIQSQIDZRuzLfkasE70,1660
-fbgemm_gpu_nightly_cpu-2024.5.29.dist-info/METADATA,sha256=VdbQrcxDE2PtY7xRBs3NcuqpgquQdYbnMgT4Y7k2H98,2602
-fbgemm_gpu_nightly_cpu-2024.5.29.dist-info/WHEEL,sha256=AdAOsf8BL1uIBxiEcIdcPDjJWWb0G5USb4X4msVaesE,105
-fbgemm_gpu_nightly_cpu-2024.5.29.dist-info/top_level.txt,sha256=2tlbTWLkPjhqvLF_6BbqKzkcPluSE-oPRVjI8axK76I,11
-fbgemm_gpu_nightly_cpu-2024.5.29.dist-info/RECORD,,
+fbgemm_gpu_nightly_cpu-2024.5.30.dist-info/METADATA,sha256=zee9nV0Uej7_T51STlLzPxr03ViovH3wp1IcFXjbUVI,2602
+fbgemm_gpu_nightly_cpu-2024.5.30.dist-info/WHEEL,sha256=OEmkRrFcnutAqrz0YyBUaC3hh1288y58dKLCWma58N0,105
+fbgemm_gpu_nightly_cpu-2024.5.30.dist-info/top_level.txt,sha256=2tlbTWLkPjhqvLF_6BbqKzkcPluSE-oPRVjI8axK76I,11
+fbgemm_gpu_nightly_cpu-2024.5.30.dist-info/RECORD,,
```

