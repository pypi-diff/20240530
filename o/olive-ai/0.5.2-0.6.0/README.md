# Comparing `tmp/olive_ai-0.5.2-py3-none-any.whl.zip` & `tmp/olive_ai-0.6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,246 +1,263 @@
-Zip file size: 517025 bytes, number of entries: 244
--rw-rw-r--  2.0 unx      608 b- defN 24-Apr-11 05:46 olive/__init__.py
--rw-rw-r--  2.0 unx     9998 b- defN 24-Apr-11 05:46 olive/cache.py
--rw-rw-r--  2.0 unx     1162 b- defN 24-Apr-11 05:46 olive/constants.py
--rw-rw-r--  2.0 unx     2626 b- defN 24-Apr-11 05:46 olive/logging.py
--rw-rw-r--  2.0 unx     8038 b- defN 24-Apr-11 05:46 olive/olive_config.json
--rw-rw-r--  2.0 unx     1406 b- defN 24-Apr-11 05:46 olive/package_config.py
--rw-rw-r--  2.0 unx    22999 b- defN 24-Apr-11 05:46 olive/resource_path.py
--rw-rw-r--  2.0 unx     5181 b- defN 24-Apr-11 05:46 olive/auto_optimizer/__init__.py
--rw-rw-r--  2.0 unx     5871 b- defN 24-Apr-11 05:46 olive/auto_optimizer/regulate_mixins.py
--rw-rw-r--  2.0 unx     3615 b- defN 24-Apr-11 05:46 olive/auto_optimizer/template_mapping.py
--rw-rw-r--  2.0 unx     1171 b- defN 24-Apr-11 05:46 olive/auto_optimizer/config_template/opt_level_passes.yaml
--rw-rw-r--  2.0 unx     2062 b- defN 24-Apr-11 05:46 olive/auto_optimizer/config_template/pass_capability.yaml
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/azureml/__init__.py
--rw-rw-r--  2.0 unx     6699 b- defN 24-Apr-11 05:46 olive/azureml/azureml_client.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/common/__init__.py
--rw-rw-r--  2.0 unx     3430 b- defN 24-Apr-11 05:46 olive/common/auto_config.py
--rw-rw-r--  2.0 unx    10881 b- defN 24-Apr-11 05:46 olive/common/config_utils.py
--rw-rw-r--  2.0 unx     1488 b- defN 24-Apr-11 05:46 olive/common/import_lib.py
--rw-rw-r--  2.0 unx    18360 b- defN 24-Apr-11 05:46 olive/common/ort_inference.py
--rw-rw-r--  2.0 unx      765 b- defN 24-Apr-11 05:46 olive/common/pydantic_v1.py
--rw-rw-r--  2.0 unx     1809 b- defN 24-Apr-11 05:46 olive/common/user_module_loader.py
--rw-rw-r--  2.0 unx    11789 b- defN 24-Apr-11 05:46 olive/common/utils.py
--rw-rw-r--  2.0 unx      345 b- defN 24-Apr-11 05:46 olive/data/__init__.py
--rw-rw-r--  2.0 unx    10680 b- defN 24-Apr-11 05:46 olive/data/config.py
--rw-rw-r--  2.0 unx     1443 b- defN 24-Apr-11 05:46 olive/data/constants.py
--rw-rw-r--  2.0 unx     8119 b- defN 24-Apr-11 05:46 olive/data/registry.py
--rw-rw-r--  2.0 unx     3573 b- defN 24-Apr-11 05:46 olive/data/template.py
--rw-rw-r--  2.0 unx      444 b- defN 24-Apr-11 05:46 olive/data/component/__init__.py
--rw-rw-r--  2.0 unx     1955 b- defN 24-Apr-11 05:46 olive/data/component/dataloader.py
--rw-rw-r--  2.0 unx    10679 b- defN 24-Apr-11 05:46 olive/data/component/dataset.py
--rw-rw-r--  2.0 unx     1928 b- defN 24-Apr-11 05:46 olive/data/component/load_dataset.py
--rw-rw-r--  2.0 unx     2256 b- defN 24-Apr-11 05:46 olive/data/component/post_process_data.py
--rw-rw-r--  2.0 unx    11446 b- defN 24-Apr-11 05:46 olive/data/component/pre_process_data.py
--rw-rw-r--  2.0 unx    29278 b- defN 24-Apr-11 05:46 olive/data/component/text_generation.py
--rw-rw-r--  2.0 unx      480 b- defN 24-Apr-11 05:46 olive/data/container/__init__.py
--rw-rw-r--  2.0 unx     3385 b- defN 24-Apr-11 05:46 olive/data/container/data_container.py
--rw-rw-r--  2.0 unx     1159 b- defN 24-Apr-11 05:46 olive/data/container/dummy_data_container.py
--rw-rw-r--  2.0 unx     1690 b- defN 24-Apr-11 05:46 olive/data/container/huggingface_container.py
--rw-rw-r--  2.0 unx     1721 b- defN 24-Apr-11 05:46 olive/data/container/raw_data_container.py
--rw-rw-r--  2.0 unx      442 b- defN 24-Apr-11 05:46 olive/engine/__init__.py
--rw-rw-r--  2.0 unx     1199 b- defN 24-Apr-11 05:46 olive/engine/config.py
--rw-rw-r--  2.0 unx    45969 b- defN 24-Apr-11 05:46 olive/engine/engine.py
--rw-rw-r--  2.0 unx    17410 b- defN 24-Apr-11 05:46 olive/engine/footprint.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/engine/packaging/__init__.py
--rw-rw-r--  2.0 unx     1642 b- defN 24-Apr-11 05:46 olive/engine/packaging/packaging_config.py
--rw-rw-r--  2.0 unx    19748 b- defN 24-Apr-11 05:46 olive/engine/packaging/packaging_generator.py
--rw-rw-r--  2.0 unx     1588 b- defN 24-Apr-11 05:46 olive/engine/packaging/sample_code/ONNXModel/cpp/README.md
--rw-rw-r--  2.0 unx     4990 b- defN 24-Apr-11 05:46 olive/engine/packaging/sample_code/ONNXModel/cpp/code_sample.cpp
--rw-rw-r--  2.0 unx     1590 b- defN 24-Apr-11 05:46 olive/engine/packaging/sample_code/ONNXModel/cs/README.md
--rw-rw-r--  2.0 unx     4991 b- defN 24-Apr-11 05:46 olive/engine/packaging/sample_code/ONNXModel/cs/code_sample.cs
--rw-rw-r--  2.0 unx     2296 b- defN 24-Apr-11 05:46 olive/engine/packaging/sample_code/ONNXModel/python/README.md
--rw-rw-r--  2.0 unx     2545 b- defN 24-Apr-11 05:46 olive/engine/packaging/sample_code/ONNXModel/python/code_sample.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/evaluator/__init__.py
--rw-rw-r--  2.0 unx     6473 b- defN 24-Apr-11 05:46 olive/evaluator/accuracy.py
--rw-rw-r--  2.0 unx     8723 b- defN 24-Apr-11 05:46 olive/evaluator/metric.py
--rw-rw-r--  2.0 unx     4461 b- defN 24-Apr-11 05:46 olive/evaluator/metric_backend.py
--rw-rw-r--  2.0 unx     4395 b- defN 24-Apr-11 05:46 olive/evaluator/metric_config.py
--rw-rw-r--  2.0 unx    47694 b- defN 24-Apr-11 05:46 olive/evaluator/olive_evaluator.py
--rw-rw-r--  2.0 unx      592 b- defN 24-Apr-11 05:46 olive/exception/__init__.py
--rw-rw-r--  2.0 unx      621 b- defN 24-Apr-11 05:46 olive/hardware/__init__.py
--rw-rw-r--  2.0 unx    15059 b- defN 24-Apr-11 05:46 olive/hardware/accelerator.py
--rw-rw-r--  2.0 unx     1273 b- defN 24-Apr-11 05:46 olive/hardware/constants.py
--rw-rw-r--  2.0 unx      451 b- defN 24-Apr-11 05:46 olive/model/__init__.py
--rw-rw-r--  2.0 unx      482 b- defN 24-Apr-11 05:46 olive/model/config/__init__.py
--rw-rw-r--  2.0 unx    10950 b- defN 24-Apr-11 05:46 olive/model/config/hf_config.py
--rw-rw-r--  2.0 unx     4843 b- defN 24-Apr-11 05:46 olive/model/config/io_config.py
--rw-rw-r--  2.0 unx     3943 b- defN 24-Apr-11 05:46 olive/model/config/model_config.py
--rw-rw-r--  2.0 unx     1045 b- defN 24-Apr-11 05:46 olive/model/config/registry.py
--rw-rw-r--  2.0 unx     1139 b- defN 24-Apr-11 05:46 olive/model/handler/__init__.py
--rw-rw-r--  2.0 unx     3190 b- defN 24-Apr-11 05:46 olive/model/handler/base.py
--rw-rw-r--  2.0 unx     4461 b- defN 24-Apr-11 05:46 olive/model/handler/composite.py
--rw-rw-r--  2.0 unx    10069 b- defN 24-Apr-11 05:46 olive/model/handler/onnx.py
--rw-rw-r--  2.0 unx     3556 b- defN 24-Apr-11 05:46 olive/model/handler/openvino.py
--rw-rw-r--  2.0 unx    16898 b- defN 24-Apr-11 05:46 olive/model/handler/pytorch.py
--rw-rw-r--  2.0 unx     4704 b- defN 24-Apr-11 05:46 olive/model/handler/qnn.py
--rw-rw-r--  2.0 unx     2597 b- defN 24-Apr-11 05:46 olive/model/handler/snpe.py
--rw-rw-r--  2.0 unx     1474 b- defN 24-Apr-11 05:46 olive/model/handler/tensorflow.py
--rw-rw-r--  2.0 unx      936 b- defN 24-Apr-11 05:46 olive/model/handler/mixin/__init__.py
--rw-rw-r--  2.0 unx      418 b- defN 24-Apr-11 05:46 olive/model/handler/mixin/composite.py
--rw-rw-r--  2.0 unx     3021 b- defN 24-Apr-11 05:46 olive/model/handler/mixin/dummy_inputs.py
--rw-rw-r--  2.0 unx     3967 b- defN 24-Apr-11 05:46 olive/model/handler/mixin/hf_config.py
--rw-rw-r--  2.0 unx      613 b- defN 24-Apr-11 05:46 olive/model/handler/mixin/io_config.py
--rw-rw-r--  2.0 unx     1472 b- defN 24-Apr-11 05:46 olive/model/handler/mixin/json.py
--rw-rw-r--  2.0 unx     1402 b- defN 24-Apr-11 05:46 olive/model/handler/mixin/onnx_ep.py
--rw-rw-r--  2.0 unx     3946 b- defN 24-Apr-11 05:46 olive/model/handler/mixin/onnx_graph.py
--rw-rw-r--  2.0 unx     2998 b- defN 24-Apr-11 05:46 olive/model/handler/mixin/resource.py
--rw-rw-r--  2.0 unx      609 b- defN 24-Apr-11 05:46 olive/model/utils/__init__.py
--rw-rw-r--  2.0 unx     3091 b- defN 24-Apr-11 05:46 olive/model/utils/hf_mappings.py
--rw-rw-r--  2.0 unx     4517 b- defN 24-Apr-11 05:46 olive/model/utils/hf_onnx_config.py
--rw-rw-r--  2.0 unx     8183 b- defN 24-Apr-11 05:46 olive/model/utils/hf_utils.py
--rw-rw-r--  2.0 unx     3467 b- defN 24-Apr-11 05:46 olive/model/utils/onnx_utils.py
--rw-rw-r--  2.0 unx     1510 b- defN 24-Apr-11 05:46 olive/model/utils/path_utils.py
--rw-rw-r--  2.0 unx      499 b- defN 24-Apr-11 05:46 olive/passes/__init__.py
--rw-rw-r--  2.0 unx    19895 b- defN 24-Apr-11 05:46 olive/passes/olive_pass.py
--rw-rw-r--  2.0 unx     6139 b- defN 24-Apr-11 05:46 olive/passes/pass_config.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/passes/onnx/__init__.py
--rw-rw-r--  2.0 unx     8408 b- defN 24-Apr-11 05:46 olive/passes/onnx/append_pre_post_processing_ops.py
--rw-rw-r--  2.0 unx     5524 b- defN 24-Apr-11 05:46 olive/passes/onnx/bnb_quantization.py
--rw-rw-r--  2.0 unx     7639 b- defN 24-Apr-11 05:46 olive/passes/onnx/common.py
--rw-rw-r--  2.0 unx    27526 b- defN 24-Apr-11 05:46 olive/passes/onnx/conversion.py
--rw-rw-r--  2.0 unx     4862 b- defN 24-Apr-11 05:46 olive/passes/onnx/dynamic_to_fixed_shape.py
--rw-rw-r--  2.0 unx    14055 b- defN 24-Apr-11 05:46 olive/passes/onnx/extract_adapters.py
--rw-rw-r--  2.0 unx     3090 b- defN 24-Apr-11 05:46 olive/passes/onnx/float16_conversion.py
--rw-rw-r--  2.0 unx     4556 b- defN 24-Apr-11 05:46 olive/passes/onnx/genai_model_exporter.py
--rw-rw-r--  2.0 unx    27096 b- defN 24-Apr-11 05:46 olive/passes/onnx/inc_quantization.py
--rw-rw-r--  2.0 unx    15972 b- defN 24-Apr-11 05:46 olive/passes/onnx/insert_beam_search.py
--rw-rw-r--  2.0 unx    18495 b- defN 24-Apr-11 05:46 olive/passes/onnx/merge_decoders.py
--rw-rw-r--  2.0 unx     9054 b- defN 24-Apr-11 05:46 olive/passes/onnx/mixed_precision.py
--rw-rw-r--  2.0 unx    10011 b- defN 24-Apr-11 05:46 olive/passes/onnx/model_optimizer.py
--rw-rw-r--  2.0 unx    15752 b- defN 24-Apr-11 05:46 olive/passes/onnx/moe_experts_distributor.py
--rw-rw-r--  2.0 unx    18666 b- defN 24-Apr-11 05:46 olive/passes/onnx/onnx_dag.py
--rw-rw-r--  2.0 unx     6162 b- defN 24-Apr-11 05:46 olive/passes/onnx/optimum_conversion.py
--rw-rw-r--  2.0 unx     3709 b- defN 24-Apr-11 05:46 olive/passes/onnx/optimum_merging.py
--rw-rw-r--  2.0 unx    29003 b- defN 24-Apr-11 05:46 olive/passes/onnx/perf_tuning.py
--rw-rw-r--  2.0 unx     5375 b- defN 24-Apr-11 05:46 olive/passes/onnx/qnn_preprocess.py
--rw-rw-r--  2.0 unx    37566 b- defN 24-Apr-11 05:46 olive/passes/onnx/quantization.py
--rw-rw-r--  2.0 unx    19292 b- defN 24-Apr-11 05:46 olive/passes/onnx/transformer_optimization.py
--rw-rw-r--  2.0 unx    15105 b- defN 24-Apr-11 05:46 olive/passes/onnx/vitis_ai_quantization.py
--rw-rw-r--  2.0 unx     3239 b- defN 24-Apr-11 05:46 olive/passes/onnx/pipeline/__init__.py
--rw-rw-r--  2.0 unx     8457 b- defN 24-Apr-11 05:46 olive/passes/onnx/pipeline/step_utils.py
--rw-rw-r--  2.0 unx      508 b- defN 24-Apr-11 05:46 olive/passes/onnx/vitis_ai/__init__.py
--rw-rw-r--  2.0 unx     7762 b- defN 24-Apr-11 05:46 olive/passes/onnx/vitis_ai/calibrate.py
--rw-rw-r--  2.0 unx    15332 b- defN 24-Apr-11 05:46 olive/passes/onnx/vitis_ai/quant_utils.py
--rw-rw-r--  2.0 unx    13580 b- defN 24-Apr-11 05:46 olive/passes/onnx/vitis_ai/quantize.py
--rw-rw-r--  2.0 unx    36359 b- defN 24-Apr-11 05:46 olive/passes/onnx/vitis_ai/quantizer.py
--rw-rw-r--  2.0 unx    18700 b- defN 24-Apr-11 05:46 olive/passes/onnx/vitis_ai/refine.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/passes/openvino/__init__.py
--rw-rw-r--  2.0 unx     4555 b- defN 24-Apr-11 05:46 olive/passes/openvino/conversion.py
--rw-rw-r--  2.0 unx    12610 b- defN 24-Apr-11 05:46 olive/passes/openvino/quantization.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/passes/pytorch/__init__.py
--rw-rw-r--  2.0 unx     7058 b- defN 24-Apr-11 05:46 olive/passes/pytorch/cluster.py
--rw-rw-r--  2.0 unx     9842 b- defN 24-Apr-11 05:46 olive/passes/pytorch/gptq.py
--rw-rw-r--  2.0 unx    11528 b- defN 24-Apr-11 05:46 olive/passes/pytorch/gptq_utils.py
--rw-rw-r--  2.0 unx    48812 b- defN 24-Apr-11 05:46 olive/passes/pytorch/lora.py
--rw-rw-r--  2.0 unx     1021 b- defN 24-Apr-11 05:46 olive/passes/pytorch/pytorch_lightning_utils.py
--rw-rw-r--  2.0 unx     8038 b- defN 24-Apr-11 05:46 olive/passes/pytorch/qat_utils.py
--rw-rw-r--  2.0 unx     6444 b- defN 24-Apr-11 05:46 olive/passes/pytorch/quantization_aware_training.py
--rw-rw-r--  2.0 unx     7085 b- defN 24-Apr-11 05:46 olive/passes/pytorch/slicegpt.py
--rw-rw-r--  2.0 unx     9021 b- defN 24-Apr-11 05:46 olive/passes/pytorch/sparsegpt.py
--rw-rw-r--  2.0 unx    10774 b- defN 24-Apr-11 05:46 olive/passes/pytorch/sparsegpt_utils.py
--rw-rw-r--  2.0 unx     7032 b- defN 24-Apr-11 05:46 olive/passes/pytorch/tensor_parallel.py
--rw-rw-r--  2.0 unx     5372 b- defN 24-Apr-11 05:46 olive/passes/pytorch/tensor_parallel_layers.py
--rw-rw-r--  2.0 unx    17239 b- defN 24-Apr-11 05:46 olive/passes/pytorch/tensor_parallel_llama2.py
--rw-rw-r--  2.0 unx     8172 b- defN 24-Apr-11 05:46 olive/passes/pytorch/torch_trt_conversion.py
--rw-rw-r--  2.0 unx     3185 b- defN 24-Apr-11 05:46 olive/passes/pytorch/trt_utils.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/passes/qnn/__init__.py
--rw-rw-r--  2.0 unx     3192 b- defN 24-Apr-11 05:46 olive/passes/qnn/context_binary_generator.py
--rw-rw-r--  2.0 unx     5268 b- defN 24-Apr-11 05:46 olive/passes/qnn/conversion.py
--rw-rw-r--  2.0 unx     3298 b- defN 24-Apr-11 05:46 olive/passes/qnn/model_lib_generator.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/passes/snpe/__init__.py
--rw-rw-r--  2.0 unx     4802 b- defN 24-Apr-11 05:46 olive/passes/snpe/conversion.py
--rw-rw-r--  2.0 unx     5254 b- defN 24-Apr-11 05:46 olive/passes/snpe/quantization.py
--rw-rw-r--  2.0 unx     2637 b- defN 24-Apr-11 05:46 olive/passes/snpe/snpe_to_onnx.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/passes/utils/__init__.py
--rw-rw-r--  2.0 unx     1619 b- defN 24-Apr-11 05:46 olive/passes/utils/whisper_prepost.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/platform_sdk/__init__.py
--rw-rw-r--  2.0 unx      341 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/__init__.py
--rw-rw-r--  2.0 unx     3740 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/configure.py
--rw-rw-r--  2.0 unx     1348 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/constants.py
--rw-rw-r--  2.0 unx     1046 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/copy_libcdsprpc.ps1
--rw-rw-r--  2.0 unx     2387 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/create_python_env.ps1
--rw-rw-r--  2.0 unx     2431 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/create_python_env.sh
--rw-rw-r--  2.0 unx     4034 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/env.py
--rw-rw-r--  2.0 unx     3652 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/runner.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/qnn/__init__.py
--rw-rw-r--  2.0 unx     2034 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/qnn/env.py
--rw-rw-r--  2.0 unx     7269 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/qnn/qnn.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/qnn/utils/__init__.py
--rw-rw-r--  2.0 unx      396 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/snpe/__init__.py
--rw-rw-r--  2.0 unx     2117 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/snpe/env.py
--rw-rw-r--  2.0 unx     3969 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/snpe/snpe.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/snpe/tools/__init__.py
--rw-rw-r--  2.0 unx    10951 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/snpe/tools/dev.py
--rw-rw-r--  2.0 unx    19039 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/snpe/tools/inference.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/snpe/utils/__init__.py
--rw-rw-r--  2.0 unx     6978 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/snpe/utils/adb.py
--rw-rw-r--  2.0 unx      374 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/utils/__init__.py
--rw-rw-r--  2.0 unx    14746 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/utils/data_loader.py
--rw-rw-r--  2.0 unx     8878 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/utils/input_list.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/scripts/__init__.py
--rw-rw-r--  2.0 unx     3130 b- defN 24-Apr-11 05:46 olive/scripts/export_adapters.py
--rw-rw-r--  2.0 unx     6435 b- defN 24-Apr-11 05:46 olive/scripts/manage_compute_instance.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/strategy/__init__.py
--rw-rw-r--  2.0 unx    11837 b- defN 24-Apr-11 05:46 olive/strategy/search_parameter.py
--rw-rw-r--  2.0 unx     5631 b- defN 24-Apr-11 05:46 olive/strategy/search_results.py
--rw-rw-r--  2.0 unx     4702 b- defN 24-Apr-11 05:46 olive/strategy/search_space.py
--rw-rw-r--  2.0 unx    12873 b- defN 24-Apr-11 05:46 olive/strategy/search_strategy.py
--rw-rw-r--  2.0 unx     2817 b- defN 24-Apr-11 05:46 olive/strategy/utils.py
--rw-rw-r--  2.0 unx      705 b- defN 24-Apr-11 05:46 olive/strategy/search_algorithm/__init__.py
--rw-rw-r--  2.0 unx     1091 b- defN 24-Apr-11 05:46 olive/strategy/search_algorithm/exhaustive.py
--rw-rw-r--  2.0 unx     4334 b- defN 24-Apr-11 05:46 olive/strategy/search_algorithm/optuna_sampler.py
--rw-rw-r--  2.0 unx     2421 b- defN 24-Apr-11 05:46 olive/strategy/search_algorithm/random_sampler.py
--rw-rw-r--  2.0 unx     2306 b- defN 24-Apr-11 05:46 olive/strategy/search_algorithm/search_algorithm.py
--rw-rw-r--  2.0 unx     1841 b- defN 24-Apr-11 05:46 olive/strategy/search_algorithm/tpe_sampler.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/systems/__init__.py
--rw-rw-r--  2.0 unx     2227 b- defN 24-Apr-11 05:46 olive/systems/common.py
--rw-rw-r--  2.0 unx     2300 b- defN 24-Apr-11 05:46 olive/systems/local.py
--rw-rw-r--  2.0 unx     2158 b- defN 24-Apr-11 05:46 olive/systems/olive_system.py
--rw-rw-r--  2.0 unx     3140 b- defN 24-Apr-11 05:46 olive/systems/system_alias.py
--rw-rw-r--  2.0 unx     7048 b- defN 24-Apr-11 05:46 olive/systems/system_config.py
--rw-rw-r--  2.0 unx      411 b- defN 24-Apr-11 05:46 olive/systems/azureml/__init__.py
--rw-rw-r--  2.0 unx     2883 b- defN 24-Apr-11 05:46 olive/systems/azureml/aml_evaluation_runner.py
--rw-rw-r--  2.0 unx     8763 b- defN 24-Apr-11 05:46 olive/systems/azureml/aml_pass_runner.py
--rw-rw-r--  2.0 unx    32108 b- defN 24-Apr-11 05:46 olive/systems/azureml/aml_system.py
--rw-rw-r--  2.0 unx      717 b- defN 24-Apr-11 05:46 olive/systems/docker/Dockerfile
--rw-rw-r--  2.0 unx      464 b- defN 24-Apr-11 05:46 olive/systems/docker/Dockerfile.cpu
--rw-rw-r--  2.0 unx     1006 b- defN 24-Apr-11 05:46 olive/systems/docker/Dockerfile.gpu
--rw-rw-r--  2.0 unx     2531 b- defN 24-Apr-11 05:46 olive/systems/docker/Dockerfile.openvino
--rw-rw-r--  2.0 unx      407 b- defN 24-Apr-11 05:46 olive/systems/docker/__init__.py
--rw-rw-r--  2.0 unx    18244 b- defN 24-Apr-11 05:46 olive/systems/docker/docker_system.py
--rw-rw-r--  2.0 unx     2187 b- defN 24-Apr-11 05:46 olive/systems/docker/eval.py
--rw-rw-r--  2.0 unx     1956 b- defN 24-Apr-11 05:46 olive/systems/docker/runner.py
--rw-rw-r--  2.0 unx     6200 b- defN 24-Apr-11 05:46 olive/systems/docker/utils.py
--rw-rw-r--  2.0 unx      357 b- defN 24-Apr-11 05:46 olive/systems/isolated_ort/__init__.py
--rw-rw-r--  2.0 unx     3600 b- defN 24-Apr-11 05:46 olive/systems/isolated_ort/inference_runner.py
--rw-rw-r--  2.0 unx    11269 b- defN 24-Apr-11 05:46 olive/systems/isolated_ort/isolated_ort_system.py
--rw-rw-r--  2.0 unx      381 b- defN 24-Apr-11 05:46 olive/systems/python_environment/__init__.py
--rw-rw-r--  2.0 unx       37 b- defN 24-Apr-11 05:46 olive/systems/python_environment/common_requirements.txt
--rw-rw-r--  2.0 unx     2279 b- defN 24-Apr-11 05:46 olive/systems/python_environment/evaluation_runner.py
--rw-rw-r--  2.0 unx     2037 b- defN 24-Apr-11 05:46 olive/systems/python_environment/pass_runner.py
--rw-rw-r--  2.0 unx     7892 b- defN 24-Apr-11 05:46 olive/systems/python_environment/python_environment_system.py
--rw-rw-r--  2.0 unx      705 b- defN 24-Apr-11 05:46 olive/systems/utils/__init__.py
--rw-rw-r--  2.0 unx     2082 b- defN 24-Apr-11 05:46 olive/systems/utils/arg_parser.py
--rw-rw-r--  2.0 unx      913 b- defN 24-Apr-11 05:46 olive/systems/utils/available_providers_runner.py
--rw-rw-r--  2.0 unx     7419 b- defN 24-Apr-11 05:46 olive/systems/utils/misc.py
--rw-rw-r--  2.0 unx      306 b- defN 24-Apr-11 05:46 olive/workflows/__init__.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/workflows/run/__init__.py
--rw-rw-r--  2.0 unx     1418 b- defN 24-Apr-11 05:46 olive/workflows/run/__main__.py
--rw-rw-r--  2.0 unx    13473 b- defN 24-Apr-11 05:46 olive/workflows/run/config.py
--rw-rw-r--  2.0 unx    13365 b- defN 24-Apr-11 05:46 olive/workflows/run/run.py
--rw-rw-r--  2.0 unx      431 b- defN 24-Apr-11 05:46 olive/workflows/snpe/__init__.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/workflows/snpe/convertquantize/__init__.py
--rw-rw-r--  2.0 unx     1339 b- defN 24-Apr-11 05:46 olive/workflows/snpe/convertquantize/__main__.py
--rw-rw-r--  2.0 unx     4445 b- defN 24-Apr-11 05:46 olive/workflows/snpe/convertquantize/convertquantize.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/workflows/snpe/evaluate/__init__.py
--rw-rw-r--  2.0 unx      955 b- defN 24-Apr-11 05:46 olive/workflows/snpe/evaluate/__main__.py
--rw-rw-r--  2.0 unx     2974 b- defN 24-Apr-11 05:46 olive/workflows/snpe/evaluate/evaluate.py
--rw-rw-r--  2.0 unx     1141 b- defN 24-Apr-11 05:46 olive_ai-0.5.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx     3438 b- defN 24-Apr-11 05:46 olive_ai-0.5.2.dist-info/METADATA
--rw-rw-r--  2.0 unx   764423 b- defN 24-Apr-11 05:46 olive_ai-0.5.2.dist-info/NOTICE.txt
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-11 05:46 olive_ai-0.5.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx      101 b- defN 24-Apr-11 05:46 olive_ai-0.5.2.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        6 b- defN 24-Apr-11 05:46 olive_ai-0.5.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    22575 b- defN 24-Apr-11 05:46 olive_ai-0.5.2.dist-info/RECORD
-244 files, 2280681 bytes uncompressed, 480997 bytes compressed:  78.9%
+Zip file size: 549086 bytes, number of entries: 261
+-rw-rw-r--  2.0 unx      608 b- defN 24-May-15 09:53 olive/__init__.py
+-rw-rw-r--  2.0 unx      488 b- defN 24-May-15 09:53 olive/__main__.py
+-rw-rw-r--  2.0 unx    10695 b- defN 24-May-15 09:53 olive/cache.py
+-rw-rw-r--  2.0 unx     1162 b- defN 24-May-15 09:53 olive/constants.py
+-rw-rw-r--  2.0 unx     2626 b- defN 24-May-15 09:53 olive/logging.py
+-rw-rw-r--  2.0 unx     8567 b- defN 24-May-15 09:53 olive/olive_config.json
+-rw-rw-r--  2.0 unx     1406 b- defN 24-May-15 09:53 olive/package_config.py
+-rw-rw-r--  2.0 unx    23380 b- defN 24-May-15 09:53 olive/resource_path.py
+-rw-rw-r--  2.0 unx     5170 b- defN 24-May-15 09:53 olive/auto_optimizer/__init__.py
+-rw-rw-r--  2.0 unx     5918 b- defN 24-May-15 09:53 olive/auto_optimizer/regulate_mixins.py
+-rw-rw-r--  2.0 unx     3615 b- defN 24-May-15 09:53 olive/auto_optimizer/template_mapping.py
+-rw-rw-r--  2.0 unx     1171 b- defN 24-May-15 09:53 olive/auto_optimizer/config_template/opt_level_passes.yaml
+-rw-rw-r--  2.0 unx     2062 b- defN 24-May-15 09:53 olive/auto_optimizer/config_template/pass_capability.yaml
+-rw-rw-r--  2.0 unx      247 b- defN 24-May-15 09:53 olive/azureml/__init__.py
+-rw-rw-r--  2.0 unx     6699 b- defN 24-May-15 09:53 olive/azureml/azureml_client.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-May-15 09:53 olive/cli/__init__.py
+-rw-rw-r--  2.0 unx      630 b- defN 24-May-15 09:53 olive/cli/base.py
+-rw-rw-r--  2.0 unx     1256 b- defN 24-May-15 09:53 olive/cli/configure_qualcomm_sdk.py
+-rw-rw-r--  2.0 unx     6236 b- defN 24-May-15 09:53 olive/cli/export_adapters.py
+-rw-rw-r--  2.0 unx     2348 b- defN 24-May-15 09:53 olive/cli/launcher.py
+-rw-rw-r--  2.0 unx     7275 b- defN 24-May-15 09:53 olive/cli/manage_aml_compute.py
+-rw-rw-r--  2.0 unx     1831 b- defN 24-May-15 09:53 olive/cli/run.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-May-15 09:53 olive/common/__init__.py
+-rw-rw-r--  2.0 unx     3430 b- defN 24-May-15 09:53 olive/common/auto_config.py
+-rw-rw-r--  2.0 unx    10422 b- defN 24-May-15 09:53 olive/common/config_utils.py
+-rw-rw-r--  2.0 unx     1488 b- defN 24-May-15 09:53 olive/common/import_lib.py
+-rw-rw-r--  2.0 unx    18372 b- defN 24-May-15 09:53 olive/common/ort_inference.py
+-rw-rw-r--  2.0 unx      765 b- defN 24-May-15 09:53 olive/common/pydantic_v1.py
+-rw-rw-r--  2.0 unx     1809 b- defN 24-May-15 09:53 olive/common/user_module_loader.py
+-rw-rw-r--  2.0 unx    13009 b- defN 24-May-15 09:53 olive/common/utils.py
+-rw-rw-r--  2.0 unx      345 b- defN 24-May-15 09:53 olive/data/__init__.py
+-rw-rw-r--  2.0 unx    10636 b- defN 24-May-15 09:53 olive/data/config.py
+-rw-rw-r--  2.0 unx     1443 b- defN 24-May-15 09:53 olive/data/constants.py
+-rw-rw-r--  2.0 unx     8119 b- defN 24-May-15 09:53 olive/data/registry.py
+-rw-rw-r--  2.0 unx     3573 b- defN 24-May-15 09:53 olive/data/template.py
+-rw-rw-r--  2.0 unx      444 b- defN 24-May-15 09:53 olive/data/component/__init__.py
+-rw-rw-r--  2.0 unx     1955 b- defN 24-May-15 09:53 olive/data/component/dataloader.py
+-rw-rw-r--  2.0 unx    10505 b- defN 24-May-15 09:53 olive/data/component/dataset.py
+-rw-rw-r--  2.0 unx     1928 b- defN 24-May-15 09:53 olive/data/component/load_dataset.py
+-rw-rw-r--  2.0 unx     2256 b- defN 24-May-15 09:53 olive/data/component/post_process_data.py
+-rw-rw-r--  2.0 unx    11446 b- defN 24-May-15 09:53 olive/data/component/pre_process_data.py
+-rw-rw-r--  2.0 unx    29278 b- defN 24-May-15 09:53 olive/data/component/text_generation.py
+-rw-rw-r--  2.0 unx      480 b- defN 24-May-15 09:53 olive/data/container/__init__.py
+-rw-rw-r--  2.0 unx     3385 b- defN 24-May-15 09:53 olive/data/container/data_container.py
+-rw-rw-r--  2.0 unx     1159 b- defN 24-May-15 09:53 olive/data/container/dummy_data_container.py
+-rw-rw-r--  2.0 unx     1690 b- defN 24-May-15 09:53 olive/data/container/huggingface_container.py
+-rw-rw-r--  2.0 unx     1721 b- defN 24-May-15 09:53 olive/data/container/raw_data_container.py
+-rw-rw-r--  2.0 unx      442 b- defN 24-May-15 09:53 olive/engine/__init__.py
+-rw-rw-r--  2.0 unx     1199 b- defN 24-May-15 09:53 olive/engine/config.py
+-rw-rw-r--  2.0 unx    46570 b- defN 24-May-15 09:53 olive/engine/engine.py
+-rw-rw-r--  2.0 unx    17415 b- defN 24-May-15 09:53 olive/engine/footprint.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-May-15 09:53 olive/engine/packaging/__init__.py
+-rw-rw-r--  2.0 unx     3285 b- defN 24-May-15 09:53 olive/engine/packaging/packaging_config.py
+-rw-rw-r--  2.0 unx    32569 b- defN 24-May-15 09:53 olive/engine/packaging/packaging_generator.py
+-rw-rw-r--  2.0 unx     1325 b- defN 24-May-15 09:53 olive/engine/packaging/sample_code/GenAIOnnxModel/cpp/CMakeLists.txt
+-rw-rw-r--  2.0 unx      438 b- defN 24-May-15 09:53 olive/engine/packaging/sample_code/GenAIOnnxModel/cpp/README.md
+-rw-rw-r--  2.0 unx     4097 b- defN 24-May-15 09:53 olive/engine/packaging/sample_code/GenAIOnnxModel/cpp/code_sample.cpp
+-rw-rw-r--  2.0 unx      184 b- defN 24-May-15 09:53 olive/engine/packaging/sample_code/GenAIOnnxModel/cs/README.md
+-rw-rw-r--  2.0 unx     3587 b- defN 24-May-15 09:53 olive/engine/packaging/sample_code/GenAIOnnxModel/cs/code_sample.cs
+-rw-rw-r--  2.0 unx      652 b- defN 24-May-15 09:53 olive/engine/packaging/sample_code/GenAIOnnxModel/cs/olive-genai-cs-sample.csproj
+-rw-rw-r--  2.0 unx     1122 b- defN 24-May-15 09:53 olive/engine/packaging/sample_code/GenAIOnnxModel/cs/olive-genai-cs-sample.sln
+-rw-rw-r--  2.0 unx      840 b- defN 24-May-15 09:53 olive/engine/packaging/sample_code/GenAIOnnxModel/python/README.md
+-rw-rw-r--  2.0 unx     5570 b- defN 24-May-15 09:53 olive/engine/packaging/sample_code/GenAIOnnxModel/python/code_sample.py
+-rw-rw-r--  2.0 unx     1588 b- defN 24-May-15 09:53 olive/engine/packaging/sample_code/ONNXModel/cpp/README.md
+-rw-rw-r--  2.0 unx     4990 b- defN 24-May-15 09:53 olive/engine/packaging/sample_code/ONNXModel/cpp/code_sample.cpp
+-rw-rw-r--  2.0 unx     1590 b- defN 24-May-15 09:53 olive/engine/packaging/sample_code/ONNXModel/cs/README.md
+-rw-rw-r--  2.0 unx     4991 b- defN 24-May-15 09:53 olive/engine/packaging/sample_code/ONNXModel/cs/code_sample.cs
+-rw-rw-r--  2.0 unx     2296 b- defN 24-May-15 09:53 olive/engine/packaging/sample_code/ONNXModel/python/README.md
+-rw-rw-r--  2.0 unx     2557 b- defN 24-May-15 09:53 olive/engine/packaging/sample_code/ONNXModel/python/code_sample.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-May-15 09:53 olive/evaluator/__init__.py
+-rw-rw-r--  2.0 unx     6368 b- defN 24-May-15 09:53 olive/evaluator/accuracy.py
+-rw-rw-r--  2.0 unx     7343 b- defN 24-May-15 09:53 olive/evaluator/metric.py
+-rw-rw-r--  2.0 unx     4548 b- defN 24-May-15 09:53 olive/evaluator/metric_backend.py
+-rw-rw-r--  2.0 unx     4523 b- defN 24-May-15 09:53 olive/evaluator/metric_config.py
+-rw-rw-r--  2.0 unx     1702 b- defN 24-May-15 09:53 olive/evaluator/metric_result.py
+-rw-rw-r--  2.0 unx    47925 b- defN 24-May-15 09:53 olive/evaluator/olive_evaluator.py
+-rw-rw-r--  2.0 unx      592 b- defN 24-May-15 09:53 olive/exception/__init__.py
+-rw-rw-r--  2.0 unx      621 b- defN 24-May-15 09:53 olive/hardware/__init__.py
+-rw-rw-r--  2.0 unx     6688 b- defN 24-May-15 09:53 olive/hardware/accelerator.py
+-rw-rw-r--  2.0 unx     1304 b- defN 24-May-15 09:53 olive/hardware/constants.py
+-rw-rw-r--  2.0 unx      451 b- defN 24-May-15 09:53 olive/model/__init__.py
+-rw-rw-r--  2.0 unx      758 b- defN 24-May-15 09:53 olive/model/config/__init__.py
+-rw-rw-r--  2.0 unx    11244 b- defN 24-May-15 09:53 olive/model/config/hf_config.py
+-rw-rw-r--  2.0 unx     9113 b- defN 24-May-15 09:53 olive/model/config/io_config.py
+-rw-rw-r--  2.0 unx     4567 b- defN 24-May-15 09:53 olive/model/config/kv_cache_config.py
+-rw-rw-r--  2.0 unx     3943 b- defN 24-May-15 09:53 olive/model/config/model_config.py
+-rw-rw-r--  2.0 unx     1045 b- defN 24-May-15 09:53 olive/model/config/registry.py
+-rw-rw-r--  2.0 unx     1139 b- defN 24-May-15 09:53 olive/model/handler/__init__.py
+-rw-rw-r--  2.0 unx     3533 b- defN 24-May-15 09:53 olive/model/handler/base.py
+-rw-rw-r--  2.0 unx     4461 b- defN 24-May-15 09:53 olive/model/handler/composite.py
+-rw-rw-r--  2.0 unx    10053 b- defN 24-May-15 09:53 olive/model/handler/onnx.py
+-rw-rw-r--  2.0 unx     3556 b- defN 24-May-15 09:53 olive/model/handler/openvino.py
+-rw-rw-r--  2.0 unx    17284 b- defN 24-May-15 09:53 olive/model/handler/pytorch.py
+-rw-rw-r--  2.0 unx     4489 b- defN 24-May-15 09:53 olive/model/handler/qnn.py
+-rw-rw-r--  2.0 unx     2898 b- defN 24-May-15 09:53 olive/model/handler/snpe.py
+-rw-rw-r--  2.0 unx     1474 b- defN 24-May-15 09:53 olive/model/handler/tensorflow.py
+-rw-rw-r--  2.0 unx     1106 b- defN 24-May-15 09:53 olive/model/handler/mixin/__init__.py
+-rw-rw-r--  2.0 unx      418 b- defN 24-May-15 09:53 olive/model/handler/mixin/composite.py
+-rw-rw-r--  2.0 unx     3010 b- defN 24-May-15 09:53 olive/model/handler/mixin/dummy_inputs.py
+-rw-rw-r--  2.0 unx     5993 b- defN 24-May-15 09:53 olive/model/handler/mixin/hf_config.py
+-rw-rw-r--  2.0 unx      625 b- defN 24-May-15 09:53 olive/model/handler/mixin/io_config.py
+-rw-rw-r--  2.0 unx     1472 b- defN 24-May-15 09:53 olive/model/handler/mixin/json.py
+-rw-rw-r--  2.0 unx     4183 b- defN 24-May-15 09:53 olive/model/handler/mixin/kv_cache.py
+-rw-rw-r--  2.0 unx     2242 b- defN 24-May-15 09:53 olive/model/handler/mixin/mlflow.py
+-rw-rw-r--  2.0 unx     1402 b- defN 24-May-15 09:53 olive/model/handler/mixin/onnx_ep.py
+-rw-rw-r--  2.0 unx     3946 b- defN 24-May-15 09:53 olive/model/handler/mixin/onnx_graph.py
+-rw-rw-r--  2.0 unx     2998 b- defN 24-May-15 09:53 olive/model/handler/mixin/resource.py
+-rw-rw-r--  2.0 unx      690 b- defN 24-May-15 09:53 olive/model/utils/__init__.py
+-rw-rw-r--  2.0 unx     3228 b- defN 24-May-15 09:53 olive/model/utils/hf_mappings.py
+-rw-rw-r--  2.0 unx     4517 b- defN 24-May-15 09:53 olive/model/utils/hf_onnx_config.py
+-rw-rw-r--  2.0 unx    10817 b- defN 24-May-15 09:53 olive/model/utils/hf_utils.py
+-rw-rw-r--  2.0 unx     3467 b- defN 24-May-15 09:53 olive/model/utils/onnx_utils.py
+-rw-rw-r--  2.0 unx     1510 b- defN 24-May-15 09:53 olive/model/utils/path_utils.py
+-rw-rw-r--  2.0 unx      515 b- defN 24-May-15 09:53 olive/passes/__init__.py
+-rw-rw-r--  2.0 unx    23315 b- defN 24-May-15 09:53 olive/passes/olive_pass.py
+-rw-rw-r--  2.0 unx     6143 b- defN 24-May-15 09:53 olive/passes/pass_config.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-May-15 09:53 olive/passes/onnx/__init__.py
+-rw-rw-r--  2.0 unx     8408 b- defN 24-May-15 09:53 olive/passes/onnx/append_pre_post_processing_ops.py
+-rw-rw-r--  2.0 unx     5524 b- defN 24-May-15 09:53 olive/passes/onnx/bnb_quantization.py
+-rw-rw-r--  2.0 unx     7639 b- defN 24-May-15 09:53 olive/passes/onnx/common.py
+-rw-rw-r--  2.0 unx    28894 b- defN 24-May-15 09:53 olive/passes/onnx/conversion.py
+-rw-rw-r--  2.0 unx     4862 b- defN 24-May-15 09:53 olive/passes/onnx/dynamic_to_fixed_shape.py
+-rw-rw-r--  2.0 unx    15977 b- defN 24-May-15 09:53 olive/passes/onnx/extract_adapters.py
+-rw-rw-r--  2.0 unx     3209 b- defN 24-May-15 09:53 olive/passes/onnx/float16_conversion.py
+-rw-rw-r--  2.0 unx     4646 b- defN 24-May-15 09:53 olive/passes/onnx/float32_conversion.py
+-rw-rw-r--  2.0 unx    27158 b- defN 24-May-15 09:53 olive/passes/onnx/inc_quantization.py
+-rw-rw-r--  2.0 unx    15972 b- defN 24-May-15 09:53 olive/passes/onnx/insert_beam_search.py
+-rw-rw-r--  2.0 unx    18495 b- defN 24-May-15 09:53 olive/passes/onnx/merge_decoders.py
+-rw-rw-r--  2.0 unx     9054 b- defN 24-May-15 09:53 olive/passes/onnx/mixed_precision.py
+-rw-rw-r--  2.0 unx    10432 b- defN 24-May-15 09:53 olive/passes/onnx/model_builder.py
+-rw-rw-r--  2.0 unx    10011 b- defN 24-May-15 09:53 olive/passes/onnx/model_optimizer.py
+-rw-rw-r--  2.0 unx    15752 b- defN 24-May-15 09:53 olive/passes/onnx/moe_experts_distributor.py
+-rw-rw-r--  2.0 unx     4749 b- defN 24-May-15 09:53 olive/passes/onnx/nvmo_quantization.py
+-rw-rw-r--  2.0 unx    18912 b- defN 24-May-15 09:53 olive/passes/onnx/onnx_dag.py
+-rw-rw-r--  2.0 unx     6162 b- defN 24-May-15 09:53 olive/passes/onnx/optimum_conversion.py
+-rw-rw-r--  2.0 unx     3709 b- defN 24-May-15 09:53 olive/passes/onnx/optimum_merging.py
+-rw-rw-r--  2.0 unx    29116 b- defN 24-May-15 09:53 olive/passes/onnx/perf_tuning.py
+-rw-rw-r--  2.0 unx     5375 b- defN 24-May-15 09:53 olive/passes/onnx/qnn_preprocess.py
+-rw-rw-r--  2.0 unx    37593 b- defN 24-May-15 09:53 olive/passes/onnx/quantization.py
+-rw-rw-r--  2.0 unx    19890 b- defN 24-May-15 09:53 olive/passes/onnx/transformer_optimization.py
+-rw-rw-r--  2.0 unx    15135 b- defN 24-May-15 09:53 olive/passes/onnx/vitis_ai_quantization.py
+-rw-rw-r--  2.0 unx     3239 b- defN 24-May-15 09:53 olive/passes/onnx/pipeline/__init__.py
+-rw-rw-r--  2.0 unx     8457 b- defN 24-May-15 09:53 olive/passes/onnx/pipeline/step_utils.py
+-rw-rw-r--  2.0 unx      508 b- defN 24-May-15 09:53 olive/passes/onnx/vitis_ai/__init__.py
+-rw-rw-r--  2.0 unx     7778 b- defN 24-May-15 09:53 olive/passes/onnx/vitis_ai/calibrate.py
+-rw-rw-r--  2.0 unx    15723 b- defN 24-May-15 09:53 olive/passes/onnx/vitis_ai/quant_utils.py
+-rw-rw-r--  2.0 unx    13588 b- defN 24-May-15 09:53 olive/passes/onnx/vitis_ai/quantize.py
+-rw-rw-r--  2.0 unx    66718 b- defN 24-May-15 09:53 olive/passes/onnx/vitis_ai/quantizer.py
+-rw-rw-r--  2.0 unx    18750 b- defN 24-May-15 09:53 olive/passes/onnx/vitis_ai/refine.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-May-15 09:53 olive/passes/openvino/__init__.py
+-rw-rw-r--  2.0 unx     4555 b- defN 24-May-15 09:53 olive/passes/openvino/conversion.py
+-rw-rw-r--  2.0 unx    12637 b- defN 24-May-15 09:53 olive/passes/openvino/quantization.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-May-15 09:53 olive/passes/pytorch/__init__.py
+-rw-rw-r--  2.0 unx    10184 b- defN 24-May-15 09:53 olive/passes/pytorch/autoawq.py
+-rw-rw-r--  2.0 unx     7058 b- defN 24-May-15 09:53 olive/passes/pytorch/cluster.py
+-rw-rw-r--  2.0 unx     9834 b- defN 24-May-15 09:53 olive/passes/pytorch/gptq.py
+-rw-rw-r--  2.0 unx    50163 b- defN 24-May-15 09:53 olive/passes/pytorch/lora.py
+-rw-rw-r--  2.0 unx     1021 b- defN 24-May-15 09:53 olive/passes/pytorch/pytorch_lightning_utils.py
+-rw-rw-r--  2.0 unx     8038 b- defN 24-May-15 09:53 olive/passes/pytorch/qat_utils.py
+-rw-rw-r--  2.0 unx    11630 b- defN 24-May-15 09:53 olive/passes/pytorch/quant_utils.py
+-rw-rw-r--  2.0 unx     6444 b- defN 24-May-15 09:53 olive/passes/pytorch/quantization_aware_training.py
+-rw-rw-r--  2.0 unx     6868 b- defN 24-May-15 09:53 olive/passes/pytorch/slicegpt.py
+-rw-rw-r--  2.0 unx     9021 b- defN 24-May-15 09:53 olive/passes/pytorch/sparsegpt.py
+-rw-rw-r--  2.0 unx    10774 b- defN 24-May-15 09:53 olive/passes/pytorch/sparsegpt_utils.py
+-rw-rw-r--  2.0 unx     7032 b- defN 24-May-15 09:53 olive/passes/pytorch/tensor_parallel.py
+-rw-rw-r--  2.0 unx     5372 b- defN 24-May-15 09:53 olive/passes/pytorch/tensor_parallel_layers.py
+-rw-rw-r--  2.0 unx    17239 b- defN 24-May-15 09:53 olive/passes/pytorch/tensor_parallel_llama2.py
+-rw-rw-r--  2.0 unx     8172 b- defN 24-May-15 09:53 olive/passes/pytorch/torch_trt_conversion.py
+-rw-rw-r--  2.0 unx     3185 b- defN 24-May-15 09:53 olive/passes/pytorch/trt_utils.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-May-15 09:53 olive/passes/qnn/__init__.py
+-rw-rw-r--  2.0 unx     3192 b- defN 24-May-15 09:53 olive/passes/qnn/context_binary_generator.py
+-rw-rw-r--  2.0 unx     5448 b- defN 24-May-15 09:53 olive/passes/qnn/conversion.py
+-rw-rw-r--  2.0 unx     3298 b- defN 24-May-15 09:53 olive/passes/qnn/model_lib_generator.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-May-15 09:53 olive/passes/snpe/__init__.py
+-rw-rw-r--  2.0 unx     4802 b- defN 24-May-15 09:53 olive/passes/snpe/conversion.py
+-rw-rw-r--  2.0 unx     5254 b- defN 24-May-15 09:53 olive/passes/snpe/quantization.py
+-rw-rw-r--  2.0 unx     2637 b- defN 24-May-15 09:53 olive/passes/snpe/snpe_to_onnx.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-May-15 09:53 olive/passes/utils/__init__.py
+-rw-rw-r--  2.0 unx     1619 b- defN 24-May-15 09:53 olive/passes/utils/whisper_prepost.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-May-15 09:53 olive/platform_sdk/__init__.py
+-rw-rw-r--  2.0 unx      341 b- defN 24-May-15 09:53 olive/platform_sdk/qualcomm/__init__.py
+-rw-rw-r--  2.0 unx     1348 b- defN 24-May-15 09:53 olive/platform_sdk/qualcomm/constants.py
+-rw-rw-r--  2.0 unx     1046 b- defN 24-May-15 09:53 olive/platform_sdk/qualcomm/copy_libcdsprpc.ps1
+-rw-rw-r--  2.0 unx     2387 b- defN 24-May-15 09:53 olive/platform_sdk/qualcomm/create_python_env.ps1
+-rw-rw-r--  2.0 unx     2431 b- defN 24-May-15 09:53 olive/platform_sdk/qualcomm/create_python_env.sh
+-rw-rw-r--  2.0 unx     4034 b- defN 24-May-15 09:53 olive/platform_sdk/qualcomm/env.py
+-rw-rw-r--  2.0 unx     3869 b- defN 24-May-15 09:53 olive/platform_sdk/qualcomm/runner.py
+-rw-rw-r--  2.0 unx      380 b- defN 24-May-15 09:53 olive/platform_sdk/qualcomm/configure/__init__.py
+-rw-rw-r--  2.0 unx      533 b- defN 24-May-15 09:53 olive/platform_sdk/qualcomm/configure/__main__.py
+-rw-rw-r--  2.0 unx     3486 b- defN 24-May-15 09:53 olive/platform_sdk/qualcomm/configure/configure.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-May-15 09:53 olive/platform_sdk/qualcomm/qnn/__init__.py
+-rw-rw-r--  2.0 unx     2015 b- defN 24-May-15 09:53 olive/platform_sdk/qualcomm/qnn/env.py
+-rw-rw-r--  2.0 unx     7269 b- defN 24-May-15 09:53 olive/platform_sdk/qualcomm/qnn/qnn.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-May-15 09:53 olive/platform_sdk/qualcomm/qnn/utils/__init__.py
+-rw-rw-r--  2.0 unx      396 b- defN 24-May-15 09:53 olive/platform_sdk/qualcomm/snpe/__init__.py
+-rw-rw-r--  2.0 unx     2079 b- defN 24-May-15 09:53 olive/platform_sdk/qualcomm/snpe/env.py
+-rw-rw-r--  2.0 unx     3969 b- defN 24-May-15 09:53 olive/platform_sdk/qualcomm/snpe/snpe.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-May-15 09:53 olive/platform_sdk/qualcomm/snpe/tools/__init__.py
+-rw-rw-r--  2.0 unx    10951 b- defN 24-May-15 09:53 olive/platform_sdk/qualcomm/snpe/tools/dev.py
+-rw-rw-r--  2.0 unx    19075 b- defN 24-May-15 09:53 olive/platform_sdk/qualcomm/snpe/tools/inference.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-May-15 09:53 olive/platform_sdk/qualcomm/snpe/utils/__init__.py
+-rw-rw-r--  2.0 unx     6978 b- defN 24-May-15 09:53 olive/platform_sdk/qualcomm/snpe/utils/adb.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-May-15 09:53 olive/platform_sdk/qualcomm/utils/__init__.py
+-rw-rw-r--  2.0 unx    16573 b- defN 24-May-15 09:53 olive/platform_sdk/qualcomm/utils/data_loader.py
+-rw-rw-r--  2.0 unx     8878 b- defN 24-May-15 09:53 olive/platform_sdk/qualcomm/utils/input_list.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-May-15 09:53 olive/strategy/__init__.py
+-rw-rw-r--  2.0 unx    11993 b- defN 24-May-15 09:53 olive/strategy/search_parameter.py
+-rw-rw-r--  2.0 unx     5638 b- defN 24-May-15 09:53 olive/strategy/search_results.py
+-rw-rw-r--  2.0 unx     4781 b- defN 24-May-15 09:53 olive/strategy/search_space.py
+-rw-rw-r--  2.0 unx    13016 b- defN 24-May-15 09:53 olive/strategy/search_strategy.py
+-rw-rw-r--  2.0 unx     2817 b- defN 24-May-15 09:53 olive/strategy/utils.py
+-rw-rw-r--  2.0 unx      717 b- defN 24-May-15 09:53 olive/strategy/search_algorithm/__init__.py
+-rw-rw-r--  2.0 unx     1148 b- defN 24-May-15 09:53 olive/strategy/search_algorithm/exhaustive.py
+-rw-rw-r--  2.0 unx     4407 b- defN 24-May-15 09:53 olive/strategy/search_algorithm/optuna_sampler.py
+-rw-rw-r--  2.0 unx     2473 b- defN 24-May-15 09:53 olive/strategy/search_algorithm/random_sampler.py
+-rw-rw-r--  2.0 unx     2160 b- defN 24-May-15 09:53 olive/strategy/search_algorithm/search_algorithm.py
+-rw-rw-r--  2.0 unx     1838 b- defN 24-May-15 09:53 olive/strategy/search_algorithm/tpe_sampler.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-May-15 09:53 olive/systems/__init__.py
+-rw-rw-r--  2.0 unx    12276 b- defN 24-May-15 09:53 olive/systems/accelerator_creator.py
+-rw-rw-r--  2.0 unx     2288 b- defN 24-May-15 09:53 olive/systems/common.py
+-rw-rw-r--  2.0 unx     2345 b- defN 24-May-15 09:53 olive/systems/local.py
+-rw-rw-r--  2.0 unx     2203 b- defN 24-May-15 09:53 olive/systems/olive_system.py
+-rw-rw-r--  2.0 unx     3140 b- defN 24-May-15 09:53 olive/systems/system_alias.py
+-rw-rw-r--  2.0 unx     7969 b- defN 24-May-15 09:53 olive/systems/system_config.py
+-rw-rw-r--  2.0 unx      411 b- defN 24-May-15 09:53 olive/systems/azureml/__init__.py
+-rw-rw-r--  2.0 unx     2883 b- defN 24-May-15 09:53 olive/systems/azureml/aml_evaluation_runner.py
+-rw-rw-r--  2.0 unx     8466 b- defN 24-May-15 09:53 olive/systems/azureml/aml_pass_runner.py
+-rw-rw-r--  2.0 unx    31865 b- defN 24-May-15 09:53 olive/systems/azureml/aml_system.py
+-rw-rw-r--  2.0 unx      717 b- defN 24-May-15 09:53 olive/systems/docker/Dockerfile
+-rw-rw-r--  2.0 unx      464 b- defN 24-May-15 09:53 olive/systems/docker/Dockerfile.cpu
+-rw-rw-r--  2.0 unx     1006 b- defN 24-May-15 09:53 olive/systems/docker/Dockerfile.gpu
+-rw-rw-r--  2.0 unx     2531 b- defN 24-May-15 09:53 olive/systems/docker/Dockerfile.openvino
+-rw-rw-r--  2.0 unx      407 b- defN 24-May-15 09:53 olive/systems/docker/__init__.py
+-rw-rw-r--  2.0 unx    18295 b- defN 24-May-15 09:53 olive/systems/docker/docker_system.py
+-rw-rw-r--  2.0 unx     2187 b- defN 24-May-15 09:53 olive/systems/docker/eval.py
+-rw-rw-r--  2.0 unx     1956 b- defN 24-May-15 09:53 olive/systems/docker/runner.py
+-rw-rw-r--  2.0 unx     6258 b- defN 24-May-15 09:53 olive/systems/docker/utils.py
+-rw-rw-r--  2.0 unx      357 b- defN 24-May-15 09:53 olive/systems/isolated_ort/__init__.py
+-rw-rw-r--  2.0 unx     3600 b- defN 24-May-15 09:53 olive/systems/isolated_ort/inference_runner.py
+-rw-rw-r--  2.0 unx    11296 b- defN 24-May-15 09:53 olive/systems/isolated_ort/isolated_ort_system.py
+-rw-rw-r--  2.0 unx      381 b- defN 24-May-15 09:53 olive/systems/python_environment/__init__.py
+-rw-rw-r--  2.0 unx       37 b- defN 24-May-15 09:53 olive/systems/python_environment/common_requirements.txt
+-rw-rw-r--  2.0 unx     2279 b- defN 24-May-15 09:53 olive/systems/python_environment/evaluation_runner.py
+-rw-rw-r--  2.0 unx     2037 b- defN 24-May-15 09:53 olive/systems/python_environment/pass_runner.py
+-rw-rw-r--  2.0 unx     7899 b- defN 24-May-15 09:53 olive/systems/python_environment/python_environment_system.py
+-rw-rw-r--  2.0 unx      705 b- defN 24-May-15 09:53 olive/systems/utils/__init__.py
+-rw-rw-r--  2.0 unx     2082 b- defN 24-May-15 09:53 olive/systems/utils/arg_parser.py
+-rw-rw-r--  2.0 unx      913 b- defN 24-May-15 09:53 olive/systems/utils/available_providers_runner.py
+-rw-rw-r--  2.0 unx     7680 b- defN 24-May-15 09:53 olive/systems/utils/misc.py
+-rw-rw-r--  2.0 unx      306 b- defN 24-May-15 09:53 olive/workflows/__init__.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-May-15 09:53 olive/workflows/run/__init__.py
+-rw-rw-r--  2.0 unx      399 b- defN 24-May-15 09:53 olive/workflows/run/__main__.py
+-rw-rw-r--  2.0 unx    11708 b- defN 24-May-15 09:53 olive/workflows/run/config.py
+-rw-rw-r--  2.0 unx    15359 b- defN 24-May-15 09:53 olive/workflows/run/run.py
+-rw-rw-r--  2.0 unx     1141 b- defN 24-May-15 09:53 olive_ai-0.6.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3568 b- defN 24-May-15 09:53 olive_ai-0.6.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx   764423 b- defN 24-May-15 09:53 olive_ai-0.6.0.dist-info/NOTICE.txt
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-15 09:53 olive_ai-0.6.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       50 b- defN 24-May-15 09:53 olive_ai-0.6.0.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        6 b- defN 24-May-15 09:53 olive_ai-0.6.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    24338 b- defN 24-May-15 09:53 olive_ai-0.6.0.dist-info/RECORD
+261 files, 2412528 bytes uncompressed, 510176 bytes compressed:  78.9%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: olive/__init__.py
 Comment: 
 
+Filename: olive/__main__.py
+Comment: 
+
 Filename: olive/cache.py
 Comment: 
 
 Filename: olive/constants.py
 Comment: 
 
 Filename: olive/logging.py
@@ -36,14 +39,35 @@
 
 Filename: olive/azureml/__init__.py
 Comment: 
 
 Filename: olive/azureml/azureml_client.py
 Comment: 
 
+Filename: olive/cli/__init__.py
+Comment: 
+
+Filename: olive/cli/base.py
+Comment: 
+
+Filename: olive/cli/configure_qualcomm_sdk.py
+Comment: 
+
+Filename: olive/cli/export_adapters.py
+Comment: 
+
+Filename: olive/cli/launcher.py
+Comment: 
+
+Filename: olive/cli/manage_aml_compute.py
+Comment: 
+
+Filename: olive/cli/run.py
+Comment: 
+
 Filename: olive/common/__init__.py
 Comment: 
 
 Filename: olive/common/auto_config.py
 Comment: 
 
 Filename: olive/common/config_utils.py
@@ -132,14 +156,41 @@
 
 Filename: olive/engine/packaging/packaging_config.py
 Comment: 
 
 Filename: olive/engine/packaging/packaging_generator.py
 Comment: 
 
+Filename: olive/engine/packaging/sample_code/GenAIOnnxModel/cpp/CMakeLists.txt
+Comment: 
+
+Filename: olive/engine/packaging/sample_code/GenAIOnnxModel/cpp/README.md
+Comment: 
+
+Filename: olive/engine/packaging/sample_code/GenAIOnnxModel/cpp/code_sample.cpp
+Comment: 
+
+Filename: olive/engine/packaging/sample_code/GenAIOnnxModel/cs/README.md
+Comment: 
+
+Filename: olive/engine/packaging/sample_code/GenAIOnnxModel/cs/code_sample.cs
+Comment: 
+
+Filename: olive/engine/packaging/sample_code/GenAIOnnxModel/cs/olive-genai-cs-sample.csproj
+Comment: 
+
+Filename: olive/engine/packaging/sample_code/GenAIOnnxModel/cs/olive-genai-cs-sample.sln
+Comment: 
+
+Filename: olive/engine/packaging/sample_code/GenAIOnnxModel/python/README.md
+Comment: 
+
+Filename: olive/engine/packaging/sample_code/GenAIOnnxModel/python/code_sample.py
+Comment: 
+
 Filename: olive/engine/packaging/sample_code/ONNXModel/cpp/README.md
 Comment: 
 
 Filename: olive/engine/packaging/sample_code/ONNXModel/cpp/code_sample.cpp
 Comment: 
 
 Filename: olive/engine/packaging/sample_code/ONNXModel/cs/README.md
@@ -165,14 +216,17 @@
 
 Filename: olive/evaluator/metric_backend.py
 Comment: 
 
 Filename: olive/evaluator/metric_config.py
 Comment: 
 
+Filename: olive/evaluator/metric_result.py
+Comment: 
+
 Filename: olive/evaluator/olive_evaluator.py
 Comment: 
 
 Filename: olive/exception/__init__.py
 Comment: 
 
 Filename: olive/hardware/__init__.py
@@ -192,14 +246,17 @@
 
 Filename: olive/model/config/hf_config.py
 Comment: 
 
 Filename: olive/model/config/io_config.py
 Comment: 
 
+Filename: olive/model/config/kv_cache_config.py
+Comment: 
+
 Filename: olive/model/config/model_config.py
 Comment: 
 
 Filename: olive/model/config/registry.py
 Comment: 
 
 Filename: olive/model/handler/__init__.py
@@ -243,14 +300,20 @@
 
 Filename: olive/model/handler/mixin/io_config.py
 Comment: 
 
 Filename: olive/model/handler/mixin/json.py
 Comment: 
 
+Filename: olive/model/handler/mixin/kv_cache.py
+Comment: 
+
+Filename: olive/model/handler/mixin/mlflow.py
+Comment: 
+
 Filename: olive/model/handler/mixin/onnx_ep.py
 Comment: 
 
 Filename: olive/model/handler/mixin/onnx_graph.py
 Comment: 
 
 Filename: olive/model/handler/mixin/resource.py
@@ -303,35 +366,41 @@
 
 Filename: olive/passes/onnx/extract_adapters.py
 Comment: 
 
 Filename: olive/passes/onnx/float16_conversion.py
 Comment: 
 
-Filename: olive/passes/onnx/genai_model_exporter.py
+Filename: olive/passes/onnx/float32_conversion.py
 Comment: 
 
 Filename: olive/passes/onnx/inc_quantization.py
 Comment: 
 
 Filename: olive/passes/onnx/insert_beam_search.py
 Comment: 
 
 Filename: olive/passes/onnx/merge_decoders.py
 Comment: 
 
 Filename: olive/passes/onnx/mixed_precision.py
 Comment: 
 
+Filename: olive/passes/onnx/model_builder.py
+Comment: 
+
 Filename: olive/passes/onnx/model_optimizer.py
 Comment: 
 
 Filename: olive/passes/onnx/moe_experts_distributor.py
 Comment: 
 
+Filename: olive/passes/onnx/nvmo_quantization.py
+Comment: 
+
 Filename: olive/passes/onnx/onnx_dag.py
 Comment: 
 
 Filename: olive/passes/onnx/optimum_conversion.py
 Comment: 
 
 Filename: olive/passes/onnx/optimum_merging.py
@@ -384,32 +453,35 @@
 
 Filename: olive/passes/openvino/quantization.py
 Comment: 
 
 Filename: olive/passes/pytorch/__init__.py
 Comment: 
 
-Filename: olive/passes/pytorch/cluster.py
+Filename: olive/passes/pytorch/autoawq.py
 Comment: 
 
-Filename: olive/passes/pytorch/gptq.py
+Filename: olive/passes/pytorch/cluster.py
 Comment: 
 
-Filename: olive/passes/pytorch/gptq_utils.py
+Filename: olive/passes/pytorch/gptq.py
 Comment: 
 
 Filename: olive/passes/pytorch/lora.py
 Comment: 
 
 Filename: olive/passes/pytorch/pytorch_lightning_utils.py
 Comment: 
 
 Filename: olive/passes/pytorch/qat_utils.py
 Comment: 
 
+Filename: olive/passes/pytorch/quant_utils.py
+Comment: 
+
 Filename: olive/passes/pytorch/quantization_aware_training.py
 Comment: 
 
 Filename: olive/passes/pytorch/slicegpt.py
 Comment: 
 
 Filename: olive/passes/pytorch/sparsegpt.py
@@ -465,17 +537,14 @@
 
 Filename: olive/platform_sdk/__init__.py
 Comment: 
 
 Filename: olive/platform_sdk/qualcomm/__init__.py
 Comment: 
 
-Filename: olive/platform_sdk/qualcomm/configure.py
-Comment: 
-
 Filename: olive/platform_sdk/qualcomm/constants.py
 Comment: 
 
 Filename: olive/platform_sdk/qualcomm/copy_libcdsprpc.ps1
 Comment: 
 
 Filename: olive/platform_sdk/qualcomm/create_python_env.ps1
@@ -486,14 +555,23 @@
 
 Filename: olive/platform_sdk/qualcomm/env.py
 Comment: 
 
 Filename: olive/platform_sdk/qualcomm/runner.py
 Comment: 
 
+Filename: olive/platform_sdk/qualcomm/configure/__init__.py
+Comment: 
+
+Filename: olive/platform_sdk/qualcomm/configure/__main__.py
+Comment: 
+
+Filename: olive/platform_sdk/qualcomm/configure/configure.py
+Comment: 
+
 Filename: olive/platform_sdk/qualcomm/qnn/__init__.py
 Comment: 
 
 Filename: olive/platform_sdk/qualcomm/qnn/env.py
 Comment: 
 
 Filename: olive/platform_sdk/qualcomm/qnn/qnn.py
@@ -531,23 +609,14 @@
 
 Filename: olive/platform_sdk/qualcomm/utils/data_loader.py
 Comment: 
 
 Filename: olive/platform_sdk/qualcomm/utils/input_list.py
 Comment: 
 
-Filename: olive/scripts/__init__.py
-Comment: 
-
-Filename: olive/scripts/export_adapters.py
-Comment: 
-
-Filename: olive/scripts/manage_compute_instance.py
-Comment: 
-
 Filename: olive/strategy/__init__.py
 Comment: 
 
 Filename: olive/strategy/search_parameter.py
 Comment: 
 
 Filename: olive/strategy/search_results.py
@@ -579,14 +648,17 @@
 
 Filename: olive/strategy/search_algorithm/tpe_sampler.py
 Comment: 
 
 Filename: olive/systems/__init__.py
 Comment: 
 
+Filename: olive/systems/accelerator_creator.py
+Comment: 
+
 Filename: olive/systems/common.py
 Comment: 
 
 Filename: olive/systems/local.py
 Comment: 
 
 Filename: olive/systems/olive_system.py
@@ -684,50 +756,29 @@
 
 Filename: olive/workflows/run/config.py
 Comment: 
 
 Filename: olive/workflows/run/run.py
 Comment: 
 
-Filename: olive/workflows/snpe/__init__.py
-Comment: 
-
-Filename: olive/workflows/snpe/convertquantize/__init__.py
-Comment: 
-
-Filename: olive/workflows/snpe/convertquantize/__main__.py
-Comment: 
-
-Filename: olive/workflows/snpe/convertquantize/convertquantize.py
-Comment: 
-
-Filename: olive/workflows/snpe/evaluate/__init__.py
-Comment: 
-
-Filename: olive/workflows/snpe/evaluate/__main__.py
-Comment: 
-
-Filename: olive/workflows/snpe/evaluate/evaluate.py
-Comment: 
-
-Filename: olive_ai-0.5.2.dist-info/LICENSE
+Filename: olive_ai-0.6.0.dist-info/LICENSE
 Comment: 
 
-Filename: olive_ai-0.5.2.dist-info/METADATA
+Filename: olive_ai-0.6.0.dist-info/METADATA
 Comment: 
 
-Filename: olive_ai-0.5.2.dist-info/NOTICE.txt
+Filename: olive_ai-0.6.0.dist-info/NOTICE.txt
 Comment: 
 
-Filename: olive_ai-0.5.2.dist-info/WHEEL
+Filename: olive_ai-0.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: olive_ai-0.5.2.dist-info/entry_points.txt
+Filename: olive_ai-0.6.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: olive_ai-0.5.2.dist-info/top_level.txt
+Filename: olive_ai-0.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: olive_ai-0.5.2.dist-info/RECORD
+Filename: olive_ai-0.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## olive/__init__.py

```diff
@@ -10,8 +10,8 @@
 
 _sc = logging.StreamHandler(stream=sys.stdout)
 _formatter = logging.Formatter("[%(asctime)s] [%(levelname)s] [%(filename)s:%(lineno)d:%(funcName)s] %(message)s")
 _sc.setFormatter(_formatter)
 _logger.addHandler(_sc)
 _logger.propagate = False
 
-__version__ = "0.5.2"
+__version__ = "0.6.0"
```

## olive/cache.py

```diff
@@ -104,15 +104,16 @@
 def download_resource(resource_path: ResourcePath, cache_dir: Union[str, Path] = ".olive-cache"):
     """Return the path to a non-local resource.
 
     Non-local resources are stored in the non_local_resources subdirectory of the cache.
     """
     non_local_resource_dir = get_cache_sub_dirs(cache_dir)[3]
 
-    resource_path_hash = hash_dict(resource_path.to_json())
+    # choose left 8 characters of hash as resource path hash to reduce the risk of length too long
+    resource_path_hash = hash_dict(resource_path.to_json())[:8]
     resource_path_json = non_local_resource_dir / f"{resource_path_hash}.json"
 
     # check if resource path is cached
     if resource_path_json.exists():
         logger.debug("Using cached resource path %s", resource_path.to_json())
         with resource_path_json.open("r") as f:
             resource_path_data = json.load(f)["dest"]
@@ -239,12 +240,26 @@
         else:
             save_dir = output_dir
             save_name = output_name
 
         # save resource to output directory
         model_json["config"][resource_name] = local_resource_path.save_to_dir(save_dir, save_name, overwrite)
 
+    # Copy "additional files" to the output folder
+    model_attributes = model_json["config"].get("model_attributes") or {}
+    additional_files = model_attributes.get("additional_files", [])
+
+    for i, src_filepath in enumerate(additional_files):
+        dst_filepath = Path(output_dir) / output_name / Path(src_filepath).name
+        additional_files[i] = str(dst_filepath)
+
+        if not dst_filepath.exists():
+            shutil.copy(str(src_filepath), str(dst_filepath))
+
+    if additional_files:
+        model_json["config"]["model_attributes"]["additional_files"] = additional_files
+
     # save model json
     with (output_dir / f"{output_name}.json").open("w") as f:
         json.dump(model_json, f, indent=4)
 
     return model_json
```

## olive/olive_config.json

### Pretty-printed

 * *Similarity: 0.9570833333333333%*

 * *Differences: {"'extra_dependencies'": "{'nvmo': ['nvidia-modelopt~=0.11.0', 'onnx-graphsurgeon']}",*

 * * "'passes'": "{'OnnxFloatToFloat16': {delete: ['module_dependencies']}, 'ModelBuilder': "*

 * *             "OrderedDict([('module_path', 'olive.passes.onnx.model_builder.ModelBuilder')]), "*

 * *             "'OnnxIOFloat16ToFloat32': OrderedDict([('module_path', "*

 * *             "'olive.passes.onnx.float32_conversion.OnnxIOFloat16ToFloat32')]), "*

 * *             "'AutoAWQQuantizer': OrderedDict([('module_path', "*

 * *             "'olive. […]*

```diff
@@ -25,14 +25,18 @@
             "neural-compressor"
         ],
         "lora": [
             "accelerate",
             "peft",
             "scipy"
         ],
+        "nvmo": [
+            "nvidia-modelopt~=0.11.0",
+            "onnx-graphsurgeon"
+        ],
         "openvino": [
             "openvino==2023.2.0",
             "nncf==2.7.0"
         ],
         "optimum": [
             "optimum"
         ],
@@ -53,23 +57,26 @@
             "torch-tensorrt"
         ]
     },
     "passes": {
         "AppendPrePostProcessingOps": {
             "module_path": "olive.passes.onnx.append_pre_post_processing_ops.AppendPrePostProcessingOps"
         },
+        "AutoAWQQuantizer": {
+            "module_dependencies": [
+                "autoawq"
+            ],
+            "module_path": "olive.passes.pytorch.autoawq.AutoAWQQuantizer"
+        },
         "DynamicToFixedShape": {
             "module_path": "olive.passes.onnx.dynamic_to_fixed_shape.DynamicToFixedShape"
         },
         "ExtractAdapters": {
             "module_path": "olive.passes.onnx.extract_adapters.ExtractAdapters"
         },
-        "GenAIModelExporter": {
-            "module_path": "olive.passes.onnx.genai_model_exporter.GenAIModelExporter"
-        },
         "GptqQuantizer": {
             "module_dependencies": [
                 "auto-gptq",
                 "optimum"
             ],
             "module_path": "olive.passes.pytorch.gptq.GptqQuantizer"
         },
@@ -102,29 +109,38 @@
         },
         "LoftQ": {
             "module_path": "olive.passes.pytorch.lora.LoftQ"
         },
         "MoEExpertsDistributor": {
             "module_path": "olive.passes.onnx.moe_experts_distributor.MoEExpertsDistributor"
         },
+        "ModelBuilder": {
+            "module_path": "olive.passes.onnx.model_builder.ModelBuilder"
+        },
+        "NVModelOptQuantization": {
+            "extra_dependencies": [
+                "nvmo"
+            ],
+            "module_path": "olive.passes.onnx.nvmo_quantization.NVModelOptQuantization"
+        },
         "OnnxBnb4Quantization": {
             "module_path": "olive.passes.onnx.bnb_quantization.OnnxBnb4Quantization"
         },
         "OnnxConversion": {
             "module_path": "olive.passes.onnx.conversion.OnnxConversion"
         },
         "OnnxDynamicQuantization": {
             "module_path": "olive.passes.onnx.quantization.OnnxDynamicQuantization"
         },
         "OnnxFloatToFloat16": {
-            "module_dependencies": [
-                "onnxconverter-common"
-            ],
             "module_path": "olive.passes.onnx.float16_conversion.OnnxFloatToFloat16"
         },
+        "OnnxIOFloat16ToFloat32": {
+            "module_path": "olive.passes.onnx.float32_conversion.OnnxIOFloat16ToFloat32"
+        },
         "OnnxMatMul4Quantizer": {
             "module_path": "olive.passes.onnx.quantization.OnnxMatMul4Quantizer"
         },
         "OnnxModelOptimizer": {
             "module_path": "olive.passes.onnx.model_optimizer.OnnxModelOptimizer"
         },
         "OnnxOpVersionConversion": {
```

## olive/resource_path.py

```diff
@@ -153,14 +153,22 @@
     if is_local_file and isinstance(resource_path, Path) and not resource_path.exists():
         raise ValueError(f"Resource path {resource_path} of type Path does not exist.")
 
     logger.debug("Resource path %s is inferred to be of type %s.", resource_path, resource_type)
     return ResourcePathConfig(type=resource_type, config={config_key: resource_path}).create_resource_path()
 
 
+def validate_resource_path(v, values, field):
+    try:
+        v = create_resource_path(v)
+    except ValueError as e:
+        raise ValueError(f"Invalid resource path '{v}': {e}") from None
+    return v
+
+
 def _overwrite_helper(new_path: Union[Path, str], overwrite: bool):
     new_path = Path(new_path).resolve()
 
     # check if the resource already exists
     if new_path.exists():
         if not overwrite:
             # raise an error if the file/folder with same name already exists and overwrite is set to False
@@ -372,15 +380,21 @@
 
     @classmethod
     def _default_config(cls) -> Dict[str, Any]:
         return {
             "azureml_client": ConfigParam(
                 type_=AzureMLClientConfig, required=False, description="AzureML client config."
             ),
-            "registry_name": ConfigParam(type_=str, required=True, description="Name of the registry."),
+            "registry_name": ConfigParam(
+                type_=str,
+                required=True,
+                description=(
+                    "Name of the registry. Basically, the value is parent directory name of given model in azureml"
+                ),
+            ),
             "name": ConfigParam(type_=str, required=True, description="Name of the model."),
             "version": ConfigParam(type_=Union[int, str], required=True, description="Version of the model."),
         }
 
     def get_path(self) -> str:
         return (
             f"azureml://registries/{self.config.registry_name}/models/{self.config.name}/versions/{self.config.version}"
```

## olive/auto_optimizer/__init__.py

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 
 import logging
 from copy import deepcopy
 from enum import Enum
-from typing import Dict, List, Optional
+from typing import List, Optional
 
 from olive.auto_optimizer.regulate_mixins import RegulatePassConfigMixin
 from olive.common.config_utils import ConfigBase
 from olive.common.pydantic_v1 import validator
 from olive.data.config import DataConfig
 from olive.evaluator.olive_evaluator import OliveEvaluatorConfig
 from olive.hardware.accelerator import AcceleratorSpec
@@ -54,21 +54,21 @@
 class AutoOptimizer(RegulatePassConfigMixin):
     def __init__(
         self,
         input_model_config: ModelConfig,
         evaluator_config: OliveEvaluatorConfig,
         accelerator_spec: AcceleratorSpec,
         auto_optimizer_config: Optional[AutoOptimizerConfig] = None,
-        data_configs: Optional[Dict[str, DataConfig]] = None,
+        data_configs: Optional[List[DataConfig]] = None,
     ):
         self.input_model_config = input_model_config
         self.evaluator_config = evaluator_config
         self.accelerator_spec = accelerator_spec
         self.auto_optimizer_config = auto_optimizer_config or AutoOptimizerConfig()
-        self.data_configs = data_configs or {}
+        self.data_configs = data_configs or []
         self._initialize()
 
     def _initialize(self):
         # 1. input model config
         self.model_config = deepcopy(self.input_model_config)
 
         # 2. evaluator config
```

## olive/auto_optimizer/regulate_mixins.py

```diff
@@ -100,27 +100,27 @@
                         )
 
             pass_flows[i] = new_pf
 
         return pass_config, pass_flows
 
     def regulate_data_config(self, pass_config, pass_flows):
-        from olive.workflows.run.config import INPUT_MODEL_DATA_CONFIG
-
-        data_configs = self.data_configs.get(INPUT_MODEL_DATA_CONFIG)
-        if not data_configs:
+        if not self.data_configs or not self.auto_optimizer_config or self.auto_optimizer_config.disable_auto_optimizer:
             return pass_config, pass_flows
 
-        # data_config
+        if len(self.data_configs) != 1:
+            raise ValueError("AutoOptimizer expects exactly one data config.")
+
         passes_require_data_config = ["OnnxQuantization", "OrtPerfTuning"]
         for p in passes_require_data_config:
             # TODO(anyone): support multi data_config for different passes, pass_flows
             p_names = self._find_pass_name_in_pass_flow(p, pass_flows)
             for pn in p_names:
-                pass_config[pn]["config"]["data_config"] = data_configs.to_json()
+                pass_config[pn]["config"]["data_config"] = self.data_configs[0]
+
         return pass_config, pass_flows
 
     def _allow_precision(self, precision):
         if not self.auto_optimizer_config.precisions:
             # empty precisions means no precision restriction
             return True
```

## olive/common/config_utils.py

```diff
@@ -235,37 +235,24 @@
     if "user_script" not in values:
         raise ValueError("Invalid user_script")
     if isinstance(v, str) and values["user_script"] is None:
         raise ValueError(f"user_script must be provided if {field.name} is a name string")
     return v
 
 
-def validate_resource_path(v, values, field):
-    from olive.resource_path import create_resource_path
-
-    try:
-        v = create_resource_path(v)
-    except ValueError as e:
-        raise ValueError(f"Invalid resource path '{v}': {e}") from None
-    return v
-
-
 def create_config_class(
     class_name: str,
     default_config: Dict[str, ConfigParam],
     base: type = ConfigBase,
     validators: Dict[str, Callable] = None,
 ) -> Type[ConfigBase]:
     """Create a Pydantic model class from a configuration dictionary."""
     config = {}
     validators = validators.copy() if validators else {}
     for param, param_config in default_config.items():
-        if param == "data_dir":
-            validator_name = f"validate_{param}_resource_path"
-            validators[validator_name] = validator(param, allow_reuse=True)(validate_resource_path)
         # automatically add validator for object params
         if param_config.category == ParamCategory.OBJECT:
             validator_name = f"validate_{param}_object"
             count = 0
             while validator_name in validators:
                 validator_name = f"{validator_name}_{count}"
                 count += 1
```

## olive/common/ort_inference.py

```diff
@@ -81,15 +81,15 @@
     extra_session_config = session_options.get("extra_session_config")
     if enable_profiling:
         sess_options.enable_profiling = True
     if inter_op_num_threads:
         sess_options.inter_op_num_threads = inter_op_num_threads
     if intra_op_num_threads:
         sess_options.intra_op_num_threads = intra_op_num_threads
-    if execution_mode:
+    if execution_mode is not None:
         if execution_mode == 0:
             sess_options.execution_mode = ort.ExecutionMode.ORT_SEQUENTIAL
         elif execution_mode == 1:
             sess_options.execution_mode = ort.ExecutionMode.ORT_PARALLEL
     if graph_optimization_level:
         sess_options.graph_optimization_level = ort.GraphOptimizationLevel(graph_optimization_level)
     if extra_session_config:
```

## olive/common/utils.py

```diff
@@ -11,25 +11,34 @@
 import platform
 import shlex
 import shutil
 import subprocess
 import tempfile
 import time
 from pathlib import Path
-from typing import Dict
+from typing import Dict, List, Tuple, Union
 
 logger = logging.getLogger(__name__)
 
 
 def run_subprocess(cmd, env=None, cwd=None, check=False):
     logger.debug("Running command: %s", cmd)
 
     assert isinstance(cmd, (str, list)), f"cmd must be a string or a list, got {type(cmd)}."
     windows = platform.system() == "Windows"
     if isinstance(cmd, str):
+        # In posix model, the cmd string will be handled with specific posix rules.
+        # https://docs.python.org/3.8/library/shlex.html#parsing-rules
+        # We listed 2 typical examples:
+        # 1. The cmd may contain the folder/file path from windows. This kind of path is like: C:\\User\\xxx\\...
+        #   in posix mode, the shlex.split will split the path into ['C:Userxxx...'], which is not correct.
+        #   in non-posix mode, the shlex.split will split the path into ['C:\\User\\xxx\\...'].
+        # 2. The cmd may contain the quotes("" or ''). This kind of cmd is like: "str_0, 'str_1'"
+        #   in posix mode, the shlex.split will split the cmd into ["str_0", "str_1"]
+        #   in non-posix mode, the shlex.split will split the cmd into ["str_0", "'str_1'"]
         cmd = shlex.split(cmd, posix=not windows)
 
     try:
         out = subprocess.run(cmd, env=env, cwd=cwd, capture_output=True, check=check)
     except subprocess.CalledProcessError as e:
         err_msg = [
             f"Failed to run {cmd} with returncode {e.returncode}!",
@@ -43,21 +52,21 @@
     stdout = out.stdout.decode("utf-8")
     stderr = out.stderr.decode("utf-8")
 
     return returncode, stdout, stderr
 
 
 def hash_string(string):  # pragma: no cover
-    md5_hash = hashlib.md5()
+    md5_hash = hashlib.sha256()
     md5_hash.update(string.encode())
     return md5_hash.hexdigest()
 
 
 def hash_io_stream(f):  # pragma: no cover
-    md5_hash = hashlib.md5()
+    md5_hash = hashlib.sha256()
     # Read and update hash in chunks of 4K
     for byte_block in iter(lambda: f.read(4096), b""):
         md5_hash.update(byte_block)
     return md5_hash.hexdigest()
 
 
 def hash_file(filename):  # pragma: no cover
@@ -81,26 +90,26 @@
             hash_value = hash_update_from_file(path, hash_value)
         elif path.is_dir():
             hash_value = hash_update_from_dir(path, hash_value)
     return hash_value
 
 
 def hash_dir(directory):
-    return hash_update_from_dir(directory, hashlib.md5()).hexdigest()
+    return hash_update_from_dir(directory, hashlib.sha256()).hexdigest()
 
 
 def hash_dict(dictionary):  # pragma: no cover
-    md5_hash = hashlib.md5()
+    md5_hash = hashlib.sha256()
     encoded_dictionary = json.dumps(dictionary, sort_keys=True).encode()
     md5_hash.update(encoded_dictionary)
     return md5_hash.hexdigest()
 
 
 def hash_function(function):  # pragma: no cover
-    md5_hash = hashlib.md5()
+    md5_hash = hashlib.sha256()
     try:
         source = inspect.getsource(function)
     except OSError:
         logger.warning("Could not get source code for %s. Hash will be based on name only.", function.__name__)
         source = function.__name__
     md5_hash.update(source.encode())
     return md5_hash.hexdigest()
@@ -342,7 +351,20 @@
     # setting as string to be safe
     logger.debug("Setting tempdir to %s from %s", tempdir, tempfile.tempdir)
     tempfile.tempdir = str(tempdir)
 
 
 def exclude_keys(original_dict: Dict, keys_to_exclude):
     return {k: v for k, v in original_dict.items() if k not in keys_to_exclude}
+
+
+def find_first_matched_value(original_dict: Dict, keys: Union[str, Tuple, List[str]], raise_key_error=False):
+    if isinstance(keys, str):
+        keys = [keys]
+
+    for possible_name in keys:
+        if possible_name in original_dict:
+            return original_dict[possible_name]
+
+    if raise_key_error:
+        raise KeyError(f"Keys {keys} not found in {original_dict}")
+    return None
```

## olive/data/config.py

```diff
@@ -31,15 +31,15 @@
     DataComponentType.PRE_PROCESS_DATA.value: DefaultDataComponent.PRE_PROCESS_DATA.value,
     DataComponentType.POST_PROCESS_DATA.value: DefaultDataComponent.POST_PROCESS_DATA.value,
     DataComponentType.DATALOADER.value: DefaultDataComponent.DATALOADER.value,
 }
 
 
 class DataConfig(ConfigBase):
-    name: str = DefaultDataContainer.DATA_CONTAINER.value
+    name: str
     type: str = DefaultDataContainer.DATA_CONTAINER.value
 
     # used to store the params for each component
     params_config: Dict = None
 
     # user script to define and register the components
     user_script: Union[Path, str] = None
```

## olive/data/component/dataset.py

```diff
@@ -7,14 +7,16 @@
 from pathlib import Path
 from typing import List, Optional, Union
 
 import numpy as np
 import torch
 from torch.utils.data import Dataset as TorchDataset
 
+from olive.common.utils import resolve_torch_dtype
+
 
 class BaseDataset(TorchDataset):
     """Define the Olive dataset which should return the data with following format.
 
     1. [data, label] for supervised learning
     2. [data] for unsupervised learning
     The data should be a list or dict of numpy arrays or torch tensors
@@ -109,23 +111,15 @@
     def __getitem__(self, index):
         # From https://docs.python.org/3/reference/datamodel.html#object.__getitem__,
         # __getitem__ should raise IndexError when index is out of range
         # Otherwise, the enumerate function will enter infinite loop
         if index < 0 or index >= len(self):
             raise IndexError("Index out of range")
 
-        str_to_type = {
-            "float32": torch.float32,
-            "float16": torch.float16,
-            "int32": torch.int32,
-            "int64": torch.int64,
-            "int8": torch.int8,
-            "bool": torch.bool,
-        }
-        input_types = [str_to_type[type_] for type_ in self.input_types]
+        input_types = [resolve_torch_dtype(dtype_str) for dtype_str in self.input_types]
 
         if not self.input_names:
             dummy_inputs = []
             for shape, dtype in zip(self.input_shapes, input_types):
                 dummy_inputs.append(torch.ones(shape, dtype=dtype))
             dummy_inputs = tuple(dummy_inputs) if len(dummy_inputs) > 1 else dummy_inputs[0]
         else:
```

## olive/engine/engine.py

```diff
@@ -13,15 +13,16 @@
 
 import olive.cache as cache_utils
 from olive.common.config_utils import validate_config
 from olive.common.utils import hash_dict
 from olive.engine.config import FAILED_CONFIG, INVALID_CONFIG, PRUNED_CONFIGS
 from olive.engine.footprint import Footprint, FootprintNodeMetric
 from olive.engine.packaging.packaging_generator import generate_output_artifacts
-from olive.evaluator.metric import Metric, MetricResult, joint_metric_key
+from olive.evaluator.metric import Metric
+from olive.evaluator.metric_result import MetricResult, joint_metric_key
 from olive.evaluator.olive_evaluator import OliveEvaluatorConfig
 from olive.exception import EXCEPTIONS_TO_RAISE, OlivePassError
 from olive.hardware import AcceleratorSpec
 from olive.model import ModelConfig
 from olive.strategy.search_strategy import SearchStrategy, SearchStrategyConfig
 from olive.systems.common import SystemType
 from olive.systems.system_config import SystemConfig
@@ -736,30 +737,30 @@
                 # set local resource path
                 model_config.config[resource_name] = downloaded_resource_path
 
         return model_config
 
     def _init_input_model(self, input_model_config: ModelConfig):
         """Initialize the input model."""
-        model_hash = hash_dict(input_model_config.to_json())
+        model_hash = hash_dict(input_model_config.to_json())[:8]
 
         # cache the model
         self._cache_model(input_model_config, model_hash, check_object=False)
 
         return model_hash
 
     def get_run_json_path(
         self,
         pass_name: int,
         input_model_number: str,
         pass_config: dict,
         accelerator_spec: "AcceleratorSpec",
     ):
         """Get the path to the run json."""
-        pass_config_hash = hash_dict(pass_config)
+        pass_config_hash = hash_dict(pass_config)[:8]
         if not accelerator_spec:
             run_json_path = self._run_cache_path / f"{pass_name}-{input_model_number}-{pass_config_hash}.json"
         else:
             run_json_path = (
                 self._run_cache_path / f"{pass_name}-{input_model_number}-{pass_config_hash}-{accelerator_spec}.json"
             )
         return run_json_path
@@ -901,15 +902,15 @@
         # new model id
         input_model_number = input_model_id.split("_")[0]
         # Note: the final output model id need contains the accelerator information
         # if the output model is accelerator dependent.
         output_model_id_parts = [
             f"{self._get_new_model_number()}_{pass_name}",
             input_model_number,
-            hash_dict(pass_config),
+            hash_dict(pass_config)[:8],
         ]
 
         if not p.is_accelerator_agnostic(accelerator_spec):
             output_model_id_parts.append(f"{accelerator_spec}")
 
         output_model_id = "-".join(map(str, output_model_id_parts))
         output_model_path = self._model_cache_path / f"{output_model_id}" / "output_model"
@@ -1067,28 +1068,37 @@
                 )
                 return create_managed_system_with_cache(config, accelerator_spec)
             else:
                 logger.debug("create native OliveSystem %s", config.type)
                 return config.create_system()
 
         if not self.target:
+            logger.info("Creating target system ...")
+            target_start_time = time.time()
             self.target = create_system(self.target_config, accelerator_spec)
+            logger.info("Target system created in %f seconds", time.time() - target_start_time)
         if not self.host:
             host_accelerators = self.host_config.config.accelerators
             if host_accelerators and host_accelerators[0].execution_providers:
                 host_accelerator_spec = AcceleratorSpec(
                     host_accelerators[0].device, host_accelerators[0].execution_providers[0]
                 )
             else:
                 host_accelerator_spec = None
+            logger.info("Creating host system ...")
+            host_start_time = time.time()
             self.host = create_system(self.host_config, host_accelerator_spec)
+            logger.info("Host system created in %f seconds", time.time() - host_start_time)
 
         yield
 
         if self.target_config.olive_managed_env:
+            # could we put it under cache system for reusing?
+            logger.info("Removing target system ...")
             self.target.remove()
             self.target = None
         if self.host_config.olive_managed_env:
+            logger.info("Removing host system ...")
             self.host.remove()
             self.host = None
 
         create_managed_system_with_cache.cache_clear()
```

## olive/engine/footprint.py

```diff
@@ -5,15 +5,15 @@
 
 import logging
 from collections import OrderedDict, defaultdict
 from copy import deepcopy
 from typing import DefaultDict, Dict, List, NamedTuple, Optional
 
 from olive.common.config_utils import ConfigBase, config_json_dumps, config_json_loads
-from olive.evaluator.metric import MetricResult
+from olive.evaluator.metric_result import MetricResult
 
 logger = logging.getLogger(__name__)
 
 
 class RunHistory(NamedTuple):
     """Run history of a model."""
 
@@ -97,15 +97,15 @@
 
     def create_pareto_frontier(self, output_model_num: int = None) -> Optional["Footprint"]:
         self._mark_pareto_frontier()
         if output_model_num is None or len(self.nodes) <= output_model_num:
             logger.info("Output all %d models", len(self.nodes))
             return self._create_pareto_frontier_from_nodes(self.nodes)
         else:
-            topk_nodes = self._get_top_ranked_nodes(output_model_num)
+            topk_nodes = self.get_top_ranked_nodes(output_model_num)
             logger.info("Output top ranked %d models based on metric priorities", len(topk_nodes))
             return self._create_pareto_frontier_from_nodes(topk_nodes)
 
     def plot_pareto_frontier_to_html(self, index=None, save_path=None, is_show=False):
         self._plot_pareto_frontier(index, save_path, is_show, "html")
 
     def plot_pareto_frontier_to_image(self, index=None, save_path=None, is_show=False):
@@ -294,15 +294,15 @@
                     equal &= current_point_metrics == other_point_metrics
                 # point is not on pareto frontier if dominated and not equal
                 _against_pareto_frontier_check = dominated and not equal
                 cmp_flag &= not _against_pareto_frontier_check
             self.nodes[k].is_pareto_frontier = cmp_flag
         self.is_marked_pareto_frontier = True
 
-    def _get_top_ranked_nodes(self, k: int) -> List[FootprintNode]:
+    def get_top_ranked_nodes(self, k: int) -> List[FootprintNode]:
         footprint_node_list = self.nodes.values()
         sorted_footprint_node_list = sorted(
             footprint_node_list,
             key=lambda x: tuple(
                 (
                     x.metrics.value[metric].value
                     if x.metrics.cmp_direction[metric] == 1
```

## olive/engine/packaging/packaging_config.py

```diff
@@ -11,14 +11,15 @@
 
 class PackagingType(str, Enum):
     """Output Artifacts type."""
 
     Zipfile = "Zipfile"
     AzureMLModels = "AzureMLModels"
     AzureMLData = "AzureMLData"
+    AzureMLDeployment = "AzureMLDeployment"
 
 
 class CommonPackagingConfig(ConfigBase):
     export_in_mlflow_format: bool = False
 
 
 class ZipfilePackagingConfig(CommonPackagingConfig):
@@ -31,26 +32,77 @@
 
 
 class AzureMLModelsPackagingConfig(CommonPackagingConfig):
     version: Union[int, str] = "1"
     description: Optional[str] = None
 
 
+class InferencingServerType(str, Enum):
+    AzureMLOnline = "AzureMLOnline"
+    AzureMLBatch = "AzureMLBatch"
+
+
+class InferenceServerConfig(ConfigBase):
+    type: InferencingServerType
+    code_folder: str
+    scoring_script: str
+
+
+class AzureMLModelModeType(str, Enum):
+    download = "download"
+    copy = "copy"
+
+
+class ModelConfigurationConfig(ConfigBase):
+    mode: AzureMLModelModeType = AzureMLModelModeType.download
+    mount_path: Optional[str] = None  # Relative mount path
+
+
+class ModelPackageConfig(ConfigBase):
+    target_environment: str = "olive-target-environment"
+    target_environment_version: Optional[str] = None
+    inferencing_server: InferenceServerConfig
+    base_environment_id: str
+    model_configurations: ModelConfigurationConfig = None
+    environment_variables: Optional[dict] = None
+
+
+class DeploymentConfig(ConfigBase):
+    endpoint_name: str = "olive-default-endpoint"
+    deployment_name: str = "olive-default-deployment"
+    instance_type: Optional[str] = None
+    compute: Optional[str] = None
+    instance_count: int = 1
+    mini_batch_size: int = 10  # AzureMLBatch only
+    extra_config: Optional[dict] = None
+
+
+class AzureMLDeploymentPackagingConfig(CommonPackagingConfig):
+    model_name: str = "olive-deployment-model"
+    model_version: Union[int, str] = "1"
+    model_description: Optional[str] = None
+    model_package: ModelPackageConfig
+    deployment_config: DeploymentConfig = DeploymentConfig()
+
+
 _type_to_config = {
     PackagingType.Zipfile: ZipfilePackagingConfig,
     PackagingType.AzureMLModels: AzureMLModelsPackagingConfig,
     PackagingType.AzureMLData: AzureMLDataPackagingConfig,
+    PackagingType.AzureMLDeployment: AzureMLDeploymentPackagingConfig,
 }
 
 
 class PackagingConfig(ConfigBase):
     """Olive output artifacts generation config."""
 
     type: PackagingType = PackagingType.Zipfile
     name: str = "OutputModels"
     config: CommonPackagingConfig = None
+    include_runtime_packages: bool = True
+    include_sample_code: bool = True
 
     @validator("config", pre=True, always=True)
     def _validate_config(cls, v, values):
         packaging_type = values.get("type")
         config_class = _type_to_config.get(packaging_type)
         return validate_config(v, config_class)
```

## olive/engine/packaging/packaging_generator.py

```diff
@@ -8,22 +8,22 @@
 import shutil
 import sys
 import tempfile
 import urllib.request
 from collections import OrderedDict
 from pathlib import Path
 from string import Template
-from typing import TYPE_CHECKING, Dict, List, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Set, Union
 
 import pkg_resources
 
 from olive.common.utils import copy_dir, retry_func, run_subprocess
 from olive.engine.packaging.packaging_config import (
-    AzureMLDataPackagingConfig,
-    AzureMLModelsPackagingConfig,
+    AzureMLDeploymentPackagingConfig,
+    InferencingServerType,
     PackagingConfig,
     PackagingType,
 )
 from olive.model import ONNXModelHandler
 from olive.resource_path import ResourceType, create_resource_path
 from olive.systems.utils import get_package_name_from_ep
 
@@ -45,15 +45,246 @@
     azureml_client_config: "AzureMLClientConfig" = None,
 ):
     if sum(len(f.nodes) if f.nodes else 0 for f in pf_footprints.values()) == 0:
         logger.warning("No model is selected. Skip packaging output artifacts.")
         return
     packaging_config_list = packaging_configs if isinstance(packaging_configs, list) else [packaging_configs]
     for packaging_config in packaging_config_list:
-        _package_candidate_models(packaging_config, output_dir, footprints, pf_footprints, azureml_client_config)
+        if packaging_config.type == PackagingType.AzureMLDeployment:
+            _package_azureml_deployment(packaging_config, footprints, pf_footprints, azureml_client_config)
+        else:
+            _package_candidate_models(packaging_config, output_dir, footprints, pf_footprints, azureml_client_config)
+
+
+def _package_azureml_deployment(
+    packaging_config: AzureMLDeploymentPackagingConfig,
+    footprints: Dict["AcceleratorSpec", "Footprint"],
+    pf_footprints: Dict["AcceleratorSpec", "Footprint"],
+    azureml_client_config: "AzureMLClientConfig" = None,
+):
+    from azure.ai.ml.entities import (
+        AzureMLBatchInferencingServer,
+        AzureMLOnlineInferencingServer,
+        BaseEnvironment,
+        BatchDeployment,
+        BatchEndpoint,
+        CodeConfiguration,
+        ManagedOnlineDeployment,
+        ManagedOnlineEndpoint,
+        ModelConfiguration,
+        ModelPackage,
+    )
+    from azure.core.exceptions import ResourceExistsError, ResourceNotFoundError, ServiceResponseError
+
+    config: AzureMLDeploymentPackagingConfig = packaging_config.config
+    if config.export_in_mlflow_format:
+        logger.warning("Exporting model in MLflow format is not supported for AzureML endpoint packaging.")
+
+    try:
+        # Get best model from footprint
+        best_node = _get_best_candidate_node(pf_footprints, footprints)
+
+        with tempfile.TemporaryDirectory() as temp_dir:
+            tempdir = Path(temp_dir)
+
+            model_config = best_node.model_config
+            _save_model(
+                model_config["config"].get("model_path", None),
+                model_config["type"],
+                model_config,
+                tempdir,
+                model_config["config"].get("inference_settings", None),
+                False,
+            )
+
+            # Register model to AzureML
+            _upload_to_azureml_models(
+                azureml_client_config,
+                tempdir,
+                config.model_name,
+                config.model_version,
+                config.model_description,
+                False,
+            )
+
+        ml_client = azureml_client_config.create_client()
+
+        # AzureML package config
+        model_package_config = config.model_package
+
+        code_folder = Path(model_package_config.inferencing_server.code_folder)
+        assert code_folder.exists(), f"Code folder {code_folder} does not exist."
+
+        scoring_script = code_folder / model_package_config.inferencing_server.scoring_script
+        assert scoring_script.exists(), f"Scoring script {scoring_script} does not exist."
+
+        code_configuration = CodeConfiguration(
+            code=model_package_config.inferencing_server.code_folder,
+            scoring_script=model_package_config.inferencing_server.scoring_script,
+        )
+
+        inferencing_server = None
+        if model_package_config.inferencing_server.type == InferencingServerType.AzureMLOnline:
+            inferencing_server = AzureMLOnlineInferencingServer(code_configuration=code_configuration)
+        elif model_package_config.inferencing_server.type == InferencingServerType.AzureMLBatch:
+            inferencing_server = AzureMLBatchInferencingServer(code_configuration=code_configuration)
+
+        model_configuration = None
+        if model_package_config.model_configurations:
+            model_configuration = ModelConfiguration(
+                mode=model_package_config.model_configurations.mode,
+                mount_path=model_package_config.model_configurations.mount_path,
+            )
+
+        base_environment_source = BaseEnvironment(
+            type="EnvironmentAsset", resource_id=model_package_config.base_environment_id
+        )
+
+        package_request = ModelPackage(
+            target_environment=model_package_config.target_environment,
+            inferencing_server=inferencing_server,
+            base_environment_source=base_environment_source,
+            target_environment_version=model_package_config.target_environment_version,
+            model_configuration=model_configuration,
+            environment_variables=model_package_config.environment_variables,
+        )
+
+        # invoke model package operation
+        model_package = retry_func(
+            func=ml_client.models.package,
+            kwargs={"name": config.model_name, "version": config.model_version, "package_request": package_request},
+            max_tries=azureml_client_config.max_operation_retries,
+            delay=azureml_client_config.operation_retry_interval,
+            exceptions=ServiceResponseError,
+        )
+
+        logger.info(
+            "Target environment created successfully: name: %s, version: %s",
+            model_package_config.target_environment,
+            model_package_config.target_environment_version,
+        )
+
+        # Deploy model package
+        deployment_config = config.deployment_config
+
+        # Get endpoint
+        try:
+            endpoint = retry_func(
+                ml_client.online_endpoints.get,
+                [deployment_config.endpoint_name],
+                max_tries=azureml_client_config.max_operation_retries,
+                delay=azureml_client_config.operation_retry_interval,
+                exceptions=ServiceResponseError,
+            )
+            logger.info(
+                "Endpoint %s already exists. The scoring_uri is: %s",
+                deployment_config.endpoint_name,
+                endpoint.scoring_uri,
+            )
+        except ResourceNotFoundError:
+            logger.info("Endpoint %s does not exist. Creating a new endpoint...", deployment_config.endpoint_name)
+            if model_package_config.inferencing_server.type == InferencingServerType.AzureMLOnline:
+                endpoint = ManagedOnlineEndpoint(
+                    name=deployment_config.endpoint_name,
+                    description="this is an endpoint created by Olive automatically",
+                )
+            elif model_package_config.inferencing_server.type == InferencingServerType.AzureMLBatch:
+                endpoint = BatchEndpoint(
+                    name=deployment_config.endpoint_name,
+                    description="this is an endpoint created by Olive automatically",
+                )
+
+            endpoint = retry_func(
+                ml_client.online_endpoints.begin_create_or_update,
+                [endpoint],
+                max_tries=azureml_client_config.max_operation_retries,
+                delay=azureml_client_config.operation_retry_interval,
+                exceptions=ServiceResponseError,
+            ).result()
+            logger.info(
+                "Endpoint %s created successfully. The scoring_uri is: %s",
+                deployment_config.endpoint_name,
+                endpoint.scoring_uri,
+            )
+
+        deployment = None
+        extra_config = deployment_config.extra_config or {}
+        if model_package_config.inferencing_server.type == InferencingServerType.AzureMLOnline:
+            deployment = ManagedOnlineDeployment(
+                name=deployment_config.deployment_name,
+                endpoint_name=deployment_config.endpoint_name,
+                environment=model_package,
+                instance_type=deployment_config.instance_type,
+                instance_count=deployment_config.instance_count,
+                **extra_config,
+            )
+
+        elif model_package_config.inferencing_server.type == InferencingServerType.AzureMLBatch:
+            deployment = BatchDeployment(
+                name=deployment_config.deployment_name,
+                endpoint_name=deployment_config.endpoint_name,
+                environment=model_package,
+                compute=deployment_config.compute,
+                mini_batch_size=deployment_config.mini_batch_size,
+                **extra_config,
+            )
+        deployment = retry_func(
+            ml_client.online_deployments.begin_create_or_update,
+            [deployment],
+            max_tries=azureml_client_config.max_operation_retries,
+            delay=azureml_client_config.operation_retry_interval,
+            exceptions=ServiceResponseError,
+        ).result()
+        logger.info("Deployment %s created successfully", deployment.name)
+
+    except ResourceNotFoundError:
+        logger.exception(
+            "Failed to package AzureML deployment. The resource is not found. Please check the exception details."
+        )
+        raise
+    except ResourceExistsError:
+        logger.exception(
+            "Failed to package AzureML deployment. The resource already exists. Please check the exception details."
+        )
+        raise
+    except Exception:
+        logger.exception("Failed to package AzureML deployment. Please check the exception details.")
+        raise
+
+
+def _get_best_candidate_node(
+    pf_footprints: Dict["AcceleratorSpec", "Footprint"], footprints: Dict["AcceleratorSpec", "Footprint"]
+):
+    objective_dict = next(iter(pf_footprints.values())).objective_dict
+    top_nodes = []
+    for accelerator_spec, pf_footprint in pf_footprints.items():
+        footprint = footprints[accelerator_spec]
+        if pf_footprint.nodes and footprint.nodes:
+            top_nodes.append(next(iter(pf_footprint.get_top_ranked_nodes(1))))
+    return next(
+        iter(
+            sorted(
+                top_nodes,
+                key=lambda x: tuple(
+                    (
+                        x.metrics.value[metric].value
+                        if x.metrics.cmp_direction[metric] == 1
+                        else -x.metrics.value[metric].value
+                    )
+                    for metric in objective_dict
+                ),
+                reverse=True,
+            )
+        )
+    )
+
+
+def _is_generative_model(config: Dict[str, Any]) -> bool:
+    model_attributes = config.get("model_attributes") or {}
+    return model_attributes.get("is_generative", False)
 
 
 def _package_candidate_models(
     packaging_config: PackagingConfig,
     output_dir: Path,
     footprints: Dict["AcceleratorSpec", "Footprint"],
     pf_footprints: Dict["AcceleratorSpec", "Footprint"],
@@ -63,21 +294,28 @@
     output_name = packaging_config.name
     config = packaging_config.config
     export_in_mlflow_format = config.export_in_mlflow_format
 
     logger.info("Packaging output models to %s", packaging_type)
 
     with tempfile.TemporaryDirectory() as temp_dir:
-
         tempdir = Path(temp_dir)
 
         if packaging_type == PackagingType.Zipfile:
-            cur_path = Path(__file__).parent
-            _package_sample_code(cur_path, tempdir)
-            _package_onnxruntime_packages(tempdir, next(iter(pf_footprints.values())))
+            best_node: FootprintNode = _get_best_candidate_node(pf_footprints, footprints)
+            is_generative = _is_generative_model(best_node.model_config["config"])
+
+            if packaging_config.include_sample_code:
+                _package_sample_code(Path(__file__).parent, tempdir, is_generative)
+
+            if packaging_config.include_runtime_packages:
+                if is_generative:
+                    _package_onnxruntime_genai_runtime_dependencies(tempdir)
+                else:
+                    _package_onnxruntime_runtime_dependencies(tempdir, next(iter(pf_footprints.values())))
 
         for accelerator_spec, pf_footprint in pf_footprints.items():
             footprint = footprints[accelerator_spec]
             if pf_footprint.nodes and footprint.nodes:
                 model_rank = 1
                 input_node = footprint.get_input_node()
                 for model_id, node in pf_footprint.nodes.items():
@@ -95,78 +333,98 @@
                     inference_config_path = model_dir / "inference_config.json"
                     inference_config = pf_footprint.get_model_inference_config(model_id) or {}
 
                     _copy_inference_config(inference_config_path, inference_config)
                     _copy_configurations(model_dir, footprint, model_id)
                     _copy_metrics(model_dir, input_node, node)
                     model_path = _save_model(
-                        pf_footprint, model_id, model_dir, inference_config, export_in_mlflow_format
+                        pf_footprint.get_model_path(model_id),
+                        pf_footprint.get_model_type(model_id),
+                        pf_footprint.get_model_config(model_id),
+                        model_dir,
+                        inference_config,
+                        export_in_mlflow_format,
                     )
 
                     model_info_list = []
                     relative_path = str(model_path.relative_to(tempdir))
                     model_info = _get_model_info(node, model_rank, relative_path, packaging_type)
                     model_info_list.append(model_info)
                     _copy_model_info(model_dir, model_info)
 
                     if packaging_type == PackagingType.AzureMLModels:
-                        _upload_to_azureml_models(azureml_client_config, model_dir, model_name, config)
+                        _upload_to_azureml_models(
+                            azureml_client_config,
+                            model_dir,
+                            model_name,
+                            config.version,
+                            config.description,
+                            export_in_mlflow_format,
+                        )
                     elif packaging_type == PackagingType.AzureMLData:
-                        _upload_to_azureml_data(azureml_client_config, model_dir, model_name, config)
+                        _upload_to_azureml_data(
+                            azureml_client_config, model_dir, model_name, config.version, config.description
+                        )
 
-                model_rank += 1
+                    model_rank += 1
 
         if packaging_type == PackagingType.Zipfile:
             _copy_models_rank(tempdir, model_info_list)
             _package_zipfile_model(output_dir, output_name, tempdir)
 
 
 def _upload_to_azureml_models(
     azureml_client_config: "AzureMLClientConfig",
     model_path: Path,
     model_name: str,
-    config: AzureMLModelsPackagingConfig,
+    version: Union[int, str],
+    description: str,
+    export_in_mlflow_format: bool,
 ):
     """Upload model to AzureML workspace Models."""
     from azure.ai.ml.constants import AssetTypes
     from azure.ai.ml.entities import Model
     from azure.core.exceptions import ServiceResponseError
 
     ml_client = azureml_client_config.create_client()
     model = Model(
         path=model_path,
-        type=AssetTypes.MLFLOW_MODEL if config.export_in_mlflow_format else AssetTypes.CUSTOM_MODEL,
+        type=AssetTypes.MLFLOW_MODEL if export_in_mlflow_format else AssetTypes.CUSTOM_MODEL,
         name=model_name,
-        version=str(config.version),
-        description=config.description,
+        version=str(version),
+        description=description,
     )
     retry_func(
         ml_client.models.create_or_update,
         [model],
         max_tries=azureml_client_config.max_operation_retries,
         delay=azureml_client_config.operation_retry_interval,
         exceptions=ServiceResponseError,
     )
 
 
 def _upload_to_azureml_data(
-    azureml_client_config: "AzureMLClientConfig", model_path: Path, model_name: str, config: AzureMLDataPackagingConfig
+    azureml_client_config: "AzureMLClientConfig",
+    model_path: Path,
+    model_name: str,
+    version: Union[int, str],
+    description: str,
 ):
     """Upload model as Data to AzureML workspace Data."""
     from azure.ai.ml.constants import AssetTypes
     from azure.ai.ml.entities import Data
     from azure.core.exceptions import ServiceResponseError
 
     ml_client = azureml_client_config.create_client()
     data = Data(
         path=str(model_path),
         type=AssetTypes.URI_FILE if model_path.is_file() else AssetTypes.URI_FOLDER,
-        description=config.description,
+        description=description,
         name=model_name,
-        version=str(config.version),
+        version=str(version),
     )
     retry_func(
         ml_client.data.create_or_update,
         [data],
         max_tries=azureml_client_config.max_operation_retries,
         delay=azureml_client_config.operation_retry_interval,
         exceptions=ServiceResponseError,
@@ -185,16 +443,17 @@
 
 
 def _copy_models_rank(tempdir: Path, model_info_list: List[Dict]):
     with (tempdir / "models_rank.json").open("w") as f:
         f.write(json.dumps(model_info_list))
 
 
-def _package_sample_code(cur_path: Path, tempdir: Path):
-    copy_dir(cur_path / "sample_code", tempdir / "SampleCode")
+def _package_sample_code(cur_path: Path, tempdir: Path, is_generative: bool):
+    subdir_name = "GenAIOnnxModel" if is_generative else "ONNXModel"
+    copy_dir(cur_path / "sample_code" / subdir_name, tempdir / "SampleCode")
 
 
 def _package_zipfile_model(output_dir: Path, output_name: str, model_dir: Path):
     shutil.make_archive(output_name, "zip", model_dir)
     package_file = f"{output_name}.zip"
     shutil.move(package_file, output_dir / package_file)
 
@@ -225,36 +484,34 @@
                 "input_model_metrics": input_node.metrics.value.to_json() if input_node.metrics else None,
                 "candidate_model_metrics": node.metrics.value.to_json(),
             }
             json.dump(metrics, f, indent=4)
 
 
 def _save_model(
-    pf_footprint: "Footprint",
-    model_id: str,
+    model_path: str,
+    model_type: str,
+    model_config: Dict,
     saved_model_path: Path,
     inference_config: Dict,
     export_in_mlflow_format: bool,
 ):
-    model_path = pf_footprint.get_model_path(model_id)
     model_resource_path = create_resource_path(model_path) if model_path else None
-    model_type = pf_footprint.get_model_type(model_id)
 
     if model_type.lower() == "onnxmodel":
         with tempfile.TemporaryDirectory(dir=saved_model_path, prefix="olive_tmp") as model_tempdir:
             # save to model_tempdir first since model_path may be a folder
             temp_resource_path = create_resource_path(model_resource_path.save_to_dir(model_tempdir, "model", True))
             # save to model_dir
             if temp_resource_path.type == ResourceType.LocalFile:
                 # if model_path is a file, rename it to model_dir / model.onnx
                 Path(temp_resource_path.get_path()).rename(saved_model_path / "model.onnx")
             elif temp_resource_path.type == ResourceType.LocalFolder:
                 # if model_path is a folder, save all files in the folder to model_dir / file_name
                 # file_name for .onnx file is model.onnx, otherwise keep the original file name
-                model_config = pf_footprint.get_model_config(model_id)
                 onnx_file_name = model_config.get("onnx_file_name")
                 onnx_model = ONNXModelHandler(temp_resource_path, onnx_file_name)
                 model_name = Path(onnx_model.model_path).name
                 for file in Path(temp_resource_path.get_path()).iterdir():
                     if file.name == model_name:
                         file_name = "model.onnx"
                     else:
@@ -316,15 +573,55 @@
         mlflow_model_path,
         onnx_execution_providers=inference_config.get("execution_provider"),
         onnx_session_options=session_dict,
     )
     return mlflow_model_path
 
 
-def _package_onnxruntime_packages(tempdir: Path, pf_footprint: "Footprint"):
+def _package_onnxruntime_genai_runtime_dependencies(tempdir: Path):
+    # pylint: disable=not-an-iterable
+    installed_packages = [
+        pkg
+        for pkg in pkg_resources.working_set
+        if pkg.key.startswith("onnxruntime-genai") or pkg.project_name.startswith("onnxruntime-genai")
+    ]
+    if not installed_packages:
+        logger.warning("ONNXRuntime-GenAI package is not installed. Skip packaging runtime packages.")
+        return
+
+    DOWNLOAD_COMMAND_TEMPLATE = Template(
+        f"{sys.executable} -m pip download $package_name==$version --no-deps -d $python_download_path"
+    )
+    python_download_path = tempdir / "ONNXRuntimePackages" / "python"
+    python_download_path.mkdir(parents=True, exist_ok=True)
+    python_download_path = str(python_download_path)
+
+    for pkg in installed_packages:
+        pkg_name = pkg.key if pkg.key.startswith("onnxruntime-genai") else pkg.project_name
+        download_command = DOWNLOAD_COMMAND_TEMPLATE.substitute(
+            package_name=pkg_name, version=pkg.version, python_download_path=python_download_path
+        )
+
+        try:
+            run_subprocess(download_command)
+        except Exception:
+            logger.exception(
+                "Failed to download %s package. Please manually download & install the required package.", pkg_name
+            )
+
+    # Download CPP && CS onnxruntime-genai packages
+    ort_version = installed_packages[0].version
+    lang_list = ("cpp", "cs")
+    for language in lang_list:
+        ort_download_path = tempdir / "ONNXRuntimePackages" / language
+        ort_download_path.mkdir(parents=True, exist_ok=True)
+        _download_native_onnx_packages(installed_packages, ort_version, ort_download_path)
+
+
+def _package_onnxruntime_runtime_dependencies(tempdir: Path, pf_footprint: "Footprint"):
     # pylint: disable=not-an-iterable
     installed_packages = pkg_resources.working_set
     onnxruntime_pkg = [i for i in installed_packages if i.key.startswith("onnxruntime")]
     ort_nightly_pkg = [i for i in installed_packages if i.key.startswith("ort-nightly")]
     is_nightly = bool(ort_nightly_pkg)
     is_stable = bool(onnxruntime_pkg)
 
@@ -332,27 +629,26 @@
         logger.warning("ONNXRuntime package is not installed. Skip packaging ONNXRuntime package.")
         return
 
     if is_nightly and is_stable:
         logger.warning("Both ONNXRuntime and ort-nightly packages are installed. Package ort-nightly package only.")
 
     ort_version = ort_nightly_pkg[0].version if is_nightly else onnxruntime_pkg[0].version
+    package_name_list = set()
     use_ort_extensions = False
-
     for model_id in pf_footprint.nodes:
         if pf_footprint.get_use_ort_extensions(model_id):
             use_ort_extensions = True
+
         inference_settings = pf_footprint.get_model_inference_config(model_id)
-        package_name_list = []
-        if not inference_settings:
-            package_name_list.append(("onnxruntime", "ort-nightly"))
-        else:
+        if inference_settings:
             ep_list = inference_settings["execution_provider"]
-            package_name_list.extend([get_package_name_from_ep(ep[0]) for ep in ep_list])
-            package_name_list = set(package_name_list)
+            package_name_list.update([get_package_name_from_ep(ep[0]) for ep in ep_list])
+        else:
+            package_name_list.update(["onnxruntime", "ort-nightly"])
 
     try:
         # Download Python onnxruntime package
         NIGHTLY_PYTHON_COMMAND = Template(
             f"{sys.executable} -m pip download -i "
             "https://aiinfra.pkgs.visualstudio.com/PublicPackages/_packaging/ORT-Nightly/pypi/simple/ "
             "$package_name==$ort_version --no-deps -d $python_download_path"
@@ -388,15 +684,15 @@
         lang_list = ("cpp", "cs")
         for language in lang_list:
             ort_download_path = tempdir / "ONNXRuntimePackages" / language
             ort_download_path.mkdir(parents=True, exist_ok=True)
             if is_nightly:
                 _skip_download_c_package(ort_download_path)
             else:
-                _download_c_packages(package_name_list, ort_version, ort_download_path)
+                _download_native_onnx_packages(package_name_list, ort_version, ort_download_path)
 
     except Exception:
         logger.exception("Failed to download onnxruntime package. Please manually download onnxruntime package.")
 
 
 def _download_ort_extensions_package(use_ort_extensions: bool, download_path: str):
     if use_ort_extensions:
@@ -426,26 +722,34 @@
         else:
             download_command = (
                 f"{sys.executable} -m pip download onnxruntime-extensions=={version} --no-deps -d {download_path}"
             )
             run_subprocess(download_command)
 
 
-def _download_c_packages(package_name_list: List[str], ort_version: str, ort_download_path: str):
+def _download_native_onnx_packages(package_name_list: Set[str], ort_version: str, ort_download_path: str):
     PACKAGE_DOWNLOAD_LINK_MAPPING = {
         "onnxruntime": Template("https://www.nuget.org/api/v2/package/Microsoft.ML.OnnxRuntime/$ort_version"),
         "onnxruntime-gpu": Template("https://www.nuget.org/api/v2/package/Microsoft.ML.OnnxRuntime.Gpu/$ort_version"),
         "onnxruntime-directml": Template(
             "https://www.nuget.org/api/v2/package/Microsoft.ML.OnnxRuntime.DirectML/$ort_version"
         ),
         "onnxruntime-openvino": None,
+        "onnxruntime-genai": Template(
+            "https://www.nuget.org/api/v2/package/Microsoft.ML.OnnxRuntimeGenAI.Managed/$ort_version"
+        ),
+        "onnxruntime-genai-cuda": Template(
+            "https://www.nuget.org/api/v2/package/Microsoft.ML.OnnxRuntime.OnnxRuntimeGenAI.Cuda/$ort_version"
+        ),
+        "onnxruntime-genai-directml": Template(
+            "https://www.nuget.org/api/v2/package/Microsoft.ML.OnnxRuntime.OnnxRuntimeGenAI.DirectML/$ort_version"
+        ),
     }
-    for package_name_tuple in package_name_list:
-        package_name = package_name_tuple[0]
-        download_link = PACKAGE_DOWNLOAD_LINK_MAPPING[package_name]
+    for package_name in package_name_list:
+        download_link = PACKAGE_DOWNLOAD_LINK_MAPPING.get(package_name)
         download_path = str(ort_download_path / f"microsoft.ml.{package_name}.{ort_version}.nupkg")
         if download_link:
             urllib.request.urlretrieve(download_link.substitute(ort_version=ort_version), download_path)
         else:
             logger.warning(
                 "Package %s is not available for packaging. Please manually install the package.", package_name
             )
```

## olive/engine/packaging/sample_code/ONNXModel/python/code_sample.py

```diff
@@ -45,15 +45,15 @@
     execution_mode = session_options.get("execution_mode")
     graph_optimization_level = session_options.get("graph_optimization_level")
     extra_session_config = session_options.get("extra_session_config")
     if inter_op_num_threads:
         sess_options.inter_op_num_threads = inter_op_num_threads
     if intra_op_num_threads:
         sess_options.intra_op_num_threads = intra_op_num_threads
-    if execution_mode:
+    if execution_mode is not None:
         if execution_mode == 0:
             sess_options.execution_mode = onnxruntime.ExecutionMode.ORT_SEQUENTIAL
         elif execution_mode == 1:
             sess_options.execution_mode = onnxruntime.ExecutionMode.ORT_PARALLEL
     if graph_optimization_level:
         sess_options.graph_optimization_level = onnxruntime.GraphOptimizationLevel(graph_optimization_level)
     if extra_session_config:
```

## olive/evaluator/accuracy.py

```diff
@@ -24,20 +24,14 @@
         "f1_score": torchmetrics.F1Score,
         "precision": torchmetrics.Precision,
         "recall": torchmetrics.Recall,
         "auroc": torchmetrics.AUROC,
         "perplexity": torchmetrics.text.perplexity.Perplexity,
     }
 
-    @classmethod
-    @property
-    @abstractmethod
-    def name(cls):
-        raise NotImplementedError
-
     def __init__(self, config: Union[ConfigBase, Dict[str, Any]] = None) -> None:
         super().__init__(config)
         self.resolve_kwargs()
 
     def resolve_kwargs(self):
         config_dict = self.config.dict()
         kwargs = config_dict.pop("kwargs", {})
```

## olive/evaluator/metric.py

```diff
@@ -1,17 +1,16 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
-import json
 import logging
 from enum import Enum
-from typing import ClassVar, Dict, List, Optional, Union
+from typing import List, Optional, Union
 
-from olive.common.config_utils import ConfigBase, ConfigDictBase, validate_config
+from olive.common.config_utils import ConfigBase, validate_config
 from olive.common.pydantic_v1 import validator
 from olive.data.config import DataConfig
 from olive.evaluator.accuracy import AccuracyBase
 from olive.evaluator.metric_config import LatencyMetricConfig, MetricGoal, ThroughputMetricConfig, get_user_config_class
 
 logger = logging.getLogger(__name__)
 
@@ -187,54 +186,14 @@
         if "type" not in values:
             raise ValueError("Invalid type")
 
         user_config_class = get_user_config_class(values["type"])
         return validate_config(v, user_config_class)
 
 
-class SubMetricResult(ConfigBase):
-    value: Union[float, int]
-    priority: int
-    higher_is_better: bool
-
-
-class MetricResult(ConfigDictBase):
-    __root__: Dict[str, SubMetricResult]
-    delimiter: ClassVar[str] = "-"
-
-    def get_value(self, metric_name, sub_type_name):
-        if not self.__root__:
-            return None
-        return self.__root__[joint_metric_key(metric_name, sub_type_name)].value
-
-    def get_all_sub_type_metric_value(self, metric_name):
-        return {k.split(self.delimiter)[-1]: v.value for k, v in self.__root__.items() if k.startswith(metric_name)}
-
-    def __str__(self) -> str:
-        repr_obj = {k: v.value for k, v in self.__root__.items()}
-        return json.dumps(repr_obj, indent=2)
-
-
-def joint_metric_key(metric_name, sub_type_name):
-    return f"{metric_name}{MetricResult.delimiter}{sub_type_name}"
-
-
-def flatten_metric_sub_type(metric_dict: Dict[str, Dict]):
-    flatten_results = {}
-    for metric_name, metric_res in metric_dict.items():
-        for sub_type_name, sub_type_res in metric_res.items():
-            key = joint_metric_key(metric_name, sub_type_name)
-            flatten_results[key] = sub_type_res
-    return flatten_results
-
-
-def flatten_metric_result(dict_results: Dict[str, MetricResult]):
-    return MetricResult.parse_obj(flatten_metric_sub_type(dict_results))
-
-
 def get_latency_config_from_metric(metric: Metric):
     warmup_num, repeat_test_num, sleep_num = None, None, None
     for sub_type in metric.sub_types:
         if sub_type.metric_config:
             warmup_num = sub_type.metric_config.warmup_num
             repeat_test_num = sub_type.metric_config.repeat_test_num
             sleep_num = sub_type.metric_config.sleep_num
```

## olive/evaluator/metric_backend.py

```diff
@@ -1,48 +1,51 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 from abc import abstractmethod
-from typing import Any, ClassVar, Dict, NamedTuple, Tuple, Type, Union
+from typing import TYPE_CHECKING, Any, ClassVar, Dict, NamedTuple, Tuple, Type, Union
 
 from olive.common.auto_config import AutoConfigClass, ConfigBase
 from olive.common.config_utils import ConfigParam
 from olive.evaluator.accuracy import AccuracyBase
-from olive.evaluator.metric import Metric, MetricResult, SubMetric, SubMetricResult
+from olive.evaluator.metric_result import MetricResult, SubMetricResult
+
+if TYPE_CHECKING:
+    from olive.evaluator.metric import Metric, SubMetric
 
 
 class MetricBackend(AutoConfigClass):
     registry: ClassVar[Dict[str, Type["MetricBackend"]]] = {}
 
     def __init__(self, config: Union[ConfigBase, Dict[str, Any]] = None) -> None:
         super().__init__(config)
 
     @classmethod
     def _default_config(cls) -> Dict[str, ConfigParam]:
         return {}
 
     @abstractmethod
     def measure_sub_metric(
-        self, model_output: Union[Tuple, NamedTuple], targets: Any, sub_metric: SubMetric
+        self, model_output: Union[Tuple, NamedTuple], targets: Any, sub_metric: "SubMetric"
     ) -> SubMetricResult:
         # model_output: (preds, logits)
         raise NotImplementedError
 
-    def measure(self, model_output, targets, metrics: Metric) -> MetricResult:
+    def measure(self, model_output, targets, metrics: "Metric") -> MetricResult:
         metric_results_dict = {}
         for sub_metric in metrics.sub_types:
             metric_results_dict[sub_metric.name] = self.measure_sub_metric(model_output, targets, sub_metric)
         return MetricResult.parse_obj(metric_results_dict)
 
 
 class TorchMetrics(MetricBackend):
     name: str = "torch_metrics"
 
-    def measure_sub_metric(self, model_output, targets, sub_metric: SubMetric) -> SubMetricResult:
+    def measure_sub_metric(self, model_output, targets, sub_metric: "SubMetric") -> SubMetricResult:
         metric_cls = AccuracyBase.registry[sub_metric.name.value]
         metric_obj = metric_cls(sub_metric.metric_config)
         result = metric_obj.measure(model_output, targets)
         return SubMetricResult(
             value=result,
             priority=sub_metric.priority,
             higher_is_better=sub_metric.higher_is_better,
@@ -76,15 +79,15 @@
                     "The key used to extract the metric result with given format."
                     "For example, if the metric result is {'accuracy': {'value': 0.9}},"
                     "then the result_key should be 'accuracy.value'."
                 ),
             ),
         }
 
-    def measure_sub_metric(self, model_output, targets, sub_metric: SubMetric) -> SubMetricResult:
+    def measure_sub_metric(self, model_output, targets, sub_metric: "SubMetric") -> SubMetricResult:
         load_params = sub_metric.metric_config.load_params or {}
         evaluator = self.evaluate_module.load(sub_metric.name, **load_params)
 
         compute_params = sub_metric.metric_config.compute_params or {}
         result = evaluator.compute(predictions=model_output[0], references=targets, **compute_params)
         if not result:
             raise ValueError(
```

## olive/evaluator/metric_config.py

```diff
@@ -4,15 +4,15 @@
 # --------------------------------------------------------------------------
 import logging
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Union
 
 from olive.common.config_utils import ConfigBase, ConfigParam, ParamCategory, create_config_class
 from olive.common.pydantic_v1 import validator
-from olive.resource_path import OLIVE_RESOURCE_ANNOTATIONS
+from olive.resource_path import OLIVE_RESOURCE_ANNOTATIONS, validate_resource_path
 
 logger = logging.getLogger(__name__)
 
 WARMUP_NUM = 10
 REPEAT_TEST_NUM = 20
 SLEEP_NUM = 0
 
@@ -27,15 +27,17 @@
     "input_names": ConfigParam(type_=List),
     "input_shapes": ConfigParam(type_=List),
     "input_types": ConfigParam(type_=List),
     "shared_kv_buffer": ConfigParam(type_=bool, default_value=False),
     "io_bind": ConfigParam(type_=bool, default_value=False),
 }
 
-_common_user_config_validators = {}
+_common_user_config_validators = {
+    "validate_data_dir_resource_path": validator("data_dir", allow_reuse=True)(validate_resource_path)
+}
 
 _type_to_user_config = {
     "accuracy": {
         "post_processing_func": ConfigParam(type_=Union[Callable, str], category=ParamCategory.OBJECT),
     },
     "custom": {
         "post_processing_func": ConfigParam(type_=Union[Callable, str], category=ParamCategory.OBJECT),
```

## olive/evaluator/olive_evaluator.py

```diff
@@ -18,26 +18,17 @@
 from olive.cache import get_local_path_from_root
 from olive.common.config_utils import ConfigBase
 from olive.common.ort_inference import OrtInferenceSession, prepare_io_bindings
 from olive.common.pydantic_v1 import validator
 from olive.common.user_module_loader import UserModuleLoader
 from olive.common.utils import tensor_data_to_device
 from olive.constants import Framework
-from olive.evaluator.metric import (
-    LatencySubType,
-    Metric,
-    MetricResult,
-    MetricType,
-    SubMetricResult,
-    ThroughputSubType,
-    flatten_metric_result,
-    get_latency_config_from_metric,
-    joint_metric_key,
-)
+from olive.evaluator.metric import LatencySubType, Metric, MetricType, ThroughputSubType, get_latency_config_from_metric
 from olive.evaluator.metric_backend import MetricBackend
+from olive.evaluator.metric_result import MetricResult, SubMetricResult, flatten_metric_result, joint_metric_key
 from olive.hardware import Device
 from olive.model import DistributedOnnxModelHandler, ONNXModelHandler
 from olive.model.config.io_config import is_io_config_static
 from olive.model.utils.onnx_utils import dump_tuning_result
 from olive.platform_sdk.qualcomm.utils.data_loader import FileListCommonDataLoader, FileListDataLoader
 
 if TYPE_CHECKING:
@@ -231,19 +222,23 @@
         # if the io_config is not specified in the metrics, use the one in the model
         # should not change the original metric object which is created from config jsons
         # otherwise, if affects hashing + caching of the olive restoring.
         metric = deepcopy(metric)
         if metric.data_config:
             return metric
 
-        io_config = model.get_io_config()
+        io_config = model.io_config
         if not io_config:
             return metric
 
         if not is_io_config_static(io_config):
+            # since Olive will not save the pytorch model's io_config to olive onnx model
+            # we cannot generate dummy data for the onnx model if this model has dynamic input shapes
+            # TODO(trajep): try to get static input shapes from onnx model.
+            # If so, we can move the dataloader for latency measurement.
             logger.debug(
                 "Model input shapes are not static. Cannot use inferred input shapes for creating dummy data. This will"
                 " cause an error when creating dummy data for tuning."
             )
         if io_config and not metric.user_config.input_names and not metric.user_config.input_shapes:
             metric.user_config.input_names = io_config["input_names"]
             # input_shapes is optional for hf models
@@ -435,15 +430,15 @@
         session = model.prepare_session(
             inference_settings=inference_settings,
             device=device,
             execution_providers=execution_providers,
         )
 
         # prepare for io binding
-        io_config = model.get_io_config()
+        io_config = model.io_config
         io_bind = OnnxEvaluator.io_bind_enabled(metric, model.inference_settings)
         shared_kv_buffer = metric.user_config.shared_kv_buffer
         use_fp16 = any(v == "float16" for v in io_config["input_types"])
         input_feed = None
         if io_bind and shared_kv_buffer and use_fp16:
             input_feed = OnnxEvaluator.format_input(next(iter(dataloader))[0], io_config)
 
@@ -473,15 +468,15 @@
         post_func=None,
         device: Device = Device.CPU,
         execution_providers: Union[str, List[str]] = None,
     ) -> Tuple[OliveModelOutput, Any]:
         session, inference_settings = OnnxEvaluator.get_session_wrapper(
             model, metric, dataloader, device, execution_providers
         )
-        io_config = model.get_io_config()
+        io_config = model.io_config
 
         preds = []
         targets = []
         logits = []
         logits_dict = collections.defaultdict(list)
         output_names = io_config["output_names"]
         is_single_tensor_output = len(output_names) == 1
@@ -536,15 +531,15 @@
         execution_providers: Union[str, List[str]] = None,
     ) -> List[float]:
         warmup_num, repeat_test_num, sleep_num = get_latency_config_from_metric(metric)
 
         session, inference_settings = OnnxEvaluator.get_session_wrapper(
             model, metric, dataloader, device, execution_providers
         )
-        io_config = model.get_io_config()
+        io_config = model.io_config
 
         input_data, _ = next(iter(dataloader))
         input_feed = OnnxEvaluator.format_input(input_data, io_config)
 
         latencies = session.time_run(
             input_feed,
             num_runs=repeat_test_num,
@@ -582,15 +577,15 @@
             for provider in execution_providers
         ]
 
         model = ONNXModelHandler(model_path, inference_settings=inference_settings)
         dataloader, _, post_func = OnnxEvaluator.get_user_config(model.framework, data_root, metric)
 
         session = model.prepare_session(inference_settings=inference_settings, device=Device.GPU, rank=int(local_rank))
-        io_config = model.get_io_config()
+        io_config = model.io_config
 
         preds = []
         targets = []
         logits = []
         output_names = io_config["output_names"]
         for _, (input_data, labels) in enumerate(dataloader):
             input_dict = OnnxEvaluator.format_input(input_data, io_config)
@@ -667,15 +662,15 @@
             {"device_id": str(local_rank)} if provider == "CUDAExecutionProvider" else {}
             for provider in execution_providers
         ]
 
         model = ONNXModelHandler(model_path, inference_settings=inference_settings)
         dataloader, _, _ = OnnxEvaluator.get_user_config(model.framework, data_root, metric)
         session = model.prepare_session(inference_settings=inference_settings, device=Device.GPU, rank=int(local_rank))
-        io_config = model.get_io_config()
+        io_config = model.io_config
 
         input_feed, _ = next(iter(dataloader))
         input_feed = OnnxEvaluator.format_input(input_feed, io_config)
         kv_cache_ortvalues = {} if metric.user_config.shared_kv_buffer else None
 
         io_bind = OnnxEvaluator.io_bind_enabled(metric, model.inference_settings)
         if io_bind:
@@ -920,15 +915,14 @@
         targets = []
         logits = []
         for data_dir, input_list, labels in dataloader:
             result = session(input_list, data_dir)
             # as the SNPE inference will return a list of outputs which is beyond the model output shape
             # we need to squeeze the fist dimensions of output to get right accuracy metrics
             for idx, output in enumerate(result.get("results")):
-                post_output = output
                 if post_func:
                     post_output = post_func(output)
                 else:
                     raise ValueError("Post processing function is required for SNPE model")
                 preds.extend(post_output.tolist())
                 if isinstance(labels[idx], (list, np.ndarray)):
                     targets.extend(labels[idx])
@@ -1060,15 +1054,14 @@
 
         preds = []
         targets = []
         logits = []
         for data_dir, input_list, labels in dataloader:
             result = session(input_list, data_dir)
             for idx, output in enumerate(result.get("result")):
-                post_output = output
                 if post_func:
                     post_output = post_func(output)
                 else:
                     raise ValueError("Post processing function is required for QNN model")
                 preds.extend(post_output.tolist())
                 if isinstance(labels[idx], (list, np.ndarray)):
                     targets.extend(labels[idx])
```

## olive/hardware/accelerator.py

```diff
@@ -1,22 +1,18 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 import logging
 from dataclasses import dataclass
 from enum import Enum
-from typing import TYPE_CHECKING, List, Union
+from typing import List, Optional, Union
 
 from olive.hardware.constants import DEVICE_TO_EXECUTION_PROVIDERS
 
-if TYPE_CHECKING:
-    from olive.systems.system_config import SystemConfig
-
-
 logger = logging.getLogger(__name__)
 
 
 class Device(str, Enum):
     CPU = "cpu"
     CPU_SPR = "cpu_spr"
     GPU = "gpu"
@@ -29,30 +25,34 @@
 
 
 @dataclass(frozen=True, eq=True)
 class AcceleratorSpec:
     """Accelerator specification is the concept of a hardware device that be used to optimize or evaluate a model."""
 
     accelerator_type: Union[str, Device]
-    execution_provider: str
+    execution_provider: Optional[str] = None
     vender: str = None
     version: str = None
     memory: int = None
     num_cores: int = None
 
     def __str__(self) -> str:
-        # remove the suffix "ExecutionProvider", len("ExecutionProvider") = 17
-        ep = self.execution_provider[:-17] or self.execution_provider
-        return f"{str(self.accelerator_type).lower()}-{ep.lower()}"
+        if self.execution_provider:
+            # remove the suffix "ExecutionProvider", len("ExecutionProvider") = 17
+            ep = self.execution_provider[:-17]
+            return f"{str(self.accelerator_type).lower()}-{ep.lower()}"
+        else:
+            return str(self.accelerator_type).lower()
 
     def to_json(self):
-        return {
-            "accelerator_type": str(self.accelerator_type),
-            "execution_provider": self.execution_provider,
-        }
+        json_data = {"accelerator_type": str(self.accelerator_type)}
+        if self.execution_provider:
+            json_data["execution_provider"] = self.execution_provider
+
+        return json_data
 
 
 DEFAULT_CPU_ACCELERATOR = AcceleratorSpec(accelerator_type=Device.CPU, execution_provider="CPUExecutionProvider")
 DEFAULT_GPU_CUDA_ACCELERATOR = AcceleratorSpec(accelerator_type=Device.GPU, execution_provider="CUDAExecutionProvider")
 DEFAULT_GPU_TRT_ACCELERATOR = AcceleratorSpec(
     accelerator_type=Device.GPU, execution_provider="TensorrtExecutionProvider"
 )
@@ -69,15 +69,15 @@
 
         return AcceleratorLookup.get_execution_providers_for_device_by_available_providers(
             device, onnxruntime.get_available_providers()
         )
 
     @staticmethod
     def get_execution_providers_for_device_by_available_providers(device: Device, available_providers):
-        eps_per_device = [*DEVICE_TO_EXECUTION_PROVIDERS.get(device), "CPUExecutionProvider"]
+        eps_per_device = AcceleratorLookup.get_managed_supported_execution_providers(device)
         return AcceleratorLookup.get_execution_providers(eps_per_device, available_providers)
 
     @staticmethod
     def get_execution_providers(execution_providers, available_providers):
         eps = AcceleratorLookup.filter_execution_providers(execution_providers, available_providers)
         return eps or available_providers
 
@@ -162,164 +162,7 @@
             assert len(inferred_devices) == 1, (
                 f"Cannot infer the devices from the execution providers {execution_providers}. "
                 f"Multiple devices are inferred: {inferred_devices}."
                 " Please specify the device in the accelerator configs."
             )
 
         return inferred_devices[0]
-
-
-def normalize_accelerators(system_config: "SystemConfig", skip_supported_eps_check: bool = True) -> "SystemConfig":
-    """Normalize the accelerators in the system config.
-
-    * the accelerators is not specified, infer the device/ep based on the installed ORT in case of local/python system.
-    * only device is specified, infer the execution providers based on the installed ORT in case of local/python system.
-    * only EP is specified, infer the device based on the installed ORT in case of local/python system.
-    * For AzureML and Docker system, the accelerators and execution providers must be specified.
-    """
-    from olive.systems.common import SystemType
-
-    if system_config.olive_managed_env:
-        if not system_config.config.accelerators:
-            raise ValueError("Managed environment requires accelerators to be specified.")
-
-        for accelerator in system_config.config.accelerators:
-            if not accelerator.execution_providers:
-                raise ValueError(
-                    f"Managed environment requires execution providers to be specified for {accelerator.device}"
-                )
-    else:
-        if system_config.type in (SystemType.Local, SystemType.PythonEnvironment, SystemType.IsolatedORT):
-            target = system_config.create_system()
-            # TODO(myguo): Handle the ORT not installed scenario. In this case, the call will raise ImportError.
-            # and the system_supported_eps will be None.
-            system_supported_eps = target.get_supported_execution_providers()
-            # Remove the AzureMLExecutionProvider
-            if "AzureExecutionProvider" in system_supported_eps:
-                system_supported_eps.remove("AzureExecutionProvider")
-
-            assert system_supported_eps, "No supported execution providers found for the target system."
-
-            if not system_config.config.accelerators:
-                # User does not specify the accelerators.
-                inferred_device = AcceleratorLookup.infer_single_device_from_execution_providers(system_supported_eps)
-                # here the pydantic validate_assignment will initialize the accelerator instances
-                system_config.config.accelerators = [
-                    {"device": inferred_device, "execution_providers": system_supported_eps}
-                ]
-                logger.info(
-                    "There is no any accelerator specified. Inferred accelerators: %s",
-                    system_config.config.accelerators,
-                )
-            else:
-                for accelerator in system_config.config.accelerators:
-                    if not accelerator.device:
-                        # User does not specify the device but providing the execution providers
-                        assert accelerator.execution_providers, "The execution providers are not specified."
-                        inferred_device = AcceleratorLookup.infer_single_device_from_execution_providers(
-                            accelerator.execution_providers
-                        )
-                        logger.info("the accelerator device is not specified. Inferred device: %s.", inferred_device)
-                        accelerator.device = inferred_device
-                    elif not accelerator.execution_providers:
-                        # User specify the device but missing the execution providers
-                        execution_providers = (
-                            AcceleratorLookup.get_execution_providers_for_device_by_available_providers(
-                                accelerator.device.lower(), system_supported_eps
-                            )
-                        )
-                        accelerator.execution_providers = execution_providers
-                        filtered_eps = [ep for ep in system_supported_eps if ep not in execution_providers]
-                        if filtered_eps:
-                            logger.warning(
-                                "The following execution providers are filtered: %s. "
-                                "Please raise issue in Olive site since it might be a bug. ",
-                                ",".join(filtered_eps),
-                            )
-
-                        logger.info(
-                            "The accelerator execution providers is not specified for %s. Use the inferred ones. %s",
-                            accelerator.device,
-                            accelerator.execution_providers,
-                        )
-                    else:
-                        logger.debug("The accelerator device and execution providers are specified, skipping deduce.")
-        else:
-            # for AzureML and Docker System
-            if not system_config.config.accelerators:
-                raise ValueError("AzureML and Docker system requires accelerators to be specified.")
-            for accelerator in system_config.config.accelerators:
-                if not accelerator.device or not accelerator.execution_providers:
-                    raise ValueError(
-                        "AzureML and Docker system requires device and execution providers to be specified explicitly."
-                    )
-
-    ep_not_supported = []
-    for accelerator in system_config.config.accelerators:
-        device = Device(accelerator.device.lower())
-
-        if system_config.olive_managed_env:
-            available_eps = AcceleratorLookup.get_managed_supported_execution_providers(device)
-        elif (
-            system_config.type in (SystemType.Local, SystemType.PythonEnvironment, SystemType.IsolatedORT)
-            and not skip_supported_eps_check
-        ):
-            # don't need to check the supported execution providers if there is no evaluation
-            # target is only used for evaluation
-            available_eps = system_supported_eps
-        else:
-            available_eps = accelerator.execution_providers
-
-        supported_eps = AcceleratorLookup.get_execution_providers_for_device_by_available_providers(
-            device, available_eps
-        )
-        logger.debug("Supported execution providers for device %s: %s", device, supported_eps)
-
-        eps = []
-        for ep in accelerator.execution_providers:
-            if ep not in supported_eps:
-                ep_not_supported.append(ep)
-            else:
-                eps.append(ep)
-
-        # remove the unsupported execution providers
-        accelerator.execution_providers = eps
-
-    if ep_not_supported:
-        logger.warning(
-            "The following execution providers are not supported: %s. "
-            "Please consider installing an onnxruntime build that contains the relevant execution providers. ",
-            ",".join(ep_not_supported),
-        )
-    return system_config
-
-
-def create_accelerators(system_config: "SystemConfig", skip_supported_eps_check: bool = True) -> List[AcceleratorSpec]:
-    system_config = normalize_accelerators(system_config, skip_supported_eps_check)
-
-    device_to_eps = {}
-    for accelerator in system_config.config.accelerators:
-        device_to_eps[accelerator.device] = accelerator.execution_providers
-    logger.debug("Initial accelerators and execution providers: %s", device_to_eps)
-
-    # Flatten the accelerators to list of AcceleratorSpec
-    accelerator_specs: List[AcceleratorSpec] = []
-    is_cpu_available = "cpu" in [accelerator.lower() for accelerator in device_to_eps]
-    for accelerator in system_config.config.accelerators:
-        device = Device(accelerator.device.lower())
-        for ep in accelerator.execution_providers:
-            if ep == "CPUExecutionProvider" and device != "cpu" and is_cpu_available:
-                logger.warning(
-                    "Ignore the CPUExecutionProvider for non-cpu device since cpu accelerator is also present."
-                )
-            else:
-                accelerator_specs.append(AcceleratorSpec(device, ep))
-
-    assert accelerator_specs, (
-        "No valid accelerator specified for target system. "
-        "Please specify the accelerators in the target system or provide valid execution providers. "
-        f"Given execution providers: {device_to_eps.values()}. "
-        f"Current accelerators: {device_to_eps.keys()}."
-        f"Supported execution providers: {DEVICE_TO_EXECUTION_PROVIDERS}."
-    )
-    logger.info("Running workflow on accelerator specs: %s", ",".join([str(spec) for spec in accelerator_specs]))
-    return accelerator_specs
```

## olive/hardware/constants.py

```diff
@@ -24,10 +24,11 @@
     "gpu": [
         "DmlExecutionProvider",
         "CUDAExecutionProvider",
         "ROCMExecutionProvider",
         "MIGraphXExecutionProvider",
         "TensorrtExecutionProvider",
         "OpenVINOExecutionProvider",
+        "JsExecutionProvider",
     ],
     "npu": ["QNNExecutionProvider"],
 }
```

## olive/model/config/__init__.py

```diff
@@ -1,9 +1,22 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 from olive.model.config.hf_config import HfComponent, HfConfig
-from olive.model.config.io_config import IoConfig
+from olive.model.config.io_config import (
+    IoConfig,
+    complete_kv_cache_with_model_attributes,
+    extend_io_config_with_kv_cache,
+)
+from olive.model.config.kv_cache_config import KVCacheConfig
 from olive.model.config.model_config import ModelConfig
 
-__all__ = ["HfComponent", "HfConfig", "IoConfig", "ModelConfig"]
+__all__ = [
+    "HfComponent",
+    "HfConfig",
+    "IoConfig",
+    "KVCacheConfig",
+    "ModelConfig",
+    "extend_io_config_with_kv_cache",
+    "complete_kv_cache_with_model_attributes",
+]
```

## olive/model/config/hf_config.py

```diff
@@ -121,15 +121,20 @@
             raise ValueError("Invalid quantization_config")
         if (values["quantization_method"] and not v) or (not values["quantization_method"] and v):
             raise ValueError("quantization_config and quantization_method must be provided together")
         if not v:
             return v
 
         try:
-            return cls.dict_to_quantization_config(values["quantization_method"], v).to_dict()
+            full_config = cls.dict_to_quantization_config(values["quantization_method"], v).to_dict()
+            # in newer versions to_dict has extra keys quant_method, _load_in_4bit and _load_in_8bit
+            # which are internal attributes and not part of init params
+            for key in ["quant_method", "_load_in_4bit", "_load_in_8bit"]:
+                full_config.pop(key, None)
+            return full_config
         except ImportError:
             # we don't want to fail since the pass target might have the correct transformers version
             logger.warning(
                 "Could not import the config class for quantization method %s. Skipping validation",
                 values["quantization_method"],
             )
             return v
@@ -238,15 +243,14 @@
     task: str = None
     # feature is optional if task is specified and don't need past
     # else, provide feature such as "causal-lm-with-past"
     feature: str = None
     # TODO(xiaoyu): remove model_class and only use task
     model_class: str = None
     components: List[HfComponent] = None
-    dataset: Dict[str, Any] = None
     from_pretrained_args: HfFromPretrainedArgs = None
 
     @validator("model_class", always=True)
     def task_or_model_class_required(cls, v, values):
         if values["model_name"] and not v and not values.get("task", None):
             raise ValueError("Either task or model_class must be specified")
         return v
```

## olive/model/config/io_config.py

```diff
@@ -1,28 +1,33 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
-from typing import Dict, List, Union
+from copy import deepcopy
+from typing import Any, Dict, List, Union
 
 from olive.common.config_utils import ConfigBase
 from olive.common.pydantic_v1 import validator
+from olive.common.utils import find_first_matched_value
+from olive.model.config.kv_cache_config import KVCacheConfig
+from olive.model.utils.hf_mappings import HIDDEN_SIZE_NAMES, NUM_HEADS_NAMES, NUM_HIDDEN_LAYER_NAMES
 
 
 class IoConfig(ConfigBase):
     """IO config for model handler.
 
     For example, in stable diffusion, the config looks like:
     "io_config": {
         "input_names": [ "clip_input", "images" ],
         "output_names": [ "out_images", "has_nsfw_concepts" ],
         "dynamic_axes": {
             "clip_input": { "0": "batch", "1": "channels", "2": "height", "3": "width" },
             "images": { "0": "batch", "1": "height", "2": "width", "3": "channels" }
-        }
+        },
+        "kv_cache": None
     }
     """
 
     # TODO(trajep): remove input names, shapes and types, turn to use olive dataset config.
     input_names: List[str]
     input_shapes: List[List[int]] = None
     input_types: List[str] = None
@@ -31,14 +36,18 @@
     output_types: List[str] = None
     dynamic_axes: Dict[str, Dict[int, str]] = None
     # ONNX exporter might mark dimension like 'Transposepresent_value_self_1_dim_2' in shape inference
     # even though we want the dimension to be a constant int.
     # We use a workaround here: first use dim_param like "1" to represent the dimension, and then
     # convert it to int in the onnx model.
     string_to_int_dim_params: List[str] = None
+    # if False, skip kv_cache input
+    # if True, use default KVCacheConfig
+    # if KVCacheConfig, use the provided KVCacheConfig
+    kv_cache: Union[bool, Dict[str, Any], KVCacheConfig] = False
 
     @validator("input_shapes", "input_types")
     def check_input_shapes(cls, v, values):
         if not v:
             return v
 
         if "input_names" not in values:
@@ -76,24 +85,108 @@
         for dim_param in v:
             try:
                 int(dim_param)
             except ValueError:
                 raise ValueError(f"Invalid string_to_int_dim_params: {dim_param}. Must be castable to int.") from None
         return v
 
+    def get_seq_len(self):
+        if not self.input_shapes or not self.input_names:
+            return 0
+        for idx, name in enumerate(self.input_names):
+            if name == "input_ids":
+                return self.input_shapes[idx][1]  # pylint: disable=E1136
+        return 0
+
+    def get_past_seq_len(self):
+        if not self.input_shapes or not self.input_names:
+            return 0
+        attention_mask_len, seq_len = 0, 0
+        for idx, name in enumerate(self.input_names):
+            if name == "attention_mask":
+                attention_mask_len = self.input_shapes[idx][1]  # pylint: disable=E1136
+            if name == "input_ids":
+                seq_len = self.input_shapes[idx][1]  # pylint: disable=E1136
+        return attention_mask_len - seq_len
+
+    def get_batch_size(self):
+        if not self.input_shapes or not self.input_names:
+            return 1
+        for idx, name in enumerate(self.input_names):
+            if name == "input_ids":
+                return self.input_shapes[idx][0]  # pylint: disable=E1136
+        # if no input_ids, return 1
+        return 1
+
+
+def complete_kv_cache_with_model_attributes(kv_cache, model_attributes):
+    num_hidden_layers = find_first_matched_value(model_attributes, NUM_HIDDEN_LAYER_NAMES)
+    num_attention_heads = find_first_matched_value(model_attributes, NUM_HEADS_NAMES)
+    hidden_size = find_first_matched_value(model_attributes, HIDDEN_SIZE_NAMES)
+    kv_cache_obj = None
+    if isinstance(kv_cache, bool) and kv_cache:
+        kv_cache_obj = KVCacheConfig(
+            num_hidden_layers=num_hidden_layers,
+            num_attention_heads=num_attention_heads,
+            hidden_size=hidden_size,
+        )
+    elif isinstance(kv_cache, dict):
+        kv_cache_dict = deepcopy(kv_cache)
+        kv_cache_dict.update(
+            {
+                "num_hidden_layers": kv_cache.get("num_hidden_layers") or num_hidden_layers,
+                "num_attention_heads": kv_cache.get("num_attention_heads") or num_attention_heads,
+                "hidden_size": kv_cache.get("hidden_size") or hidden_size,
+            }
+        )
+        kv_cache_obj = KVCacheConfig.parse_obj(kv_cache_dict)
+    elif isinstance(kv_cache, KVCacheConfig):
+        # as num_hidden_layers, num_attention_heads, hidden_size are required for kv_cache
+        # there is no need to update them
+        kv_cache_obj = kv_cache
+
+    if not kv_cache_obj.num_hidden_layers or not kv_cache_obj.num_attention_heads or not kv_cache_obj.hidden_size:
+        raise ValueError(
+            "num_hidden_layers, num_attention_heads, and hidden_size cannot be 0 or None, they"
+            "are required for kv_cache."
+        )
+    return kv_cache_obj
+
+
+def extend_io_config_with_kv_cache(io_config, kv_cache_config: KVCacheConfig):
+    kv_cache_config.past_sequence_length = kv_cache_config.past_sequence_length or io_config.get_past_seq_len()
+    kv_cache_config.batch_size = kv_cache_config.batch_size or io_config.get_batch_size()
+
+    kv_names, kv_shapes, kv_types = kv_cache_config.get_input_names_shapes_types()
+    output_names = kv_cache_config.get_output_names()
+    dynamic_axes = deepcopy(io_config.dynamic_axes or {})
+    dynamic_axes.update(kv_cache_config.get_dynamic_axes())
+    return IoConfig(
+        input_names=(io_config.input_names or []) + kv_names,
+        input_shapes=(io_config.input_shapes or []) + kv_shapes,
+        input_types=(io_config.input_types or []) + kv_types,
+        output_names=(io_config.output_names or []) + output_names,
+        output_shapes=io_config.output_shapes,  # ignore kv_cache output shapes
+        output_types=io_config.output_types,  # ignore kv_cache output types
+        dynamic_axes=dynamic_axes,
+        kv_cache=kv_cache_config,
+    )
+
 
 def is_io_config_static(config: Union[IoConfig, Dict]):
     if isinstance(config, IoConfig):
         config = config.dict()
     if not config.get("input_shapes"):
         return False
     return all(all(isinstance(dim, int) for dim in shape) for shape in config["input_shapes"])
 
 
 def is_kv_cache_required(input_past_kv_list, io_config: IoConfig):
+    if io_config.kv_cache:
+        return True
     # In the case of dynamo exporting, user do not need to provide input names
     # for past_key_values in huggingface pytorch model, when exported to onnx
     # and after PhiOnnxModel optimization, the pass_key_value will be extended as
     # `past_(key|value)_(hidden_layer_num)` pattern (phi2 case)
     # https://github.com/Microsoft/onnxruntime/blob/f53d2c2465d81cdb4e14c7241eab327184192c88/onnxruntime/python/tools/transformers/onnx_model_phi.py#L845C1-L845C31
     hidden_layer_num = len(input_past_kv_list)
     # possible kv-related variables which might be provided by the user
```

## olive/model/handler/base.py

```diff
@@ -1,13 +1,15 @@
 import logging
 from abc import ABC, abstractmethod
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
+from olive.common.config_utils import validate_config
 from olive.constants import Framework, ModelFileFormat
 from olive.hardware.accelerator import Device
+from olive.model.config import IoConfig
 from olive.model.handler.mixin import CompositeMixin, IoConfigMixin, JsonMixin, ResourceMixin
 from olive.resource_path import OLIVE_RESOURCE_ANNOTATIONS
 
 logger = logging.getLogger(__name__)
 
 
 class OliveModelHandler(ABC, ResourceMixin, IoConfigMixin, JsonMixin, CompositeMixin):
@@ -32,20 +34,25 @@
 
     def __init__(
         self,
         framework: Framework,
         model_file_format: ModelFileFormat,
         model_path: OLIVE_RESOURCE_ANNOTATIONS = None,
         model_attributes: Optional[Dict[str, Any]] = None,
+        io_config: Union[Dict[str, Any], "IoConfig", str, Callable] = None,
     ):
         self.framework = framework
         self.model_file_format = model_file_format
         self.composite_parent = None
         self.model_attributes = model_attributes
-        self.io_config = None
+        self._io_config = (
+            validate_config(io_config, IoConfig).dict(exclude_none=True)
+            if isinstance(io_config, (IoConfig, dict))
+            else io_config
+        )
 
         # store resource paths
         self.resource_paths: Dict[str, str] = {}
 
         # Only update the resource_paths when the resource_key is model_path.
         # All other case will be handled by subclass.
         if len(self.resource_keys) == 1 and self.resource_keys[0] == "model_path":
```

## olive/model/handler/onnx.py

```diff
@@ -59,15 +59,14 @@
         )
         self.inference_settings = inference_settings
         self.use_ort_extensions = use_ort_extensions
         self.onnx_file_name = onnx_file_name
         self.external_initializers_file_name = external_initializers_file_name
         self.constant_inputs_file_name = constant_inputs_file_name
 
-        self.io_config = None
         self.graph = None
         self.all_graphs: Optional[List[GraphProto]] = None
 
         # check for file names since it will automatically validate the paths
         # these call the property methods which in turn validate the paths using get_onnx_file_path
         # and get_additional_file_path
         to_check = ["model_path", "external_initializers_path", "constant_inputs_path"]
@@ -138,25 +137,26 @@
             inference_settings_merged["provider_options"] = None
 
         # execution_provider should be a list
         if isinstance(inference_settings_merged["execution_provider"], (str, tuple)):
             inference_settings_merged["execution_provider"] = [inference_settings_merged["execution_provider"]]
         return inference_settings_merged
 
-    def get_io_config(self):
+    @property
+    def io_config(self):
         """Get input/output names, shapes, types of the onnx model without creating an ort session.
 
         This function loads the onnx model and parses the graph to get the io config.
         """
-        if self.io_config:
-            return self.io_config
+        if self._io_config:
+            return self._io_config
 
         # save io_config
-        self.io_config = self.get_graph_io_config()
-        return self.io_config
+        self._io_config = self.get_graph_io_config()
+        return self._io_config
 
     def _get_default_execution_providers(self, device: Device):
         # return available ep as ort default ep
         available_providers = AcceleratorLookup.get_execution_providers_for_device(device)
         eps = [ep for ep in available_providers if self.is_valid_ep(self.model_path, ep)]
 
         if not eps:
```

## olive/model/handler/pytorch.py

```diff
@@ -1,52 +1,57 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 import logging
 import os
-import tempfile
 from copy import deepcopy
 from pathlib import Path
 from typing import Any, Callable, ClassVar, Dict, List, Optional, Tuple, Union
 
 import torch
 import yaml
 
 from olive.common.config_utils import serialize_to_json, validate_config
 from olive.common.user_module_loader import UserModuleLoader
-from olive.common.utils import copy_dir
 from olive.constants import Framework, ModelFileFormat
 from olive.hardware.accelerator import Device
-from olive.model.config import HfComponent, HfConfig, IoConfig
+from olive.model.config import (
+    HfComponent,
+    HfConfig,
+    IoConfig,
+    complete_kv_cache_with_model_attributes,
+    extend_io_config_with_kv_cache,
+)
 from olive.model.config.registry import model_handler_registry
 from olive.model.handler.base import OliveModelHandler
-from olive.model.handler.mixin import DummyInputsMixin, HfConfigMixin
+from olive.model.handler.mixin import DummyInputsMixin, HfConfigMixin, MLFlowMixin, PytorchKvCacheMixin
 from olive.model.utils.hf_utils import load_hf_model_from_model_class
 from olive.resource_path import OLIVE_RESOURCE_ANNOTATIONS, ResourceType, create_resource_path
 
 logger = logging.getLogger(__name__)
 
 
 @model_handler_registry("PyTorchModel")
-class PyTorchModelHandler(OliveModelHandler, HfConfigMixin, DummyInputsMixin):  # pylint: disable=too-many-ancestors
+class PyTorchModelHandler(
+    OliveModelHandler, HfConfigMixin, DummyInputsMixin, PytorchKvCacheMixin, MLFlowMixin
+):  # pylint: disable=too-many-ancestors
     """PyTorch model handler.
 
     Besides the model loading for PyTorch model, the model handler also provides the following functionalities:
       * Get the model io configuration either from user provider io_config or from hf_config. The priority is user
         provided io_config is higher than hf_config.
       * Get the dummy inputs for PyTorch model used to evaluate the latency.
       * All kinds of Hf model functionalities by HfConfigMixin.
     """
 
     resource_keys: Tuple[str, ...] = ("model_path", "script_dir", "model_script", "adapter_path")
     json_config_keys: Tuple[str, ...] = (
         "model_file_format",
         "model_loader",
-        "io_config",
         "dummy_inputs_func",
         "hf_config",
     )
 
     def __init__(
         self,
         model_path: OLIVE_RESOURCE_ANNOTATIONS = None,
@@ -55,35 +60,36 @@
         model_script: Union[str, Path] = None,
         script_dir: Union[str, Path] = None,
         io_config: Union[Dict[str, Any], IoConfig, str, Callable] = None,
         dummy_inputs_func: Union[str, Callable] = None,
         hf_config: Union[Dict[str, Any], HfConfig] = None,
         adapter_path: OLIVE_RESOURCE_ANNOTATIONS = None,
         model_attributes: Optional[Dict[str, Any]] = None,
+        mlflow_transformer_model_cache_dir: Optional[str] = None,
     ):
         if not (
             isinstance(model_loader, Callable)
             or (isinstance(model_loader, str) and model_script)
             or model_path
             or hf_config
         ):
             raise ValueError(
                 "model_path is required since model_loader is not callable or model_script is not provided"
             )
-
+        self.mlflow_transformer_model_cache_dir = mlflow_transformer_model_cache_dir
         self.model_loader = model_loader
         self.model = None
         super().__init__(
             framework=Framework.PYTORCH,
             model_file_format=model_file_format,
             model_path=model_path,
             model_attributes=model_attributes,
+            io_config=io_config,
         )
         self.add_resources(locals())
-
         self.hf_config = None
         if hf_config:
             self.hf_config = validate_config(hf_config, HfConfig)
             hf_model_config = self.get_hf_model_config().to_dict()
             model_attr = self.model_attributes or {}
             hf_model_config.update(model_attr)
             self.model_attributes = hf_model_config
@@ -97,35 +103,32 @@
         model_script_resource = create_resource_path(self.model_script)
         if model_script_resource:
             assert model_script_resource.type in (
                 ResourceType.LocalFile,
                 ResourceType.StringName,
             ), "model_script must be a local file or a string name."
 
-        # io config for conversion to onnx
-        self.io_config = (
-            validate_config(io_config, IoConfig).dict() if isinstance(io_config, (IoConfig, dict)) else io_config
-        )
-
         self.dummy_inputs_func = dummy_inputs_func
-
         self.dummy_inputs = None
 
     @property
     def script_dir(self) -> str:
         return self.get_resource("script_dir")
 
     @property
     def model_script(self) -> str:
         return self.get_resource("model_script")
 
     @property
     def adapter_path(self) -> str:
         return self.get_resource("adapter_path")
 
+    def get_mlflow_transformers_dir(self):
+        return self.mlflow_transformer_model_cache_dir or self.model_path
+
     def load_model(self, rank: int = None) -> torch.nn.Module:
         if self.model is not None:
             return self.model
 
         # Load user module at the beginning since we may need user defined models to load model
         user_module_loader = UserModuleLoader(self.model_script, self.script_dir)
 
@@ -189,56 +192,54 @@
         execution_providers: Union[str, List[str]] = None,
         rank: Optional[int] = None,
     ):
         return self.load_model(rank).eval()
 
     def _load_mlflow_model(self):
         logger.info("Loading MLFlow model from %s", self.model_path)
-        with tempfile.TemporaryDirectory(prefix="mlflow_tmp") as tmp_dir:
-            copy_dir(os.path.join(self.model_path, "data/model"), tmp_dir, dirs_exist_ok=True)
-            copy_dir(os.path.join(self.model_path, "data/config"), tmp_dir, dirs_exist_ok=True)
-            copy_dir(os.path.join(self.model_path, "data/tokenizer"), tmp_dir, dirs_exist_ok=True)
-
-            with open(os.path.join(self.model_path, "MLmodel")) as fp:
-                mlflow_data = yaml.safe_load(fp)
-                # default flavor is "hftransformersv2" from azureml.evaluate.mlflow>=0.0.8
-                # "hftransformers" from azureml.evaluate.mlflow<0.0.8
-                # TODO(trajep): let user specify flavor name if needed
-                # to support other flavors in mlflow not only hftransformers
-                hf_pretrained_class = None
-                flavors = mlflow_data.get("flavors", {})
-                if not flavors:
-                    raise ValueError(
-                        "Invalid MLFlow model format. Please make sure the input model"
-                        " format is same with the result of mlflow.transformers.save_model,"
-                        " or aml_mlflow.hftransformers.save_model from azureml.evaluate.mlflow"
-                    )
-
-                if "hftransformersv2" in flavors:
-                    hf_pretrained_class = flavors["hftransformersv2"].get("hf_pretrained_class", "AutoModel")
-                elif "hftransformers" in flavors:
-                    hf_pretrained_class = flavors["hftransformers"].get("hf_pretrained_class", "AutoModel")
-                else:
-                    raise ValueError(
-                        "Unsupported MLFlow model flavor. Currently only support hftransformersv2/hftransformers."
-                    )
-            loading_args = self.hf_config.get_loading_args_from_pretrained() if self.hf_config else {}
-            loaded_model = load_hf_model_from_model_class(hf_pretrained_class, tmp_dir, **loading_args)
-            loaded_model.eval()
-            return loaded_model
+        mlflow_transformers_path = self.to_mlflow_transformer_model(self.get_mlflow_transformers_dir())
+        with open(os.path.join(self.model_path, "MLmodel")) as fp:
+            mlflow_data = yaml.safe_load(fp)
+            # default flavor is "hftransformersv2" from azureml.evaluate.mlflow>=0.0.8
+            # "hftransformers" from azureml.evaluate.mlflow<0.0.8
+            # TODO(trajep): let user specify flavor name if needed
+            # to support other flavors in mlflow not only hftransformers
+            hf_pretrained_class = None
+            flavors = mlflow_data.get("flavors", {})
+            if not flavors:
+                raise ValueError(
+                    "Invalid MLFlow model format. Please make sure the input model"
+                    " format is same with the result of mlflow.transformers.save_model,"
+                    " or aml_mlflow.hftransformers.save_model from azureml.evaluate.mlflow"
+                )
+
+            if "hftransformersv2" in flavors:
+                hf_pretrained_class = flavors["hftransformersv2"].get("hf_pretrained_class", "AutoModel")
+            elif "hftransformers" in flavors:
+                hf_pretrained_class = flavors["hftransformers"].get("hf_pretrained_class", "AutoModel")
+            else:
+                raise ValueError(
+                    "Unsupported MLFlow model flavor. Currently only support hftransformersv2/hftransformers."
+                )
+        loading_args = self.hf_config.get_loading_args_from_pretrained() if self.hf_config else {}
+        loaded_model = load_hf_model_from_model_class(hf_pretrained_class, mlflow_transformers_path, **loading_args)
+        loaded_model.eval()
+        return loaded_model
 
     def _load_slicegpt_model(self):
         logger.info("Loading SliceGPT model from %s", self.model_path)
         from slicgpt.hf_utils import load_sliced_model
 
         loaded_model, _ = load_sliced_model(self.hf_config.model_name, self.model_path)
         return loaded_model
 
     def to_json(self, check_object: bool = False):
         config = super().to_json(check_object)
+        # add _io_config to config to keep what was provided at init
+        config["config"]["io_config"] = self._io_config
         # only keep model_attributes that are not in hf_config
         if self.model_attributes and self.hf_config:
             model_attributes = {}
             hf_config_dict = self.get_hf_model_config().to_dict()
             for key, value in self.model_attributes.items():
                 if key not in hf_config_dict or hf_config_dict[key] != value:
                     model_attributes[key] = value
@@ -246,46 +247,50 @@
         return serialize_to_json(config, check_object)
 
     def get_user_io_config(self, io_config: Union[Dict[str, Any], IoConfig, str, Callable]) -> Dict[str, Any]:
         """Resolve io_config to a dictionary.
 
         If io_config is a string name or a callable, it will be called to get io_config.
         """
+        io_config_obj = None
         if isinstance(io_config, dict):
-            # io_config is provided
-            return io_config
-
-        if isinstance(io_config, IoConfig):
-            # io_config is an IoConfig
-            return io_config.dict()
-
-        if isinstance(io_config, (str, Callable)):
+            io_config_obj = IoConfig.parse_obj(io_config)
+        elif isinstance(io_config, IoConfig):
+            # return a new copy of io_config to avoid modifying the original one
+            io_config_obj = io_config.copy(deep=True)
+        elif isinstance(io_config, (str, Callable)):
             # io_config is a string name or a callable
             logger.debug("Calling %s to get io_config", io_config)
             user_module_loader = UserModuleLoader(self.model_script, self.script_dir)
             io_config = user_module_loader.call_object(io_config, self)
-            return validate_config(io_config, IoConfig).dict()
+            io_config_obj = validate_config(io_config, IoConfig)
+        # TODO(anyone): infer if to use kv_cache from task config
+        if io_config_obj.kv_cache:
+            kv_cache_config = complete_kv_cache_with_model_attributes(io_config_obj.kv_cache, self.model_attributes)
+            io_config_obj = extend_io_config_with_kv_cache(io_config_obj, kv_cache_config)
+        return io_config_obj.dict(exclude_none=True)
 
-        return None
-
-    def get_io_config(self) -> Dict[str, Any]:
+    @property
+    def io_config(self) -> Dict[str, Any]:
         """Return io config of the model.
 
         Priority: io_config > hf_config (using onnx_config)
         """
         io_config = None
-        if self.io_config:
+        if self._io_config:
             # io_config is provided
-            io_config = self.get_user_io_config(self.io_config)
+            io_config = self.get_user_io_config(self._io_config)
         elif self.hf_config and self.hf_config.task and not self.hf_config.components:
             # hf_config is provided
-            logger.debug("Using hf onnx_config to get io_config")
+            logger.debug("Trying hf onnx_config to get io_config")
             # For MLFlow model, get io config from model_name instead of model_path
             # TODO(xiaoyu): more investigation on the integration between MLFlow and HF
             io_config = self.get_hf_io_config()
+            if io_config:
+                logger.debug("Got io_config from hf_config")
 
         return io_config
 
 
 @model_handler_registry("DistributedPyTorchModel")
 class DistributedPyTorchModelHandler(OliveModelHandler, HfConfigMixin):
     resource_keys: Tuple[str, ...] = ("model_path", "script_dir", "model_script", "adapter_path")
@@ -316,24 +321,22 @@
         model_attributes: Optional[Dict[str, Any]] = None,
     ):
         super().__init__(
             framework=Framework.PYTORCH,
             model_file_format=model_file_format,
             model_path=model_path,
             model_attributes=model_attributes,
+            io_config=io_config,
         )
 
         self.add_resources(locals())
 
         self.model_name_pattern = model_name_pattern
         self.num_ranks = num_ranks
         self.model_loader = model_loader
-        self.io_config = (
-            validate_config(io_config, IoConfig).dict() if isinstance(io_config, (IoConfig, dict)) else io_config
-        )
         self.dummy_inputs_func = dummy_inputs_func
         self.hf_config = validate_config(hf_config, HfConfig) if hf_config else None
 
     @property
     def script_dir(self) -> str:
         return self.get_resource("script_dir")
 
@@ -354,15 +357,15 @@
     def load_model(self, rank: int = None) -> PyTorchModelHandler:
         return PyTorchModelHandler(
             model_path=self.ranked_model_path(rank),
             model_file_format=ModelFileFormat.PYTORCH_ENTIRE_MODEL,
             model_loader=self.model_loader,
             model_script=self.model_script,
             script_dir=self.script_dir,
-            io_config=self.io_config,
+            io_config=self._io_config,
             dummy_inputs_func=self.dummy_inputs_func,
             hf_config=self.hf_config,
             adapter_path=self.adapter_path,
             model_attributes=self.model_attributes,
         )
 
     def get_component_model(self, component: HfComponent, rank: int = 0) -> PyTorchModelHandler:
```

## olive/model/handler/qnn.py

```diff
@@ -3,15 +3,14 @@
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 import logging
 import platform
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
-from olive.common.config_utils import validate_config
 from olive.constants import Framework, ModelFileFormat
 from olive.hardware.accelerator import Device
 from olive.model.config import IoConfig
 from olive.model.config.registry import model_handler_registry
 from olive.model.handler.base import OliveModelHandler
 from olive.platform_sdk.qualcomm.qnn.qnn import QNNInferenceSession, QNNSessionOptions
 
@@ -30,18 +29,15 @@
         model_file_format: ModelFileFormat = ModelFileFormat.QNN_CPP,
     ):
         super().__init__(
             framework=Framework.QNN,
             model_file_format=model_file_format,
             model_path=model_path,
             model_attributes=model_attributes,
-        )
-        # io config for conversion to onnx
-        self.io_config = (
-            validate_config(io_config, IoConfig).dict() if isinstance(io_config, (IoConfig, dict)) else io_config
+            io_config=io_config,
         )
 
     @property
     def model_path(self):
         model_path = super().model_path
         if self.model_file_format == ModelFileFormat.QNN_CPP:
             logger.debug("QNNModelHandler: model_path is the cpp file for QNN_CPP model format.")
```

## olive/model/handler/snpe.py

```diff
@@ -27,21 +27,28 @@
         model_attributes: Optional[Dict[str, Any]] = None,
     ):
         super().__init__(
             framework=Framework.SNPE,
             model_file_format=ModelFileFormat.SNPE_DLC,
             model_path=model_path,
             model_attributes=model_attributes,
+            io_config={
+                "input_names": input_names,
+                "input_shapes": input_shapes,
+                "output_names": output_names,
+                "output_shapes": output_shapes,
+            },
         )
-        self.io_config = {
-            "input_names": input_names,
-            "input_shapes": input_shapes,
-            "output_names": output_names,
-            "output_shapes": output_shapes,
-        }
+
+    @property
+    def io_config(self) -> Dict[str, Any]:
+        assert self._io_config, "SNPEModelHandler: io_config is not set"
+
+        keys = {"input_names", "input_shapes", "output_names", "output_shapes"}
+        return {k: v for k, v in self._io_config.items() if k in keys}
 
     def load_model(self, rank: int = None):
         raise NotImplementedError
 
     def prepare_session(
         self,
         inference_settings: Optional[Dict[str, Any]] = None,
```

## olive/model/handler/mixin/__init__.py

```diff
@@ -3,21 +3,25 @@
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 from olive.model.handler.mixin.composite import CompositeMixin
 from olive.model.handler.mixin.dummy_inputs import DummyInputsMixin
 from olive.model.handler.mixin.hf_config import HfConfigMixin
 from olive.model.handler.mixin.io_config import IoConfigMixin
 from olive.model.handler.mixin.json import JsonMixin
+from olive.model.handler.mixin.kv_cache import PytorchKvCacheMixin
+from olive.model.handler.mixin.mlflow import MLFlowMixin
 from olive.model.handler.mixin.onnx_ep import OnnxEpValidateMixin
 from olive.model.handler.mixin.onnx_graph import OnnxGraphMixin
 from olive.model.handler.mixin.resource import ResourceMixin
 
 __all__ = [
     "CompositeMixin",
     "DummyInputsMixin",
     "HfConfigMixin",
     "IoConfigMixin",
     "JsonMixin",
+    "MLFlowMixin",
     "OnnxEpValidateMixin",
     "OnnxGraphMixin",
+    "PytorchKvCacheMixin",
     "ResourceMixin",
 ]
```

## olive/model/handler/mixin/dummy_inputs.py

```diff
@@ -12,56 +12,55 @@
 
 class DummyInputsMixin:
     """Provide the dummy inputs functionality for the model handler.
 
     the dummy data is used to evaluate the latency if user doesn't provide the data for evaluation.
     """
 
-    def get_dummy_inputs(self):
+    def _get_dummy_dataloader_from_io_config(self):
+        dataloader = None
+        # resolved self.io_config
+        # won't use self.io_config since we don't want hf_config to be used
+        resolved_io_config = self.get_user_io_config(self.io_config) or {}
+        if resolved_io_config.get("input_shapes"):
+            logger.debug("Using io_config.input_shapes to build dummy dataloader")
+            dataloader = (
+                # input_types is optional
+                data_config_template.dummy_data_config_template(
+                    input_shapes=resolved_io_config["input_shapes"],
+                    input_types=resolved_io_config.get("input_types"),
+                    input_names=resolved_io_config.get("input_names"),
+                ).to_data_container()
+            )
+        return dataloader
+
+    def get_dummy_inputs(self, filter_hook=None, filter_hook_kwargs=None):
         """Return a dummy input for the model."""
         if self.dummy_inputs is not None:
             return self.dummy_inputs
 
         # Priority: dummy_inputs_func > io_config.input_shapes > hf_config.dataset > onnx_config
         dummy_inputs = None
-        # resolved self.io_config
-        # won't use self.get_io_config() since we don't want hf_config to be used
-        resolved_io_config = self.get_user_io_config(self.io_config) or {}
+
         if self.dummy_inputs_func is not None:
             logger.debug("Using dummy_inputs_func to get dummy inputs")
             user_module_loader = UserModuleLoader(self.model_script, self.script_dir)
             dummy_inputs = user_module_loader.call_object(self.dummy_inputs_func, self)
-        elif resolved_io_config.get("input_shapes"):
-            logger.debug("Using io_config.input_shapes to get dummy inputs")
-            dummy_inputs, _ = (
-                # input_types is optional
-                data_config_template.dummy_data_config_template(
-                    input_shapes=resolved_io_config["input_shapes"],
-                    input_types=resolved_io_config.get("input_types"),
-                )
-                .to_data_container()
-                .get_first_batch(data_root_path=None)
-            )
-        elif self.hf_config and self.hf_config.model_name and self.hf_config.task:
-            # need both model_name and task to get dummy inputs
-            if self.hf_config.dataset:
-                logger.debug("Using hf_config.dataset to get dummy inputs")
-                dummy_inputs, _ = (
-                    data_config_template.huggingface_data_config_template(
-                        self.hf_config.model_name,
-                        self.hf_config.task,
-                        **self.hf_config.dataset,
-                    )
-                    .to_data_container()
-                    .get_first_batch(data_root_path=None)
-                )
-            elif not self.hf_config.components:
-                logger.debug("Using hf onnx_config to get dummy inputs")
+            # respect user's dummy_inputs_func, no hook
+        else:
+            dataloader = self._get_dummy_dataloader_from_io_config()
+            if dataloader:
+                dummy_inputs, _ = dataloader.get_first_batch()
+            elif self.hf_config and not self.hf_config.components and self.hf_config.task:
+                logger.debug("Trying hf onnx_config to get dummy inputs")
                 dummy_inputs = self.get_hf_dummy_inputs()
+                if dummy_inputs is not None:
+                    logger.debug("Got dummy inputs from hf onnx_config")
+            if filter_hook:
+                dummy_inputs = filter_hook(dummy_inputs, **(filter_hook_kwargs or {}))
 
         if dummy_inputs is None:
             raise ValueError(
                 "Unable to get dummy inputs. Please provide dummy_inputs_func, io_config.input_shapes,"
                 " hf_config.dataset, or hf_config."
             )
-
         return dummy_inputs
```

## olive/model/handler/mixin/hf_config.py

```diff
@@ -1,21 +1,27 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 import logging
-from typing import TYPE_CHECKING, Generator, Optional, Tuple
+from pathlib import Path
+from typing import TYPE_CHECKING, Generator, List, Optional, Tuple
 
 from olive.constants import ModelFileFormat
 from olive.model.utils.hf_utils import (
     get_hf_model_config,
     get_hf_model_dummy_input,
+    get_hf_model_generation_config,
     get_hf_model_io_config,
+    get_hf_model_tokenizer,
     load_hf_model_from_model_class,
     load_hf_model_from_task,
+    save_hf_model_config,
+    save_hf_model_generation_config,
+    save_hf_model_tokenizer,
 )
 
 if TYPE_CHECKING:
     from olive.model.handler.pytorch import PyTorchModelHandler
 
 logger = logging.getLogger(__name__)
 
@@ -38,21 +44,60 @@
         * hf_config
     """
 
     def get_hf_model_config(self):
         if self.hf_config is None:
             raise ValueError("HF model_config is not available")
 
-        return get_hf_model_config(self._get_model_path_or_name(), **self.hf_config.get_loading_args_from_pretrained())
+        return get_hf_model_config(self.get_model_path_or_name(), **self.hf_config.get_loading_args_from_pretrained())
+
+    def _get_hf_model_generation_config(self):
+        if self.hf_config is None:
+            raise ValueError("HF model_config is not available")
+
+        return get_hf_model_generation_config(
+            self.get_model_path_or_name(), **self.hf_config.get_loading_args_from_pretrained()
+        )
+
+    def _get_hf_model_tokenizer(self, **kwargs):
+        if self.hf_config is None:
+            raise ValueError("HF model_config is not available")
+
+        # don't provide loading args for tokenizer directly since it tries to serialize all kwargs
+        # TODO(anyone): only provide relevant kwargs, no use case for now to provide kwargs
+        return get_hf_model_tokenizer(self.get_model_path_or_name(), **kwargs)
+
+    def save_metadata_for_token_generation(self, output_dir: str, **kwargs) -> List[str]:
+        """Save metadata for token generation.
+
+        :param output_dir: output directory to save metadata files
+        :param kwargs: additional keyword arguments to pass to `save_pretrained` method
+        :return: list of file paths
+        """
+        if self.hf_config is None:
+            raise ValueError("HF model_config is not available.")
+        if not Path(output_dir).is_dir():
+            raise ValueError("Expecting a directory as input.")
+
+        save_hf_model_config(self.get_hf_model_config(), output_dir, **kwargs)
+        save_hf_model_generation_config(self._get_hf_model_generation_config(), output_dir, **kwargs)
+        tokenizer_filepaths = save_hf_model_tokenizer(self._get_hf_model_tokenizer(), output_dir, **kwargs)
+
+        output_dir = Path(output_dir)
+        return [
+            str(output_dir / "config.json"),
+            str(output_dir / "generation_config.json"),
+            *[fp for fp in tokenizer_filepaths if Path(fp).exists()],
+        ]
 
     def get_hf_io_config(self):
         """Get Io config for the model."""
         if self.hf_config and self.hf_config.task and not self.hf_config.components:
             return get_hf_model_io_config(
-                self._get_model_path_or_name(),
+                self.get_model_path_or_name(),
                 self.hf_config.task,
                 self.hf_config.feature,
                 **self.hf_config.get_loading_args_from_pretrained(),
             )
         else:
             return None
 
@@ -74,15 +119,15 @@
             raise ValueError("Either task or model_class must be specified")
 
         return model
 
     def get_hf_dummy_inputs(self):
         """Get dummy inputs for the model."""
         return get_hf_model_dummy_input(
-            self._get_model_path_or_name(),
+            self.get_model_path_or_name(),
             self.hf_config.task,
             self.hf_config.feature,
             **self.hf_config.get_loading_args_from_pretrained(),
         )
 
     def is_model_loaded_from_hf_config(self) -> bool:
         """Return True if the model is loaded from hf_config, False otherwise."""
@@ -92,12 +137,12 @@
                 self.model_file_format
                 not in (ModelFileFormat.PYTORCH_TORCH_SCRIPT, ModelFileFormat.PYTORCH_MLFLOW_MODEL)
             )
             and self.hf_config
             and (self.hf_config.model_class or self.hf_config.task)
         )
 
-    def _get_model_path_or_name(self):
+    def get_model_path_or_name(self):
         if self.model_file_format == ModelFileFormat.PYTORCH_MLFLOW_MODEL:
-            return self.hf_config.model_name
+            return self.get_mlflow_model_path_or_name(self.get_mlflow_transformers_dir())
         else:
             return self.model_path or self.hf_config.model_name
```

## olive/model/handler/mixin/io_config.py

```diff
@@ -2,15 +2,16 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 from typing import Any, Dict
 
 
 class IoConfigMixin:
-    """Provide the following model get io config functionalites.
+    """Provide the following model get io config functionalities.
 
     Each model handler could choose to override the behavior.
     For example, both PyTorch model and ONNX model handler choose to override the default behavior.
     """
 
-    def get_io_config(self) -> Dict[str, Any]:
-        return self.io_config
+    @property
+    def io_config(self) -> Dict[str, Any]:
+        return self._io_config
```

## olive/model/utils/__init__.py

```diff
@@ -1,15 +1,21 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
-from olive.model.utils.hf_mappings import HIDDEN_SIZE_NAMES, MODEL_TYPE_MAPPING, NUM_HEADS_NAMES
+from olive.model.utils.hf_mappings import (
+    HIDDEN_SIZE_NAMES,
+    MODEL_TYPE_MAPPING,
+    NUM_HEADS_NAMES,
+    NUM_KEY_VALUE_HEADS_NAMES,
+)
 from olive.model.utils.onnx_utils import resolve_onnx_path
 from olive.model.utils.path_utils import normalize_path_suffix
 
 __all__ = [
     "HIDDEN_SIZE_NAMES",
     "MODEL_TYPE_MAPPING",
     "NUM_HEADS_NAMES",
+    "NUM_KEY_VALUE_HEADS_NAMES",
     "normalize_path_suffix",
     "resolve_onnx_path",
 ]
```

## olive/model/utils/hf_mappings.py

```diff
@@ -69,14 +69,16 @@
 }
 
 
 # To extend following list/map from huggingface config
 # there is the priority order: NUM_HEADS_NAMES[0] and HIDDEN_SIZE_NAMES[0] are the first choice
 # which means user can override the value in config file
 NUM_HEADS_NAMES = ("num_heads", "num_attention_heads", "n_head", "n_heads", "encoder_attention_heads")
+NUM_HIDDEN_LAYER_NAMES = ("num_hidden_layers", "num_layers", "n_layer", "n_layers")
+NUM_KEY_VALUE_HEADS_NAMES = ("num_key_value_heads",)
 HIDDEN_SIZE_NAMES = ("hidden_size", "dim", "d_model", "n_embd")
 MODEL_TYPE_MAPPING = {
     "whisper": "bart",
     "camembert": "bert",
     "deberta": "bert",
     "deberta-v2": "bert",
     "distilbert": "bert",
```

## olive/model/utils/hf_utils.py

```diff
@@ -1,75 +1,119 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 import logging
 from functools import partial
 from itertools import chain
-from typing import Callable, Dict, Optional
+from typing import TYPE_CHECKING, Callable, Dict, Optional, Tuple, Union
 
 import transformers
-from transformers import AutoConfig, AutoModel, AutoTokenizer
+from transformers import AutoConfig, AutoModel, AutoTokenizer, GenerationConfig
 
+from olive.common.utils import get_attr
 from olive.model.utils.hf_mappings import FEATURE_TO_PEFT_TASK_TYPE, MODELS_TO_MAX_LENGTH_MAPPING, TASK_TO_FEATURE
 
+if TYPE_CHECKING:
+    from transformers import PretrainedConfig, PreTrainedModel, PreTrainedTokenizer, PreTrainedTokenizerFast
+    from transformers.onnx import OnnxConfig
+
 logger = logging.getLogger(__name__)
 
 
-def load_hf_model_from_task(task: str, name: str, **kwargs):
+def load_hf_model_from_task(task: str, name: str, **kwargs) -> "PreTrainedModel":
     """Load huggingface model from task and name."""
     from transformers.pipelines import check_task
 
     task_results = check_task(task)
     assert isinstance(task_results, tuple)
     if len(task_results) == 2:
         targeted_task = task_results[0]
     elif len(task_results) == 3:
         targeted_task = task_results[1]
     else:
         raise ValueError("unsupported transformers version")
 
-    model_class = {"pt": targeted_task["pt"]}
-    class_tuple = ()
-    class_tuple = class_tuple + model_class.get("pt", (AutoModel,))
-
+    class_tuple = targeted_task["pt"] or (AutoModel,)
     model = None
-    for model_class in class_tuple:
+    for i, model_class in enumerate(class_tuple):
         try:
             model = model_class.from_pretrained(name, **kwargs)
             logger.debug("Loaded model %s with name_or_path %s", model_class, name)
-            return model
-        except (OSError, ValueError):
+            break
+        except (OSError, ValueError) as e:
+            if i == len(class_tuple) - 1:
+                # len(class_tuple) == 1 covers most common tasks like text-generation, text-classification, etc
+                # error could be device OOM, device_map: "auto" not supported, etc
+
+                # len(class_tuple) > 1: not common - image-segmentation, conversational, etc
+                # there is no easy way to get tracebacks for earlier failures, so just raise from last
+                raise
             # the ValueError need to be caught since there will be multiple model_class for single task.
             # if the model_class is not the one for the task, it will raise ValueError and
             # next model_class will be tried.
-            continue
+            logger.info(
+                "Failed to load model %s with name_or_path %s.\n kwargs: %s.\n Exception raised: %s",
+                model_class,
+                name,
+                kwargs,
+                e,
+            )
 
+    # this won't be None since class_tuple is never empty and we only reach here if model loaded successfully
+    # satisfies linter too
     return model
 
 
-def huggingface_model_loader(model_loader):
+def huggingface_model_loader(model_loader: Union[str, Callable]) -> Callable:
     if model_loader is None:
         model_loader = "AutoModel"
     if isinstance(model_loader, str):
         try:
             model_loader = getattr(transformers, model_loader)
         except AttributeError:
             raise AttributeError(f"{model_loader} is not found in transformers") from None
     elif not isinstance(model_loader, Callable):
         raise ValueError("model_loader must be a callable or a string defined in transformers")
 
     return model_loader.from_pretrained
 
 
-def get_hf_model_config(model_name: str, **kwargs):
+def get_hf_model_config(model_name: str, **kwargs) -> "PretrainedConfig":
     """Get HF Config for the given model name."""
     return AutoConfig.from_pretrained(model_name, **kwargs)
 
 
+def save_hf_model_config(config: "PretrainedConfig", output_dir: str, **kwargs):
+    """Save input HF Config to output directory."""
+    config.save_pretrained(output_dir, **kwargs)
+
+
+def get_hf_model_generation_config(model_name: str, **kwargs) -> GenerationConfig:
+    """Get HF model's generation config for the given model name."""
+    return GenerationConfig.from_pretrained(model_name, **kwargs)
+
+
+def save_hf_model_generation_config(config: GenerationConfig, output_dir: str, **kwargs):
+    """Save input HF generation Config to output directory."""
+    config.save_pretrained(output_dir, **kwargs)
+
+
+def get_hf_model_tokenizer(model_name: str, **kwargs) -> Union["PreTrainedTokenizer", "PreTrainedTokenizerFast"]:
+    """Get HF model's tokenizer."""
+    return AutoTokenizer.from_pretrained(model_name, **kwargs)
+
+
+def save_hf_model_tokenizer(
+    tokenizer: Union["PreTrainedTokenizer", "PreTrainedTokenizerFast"], output_dir: str, **kwargs
+) -> Tuple[str]:
+    """Save input tokenizer to output directory."""
+    return tokenizer.save_pretrained(output_dir, **kwargs)
+
+
 def load_hf_model_from_model_class(model_class: str, name: str, **kwargs):
     """Load huggingface model from model_loader and name."""
     return huggingface_model_loader(model_class)(name, **kwargs)
 
 
 # patched version of transformers.onnx.features.supported_features_mapping
 # to support additional models in olive
@@ -83,39 +127,39 @@
     Returns:
         The dictionary mapping a feature to an OnnxConfig constructor.
 
     """
     if onnx_config_cls is None:
         raise ValueError("A OnnxConfig class must be provided")
 
-    import olive.model.utils.hf_onnx_config as config_cls
+    from olive.model.utils import hf_onnx_config
 
-    for attr_name in onnx_config_cls.split("."):
-        config_cls = getattr(config_cls, attr_name)
+    config_cls = get_attr(hf_onnx_config, onnx_config_cls)
     mapping = {}
     for feature in supported_features:
         if "-with-past" in feature:
             task = feature.replace("-with-past", "")
             mapping[feature] = partial(config_cls.with_past, task=task)
         else:
             mapping[feature] = partial(config_cls.from_model_config, task=feature)
 
     return mapping
 
 
-def get_onnx_config(model_name: str, task: str, feature: Optional[str] = None, **kwargs):
+def get_onnx_config(model_name: str, task: str, feature: Optional[str] = None, **kwargs) -> "OnnxConfig":
     # pylint: disable=protected-access
     from transformers.onnx import FeaturesManager
 
     from olive.model.utils.hf_onnx_config import ADDITIONAL_MODEL_TYPES
 
     # patch FeaturesManager._SUPPORTED_MODEL_TYPE to support additional models in olive
     for model_type, feature_list in ADDITIONAL_MODEL_TYPES.items():
         if model_type in FeaturesManager._SUPPORTED_MODEL_TYPE:
             continue
+        # TODO(trajep): remove the need for unpacking feature_list
         features, onnx_config_cls = feature_list
         FeaturesManager._SUPPORTED_MODEL_TYPE[model_type] = patched_supported_features_mapping(
             *features, onnx_config_cls=onnx_config_cls
         )
 
     # if feature is not provided, try to get it from task
     # else use "default"
@@ -123,41 +167,55 @@
 
     # don't want to load the model here since all we need is the config
     # model loading is expensive computationally and memory-wise for large models
     config = get_hf_model_config(model_name, **kwargs)
     # recreate the logic for FeaturesManager.check_supported_model_or_raise to get the model_onnx_config
     # https://github.com/huggingface/transformers/blob/main/src/transformers/onnx/features.py#L712
     model_type = config.model_type.replace("_", "-")
-    model_features = FeaturesManager.get_supported_features_for_model_type(model_type, model_name=model_name)
-    if feature not in model_features:
-        raise ValueError(
-            f"{config.model_type} doesn't support feature {feature}. Supported values are: {model_features}"
-        )
-    return FeaturesManager.get_config(model_type, feature)(config)
+    onnx_config = None
+    try:
+        model_features = FeaturesManager.get_supported_features_for_model_type(model_type, model_name=model_name)
+        if feature in model_features:
+            onnx_config = FeaturesManager.get_config(model_type, feature)(config)
+        else:
+            logger.debug(
+                "%s doesn't support feature %s. Supported features are: %s", model_type, feature, model_features
+            )
+    except KeyError:
+        logger.debug("Model type %s is not supported", model_type)
+
+    return onnx_config
 
 
 def get_hf_model_io_config(model_name: str, task: str, feature: Optional[str] = None, **kwargs):
+    # just log a debug message if io_config is not found
+    # this is not a critical error and the caller may not need the io_config
     model_config = get_onnx_config(model_name, task, feature, **kwargs)
+    if not model_config:
+        return None
+
     inputs = model_config.inputs
     outputs = model_config.outputs
     if not inputs or not outputs:
         # just log a warning and return None, since this is not a critical error
         # and following pass may not use the io_config, like OptimumConversion
-        logger.warning("No inputs or outputs found from model %s", model_config)
+        logger.debug("No inputs or outputs found from hf onnx_config %s. Won't use it to get io config", model_config)
         return None
 
     io_config = {}
     io_config["input_names"] = list(inputs.keys())
     io_config["output_names"] = list(outputs.keys())
     io_config["dynamic_axes"] = dict(chain(inputs.items(), outputs.items()))
     return io_config
 
 
 def get_hf_model_dummy_input(model_name: str, task: str, feature: Optional[str] = None, **kwargs):
     model_config = get_onnx_config(model_name, task, feature, **kwargs)
+    if not model_config:
+        return None
     tokenizer = AutoTokenizer.from_pretrained(model_name, **kwargs)
     return model_config.generate_dummy_inputs(tokenizer, framework="pt")
 
 
 def get_peft_task_type_from_task(task: str, fail_on_not_found=False) -> str:
     """Get peft task type from feature."""
     feature = TASK_TO_FEATURE.get(task, None)
```

## olive/passes/__init__.py

```diff
@@ -8,8 +8,9 @@
 REGISTRY = Pass.registry
 
 __all__ = [
     "Pass",
     "PassParamDefault",
     "PassModuleConfig",
     "FullPassConfig",
+    "REGISTRY",
 ]
```

## olive/passes/olive_pass.py

```diff
@@ -1,22 +1,23 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 import inspect
 import logging
+import shutil
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Any, Callable, ClassVar, Dict, Optional, Tuple, Type, Union, get_args
 
 from olive.common.config_utils import ConfigBase, ParamCategory, validate_config
 from olive.common.user_module_loader import UserModuleLoader
 from olive.data.config import DataConfig
 from olive.hardware import DEFAULT_CPU_ACCELERATOR, AcceleratorSpec
-from olive.model import CompositeModelHandler, DistributedOnnxModelHandler, OliveModelHandler
+from olive.model import CompositeModelHandler, DistributedOnnxModelHandler, OliveModelHandler, ONNXModelHandler
 from olive.passes.pass_config import (
     PassConfigBase,
     PassConfigParam,
     PassParamDefault,
     create_config_class,
     get_user_script_config,
 )
@@ -187,42 +188,103 @@
         # Optimization pass still works on individual graphs.
         if isinstance(model, DistributedOnnxModelHandler):
             for rank in range(model.num_ranks):
                 input_ranked_model = model.load_model(rank)
                 ranked_output_path = Path(output_model_path).with_suffix("") / model.ranked_model_name(rank)
                 self._run_for_config(input_ranked_model, data_root, config, str(ranked_output_path))
 
+            # ranked model don't have their own model_attributes, they are just part of the distributed model
+            # which has the model_attributes
             output_model = DistributedOnnxModelHandler(
                 model_path=str(Path(output_model_path).with_suffix("")),
                 model_name_pattern=model.model_name_pattern,
                 num_ranks=model.num_ranks,
                 inference_settings=model.inference_settings,
+                model_attributes=model.model_attributes,
             )
+            Pass._carry_forward_additional_files(model, output_model)
         elif isinstance(model, CompositeModelHandler) and not self._accepts_composite_model:
             # CompositePyTorchModel is also handled here.
             components = []
             component_names = []
             for component_name, component_model in model.get_model_components():
                 component_output_path = Path(output_model_path).with_suffix("") / component_name
                 output_model_component = self._run_for_config(
                     component_model, data_root, config, str(component_output_path)
                 )
                 output_model_component.model_attributes = (
                     output_model_component.model_attributes or component_model.model_attributes
                 )
                 components.append(output_model_component)
                 component_names.append(component_name)
+                Pass._carry_forward_additional_files(component_model, output_model_component)
             output_model = CompositeModelHandler(components, component_names)
+            output_model.model_attributes = output_model.model_attributes or model.model_attributes
         else:
             output_model = self._run_for_config(model, data_root, config, output_model_path)
-        # assumption: the model attributes from passes, if any, are more important than
-        # the input model attributes, we should not update/extend anymore outside of the pass run
-        output_model.model_attributes = output_model.model_attributes or model.model_attributes
+            # assumption: the model attributes from passes, if any, are more important than
+            # the input model attributes, we should not update/extend anymore outside of the pass run
+            output_model.model_attributes = output_model.model_attributes or model.model_attributes
+            Pass._carry_forward_additional_files(model, output_model)
+
         return output_model
 
+    @staticmethod
+    def _carry_forward_additional_files(input_model: OliveModelHandler, output_model: OliveModelHandler):
+        # NOTE: Can't use model.model_path because that always gets resolved to a filepath.
+        # We need the directory path here.
+        input_model_path = input_model.get_resource("model_path")
+        if not input_model_path:
+            return
+
+        input_model_path = Path(input_model_path)
+        if not input_model_path.is_dir():
+            return
+
+        input_model_attributes = input_model.model_attributes or {}
+        input_model_additional_files = set(input_model_attributes.get("additional_files", []))
+        if not input_model_additional_files:
+            return
+
+        output_model_path = Path(output_model.get_resource("model_path"))
+        if not output_model_path.is_dir():
+            if isinstance(output_model, ONNXModelHandler):
+                # change the "model_path" resource to the parent directory of the model file
+                output_model.set_resource("model_path", output_model_path.parent)
+                output_model.onnx_file_name = output_model_path.name
+                output_model_path = output_model_path.parent
+            else:
+                logger.warning("Expecting the output model to be in a directory but found a file.")
+                return
+
+        output_model_attributes = output_model.model_attributes or {}
+        # output model might have inherited model_attributes from input model
+        # remove the input model's additional files from the output model's additional files
+        # we will add the files that are not already present in the output model
+        output_model_additional_files = (
+            set(output_model_attributes.get("additional_files", [])) - input_model_additional_files
+        )
+
+        for filepath in input_model_additional_files:
+            input_filepath = Path(filepath)
+
+            # Make sure we don't overwrite an existing file in the output's directory.
+            # The follow up pass could have *potentially* generated a file with the same name.
+            output_filepath = output_model_path / input_filepath.name
+            if not output_filepath.exists():
+                # TODO(team): Use symlinks instead of copying the files.
+                shutil.copy(str(input_filepath), str(output_filepath))
+            # always add the file_path to the output model's additional files
+            # this covers the case where the output model_path is the same as the input model_path
+            # like for perf-tuning pass
+            output_model_additional_files.add(str(output_filepath))
+
+        output_model_attributes["additional_files"] = list(output_model_additional_files)
+        output_model.model_attributes = output_model_attributes
+
     def serialize_config(self, config: Dict[str, Any], check_object: bool = False) -> str:
         """Serialize the configuration."""
         return self._config_class(**config).to_json(check_object)
 
     def to_json(self, check_object: bool = False) -> Dict[str, Any]:
         """Convert the pass to json."""
         return {
@@ -240,14 +302,15 @@
 
     @classmethod
     @abstractmethod
     def _default_config(cls, accelerator_spec: AcceleratorSpec) -> Dict[str, PassConfigParam]:
         """Get the default configuration for the pass. Doesn't include user_script and script_dir.
 
         Example:
+            ```
             return {
                 # required parameter
                 "param1": PassConfigParam(type_=int, required=True, description="param1 description"),
                 # optional parameter with default value
                 "param2": PassConfigParam(type_=int, default_value=1, description="param2 description"),
                 # optional parameter with default value and searchable values
                 "param3": PassConfigParam(
@@ -281,14 +344,15 @@
                             (1, 1): Categorical([1, 2, 3]),
                             (1, 2): Categorical([4, 5, 6]),
                         },
                     ),
                     description="param6 description",
                 ),
             }
+            ```
 
         """
         raise NotImplementedError
 
     @classmethod
     def _resolve_defaults(cls, config: Dict[str, Any], default_config: Dict[str, PassConfigParam]) -> Dict[str, Any]:
         """Resolve default values."""
```

## olive/passes/pass_config.py

```diff
@@ -2,16 +2,17 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 from enum import Enum
 from pathlib import Path
 from typing import Callable, ClassVar, Dict, List, Optional, Type, Union
 
-from olive.common.config_utils import ConfigBase, ConfigParam, ParamCategory, validate_object, validate_resource_path
+from olive.common.config_utils import ConfigBase, ConfigParam, ParamCategory, validate_object
 from olive.common.pydantic_v1 import create_model, validator
+from olive.resource_path import validate_resource_path
 from olive.strategy.search_parameter import SearchParameter, SpecialParamValue, json_to_search_parameter
 
 
 class PassParamDefault(str, Enum):
     """Default values for passes."""
 
     DEFAULT_VALUE = "DEFAULT_VALUE"
@@ -76,23 +77,28 @@
                 " be imported from this script."
             ),
         ),
     }
     return user_script_config  # noqa: RET504
 
 
+DEFAULT_SET = set(PassParamDefault)
+
+
 class PassConfigBase(ConfigBase):
+
     @validator("*", pre=True)
     def _validate_default_str(cls, v, field):
-        try:
-            v = PassParamDefault(v)
-        finally:
-            if field.required and isinstance(v, PassParamDefault):
-                raise ValueError(f"{field.name} is required and cannot be set to {v.value}")
-            return v  # noqa: B012 # pylint: disable=lost-exception, return-in-finally
+        if not isinstance(v, (str, PassParamDefault)) or v not in DEFAULT_SET:
+            return v
+
+        if field.required:
+            raise ValueError(f"{field.name} is required and cannot be set to {v}")
+
+        return PassParamDefault(v)
 
     @validator("*", pre=True)
     def _validate_search_parameter(cls, v):
         if isinstance(v, dict) and v.get("olive_parameter_type") == "SearchParameter":
             return json_to_search_parameter(v)
         return v
```

## olive/passes/onnx/conversion.py

```diff
@@ -11,27 +11,26 @@
 from typing import Any, Dict, Optional, Tuple, Union
 
 import onnx
 import torch
 from packaging import version
 
 from olive.common.config_utils import validate_config
-from olive.common.utils import exclude_keys, find_submodules, resolve_torch_dtype, tensor_data_to_device
+from olive.common.utils import find_submodules, resolve_torch_dtype, tensor_data_to_device
 from olive.hardware import AcceleratorSpec
 from olive.model import (
     CompositeModelHandler,
     DistributedOnnxModelHandler,
     DistributedPyTorchModelHandler,
     HfFromPretrainedArgs,
     ONNXModelHandler,
     PyTorchModelHandler,
 )
 from olive.model.config import IoConfig
 from olive.model.config.hf_config import HfConfig, get_model_type_from_hf_config
-from olive.model.config.io_config import is_kv_cache_required
 from olive.model.utils import resolve_onnx_path
 from olive.passes import Pass
 from olive.passes.onnx.common import get_external_data_config, model_proto_to_olive_model
 from olive.passes.onnx.merge_decoders import merge_decoders
 from olive.passes.pass_config import PassConfigParam
 
 logger = logging.getLogger(__name__)
@@ -68,14 +67,22 @@
         config = {
             "target_opset": PassConfigParam(
                 type_=int, default_value=13, description="The version of the default (ai.onnx) opset to target."
             ),
             "use_dynamo_exporter": PassConfigParam(
                 type_=bool, default_value=False, description="Whether to use dynamo_export API to export ONNX model."
             ),
+            "past_key_value_name": PassConfigParam(
+                type_=str,
+                default_value="past_key_values",
+                description=(
+                    "The arguments name to point to past key values. For model loaded from huggingface, "
+                    "it is 'past_key_values'. Basically, it is used only when `use_dynamo_exporter` is True."
+                ),
+            ),
             "device": PassConfigParam(
                 type_=str,
                 description=(
                     "The device to use for conversion, e.g., 'cuda' or 'cpu'. If not specified, will use 'cpu' for"
                     " PyTorch model and 'cuda' for DistributedPyTorchModel."
                 ),
             ),
@@ -103,21 +110,63 @@
                 description=(
                     "Whether to merge adapter weights before conversion. "
                     "After merging, the model structure is consistent with base model. "
                     "That is useful if you cannot run conversion for some fine-tuned "
                     "models with adapter weights"
                 ),
             ),
+            "save_metadata_for_token_generation": PassConfigParam(
+                type_=bool,
+                default_value=False,
+                description=(
+                    "Whether to save metadata for token generation or not. "
+                    "Includes config.json, generation_config.json, and  tokenizer related files."
+                ),
+            ),
         }
         config.update(get_external_data_config())
         return config
 
     def _run_for_config(
         self, model: PyTorchModelHandler, data_root: str, config: Dict[str, Any], output_model_path: str
     ) -> Union[CompositeModelHandler, DistributedOnnxModelHandler, ONNXModelHandler]:
+        output_model = self._run_for_config_internal(model, data_root, config, output_model_path)
+
+        if model.hf_config and config["save_metadata_for_token_generation"]:
+            if isinstance(output_model, CompositeModelHandler):
+                for _, component_model in output_model.get_model_components():
+                    output_dir = Path(component_model.get_resource("model_path"))
+                    if not output_dir.is_dir():
+                        output_dir = str(output_dir.parent)
+                        component_model.set_resource("model_path", output_dir)
+
+                    component_model.model_attributes = model_attributes = component_model.model_attributes or {}
+                    model_attributes["additional_files"] = additional_files = model_attributes.get(
+                        "additional_files", []
+                    )
+                    additional_files.extend(model.save_metadata_for_token_generation(str(output_dir)))
+
+            elif isinstance(output_model, (DistributedOnnxModelHandler, ONNXModelHandler)):
+                output_dir = Path(output_model.get_resource("model_path"))
+                if not output_dir.is_dir():
+                    output_dir = str(output_dir.parent)
+                    output_model.set_resource("model_path", output_dir)
+
+                output_model.model_attributes = model_attributes = output_model.model_attributes or {}
+                model_attributes["additional_files"] = additional_files = model_attributes.get("additional_files", [])
+                additional_files.extend(model.save_metadata_for_token_generation(str(output_dir)))
+
+            else:
+                raise RuntimeError("Encountered an unknown model type during conversion.")
+
+        return output_model
+
+    def _run_for_config_internal(
+        self, model: PyTorchModelHandler, data_root: str, config: Dict[str, Any], output_model_path: str
+    ) -> Union[CompositeModelHandler, DistributedOnnxModelHandler, ONNXModelHandler]:
         # get the device to use for conversion
         # default to "cpu" for PyTorchModelHandler and "cuda" for DistributedPyTorchModel
         device = config["device"] or "cpu"
         # get the dtype to use for conversion
         torch_dtype = resolve_torch_dtype(config["torch_dtype"]) if config["torch_dtype"] else None
         if torch_dtype == torch.float16 and device == "cpu":
             raise ValueError("Conversion to float16 is not supported for CPU.")
@@ -192,95 +241,60 @@
             pytorch_model = TraceModelWrapper(pytorch_model)
 
         # get input and output names, and dynamic axes
         assert (
             io_config is not None
         ), "Cannot get io_config for the model. Please specify io_config or hf_config for the model"
         io_config = validate_config(io_config, IoConfig)
-        input_names = io_config.input_names
-
-        # some dummy inputs might not be used in the model, so we need to remove them
-        # this can happen when we are using an hf dataset to generate dummy inputs
-        # only handle dict for now since we cannot get the name of the input from a list/tuple
-        if isinstance(dummy_inputs, dict):
-            dummy_input_keys = set(dummy_inputs.keys())
-
-            # after the expansion, user should provide the correct input names for inference
-            for name, dm_input in dummy_inputs.items():
-                # the `past_key_values` is the argument name from huggingface model class
-                # which is independent of the kv-related variables in input list provided by users
-                # if user provided the kv-related variables, we should not remove
-                # the `past_key_values` from dummy inputs. But if not, we should remove it.
-                if (
-                    name == "past_key_values"
-                    and isinstance(dm_input, list)
-                    and is_kv_cache_required(dm_input, io_config)
-                ):
-                    dummy_input_keys.discard(name)
-
-            unused_keys = dummy_input_keys - set(input_names)
-
-            if unused_keys:
-                logger.debug("Removing unused dummy inputs: %s", unused_keys)
 
         onnx_model = None
         if config["use_dynamo_exporter"]:
             torch_version = torch.__version__
             if version.parse(torch_version) < version.parse("2.2.0"):
                 raise ImportError(
                     f"torch.onnx.dynamo_export is not available for torch version {torch_version}. "
                     "Please upgrade your torch version to 2.2.0 or above."
                 )
-            from torch._dynamo import config
+            from torch._dynamo import config as dynamo_config
             from torch.onnx import dynamo_export
 
-            config.capture_scalar_outputs = True
-
-            if isinstance(dummy_inputs, dict):
-                for key in unused_keys:
-                    dummy_inputs[key] = None
+            dynamo_config.capture_scalar_outputs = True
 
-            pytorch_model(*dummy_inputs.values())
+            dummy_inputs = dummy_inputs.values() if isinstance(dummy_inputs, dict) else dummy_inputs
+            pytorch_model(*dummy_inputs)
 
             with tempfile.TemporaryDirectory(dir=tempdir, prefix="olive_tmp") as tmp_dir:
                 tmp_dir_path = Path(tmp_dir)
                 tmp_model_path = resolve_onnx_path(tmp_dir_path)
 
                 dynamo_export(
                     pytorch_model,
-                    *dummy_inputs.values(),
+                    *dummy_inputs,
                     export_options=torch.onnx.ExportOptions(dynamic_shapes=True),
                 ).save(tmp_model_path)
                 onnx.checker.check_model(tmp_model_path)
                 onnx.shape_inference.infer_shapes_path(tmp_model_path)
                 onnx_model = onnx.load(tmp_model_path)
         else:
-            # Standard ONNX export
-            if isinstance(dummy_inputs, dict):
-                dummy_inputs = exclude_keys(dummy_inputs, unused_keys)
-
-            output_names = io_config.output_names
-            dynamic_axes = io_config.dynamic_axes
-
             # there might be multiple files created during export, so we need to track the dir
             # if there are other processes writing to the same dir, we might end up deleting files created by
             # other processes
             with tempfile.TemporaryDirectory(dir=tempdir, prefix="olive_tmp") as tmp_dir:
                 tmp_dir_path = Path(tmp_dir)
                 tmp_model_path = resolve_onnx_path(tmp_dir_path)
 
                 torch.onnx.export(
                     pytorch_model,
                     dummy_inputs,
                     tmp_model_path,
                     export_params=True,
                     opset_version=config["target_opset"],
-                    input_names=input_names,
-                    output_names=output_names,
-                    dynamic_axes=dynamic_axes,
+                    input_names=io_config.input_names,
+                    output_names=io_config.output_names,
+                    dynamic_axes=io_config.dynamic_axes,
                 )
                 onnx_model = onnx.load(tmp_model_path)
                 # the model is loaded into memory, so it's safe to delete previously exported file(s)
 
             # Workaround as described under IoConfig.string_to_int_dim_params: change numeric dim_param to dim_value
             if io_config.string_to_int_dim_params:
                 for tensor in onnx_model.graph.output:
@@ -407,16 +421,24 @@
         pytorch_model, model_attributes = self._load_pytorch_model(model, device, torch_dtype)
         if config["merge_adapter_weights"] and is_peft_model(pytorch_model):
             logger.debug("Merging adapter weights into base model. This is specific to PeftModel.")
             pytorch_model = pytorch_model.merge_and_unload()
         pytorch_model.eval()
 
         # get dummy inputs
-        dummy_inputs = model.get_dummy_inputs()
-        io_config = model.get_io_config()
+
+        dummy_inputs = model.get_dummy_inputs(
+            filter_hook=(
+                model.merge_kv_cache_hook if config["use_dynamo_exporter"] else model.merge_kv_cache_to_tuple_hook
+            ),
+            filter_hook_kwargs={
+                "past_kv_names": config["past_key_value_name"],
+            },
+        )
+        io_config = model.io_config
 
         converted_onnx_model = OnnxConversion._export_pytorch_model(
             pytorch_model, dummy_inputs, io_config, config, device, torch_dtype, tempfile.tempdir
         )
 
         # save the model to the output path and return the model
         output_model_path = resolve_onnx_path(output_model_path)
@@ -460,15 +482,15 @@
 
             input_model = DistributedPyTorchModelHandler(**model_config)
 
             if input_model.hf_config and input_model.hf_config.components:
                 ranked_models = []
                 for _, component_model in input_model.get_hf_components(local_rank):
                     dummy_inputs = component_model.get_dummy_inputs()
-                    io_config = None if pass_config["use_dynamo_exporter"] else component_model.get_io_config()
+                    io_config = None if pass_config["use_dynamo_exporter"] else component_model.io_config
                     pytorch_model = component_model.prepare_session(rank=local_rank)
 
                     ranked_component_modelproto = OnnxConversion._export_pytorch_model(
                         pytorch_model,
                         dummy_inputs,
                         io_config,
                         pass_config,
@@ -482,15 +504,15 @@
                 if len(ranked_models) == 2:
                     ranked_onnx_modelproto = merge_decoders(ranked_models[0], ranked_models[1])
                 else:
                     raise RuntimeError("DistributedOnnxModelHandler can handle exactly 2 components.")
             else:
                 olive_pytorch_model = input_model.load_model(local_rank)
                 dummy_inputs = olive_pytorch_model.get_dummy_inputs()
-                io_config = None if pass_config["use_dynamo_exporter"] else olive_pytorch_model.get_io_config()
+                io_config = None if pass_config["use_dynamo_exporter"] else olive_pytorch_model.io_config
                 pytorch_model = olive_pytorch_model.prepare_session(rank=local_rank)
 
                 ranked_onnx_modelproto = OnnxConversion._export_pytorch_model(
                     pytorch_model,
                     dummy_inputs,
                     io_config,
                     pass_config,
```

## olive/passes/onnx/extract_adapters.py

```diff
@@ -2,24 +2,24 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 import logging
 import re
 from copy import deepcopy
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Dict, List
+from typing import TYPE_CHECKING, Any, Dict, List, Set, Tuple
 
 import numpy as np
 import onnx
 
 from olive.hardware.accelerator import AcceleratorSpec
 from olive.model import ONNXModelHandler
 from olive.model.utils import resolve_onnx_path
 from olive.passes import Pass
-from olive.passes.onnx.common import model_proto_to_olive_model
+from olive.passes.onnx.common import get_external_data_config, model_proto_to_olive_model
 from olive.passes.onnx.onnx_dag import OnnxDAG
 from olive.passes.pass_config import PassConfigParam
 
 if TYPE_CHECKING:
     from numpy.typing import NDArray
 
 logger = logging.getLogger(__name__)
@@ -33,15 +33,15 @@
     SessionOptions.add_external_initializers.
 
     If make_inputs is True, the adapter weights are inputs to the model and must be provided during inference.
     """
 
     @classmethod
     def _default_config(cls, accelerator_spec: AcceleratorSpec) -> Dict[str, PassConfigParam]:
-        return {
+        config = {
             "make_inputs": PassConfigParam(
                 type_=bool,
                 default_value=False,
                 description=(
                     "Convert adapter weights to inputs. If false, the adapter weights will be set as initializers with"
                     " external data."
                 ),
@@ -51,22 +51,24 @@
                 default_value=True,
                 description=(
                     "Pack adapter weights for the same module type into a single input tensor. Only used if make_inputs"
                     " is True."
                 ),
             ),
         }
+        config.update(get_external_data_config())
+        return config
 
     def _run_for_config(
         self, model: ONNXModelHandler, data_root: str, config: Dict[str, Any], output_model_path: str
     ) -> ONNXModelHandler:
         output_model_path = resolve_onnx_path(output_model_path, Path(model.model_path).name)
 
-        if "lora_modules" not in model.model_attributes:
-            raise ValueError("Model does not contain lora_modules attribute")
+        if "lora_modules" not in (model.model_attributes or {}):
+            raise ValueError("Model does not contain lora_modules model_attribute")
 
         # create a dag from the model
         dag = OnnxDAG.from_model_path(model.model_path)
         # remove unnecessary identity nodes
         dag.remove_identity_nodes()
 
         # get lora modules
@@ -79,135 +81,109 @@
         float_modules = set()
         quant_modules = set()
 
         # nodes to remove at the end
         nodes_to_remove = set()
 
         for node_name in dag.get_node_names():
-            if dag.get_node_op_type(node_name) != "MatMul" or not any(
+            op_type = dag.get_node_op_type(node_name)
+            if op_type not in {"MatMul", "MatMulNBits"} or not any(
                 re.match(pattern, node_name) for pattern in lora_name_patterns
             ):
                 # not a lora module
                 continue
 
-            # new name for the weight
+            # new name for the float weight
             new_weight_name = self._create_new_weight_name(node_name)
+            # new names for quantized weight and parameters
+            # zero point is optional if symmetric
+            quantized_suffices = [".quant.weight", ".quant.scale", ".quant.zero_point"]
+            new_quantized_names = [new_weight_name.replace(".weight", suffix) for suffix in quantized_suffices]
+
+            if op_type == "MatMul":
+                # float or QDQ quantized
+                # original weight name
+                old_weight_name = dag.get_node_inputs(node_name)[1]
 
-            # original weight name
-            old_weight_name = dag.get_node_inputs(node_name)[1]
-
-            if dag.is_input(old_weight_name):
-                # nothing we can do here
-                continue
-            elif dag.is_initializer(old_weight_name):
-                # weight is an initializer (not quantized)
-                # create initializer with new weight name
-                self._create_empty_initializer(dag, weights, old_weight_name, new_weight_name)
-
-                # change input to the new name
-                dag.replace_node_input(node_name, old_weight_name, new_weight_name)
-
-                # add the module to the float modules
-                float_modules.add(new_weight_name.replace(".weight", ""))
-            elif dag.get_node_op_type(dag.get_producer(old_weight_name)) == "DequantizeLinear":
-                # weight is quantized
-                # get the dequantize node
-                old_dequantize_name = dag.get_producer(old_weight_name)
-                old_dequantize_node = dag.get_node(old_dequantize_name)
-
-                # new names for the dequantize node inputs
-                suffixes = ["quant.weight", "quant.scale", "quant.zero_point"]
-                new_input_names = [new_weight_name.replace("weight", suffix) for suffix in suffixes]
-
-                # zero point is optional so we keep track of used inputs
-                used_inputs = []
-                # create new initializers for the dequantize node
-                for old_input, new_input in zip(old_dequantize_node.inputs, new_input_names):
+                if dag.is_input(old_weight_name):
+                    # nothing to do here
+                    continue
+                elif dag.is_initializer(old_weight_name):
+                    # weight is an float initializer
+                    # create initializer with new weight name
+                    self._create_empty_initializer(dag, weights, old_weight_name, new_weight_name)
+
+                    # change input to the new name
+                    dag.replace_node_input(node_name, old_weight_name, new_weight_name)
+
+                    # add the module to the float modules
+                    float_modules.add(new_weight_name.replace(".weight", ""))
+                elif dag.get_node_op_type(dag.get_producer(old_weight_name)) == "DequantizeLinear":
+                    # weight is QDQ quantized
+                    # get the dequantize node
+                    old_dequantize_name = dag.get_producer(old_weight_name)
+                    old_dequantize_node = dag.get_node(old_dequantize_name)
+
+                    # zero point is optional so we keep track of used inputs
+                    used_inputs = []
+                    # create new initializers for the dequantize node
+                    for old_input, new_input in zip(old_dequantize_node.inputs, new_quantized_names):
+                        self._create_empty_initializer(dag, weights, old_input, new_input)
+                        used_inputs.append(new_input)
+
+                    # create a new dequantize node
+                    # NOTE: We could directly modify the original dequantize node but this assumes that the dequantize
+                    # node is not used elsewhere
+                    # this cannot be guaranteed (for instance, if the float model has lora modules with same weights,
+                    # they might all share the same dequantize node)
+                    new_dequantize_proto = onnx.NodeProto()
+                    new_dequantize_proto.CopyFrom(old_dequantize_node.proto)
+                    # change node name
+                    new_dequantize_proto.name = new_weight_name.replace("weight", "dequantize")
+                    # change input names
+                    for i, new_input in enumerate(used_inputs):
+                        new_dequantize_proto.input[i] = new_input
+                    # change output name
+                    new_dequantize_proto.output[0] = new_weight_name
+
+                    # add new dequantize node
+                    dag.add_node(new_dequantize_proto, old_dequantize_node.graph_idx)
+
+                    # replace input to the new name
+                    dag.replace_node_input(node_name, old_weight_name, new_weight_name)
+
+                    # add old dequantize node to remove
+                    nodes_to_remove.add(old_dequantize_name)
+
+                    # add the module to the quant modules
+                    quant_modules.add(new_weight_name.replace(".weight", ".quant"))
+            elif op_type == "MatMulNBits":
+                # weight is Nbits quantized
+                # create empty initializers and change node inputs
+                for old_input, new_input in zip(dag.get_node_inputs(node_name)[1:], new_quantized_names):
                     self._create_empty_initializer(dag, weights, old_input, new_input)
-                    used_inputs.append(new_input)
-
-                # create a new dequantize node
-                # NOTE: We could directly modify the original dequantize node but this assumes that the dequantize node
-                # is not used elsewhere
-                # this cannot be guaranteed (for instance, if the float model has lora modules with same weights, they
-                # might all share the same dequantize node)
-                new_dequantize_proto = onnx.NodeProto()
-                new_dequantize_proto.CopyFrom(old_dequantize_node.proto)
-                # change node name
-                new_dequantize_proto.name = new_weight_name.replace("weight", "dequantize")
-                # change input names
-                for i, new_input in enumerate(used_inputs):
-                    new_dequantize_proto.input[i] = new_input
-                # change output name
-                new_dequantize_proto.output[0] = new_weight_name
-
-                # add new dequantize node
-                dag.add_node(new_dequantize_proto, old_dequantize_node.graph_idx)
-
-                # replace input to the new name
-                dag.replace_node_input(node_name, old_weight_name, new_weight_name)
-
-                # add old dequantize node to remove
-                nodes_to_remove.add(old_dequantize_name)
+                    dag.replace_node_input(node_name, old_input, new_input)
 
                 # add the module to the quant modules
                 quant_modules.add(new_weight_name.replace(".weight", ".quant"))
-            # TODO(jambayk): Add int4 quantization support
 
         # remove old dequantize nodes
         for node_name in nodes_to_remove:
             dag.remove_node(node_name, check_no_consumers=True)
 
         if config["make_inputs"] and not config["pack_inputs"]:
             # create inputs for the weights
             for weight_name in weights:
                 dag.convert_initializer_to_input(weight_name)
         elif config["make_inputs"] and config["pack_inputs"]:
             # what weights are packed together
-            packings = {}
-
-            def get_sort_key(module_name: str):
-                parts = module_name.split(".")
-                for i, part in enumerate(parts):
-                    try:
-                        # want the layers to be sorted by the number
-                        parts[i] = int(part)
-                    except ValueError:
-                        pass
-                return parts
-
-            # group by module type, sort by name and pack them together
-            for module_type in lora_modules:
-                for lora_i in ["lora_A", "lora_B"]:
-                    # base name to use for split node and input
-                    base_name = f"{module_type}.{lora_i}"
-
-                    matching_float_modules = sorted(
-                        [name for name in float_modules if module_type in name and lora_i in name], key=get_sort_key
-                    )
-                    if matching_float_modules:
-                        packings[f"{base_name}.weight.packed"] = [f"{name}.weight" for name in matching_float_modules]
-
-                    matching_quant_modules = sorted(
-                        [name for name in quant_modules if module_type in name and lora_i in name], key=get_sort_key
-                    )
-                    if matching_quant_modules:
-                        # zero point is optional so we need to check if it exists
-                        for suffix in [".weight", ".scale", ".zero_point"]:
-                            packings[f"{base_name}.quant{suffix}.packed"] = [
-                                name + suffix for name in matching_quant_modules if name + suffix in weights
-                            ]
+            packed_weights, packings = self.pack_weights(weights, lora_modules, float_modules, quant_modules)
 
-            # pack the weights, create inputs and split nodes
-            packed_weights = {}
+            # create inputs and split nodes for the packed weights
             for weight_name, to_pack in packings.items():
-                if not to_pack:
-                    continue
-                packed_weights[weight_name] = np.concatenate([np.atleast_1d(weights[name]) for name in to_pack], axis=0)
-
                 # input proto
                 input_proto = onnx.helper.make_tensor_value_info(
                     name=weight_name,
                     elem_type=onnx.helper.np_dtype_to_tensor_dtype(packed_weights[weight_name].dtype),
                     shape=packed_weights[weight_name].shape,
                 )
                 # TODO(jambayk): check if graph_idx can be 0 even if they might be used in subgraphs
@@ -235,46 +211,102 @@
         weights_path = Path(output_model_path).parent / "adapter_weights.npz"
         np.savez(weights_path, **weights)
 
         # save the model
         output_model = model_proto_to_olive_model(
             dag.model,
             output_model_path,
-            external_data_config={"save_as_external_data": True, "all_tensors_to_one_file": True},
+            config,
             external_initializers_file_name=weights_path.name if not config["make_inputs"] else None,
             constant_inputs_file_name=weights_path.name if config["make_inputs"] else None,
         )
         output_model.model_attributes = deepcopy(model.model_attributes)
+        # add adapter weights to the model attributes
+        output_model.model_attributes["additional_files"] = additional_files = output_model.model_attributes.get(
+            "additional_files", []
+        )
+        additional_files.append(str(weights_path))
         # save information about the weights in the model attributes
         weights_info = {name: [list(value.shape), str(value.dtype)] for name, value in weights.items()}
         if not config["make_inputs"]:
             output_model.model_attributes["external_initializers"] = weights_info
         else:
             output_model.model_attributes["constant_inputs"] = weights_info
             if config["pack_inputs"]:
                 output_model.model_attributes["packed_inputs"] = packings
         return output_model
 
     @staticmethod
+    def pack_weights(
+        weights: Dict[str, "NDArray"], module_types: List[str], float_modules: Set[str], quant_modules: Set[str]
+    ) -> Tuple[Dict[str, "NDArray"], Dict[str, List[str]]]:
+        """Pack the weights for a given module type into an array each for lora_A and lora_B.
+
+        Assumes the weights for the same module type are in the same format (float, QDQ, Nbits).
+        :param weights: dictionary of weights
+        :param module_types: list of module types
+        :param float_modules: set of float module names
+        :param quant_modules: set of quantized module names
+        :return: dictionary of packed weights and dictionary of packed weights and their corresponding weights
+        """
+
+        def get_sort_key(module_name: str):
+            # want the layers to be sorted by the number
+            return [int(part) if part.isdigit() else part for part in module_name.split(".")]
+
+        packings = {}
+        for module_type in module_types:
+            for lora_i in ["lora_A", "lora_B"]:
+                matching_float_modules = sorted(
+                    [name for name in float_modules if module_type in name and lora_i in name], key=get_sort_key
+                )
+                if matching_float_modules:
+                    weight_name = f"{module_type}.{lora_i}.weight.packed"
+                    packings[weight_name] = [f"{name}.weight" for name in matching_float_modules]
+
+                matching_quant_modules = sorted(
+                    [name for name in quant_modules if module_type in name and lora_i in name], key=get_sort_key
+                )
+                if matching_quant_modules:
+                    # zero point is optional so we need to check if it exists
+                    for suffix in [".weight", ".scale", ".zero_point"]:
+                        weight_name = f"{module_type}.{lora_i}.quant{suffix}.packed"
+                        to_pack = [name + suffix for name in matching_quant_modules if name + suffix in weights]
+                        if to_pack:
+                            packings[weight_name] = to_pack
+
+        packed_weights = {}
+        for weight_name, to_pack in packings.items():
+            packed_weights[weight_name] = np.concatenate([np.atleast_1d(weights[name]) for name in to_pack], axis=0)
+
+        return packed_weights, packings
+
+    @staticmethod
     def _get_lora_name_patterns(lora_modules: List[str]) -> List[str]:
         """Get the node name patterns for lora modules."""
-        return [f".*[./]{key}[./]{name}[./]MatMul$" for key in lora_modules for name in ["default", "default_1"]]
+        return [
+            f".*[./]{key}[./]{name}[./]{matmul}$"
+            for key in lora_modules
+            for name in ["default", "default_1"]
+            for matmul in ["MatMul", "MatMul_Q4"]
+        ]
 
     @staticmethod
     def _create_new_weight_name(old_name: str) -> str:
         """Create new weight name based on old name.
 
         The new weight name is of the form model.layers.0.self_attn.q_proj.lora_A.quant.weight
         """
         weight_name = old_name[1:] if old_name.startswith("/") else old_name
+        matmul_name = weight_name.split("/")[-1]
         return (
             weight_name.replace("/", ".")
             .replace("default.", "lora_A.")
             .replace("default_1.", "lora_B.")
-            .replace("MatMul", "weight")
+            .replace(matmul_name, "weight")
         )
 
     @staticmethod
     def _copy_initializer(old_initializer: onnx.TensorProto, new_name: str) -> onnx.TensorProto:
         """Copy initializer with a new name and dummy external data location."""
         from onnx.external_data_helper import set_external_data
```

## olive/passes/onnx/float16_conversion.py

```diff
@@ -1,71 +1,74 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 from pathlib import Path
 from typing import Any, Dict, List
 
-import onnx
-
 from olive.hardware.accelerator import AcceleratorSpec
 from olive.model import ONNXModelHandler
 from olive.model.utils import resolve_onnx_path
 from olive.passes import Pass
 from olive.passes.onnx.common import get_external_data_config, model_proto_to_olive_model
 from olive.passes.pass_config import PassConfigParam
 
 
 class OnnxFloatToFloat16(Pass):
     """Converts a model to float16.
 
-    It is based on onnxconverter-common.convert_float_to_float16.
-    See https://onnxruntime.ai/docs/performance/model-optimizations/float16.html#float16-conversion
+    It uses the float16 converter from onnxruntime to convert the model to float16.
     """
 
     @classmethod
     def _default_config(cls, accelerator_spec: AcceleratorSpec) -> Dict[str, PassConfigParam]:
         config = {
             "min_positive_val": PassConfigParam(
                 type_=float, default_value=1e-7, description="Constant values will be clipped against this value"
             ),
             "max_finite_val": PassConfigParam(
                 type_=float, default_value=1e4, description="Constant values will be clipped against this value"
             ),
             "keep_io_types": PassConfigParam(
                 type_=bool, default_value=False, description="Whether model inputs/outputs should be left as float32"
             ),
-            "disable_shape_infer": PassConfigParam(
-                type_=bool, default_value=False, description="Skips running onnx shape/type inference."
+            "use_symbolic_shape_infer": PassConfigParam(
+                type_=bool,
+                default_value=True,
+                description="Use symbolic shape inference instead of onnx shape inference. Defaults to True.",
             ),
             "op_block_list": PassConfigParam(
                 type_=List[str], default_value=None, description="List of op types to leave as float32"
             ),
             "node_block_list": PassConfigParam(
                 type_=List[str], default_value=None, description="List of node names to leave as float32"
             ),
         }
         config.update(get_external_data_config())
         return config
 
     def _run_for_config(
         self, model: ONNXModelHandler, data_root: str, config: Dict[str, Any], output_model_path: str
     ) -> ONNXModelHandler:
-        from onnxconverter_common import float16
+        from onnxruntime.transformers.onnx_model import OnnxModel
 
         output_model_path = resolve_onnx_path(output_model_path, Path(model.model_path).name)
 
-        config = self._config_class(**config)
-
-        model_fp32 = onnx.load(str(model.model_path))
-        model_fp16 = float16.convert_float_to_float16(
-            model_fp32,
-            min_positive_val=config.min_positive_val,
-            max_finite_val=config.max_finite_val,
-            keep_io_types=config.keep_io_types,
-            disable_shape_infer=config.disable_shape_infer,
-            op_block_list=config.op_block_list,
-            node_block_list=config.node_block_list,
+        # using the float16 converter from onnxruntime since it is regularly updated
+        # and can handle large models (>2GB) as well as ort contrib ops
+        ort_onnx_model = OnnxModel(model.load_model())
+        ort_onnx_model.convert_float_to_float16(
+            **{
+                key: config[key]
+                for key in [
+                    "min_positive_val",
+                    "max_finite_val",
+                    "keep_io_types",
+                    "use_symbolic_shape_infer",
+                    "op_block_list",
+                    "node_block_list",
+                ]
+            }
         )
 
         # save the model to the output path and return the model
-        return model_proto_to_olive_model(model_fp16, output_model_path, config.dict())
+        return model_proto_to_olive_model(ort_onnx_model.model, output_model_path, config)
```

## olive/passes/onnx/inc_quantization.py

```diff
@@ -11,15 +11,16 @@
 
 from packaging import version
 
 from olive.cache import get_local_path_from_root
 from olive.common.config_utils import validate_config
 from olive.common.utils import exclude_keys
 from olive.data.config import DataConfig
-from olive.evaluator.metric import Metric, joint_metric_key
+from olive.evaluator.metric import Metric
+from olive.evaluator.metric_result import joint_metric_key
 from olive.evaluator.olive_evaluator import OliveEvaluatorFactory
 from olive.exception import OlivePassError
 from olive.hardware.accelerator import AcceleratorSpec
 from olive.model import ONNXModelHandler
 from olive.model.utils import resolve_onnx_path
 from olive.passes import Pass
 from olive.passes.onnx.common import get_external_data_config, model_proto_to_olive_model
@@ -499,15 +500,16 @@
             config["approach"] == "weight_only"
             and version.parse(neural_compressor.__version__) < version.parse("2.3.0")
         ), "Require neural-compressor >= 2.3.0 to support weight only quantization."
 
         # start with a copy of the config
         run_config = deepcopy(config)
         require_dataloader = run_config["approach"] == "static" or (
-            run_config["approach"] == "weight_only" and run_config["weight_only_config"]["algorithm"].upper() == "GPTQ"
+            run_config["approach"] == "weight_only"
+            and run_config["weight_only_config"]["algorithm"].upper() in {"GPTQ", "AWQ"}
         )
         if require_dataloader:
             assert (
                 config["dataloader_func"] or config["data_config"]
             ), "dataloader_func or data_config is required for {} quantization.".format(run_config["approach"])
 
         output_model_path = resolve_onnx_path(output_model_path, Path(model.model_path).name)
```

## olive/passes/onnx/onnx_dag.py

```diff
@@ -110,14 +110,17 @@
         """
         for i in graph.input:
             ios[i.name] = OnnxIO(proto=i, source=SpecialInput.INPUT, graph_idx=graph_idx)
         for o in graph.output:
             ios[o.name] = OnnxIO(proto=o, destination=[SpecialOutput.OUTPUT], graph_idx=graph_idx)
         for initializer in graph.initializer:
             ios[initializer.name] = OnnxIO(proto=initializer, source=SpecialInput.INITIALIZER, graph_idx=graph_idx)
+        for vi in graph.value_info:
+            if vi.name not in ios:
+                ios[vi.name] = OnnxIO(proto=vi, graph_idx=graph_idx)
         return ios
 
     @staticmethod
     def _process_node(
         node_proto: NodeProto,
         nodes: Dict[str, OnnxNode],
         ios: Dict[str, OnnxIO],
@@ -142,14 +145,17 @@
             inputs=list(node_proto.input),
             outputs=list(node_proto.output),
             graph_idx=graph_idx,
         )
         nodes[name] = onnx_node
 
         for i in node_proto.input:
+            if i == "":
+                # some nodes have unnamed, unused inputs
+                continue
             if i not in ios:
                 raise ValueError(
                     f"Input {i} does not exist in the graph. Please process the nodes in topological order."
                 )
             ios[i].destination.append(name)
             parent = ios[i].source
             if parent not in [SpecialInput.INPUT, SpecialInput.INITIALIZER]:
```

## olive/passes/onnx/perf_tuning.py

```diff
@@ -9,16 +9,17 @@
 import tempfile
 import time
 from pathlib import Path
 from typing import Any, Callable, Dict, Union
 
 from olive.common.ort_inference import check_and_normalize_provider_args
 from olive.data.config import DataConfig
-from olive.evaluator.metric import LatencySubType, Metric, MetricType, joint_metric_key
+from olive.evaluator.metric import LatencySubType, Metric, MetricType
 from olive.evaluator.metric_config import get_user_config_properties_from_metric_type
+from olive.evaluator.metric_result import joint_metric_key
 from olive.exception import EXCEPTIONS_TO_RAISE
 from olive.hardware.accelerator import AcceleratorLookup, AcceleratorSpec
 from olive.model import ONNXModelHandler
 from olive.passes import Pass
 from olive.passes.pass_config import ParamCategory, PassConfigParam
 from olive.resource_path import OLIVE_RESOURCE_ANNOTATIONS
 
@@ -516,24 +517,27 @@
 
     def threads_num_binary_search(self, model, latency_metric, test_params, io_bind, tuning_op_result):
         """Binary search based benchmark for inter_op_num_threads and intra_op_num_threads."""
         import onnxruntime as ort
         import psutil
 
         # prepare the inter_op_num_threads/intra_op_num_threads to be tune.
+        threads_names = []
         extra_session_config = test_params["session_options"].get("extra_session_config")
         if extra_session_config:
             affinity_str = extra_session_config.get("session.intra_op_thread_affinities")
             if affinity_str:
                 test_params["session_options"]["intra_op_num_threads"] = get_thread_affinity_nums(affinity_str) + 1
                 threads_names = ["inter_op_num_threads"]
-        elif test_params["session_options"].get("execution_mode") == ort.ExecutionMode.ORT_SEQUENTIAL:
-            threads_names = ["intra_op_num_threads"]
-        else:
-            threads_names = ["inter_op_num_threads", "intra_op_num_threads"]
+
+        if not threads_names:
+            if test_params["session_options"].get("execution_mode") == ort.ExecutionMode.ORT_SEQUENTIAL:
+                threads_names = ["intra_op_num_threads"]
+            else:
+                threads_names = ["inter_op_num_threads", "intra_op_num_threads"]
 
         if (
             test_params["session_options"].get("inter_op_num_threads") is not None
             and test_params["session_options"].get("intra_op_num_threads") is not None
         ):
             # If user specify both inter_op_num_threads and intra_op_num_threads, we will not do tuning
             test_result = self.get_benchmark(model, latency_metric, test_params, io_bind, tuning_op_result)
```

## olive/passes/onnx/quantization.py

```diff
@@ -227,14 +227,16 @@
             Should be set to True if model is targeted for QNN EP.
         """,
     ),
 }
 
 
 def get_calibration_dataloader(data_root, user_module_loader, config):
+    dataloader = None
+
     if config["dataloader_func"]:
         # TODO(trajep): replace legacy dataloader_func with data config
         data_dir = get_local_path_from_root(data_root, config["data_dir"])
         dataloader = user_module_loader.call_object(
             config["dataloader_func"],
             data_dir,
             config["batch_size"],
@@ -373,15 +375,15 @@
             extra_options[key] = run_config[key]
             del run_config[key]
 
         # preprocess the model
         # we hash the entire path of the input model to ensure we are not accidentally using a preprocessed model
         # from a different model
         preprocessed_temp_model_path = (
-            Path(self.tmp_dir.name) / f"{hash_string(str(Path(model.model_path).resolve()))}" / "preprocessed.onnx"
+            Path(self.tmp_dir.name) / f"{hash_string(str(Path(model.model_path).resolve()))[:8]}" / "preprocessed.onnx"
         )
         preprocessed_temp_model_path.parent.mkdir(exist_ok=True, parents=True)
         if run_config["quant_preprocess"]:
             if not preprocessed_temp_model_path.exists():
                 # overwrite the model path with the preprocessed model path
                 logger.info("Preprocessing model for quantization")
                 model = self._quant_preprocess(model, preprocessed_temp_model_path)
```

## olive/passes/onnx/transformer_optimization.py

```diff
@@ -8,15 +8,21 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Union
 
 import onnx
 
 from olive.common.utils import exclude_keys
 from olive.hardware.accelerator import AcceleratorSpec, Device
 from olive.model import ONNXModelHandler
-from olive.model.utils import HIDDEN_SIZE_NAMES, MODEL_TYPE_MAPPING, NUM_HEADS_NAMES, resolve_onnx_path
+from olive.model.utils import (
+    HIDDEN_SIZE_NAMES,
+    MODEL_TYPE_MAPPING,
+    NUM_HEADS_NAMES,
+    NUM_KEY_VALUE_HEADS_NAMES,
+    resolve_onnx_path,
+)
 from olive.passes import Pass
 from olive.passes.onnx.common import get_external_data_config, model_proto_to_olive_model
 from olive.passes.pass_config import PassConfigParam
 from olive.strategy.search_parameter import Boolean, Categorical, Conditional
 
 if TYPE_CHECKING:
     from onnxruntime.transformers.onnx_model import OnnxModel
@@ -27,41 +33,51 @@
 class OrtTransformersOptimization(Pass):
     """Use ONNX Transformer Optimizer to optimize transformer based models.
 
     Optimize transformer based models in scenarios where ONNX Runtime does not apply the optimization at load time.
     It is based on onnxruntime.transformers.optimizer.
     """
 
-    run_on_target = True
+    # NOTE: Don't run this on target since it only needs to create an inference session if `opt_level` > 0
+    # this is not common and running on target blocks cross platform workflows such as optimizing for DML EP
+    # using a Linux machine which doesn't support onnxruntime-directml package.
+    # It is enough for the pass to fail if `opt_level` > 0 and the host doesn't have the required packages.
 
     @staticmethod
     def is_accelerator_agnostic(accelerator_spec: AcceleratorSpec) -> bool:
         """Override this method to return False by using the accelerator spec information."""
         from onnxruntime import __version__ as OrtVersion
         from packaging import version
 
         return version.parse(OrtVersion) < version.parse("1.17.0")
 
     @classmethod
     def _default_config(cls, accelerator_spec: AcceleratorSpec) -> Dict[str, PassConfigParam]:
         from onnxruntime.transformers.fusion_options import FusionOptions
 
-        is_gpu = accelerator_spec.accelerator_type == Device.GPU
+        # if device is GPU, but user choose CPU EP, the is_gpu should be False
+        is_gpu = (
+            accelerator_spec.accelerator_type == Device.GPU
+            and accelerator_spec.execution_provider != "CPUExecutionProvider"
+        )
 
         config = {
             "model_type": PassConfigParam(
                 type_=str,
                 default_value=None,
                 description=(
                     "Transformer based model type, including bert (exported by PyTorch), gpt2 (exported by PyTorch), "
                     "bert_tf (BERT exported by tf2onnx), bert_keras (BERT exported by keras2onnx), and "
                     "unet/vae/clip (stable diffusion)."
                 ),
             ),
             "num_heads": PassConfigParam(type_=int, default_value=0, description="Number of attention heads."),
+            "num_key_value_heads": PassConfigParam(
+                type_=int, default_value=0, description="Number of key/value attention heads."
+            ),
             "hidden_size": PassConfigParam(type_=int, default_value=0, description="Number of hidden nodes."),
             # TODO(jambayk): Figure out what the expected type is
             "optimization_options": PassConfigParam(
                 type_=Union[Dict[str, Any], FusionOptions],
                 default_value=None,
                 description="Optimization options that turn on/off some fusions.",
             ),
@@ -205,24 +221,27 @@
         run_config["optimization_options"] = fusion_options
 
     def _run_for_config(
         self, model: ONNXModelHandler, data_root: str, config: Dict[str, Any], output_model_path: str
     ) -> ONNXModelHandler:
         from onnxruntime.transformers import optimizer as transformers_optimizer
 
+        num_kv_heads = config["num_key_value_heads"]
+
         # start with a copy of the config
         run_config = deepcopy(config)
         keys_to_remove = [
             "float16",
             "keep_io_types",
             "force_fp32_ops",
             "force_fp32_nodes",
             "force_fp16_inputs",
             "use_gqa",
             "input_int32",
+            "num_key_value_heads",
         ]
         keys_to_remove += get_external_data_config()
         run_config = exclude_keys(run_config, keys_to_remove)
 
         if model.model_attributes:
             model_attributes = model.model_attributes
             input_model_type = model_attributes.get("model_type")
@@ -241,14 +260,19 @@
                         break
             if run_config["hidden_size"] == 0:
                 for hidden_size_name in HIDDEN_SIZE_NAMES:
                     if hidden_size_name in model_attributes:
                         run_config["hidden_size"] = model_attributes[hidden_size_name]
                         logger.debug("hidden_size is set to %d from model attributes", run_config["hidden_size"])
                         break
+            if num_kv_heads == 0:
+                for num_key_value_heads_name in NUM_KEY_VALUE_HEADS_NAMES:
+                    if num_key_value_heads_name in model_attributes:
+                        num_kv_heads = model_attributes[num_key_value_heads_name]
+                        break
 
         if run_config["model_type"] is None or run_config["model_type"] not in transformers_optimizer.MODEL_TYPES:
             raise ValueError(
                 f"Unsupported model type: {run_config['model_type']}, please select one from "
                 f"[{', '.join(transformers_optimizer.MODEL_TYPES.keys())}] which need to be set under "
                 "OrtTransformersOptimization.config"
             )
@@ -288,24 +312,15 @@
                 keep_io_types=config["keep_io_types"],
                 op_block_list=config["force_fp32_ops"],
                 node_block_list=config["force_fp32_nodes"],
                 force_fp16_inputs=config["force_fp16_inputs"],
             )
 
             if config["use_gqa"]:
-                # Replace MultiHeadAttention with GroupQueryAttention
-                # TODO(anyone): treat `num_key_value_heads` like `num_heads` and `hidden_size`.
-                # Should be provided either in the model attributes or in the config.
-                num_kv_heads = model.model_attributes.get("num_key_value_heads", None)
-                if num_kv_heads is None:
-                    raise ValueError(
-                        "num_key_value_heads is not specified in the model attributes. "
-                        "Please specify it in the model attributes."
-                    )
-                world_size = model.model_attributes.get("world_size") or 1
+                world_size = model.model_attributes.get("world_size", 1) if model.model_attributes is not None else 1
                 optimizer = self._replace_mha_with_gqa(optimizer, kv_num_heads=num_kv_heads, world_size=world_size)
                 optimizer.prune_graph()
                 # add allow_remove_graph_inputs to pass config
                 optimizer.update_graph(allow_remove_graph_inputs=True)
 
         if config["input_int32"]:
             optimizer.change_graph_inputs_to_int32()
```

## olive/passes/onnx/vitis_ai_quantization.py

```diff
@@ -285,15 +285,15 @@
             extra_options[key] = run_config[key]
             del run_config[key]
 
         # preprocess the model
         # we hash the entire path of the input model to ensure we are not accidentally using a preprocessed model
         # from a different model
         preprocessed_temp_model_path = (
-            Path(self.tmp_dir.name) / f"{hash_string(str(Path(model.model_path).resolve()))}" / "preprocessed.onnx"
+            Path(self.tmp_dir.name) / f"{hash_string(str(Path(model.model_path).resolve()))[:8]}" / "preprocessed.onnx"
         )
         preprocessed_temp_model_path.parent.mkdir(exist_ok=True, parents=True)
         if run_config["quant_preprocess"]:
             if not preprocessed_temp_model_path.exists():
                 # overwrite the model path with the preprocessed model path
                 logger.info("Preprocessing model for quantization")
                 model = self._quant_preprocess(model, preprocessed_temp_model_path)
@@ -335,14 +335,15 @@
         # the pass inefficient
         tmp_dir = tempfile.TemporaryDirectory(prefix="olive_vaiq_tmp")
         tmp_dir_path = Path(tmp_dir.name)
         tmp_model_path = str(tmp_dir_path / Path(output_model_path).name)
 
         # get the dataloader
         # TODO(XiaoSheng): only use data config
+        dataloader = None
         if config["dataloader_func"]:
             data_dir = get_local_path_from_root(data_root, config["data_dir"])
             dataloader = self._user_module_loader.call_object(
                 config["dataloader_func"],
                 data_dir,
                 config["batch_size"],
                 **(config["dataloader_func_kwargs"] or {}),
```

## olive/passes/onnx/vitis_ai/calibrate.py

```diff
@@ -177,15 +177,14 @@
     use_external_data_format=False,
     execution_providers=["CPUExecutionProvider"],
     extra_options={},
 ):
     calibrator = None
 
     # default settings for min-max algorithm
-    method = method
     symmetric = False if "symmetric" not in extra_options else extra_options["symmetric"]
 
     if method == PowerOfTwoMethod.NonOverflow:
         calibrator = MinMaxCalibrater(
             model,
             op_types_to_calibrate,
             augmented_model_path,
@@ -204,7 +203,9 @@
         )
 
     if calibrator:
         calibrator.augment_graph()
         calibrator.execution_providers = execution_providers
         calibrator.create_inference_session()
         return calibrator
+    else:
+        return calibrator
```

## olive/passes/onnx/vitis_ai/quant_utils.py

```diff
@@ -86,14 +86,16 @@
     """
     Quantize the input data using the PowerOfTwoMethod.
     """
     if method == PowerOfTwoMethod.NonOverflow:
         pos = get_pos_overflow(data)
     elif method == PowerOfTwoMethod.MinMSE:
         pos = get_pos_min_mse(data)
+    else:
+        raise ValueError(f"Unsupported method: {method}")
 
     scale, lower_bound, upper_bound = get_bound_and_scale(pos)
     zero_point = 0
     quantized_data = vitis_quantize(data, pos=pos)
     return lower_bound, upper_bound, zero_point, scale, quantized_data
 
 
@@ -358,16 +360,14 @@
     - *q*: quantized value
     - *S*: scale
     - *z*: zero point
     """
     if is_ort_version_below_1_17():
         rmin = 0
         rmax = 0
-        zero_point = 0
-        scale = 1.0
         if isinstance(data, np.ndarray):
             rmin = data.min()
             rmax = data.max()
 
         elif isinstance(data, list) and len(data):
             rmin = min(data)
             rmax = max(data)
@@ -422,14 +422,16 @@
         rmin_mse = (qmin - zp_mse) * scale_mse
         rmax_mse = (qmax - zp_mse) * scale_mse
         if not is_ort_version_below_1_17():
             rmin_mse = np.array(rmin_mse, dtype=rmin_dtype)
             rmax_mse = np.array(rmax_mse, dtype=rmax.dtype)
 
         return rmin_mse, rmax_mse, zp_mse, scale_mse, quantized_data_mse
+    else:
+        raise ValueError(f"Unsupported method: {method}")
 
 
 def is_ort_version_below_1_16():
     """
     This function checks whether the current version of ONNX Runtime (ORT) is below 1.16.0.
 
     Returns:
@@ -442,7 +444,17 @@
     """
     This function checks whether the current version of ONNX Runtime (ORT) is below 1.17.0.
 
     Returns:
         True if the current ORT version is less than 1.17.0, False otherwise.
     """
     return version.parse(OrtVersion) < version.parse("1.17.0")
+
+
+def is_ort_version_below_1_18():
+    """
+    This function checks whether the current version of ONNX Runtime (ORT) is below 1.18.0.
+
+    Returns:
+        True if the current ORT version is less than 1.18.0, False otherwise.
+    """
+    return version.parse(OrtVersion) < version.parse("1.18.0")
```

## olive/passes/onnx/vitis_ai/quantize.py

```diff
@@ -163,15 +163,16 @@
             "extra_options": extra_options,
         }
         # for ORT version < 1.16.0, set optimize_model to False
         # always set it to False since it is not recommended and is removed in ORT 1.16.0
         # user needs to call pre-process to optimize the model
         if is_ort_version_below_1_16():
             ort_quantize_args["optimize_model"] = False
-        return ort_quantize_static(**ort_quantize_args)
+        ort_quantize_static(**ort_quantize_args)
+        return
 
     mode = QuantizationMode.QLinearOps
 
     if not op_types_to_quantize or len(op_types_to_quantize) == 0:
         q_linear_ops = list(QLinearOpsRegistry.keys())
         qdq_ops = list(QDQRegistry.keys())
         op_types_to_quantize = list(set(q_linear_ops + qdq_ops))
```

## olive/passes/onnx/vitis_ai/quantizer.py

```diff
@@ -40,95 +40,185 @@
     PowerOfTwoMethod,
     compute_scale_zp_pof2s,
     convert_relu_input_to_annotate_output,
     get_annotate_output_name,
     get_qdq_to_remove,
     get_relu_name,
     is_ort_version_below_1_17,
+    is_ort_version_below_1_18,
     quantize_data_pof2s,
     remove_nodes,
     vitis_quantize_data,
 )
 from olive.passes.onnx.vitis_ai.refine import adjust_quantize_info
 
 logger = logging.getLogger(__name__)
 
 # pylint: skip-file
 # ruff: noqa
 
 
 class VitisDPUQuantizer(QDQQuantizer):
-    def __init__(
-        self,
-        model,
-        per_channel,
-        reduce_range,
-        mode,
-        static,
-        weight_qType,
-        activation_qType,
-        tensors_range,
-        nodes_to_quantize,
-        nodes_to_exclude,
-        op_types_to_quantize,
-        calibrate_method,
-        need_layer_fusing,
-        extra_options=None,
-    ):
-        QDQQuantizer.__init__(
+    if is_ort_version_below_1_18():
+
+        def __init__(
             self,
             model,
             per_channel,
             reduce_range,
             mode,
             static,
             weight_qType,
             activation_qType,
             tensors_range,
             nodes_to_quantize,
             nodes_to_exclude,
             op_types_to_quantize,
-            extra_options,
-        )
-        self.tensors_to_quantize = {}
-        self.calibrate_method = calibrate_method
-        self.need_layer_fusing = need_layer_fusing
-
-        if per_channel:
-            logger.warning(
-                "Only per-tensor quantization is supported when enable_dpu=True, `per_channel` will be set to False."
-            )
-
-        if activation_qType != QuantType.QInt8:
-            logger.warning(
-                "Only QuantType.QInt8 activation_type is supported is supported when enable_dpu=True, "
-                "`activation_type` will be set to QuantType.QInt8."
-            )
-
-        if weight_qType != QuantType.QInt8:
-            logger.warning(
-                "Only QuantType.QInt8 weight_type is supported when enable_dpu=True, `weight_type` will "
-                "be set to QuantType.QInt8."
-            )
-
-        # If using enable_dpu, QDQ should always appear as a pair.
-        # Therefore, we need to add qdq pair to weight.
-        if "AddQDQPairToWeight" in self.extra_options and not self.extra_options["AddQDQPairToWeight"]:
-            logger.warning("When using enable_dpu, AddQDQPairToWeight will be changed to true.")
-        self.add_qdq_pair_to_weight = True
-
-        # If using nable_dpu, QDQ should always set WeightSymmetric as True.
-        if "WeightSymmetric" in self.extra_options and not self.extra_options["WeightSymmetric"]:
-            logger.warning("When enable_dpu=True, WeightSymmetric will be set to true.")
-        self.is_weight_symmetric = True
-
-        # If using enable_dpu, QDQ should always always set ActivationSymmetric as True.
-        if "ActivationSymmetric" in self.extra_options and not self.extra_options["ActivationSymmetric"]:
-            logger.warning("When enable_dpu=True, ActivationSymmetric will be set to true.")
-        self.is_activation_symmetric = True
+            calibrate_method,
+            need_layer_fusing,
+            extra_options={},
+        ):
+            QDQQuantizer.__init__(
+                self,
+                model,
+                per_channel,
+                reduce_range,
+                mode,
+                static,
+                weight_qType,
+                activation_qType,
+                tensors_range,
+                nodes_to_quantize,
+                nodes_to_exclude,
+                op_types_to_quantize,
+                extra_options,
+            )
+            self.tensors_to_quantize = {}
+            self.calibrate_method = calibrate_method
+            self.need_layer_fusing = need_layer_fusing
+
+            if per_channel:
+                logger.warning(
+                    "Only per-tensor quantization is supported when enable_dpu=True, `per_channel` will be set to False."
+                )
+
+            if activation_qType != QuantType.QInt8:
+                logger.warning(
+                    "Only QuantType.QInt8 activation_type is supported is supported when enable_dpu=True, "
+                    "`activation_type` will be set to QuantType.QInt8."
+                )
+
+            if weight_qType != QuantType.QInt8:
+                logger.warning(
+                    "Only QuantType.QInt8 weight_type is supported when enable_dpu=True, `weight_type` will "
+                    "be set to QuantType.QInt8."
+                )
+
+            # If using enable_dpu, QDQ should always appear as a pair.
+            # Therefore, we need to add qdq pair to weight.
+            if "AddQDQPairToWeight" in self.extra_options and not self.extra_options["AddQDQPairToWeight"]:
+                logger.warning("When using enable_dpu, AddQDQPairToWeight will be changed to true.")
+            self.add_qdq_pair_to_weight = True
+
+            # If using nable_dpu, QDQ should always set WeightSymmetric as True.
+            if "WeightSymmetric" in self.extra_options and not self.extra_options["WeightSymmetric"]:
+                logger.warning("When enable_dpu=True, WeightSymmetric will be set to true.")
+            self.is_weight_symmetric = True
+
+            # If using enable_dpu, QDQ should always always set ActivationSymmetric as True.
+            if "ActivationSymmetric" in self.extra_options and not self.extra_options["ActivationSymmetric"]:
+                logger.warning("When enable_dpu=True, ActivationSymmetric will be set to true.")
+            self.is_activation_symmetric = True
+
+        def quantize_bias_tensor(self, bias_name, input_name, weight_name, beta=1.0):
+            weight = find_by_name(bias_name, self.model.initializer())
+            if weight is not None:
+                if weight.data_type == onnx_proto.TensorProto.FLOAT:
+                    # Use int8 quantization for bias as well as weights.
+                    self.tensors_to_quantize[bias_name] = QDQTensorQuantInfo()
+            else:
+                logger.warning("Expected {} to be a weight".format(bias_name))
+
+    else:
+
+        def __init__(
+            self,
+            model,
+            per_channel,
+            reduce_range,
+            mode,
+            static,
+            weight_qType,
+            activation_qType,
+            tensors_range,
+            nodes_to_quantize,
+            nodes_to_exclude,
+            op_types_to_quantize,
+            calibrate_method,
+            need_layer_fusing,
+            extra_options={},
+        ):
+            QDQQuantizer.__init__(
+                self,
+                model,
+                per_channel,
+                reduce_range,
+                weight_qType,
+                activation_qType,
+                tensors_range,
+                nodes_to_quantize,
+                nodes_to_exclude,
+                op_types_to_quantize,
+                extra_options,
+            )
+            self.tensors_to_quantize = {}
+            self.calibrate_method = calibrate_method
+            self.need_layer_fusing = need_layer_fusing
+
+            if per_channel:
+                logger.warning(
+                    "Only per-tensor quantization is supported when enable_dpu=True, `per_channel` will be set to False."
+                )
+
+            if activation_qType != QuantType.QInt8:
+                logger.warning(
+                    "Only QuantType.QInt8 activation_type is supported is supported when enable_dpu=True, "
+                    "`activation_type` will be set to QuantType.QInt8."
+                )
+
+            if weight_qType != QuantType.QInt8:
+                logger.warning(
+                    "Only QuantType.QInt8 weight_type is supported when enable_dpu=True, `weight_type` will "
+                    "be set to QuantType.QInt8."
+                )
+
+            # If using enable_dpu, QDQ should always appear as a pair.
+            # Therefore, we need to add qdq pair to weight.
+            if "AddQDQPairToWeight" in self.extra_options and not self.extra_options["AddQDQPairToWeight"]:
+                logger.warning("When using enable_dpu, AddQDQPairToWeight will be changed to true.")
+            self.add_qdq_pair_to_weight = True
+
+            # If using nable_dpu, QDQ should always set WeightSymmetric as True.
+            if "WeightSymmetric" in self.extra_options and not self.extra_options["WeightSymmetric"]:
+                logger.warning("When enable_dpu=True, WeightSymmetric will be set to true.")
+            self.is_weight_symmetric = True
+
+            # If using enable_dpu, QDQ should always always set ActivationSymmetric as True.
+            if "ActivationSymmetric" in self.extra_options and not self.extra_options["ActivationSymmetric"]:
+                logger.warning("When enable_dpu=True, ActivationSymmetric will be set to true.")
+            self.is_activation_symmetric = True
+
+        def quantize_bias_tensor(self, node_name, bias_name, input_name, weight_name, beta=1.0):
+            weight = find_by_name(bias_name, self.model.initializer())
+            if weight is not None:
+                if weight.data_type == onnx_proto.TensorProto.FLOAT:
+                    # Use int8 quantization for bias as well as weights.
+                    self.quantize_weight_tensor(bias_name)
+            else:
+                logger.warning("Expected {} to be a weight".format(bias_name))
 
     def vitis_quantize_initializer(self, weight, bit_width=8, keep_float_weight=False):
         # Find if this input is already quantized
         if weight.name in self.quantized_value_map:
             quantized_value = self.quantized_value_map[weight.name]
             return (
                 quantized_value.q_name,
@@ -226,660 +316,1153 @@
                 [weight_dequant_output],
                 add_dequant_suffix(weight_name),
                 axis=axis,
             )
 
             self.model.add_node(dequant_node)
 
-    def quantize_bias_tensor(self, bias_name, input_name, weight_name, beta=1.0):
-        weight = find_by_name(bias_name, self.model.initializer())
-        if weight is not None:
-            if weight.data_type == onnx_proto.TensorProto.FLOAT:
-                # Use int8 quantization for bias as well as weights.
-                self.tensors_to_quantize[bias_name] = QDQTensorQuantInfo()
-        else:
-            logger.warning("Expected {} to be a weight".format(bias_name))
-
     def _quantize_refine(self):
         self.model = adjust_quantize_info(
             self.model,
             adjust_vitis_sigmoid=True,
             adjust_shift_cut=True,
             adjust_shift_bias=True,
             adjust_shift_read=True,
             adjust_shift_write=True,
             align_concat=True,
             align_pool=True,
         )
 
 
-class VitisQOpQuantizer(ONNXQuantizer):
-    def __init__(
-        self,
-        model,
-        per_channel,
-        reduce_range,
-        mode,
-        static,
-        weight_qType,
-        activation_qType,
-        tensors_range,
-        nodes_to_quantize,
-        nodes_to_exclude,
-        op_types_to_quantize,
-        calibrate_method,
-        extra_options=None,
-    ):
-        ONNXQuantizer.__init__(
+if is_ort_version_below_1_18():
+
+    class VitisQOpQuantizer(ONNXQuantizer):
+        def __init__(
             self,
             model,
             per_channel,
             reduce_range,
             mode,
             static,
             weight_qType,
             activation_qType,
             tensors_range,
             nodes_to_quantize,
             nodes_to_exclude,
             op_types_to_quantize,
-            extra_options=None,
-        )
-        self.calibrate_method = calibrate_method
-
-    def quantize_initializer(self, weight, qType, reduce_range=False, keep_float_weight=False):
-        """
-        :param weight: TensorProto initializer
-        :param qType: type to quantize to
-        :param keep_float_weight: Whether to quantize the weight. In some cases, we only want to
-                                  qunatize scale and zero point. If keep_float_weight is False,
-                                  quantize the weight, or don't quantize the weight.
-        :return: quantized weight name, zero point name, scale name
-        """
-        # Find if this input is already quantized
-        if weight.name in self.quantized_value_map:
-            quantized_value = self.quantized_value_map[weight.name]
-            return (
-                quantized_value.q_name,
-                quantized_value.zp_name,
-                quantized_value.scale_name,
+            calibrate_method,
+            extra_options={},
+        ):
+            ONNXQuantizer.__init__(
+                self,
+                model,
+                per_channel,
+                reduce_range,
+                mode,
+                static,
+                weight_qType,
+                activation_qType,
+                tensors_range,
+                nodes_to_quantize,
+                nodes_to_exclude,
+                op_types_to_quantize,
+                extra_options={},
             )
+            self.calibrate_method = calibrate_method
 
-        q_weight_name = weight.name + TENSOR_NAME_QUANT_SUFFIX
-        zp_name = weight.name + "_zero_point"
-        scale_name = weight.name + "_scale"
-
-        # Update packed weight, zero point, and scale initializers
-        weight_data = tensor_proto_to_array(weight)
-        _, _, zero_point, scale, q_weight_data = quantize_data_pof2s(
-            weight_data.flatten(),
-            qType,
-            self.is_weight_symmetric,
-            self.reduce_range and reduce_range,
-            method=PowerOfTwoMethod.NonOverflow,
-        )
-        if is_ort_version_below_1_17():
-            scale_qType = onnx_proto.TensorProto.FLOAT
-            weight_qType = onnx.mapping.TENSOR_TYPE_TO_NP_TYPE[qType]
-        else:
-            scale_qType = onnx.helper.np_dtype_to_tensor_dtype(scale.dtype)
-            weight_qType = onnx.helper.tensor_dtype_to_np_dtype(qType)
-
-        scale_initializer = onnx.helper.make_tensor(scale_name, scale_qType, [], [float(scale)])
-        zero_initializer = onnx.helper.make_tensor(zp_name, qType, [], [int(zero_point)])
-        self.model.initializer().extend([scale_initializer, zero_initializer])
-        if not keep_float_weight:
-            q_weight_data = np.asarray(q_weight_data, dtype=weight_qType).reshape(weight.dims)
-            q_weight_initializer = onnx.numpy_helper.from_array(q_weight_data, q_weight_name)
-            self.model.initializer().extend([q_weight_initializer])
-
-        # Log entry for this quantized weight
-        quantized_value = QuantizedValue(
-            weight.name,
-            q_weight_name,
-            scale_name,
-            zp_name,
-            QuantizedValueType.Initializer,
-            None,
-        )
-        self.quantized_value_map[weight.name] = quantized_value
-
-        return q_weight_name, zp_name, scale_name
-
-    def quantize_weight_per_channel(
-        self,
-        weight_name,
-        weight_qType,
-        channel_axis,
-        reduce_range=True,
-        keep_float_weight=False,
-    ):
-        # Find if this input is already quantized
-        if weight_name in self.quantized_value_map:
-            quantized_value = self.quantized_value_map[weight_name]
-            return (
-                quantized_value.q_name,
-                quantized_value.zp_name,
-                quantized_value.scale_name,
-            )
+        def quantize_initializer(self, weight, qType, reduce_range=False, keep_float_weight=False):
+            """
+            :param weight: TensorProto initializer
+            :param qType: type to quantize to
+            :param keep_float_weight: Whether to quantize the weight. In some cases, we only want to
+                                    qunatize scale and zero point. If keep_float_weight is False,
+                                    quantize the weight, or don't quantize the weight.
+            :return: quantized weight name, zero point name, scale name
+            """
+            # Find if this input is already quantized
+            if weight.name in self.quantized_value_map:
+                quantized_value = self.quantized_value_map[weight.name]
+                return (
+                    quantized_value.q_name,
+                    quantized_value.zp_name,
+                    quantized_value.scale_name,
+                )
 
-        initializer = find_by_name(weight_name, self.model.initializer())
-        if initializer is None:
-            raise ValueError("{} is not an initializer", weight_name)
-
-        weights = tensor_proto_to_array(initializer)
-        channel_count = weights.shape[channel_axis]
-        rmin_list = []
-        rmax_list = []
-        zero_point_list = []
-        scale_list = []
-        quantized_per_channel_data_list = []
-        for i in range(channel_count):
-            per_channel_data = weights.take(i, channel_axis)
-            rmin, rmax, zero_point, scale, quantized_per_channel_data = quantize_data_pof2s(
-                per_channel_data.flatten().tolist(),
-                weight_qType,
-                self.is_weight_symmetric or weight_qType == onnx_proto.TensorProto.INT8,
+            q_weight_name = weight.name + TENSOR_NAME_QUANT_SUFFIX
+            zp_name = weight.name + "_zero_point"
+            scale_name = weight.name + "_scale"
+
+            # Update packed weight, zero point, and scale initializers
+            weight_data = tensor_proto_to_array(weight)
+            _, _, zero_point, scale, q_weight_data = quantize_data_pof2s(
+                weight_data.flatten(),
+                qType,
+                self.is_weight_symmetric,
                 self.reduce_range and reduce_range,
                 method=PowerOfTwoMethod.NonOverflow,
             )
-            rmin_list.append(rmin)
-            rmax_list.append(rmax)
-            zero_point_list.append(zero_point)
-            scale_list.append(scale)
-            quantized_per_channel_data_list.append(quantized_per_channel_data)
-
-        # combine per_channel_data into one
-        reshape_dims = list(weights.shape)  # deep copy
-        reshape_dims[channel_axis] = 1  # only one per channel for reshape
-        quantized_weights = np.asarray(quantized_per_channel_data_list[0]).reshape(reshape_dims)
-        for i in range(1, len(quantized_per_channel_data_list)):
-            channel_weights = np.asarray(quantized_per_channel_data_list[i]).reshape(reshape_dims)
-            quantized_weights = np.concatenate((quantized_weights, channel_weights), channel_axis)
-
-        q_weight_name = weight_name + TENSOR_NAME_QUANT_SUFFIX
-        zp_name = weight_name + "_zero_point"
-        scale_name = weight_name + "_scale"
-
-        quantized_value = QuantizedValue(
-            weight_name,
-            q_weight_name,
-            scale_name,
-            zp_name,
-            QuantizedValueType.Initializer,
-            None,
-        )
-        self.quantized_value_map[weight_name] = quantized_value
+            if is_ort_version_below_1_17():
+                scale_qType = onnx_proto.TensorProto.FLOAT
+                weight_qType = onnx.mapping.TENSOR_TYPE_TO_NP_TYPE[qType]
+            else:
+                scale_qType = onnx.helper.np_dtype_to_tensor_dtype(scale.dtype)
+                weight_qType = onnx.helper.tensor_dtype_to_np_dtype(qType)
 
-        # Update packed weight, zero point, and scale initializers
-        zero_scale_shape = [initializer.dims[channel_axis]]
-        scale_initializer = onnx.helper.make_tensor(
-            scale_name, onnx_proto.TensorProto.FLOAT, zero_scale_shape, scale_list
-        )
-        zero_initializer = onnx.helper.make_tensor(zp_name, weight_qType, zero_scale_shape, zero_point_list)
+            scale_initializer = onnx.helper.make_tensor(scale_name, scale_qType, [], [float(scale)])
+            zero_initializer = onnx.helper.make_tensor(zp_name, qType, [], [int(zero_point)])
+            self.model.initializer().extend([scale_initializer, zero_initializer])
+            if not keep_float_weight:
+                q_weight_data = np.asarray(q_weight_data, dtype=weight_qType).reshape(weight.dims)
+                q_weight_initializer = onnx.numpy_helper.from_array(q_weight_data, q_weight_name)
+                self.model.initializer().extend([q_weight_initializer])
 
-        self.model.initializer().extend([scale_initializer, zero_initializer])
+            # Log entry for this quantized weight
+            quantized_value = QuantizedValue(
+                weight.name,
+                q_weight_name,
+                scale_name,
+                zp_name,
+                QuantizedValueType.Initializer,
+                None,
+            )
+            self.quantized_value_map[weight.name] = quantized_value
 
-        if not keep_float_weight:
-            quantized_weights = np.asarray(
-                quantized_weights,
-                dtype=onnx.mapping.TENSOR_TYPE_TO_NP_TYPE[weight_qType],
-            ).reshape(initializer.dims)
-            q_weight_initializer = onnx.numpy_helper.from_array(quantized_weights, q_weight_name)
-            self.model.initializer().extend([q_weight_initializer])
+            return q_weight_name, zp_name, scale_name
 
-        return q_weight_name, zp_name, scale_name
+        def quantize_weight_per_channel(
+            self,
+            weight_name,
+            weight_qType,
+            channel_axis,
+            reduce_range=True,
+            keep_float_weight=False,
+        ):
+            # Find if this input is already quantized
+            if weight_name in self.quantized_value_map:
+                quantized_value = self.quantized_value_map[weight_name]
+                return (
+                    quantized_value.q_name,
+                    quantized_value.zp_name,
+                    quantized_value.scale_name,
+                )
 
-    def calculate_quantization_params(self):
-        from olive.passes.onnx.vitis_ai.quant_utils import is_ort_version_below_1_16, is_ort_version_below_1_17
+            initializer = find_by_name(weight_name, self.model.initializer())
+            if initializer is None:
+                raise ValueError("{} is not an initializer", weight_name)
+
+            weights = tensor_proto_to_array(initializer)
+            channel_count = weights.shape[channel_axis]
+            rmin_list = []
+            rmax_list = []
+            zero_point_list = []
+            scale_list = []
+            quantized_per_channel_data_list = []
+            for i in range(channel_count):
+                per_channel_data = weights.take(i, channel_axis)
+                rmin, rmax, zero_point, scale, quantized_per_channel_data = quantize_data_pof2s(
+                    per_channel_data.flatten().tolist(),
+                    weight_qType,
+                    self.is_weight_symmetric or weight_qType == onnx_proto.TensorProto.INT8,
+                    self.reduce_range and reduce_range,
+                    method=PowerOfTwoMethod.NonOverflow,
+                )
+                rmin_list.append(rmin)
+                rmax_list.append(rmax)
+                zero_point_list.append(zero_point)
+                scale_list.append(scale)
+                quantized_per_channel_data_list.append(quantized_per_channel_data)
+
+            # combine per_channel_data into one
+            reshape_dims = list(weights.shape)  # deep copy
+            reshape_dims[channel_axis] = 1  # only one per channel for reshape
+            quantized_weights = np.asarray(quantized_per_channel_data_list[0]).reshape(reshape_dims)
+            for i in range(1, len(quantized_per_channel_data_list)):
+                channel_weights = np.asarray(quantized_per_channel_data_list[i]).reshape(reshape_dims)
+                quantized_weights = np.concatenate((quantized_weights, channel_weights), channel_axis)
+
+            q_weight_name = weight_name + TENSOR_NAME_QUANT_SUFFIX
+            zp_name = weight_name + "_zero_point"
+            scale_name = weight_name + "_scale"
 
-        if self.tensors_range is None:
-            return
+            quantized_value = QuantizedValue(
+                weight_name,
+                q_weight_name,
+                scale_name,
+                zp_name,
+                QuantizedValueType.Initializer,
+                None,
+            )
+            self.quantized_value_map[weight_name] = quantized_value
 
-        # adjust tensor_ranges for input of Clip and Relu node
-        for node in self.model.nodes():
-            if node.op_type not in ["Clip", "Relu"]:
-                continue
-            if self.is_activation_symmetric:
-                continue
-            if not self.should_quantize_node(node):
-                continue
-            if len(self.model.input_name_to_nodes()[node.input[0]]) != 1:
-                continue
-            if node.input[0] not in self.tensors_range or node.output[0] not in self.tensors_range:
-                continue
-            self.tensors_range[node.input[0]] = self.tensors_range[node.output[0]]
-        quantization_params = {}
-        if is_ort_version_below_1_16():
-            for tensor_name in self.tensors_range.keys():
-                rmin, rmax = self.tensors_range[tensor_name]
-                qmin, qmax = get_qmin_qmax_for_qType(self.activation_qType, symmetric=self.is_activation_symmetric)
+            # Update packed weight, zero point, and scale initializers
+            zero_scale_shape = [initializer.dims[channel_axis]]
+            scale_initializer = onnx.helper.make_tensor(
+                scale_name, onnx_proto.TensorProto.FLOAT, zero_scale_shape, scale_list
+            )
+            zero_initializer = onnx.helper.make_tensor(zp_name, weight_qType, zero_scale_shape, zero_point_list)
 
-                quantization_params[tensor_name] = compute_scale_zp_pof2s(
-                    rmin, rmax, qmin, qmax, self.is_activation_symmetric
-                )
-        else:
-            from onnxruntime.quantization.onnx_quantizer import QuantizationParams
+            self.model.initializer().extend([scale_initializer, zero_initializer])
 
-            for tensor_name in self.tensors_range:
-                td = self.tensors_range[tensor_name]
-                rmin, rmax = td.range_value
-                qmin, qmax = get_qmin_qmax_for_qType(self.activation_qType, symmetric=self.is_activation_symmetric)
+            if not keep_float_weight:
+                quantized_weights = np.asarray(
+                    quantized_weights,
+                    dtype=onnx.mapping.TENSOR_TYPE_TO_NP_TYPE[weight_qType],
+                ).reshape(initializer.dims)
+                q_weight_initializer = onnx.numpy_helper.from_array(quantized_weights, q_weight_name)
+                self.model.initializer().extend([q_weight_initializer])
+
+            return q_weight_name, zp_name, scale_name
+
+        def calculate_quantization_params(self):
+            from olive.passes.onnx.vitis_ai.quant_utils import is_ort_version_below_1_16, is_ort_version_below_1_17
+
+            if self.tensors_range is None:
+                return None
+
+            # adjust tensor_ranges for input of Clip and Relu node
+            for node in self.model.nodes():
+                if node.op_type not in ["Clip", "Relu"]:
+                    continue
+                if self.is_activation_symmetric:
+                    continue
+                if not self.should_quantize_node(node):
+                    continue
+                if len(self.model.input_name_to_nodes()[node.input[0]]) != 1:
+                    continue
+                if node.input[0] not in self.tensors_range or node.output[0] not in self.tensors_range:
+                    continue
+                self.tensors_range[node.input[0]] = self.tensors_range[node.output[0]]
+            quantization_params = {}
+            if is_ort_version_below_1_16():
+                for tensor_name in self.tensors_range.keys():
+                    rmin, rmax = self.tensors_range[tensor_name]
+                    qmin, qmax = get_qmin_qmax_for_qType(self.activation_qType, symmetric=self.is_activation_symmetric)
 
-                zero, scale = compute_scale_zp_pof2s(rmin, rmax, qmin, qmax, self.is_activation_symmetric)
-                if is_ort_version_below_1_17():
-                    quantization_params[tensor_name] = QuantizationParams(zero_point=int(zero), scale=float(scale))
-                else:
-                    quantization_params[tensor_name] = QuantizationParams(
-                        zero_point=zero, scale=scale, quant_type=self.activation_qType
+                    quantization_params[tensor_name] = compute_scale_zp_pof2s(
+                        rmin, rmax, qmin, qmax, self.is_activation_symmetric
                     )
+            else:
+                from onnxruntime.quantization.onnx_quantizer import QuantizationParams
 
-        return quantization_params
+                for tensor_name in self.tensors_range:
+                    td = self.tensors_range[tensor_name]
+                    rmin, rmax = td.range_value
+                    qmin, qmax = get_qmin_qmax_for_qType(self.activation_qType, symmetric=self.is_activation_symmetric)
+
+                    zero, scale = compute_scale_zp_pof2s(rmin, rmax, qmin, qmax, self.is_activation_symmetric)
+                    if is_ort_version_below_1_17():
+                        quantization_params[tensor_name] = QuantizationParams(zero_point=int(zero), scale=float(scale))
+                    else:
+                        quantization_params[tensor_name] = QuantizationParams(
+                            zero_point=zero, scale=scale, quant_type=self.activation_qType
+                        )
 
+            return quantization_params
 
-class VitisQDQQuantizer(VitisQOpQuantizer):
-    def __init__(
-        self,
-        model,
-        per_channel,
-        reduce_range,
-        mode,
-        static,
-        weight_qType,
-        activation_qType,
-        tensors_range,
-        nodes_to_quantize,
-        nodes_to_exclude,
-        op_types_to_quantize,
-        extra_options=None,
-    ):
-        ONNXQuantizer.__init__(
+    class VitisQDQQuantizer(VitisQOpQuantizer):
+        def __init__(
             self,
             model,
             per_channel,
             reduce_range,
             mode,
             static,
             weight_qType,
             activation_qType,
             tensors_range,
             nodes_to_quantize,
             nodes_to_exclude,
             op_types_to_quantize,
-            extra_options,
-        )
-        self.tensors_to_quantize = {}
-        self.bias_to_quantize = []
-
-        self.nodes_to_remove = []
+            extra_options={},
+        ):
+            ONNXQuantizer.__init__(
+                self,
+                model,
+                per_channel,
+                reduce_range,
+                mode,
+                static,
+                weight_qType,
+                activation_qType,
+                tensors_range,
+                nodes_to_quantize,
+                nodes_to_exclude,
+                op_types_to_quantize,
+                extra_options,
+            )
+            self.tensors_to_quantize = {}
+            self.bias_to_quantize = []
 
-        # Specific op types to exclude qdq quantization for their outputs.
-        # In TRT, it's not recommended to quantize outputs for weighted ops such as Conv, Matmul, Gemm
-        # because those ops may be followed by nodes that require high resolution inputs.
-        # Adding QDQ for those ops' output may end up with worse accuracy.
-        # So, we don't recommend to add QDQ to node's output under such condition.
-        self.op_types_to_exclude_output_quantization = (
-            []
-            if "OpTypesToExcludeOutputQuantization" not in extra_options
-            else extra_options["OpTypesToExcludeOutputQuantization"]
-        )
+            self.nodes_to_remove = []
 
-        # We do quantization on Dequantizelinear's input to remove Quantizelinear for weight as an optimization.
-        # In some cases, for example QDQ BERT model for TensorRT, QDQ should always appear as a pair.
-        # Therefore, we need to disable this optimization and add qdq pair to weight.
-        self.add_qdq_pair_to_weight = (
-            False if "AddQDQPairToWeight" not in extra_options else extra_options["AddQDQPairToWeight"]
-        )
+            # Specific op types to exclude qdq quantization for their outputs.
+            # In TRT, it's not recommended to quantize outputs for weighted ops such as Conv, Matmul, Gemm
+            # because those ops may be followed by nodes that require high resolution inputs.
+            # Adding QDQ for those ops' output may end up with worse accuracy.
+            # So, we don't recommend to add QDQ to node's output under such condition.
+            self.op_types_to_exclude_output_quantization = (
+                []
+                if "OpTypesToExcludeOutputQuantization" not in extra_options
+                else extra_options["OpTypesToExcludeOutputQuantization"]
+            )
 
-        # The default behavior is that multiple nodes can share a QDQ pair as their inputs.
-        # In TRT, QDQ pair can’t be shared between nodes, so it will create dedicated QDQ pairs for each node.
-        self.dedicated_qdq_pair = (
-            False if "DedicatedQDQPair" not in extra_options else extra_options["DedicatedQDQPair"]
-        )
-        if self.dedicated_qdq_pair:
-            self.tensor_to_its_receiving_nodes = {}
+            # We do quantization on Dequantizelinear's input to remove Quantizelinear for weight as an optimization.
+            # In some cases, for example QDQ BERT model for TensorRT, QDQ should always appear as a pair.
+            # Therefore, we need to disable this optimization and add qdq pair to weight.
+            self.add_qdq_pair_to_weight = (
+                False if "AddQDQPairToWeight" not in extra_options else extra_options["AddQDQPairToWeight"]
+            )
 
-        # Let user set channel axis for specific op type and it's effective only when per channel quantization
-        # is supported and per_channel is True.
-        self.qdq_op_type_per_channel_support_to_axis = (
-            {}
-            if "QDQOpTypePerChannelSupportToAxis" not in extra_options
-            else extra_options["QDQOpTypePerChannelSupportToAxis"]
-        )
+            # The default behavior is that multiple nodes can share a QDQ pair as their inputs.
+            # In TRT, QDQ pair can’t be shared between nodes, so it will create dedicated QDQ pairs for each node.
+            self.dedicated_qdq_pair = (
+                False if "DedicatedQDQPair" not in extra_options else extra_options["DedicatedQDQPair"]
+            )
+            if self.dedicated_qdq_pair:
+                self.tensor_to_its_receiving_nodes = {}
 
-    def _is_tensor_quantizable(self, tensor_name):
-        """
-        Check if tensor can be quantized
-        """
-        return self._tensor_quantizable_data_type(tensor_name) is not None
-
-    def _tensor_quantizable_data_type(self, tensor_name):
-        """
-        Return the tensor type if it is quantizable.
-        """
-        weight = find_by_name(tensor_name, self.model.initializer())
-        if weight is not None:
-            if weight.data_type in {onnx_proto.TensorProto.FLOAT, onnx_proto.TensorProto.FLOAT16}:
-                return weight.data_type
-        elif tensor_name in self.value_infos.keys():
-            vi = self.value_infos[tensor_name]
-            if vi.type.HasField("tensor_type") and vi.type.tensor_type.elem_type in {
-                TensorProto.FLOAT,
-                TensorProto.FLOAT16,
-            }:
-                return vi.type.tensor_type.elem_type
-        else:
-            logger.warning(
-                "failed to infer the type of tensor: {}. Skip to quantize it. Please check if it is expected.".format(
-                    tensor_name
-                )
+            # Let user set channel axis for specific op type and it's effective only when per channel quantization
+            # is supported and per_channel is True.
+            self.qdq_op_type_per_channel_support_to_axis = (
+                {}
+                if "QDQOpTypePerChannelSupportToAxis" not in extra_options
+                else extra_options["QDQOpTypePerChannelSupportToAxis"]
             )
 
-        return None
-
-    def __quantize_tensor(self, tensor_name, quant_sharing_param=None, tensor_type=QDQQuantTensorType.ACTIVATION):
-        """
-        Quantize tensors. If quant_param_tensor is not None, tensor with name tensor_name will be quantized with same
-        quantization parameters as tensor quant_param_tensor
-        Args:
-            tensor_name: name of the tensor to quantize
-            quant_sharing_param: name of the tensor that provides quantization parameter
-            tensor_type: QDQQuantTensorType default ACTIVATION
-        """
-        data_type = self._tensor_quantizable_data_type(tensor_name)
-        if data_type is not None:
-            if quant_sharing_param:
-                try:
-                    self.tensors_to_quantize[tensor_name] = QDQTensorQuantInfo(
-                        tensor_type=tensor_type, quant_para_provider=quant_sharing_param, data_type=data_type
-                    )
-                except TypeError:
-                    # onnxruntime<1.17
-                    self.tensors_to_quantize[tensor_name] = QDQTensorQuantInfo(
-                        tensor_type=tensor_type,
-                        quant_para_provider=quant_sharing_param,
-                    )
-            elif tensor_name not in self.tensors_to_quantize:
-                try:
-                    self.tensors_to_quantize[tensor_name] = QDQTensorQuantInfo(
-                        tensor_type=tensor_type, data_type=data_type
+        def _is_tensor_quantizable(self, tensor_name):
+            """
+            Check if tensor can be quantized
+            """
+            return self._tensor_quantizable_data_type(tensor_name) is not None
+
+        def _tensor_quantizable_data_type(self, tensor_name):
+            """
+            Return the tensor type if it is quantizable.
+            """
+            weight = find_by_name(tensor_name, self.model.initializer())
+            if weight is not None:
+                if weight.data_type in {onnx_proto.TensorProto.FLOAT, onnx_proto.TensorProto.FLOAT16}:
+                    return weight.data_type
+            elif tensor_name in self.value_infos.keys():
+                vi = self.value_infos[tensor_name]
+                if vi.type.HasField("tensor_type") and vi.type.tensor_type.elem_type in {
+                    TensorProto.FLOAT,
+                    TensorProto.FLOAT16,
+                }:
+                    return vi.type.tensor_type.elem_type
+            else:
+                logger.warning(
+                    "failed to infer the type of tensor: {}. Skip to quantize it. Please check if it is expected.".format(
+                        tensor_name
                     )
-                except TypeError:
-                    # onnxruntime<1.17
-                    self.tensors_to_quantize[tensor_name] = QDQTensorQuantInfo(tensor_type=tensor_type)
-
-    def quantize_activation_tensor(self, tensor_name, quant_sharing_param=None):
-        """
-        Quantize Activation Tensor
-        Args:
-            tensor_name: name of the tensor to quantize
-            quant_sharing_param: name of the tensor that provides quantization parameter
-        """
-        return self.__quantize_tensor(tensor_name, quant_sharing_param, QDQQuantTensorType.ACTIVATION)
-
-    def quantize_weight_tensor(self, tensor_name, quant_sharing_param=None):
-        """
-        Quantize Weight Tensor
-        Args:
-            tensor_name: name of the tensor to quantize
-            quant_sharing_param: name of the tensor that provides quantization parameter
-        """
-        return self.__quantize_tensor(tensor_name, quant_sharing_param, QDQQuantTensorType.WEIGHT)
-
-    def quantize_weight_tensor_per_channel(self, tensor_name, axis):
-        weight = find_by_name(tensor_name, self.model.initializer())
-        if weight:
-            if weight.data_type == onnx_proto.TensorProto.FLOAT:
-                self.tensors_to_quantize[tensor_name] = QDQTensorQuantInfo(
-                    tensor_type=QDQQuantTensorType.WEIGHT, axis=axis
                 )
-        else:
-            logger.warning(
-                "only support per-channel quantization on weight. Tensor: {} is not quantized.".format(tensor_name)
-            )
-
-    def quantize_bias_tensor(self, bias_name, input_name, weight_name, beta=1.0):
-        weight = find_by_name(bias_name, self.model.initializer())
-        if weight is not None:
-            if weight.data_type == onnx_proto.TensorProto.FLOAT:
-                self.bias_to_quantize.append((bias_name, input_name, weight_name, beta))
-        else:
-            logger.warning("Expected {} to be a weight".format(bias_name))
 
-    def remove_node(self, node):
-        self.nodes_to_remove.append(node)
+            return None
 
-    def remove_nodes(self):
-        self.model.remove_nodes(self.nodes_to_remove)
-
-    def quantize_model(self):
-        for node in self.model.nodes():
-            if self.should_quantize_node(node):
-                op_quantizer = CreateQDQQuantizer(self, node)
-                op_quantizer.quantize()
+        def __quantize_tensor(self, tensor_name, quant_sharing_param=None, tensor_type=QDQQuantTensorType.ACTIVATION):
+            """
+            Quantize tensors. If quant_param_tensor is not None, tensor with name tensor_name will be quantized with same
+            quantization parameters as tensor quant_param_tensor
+            Args:
+                tensor_name: name of the tensor to quantize
+                quant_sharing_param: name of the tensor that provides quantization parameter
+                tensor_type: QDQQuantTensorType default ACTIVATION
+            """
+            data_type = self._tensor_quantizable_data_type(tensor_name)
+            if data_type is not None:
+                if quant_sharing_param:
+                    try:
+                        self.tensors_to_quantize[tensor_name] = QDQTensorQuantInfo(
+                            tensor_type=tensor_type, quant_para_provider=quant_sharing_param, data_type=data_type
+                        )
+                    except TypeError:
+                        # onnxruntime<1.17
+                        self.tensors_to_quantize[tensor_name] = QDQTensorQuantInfo(
+                            tensor_type=tensor_type,
+                            quant_para_provider=quant_sharing_param,
+                        )
+                elif tensor_name not in self.tensors_to_quantize:
+                    try:
+                        self.tensors_to_quantize[tensor_name] = QDQTensorQuantInfo(
+                            tensor_type=tensor_type, data_type=data_type
+                        )
+                    except TypeError:
+                        # onnxruntime<1.17
+                        self.tensors_to_quantize[tensor_name] = QDQTensorQuantInfo(tensor_type=tensor_type)
+
+        def quantize_activation_tensor(self, tensor_name, quant_sharing_param=None):
+            """
+            Quantize Activation Tensor
+            Args:
+                tensor_name: name of the tensor to quantize
+                quant_sharing_param: name of the tensor that provides quantization parameter
+            """
+            return self.__quantize_tensor(tensor_name, quant_sharing_param, QDQQuantTensorType.ACTIVATION)
+
+        def quantize_weight_tensor(self, tensor_name, quant_sharing_param=None):
+            """
+            Quantize Weight Tensor
+            Args:
+                tensor_name: name of the tensor to quantize
+                quant_sharing_param: name of the tensor that provides quantization parameter
+            """
+            return self.__quantize_tensor(tensor_name, quant_sharing_param, QDQQuantTensorType.WEIGHT)
+
+        def quantize_weight_tensor_per_channel(self, tensor_name, axis):
+            weight = find_by_name(tensor_name, self.model.initializer())
+            if weight:
+                if weight.data_type == onnx_proto.TensorProto.FLOAT:
+                    self.tensors_to_quantize[tensor_name] = QDQTensorQuantInfo(
+                        tensor_type=QDQQuantTensorType.WEIGHT, axis=axis
+                    )
+            else:
+                logger.warning(
+                    "only support per-channel quantization on weight. Tensor: {} is not quantized.".format(tensor_name)
+                )
 
-                if self.dedicated_qdq_pair:
-                    for tensor_name in node.input:
-                        if tensor_name not in self.tensor_to_its_receiving_nodes:
-                            self.tensor_to_its_receiving_nodes[tensor_name] = []
-                        self.tensor_to_its_receiving_nodes[tensor_name].append(node)
+        def quantize_bias_tensor(self, bias_name, input_name, weight_name, beta=1.0):
+            weight = find_by_name(bias_name, self.model.initializer())
+            if weight is not None:
+                if weight.data_type == onnx_proto.TensorProto.FLOAT:
+                    self.bias_to_quantize.append((bias_name, input_name, weight_name, beta))
+            else:
+                logger.warning("Expected {} to be a weight".format(bias_name))
 
-        self._quantize_normal_tensors()
-        self._quantize_sharing_param_tensors()
-        self._quantize_bias_tensors()
-        self.remove_nodes()
-        if not self.add_qdq_pair_to_weight:
-            self.model.clean_initializers()
+        def remove_node(self, node):
+            self.nodes_to_remove.append(node)
 
-        self.model.model.producer_name = __producer__
-        self.model.model.producer_version = __version__
+        def remove_nodes(self):
+            self.model.remove_nodes(self.nodes_to_remove)
 
-        return self.model.model
+        def quantize_model(self):
+            for node in self.model.nodes():
+                if self.should_quantize_node(node):
+                    op_quantizer = CreateQDQQuantizer(self, node)
+                    op_quantizer.quantize()
+
+                    if self.dedicated_qdq_pair:
+                        for tensor_name in node.input:
+                            if tensor_name not in self.tensor_to_its_receiving_nodes:
+                                self.tensor_to_its_receiving_nodes[tensor_name] = []
+                            self.tensor_to_its_receiving_nodes[tensor_name].append(node)
+
+            self._quantize_normal_tensors()
+            self._quantize_sharing_param_tensors()
+            self._quantize_bias_tensors()
+            self.remove_nodes()
+            if not self.add_qdq_pair_to_weight:
+                self.model.clean_initializers()
+
+            self.model.model.producer_name = __producer__
+            self.model.model.producer_version = __version__
+
+            return self.model.model
+
+        def try_replacing_upstream_output(self, upstream_output_name, output_name):
+            if (
+                output_name in self.quantization_params.keys()
+                and len(self.model.input_name_to_nodes()[upstream_output_name]) == 1
+                and not self.model.is_graph_output(upstream_output_name)
+                and not self.model.is_graph_input(upstream_output_name)
+            ):
+                self.model.replace_output_of_all_nodes(upstream_output_name, output_name)
+                if upstream_output_name in self.tensors_to_quantize:
+                    del self.tensors_to_quantize[upstream_output_name]
+                return True
+            return False
 
-    def try_replacing_upstream_output(self, upstream_output_name, output_name):
-        if (
-            output_name in self.quantization_params.keys()
-            and len(self.model.input_name_to_nodes()[upstream_output_name]) == 1
-            and not self.model.is_graph_output(upstream_output_name)
-            and not self.model.is_graph_input(upstream_output_name)
-        ):
-            self.model.replace_output_of_all_nodes(upstream_output_name, output_name)
-            if upstream_output_name in self.tensors_to_quantize:
-                del self.tensors_to_quantize[upstream_output_name]
-            return True
-        return False
-
-    def _create_qdq_nodes(
-        self, q_input, q_output, quant_node_name, dq_input, dq_output, dequant_node_name, scale_name, zp_name, axis=None
-    ):
-        qlinear_node = onnx.helper.make_node(
-            QUANT_OP_NAME,
-            [q_input, scale_name, zp_name],
-            [q_output],
+        def _create_qdq_nodes(
+            self,
+            q_input,
+            q_output,
             quant_node_name,
-            axis=axis,
-        )
-        dequant_node = onnx.helper.make_node(
-            DEQUANT_OP_NAME,
-            [dq_input, scale_name, zp_name],
-            [dq_output],
+            dq_input,
+            dq_output,
             dequant_node_name,
-            axis=axis,
-        )
-        self.model.add_nodes([qlinear_node, dequant_node])
-
-    def _add_qdq_pair_for_initializer(self, weight_proto, tensor_type, axis=None):
-        weight_name = weight_proto.name
-        if axis is not None:
-            if self.opset_version < 13:
-                raise ValueError("Per-Channel support with QDQ format requires onnx opset version 13 or above.")
-            q_weight_name, zp_name, scale_name = self.quantize_weight_per_channel(
-                weight_name, onnx_proto.TensorProto.INT8, axis, keep_float_weight=self.add_qdq_pair_to_weight
-            )
-        else:
-            q_weight_name, zp_name, scale_name = self.quantize_initializer(
-                weight_proto,
-                self.weight_qType if tensor_type is QDQQuantTensorType.WEIGHT else self.activation_qType,
-                keep_float_weight=self.add_qdq_pair_to_weight,
-            )
-
-        weight_dequant_output = add_dequant_output_suffix(weight_name)
-        self.model.replace_input_of_all_nodes(weight_name, weight_dequant_output)
-        if self.add_qdq_pair_to_weight:
-            weight_quant_output = add_quant_output_suffix(weight_name)
-
-            self._create_qdq_nodes(
-                weight_name,
-                weight_quant_output,
-                add_quant_suffix(weight_name),
-                weight_quant_output,
-                weight_dequant_output,
-                add_dequant_suffix(weight_name),
-                scale_name,
-                zp_name,
-                axis,
+            scale_name,
+            zp_name,
+            axis=None,
+        ):
+            qlinear_node = onnx.helper.make_node(
+                QUANT_OP_NAME,
+                [q_input, scale_name, zp_name],
+                [q_output],
+                quant_node_name,
+                axis=axis,
             )
-        else:
             dequant_node = onnx.helper.make_node(
                 DEQUANT_OP_NAME,
-                [q_weight_name, scale_name, zp_name],
-                [weight_dequant_output],
-                add_dequant_suffix(weight_name),
+                [dq_input, scale_name, zp_name],
+                [dq_output],
+                dequant_node_name,
                 axis=axis,
             )
-            self.model.add_node(dequant_node)
+            self.model.add_nodes([qlinear_node, dequant_node])
+
+        def _add_qdq_pair_for_initializer(self, weight_proto, tensor_type, axis=None):
+            weight_name = weight_proto.name
+            if axis is not None:
+                if self.opset_version < 13:
+                    raise ValueError("Per-Channel support with QDQ format requires onnx opset version 13 or above.")
+                q_weight_name, zp_name, scale_name = self.quantize_weight_per_channel(
+                    weight_name, onnx_proto.TensorProto.INT8, axis, keep_float_weight=self.add_qdq_pair_to_weight
+                )
+            else:
+                q_weight_name, zp_name, scale_name = self.quantize_initializer(
+                    weight_proto,
+                    self.weight_qType if tensor_type is QDQQuantTensorType.WEIGHT else self.activation_qType,
+                    keep_float_weight=self.add_qdq_pair_to_weight,
+                )
+
+            weight_dequant_output = add_dequant_output_suffix(weight_name)
+            self.model.replace_input_of_all_nodes(weight_name, weight_dequant_output)
+            if self.add_qdq_pair_to_weight:
+                weight_quant_output = add_quant_output_suffix(weight_name)
 
-    def _add_qdq_pair_for_activation(self, tensor_name, scale_name, zp_name):
-        if (
-            self.dedicated_qdq_pair
-            and tensor_name in self.tensor_to_its_receiving_nodes
-            and len(self.tensor_to_its_receiving_nodes[tensor_name]) > 1
-        ):
-            num_dedicated_qdq_pair = len(self.tensor_to_its_receiving_nodes[tensor_name])
-            for i in range(num_dedicated_qdq_pair):
-                postfix = f"_{i + 1}"
-                tensor_name_quant_output_postfix = add_quant_output_suffix(tensor_name) + postfix
-                tensor_name_dequant_output_postfix = add_dequant_output_suffix(tensor_name) + postfix
-                quant_node_name_postfix = add_quant_suffix(tensor_name) + postfix
-                dequant_node_name_postfix = add_dequant_suffix(tensor_name) + postfix
                 self._create_qdq_nodes(
-                    tensor_name,
-                    tensor_name_quant_output_postfix,
-                    quant_node_name_postfix,
-                    tensor_name_quant_output_postfix,
-                    tensor_name_dequant_output_postfix,
-                    dequant_node_name_postfix,
+                    weight_name,
+                    weight_quant_output,
+                    add_quant_suffix(weight_name),
+                    weight_quant_output,
+                    weight_dequant_output,
+                    add_dequant_suffix(weight_name),
                     scale_name,
                     zp_name,
+                    axis,
                 )
+            else:
+                dequant_node = onnx.helper.make_node(
+                    DEQUANT_OP_NAME,
+                    [q_weight_name, scale_name, zp_name],
+                    [weight_dequant_output],
+                    add_dequant_suffix(weight_name),
+                    axis=axis,
+                )
+                self.model.add_node(dequant_node)
 
-                node = self.tensor_to_its_receiving_nodes[tensor_name][i]
-                self.model.replace_node_input(node, tensor_name, tensor_name_dequant_output_postfix)
-                if i == 0:
-                    quantized_value = QuantizedValue(
+        def _add_qdq_pair_for_activation(self, tensor_name, scale_name, zp_name):
+            if (
+                self.dedicated_qdq_pair
+                and tensor_name in self.tensor_to_its_receiving_nodes
+                and len(self.tensor_to_its_receiving_nodes[tensor_name]) > 1
+            ):
+                num_dedicated_qdq_pair = len(self.tensor_to_its_receiving_nodes[tensor_name])
+                for i in range(num_dedicated_qdq_pair):
+                    postfix = f"_{i + 1}"
+                    tensor_name_quant_output_postfix = add_quant_output_suffix(tensor_name) + postfix
+                    tensor_name_dequant_output_postfix = add_dequant_output_suffix(tensor_name) + postfix
+                    quant_node_name_postfix = add_quant_suffix(tensor_name) + postfix
+                    dequant_node_name_postfix = add_dequant_suffix(tensor_name) + postfix
+                    self._create_qdq_nodes(
                         tensor_name,
+                        tensor_name_quant_output_postfix,
+                        quant_node_name_postfix,
+                        tensor_name_quant_output_postfix,
                         tensor_name_dequant_output_postfix,
+                        dequant_node_name_postfix,
                         scale_name,
                         zp_name,
-                        QuantizedValueType.Input,
                     )
-                    self.quantized_value_map[tensor_name] = quantized_value
-        else:
-            q_input = tensor_name
-            dq_output = add_dequant_output_suffix(tensor_name)
-            if self.model.is_graph_output(tensor_name):
-                q_input = add_quant_input_suffix(tensor_name)
-                dq_output = tensor_name
-                self.model.replace_output_of_all_nodes(tensor_name, q_input)
+
+                    node = self.tensor_to_its_receiving_nodes[tensor_name][i]
+                    self.model.replace_node_input(node, tensor_name, tensor_name_dequant_output_postfix)
+                    if i == 0:
+                        quantized_value = QuantizedValue(
+                            tensor_name,
+                            tensor_name_dequant_output_postfix,
+                            scale_name,
+                            zp_name,
+                            QuantizedValueType.Input,
+                        )
+                        self.quantized_value_map[tensor_name] = quantized_value
             else:
-                self.model.replace_input_of_all_nodes(tensor_name, dq_output)
+                q_input = tensor_name
+                dq_output = add_dequant_output_suffix(tensor_name)
+                if self.model.is_graph_output(tensor_name):
+                    q_input = add_quant_input_suffix(tensor_name)
+                    dq_output = tensor_name
+                    self.model.replace_output_of_all_nodes(tensor_name, q_input)
+                else:
+                    self.model.replace_input_of_all_nodes(tensor_name, dq_output)
 
-            self._create_qdq_nodes(
-                q_input,
-                add_quant_output_suffix(tensor_name),
-                add_quant_suffix(tensor_name),
-                add_quant_output_suffix(tensor_name),
-                dq_output,
-                add_dequant_suffix(tensor_name),
+                self._create_qdq_nodes(
+                    q_input,
+                    add_quant_output_suffix(tensor_name),
+                    add_quant_suffix(tensor_name),
+                    add_quant_output_suffix(tensor_name),
+                    dq_output,
+                    add_dequant_suffix(tensor_name),
+                    scale_name,
+                    zp_name,
+                )
+
+                quantized_value = QuantizedValue(
+                    tensor_name,
+                    dq_output,
+                    scale_name,
+                    zp_name,
+                    QuantizedValueType.Input,
+                )
+                self.quantized_value_map[tensor_name] = quantized_value
+
+        def _quantize_normal_tensors(self):
+            for tensor_name, tensor_info in self.tensors_to_quantize.copy().items():
+                if tensor_name in self.quantized_value_map.keys():
+                    continue
+
+                if not tensor_info.is_shared:
+                    # Quantize the input
+                    initializer = find_by_name(tensor_name, self.model.initializer())
+                    if initializer:
+                        self._add_qdq_pair_for_initializer(initializer, tensor_info.tensor_type, tensor_info.axis)
+                    else:
+                        used_scale, used_zp = self.find_quant_scale_zp(tensor_name)
+                        data_found, scale_name, zp_name, _, _ = self._get_quantization_params(
+                            tensor_name, used_scale, used_zp
+                        )
+
+                        if not data_found:
+                            raise ValueError(
+                                f"Quantization parameters are not specified for param {tensor_name}. "
+                                "In static mode quantization params for inputs and outputs of nodes to "
+                                "be quantized are required."
+                            )
+
+                        self._add_qdq_pair_for_activation(tensor_name, scale_name, zp_name)
+
+                    del self.tensors_to_quantize[tensor_name]
+
+        def _quantize_sharing_param_tensors(self):
+            while self.tensors_to_quantize:
+                for tensor_name, tensor_info in self.tensors_to_quantize.copy().items():
+                    tensor_provider_name = tensor_info.quant_para_provider
+                    if tensor_provider_name in self.quantized_value_map:
+                        del self.tensors_to_quantize[tensor_name]
+
+                        quantized_value = self.quantized_value_map[tensor_provider_name]
+                        # Quantize the input
+                        initializer = find_by_name(tensor_name, self.model.initializer())
+                        if initializer is not None:
+                            raise ValueError("Quantization parameter shared mode is not supported for weight yet")
+                        self._add_qdq_pair_for_activation(
+                            tensor_name, quantized_value.scale_name, quantized_value.zp_name
+                        )
+
+        def _quantize_bias_tensors(self):
+            for bias_name, input_name, weight_name, beta in self.bias_to_quantize:
+                if bias_name in self.quantized_value_map.keys():
+                    continue
+                # Quantize the input
+                self.quantize_bias_static(bias_name, input_name, weight_name, beta)
+                self.model.remove_initializer(find_by_name(bias_name, self.model.initializer()))
+                quant_value = self.quantized_value_map[bias_name]
+                inputs = [quant_value.q_name, quant_value.scale_name, quant_value.zp_name]
+                node_name = add_dequant_suffix(bias_name)
+                if quant_value.axis is not None:
+                    dequant_node = onnx.helper.make_node(
+                        "DequantizeLinear",
+                        inputs,
+                        [bias_name],
+                        node_name,
+                        axis=quant_value.axis,
+                    )
+                else:
+                    dequant_node = onnx.helper.make_node(
+                        "DequantizeLinear",
+                        inputs,
+                        [bias_name],
+                        node_name,
+                    )
+                self.model.add_node(dequant_node)
+
+        def is_tensor_quantized(self, tensor_name):
+            return tensor_name in self.tensors_to_quantize or tensor_name in self.bias_to_quantize
+
+else:
+    from onnxruntime.quantization.base_quantizer import QuantizationParams, to_array_extended
+    from onnxruntime.quantization.quant_utils import ONNX_TYPE_TO_NP_TYPE, normalize_axis, quantize_nparray
+
+    class VitisQOpQuantizer(ONNXQuantizer):
+        def __init__(
+            self,
+            model,
+            per_channel,
+            reduce_range,
+            mode,
+            static,
+            weight_qType,
+            activation_qType,
+            tensors_range,
+            nodes_to_quantize,
+            nodes_to_exclude,
+            op_types_to_quantize,
+            calibrate_method,
+            extra_options={},
+        ):
+            ONNXQuantizer.__init__(
+                self,
+                model,
+                per_channel,
+                reduce_range,
+                mode,
+                static,
+                weight_qType,
+                activation_qType,
+                tensors_range,
+                nodes_to_quantize,
+                nodes_to_exclude,
+                op_types_to_quantize,
+                extra_options={},
+            )
+            self.calibrate_method = calibrate_method
+
+        def quantize_initializer(self, weight, qType, reduce_range=False, keep_float_weight=False):
+            """
+            :param weight: TensorProto initializer
+            :param qType: type to quantize to
+            :param keep_float_weight: Whether to quantize the weight. In some cases, we only want to
+                                    qunatize scale and zero point. If keep_float_weight is False,
+                                    quantize the weight, or don't quantize the weight.
+            :return: quantized weight name, zero point name, scale name
+            """
+            # Find if this input is already quantized
+            if weight.name in self.quantized_value_map:
+                quantized_value = self.quantized_value_map[weight.name]
+                return (
+                    quantized_value.q_name,
+                    quantized_value.zp_name,
+                    quantized_value.scale_name,
+                )
+
+            q_weight_name = weight.name + TENSOR_NAME_QUANT_SUFFIX
+            zp_name = weight.name + "_zero_point"
+            scale_name = weight.name + "_scale"
+
+            # Update packed weight, zero point, and scale initializers
+            weight_data = tensor_proto_to_array(weight)
+            _, _, zero_point, scale, q_weight_data = quantize_data_pof2s(
+                weight_data.flatten(),
+                qType,
+                self.is_weight_symmetric,
+                self.reduce_range and reduce_range,
+                method=PowerOfTwoMethod.NonOverflow,
+            )
+            if is_ort_version_below_1_17():
+                scale_qType = onnx_proto.TensorProto.FLOAT
+                weight_qType = onnx.mapping.TENSOR_TYPE_TO_NP_TYPE[qType]
+            else:
+                scale_qType = onnx.helper.np_dtype_to_tensor_dtype(scale.dtype)
+                weight_qType = onnx.helper.tensor_dtype_to_np_dtype(qType)
+
+            scale_initializer = onnx.helper.make_tensor(scale_name, scale_qType, [], [float(scale)])
+            zero_initializer = onnx.helper.make_tensor(zp_name, qType, [], [int(zero_point)])
+            self.model.initializer().extend([scale_initializer, zero_initializer])
+            if not keep_float_weight:
+                q_weight_data = np.asarray(q_weight_data, dtype=weight_qType).reshape(weight.dims)
+                q_weight_initializer = onnx.numpy_helper.from_array(q_weight_data, q_weight_name)
+                self.model.initializer().extend([q_weight_initializer])
+
+            # Log entry for this quantized weight
+            quantized_value = QuantizedValue(
+                weight.name,
+                q_weight_name,
                 scale_name,
                 zp_name,
+                QuantizedValueType.Initializer,
+                None,
             )
+            self.quantized_value_map[weight.name] = quantized_value
+
+            return q_weight_name, zp_name, scale_name
+
+        def quantize_weight_per_channel(
+            self,
+            weight_name,
+            weight_qType,
+            channel_axis,
+            reduce_range=True,
+            keep_float_weight=False,
+        ):
+            # Find if this input is already quantized
+            if weight_name in self.quantized_value_map:
+                quantized_value = self.quantized_value_map[weight_name]
+                return (
+                    quantized_value.q_name,
+                    quantized_value.zp_name,
+                    quantized_value.scale_name,
+                )
+
+            initializer = find_by_name(weight_name, self.model.initializer())
+            if initializer is None:
+                raise ValueError("{} is not an initializer", weight_name)
+
+            weights = tensor_proto_to_array(initializer)
+            channel_count = weights.shape[channel_axis]
+            rmin_list = []
+            rmax_list = []
+            zero_point_list = []
+            scale_list = []
+            quantized_per_channel_data_list = []
+            for i in range(channel_count):
+                per_channel_data = weights.take(i, channel_axis)
+                rmin, rmax, zero_point, scale, quantized_per_channel_data = quantize_data_pof2s(
+                    per_channel_data.flatten().tolist(),
+                    weight_qType,
+                    self.is_weight_symmetric or weight_qType == onnx_proto.TensorProto.INT8,
+                    self.reduce_range and reduce_range,
+                    method=PowerOfTwoMethod.NonOverflow,
+                )
+                rmin_list.append(rmin)
+                rmax_list.append(rmax)
+                zero_point_list.append(zero_point)
+                scale_list.append(scale)
+                quantized_per_channel_data_list.append(quantized_per_channel_data)
+
+            # combine per_channel_data into one
+            reshape_dims = list(weights.shape)  # deep copy
+            reshape_dims[channel_axis] = 1  # only one per channel for reshape
+            quantized_weights = np.asarray(quantized_per_channel_data_list[0]).reshape(reshape_dims)
+            for i in range(1, len(quantized_per_channel_data_list)):
+                channel_weights = np.asarray(quantized_per_channel_data_list[i]).reshape(reshape_dims)
+                quantized_weights = np.concatenate((quantized_weights, channel_weights), channel_axis)
+
+            q_weight_name = weight_name + TENSOR_NAME_QUANT_SUFFIX
+            zp_name = weight_name + "_zero_point"
+            scale_name = weight_name + "_scale"
 
             quantized_value = QuantizedValue(
-                tensor_name,
-                dq_output,
+                weight_name,
+                q_weight_name,
                 scale_name,
                 zp_name,
-                QuantizedValueType.Input,
+                QuantizedValueType.Initializer,
+                None,
             )
-            self.quantized_value_map[tensor_name] = quantized_value
+            self.quantized_value_map[weight_name] = quantized_value
 
-    def _quantize_normal_tensors(self):
-        for tensor_name, tensor_info in self.tensors_to_quantize.copy().items():
-            if tensor_name in self.quantized_value_map.keys():
-                continue
+            # Update packed weight, zero point, and scale initializers
+            zero_scale_shape = [initializer.dims[channel_axis]]
+            scale_initializer = onnx.helper.make_tensor(
+                scale_name, onnx_proto.TensorProto.FLOAT, zero_scale_shape, scale_list
+            )
+            zero_initializer = onnx.helper.make_tensor(zp_name, weight_qType, zero_scale_shape, zero_point_list)
 
-            if not tensor_info.is_shared:
-                # Quantize the input
-                initializer = find_by_name(tensor_name, self.model.initializer())
-                if initializer:
-                    self._add_qdq_pair_for_initializer(initializer, tensor_info.tensor_type, tensor_info.axis)
-                else:
-                    used_scale, used_zp = self.find_quant_scale_zp(tensor_name)
-                    data_found, scale_name, zp_name, _, _ = self._get_quantization_params(
-                        tensor_name, used_scale, used_zp
+            self.model.initializer().extend([scale_initializer, zero_initializer])
+
+            if not keep_float_weight:
+                quantized_weights = np.asarray(
+                    quantized_weights,
+                    dtype=onnx.mapping.TENSOR_TYPE_TO_NP_TYPE[weight_qType],
+                ).reshape(initializer.dims)
+                q_weight_initializer = onnx.numpy_helper.from_array(quantized_weights, q_weight_name)
+                self.model.initializer().extend([q_weight_initializer])
+
+            return q_weight_name, zp_name, scale_name
+
+        def calculate_quantization_params(self):
+            from olive.passes.onnx.vitis_ai.quant_utils import is_ort_version_below_1_16, is_ort_version_below_1_17
+
+            if self.tensors_range is None:
+                return None
+
+            # adjust tensor_ranges for input of Clip and Relu node
+            for node in self.model.nodes():
+                if node.op_type not in ["Clip", "Relu"]:
+                    continue
+                if self.is_activation_symmetric:
+                    continue
+                if not self.should_quantize_node(node):
+                    continue
+                if len(self.model.input_name_to_nodes()[node.input[0]]) != 1:
+                    continue
+                if node.input[0] not in self.tensors_range or node.output[0] not in self.tensors_range:
+                    continue
+                self.tensors_range[node.input[0]] = self.tensors_range[node.output[0]]
+            quantization_params = {}
+            if is_ort_version_below_1_16():
+                for tensor_name in self.tensors_range.keys():
+                    rmin, rmax = self.tensors_range[tensor_name]
+                    qmin, qmax = get_qmin_qmax_for_qType(self.activation_qType, symmetric=self.is_activation_symmetric)
+
+                    quantization_params[tensor_name] = compute_scale_zp_pof2s(
+                        rmin, rmax, qmin, qmax, self.is_activation_symmetric
                     )
+            else:
+                from onnxruntime.quantization.onnx_quantizer import QuantizationParams
 
-                    if not data_found:
-                        raise ValueError(
-                            f"Quantization parameters are not specified for param {tensor_name}. "
-                            "In static mode quantization params for inputs and outputs of nodes to "
-                            "be quantized are required."
+                for tensor_name in self.tensors_range:
+                    td = self.tensors_range[tensor_name]
+                    rmin, rmax = td.range_value
+                    qmin, qmax = get_qmin_qmax_for_qType(self.activation_qType, symmetric=self.is_activation_symmetric)
+
+                    zero, scale = compute_scale_zp_pof2s(rmin, rmax, qmin, qmax, self.is_activation_symmetric)
+                    if is_ort_version_below_1_17():
+                        quantization_params[tensor_name] = QuantizationParams(zero_point=int(zero), scale=float(scale))
+                    else:
+                        quantization_params[tensor_name] = QuantizationParams(
+                            zero_point=zero, scale=scale, quant_type=self.activation_qType
                         )
 
-                    self._add_qdq_pair_for_activation(tensor_name, scale_name, zp_name)
+            return quantization_params
+
+    class VitisQDQQuantizer(QDQQuantizer):
+        def __init__(
+            self,
+            model,
+            per_channel,
+            reduce_range,
+            mode,
+            static,
+            weight_qType,
+            activation_qType,
+            tensors_range,
+            nodes_to_quantize,
+            nodes_to_exclude,
+            op_types_to_quantize,
+            calibrate_method,
+            extra_options={},
+        ):
+            QDQQuantizer.__init__(
+                self,
+                model,
+                per_channel,
+                reduce_range,
+                weight_qType,
+                activation_qType,
+                tensors_range,
+                nodes_to_quantize,
+                nodes_to_exclude,
+                op_types_to_quantize,
+                extra_options,
+            )
+            self.calibrate_method = calibrate_method
+
+            # Specific op types to exclude qdq quantization for their outputs.
+            # In TRT, it's not recommended to quantize outputs for weighted ops such as Conv, Matmul, Gemm
+            # because those ops may be followed by nodes that require high resolution inputs.
+            # Adding QDQ for those ops' output may end up with worse accuracy.
+            # So, we don't recommend to add QDQ to node's output under such condition.
+
+        def quantize_initializer_impl(self, weight, qType, reduce_range=False, keep_float_weight=False):
+            """
+            :param weight: TensorProto initializer
+            :param qType: type to quantize to
+            :param keep_float_weight: Whether to quantize the weight. In some cases, we only want to qunatize scale and zero point.
+                                    If keep_float_weight is False, quantize the weight, or don't quantize the weight.
+            :return: quantized weight name, zero point name, scale name
+            """
+            q_weight_name = weight.name + TENSOR_NAME_QUANT_SUFFIX
+            zp_name = weight.name + "_zero_point"
+            scale_name = weight.name + "_scale"
+
+            # Quantize weight data. Use quantization overrides if provided by the user.
+            weight_data = tensor_proto_to_array(weight)
+            quant_overrides = self.tensor_quant_overrides.get_per_tensor_overrides(weight.name, default_val={})
+            if "quant_type" in quant_overrides:
+                qType = quant_overrides["quant_type"].tensor_type  # noqa: N806
+
+            if "scale" in quant_overrides and "zero_point" in quant_overrides:
+                zero_point = np.array(quant_overrides["zero_point"], dtype=ONNX_TYPE_TO_NP_TYPE[qType])
+                scale = np.array(quant_overrides["scale"])
+                q_weight_data = quantize_nparray(qType, weight_data.flatten(), scale, zero_point)
+                assert isinstance(zero_point, np.ndarray), f"Unexpected type {type(zero_point)}"
+                assert (
+                    zero_point.dtype != np.float32 and zero_point.dtype != np.float16
+                ), f"Unexpected dtype {zero_point.dtype}"
+                assert isinstance(scale, np.ndarray), f"Unexpected type {type(scale)}"
 
-                del self.tensors_to_quantize[tensor_name]
+            else:
+                _, _, zero_point, scale, q_weight_data = quantize_data_pof2s(
+                    weight_data.flatten(),
+                    qType,
+                    self.is_weight_symmetric,
+                    self.reduce_range and reduce_range,
+                    method=PowerOfTwoMethod.NonOverflow,
+                )
 
-    def _quantize_sharing_param_tensors(self):
-        while self.tensors_to_quantize:
-            for tensor_name, tensor_info in self.tensors_to_quantize.copy().items():
-                tensor_provider_name = tensor_info.quant_para_provider
-                if tensor_provider_name in self.quantized_value_map:
-                    del self.tensors_to_quantize[tensor_name]
+                assert isinstance(zero_point, np.ndarray), f"Unexpected type {type(zero_point)}"
+                assert (
+                    zero_point.dtype != np.float32 and zero_point.dtype != np.float16
+                ), f"Unexpected dtype {zero_point.dtype}"
+                assert isinstance(scale, np.ndarray), f"Unexpected type {type(scale)}"
+
+            scale_dtype = weight.data_type
+            scale_initializer = onnx.helper.make_tensor(scale_name, scale_dtype, [], scale.reshape((-1,)).tolist())
+            zero_initializer = onnx.helper.make_tensor(zp_name, qType, [], zero_point.reshape((-1,)).tolist())
+            self.model.initializer_extend([scale_initializer, zero_initializer])
+
+            if not keep_float_weight:
+                if self.weight_qType == onnx.TensorProto.FLOAT8E4M3FN:
+                    q_weight_initializer = onnx.TensorProto()
+                    q_weight_initializer.data_type = self.weight_qType
+                    q_weight_initializer.dims.extend(weight.dims)
+                    q_weight_initializer.name = q_weight_name
+                    # Do not remove .flatten().copy() numpy is not clear about data persistence.
+                    q_weight_initializer.raw_data = q_weight_data.flatten().copy().tobytes()
+                    if to_array_extended is not None:
+                        # This test should not be needed but it helped catch some issues
+                        # with data persistence and tobytes.
+                        check = to_array_extended(q_weight_initializer)
+                        if check.shape != weight_data.shape or check.tobytes() != q_weight_data.tobytes():
+                            raise RuntimeError(
+                                f"The initializer of shape {weight_data.shape} could not be created, expecting "
+                                f"{q_weight_data.tobytes()[:10]}, got {check.tobytes()[:10]} and shape={weight.shape}"
+                                f"\nraw={str(q_weight_initializer)[:200]}."
+                            )
+                else:
+                    q_weight_data = np.asarray(
+                        q_weight_data, dtype=onnx.helper.tensor_dtype_to_np_dtype(qType)
+                    ).reshape(weight.dims)
+                    q_weight_initializer = onnx.numpy_helper.from_array(q_weight_data, q_weight_name)
+                self.model.initializer_extend([q_weight_initializer])
 
-                    quantized_value = self.quantized_value_map[tensor_provider_name]
-                    # Quantize the input
-                    initializer = find_by_name(tensor_name, self.model.initializer())
-                    if initializer is not None:
-                        raise ValueError("Quantization parameter shared mode is not supported for weight yet")
-                    self._add_qdq_pair_for_activation(tensor_name, quantized_value.scale_name, quantized_value.zp_name)
-
-    def _quantize_bias_tensors(self):
-        for bias_name, input_name, weight_name, beta in self.bias_to_quantize:
-            if bias_name in self.quantized_value_map.keys():
-                continue
-            # Quantize the input
-            self.quantize_bias_static(bias_name, input_name, weight_name, beta)
-            self.model.remove_initializer(find_by_name(bias_name, self.model.initializer()))
-            quant_value = self.quantized_value_map[bias_name]
-            inputs = [quant_value.q_name, quant_value.scale_name, quant_value.zp_name]
-            node_name = add_dequant_suffix(bias_name)
-            if quant_value.axis is not None:
-                dequant_node = onnx.helper.make_node(
-                    "DequantizeLinear",
-                    inputs,
-                    [bias_name],
-                    node_name,
-                    axis=quant_value.axis,
+            return q_weight_name, zp_name, scale_name
+
+        def quantize_weight_per_channel_impl(
+            self,
+            weight_name,
+            weight_qType,
+            channel_axis,
+            reduce_range=True,
+            keep_float_weight=False,
+        ):
+            initializer = find_by_name(weight_name, self.model.initializer())
+            if initializer is None:
+                raise ValueError("{} is not an initializer", weight_name)
+
+            weights = tensor_proto_to_array(initializer)
+            weights_rank = len(weights.shape)
+            is_axis_valid, axis_norm = normalize_axis(channel_axis, weights_rank)
+            if not is_axis_valid:
+                raise ValueError(
+                    f"Weight {weight_name} has a per-channel axis with value {channel_axis} that is "
+                    f"out-of-bounds for rank {weights_rank}"
                 )
-            else:
-                dequant_node = onnx.helper.make_node(
-                    "DequantizeLinear",
-                    inputs,
-                    [bias_name],
-                    node_name,
+
+            channel_axis = axis_norm
+            channel_count = weights.shape[channel_axis]
+            quant_overrides_for_channels = self.tensor_quant_overrides.get_per_channel_overrides(
+                weight_name, default_val=[{"axis": channel_axis}]
+            )
+
+            num_channel_overrides = len(quant_overrides_for_channels)
+            if num_channel_overrides != 1 and num_channel_overrides != channel_count:
+                raise ValueError(
+                    f"Per-channel tensor quantization overrides for {weight_name} must have "
+                    f"either 1 or {channel_count} elements in the list of dictionaries."
                 )
-            self.model.add_node(dequant_node)
 
-    def is_tensor_quantized(self, tensor_name):
-        return tensor_name in self.tensors_to_quantize or tensor_name in self.bias_to_quantize
+            is_axis_override_valid, axis_override = normalize_axis(
+                quant_overrides_for_channels[0]["axis"], weights_rank
+            )
+            if not is_axis_override_valid or axis_override != channel_axis:
+                raise ValueError(
+                    f"Tensor quantization overrides for {weight_name} specify an unexpected axis. "
+                    f"Expected {channel_axis}, but got {quant_overrides_for_channels[0]['axis']}."
+                )
+
+            # If user provides per-channel quantization overrides, all channels must use the same quant_type,
+            # axis, symmetric, and reduce_range values. So, just use the first channel's values.
+            if "quant_type" in quant_overrides_for_channels[0]:
+                weight_qType = quant_overrides_for_channels[0]["quant_type"].tensor_type  # noqa: N806
+
+            reduce_range = quant_overrides_for_channels[0].get("reduce_range", self.reduce_range and reduce_range)
+            zero_point_list = []
+            scale_list = []
+            quantized_per_channel_data_list = []
+            for i in range(channel_count):
+                per_channel_data = weights.take(i, channel_axis)
+                channel_override_index = i if i < num_channel_overrides else 0
+                channel_quant_overrides = quant_overrides_for_channels[channel_override_index]
+
+                if "scale" in channel_quant_overrides and "zero_point" in channel_quant_overrides:
+                    zero_point = np.array(
+                        channel_quant_overrides["zero_point"], dtype=ONNX_TYPE_TO_NP_TYPE[weight_qType]
+                    )
+                    scale = np.array(channel_quant_overrides["scale"])
+                    quantized_per_channel_data = quantize_nparray(
+                        weight_qType, per_channel_data.flatten(), scale, zero_point
+                    )
+                    assert isinstance(zero_point, np.ndarray), f"Unexpected type {type(zero_point)}"
+                    assert (
+                        zero_point.dtype != np.float32 and zero_point.dtype != np.float16
+                    ), f"Unexpected dtype {zero_point.dtype}"
+                    assert isinstance(scale, np.ndarray), f"Unexpected type {type(scale)}"
+                    assert isinstance(
+                        quantized_per_channel_data, np.ndarray
+                    ), f"Unexpected type {type(quantized_per_channel_data)}"
+
+                else:
+                    _, _, zero_point, scale, quantized_per_channel_data = quantize_data_pof2s(
+                        per_channel_data.flatten().tolist(),
+                        weight_qType,
+                        self.is_weight_symmetric or weight_qType == onnx_proto.TensorProto.INT8,
+                        self.reduce_range and reduce_range,
+                        method=PowerOfTwoMethod.NonOverflow,
+                    )
+
+                    assert isinstance(zero_point, np.ndarray), f"Unexpected type {type(zero_point)}"
+                    assert (
+                        zero_point.dtype != np.float32 and zero_point.dtype != np.float16
+                    ), f"Unexpected dtype {zero_point.dtype}"
+                    assert isinstance(scale, np.ndarray), f"Unexpected type {type(scale)}"
+                    assert isinstance(
+                        quantized_per_channel_data, np.ndarray
+                    ), f"Unexpected type {type(quantized_per_channel_data)}"
+
+                zero_point_list.append(zero_point)
+                scale_list.append(scale)
+                quantized_per_channel_data_list.append(quantized_per_channel_data)
+
+            # combine per_channel_data into one
+            reshape_dims = list(weights.shape)  # deep copy
+            reshape_dims[channel_axis] = 1  # only one per channel for reshape
+            quantized_weights = np.asarray(quantized_per_channel_data_list[0]).reshape(reshape_dims)
+            for i in range(1, len(quantized_per_channel_data_list)):
+                channel_weights = np.asarray(quantized_per_channel_data_list[i]).reshape(reshape_dims)
+                quantized_weights = np.concatenate((quantized_weights, channel_weights), channel_axis)
+
+            q_weight_name = weight_name + TENSOR_NAME_QUANT_SUFFIX
+            zp_name = weight_name + "_zero_point"
+            scale_name = weight_name + "_scale"
+
+            # Update packed weight, zero point, and scale initializers
+            zero_scale_shape = [initializer.dims[channel_axis]]
+            scale_initializer = onnx.helper.make_tensor(
+                scale_name, initializer.data_type, zero_scale_shape, np.hstack(scale_list).tolist()
+            )
+            zero_initializer = onnx.helper.make_tensor(
+                zp_name, weight_qType, zero_scale_shape, np.hstack(zero_point_list).tolist()
+            )
+
+            self.model.initializer_extend([scale_initializer, zero_initializer])
+
+            if not keep_float_weight:
+                quantized_weights = np.asarray(
+                    quantized_weights,
+                    dtype=onnx.mapping.TENSOR_TYPE_TO_NP_TYPE[weight_qType],
+                ).reshape(initializer.dims)
+                q_weight_initializer = onnx.numpy_helper.from_array(quantized_weights, q_weight_name)
+                self.model.initializer_extend([q_weight_initializer])
+
+            return q_weight_name, zp_name, scale_name
+
+        def calc_quant_params(self, tensor_data, quant_overrides):
+            """
+            Calculates quantization parameters (scale/zero-point) given a tensor's min/max range and optional
+            user-provided overrides.
+            """
+            quant_type = self.activation_qType
+            if "quant_type" in quant_overrides:
+                quant_type = quant_overrides["quant_type"].tensor_type
+
+            if "scale" in quant_overrides and "zero_point" in quant_overrides:
+                zero, scale = quant_overrides["zero_point"], quant_overrides["scale"]
+            else:
+                rmin = quant_overrides.get("rmin", tensor_data.range_value[0])
+                rmax = quant_overrides.get("rmax", tensor_data.range_value[1])
+                symmetric = quant_overrides.get("symmetric", self.is_activation_symmetric)
+                reduce_range = quant_overrides.get("reduce_range", False)
+                qmin, qmax = get_qmin_qmax_for_qType(quant_type, reduce_range=reduce_range, symmetric=symmetric)
+                zero, scale = compute_scale_zp_pof2s(rmin, rmax, qmin, qmax, self.is_activation_symmetric)
+
+            return QuantizationParams(zero_point=zero, scale=scale, quant_type=quant_type)
```

## olive/passes/onnx/vitis_ai/refine.py

```diff
@@ -55,14 +55,16 @@
                     self.set_scale(node, new_scale)
 
     def find_node_name(self, name):
         for node in self.model.model.graph.node:
             if node.output[0] == name:
                 return node.name
 
+        return None
+
     def get_ipos_name(self, node, input_id=None):
         if len(node.input) > 0:
             i_name = node.input[0]
             return self.find_node_name(i_name)
         else:
             return None
 
@@ -276,22 +278,22 @@
         """Adjust the shift bias of node.
 
         shift_read = max(ipos) - min(ipos)
 
         DPU compiler constraints of shift_bias:
         1. 0 <= shift_read <= 15
         """
-        for i, node in enumerate(self.model.model.graph.node):
+        for index, node in enumerate(self.model.model.graph.node):
             if node.op_type not in ["Add"] or node.op_type not in ["Mul"]:
                 continue
             ipos_layers = []
             iposes = []
             skip = False
 
-            for i in len(node.input):
+            for i in range(len(node.input)):
                 ipos_name = self.get_ipos_name_by_id(node, i)
                 ipos_layers.append(ipos_name)
             for i in ipos_layers:
                 ipos, _ = self.get_pos_by_name(i)
                 if ipos is None:
                     logger.info(
                         "Fail to get quantize position for layer {}, "
@@ -333,41 +335,40 @@
         """Adjust the shift write of node.
 
         shift_write = min(ipos) - opos
 
         DPU compiler constraints of shift_write:
         1. -15 <= shift_write <= 15
         """
-        for i, node in enumerate(self.model.model.graph.node):
+        for node in self.model.model.graph.node:
             if node.op_type not in ["Add"] or node.op_type not in ["Mul"]:
                 continue
             ipos_layers = []
             iposes = []
             skip = False
 
-            for i in len(node.input):
-                ipos_name = self.get_ipos_name_by_id(node, i)
+            for input_id in range(len(node.input)):
+                ipos_name = self.get_ipos_name_by_id(node, input_id)
                 ipos_layers.append(ipos_name)
-            for i in ipos_layers:
-                ipos, _ = self.get_pos_by_name(i)
+            for layer_id in ipos_layers:
+                ipos, _ = self.get_pos_by_name(layer_id)
                 if ipos is None:
                     logger.info(
                         "Fail to get quantize position for layer {}(input:{}) (output of layer {}), "
-                        "skip adjust_shift_read for it.".format(ipos_layers[i], i, ipos_layers[i])
+                        "skip adjust_shift_read for it.".format(ipos_layers[layer_id], layer_id, ipos_layers[layer_id])
                     )
                     skip = True
                 iposes.append(ipos)
             opos_name = self.get_opos_name(node)
             opos, _ = self.get_pos_by_name(opos_name)
             if opos is None:
                 logger.info(
                     "Fail to get quantize position for layer {}(output:0), "
                     "skip adjust_shift_write for it.".format(node.name)
                 )
-            skip = True
             if skip:
                 continue
 
             id_min = np.argmin(iposes)
             sw = iposes[id_min] - opos
             min_sw, max_sw = -15, 15
 
@@ -392,25 +393,25 @@
                         int(opos),
                         int(new_opos),
                     )
                 )
 
     def align_concat(self):
         """Align concat op's inputs and output pos."""
-        for i, node in enumerate(self.model.model.graph.node):
+        for node in self.model.model.graph.node:
             if node.op_type not in ["Concat"]:
                 continue
             input_node_num = len(node.input)
             opos_name = self.get_opos_name(node)
             opos, _ = self.get_pos_by_name(opos_name)
             min_pos = opos
             ipos_layers = []
 
-            for i in range(input_node_num):
-                ipos_name = self.get_ipos_name_by_id(node, i)
+            for input_id in range(input_node_num):
+                ipos_name = self.get_ipos_name_by_id(node, input_id)
                 ipos_layers.append(ipos_name)
             for name in ipos_layers:
                 ipos, _ = self.get_pos_by_name(name)
                 if ipos is not None:
                     min_pos = min(ipos, min_pos)
             if opos != min_pos:
                 self.set_pos(self.get_node_by_name(self.find_o_name(node.output[0])), min_pos)
```

## olive/passes/openvino/quantization.py

```diff
@@ -171,14 +171,15 @@
 
     def _get_nncf_dataset(self, config, data_root):
         try:
             import nncf
         except ImportError:
             raise ImportError("Please install olive-ai[openvino] to use OpenVINO pass") from None
 
+        data_loader = None
         if config["dataloader_func"]:
             data_dir = get_local_path_from_root(data_root, config["data_dir"])
             data_loader = self._user_module_loader.call_object(
                 config["dataloader_func"], data_dir, config["batch_size"], **(config["dataloader_func_kwargs"] or {})
             )
         elif config["data_config"]:
             data_config = validate_config(config["data_config"], DataConfig)
```

## olive/passes/pytorch/gptq.py

```diff
@@ -122,15 +122,15 @@
     def _run_for_config(
         self, model: PyTorchModelHandler, data_root: str, config: Dict[str, Any], output_model_path: str
     ) -> PyTorchModelHandler:
         from auto_gptq import BaseQuantizeConfig
         from auto_gptq.modeling import BaseGPTQForCausalLM
         from auto_gptq.modeling.auto import GPTQ_CAUSAL_LM_MODEL_MAP
 
-        from olive.passes.pytorch.gptq_utils import QuantLinearORT
+        from olive.passes.pytorch.quant_utils import QuantLinear
 
         if not torch.cuda.is_available():
             raise ValueError("Please use GPU to run gptq quantization.")
         elif self.host_device != Device.GPU:
             logger.warning(
                 "GPTQ quantization requires GPU but the host device is %s, will ignore the host device",
                 self.host_device,
@@ -166,15 +166,15 @@
             static_groups=config["static_groups"],
             true_sequential=config["true_sequential"],
             desc_act=config["desc_act"],
             sym=config["sym"],
         )
 
         def get_onnx_quant_linear(*args, **kwargs):
-            return QuantLinearORT
+            return QuantLinear
 
         if hasattr(pytorch_model, "config") and pytorch_model.config.model_type in GPTQ_CAUSAL_LM_MODEL_MAP:
             model_type = pytorch_model.config.model_type
             model_class = GPTQ_CAUSAL_LM_MODEL_MAP[model_type]
             quantized_model = model_class(pytorch_model, False, quantize_config)
         else:
             quantized_model = BaseGPTQForCausalLM(pytorch_model, False, quantize_config)
@@ -187,15 +187,15 @@
             quantized_model.outside_layer_modules = config["outside_layer_modules"]
             quantized_model.inside_layer_modules = config["inside_layer_modules"]
 
         import auto_gptq
 
         original = auto_gptq.modeling._utils.dynamically_import_QuantLinear  # pylint: disable=protected-access
         try:
-            # Replace QuantLinear in autogptq with QuantLinearORT for quant linear layer packing
+            # Replace QuantLinear in autogptq with QuantLinear for quant linear layer packing
             auto_gptq.modeling._utils.dynamically_import_QuantLinear = (  # pylint: disable=protected-access
                 get_onnx_quant_linear
             )
 
             # Autogpq quantize_model currently only support cuda device. It accepts model on cpu but
             # will move each block(layer) to cuda before quantization and move back to cpu when finished.
             quantized_model.quantize(dataset)
```

## olive/passes/pytorch/lora.py

```diff
@@ -20,15 +20,15 @@
 import torch
 import transformers
 from packaging import version
 from transformers import AutoTokenizer
 
 from olive.common.config_utils import ConfigBase, ConfigWithExtraArgs
 from olive.common.pydantic_v1 import Field, validator
-from olive.common.utils import find_submodules
+from olive.common.utils import find_submodules, resolve_torch_dtype
 from olive.data.config import DataConfig
 from olive.data.constants import IGNORE_INDEX
 from olive.hardware.accelerator import AcceleratorSpec
 from olive.model import PyTorchModelHandler
 from olive.model.config.hf_config import HfFromPretrainedArgs
 from olive.model.utils.hf_utils import get_peft_task_type_from_task
 from olive.passes import Pass
@@ -644,33 +644,52 @@
 
             trainer_cls = transformers.Trainer
             if config.use_ort_trainer:
                 from optimum.onnxruntime import ORTTrainer
 
                 trainer_cls = ORTTrainer
 
-            # get trainer
-            trainer = trainer_cls(
-                model=model,
-                tokenizer=tokenizer,
-                args=config.training_args.create_training_args(config.use_ort_trainer),
-                train_dataset=train_dataset,
-                eval_dataset=eval_dataset,
-                data_collator=partial(self.collate_batch, tokenizer=tokenizer),
-            )
-            # TODO(jambayk): trainer callback for saving might be needed for DDP training
-            # worry about this later
+            # there is a bug in accelerate where it assumes 4bit models on multiple gpus cannot be trained but it is
+            # not the case. refer to https://github.com/huggingface/accelerate/pull/2714 for more details
+            # we will force the accelerator to use the first device using the ACCELERATE_TORCH_DEVICE env variable
+            # only catches the bug on aml compute with multiple gpus where the model has no weights on device 0 for
+            # some reason
+            # TODO(jambayk): add a version check when the fix is released
+            accelerate_torch_device = os.environ.get("ACCELERATE_TORCH_DEVICE", None)
+            try:
+                # using a try finally block in case the environment variable is used elsewhere
+                first_device = next(iter(set(model.hf_device_map.values())))
+                first_device_index = first_device.index if isinstance(first_device, torch.device) else first_device
+                os.environ["ACCELERATE_TORCH_DEVICE"] = f"cuda:{first_device_index}"
+                logger.debug("ACCELERATE_TORCH_DEVICE set to: %s", os.environ["ACCELERATE_TORCH_DEVICE"])
+
+                # get trainer'
+                trainer = trainer_cls(
+                    model=model,
+                    tokenizer=tokenizer,
+                    args=config.training_args.create_training_args(config.use_ort_trainer),
+                    train_dataset=train_dataset,
+                    eval_dataset=eval_dataset,
+                    data_collator=partial(self.collate_batch, tokenizer=tokenizer),
+                )
+                # TODO(jambayk): trainer callback for saving might be needed for DDP training
+                # worry about this later
 
-            # train
-            logger.info("Running fine-tuning")
-            train_result = trainer.train(resume_from_checkpoint=checkpoint)
-            logger.debug("train_result: %s", train_result)
+                # train
+                logger.info("Running fine-tuning")
+                train_result = trainer.train(resume_from_checkpoint=checkpoint)
+                logger.debug("train_result: %s", train_result)
+            finally:
+                if accelerate_torch_device is not None:
+                    os.environ["ACCELERATE_TORCH_DEVICE"] = accelerate_torch_device
+                else:
+                    os.environ.pop("ACCELERATE_TORCH_DEVICE", None)
 
         if torch.cuda.is_available():
-            torch.backends.cuda.matmul.allow_tf32 = allow_tf32
+            torch.backends.cuda.matmul.allow_tf32 = allow_tf32  # lgtm
 
         # save adapter weights
         adapter_path = Path(output_model_path) / "adapter"
         adapter_path.mkdir(parents=True, exist_ok=True)
         # don't save embedding layers since only adapter weights are trained
         # if we don't provide as False, it defaults to "auto" which checks if the vocab size changed
         model.save_pretrained(adapter_path, save_embedding_layers=False)
@@ -717,23 +736,17 @@
             # set the new embeddings to the average
             input_embeddings_data[-num_new_tokens:] = input_embeddings_avg
             output_embeddings_data[-num_new_tokens:] = output_embeddings_avg
 
     @staticmethod
     def get_torch_dtype(torch_dtype: str) -> torch.dtype:
         """Get the torch dtype from the string."""
-        supported_dtypes = {
-            "bfloat16": torch.bfloat16,
-            "float16": torch.float16,
-            "float32": torch.float32,
-        }
-        assert (
-            torch_dtype in supported_dtypes
-        ), f"torch_dtype must be one of {list(supported_dtypes.keys())} but got {torch_dtype}"
-        return supported_dtypes[torch_dtype]
+        supported_dtypes = ("bfloat16", "float16", "float32")
+        assert torch_dtype in supported_dtypes, f"torch_dtype must be one of {supported_dtypes} but got {torch_dtype}"
+        return resolve_torch_dtype(torch_dtype)
 
     @classmethod
     def input_model_check(cls, model: PyTorchModelHandler) -> PyTorchModelHandler:
         """Validate the input model and reset from_pretrained_args and adapter_path."""
         if not model.hf_config:
             raise ValueError(f"{cls.__name__} pass only supports PyTorchModelHandler with hf_config.")
```

## olive/passes/pytorch/slicegpt.py

```diff
@@ -5,15 +5,17 @@
 # -------------------------------------------------------------------------
 import json
 import logging
 import sys
 from typing import Any, Dict, Union
 
 import torch
+from torch.utils.data import DataLoader, SubsetRandomSampler
 
+from olive.common.config_utils import validate_config
 from olive.constants import ModelFileFormat
 from olive.data.config import DataConfig
 from olive.hardware.accelerator import AcceleratorSpec
 from olive.model import PyTorchModelHandler
 from olive.model.utils.path_utils import normalize_path_suffix
 from olive.passes import Pass
 from olive.passes.olive_pass import PassConfigParam
@@ -45,26 +47,14 @@
             ),
             "calibration_batch_size": PassConfigParam(
                 type_=int,
                 required=False,
                 default_value=16,
                 description=("Batch size for loading the calibration data."),
             ),
-            "calibration_max_seqlen": PassConfigParam(
-                type_=int,
-                required=False,
-                default_value=2048,
-                description=("Maximum sequence length for the calibration data."),
-            ),
-            "varied_seqlen": PassConfigParam(
-                type_=bool,
-                required=False,
-                default_value=False,
-                description=("Varied sequence lengths in the calibration data."),
-            ),
             "seed": PassConfigParam(
                 type_=int,
                 required=False,
                 default_value=42,
                 description=("Seed for sampling the calibration data."),
             ),
             "sparsity": PassConfigParam(
@@ -88,30 +78,29 @@
     def _run_for_config(
         self, model: PyTorchModelHandler, data_root: str, config: Dict[str, Any], output_model_path: str
     ) -> PyTorchModelHandler:
         if sys.version_info < (3, 10):
             raise ValueError("SliceGPT requires python3.10 or higher")
 
         from slicegpt import layernorm_fusion, rotate
-        from slicegpt.data_utils import get_dataset, prepare_dataloader
         from slicegpt.hf_utils import get_model_and_tokenizer
         from slicegpt.slicing_scheduler import ConstSlicingScheduler
 
         # Renaming variables to match their contextual use
         model_handler = model
         model = None
 
         # convert config to pass config class
         # this will validate the config and convert to the correct types
         config = self._config_class(**config)
 
         if model_handler.hf_config is None or model_handler.hf_config.model_name is None:
             raise ValueError("SliceGPT only supports select HuggingFace models")
 
-        model_adapter, tokenizer = get_model_and_tokenizer(model_handler.hf_config.model_name)
+        model_adapter, _ = get_model_and_tokenizer(model_handler.hf_config.model_name)
         model_handler.model = model_adapter.model
         model = model_handler.load_model()
 
         # replace and fuse layers
         layernorm_fusion.replace_layers(model_adapter)
         layernorm_fusion.fuse_modules(model_adapter)
 
@@ -124,24 +113,28 @@
         new_embedding_dim -= new_embedding_dim % config.round_interval
         logger.info(
             "New embedding dimension: %f (sparsity %.4f%%)",
             new_embedding_dim,
             100 * (1 - new_embedding_dim / model_adapter.hidden_size),
         )
 
-        train_dataset = get_dataset(config.calibration_data_config.name)["train"]
-        train_loader = prepare_dataloader(
-            dataset=train_dataset,
-            tokenizer=tokenizer,
-            max_seqlen=config.calibration_max_seqlen,
-            batch_size=config.calibration_batch_size,
-            nsamples=config.calibration_nsamples,
-            varied_seqlen=config.varied_seqlen,
-            seed=config.seed,
-        )
+        data_config = validate_config(config.calibration_data_config, DataConfig)
+        dataloader = data_config.to_data_container().create_dataloader(data_root)
+        dataset = [
+            {
+                "input_ids": data[0]["input_ids"].squeeze(),
+                "attention_mask": data[0]["attention_mask"].squeeze(),
+                "labels": data[1].squeeze(),
+            }
+            for data in dataloader
+        ]
+
+        torch.manual_seed(config.seed)
+        sampler = SubsetRandomSampler(torch.randperm(len(dataset))[: config.calibration_nsamples])
+        train_loader = DataLoader(dataset, batch_size=config.calibration_batch_size, sampler=sampler)
 
         # rotate and slice
         schedular = ConstSlicingScheduler(new_embedding_dim)
         rotate.rotate_and_slice(model_adapter, train_loader, schedular, final_orientation=config.final_orientation)
 
         sliced_param_count = sum(int(p.nelement()) for p in model.parameters())
         sliced_fraction = 1.0 - sliced_param_count / original_param_count
```

## olive/passes/qnn/conversion.py

```diff
@@ -30,19 +30,19 @@
             # The `input_network` will be set in the runtime.
             "input_dim": PassConfigParam(
                 type_=List[str],
                 required=False,
                 description=(
                     "The names and dimensions of the network input layers specified in the format"
                     " [input_name comma-separated-dimensions], for example:"
-                    "        [\"'data' 1,224,224,3\"]"
+                    '        ["data 1,224,224,3"]'
                     " Note that the quotes should always be included in order to"
                     " handle special characters, spaces, etc."
                     " For multiple inputs specify multiple --input_dim on the command line like:"
-                    "        [\"'data' 1,224,224,3\", \"'data2' 1,224,224,3\"]"
+                    '        ["data 1,224,224,3", "data2 1,224,224,3"]'
                     " If --input_dim is not specified, the input dimensions will be inferred from the model."
                     " If --input_dim is specified, the input dimensions will be used as-is."
                 ),
             ),
             "out_node": PassConfigParam(
                 type_=List[str],
                 required=False,
@@ -75,42 +75,50 @@
         elif isinstance(model, PyTorchModelHandler):
             converter_platform = "pytorch"
         elif isinstance(model, ONNXModelHandler):
             converter_platform = "onnx"
         else:
             # TODO(trajep): add tflite support
             raise NotImplementedError(f"Unsupported model handler type: {type(model)}")
-        converter_program = f"qnn-{converter_platform}-converter"
+        converter_program = [f"qnn-{converter_platform}-converter"]
 
         runner = QNNSDKRunner(use_dev_tools=True)
         if platform.system() == "Windows":
-            converter_program = "python " + str(
-                Path(runner.sdk_env.sdk_root_path) / "bin" / runner.sdk_env.target_arch / converter_program
-            )
+            converter_program = [
+                "python",
+                str(Path(runner.sdk_env.sdk_root_path) / "bin" / runner.sdk_env.target_arch / converter_program[0]),
+            ]
 
         # get input dim from io_config
         input_dims = None
         if config.get("input_dim"):
-            input_dims = config["input_dim"]
+            input_dims = map(str.split, config["input_dim"])
         elif model.io_config:
-            input_dims_tuple = zip(model.io_config.input_names, model.io_config.input_shapes)
-            # '{name}' is required to wrap the input name
-            input_dims = [f"'{name}' {','.joint(shape)}" for name, shape in input_dims_tuple]
+            input_dims_tuple = zip(model.io_config["input_names"], model.io_config["input_shapes"])
+            input_dims = [[name, ",".join(map(str, shape))] for name, shape in input_dims_tuple]
 
         out_nodes = None
         if config.get("out_node"):
             out_nodes = config["out_node"]
         elif model.io_config:
-            out_nodes = model.io_config.output_names
+            out_nodes = model.io_config["output_names"]
 
         output_model_path = normalize_path_suffix(output_model_path, "model.cpp")
-
+        # TODO(anyone): unify other cmd to list to avoid shlex.split error in non-posix mode
         cmd_list = [
-            converter_program,
-            f"--input_network {model.model_path}",
-            f"--output_path {output_model_path}",
-            " ".join([f"--input_dim {i}" for i in input_dims]) if input_dims else "",
-            " ".join([f"--out_node {o}" for o in out_nodes]) if out_nodes else "",
-            config["extra_args"] or "",
+            *converter_program,
+            "--input_network",
+            model.model_path,
+            "--output_path",
+            output_model_path,
         ]
-        runner.run(" ".join(cmd_list))
+        if input_dims:
+            for i in input_dims:
+                cmd_list.extend(["--input_dim", *i])
+        if out_nodes:
+            for o in out_nodes:
+                cmd_list.extend(["--out_node", o])
+        if config["extra_args"]:
+            cmd_list.extend(config["extra_args"].split())
+
+        runner.run(cmd_list)
         return QNNModelHandler(output_model_path, model_file_format=ModelFileFormat.QNN_CPP)
```

## olive/platform_sdk/qualcomm/runner.py

```diff
@@ -4,14 +4,15 @@
 # --------------------------------------------------------------------------
 import logging
 import os
 import shlex
 import shutil
 import time
 from pathlib import Path
+from typing import List, Union
 
 from olive.common.utils import run_subprocess
 from olive.platform_sdk.qualcomm.qnn.env import QNNSDKEnv
 from olive.platform_sdk.qualcomm.snpe.env import SNPESDKEnv
 
 logger = logging.getLogger(__name__)
 
@@ -39,40 +40,45 @@
             self.sdk_env = SNPESDKEnv(use_dev_tools=self.use_dev_tools)
         elif self.platform == "QNN":
             self.sdk_env = QNNSDKEnv(use_dev_tools=self.use_dev_tools)
 
     def _use_olive_env(self):
         return os.environ.get(USE_OLIVE_ENV, USE_OLIVE_ENV_DEFAULT_VALUE) == USE_OLIVE_ENV_DEFAULT_VALUE
 
-    def _resolve_cmd(self, cmd: str):
+    def _resolve_cmd(self, cmd: Union[str, List[str]]) -> List[str]:
+        # TODO(trajep): use list instead of string to avoid shlex.split error in non-posix mode
         import platform
 
-        if platform.system() == "Windows" and cmd.startswith(("snpe-", "qnn-")):
-            logger.debug("Resolving command %s on Windows.", cmd)
+        if isinstance(cmd, str):
+            cmd_list = shlex.split(cmd, posix=(platform.system() != "Windows"))
+        else:
+            cmd_list = cmd
+
+        if platform.system() == "Windows" and cmd_list[0].startswith(("snpe-", "qnn-")):
+            logger.debug("Resolving command %s on Windows.", cmd_list)
             cmd_dir = Path(self.sdk_env.sdk_root_path) / "bin" / self.sdk_env.target_arch
-            cmd_name = cmd.split(" ")[0]
+            cmd_name = cmd_list[0]
             cmd_full_path = cmd_dir / cmd_name
             if cmd_full_path.with_suffix(".exe").exists():
                 cmd_full_path = cmd_full_path.with_suffix(".exe")
             if cmd_full_path.exists():
-                cmd = str(cmd_full_path) + cmd[len(cmd_name) :]
+                cmd_list[0] = str(cmd_full_path)
                 try:
                     with cmd_full_path.open() as f:
                         first_line = f.readline()
                         if "python" in first_line:
-                            cmd = f"python {cmd}"
+                            cmd_list.insert(0, "python")
                 except UnicodeDecodeError as e:
                     logger.warning(
                         "Failed to read the first line of %s: %s. Will ignore to wrap it with python.", cmd_name, e
                     )
-        if isinstance(cmd, str):
-            cmd = shlex.split(cmd, posix=(platform.system() != "Windows"))
-            path_env = self.sdk_env.env.get("PATH") if self._use_olive_env() else None
-            cmd[0] = shutil.which(cmd[0], path=path_env) or cmd[0]
-        return cmd
+
+        path_env = self.sdk_env.env.get("PATH") if self._use_olive_env() else None
+        cmd_list[0] = shutil.which(cmd_list[0], path=path_env) or cmd_list[0]
+        return cmd_list
 
     def run(self, cmd: str):
         env = self.sdk_env.env if self._use_olive_env() else None
         cmd = self._resolve_cmd(cmd)
 
         for run in range(self.runs):
             run_log_msg = "" if self.runs == 1 else f" (run {run + 1}/{self.runs})"
```

## olive/platform_sdk/qualcomm/qnn/env.py

```diff
@@ -23,15 +23,15 @@
         python_env_bin_path = str(Path(f"{sdk_root_path}/olive-pyenv/{python_env_parent_folder}"))
 
         env["PATH"] += delimiter + os.environ["PATH"]
         if self.use_dev_tools:
             if not Path(python_env_bin_path).exists():
                 raise FileNotFoundError(
                     f"Path {python_env_bin_path} does not exist. Please run"
-                    " 'python -m olive.platform_sdk.qualcomm.configure --py_version 3.8 --sdk qnn'"
+                    " 'olive configure-qualcomm-sdk --py_version 3.8 --sdk qnn'"
                     " to add the missing file."
                 )
             env["PATH"] = python_env_bin_path + delimiter + env["PATH"]
         if platform.system() == "Windows":
             for k, v in os.environ.items():
                 if k not in env:
                     env[k] = v
```

## olive/platform_sdk/qualcomm/snpe/env.py

```diff
@@ -25,27 +25,27 @@
         python_env_bin_path = str(Path(f"{sdk_root_path}/olive-pyenv/{python_env_parent_folder}"))
 
         env["PATH"] += delimiter + os.environ["PATH"]
         if self.use_dev_tools:
             if not Path(python_env_bin_path).exists():
                 raise FileNotFoundError(
                     f"Path {python_env_bin_path} does not exist. Please run"
-                    " 'python -m olive.platform_sdk.qualcomm.configure --py_version 3.8 --sdk snpe'"
+                    " 'olive configure-qualcomm-sdk --py_version 3.8 --sdk snpe'"
                     " to add the missing file."
                 )
 
             env["PATH"] = python_env_bin_path + delimiter + env["PATH"]
 
         if platform.system() == "Windows":
             os_env = os.environ.copy()
             os_env.update(env)
             env = os_env
             if target_arch == SDKTargetDevice.arm64x_windows:
                 bin_path = str(Path(f"{sdk_root_path}/olive-arm-win"))
                 if not Path(bin_path).exists():
                     raise FileNotFoundError(
                         f"Path {bin_path} does not exist. Please run"
-                        " 'python -m olive.platform_sdk.qualcomm.configure --py_version 3.8 --sdk snpe' to add the"
+                        " 'olive configure-qualcomm-sdk --py_version 3.8 --sdk snpe' to add the"
                         " missing folder"
                     )
 
         return env
```

## olive/platform_sdk/qualcomm/snpe/tools/inference.py

```diff
@@ -209,14 +209,15 @@
     elif accumulate_outputs:
         logger.warning("accumulate_outputs is set to True, but no workspace is provided. Ignoring accumulate_outputs.")
 
     # input ids for each sample in the input list
     input_ids = get_input_ids(input_list)
 
     # get the delimiter for the output files
+    delimiter = None
     if platform.system() == "Linux":
         delimiter = ":"
     elif platform.system() == "Windows":
         delimiter = "_"
 
     # dictionary to store the results as numpy arrays
     results = {}
@@ -410,14 +411,15 @@
     android_persist_ws: Whether to persist the workspace on android.
     android_initialized: Whether the inference session has already been initialized on android using
         init_snpe_net_adb.
     """
     cmd = f"snpe-throughput-net-run --container {dlc_path} --duration {duration} --use_{device}"
 
     input_raw = ""
+    first = ""
     with Path(input_list).open() as f:
         for line in f:
             if line.startswith(("#", "%")):
                 continue
             else:
                 first = line.strip()
                 break
```

## olive/platform_sdk/qualcomm/utils/__init__.py

```diff
@@ -1,7 +1,4 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
-
-from olive.platform_sdk.qualcomm.constants import *  # noqa: F403
-from olive.platform_sdk.qualcomm.env import *  # noqa: F403
```

## olive/platform_sdk/qualcomm/utils/data_loader.py

```diff
@@ -1,57 +1,62 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 import logging
 import shutil
 import tempfile
-from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import Any, Tuple
+from typing import Any
 
 import numpy as np
 import torch
 
 from olive.platform_sdk.qualcomm.utils import input_list as input_list_utils
 
 logger = logging.getLogger(__name__)
 
 
-class FileListDataLoader(ABC):
-    """Abstraction for logical "FileListDataLoader", it contains data path and related metadata."""
+class FileListDataLoader:
+    """Data loader for use with Qualcomm SDKs that loads data from a file list."""
 
-    def __init__(self, config: dict, batch_size: int = None):
+    def __init__(self, data_dir: str, input_list: str, annotation: np.ndarray = None, batch_size: int = None):
         # TODO(anyone): try to add file_chunk_size to distinguish the concept of batch_size and file_chunk_size
-        """:param config: data loader specific config."""
-        self.config = config
+        """Initialize FileListDataLoader.
+
+        :param data_dir: directory containing data.
+        :param input_list: path to input list file. The paths in the input list file must be absolute paths.
+        :param annotation: annotations for the data. Numpy array with shape (num_samples, ...).
+        :param batch_size: number of inputs per chunked input list file for batch processing. If None, all inputs are
+            loaded as a single chunk.
+        """
+        self.data_dir = data_dir
+        self.input_list = input_list
+        self.annotation = annotation
         self.batch_size = batch_size
-        self.tmp_dir = None
-        self.data_dir, self.input_list, self.annotation = self.load_data()
         self.prepare_batches()
 
-    @abstractmethod
-    def load_data(self) -> Tuple[str, str, Any]:
-        """Return path to data directory, input list file and loaded annotation.
+    def prepare_batches(self):
+        """Prepare batches by splitting input list into chunks of batch_size.
 
-        Derived class should override this method
+        Data won't be copied to batch directory until get_batch is called.
         """
-        raise NotImplementedError
-
-    def prepare_batches(self):
         if self.batch_size is None:
             self.num_batches = 1
             return
 
-        if self.tmp_dir is None:
-            self.tmp_dir = tempfile.TemporaryDirectory(prefix="olive_tmp_")  # pylint: disable=consider-using-with
-        self.batch_dir = str(Path(self.tmp_dir.name) / "batch")
+        # create temporary directory for batch processing
+        self.batch_tmp_dir = tempfile.TemporaryDirectory("olive_tmp_")  # pylint: disable=consider-using-with
+        # directory to save batch data
+        self.batch_dir = Path(self.batch_tmp_dir.name) / "batch"
 
+        # create batch input list replacing self.data_dir with self.batch_dir
+        # batch data will be moved to self.batch_dir when get_batch is called
         batch_input_list = input_list_utils.resolve_input_list(
-            self.batch_dir, self.input_list, self.tmp_dir.name, self.data_dir, "batch_input_list.txt"
+            self.batch_dir, self.input_list, self.batch_tmp_dir.name, self.data_dir, "batch_input_list.txt"
         )
 
         self.batch_input_list_headers = []
         self.batch_input_list_contents = []
         with open(self.input_list) as f, open(batch_input_list) as f_batch:
             for line, line_batch in zip(f, f_batch):
                 if line.startswith(("#", "%")):
@@ -84,168 +89,181 @@
             annotation = None
             if self.annotation is not None:
                 annotation = self.annotation[
                     self.batch_size * batch_id : self.batch_size * (batch_id + 1)  # noqa: E203, RUF100
                 ]
             batch = self.batches[batch_id]
 
+            # empty batch directory and copy current batch data
             shutil.rmtree(self.batch_dir, ignore_errors=True)
             for _, to_copy in batch:
                 for input_str, input_batch in to_copy:
                     Path(input_batch).parent.mkdir(parents=True, exist_ok=True)
                     # Path(input_batch).symlink_to(input)
                     shutil.copy(input_str, input_batch)
 
+            # create input list for the batch
             batch_input_list = Path(self.batch_dir) / "input_list.txt"
             with batch_input_list.open("w") as f:
                 for header in self.batch_input_list_headers:
                     f.write(f"{header}\n")
                 for line_batch, _ in batch:
                     f.write(f"{line_batch}\n")
 
             return self.batch_dir, str(batch_input_list), annotation
 
     def __len__(self):
         return self.num_batches
 
     def __iter__(self):
-        # pylint: disable=attribute-defined-outside-init
-        self.n = 0
-        return self
-
-    def __next__(self):
-        if self.n < self.num_batches:
-            batch = self.get_batch(self.n)
-            self.n += 1
-            return batch
-        else:
-            raise StopIteration
+        for batch_idx in range(self.num_batches):
+            yield self.get_batch(batch_idx)
 
     def get_data_dir(self):
         return self.data_dir
 
     def get_input_list(self):
         return self.input_list
 
 
 class FileListProcessedDataLoader(FileListDataLoader):
+    """FileList dataloader created from directory with processed data."""
+
     def __init__(
         self,
         data_dir: str,
         input_list_file: str = "input_list.txt",
+        relative_input_paths: bool = False,
         annotations_file: str = None,
         batch_size: int = None,
     ):
-        config = {"data_dir": data_dir, "input_list_file": input_list_file, "annotations_file": annotations_file}
-        super().__init__(config, batch_size)
+        """Initialize FileListProcessedDataLoader.
 
-    def load_data(self) -> Tuple[str, str, np.ndarray]:
-        self.tmp_dir = tempfile.TemporaryDirectory(prefix="olive_tmp_")  # pylint: disable=consider-using-with
-        input_list = input_list_utils.get_input_list(
-            self.config["data_dir"], self.config["input_list_file"], self.tmp_dir.name
+        :param data_dir: directory containing processed data.
+        :param input_list_file: file containing input list. Expected to be a file in the data directory if not an
+            absolute path.
+        :param relative_input_paths: whether input paths in the input list file are relative to the data directory.
+        :param annotations_file: npy file containing annotations. Expected to be a file in the data directory if not
+            an absolute path. If None, no annotations are loaded.
+        :param batch_size: number of inputs per chunked input list file for batch processing. If None, all inputs are
+            loaded as a single chunk.
+        """
+        data_dir = Path(data_dir).resolve()
+
+        # change input paths in input list file to absolute paths
+        input_list_temp_dir = tempfile.TemporaryDirectory("olive_tmp_")  # pylint: disable=consider-using-with
+        input_list = input_list_utils.resolve_input_list(
+            data_dir,
+            data_dir / input_list_file,
+            input_list_temp_dir.name,
+            input_path_parent=None if relative_input_paths else data_dir,
         )
 
         annotations = None
-        if self.config["annotations_file"] is not None:
-            annotations_path = Path(self.config["data_dir"]) / self.config["annotations_file"]
+        if annotations_file is not None:
+            annotations_path = Path(data_dir) / annotations_file
             if not annotations_path.is_file():
-                raise FileNotFoundError(
-                    f"{self.config['annotations_file']} not found in data directory {self.config['data_dir']}"
-                )
+                raise FileNotFoundError(f"{annotations_file} not found in data directory {data_dir}")
             if annotations_path.suffix == ".npy":
                 annotations = np.load(annotations_path)
             else:
                 raise ValueError(f"Unsupported annotations file format {annotations_path.suffix}")
 
-        return self.config["data_dir"], input_list, annotations
+        super().__init__(str(data_dir), input_list, annotations, batch_size)
+        # save a reference to the temp_data_dir so that it persists with the object
+        self.temp_data_dir = input_list_temp_dir
 
 
 class FileListRandomDataLoader(FileListDataLoader):
+    """FileList dataloader created from random data."""
+
     def __init__(
         self,
         io_config: dict,
         num_samples: int,
         data_dir: str = None,
         input_list_file: str = "input_list.txt",
         append_0: bool = False,
         batch_size: int = None,
     ):
-        config = {
-            "io_config": io_config,
-            "num_samples": num_samples,
-            "data_dir": data_dir,
-            "input_list_file": input_list_file,
-            "append_0": append_0,
-        }
-        super().__init__(config, batch_size)
+        """Initialize FileListRandomDataLoader.
 
-    def load_data(self) -> Tuple[str, str, np.ndarray]:
-        self.tmp_dir = tempfile.TemporaryDirectory(prefix="olive_tmp_")  # pylint: disable=consider-using-with
+        :param io_config: dictionary containing input and output names and shapes of the model.
+        :param num_samples: number of random samples to generate.
+        :param data_dir: directory to save random data. If None, a temporary directory is created.
+        :param input_list_file: name of the input list file to save.
+        :param append_0: whether to append ":0" to input names in the input list file. Might be relevant if the model is
+            converted from TensorFlow.
+        :param batch_size: number of inputs per chunked input list file for batch processing. If None, all inputs are in
+            a single input list file.
+        """
+        # create temporary directory for random data
+        temp_data_dir = tempfile.TemporaryDirectory("olive_tmp_")  # pylint: disable=consider-using-with
 
         # get data_dir
-        if self.config["data_dir"] is None:
-            data_dir = Path(self.tmp_dir.name).resolve() / "data"
+        if data_dir is None:
+            data_dir = Path(temp_data_dir.name).resolve() / "data"
             data_dir.mkdir(parents=True, exist_ok=True)
         else:
-            data_dir = Path(self.config["data_dir"]).resolve()
+            data_dir = Path(data_dir).resolve()
 
         # create random data
-        for input_name, input_shape in zip(
-            self.config["io_config"]["input_names"], self.config["io_config"]["input_shapes"]
-        ):
+        for input_name, input_shape in zip(io_config["input_names"], io_config["input_shapes"]):
             input_dir = data_dir / input_name
             input_dir.mkdir(parents=True, exist_ok=True)
-            raw_shape = np.product(input_shape)  # noqa: NPY003
-            name_length = len(str(self.config["num_samples"]))
-            for i in range(self.config["num_samples"]):
+            raw_shape = np.prod(input_shape)
+            name_length = len(str(num_samples))
+            for i in range(num_samples):
                 input_file = input_dir / (f"{i}".zfill(name_length) + ".raw")
                 raw_input = np.random.uniform(-1.0, 1.0, raw_shape).astype(np.float32)
                 raw_input.tofile(input_file)
 
         # create input_list
         input_list_utils.create_input_list(
             str(data_dir),
-            self.config["io_config"]["input_names"],
-            input_list_file=str((data_dir / self.config["input_list_file"]).resolve()),
-            add_input_names=len(self.config["io_config"]["input_names"]) > 1,
-            add_output_names=len(self.config["io_config"]["output_names"]) > 1,
-            output_names=self.config["io_config"]["output_names"],
-            append_0=self.config["append_0"],
+            io_config["input_names"],
+            input_list_file=str((data_dir / input_list_file).resolve()),
+            add_input_names=len(io_config["input_names"]) > 1,
+            add_output_names=len(io_config["output_names"]) > 1,
+            output_names=io_config["output_names"],
+            append_0=append_0,
         )
 
-        input_list = input_list_utils.get_input_list(data_dir, self.config["input_list_file"], self.tmp_dir.name)
+        # get input list with absolute paths
+        input_list = input_list_utils.get_input_list(data_dir, input_list_file, temp_data_dir.name)
 
-        return str(data_dir), input_list, None
+        super().__init__(data_dir, input_list, None, batch_size)
+        # save a reference to the temp_data_dir so that it persists with the object
+        self.temp_data_dir = temp_data_dir
 
 
 class FileListCommonDataLoader(FileListDataLoader):
     """FileList dataloader created from a common dataloader such as torch.data.DataLoader."""
 
     def __init__(self, dataloader: Any, io_config: dict, batch_size: int = None):
-        """Initialize FileList Dataloader.
+        """Initialize FileListCommonDataLoader.
+
+        Each batch in the common dataloader is saved as a raw input file.
 
         :param dataloader: dataloader object. Dataloader must be iterable and return a tuple of (input, target).
-        input is a dictionary of input names and input tensors.
+            input is a dictionary of input names and input tensors.
         :param io_config: dictionary containing input and output names and shapes of the model.
-        :param batch_size: batch size for the FileList dataloader. This is not the same as the batch size of the common
-        dataloader.
+        :param batch_size: number of inputs per chunked input list file for batch processing. If None, all inputs are in
+            a single input list file. This is not the same as the batch size of the common dataloader.
         """
-        config = {"dataloader": dataloader, "io_config": io_config}
-        super().__init__(config, batch_size)
+        # create temporary directory for processed data
+        temp_data_dir = tempfile.TemporaryDirectory("olive_tmp_")  # pylint: disable=consider-using-with
 
-    def load_data(self) -> Tuple[str, str, np.ndarray]:
-        logger.debug("Converting dataloader of type %s to FileList dataloader", type(self.config["dataloader"]))
+        logger.debug("Converting dataloader of type %s to FileList dataloader", type(dataloader))
         input_specs = {}
-        for input_name, input_shape in zip(
-            self.config["io_config"]["input_names"], self.config["io_config"]["input_shapes"]
-        ):
+        for input_name, input_shape in zip(io_config["input_names"], io_config["input_shapes"]):
             input_specs[input_name] = {"target_shape": input_shape}
 
         # get single data sample
-        input_data, _ = next(iter(self.config["dataloader"]))
+        input_data, _ = next(iter(dataloader))
         # source input names
         for input_name, input_spec in input_specs.items():
             if input_name in input_data:
                 source_name = input_name
             elif input_name.strip(":0") in input_data:
                 source_name = input_name.strip(":0")
             else:
@@ -284,23 +302,22 @@
                     f"Cannot find a valid permutation of the source shape {source_shape} that matches the target"
                     f" shape {target_shape}"
                 )
 
             input_spec["permutation"] = permutation
         logger.debug("Input specs: %s", input_specs)
 
-        self.tmp_dir = tempfile.TemporaryDirectory(prefix="olive_tmp_")  # pylint: disable=consider-using-with
-        data_dir = Path(self.tmp_dir.name) / "data"
+        data_dir = Path(temp_data_dir.name) / "data"
         data_dir.mkdir()  # create data dir
 
         input_order = []
         annotations = []
-        num_samples = len(self.config["dataloader"])
+        num_samples = len(dataloader)
         sample_digits = len(str(num_samples))
-        for i, (input_data_i, annotation) in enumerate(self.config["dataloader"]):
+        for i, (input_data_i, annotation) in enumerate(dataloader):
             if isinstance(input_data_i, tuple):
                 input_data = dict(zip(input_specs.keys(), input_data_i))
             elif isinstance(input_data_i, (torch.Tensor, np.ndarray)):
                 input_data = dict(zip(input_specs.keys(), [input_data_i]))
             else:
                 input_data = input_data_i
                 assert isinstance(
@@ -330,14 +347,17 @@
 
         # create input_list
         input_list_file = input_list_utils.create_input_list(
             data_dir=str(data_dir),
             input_names=list(input_specs.keys()),
             input_dirs=[input_spec["source_name"] for input_spec in input_specs.values()],
             add_input_names=len(input_specs) > 1,
-            add_output_names=len(self.config["io_config"]["output_names"]) > 1,
-            output_names=self.config["io_config"]["output_names"],
+            add_output_names=len(io_config["output_names"]) > 1,
+            output_names=io_config["output_names"],
         )
 
-        input_list = input_list_utils.get_input_list(str(data_dir), input_list_file, self.tmp_dir.name)
+        # get input list with absolute paths
+        input_list = input_list_utils.get_input_list(str(data_dir), input_list_file, temp_data_dir.name)
 
-        return str(data_dir), input_list, annotations
+        super().__init__(str(data_dir), input_list, annotations, batch_size)
+        # save a reference to the temp_data_dir so that it persists with the object
+        self.temp_data_dir = temp_data_dir
```

## olive/strategy/search_parameter.py

```diff
@@ -127,15 +127,20 @@
             assert isinstance(key, tuple), "support key must be a tuple"
             assert len(key) == len(parents), "support key length must match the number of parents"
 
         self.parents = parents
         self.support = support
         self.default = default or self.get_invalid_choice()
 
-    def get_support(self, parent_values: Dict[str, Any]) -> Union[List[str], List[int], List[float], List[bool]]:
+    def get_support(self) -> List[Any]:
+        raise NotImplementedError("Use get_support_with_args instead")
+
+    def get_support_with_args(
+        self, parent_values: Dict[str, Any]
+    ) -> Union[List[str], List[int], List[float], List[bool]]:
         """Get the support for the search parameter for a given parent value."""
         # pylint: disable=arguments-differ
         assert parent_values.keys() == set(self.parents), "parent values keys do not match the parents"
         parent_values = tuple(parent_values[parent] for parent in self.parents)
         return self.support.get(parent_values, self.default).get_support()
 
     def condition(self, parent_values: Dict[str, Any]) -> SearchParameter:
@@ -230,17 +235,17 @@
     """
 
     def __init__(self, parents: Tuple[str], support: Dict[Tuple[Any], Any], default: Any = SpecialParamValue.INVALID):
         support = {key: Categorical([value]) for key, value in support.items()}
         default = Categorical([default])
         super().__init__(parents, support, default)
 
-    def get_support(self, parent_values: Dict[str, Any]) -> Union[bool, int, float, str]:
+    def get_support_with_args(self, parent_values: Dict[str, Any]) -> Union[bool, int, float, str]:
         """Get the support for the search parameter for a given parent value."""
-        return super().get_support(parent_values)[0]
+        return super().get_support_with_args(parent_values)[0]
 
     def condition(self, parent_values: Dict[str, Any]) -> Union[bool, int, float, str, "ConditionalDefault"]:
         """Fix the parent value and return a new search parameter."""
         value = super().condition(parent_values)
         if isinstance(value, Categorical):
             return value.get_support()[0]
         if isinstance(value, Conditional):
```

## olive/strategy/search_results.py

```diff
@@ -6,15 +6,15 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Tuple
 
 import numpy as np
 
 from olive.common.utils import hash_dict
 
 if TYPE_CHECKING:
-    from olive.evaluator.metric import MetricResult
+    from olive.evaluator.metric_result import MetricResult
 
 
 class SearchResults:
     def __init__(
         self,
         objective_dict: Dict[str, dict],
         init_model_history: Dict[str, Any] = None,
```

## olive/strategy/search_space.py

```diff
@@ -42,17 +42,18 @@
         """Sample a random configuration from the search space."""
         # initialize search point
         search_point = deepcopy(self._empty_search_point)
 
         # sample from search space
         for space_name, param_name in self._iter_order:
             param = self._search_space[space_name][param_name]
+            options = []
             if isinstance(param, Conditional):
                 parent_vals = {parent: search_point[space_name][parent] for parent in param.parents}
-                options = param.get_support(parent_vals)
+                options = param.get_support_with_args(parent_vals)
             elif isinstance(param, Categorical):
                 options = param.get_support()
             search_point[space_name][param_name] = self.rng.choice(options)
             if search_point[space_name][param_name] == SpecialParamValue.INVALID:
                 return self.random_sample()
 
         return search_point
@@ -65,17 +66,20 @@
             return
 
         space_name, param_name = full_iter_order[index]
         param = self._search_space[space_name][param_name]
 
         if isinstance(param, Conditional):
             parent_vals = {parent: search_point[space_name][parent] for parent in param.parents}
-            options = param.get_support(parent_vals)
+            options = param.get_support_with_args(parent_vals)
         elif isinstance(param, Categorical):
             options = param.get_support()
+        else:
+            return
+
         for option in options:
             if option == SpecialParamValue.INVALID:
                 continue
             search_point[space_name][param_name] = option
             yield from self._iterate_util(full_iter_order, search_point, index + 1)
 
     def iterate(self) -> Iterator[Dict[str, Dict[str, Any]]]:
```

## olive/strategy/search_strategy.py

```diff
@@ -8,15 +8,15 @@
 
 from olive.common.config_utils import ConfigBase, validate_config
 from olive.common.pydantic_v1 import validator
 from olive.strategy.search_algorithm import REGISTRY, SearchAlgorithm
 from olive.strategy.search_results import SearchResults
 
 if TYPE_CHECKING:
-    from olive.evaluator.metric import MetricResult
+    from olive.evaluator.metric_result import MetricResult
     from olive.strategy.search_parameter import SearchParameter
 
 logger = logging.getLogger(__name__)
 
 _VALID_EXECUTION_ORDERS = ("joint", "pass-by-pass")
 
 # pylint: disable=attribute-defined-outside-init
@@ -137,14 +137,16 @@
         if init_model_id is None and self._active_spaces_group is None:
             raise ValueError("init_model_id must be provided for the first search group")
 
         if self._config.execution_order == "joint":
             next_sg = self._next_search_group_joint(init_model_id)
         elif self._config.execution_order == "pass-by-pass":
             next_sg = self._next_search_group_pass_by_pass(init_model_id)
+        else:
+            raise ValueError(f"Invalid execution order {self._config.execution_order}")
         return next_sg
 
     def _next_search_group_pass_by_pass(self, init_model_id: Optional[str] = None) -> Optional[SearchAlgorithm]:
         # passes are exhausted or empty for current flow, try next pass flow
         if not self._pass_by_pass_sg:
             self._pass_by_pass_sg = self._spaces_groups.pop(0)
             self._active_spaces_group = None
@@ -207,14 +209,15 @@
         search_spaces_dict = {space_name: deepcopy(self._spaces_dict[space_name]) for space_name in search_space_names}
         objectives = list(self._objective_dict.keys())
         higher_is_betters = [self._objective_dict[objective]["higher_is_better"] for objective in objectives]
         if self._config.search_algorithm in REGISTRY:
             searcher = REGISTRY[self._config.search_algorithm](
                 search_spaces_dict, objectives, higher_is_betters, self._config.search_algorithm_config
             )
+            searcher.initialize()
         else:
             raise ValueError(f"Unknown search algorithm: {self._config.search_algorithm}")
         return searcher
 
     def next_step(self) -> Optional[Dict[str, Any]]:
         """Get the next step in the search."""
         if not self._initialized:
```

## olive/strategy/search_algorithm/__init__.py

```diff
@@ -5,8 +5,8 @@
 from olive.strategy.search_algorithm.exhaustive import ExhaustiveSearchAlgorithm
 from olive.strategy.search_algorithm.random_sampler import RandomSearchAlgorithm
 from olive.strategy.search_algorithm.search_algorithm import SearchAlgorithm
 from olive.strategy.search_algorithm.tpe_sampler import TPESearchAlgorithm
 
 REGISTRY = SearchAlgorithm.registry
 
-__all__ = ["SearchAlgorithm", "ExhaustiveSearchAlgorithm", "RandomSearchAlgorithm", "TPESearchAlgorithm"]
+__all__ = ["SearchAlgorithm", "ExhaustiveSearchAlgorithm", "RandomSearchAlgorithm", "TPESearchAlgorithm", "REGISTRY"]
```

## olive/strategy/search_algorithm/exhaustive.py

```diff
@@ -14,14 +14,15 @@
 
     @classmethod
     def _default_config(cls):
         return {}
 
     def initialize(self):
         """Initialize the searcher."""
+        # pylint: disable=attribute-defined-outside-init
         self._iterator = self._search_space.iterate()
 
     def suggest(self) -> Dict[str, Dict[str, Any]]:
         """Suggest a new configuration to try."""
         try:
             return next(self._iterator)
         except StopIteration:
```

## olive/strategy/search_algorithm/optuna_sampler.py

```diff
@@ -9,15 +9,15 @@
 
 from olive.common.config_utils import ConfigParam
 from olive.common.utils import hash_dict
 from olive.strategy.search_algorithm.search_algorithm import SearchAlgorithm
 from olive.strategy.search_parameter import Categorical, Conditional, SpecialParamValue
 
 if TYPE_CHECKING:
-    from olive.evaluator.metric import MetricResult
+    from olive.evaluator.metric_result import MetricResult
 
 
 optuna.logging.set_verbosity(optuna.logging.WARNING)
 
 
 class OptunaSearchAlgorithm(SearchAlgorithm):
     """Optuna sampler for search algorithms."""
@@ -28,25 +28,26 @@
     def _default_config(cls) -> Dict[str, ConfigParam]:
         return {
             "num_samples": ConfigParam(type_=int, default_value=1, description="Number of samples to suggest."),
             "seed": ConfigParam(type_=int, default_value=1, description="Seed for the rng."),
         }
 
     def initialize(self):
+        # pylint: disable=attribute-defined-outside-init
         """Initialize the searcher."""
         self._sampler = self._create_sampler()
         directions = ["maximize" if higher_is_better else "minimize" for higher_is_better in self._higher_is_betters]
         self._study = optuna.create_study(directions=directions, sampler=self._sampler)
         self._trial_ids = {}
         self._num_samples_suggested = 0
 
     def should_stop(self):
         return (
             (self._search_space.empty() and self._num_samples_suggested > 0)
-            or (self._num_samples_suggested >= self._config.num_samples)
+            or (self._num_samples_suggested >= self.config.num_samples)
             or super().should_stop()
         )
 
     @abstractmethod
     def _create_sampler(self) -> optuna.samplers.BaseSampler:
         """Create the sampler."""
 
@@ -77,15 +78,15 @@
             if space_name not in search_point:
                 search_point[space_name] = {}
             suggestion_name = f"{space_name}___{param_name}"
             if isinstance(param, Categorical):
                 search_point[space_name][param_name] = trial.suggest_categorical(suggestion_name, param.get_support())
             elif isinstance(param, Conditional):
                 parent_vals = {parent: search_point[space_name][parent] for parent in param.parents}
-                options = param.get_support(parent_vals)
+                options = param.get_support_with_args(parent_vals)
                 parent_vals_name = "_".join([f"{v}" for _, v in parent_vals.items()])
                 suggestion_name = f"{space_name}___{param_name}___{parent_vals_name}"
                 search_point[space_name][param_name] = trial.suggest_categorical(suggestion_name, options)
             else:
                 raise ValueError(f"Unsupported parameter type: {type(param)}")
             invalid_trial = invalid_trial or (search_point[space_name][param_name] == SpecialParamValue.INVALID)
         return trial, search_point, invalid_trial
```

## olive/strategy/search_algorithm/random_sampler.py

```diff
@@ -19,33 +19,34 @@
             "num_samples": ConfigParam(type_=int, default_value=1, description="Number of samples to suggest."),
             "seed": ConfigParam(type_=int, default_value=1, description="Seed for the rng."),
             "with_replacement": ConfigParam(type_=bool, default_value=False, description="Sample with replacement."),
         }
 
     def initialize(self):
         """Initialize the searcher."""
-        self._search_space.set_seed(self._config.seed)
-        if not self._config.with_replacement:
+        # pylint: disable=attribute-defined-outside-init
+        self._search_space.set_seed(self.config.seed)
+        if not self.config.with_replacement:
             self._options = list(self._search_space.iterate())
         self._num_samples_suggested = 0
 
     def should_stop(self):
         should_stop = (self._search_space.empty() and self._num_samples_suggested > 0) or (
-            self._num_samples_suggested >= self._config.num_samples
+            self._num_samples_suggested >= self.config.num_samples
         )
-        if not self._config.with_replacement:
+        if not self.config.with_replacement:
             should_stop = should_stop or (len(self._options) == 0)
         return should_stop or super().should_stop()
 
     def suggest(self) -> Dict[str, Dict[str, Any]]:
         """Suggest a new configuration to try."""
         if self.should_stop():
             return None
 
-        if self._config.with_replacement:
+        if self.config.with_replacement:
             # sample a randrom point from the search space with replacement
             search_point = self._search_space.random_sample()
         else:
             # sample a random point from the search space without replacement
             search_point = self._search_space.rng.choice(self._options)
             self._options.remove(search_point)
```

## olive/strategy/search_algorithm/search_algorithm.py

```diff
@@ -35,17 +35,14 @@
         objectives = objectives or []
         higher_is_betters = higher_is_betters or []
         assert len(objectives) == len(higher_is_betters), "Number of objectives must match number of higher_is_betters"
         self._objectives = objectives
         self._higher_is_betters = higher_is_betters
 
         super().__init__(config)
-        # TODO(jambayk): Stop using _ private methods like _objectives, _config, etc
-        self._config = self.config
-        self.initialize()
 
     @abstractmethod
     def initialize(self):
         """Initialize the searcher."""
 
     def should_stop(self):
         """Check if the searcher should prune the current trial."""
```

## olive/strategy/search_algorithm/tpe_sampler.py

```diff
@@ -37,9 +37,9 @@
                 ),
             ),
         }
 
     def _create_sampler(self) -> optuna.samplers.TPESampler:
         """Create the sampler."""
         return optuna.samplers.TPESampler(
-            multivariate=self._config.multivariate, group=self._config.group, seed=self._config.seed
+            multivariate=self.config.multivariate, group=self.config.group, seed=self.config.seed
         )
```

## olive/systems/common.py

```diff
@@ -4,26 +4,27 @@
 # --------------------------------------------------------------------------
 from enum import Enum
 from pathlib import Path
 from typing import List, Optional, Union
 
 from olive.common.config_utils import ConfigBase
 from olive.common.pydantic_v1 import validator
+from olive.hardware.accelerator import Device
 
 
 class SystemType(str, Enum):
     Docker = "Docker"
     Local = "LocalSystem"
     AzureML = "AzureML"
     PythonEnvironment = "PythonEnvironment"
     IsolatedORT = "IsolatedORT"
 
 
 class AcceleratorConfig(ConfigBase):
-    device: str = None
+    device: Union[str, Device] = None
     execution_providers: List[str] = None
 
     @validator("execution_providers", always=True)
     def validate_device_and_execution_providers(cls, v, values):
         if v is None and values.get("device") is None:
             raise ValueError("Either device or execution_providers must be provided")
         return v
```

## olive/systems/local.py

```diff
@@ -7,15 +7,16 @@
 from olive.evaluator.olive_evaluator import OliveEvaluator, OliveEvaluatorFactory
 from olive.hardware.accelerator import AcceleratorSpec, Device
 from olive.model import ModelConfig
 from olive.systems.common import SystemType
 from olive.systems.olive_system import OliveSystem
 
 if TYPE_CHECKING:
-    from olive.evaluator.metric import Metric, MetricResult
+    from olive.evaluator.metric import Metric
+    from olive.evaluator.metric_result import MetricResult
     from olive.passes.olive_pass import Pass
 
 
 class LocalSystem(OliveSystem):
     system_type = SystemType.Local
 
     def run_pass(
```

## olive/systems/olive_system.py

```diff
@@ -6,15 +6,16 @@
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
 from olive.common.config_utils import validate_config
 from olive.systems.common import AcceleratorConfig, SystemType
 
 if TYPE_CHECKING:
-    from olive.evaluator.metric import Metric, MetricResult
+    from olive.evaluator.metric import Metric
+    from olive.evaluator.metric_result import MetricResult
     from olive.hardware.accelerator import AcceleratorSpec
     from olive.model import ModelConfig
     from olive.passes.olive_pass import Pass
 
 
 logger = logging.getLogger(__name__)
```

## olive/systems/system_config.py

```diff
@@ -142,16 +142,36 @@
 
     @root_validator(pre=True)
     def validate_config_type(cls, values):
         type_name = values.get("type")
         system_alias_class = getattr(system_alias, type_name, None)
         if system_alias_class:
             values["type"] = system_alias_class.system_type
+            if "config" not in values:
+                values["config"] = {}
+
+            if values["type"] == SystemType.AzureML and not values["config"].get("accelerators"):
+                raise ValueError("accelerators is required for AzureML system")
+
             if system_alias_class.accelerators:
-                values["config"]["accelerators"] = [{"device": acc} for acc in system_alias_class.accelerators]
+                valid_accelerators = []
+
+                if not values["config"].get("accelerators"):
+                    valid_accelerators = [
+                        {"device": acc, "execution_providers": None} for acc in system_alias_class.accelerators
+                    ]
+                else:
+                    for device in system_alias_class.accelerators:
+                        valid_accelerators.extend(
+                            {"device": acc["device"], "execution_providers": acc.get("execution_providers")}
+                            for acc in values["config"]["accelerators"]
+                            if acc["device"].lower() == device.lower()
+                        )
+
+                values["config"]["accelerators"] = valid_accelerators or None
             # TODO(myguo): consider how to use num_cpus and num_gpus in distributed inference.
         return values
 
     @validator("config", pre=True, always=True)
     def validate_config(cls, v, values):
         if "type" not in values:
             raise ValueError("Invalid type")
```

## olive/systems/azureml/aml_pass_runner.py

```diff
@@ -25,18 +25,14 @@
 
 
 def parse_pass_config_arg(raw_args):
     parser = argparse.ArgumentParser("Pass config")
 
     # parse config arg
     parser.add_argument("--pass_config", type=str, help="pass config", required=True)
-    parser.add_argument("--pass_accelerator_type", type=str, help="pass accelerator type", default="cpu")
-    parser.add_argument(
-        "--pass_execution_provider", type=str, help="pass execution provider", default="CPUExecutionProvider"
-    )
 
     return parser.parse_known_args(raw_args)
 
 
 def parse_pass_args(pass_type, accelerator_spec, raw_args):
     pass_class = PASS_REGISTRY[pass_type]
 
@@ -131,15 +127,15 @@
                 shutil.copy(old_path, new_path)
             else:
                 new_path.mkdir(parents=True, exist_ok=True)
                 copy_dir(old_path, new_path, dirs_exist_ok=True)
             input_model_config["config"]["model_path"] = str(new_path)
 
     # pass specific args
-    accelerator_spec = AcceleratorSpec(pass_config_arg.pass_accelerator_type, pass_config_arg.pass_execution_provider)
+    accelerator_spec = AcceleratorSpec(**pass_config["accelerator"])
     pass_args, extra_args = parse_pass_args(pass_type, accelerator_spec, extra_args)
 
     # load input_model
     input_model = ModelConfig.from_json(input_model_config).create_model()
 
     # load pass
     p = create_pass(pass_config, pass_args)
```

## olive/systems/azureml/aml_system.py

```diff
@@ -1,12 +1,11 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
-import copy
 import json
 import logging
 import shutil
 import tempfile
 from copy import deepcopy
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, List, NamedTuple, Optional, Tuple, Union
@@ -18,15 +17,15 @@
 from azure.core.exceptions import HttpResponseError, ServiceResponseError
 
 from olive.azureml.azureml_client import AzureMLClientConfig
 from olive.cache import normalize_data_path
 from olive.common.config_utils import ParamCategory, validate_config
 from olive.common.utils import copy_dir, retry_func
 from olive.data.config import DataConfig
-from olive.evaluator.metric import Metric, MetricResult
+from olive.evaluator.metric_result import MetricResult
 from olive.model import ModelConfig
 from olive.resource_path import (
     AZUREML_RESOURCE_TYPES,
     LOCAL_RESOURCE_TYPES,
     OLIVE_RESOURCE_ANNOTATIONS,
     AzureMLModel,
     ResourcePath,
@@ -34,14 +33,15 @@
     create_resource_path,
 )
 from olive.systems.common import AcceleratorConfig, AzureMLDockerConfig, AzureMLEnvironmentConfig, SystemType
 from olive.systems.olive_system import OliveSystem
 from olive.systems.system_config import AzureMLTargetUserConfig
 
 if TYPE_CHECKING:
+    from olive.evaluator.metric import Metric
     from olive.hardware.accelerator import AcceleratorSpec
     from olive.passes.olive_pass import Pass
 
 
 logger = logging.getLogger(__name__)
 
 RESOURCE_TYPE_TO_ASSET_TYPE = {
@@ -342,15 +342,15 @@
                 parameters.append(f"$[[--{param} ${{{{inputs.{param}}}}}]]")
             else:
                 parameters.append(f"--{param} ${{{{inputs.{param}}}}}")
         outputs = outputs or {}
         parameters.extend([f"--{param} ${{{{outputs.{param}}}}}" for param in outputs])
 
         cmd_line = f"python {script_name} {' '.join(parameters)}"
-        env_vars = copy.deepcopy(self.env_vars) if self.env_vars else {}
+        env_vars = deepcopy(self.env_vars) if self.env_vars else {}
         env_vars["OLIVE_LOG_LEVEL"] = logging.getLevelName(logger.getEffectiveLevel())
 
         # the name need to be lowercase
         # https://github.com/Azure/azure-sdk-for-python/blob/8b5217499caedba762b47fa6a118e51209f6f604/sdk/ml/azure-ai-ml/azure/ai/ml/entities/_builders/base_node.py#L217
         return command(
             name=name.lower(),  # convert to lowercase to avoid AzureML name restrictions
             display_name=display_name,
@@ -387,25 +387,20 @@
 
         olive_config_path = self._create_olive_config_file(self.olive_config, tmp_dir)
         if olive_config_path:
             code_files.append(olive_config_path)
 
         self.copy_code(code_files, code_root)
 
-        accelerator_info = {
-            "pass_accelerator_type": pass_config["accelerator"]["accelerator_type"],
-            "pass_execution_provider": pass_config["accelerator"]["execution_provider"],
-        }
         # prepare inputs
         model_resource_paths = model_config.get_resource_paths()
         inputs = {
             **self._create_model_inputs(model_resource_paths),
             **self._create_pass_inputs(pass_path_params),
             **data_params.data_inputs,
-            **accelerator_info,
         }
         # prepare outputs
         outputs = {"pipeline_output": Output(type=AssetTypes.URI_FOLDER)}
 
         # pass type
         pass_type = pass_config["type"]
 
@@ -428,15 +423,14 @@
         model_json = model_config.to_json(check_object=True)
 
         # input argument values
         args = {
             **self._create_model_args(model_json, model_resource_paths, tmp_dir),
             **self._create_pass_args(pass_config, pass_path_params, data_root, tmp_dir),
             **data_params.data_args,
-            **accelerator_info,
         }
 
         @pipeline()
         def pass_runner_pipeline():
             outputs = {}
             component = cmd(**args)
             outputs["pipeline_output"] = component.outputs.pipeline_output
@@ -600,15 +594,15 @@
             "metric_config": metric_config,
             "metric_user_script": metric_user_script,
             "metric_script_dir": metric_script_dir,
             "metric_data_dir": metric_data_dir,
         }
 
     def evaluate_model(
-        self, model_config: ModelConfig, data_root: str, metrics: List[Metric], accelerator: "AcceleratorSpec"
+        self, model_config: ModelConfig, data_root: str, metrics: List["Metric"], accelerator: "AcceleratorSpec"
     ) -> MetricResult:
         if model_config.type.lower() == "SNPEModel".lower():
             raise NotImplementedError("SNPE model does not support azureml evaluation")
         if model_config.type.lower() == "OpenVINOModel".lower():
             raise NotImplementedError("OpenVINO model does not support azureml evaluation")
 
         with tempfile.TemporaryDirectory() as tempdir:
@@ -628,15 +622,15 @@
             return MetricResult.parse_obj(metric_results)
 
     def _create_pipeline_for_evaluation(
         self,
         data_root: str,
         tmp_dir: str,
         model_config: ModelConfig,
-        metrics: List[Metric],
+        metrics: List["Metric"],
         accelerator: "AcceleratorSpec",
     ):
         tmp_dir = Path(tmp_dir)
 
         # model json
         model_json = model_config.to_json(check_object=True)
 
@@ -669,15 +663,15 @@
 
         return pipeline_job
 
     def _create_metric_component(
         self,
         data_root: str,
         tmp_dir: Path,
-        metric: Metric,
+        metric: "Metric",
         model_args: Dict[str, Input],
         model_resource_paths: Dict[str, ResourcePath],
         accelerator_config_path: str,
     ):
         metric_json = metric.to_json(check_object=True)
 
         # prepare code
```

## olive/systems/docker/docker_system.py

```diff
@@ -12,22 +12,23 @@
 
 import docker
 from docker.errors import BuildError, ContainerError
 
 import olive.systems.docker.utils as docker_utils
 from olive.cache import get_local_path_from_root
 from olive.common.config_utils import ParamCategory, validate_config
-from olive.evaluator.metric import Metric, MetricResult
+from olive.evaluator.metric_result import MetricResult
 from olive.hardware import Device
 from olive.model import ModelConfig
 from olive.systems.common import AcceleratorConfig, LocalDockerConfig, SystemType
 from olive.systems.olive_system import OliveSystem
 from olive.systems.system_config import DockerTargetUserConfig
 
 if TYPE_CHECKING:
+    from olive.evaluator.metric import Metric
     from olive.hardware.accelerator import AcceleratorSpec
     from olive.passes import Pass
 
 logger = logging.getLogger(__name__)
 
 
 class DockerSystem(OliveSystem):
@@ -214,15 +215,15 @@
                 logger.debug("Model path is: %s", output_model.config["model_path"])
                 return output_model
         else:
             logger.error("Model output file %s not found.", model_output_json_file)
             return None
 
     def evaluate_model(
-        self, model_config: "ModelConfig", data_root: str, metrics: List[Metric], accelerator: "AcceleratorSpec"
+        self, model_config: "ModelConfig", data_root: str, metrics: List["Metric"], accelerator: "AcceleratorSpec"
     ) -> Dict[str, Any]:
         container_root_path = Path("/olive-ws/")
         with tempfile.TemporaryDirectory() as tempdir:
             metric_json = self._run_eval_container(
                 tempdir, model_config, data_root, metrics, accelerator, container_root_path
             )
             if metric_json.is_file():
@@ -234,15 +235,15 @@
                 return None
 
     def _run_eval_container(
         self,
         workdir,
         model_config: "ModelConfig",
         data_root: str,
-        metrics: List[Metric],
+        metrics: List["Metric"],
         accelerator: "AcceleratorSpec",
         container_root_path: Path,
     ):
         eval_output_path = "eval_output"
         eval_output_name = "eval_res.json"
 
         volumes_list = []
@@ -295,15 +296,15 @@
             output_path=output_mount_path,
             output_name=eval_output_name,
             accelerator=accelerator,
         )
         return self._run_container(eval_command, volumes_list, output_local_path, eval_output_name, accelerator)
 
     @staticmethod
-    def _create_eval_config(model_config: "ModelConfig", metrics: List[Metric], model_mounts: Dict[str, str]):
+    def _create_eval_config(model_config: "ModelConfig", metrics: List["Metric"], model_mounts: Dict[str, str]):
         model_json = model_config.to_json(check_object=True)
         for k, v in model_mounts.items():
             model_json["config"][k] = v
 
         return {"metrics": [k.dict() for k in metrics], "model": model_json}
 
     @staticmethod
```

## olive/systems/docker/utils.py

```diff
@@ -48,16 +48,18 @@
 ):
     # no need to pass model_path since it's already updated in config file
     parameters = [
         f"--config {config_path}",
         f"--output_path {output_path}",
         f"--output_name {output_name}",
         f"--accelerator_type {accelerator.accelerator_type}",
-        f"--execution_provider {accelerator.execution_provider}",
     ]
+    if accelerator.execution_provider:
+        parameters.append(f"--execution_provider {accelerator.execution_provider}")
+
     return f"python {eval_script_path} {' '.join(parameters)}"
 
 
 def create_run_command(run_params: dict):
     if not run_params:
         return {}
     run_command_dict = {}
```

## olive/systems/isolated_ort/isolated_ort_system.py

```diff
@@ -20,15 +20,16 @@
 from olive.hardware import Device
 from olive.systems.common import AcceleratorConfig, SystemType
 from olive.systems.olive_system import OliveSystem
 from olive.systems.system_config import IsolatedORTTargetUserConfig
 from olive.systems.utils import create_new_environ, run_available_providers_runner
 
 if TYPE_CHECKING:
-    from olive.evaluator.metric import Metric, MetricResult
+    from olive.evaluator.metric import Metric
+    from olive.evaluator.metric_result import MetricResult
     from olive.hardware.accelerator import AcceleratorSpec
     from olive.model import ModelConfig, ONNXModelHandler
     from olive.passes.olive_pass import Pass
 
 logger = logging.getLogger(__name__)
 
 
@@ -114,15 +115,15 @@
         inference_settings = model.merge_inference_settings(inference_settings, execution_providers)
         return {
             "inference_settings": inference_settings,
             "use_ort_extensions": model.use_ort_extensions,
             "io_bind": cls.io_bind_enabled(metric, model.inference_settings),
             "device": str(device),
             "share_kv_buffer": metric.user_config.shared_kv_buffer,
-            "use_fp16": any(v == "float16" for v in model.get_io_config()["input_types"]),
+            "use_fp16": any(v == "float16" for v in model.io_config["input_types"]),
         }
 
     def _run_inference(self, **kwargs):
         """Run inference using the inference runner.
 
         :param kwargs: arguments to be passed to the inference runner
         """
@@ -141,15 +142,15 @@
         post_func: Callable = None,
         device: Device = Device.CPU,
         execution_providers: Union[str, List[str]] = None,
     ) -> Tuple[OliveModelOutput, Any]:
         inference_config = self._get_common_config(model, metric, device, execution_providers)
         inference_config["mode"] = "inference"
 
-        io_config = model.get_io_config()
+        io_config = model.io_config
 
         preds = []
         targets = []
         logits = []
         logits_dict = collections.defaultdict(list)
         output_names = io_config["output_names"]
         is_single_tensor_output = len(output_names) == 1
@@ -242,15 +243,15 @@
                 "mode": "latency",
                 "warmup_num": warmup_num,
                 "repeat_test_num": repeat_test_num,
                 "sleep_num": sleep_num,
             }
         )
 
-        io_config = model.get_io_config()
+        io_config = model.io_config
 
         with tempfile.TemporaryDirectory() as temp_dir:
             temp_dir_path = Path(temp_dir)
             # create input and output dir
             input_dir = temp_dir_path / "input"
             input_dir.mkdir(parents=True, exist_ok=True)
             output_dir = temp_dir_path / "output"
```

## olive/systems/python_environment/python_environment_system.py

```diff
@@ -8,15 +8,15 @@
 import platform
 import shutil
 import tempfile
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
 from olive.common.utils import run_subprocess
-from olive.evaluator.metric import MetricResult
+from olive.evaluator.metric_result import MetricResult
 from olive.model import ModelConfig
 from olive.systems.common import AcceleratorConfig, SystemType
 from olive.systems.olive_system import OliveSystem
 from olive.systems.system_config import PythonEnvironmentTargetUserConfig
 from olive.systems.utils import create_new_environ, get_package_name_from_ep, run_available_providers_runner
 
 if TYPE_CHECKING:
```

## olive/systems/utils/misc.py

```diff
@@ -35,17 +35,17 @@
 
 def create_managed_system(system_config: "SystemConfig", accelerator: "AcceleratorSpec"):
     # pylint: disable=consider-using-with
     assert system_config.olive_managed_env, "system_config.olive_managed_env must be True"
 
     # for host system, use the first available accelerator
     if accelerator:
-        accelerator_cfg = [
-            {"device": accelerator.accelerator_type, "execution_providers": [accelerator.execution_provider]}
-        ]
+        accelerator_cfg = [{"device": accelerator.accelerator_type}]
+        if accelerator.execution_provider:
+            accelerator_cfg[0]["execution_providers"] = [accelerator.execution_provider]
     else:
         accelerator_cfg = None
         accelerator = DEFAULT_CPU_ACCELERATOR
 
     # create a new system with the same type as the origin system
     if system_config.type in [SystemType.Local, SystemType.IsolatedORT]:
         raise NotImplementedError(f"olive_managed_env is not supported for {system_config.type} System")
@@ -79,14 +79,15 @@
             olive_managed_env=True,
             requirements_file=system_config.config.requirements_file,
         )
         new_system.install_requirements(accelerator)
     elif system_config.type == SystemType.Docker:
         from olive.systems.docker import DockerSystem
 
+        assert accelerator.execution_provider, "Execution provider must be specified for Docker system"
         dockerfile = PROVIDER_DOCKERFILE_MAPPING.get(accelerator.execution_provider, "Dockerfile.cpu")
         # TODO(myguo): create a temp dir for the build context
         new_system = DockerSystem(
             local_docker_config={
                 "image_name": f"olive_{accelerator.execution_provider[:-17].lower()}",
                 "dockerfile": dockerfile,
                 "build_context_path": Path(__file__).parents[1] / "docker",
@@ -98,14 +99,15 @@
                 str(system_config.config.requirements_file) if system_config.config.requirements_file else None
             ),
         )
 
     elif system_config.type == SystemType.AzureML:
         from olive.systems.azureml import AzureMLSystem
 
+        assert accelerator.execution_provider, "Execution provider must be specified for Docker system"
         dockerfile = PROVIDER_DOCKERFILE_MAPPING.get(accelerator.execution_provider, "Dockerfile.cpu")
         temp_dir = tempfile.TemporaryDirectory()  # pylint: disable=consider-using-with
         build_context_path = Path(temp_dir.name)
         shutil.copy2(str(Path(__file__).parents[1] / "docker" / dockerfile), build_context_path)
         if system_config.config.requirements_file:
             shutil.copyfile(system_config.config.requirements_file, build_context_path / "requirements.txt")
         else:
```

## olive/workflows/run/__main__.py

```diff
@@ -1,33 +1,10 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
-import argparse
-
-from olive.common.utils import set_tempdir
-from olive.workflows import run
-
 if __name__ == "__main__":
-    parser = argparse.ArgumentParser("Olive Workflow: Custom Run")
-    parser.add_argument(
-        "--package-config",
-        type=str,
-        required=False,
-        help=(
-            "For advanced users. Path to optional package (json) config file with location "
-            "of individual pass module implementation and corresponding dependencies."
-            "Configuration might also include user owned/proprietary/private pass implementations."
-        ),
-    )
-    parser.add_argument("--run-config", "--config", type=str, help="Path to json config file", required=True)
-    parser.add_argument("--setup", help="Whether run environment setup", action="store_true")
-    parser.add_argument("--data-root", "--data_root", help="The data root path for optimization", required=False)
-    parser.add_argument("--tempdir", type=str, help="Root directory for tempfile directories and files", required=False)
-
-    args = parser.parse_args()
+    import sys
 
-    set_tempdir(args.tempdir)
+    from olive.cli.launcher import legacy_call
 
-    var_args = vars(args)
-    del var_args["tempdir"]
-    run(**var_args)
+    legacy_call("olive.workflows.run", "run", *sys.argv[1:])
```

## olive/workflows/run/config.py

```diff
@@ -42,23 +42,20 @@
     log_to_file: bool = False
 
     def create_engine(self, azureml_client_config):
         config = self.dict(include=EngineConfig.__fields__.keys())
         return Engine(**config, azureml_client_config=azureml_client_config)
 
 
-INPUT_MODEL_DATA_CONFIG = "__input_model_data_config__"
-
-
 class RunConfig(ConfigBase):
     azureml_client: AzureMLClientConfig = None
     input_model: ModelConfig
     systems: Dict[str, SystemConfig] = None
     data_root: str = None
-    data_configs: Dict[str, DataConfig] = None
+    data_configs: List[DataConfig] = []  # noqa: RUF012
     evaluators: Dict[str, OliveEvaluatorConfig] = None
     engine: RunEngineConfig = None
     pass_flows: List[List[str]] = None
     passes: Dict[str, RunPassConfig] = None
     auto_optimizer_config: AutoOptimizerConfig = None
 
     @validator("input_model", pre=True)
@@ -77,56 +74,22 @@
 
     @validator("engine", pre=True, always=True)
     def default_engine_config(cls, v):
         if v is None:
             v = {}
         return v
 
-    @validator("data_configs", pre=True, always=True)
-    def insert_input_model_data_config(cls, v, values):
-        if "input_model" not in values:
-            raise ValueError("Invalid input model")
-
-        if not v:
-            # if data_configs is None, create an empty dict
-            v = {}
-
-        if INPUT_MODEL_DATA_CONFIG in v:
-            raise ValueError(f"Data config name {INPUT_MODEL_DATA_CONFIG} is reserved. Please use another name.")
-
-        # insert input model hf data config if present
-        hf_config = values["input_model"].dict()["config"].get("hf_config", {})
-        hf_config_dataset = hf_config.get("dataset", None)
-        if hf_config_dataset:
-            params_config = {
-                "model_name": hf_config.get("model_name", None),
-                "task": hf_config.get("task", None),
-                **hf_config_dataset,
-            }
-            # insert trust_remote_code from from_pretrained_args if present
-            # won't override if value was set to False explicitly
-            # will keep as list of keys for future extension
-            for key in ["trust_remote_code"]:
-                if hf_config.get("from_pretrained_args", {}).get(key) and params_config.get(key) is None:
-                    params_config[key] = hf_config["from_pretrained_args"][key]
-            v[INPUT_MODEL_DATA_CONFIG] = {
-                "name": INPUT_MODEL_DATA_CONFIG,
-                "type": HuggingfaceContainer.__name__,
-                "params_config": params_config,
-            }
-        return v
-
     @validator("data_configs", pre=True)
     def validate_data_config_names(cls, v):
         if not v:
             return v
 
         # validate data config name is unique
         data_name_set = set()
-        for data_config in v.values():
+        for data_config in v:
             data_config_obj = validate_config(data_config, DataConfig)
             if data_config_obj.name in data_name_set:
                 raise ValueError(f"Data config name {data_config_obj.name} is duplicated. Please use another name.")
             data_name_set.add(data_config_obj.name)
         return v
 
     @validator("data_configs", pre=True, each_item=True)
@@ -135,18 +98,14 @@
             raise ValueError("Invalid input model")
 
         hf_config = values["input_model"].dict()["config"].get("hf_config", {})
 
         if isinstance(v, DataConfig):
             v = v.dict()
 
-        if v["name"] == INPUT_MODEL_DATA_CONFIG:
-            # skip validation for input model data config
-            return v
-
         if v["type"] == HuggingfaceContainer.__name__:
             # auto insert model_name and task from input model hf config if not present
             # both are required for huggingface container
             for key in ["model_name", "task"]:
                 if not v["params_config"].get(key, None):
                     v["params_config"][key] = hf_config.get(key, None)
             # auto insert trust_remote_code from input model hf config
@@ -212,17 +171,15 @@
             return v
 
         searchable_configs = set()
         for param_name in v["config"]:
             if v["config"][param_name] == PassParamDefault.SEARCHABLE_VALUES:
                 searchable_configs.add(param_name)
             if param_name.endswith("data_config"):
-                # we won't auto insert the input model data config for pass
-                # user must explicitly set the data config to INPUT_MODEL_DATA_CONFIG if needed
-                v["config"] = _resolve_data_config(v["config"], values, param_name, auto_insert=False)
+                v["config"] = _resolve_data_config(v["config"], values, param_name)
 
         data_dir_config = v["config"].get("data_dir", None)
         if isinstance(data_dir_config, dict):
             if _have_aml_client(data_dir_config, values):
                 data_dir_config["config"]["azureml_client"] = values["azureml_client"]
             v["config"]["data_dir"] = data_dir_config
 
@@ -292,22 +249,34 @@
         if v[system_alias].type == "AzureML":
             if not values["azureml_client"]:
                 raise ValueError("AzureML client config is required for AzureML system")
             v[system_alias].config.azureml_client_config = values["azureml_client"]
     return v
 
 
-def _resolve_data_config(v, values, data_config_alias, auto_insert=True):
-    # get the value for data_config_alias in v
-    data_container_config = v.get(data_config_alias, None)
-    # auto insert input model data config if data_container_config is None
-    if not data_container_config and INPUT_MODEL_DATA_CONFIG in values["data_configs"] and auto_insert:
-        v[data_config_alias] = INPUT_MODEL_DATA_CONFIG
+def _resolve_data_config(v, values, data_config_alias):
+    if not isinstance(v, dict):
+        # if not a dict, return the original value
+        return v
+
+    # get name of sub component
+    sub_component = v.get(data_config_alias)
+    if not isinstance(sub_component, str):
+        return v
+
     # resolve data_config_alias to data config
-    return _resolve_config_str(v, values, data_config_alias, component_name="data_configs")
+    components = values.get("data_configs") or []
+    component_map = {cmp.name: cmp for cmp in components}
+
+    # resolve sub component name to component config
+    if sub_component not in component_map:
+        raise ValueError(f"{data_config_alias} {sub_component} not found in {components}")
+
+    v[data_config_alias] = component_map[sub_component]
+    return v
 
 
 def _resolve_evaluator(v, values):
     if not isinstance(v, dict):
         return v
 
     evaluator = v.get("evaluator")
@@ -329,10 +298,10 @@
 
 def _have_aml_client(config_item, values):
     resource_path_type = config_item.get("type")
     if resource_path_type in AZUREML_RESOURCE_TYPES:
         rp_aml_client = config_item.get("config", {}).get("azureml_client")
         if not rp_aml_client:
             if "azureml_client" not in values:
-                raise ValueError(f"azureml_client is required for azureml resource path in config if {config_item}")
+                raise ValueError(f"azureml_client is required for azureml resource path in config of {config_item}")
             return True
     return False
```

## olive/workflows/run/run.py

```diff
@@ -4,20 +4,20 @@
 # --------------------------------------------------------------------------
 import importlib.metadata
 import logging
 import subprocess
 import sys
 from copy import deepcopy
 from pathlib import Path
-from typing import List, Union
+from typing import Generator, List, Union
 
 from olive.auto_optimizer import AutoOptimizer
-from olive.hardware.accelerator import create_accelerators
 from olive.logging import enable_filelog, set_default_logger_severity, set_ort_logger_severity, set_verbosity_info
 from olive.package_config import OlivePackageConfig
+from olive.systems.accelerator_creator import create_accelerators
 from olive.systems.common import SystemType
 from olive.workflows.run.config import RunConfig, RunPassConfig
 
 logger = logging.getLogger(__name__)
 
 
 def dependency_setup(package_config: OlivePackageConfig, run_config: RunConfig):
@@ -115,14 +115,24 @@
         logger.info(
             "Please make sure the following packages are installed in %s environment: %s",
             run_config.engine.host.type,
             remote_packages,
         )
 
 
+def get_pass_module_path(pass_type: str, package_config: OlivePackageConfig) -> str:
+    pass_module_config = package_config.passes.get(pass_type)
+    return pass_module_config.module_path
+
+
+def is_execution_provider_required(run_config: RunConfig, package_config: OlivePackageConfig) -> bool:
+    passes = get_used_passes(run_config)
+    return any(get_pass_module_path(p.type, package_config).startswith("olive.passes.onnx") for p in passes)
+
+
 def run_engine(package_config: OlivePackageConfig, run_config: RunConfig, data_root: str = None):
     import onnxruntime as ort
 
     from olive.passes import Pass
 
     # for onnxruntime
     # ort_py_log_severity_level: python logging levels
@@ -143,28 +153,50 @@
     )
 
     if is_azureml_system:
         from olive.systems.azureml.aml_system import AzureMLSystem
 
         AzureMLSystem.olive_config = run_config.to_json()
 
-    no_evaluation = (
+    auto_optimizer_enabled = (
+        not run_config.passes
+        and run_config.auto_optimizer_config is not None
+        and not run_config.auto_optimizer_config.disable_auto_optimizer
+    )
+    if auto_optimizer_enabled:
+        is_ep_required = True
+    else:
+        is_ep_required = is_execution_provider_required(run_config, package_config)
+
+    # Register passes since we need to know whether they need to run on target
+    used_passes = list(get_used_passes(run_config))
+    for pass_config in used_passes:
+        logger.debug("Registering pass %s", pass_config.type)
+        package_config.import_pass_module(pass_config.type)
+
+    # check if target is not used
+    target_not_used = (
+        # no evaluator given (also implies no search)
         engine.evaluator_config is None
-        and run_config.passes
-        and all(pass_config.evaluator is None for pass_config in run_config.passes.values())
+        # not using auto optimizer
+        and used_passes
+        # no pass specific evaluator
+        # no pass needs to run on target
+        and all(
+            pass_config.evaluator is None and Pass.registry[pass_config.type.lower()].run_on_target is False
+            for pass_config in used_passes
+        )
+    )
+    accelerator_specs = create_accelerators(
+        engine.target_config, skip_supported_eps_check=target_not_used, is_ep_required=is_ep_required
     )
-    accelerator_specs = create_accelerators(engine.target_config, skip_supported_eps_check=no_evaluation)
 
     pass_list = []
     acc_list = []
-    if (
-        not run_config.passes
-        and run_config.auto_optimizer_config is not None
-        and not run_config.auto_optimizer_config.disable_auto_optimizer
-    ):
+    if auto_optimizer_enabled:
         # For auto optimizer, Olive generates passes and pass_flows for each accelerator
         # that means, the passes and pass_flows might be different for each accelerator
         for acc_spec in accelerator_specs:
             _passes, pass_flows = AutoOptimizer(
                 input_model,
                 engine.evaluator_config,
                 acc_spec,
@@ -189,15 +221,19 @@
     # For time being, we are keeping both loops, but in future, we might want to refactor the code
     # to remove engine level loop and pass the accelerator_specs to the engine directly.
     for accelerator_spec, (passes, pass_flows) in zip(acc_list, pass_list):
         engine.reset_passes()
         if passes:
             # First pass registers the necessary module implementation
             for pass_config in passes.values():
-                logger.info("Importing pass module %s", pass_config.type)
+                if pass_config.type.lower() in Pass.registry:
+                    logger.debug("Pass %s already registered", pass_config.type)
+                    continue
+                # auto optimizer scenario
+                logger.debug("Registering pass %s", pass_config.type)
                 package_config.import_pass_module(pass_config.type)
 
             # Second pass, initializes the pass and registers it with the engine
             for pass_name, pass_config in passes.items():
                 host = pass_config.host.create_system() if pass_config.host is not None else None
                 engine.register(
                     Pass.registry[pass_config.type.lower()],
@@ -309,7 +345,19 @@
         if package_name == "onnxruntime-extensions":
             # onnxruntime-packages is under onnxruntime_extensions namespace
             # not an actual onnxruntime package
             continue
         if package_name.startswith(("onnxruntime", "ort-nightly")):
             local_ort_packages.append(package_name)
     return local_ort_packages
+
+
+def get_used_passes(run_config: RunConfig) -> Generator["RunPassConfig", None, None]:
+    if run_config.pass_flows:
+        passes = set()
+        for pass_flow in run_config.pass_flows:
+            for pass_name in pass_flow:
+                if run_config.passes[pass_name].type not in passes:
+                    passes.add(run_config.passes[pass_name].type)
+                    yield run_config.passes[pass_name]
+    elif run_config.passes:
+        yield from run_config.passes.values()
```

## Comparing `olive/passes/pytorch/gptq_utils.py` & `olive/passes/pytorch/quant_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,41 +132,42 @@
 
 
 def _quant_linear_forward(inputs, qweight, scales, qzeros, bits, groupsize, in_features, out_features):
     assert bits == 4, "Only 4 bits are supported."
     return QuantLinearTorchFunction().apply(inputs, qweight, scales, qzeros, bits, groupsize, in_features, out_features)
 
 
-class QuantLinearORT(nn.Module):
+class QuantLinear(nn.Module):
     # pylint: disable=W0201
     def __init__(self, bits, groupsize, infeatures, outfeatures, bias, *args, **kwargs):
         super().__init__()
         if bits not in [2, 3, 4, 5, 6, 7, 8]:
             raise ValueError("Only 2,4,5,6,7,8 bits are supported.")
         self.infeatures = infeatures
         self.outfeatures = outfeatures
         self.bits = bits
         self.orig_fp_weight = None
         self.maxq = 2**self.bits - 1
         self.groupsize = groupsize if groupsize != -1 else infeatures
+        self.input_model_dtype = kwargs.get("input_model_dtype", torch.float16)
 
         self.register_buffer(
             "qweight",
             torch.zeros((outfeatures, infeatures // self.groupsize, self.groupsize // (8 // bits)), dtype=torch.uint8),
         )
         self.register_buffer(
             "qzeros",
             torch.zeros((math.ceil(infeatures // self.groupsize) * (outfeatures // 8 * self.bits)), dtype=torch.uint8),
         )
         self.register_buffer(
-            "scales", torch.zeros((math.ceil(infeatures / self.groupsize) * outfeatures), dtype=torch.float)
+            "scales", torch.zeros((math.ceil(infeatures / self.groupsize) * outfeatures), dtype=self.input_model_dtype)
         )
         self.register_buffer("g_idx", torch.tensor([i // self.groupsize for i in range(infeatures)], dtype=torch.int32))
         if bias:
-            self.register_buffer("bias", torch.zeros((outfeatures), dtype=torch.float))
+            self.register_buffer("bias", torch.zeros((outfeatures), dtype=self.input_model_dtype))
         else:
             self.bias = None
 
     def forward(self, x):
         out = _quant_linear_forward(
             x, self.qweight, self.scales, self.qzeros, self.bits, self.groupsize, self.infeatures, self.outfeatures
         )
@@ -230,15 +231,15 @@
         if pad_len > 0:
             intweight_pt = torch.nn.functional.pad(intweight_pt, (0, 0, 0, pad_len), "constant", 0)
             intzeros_pt = torch.nn.functional.pad(intzeros_pt, (0, 0, 0, pad_len), "constant", 0)
 
         intzeros_pt = (intzeros_pt[:, 0::2]) | (intzeros_pt[:, 1::2] << 4)
         intzeros_pt = intzeros_pt.reshape(-1)
 
-        intweight_pt_t = intweight.T
+        intweight_pt_t = intweight_pt.T
         intweight_pt_t = (intweight_pt_t[:, 0::2]) | (intweight_pt_t[:, 1::2] << 4)
         intweight_pt_t = intweight_pt_t.reshape(cols, k_blocks, blob_size)
 
         scales_pt = scales_pt.reshape(-1)
 
         assert self.qweight.shape == intweight_pt_t.shape
         assert self.qzeros.shape == intzeros_pt.shape
```

## Comparing `olive/platform_sdk/qualcomm/configure.py` & `olive/platform_sdk/qualcomm/configure/configure.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,65 +1,67 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 
-import argparse
 import logging
 import os
 import platform
 import shutil
 from importlib import resources
 from pathlib import Path
 
 from olive.common.utils import run_subprocess
 from olive.platform_sdk.qualcomm.constants import SDKTargetDevice
 from olive.platform_sdk.qualcomm.qnn.env import QNNSDKEnv
 from olive.platform_sdk.qualcomm.snpe.env import SNPESDKEnv
 
-# pylint: disable=redefined-outer-name
-
 logger = logging.getLogger(__name__)
 
-script_name = "create_python_env.sh" if platform.system() == "Linux" else "create_python_env.ps1"
 
+def configure_dev(py_version: str, sdk: str):
+    """Configure Qualcomm SDK for model development."""
+    os.environ["PIP_EXTRA_ARGS"] = "--no-cache-dir"
 
-def dev(args):
     resource_path = "olive.platform_sdk.qualcomm"
-    if args.sdk == "snpe":
+    if sdk == "snpe":
         sdk_env = SNPESDKEnv()
     else:
         sdk_env = QNNSDKEnv()
     sdk_arch = sdk_env.target_arch
     if sdk_arch not in (SDKTargetDevice.x86_64_linux, SDKTargetDevice.x86_64_windows):
         return
 
-    logger.info("Configuring %s for %s with python %s...", args.sdk, sdk_arch, args.py_version)
+    script_name = "create_python_env.sh" if platform.system() == "Linux" else "create_python_env.ps1"
+
+    logger.info("Configuring %s for %s with python %s...", sdk, sdk_arch, py_version)
+    cmd = None
     with resources.path(resource_path, script_name) as create_python_env_path:
         if platform.system() == "Linux":
-            cmd = f"bash {create_python_env_path} -v {args.py_version} --sdk {args.sdk}"
+            cmd = f"bash {create_python_env_path} -v {py_version} --sdk {sdk}"
         elif platform.system() == "Windows":
-            cmd = f"powershell {create_python_env_path} {args.py_version} {args.sdk}"
+            cmd = f"powershell {create_python_env_path} {py_version} {sdk}"
         run_subprocess(cmd, check=True)
     logger.info("Done")
 
 
-def eval(args):  # noqa: A001  #pylint: disable=redefined-builtin
+def configure_eval(sdk: str):
+    """Configure Qualcomm SDK for model evaluation."""
     resource_path = "olive.platform_sdk.qualcomm"
-    if args.sdk == "snpe":
+    if sdk == "snpe":
         sdk_env = SNPESDKEnv()
     else:
         sdk_env = QNNSDKEnv()
     target_arch_name = sdk_env.target_arch
     if target_arch_name not in [SDKTargetDevice.aarch64_windows, SDKTargetDevice.arm64x_windows]:
         return
 
     sdk_root = sdk_env.sdk_root_path
 
-    logger.info("Configuring %s for %s...", args.sdk, target_arch_name)
+    logger.info("Configuring %s for %s...", sdk, target_arch_name)
 
     bin_path = Path(f"{sdk_root}/bin/{target_arch_name}")
     lib_path = Path(f"{sdk_root}/lib/{target_arch_name}")
     dsp_lib_path = Path(f"{sdk_root}/lib/dsp")
 
     # symlink all files under 'olive-arm-win'
     # If all files are not under the same path, there are problems with the dll files being spread under
@@ -78,28 +80,15 @@
         run_subprocess(cmd, check=True)
         if not (olive_sdk_path / "libcdsprpc.dll").exists():
             raise RuntimeError(f"Failed to copy libcdsprpc.dll to {olive_sdk_path}")
 
     logger.info("Done")
 
 
-if __name__ == "__main__":
-    # create args for py_version
-    os.environ["PIP_EXTRA_ARGS"] = "--no-cache-dir"
-    parser = argparse.ArgumentParser("Olive Qualcomm SDK: Configure")
-    parser.add_argument(
-        "--py_version",
-        type=str,
-        help="Python version, use 3.6 for tensorflow 1.15. Otherwise 3.8",
-        required=True,
-        choices=["3.6", "3.8"],
-    )
-    parser.add_argument(
-        "--sdk",
-        type=str,
-        help="Qualcomm SDK, snpe or qnn",
-        required=True,
-        choices=["snpe", "qnn"],
-    )
-    args = parser.parse_args()
-    dev(args)
-    eval(args)
+def configure(py_version: str, sdk: str):
+    """Configure Qualcomm SDK for Olive.
+
+    :param py_version: Python version, use 3.6 for tensorflow 1.15 and 3.8 otherwise
+    :param sdk: Qualcomm SDK, snpe or qnn
+    """
+    configure_dev(py_version, sdk)
+    configure_eval(sdk)
```

## Comparing `olive/scripts/manage_compute_instance.py` & `olive/cli/manage_aml_compute.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,152 +1,152 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
-import argparse
 import logging
+from argparse import ArgumentParser
 from pathlib import Path
 
-try:
-    from azure.ai.ml import MLClient
-    from azure.ai.ml.entities import AmlCompute
-except ImportError:
-    raise ImportError("azure-ai-ml is not installed. Please install azure-ai-ml packages to use this script.") from None
-
-try:
-    from azure.identity import AzureCliCredential, DefaultAzureCredential, InteractiveBrowserCredential
-except ImportError:
-    raise ImportError(
-        "azure-identity is not installed. Please install azure-identity packages to use this script."
-    ) from None
+from olive.cli.base import BaseOliveCLICommand
 
 logger = logging.getLogger(__name__)
 
 
-def get_args():
-    parser = argparse.ArgumentParser(description="Create new compute in your AzureML workspace")
-    group = parser.add_mutually_exclusive_group(required=True)
-    group.add_argument("--create", "-c", action="store_true", help="Create new compute")
-    group.add_argument("--delete", "-d", action="store_true", help="Delete existing compute")
-    parser.add_argument("--subscription_id", type=str, required=False, help="Azure subscription ID")
-    parser.add_argument("--resource_group", type=str, required=False, help="Name of the Azure resource group")
-    parser.add_argument("--workspace_name", type=str, required=False, help="Name of the AzureML workspace")
-    parser.add_argument(
-        "--aml_config_path",
-        type=str,
-        required=False,
-        help="Path to AzureML config file. If provided, subscription_id, resource_group and workspace_name are ignored",
-    )
-    parser.add_argument("--compute_name", type=str, required=True, help="Name of the new compute")
-    parser.add_argument(
-        "--vm_size",
-        type=str,
-        required=False,
-        help="VM size of the new compute. This is required if you are creating a compute instance",
-    )
-    parser.add_argument(
-        "--location",
-        type=str,
-        required=False,
-        help="Location of the new compute. This is required if you are creating a compute instance",
-    )
-    parser.add_argument("--min_nodes", type=int, required=False, default=0, help="Minimum number of nodes")
-    parser.add_argument("--max_nodes", type=int, required=False, default=2, help="Maximum number of nodes")
-    parser.add_argument(
-        "--idle_time_before_scale_down", type=int, required=False, default=120, help="Idle seconds before scaledown"
-    )
-    return parser.parse_args()
-
-
-def main():
-    logger.info("Running create new compute script...")
-    args = get_args()
-    aml_config_path = args.aml_config_path
-    subscription_id = args.subscription_id
-    resource_group = args.resource_group
-    workspace_name = args.workspace_name
-    ml_client = get_ml_client(aml_config_path, subscription_id, resource_group, workspace_name)
-    compute_name = args.compute_name
-
-    is_create = args.create
-    is_delete = args.delete
-    if is_create:
-        logger.info("Creating compute %s...", compute_name)
-        vm_size = args.vm_size
-        location = args.location
-        min_nodes = args.min_nodes
-        max_nodes = args.max_nodes
-        idle_time_before_scale_down = args.idle_time_before_scale_down
-        if vm_size is None:
-            raise ValueError("vm_size must be provided if operation is create")
-        if location is None:
-            raise ValueError("location must be provided if operation is create")
-        cluster_basic = AmlCompute(
-            name=compute_name,
-            type="amlcompute",
-            size=vm_size,
-            location=location,
-            min_instances=min_nodes,
-            max_instances=max_nodes,
-            idle_time_before_scale_down=idle_time_before_scale_down,
+class ManageAMLComputeCommand(BaseOliveCLICommand):
+    @staticmethod
+    def register_subcommand(parser: ArgumentParser):
+        sub_parser = parser.add_parser("manage-aml-compute", help="Create new compute in your AzureML workspace")
+        group = sub_parser.add_mutually_exclusive_group(required=True)
+        group.add_argument("--create", "-c", action="store_true", help="Create new compute")
+        group.add_argument("--delete", "-d", action="store_true", help="Delete existing compute")
+        sub_parser.add_argument("--subscription_id", type=str, required=False, help="Azure subscription ID")
+        sub_parser.add_argument("--resource_group", type=str, required=False, help="Name of the Azure resource group")
+        sub_parser.add_argument("--workspace_name", type=str, required=False, help="Name of the AzureML workspace")
+        sub_parser.add_argument(
+            "--aml_config_path",
+            type=str,
+            required=False,
+            help=(
+                "Path to AzureML config file. If provided, subscription_id, resource_group and workspace_name are"
+                " ignored"
+            ),
         )
-        ml_client.begin_create_or_update(cluster_basic).result()
-        logger.info(
-            "Successfully created compute: %s at %s with vm_size:%s and "
-            "min_nodes=%d and max_nodes=%d and idle_time_before_scale_down=%d",
-            compute_name,
-            location,
-            vm_size,
-            min_nodes,
-            max_nodes,
-            idle_time_before_scale_down,
+        sub_parser.add_argument("--compute_name", type=str, required=True, help="Name of the new compute")
+        sub_parser.add_argument(
+            "--vm_size",
+            type=str,
+            required=False,
+            help="VM size of the new compute. This is required if you are creating a compute instance",
         )
-    elif is_delete:
-        logger.info("Deleting compute %s...", compute_name)
-        ml_client.compute.begin_delete(compute_name).wait()
-        logger.info("Successfully deleted compute: %s", compute_name)
-
-
-def get_ml_client(aml_config_path, subscription_id, resource_group, workspace_name):
-    if aml_config_path is not None:
-        if not Path(aml_config_path).exists():
-            raise ValueError(f"aml_config_path {aml_config_path} does not exist")
-        if not Path(aml_config_path).is_file():
-            raise ValueError(f"aml_config_path {aml_config_path} is not a file")
-        return MLClient.from_config(credential=get_credentials(), path=aml_config_path)
-    else:
-        if subscription_id is None:
-            raise ValueError("subscription_id must be provided if aml_config_path is not provided")
-        if resource_group is None:
-            raise ValueError("resource_group must be provided if aml_config_path is not provided")
-        if workspace_name is None:
-            raise ValueError("workspace_name must be provided if aml_config_path is not provided")
-        return MLClient(
-            credential=get_credentials(),
-            subscription_id=subscription_id,
-            resource_group_name=resource_group,
-            workspace_name=workspace_name,
+        sub_parser.add_argument(
+            "--location",
+            type=str,
+            required=False,
+            help="Location of the new compute. This is required if you are creating a compute instance",
+        )
+        sub_parser.add_argument("--min_nodes", type=int, required=False, default=0, help="Minimum number of nodes")
+        sub_parser.add_argument("--max_nodes", type=int, required=False, default=2, help="Maximum number of nodes")
+        sub_parser.add_argument(
+            "--idle_time_before_scale_down", type=int, required=False, default=120, help="Idle seconds before scaledown"
+        )
+        sub_parser.set_defaults(func=ManageAMLComputeCommand)
+
+    def run(self):
+        try:
+            from azure.ai.ml.entities import AmlCompute
+        except ImportError:
+            raise ImportError(
+                "azure-ai-ml is not installed. Please install azure-ai-ml packages to use this script."
+            ) from None
+
+        logger.info("Running create new compute script...")
+
+        ml_client = self.get_ml_client(
+            self.args.aml_config_path, self.args.subscription_id, self.args.resource_group, self.args.workspace_name
         )
 
+        if self.args.create:
+            logger.info("Creating compute %s...", self.args.compute_name)
+            if self.args.vm_size is None:
+                raise ValueError("vm_size must be provided if operation is create")
+            if self.args.location is None:
+                raise ValueError("location must be provided if operation is create")
+            cluster_basic = AmlCompute(
+                name=self.args.compute_name,
+                type="amlcompute",
+                size=self.args.vm_size,
+                location=self.args.location,
+                min_instances=self.args.min_nodes,
+                max_instances=self.args.max_nodes,
+                idle_time_before_scale_down=self.args.idle_time_before_scale_down,
+            )
+            ml_client.begin_create_or_update(cluster_basic).result()
+            logger.info(
+                "Successfully created compute: %s at %s with vm_size:%s and "
+                "min_nodes=%d and max_nodes=%d and idle_time_before_scale_down=%d",
+                self.args.compute_name,
+                self.args.location,
+                self.args.vm_size,
+                self.args.min_nodes,
+                self.args.max_nodes,
+                self.args.idle_time_before_scale_down,
+            )
+        elif self.args.delete:
+            logger.info("Deleting compute %s...", self.args.compute_name)
+            ml_client.compute.begin_delete(self.args.compute_name).wait()
+            logger.info("Successfully deleted compute: %s", self.args.compute_name)
 
-def get_credentials():
-    logger.info("Getting credentials for MLClient")
-    try:
-        credential = AzureCliCredential()
-        credential.get_token("https://management.azure.com/.default")
-        logger.info("Using AzureCliCredential")
-    except Exception:
+    @classmethod
+    def get_ml_client(cls, aml_config_path: str, subscription_id: str, resource_group: str, workspace_name: str):
         try:
-            credential = DefaultAzureCredential()
-            # Check if given credential can get token successfully.
-            credential.get_token("https://management.azure.com/.default")
-            logger.info("Using DefaultAzureCredential")
-        except Exception:
-            # Fall back to InteractiveBrowserCredential in case DefaultAzureCredential not work
-            credential = InteractiveBrowserCredential()
-            logger.info("Using InteractiveBrowserCredential")
+            from azure.ai.ml import MLClient
+        except ImportError:
+            raise ImportError(
+                "azure-ai-ml is not installed. Please install azure-ai-ml packages to use this script."
+            ) from None
+
+        if aml_config_path is not None:
+            if not Path(aml_config_path).exists():
+                raise ValueError(f"aml_config_path {aml_config_path} does not exist")
+            if not Path(aml_config_path).is_file():
+                raise ValueError(f"aml_config_path {aml_config_path} is not a file")
+            return MLClient.from_config(credential=cls.get_credentials(), path=aml_config_path)
+        else:
+            if subscription_id is None:
+                raise ValueError("subscription_id must be provided if aml_config_path is not provided")
+            if resource_group is None:
+                raise ValueError("resource_group must be provided if aml_config_path is not provided")
+            if workspace_name is None:
+                raise ValueError("workspace_name must be provided if aml_config_path is not provided")
+            return MLClient(
+                credential=cls.get_credentials(),
+                subscription_id=subscription_id,
+                resource_group_name=resource_group,
+                workspace_name=workspace_name,
+            )
 
-    return credential
+    @staticmethod
+    def get_credentials():
+        try:
+            from azure.identity import AzureCliCredential, DefaultAzureCredential, InteractiveBrowserCredential
+        except ImportError:
+            raise ImportError(
+                "azure-identity is not installed. Please install azure-identity packages to use this command."
+            ) from None
 
+        logger.info("Getting credentials for MLClient")
+        try:
+            credential = AzureCliCredential()
+            credential.get_token("https://management.azure.com/.default")
+            logger.info("Using AzureCliCredential")
+        except Exception:
+            try:
+                credential = DefaultAzureCredential()
+                # Check if given credential can get token successfully.
+                credential.get_token("https://management.azure.com/.default")
+                logger.info("Using DefaultAzureCredential")
+            except Exception:
+                # Fall back to InteractiveBrowserCredential in case DefaultAzureCredential not work
+                credential = InteractiveBrowserCredential()
+                logger.info("Using InteractiveBrowserCredential")
 
-if __name__ == "__main__":
-    main()
+        return credential
```

## Comparing `olive/workflows/snpe/convertquantize/__main__.py` & `olive/cli/run.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
-import argparse
+from argparse import ArgumentParser
 
-from olive.workflows.snpe import convertquantize
+from olive.cli.base import BaseOliveCLICommand
 
-if __name__ == "__main__":
-    parser = argparse.ArgumentParser("SNPE workflow: Convert and Quantize")
-    parser.add_argument("--model", type=str, help="Path to the model", required=True)
-    parser.add_argument("--config", type=str, help="Either the path to json config file", required=True)
-    parser.add_argument("--data", type=str, help="Path to the data", required=True)
-    parser.add_argument(
-        "--input_list_file",
-        type=str,
-        help="Name of the input list file. Optional if 'input_list.txt'",
-        required=False,
-        default="input_list.txt",
-    )
-    parser.add_argument(
-        "--output_dir",
-        type=str,
-        help="Path to the output directory. Optional if same as model directory",
-        required=False,
-    )
-    parser.add_argument(
-        "--output_name",
-        type=str,
-        help="Name of the output model (without extension). Optional if same as model name",
-        required=False,
-    )
 
-    args = parser.parse_args()
+class WorkflowRunCommand(BaseOliveCLICommand):
+    @staticmethod
+    def register_subcommand(parser: ArgumentParser):
+        sub_parser = parser.add_parser("run", help="Run an olive workflow")
+        sub_parser.add_argument(
+            "--package-config",
+            type=str,
+            required=False,
+            help=(
+                "For advanced users. Path to optional package (json) config file with location "
+                "of individual pass module implementation and corresponding dependencies. "
+                "Configuration might also include user owned/proprietary/private pass implementations."
+            ),
+        )
+        sub_parser.add_argument("--run-config", "--config", type=str, help="Path to json config file", required=True)
+        sub_parser.add_argument("--setup", help="Whether run environment setup", action="store_true")
+        sub_parser.add_argument(
+            "--data-root", "--data_root", help="The data root path for optimization", required=False
+        )
+        sub_parser.add_argument(
+            "--tempdir", type=str, help="Root directory for tempfile directories and files", required=False
+        )
+        sub_parser.set_defaults(func=WorkflowRunCommand)
 
-    convertquantize(**vars(args))
+    def run(self):
+        from olive.common.utils import set_tempdir
+        from olive.workflows import run as olive_run
+
+        set_tempdir(self.args.tempdir)
+
+        var_args = vars(self.args)
+        del var_args["func"], var_args["tempdir"]
+        olive_run(**var_args)
```

## Comparing `olive_ai-0.5.2.dist-info/LICENSE` & `olive_ai-0.6.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `olive_ai-0.5.2.dist-info/METADATA` & `olive_ai-0.6.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olive-ai
-Version: 0.5.2
+Version: 0.6.0
 Summary: Olive is an easy-to-use hardware-aware model optimization tool that composes industry-leading techniques across model compression, optimization, and compilation.
 Home-page: https://microsoft.github.io/Olive/
 Download-URL: https://github.com/microsoft/Olive/tags
 Author: Microsoft Corporation
 Author-email: olivedevteam@microsoft.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
@@ -52,14 +52,17 @@
 Requires-Dist: onnxruntime-gpu ; extra == 'gpu'
 Provides-Extra: inc
 Requires-Dist: neural-compressor ; extra == 'inc'
 Provides-Extra: lora
 Requires-Dist: accelerate ; extra == 'lora'
 Requires-Dist: peft ; extra == 'lora'
 Requires-Dist: scipy ; extra == 'lora'
+Provides-Extra: nvmo
+Requires-Dist: nvidia-modelopt ~=0.11.0 ; extra == 'nvmo'
+Requires-Dist: onnx-graphsurgeon ; extra == 'nvmo'
 Provides-Extra: openvino
 Requires-Dist: openvino ==2023.2.0 ; extra == 'openvino'
 Requires-Dist: nncf ==2.7.0 ; extra == 'openvino'
 Provides-Extra: optimum
 Requires-Dist: optimum ; extra == 'optimum'
 Provides-Extra: ort
 Requires-Dist: onnxruntime ; extra == 'ort'
```

## Comparing `olive_ai-0.5.2.dist-info/NOTICE.txt` & `olive_ai-0.6.0.dist-info/NOTICE.txt`

 * *Files identical despite different names*

## Comparing `olive_ai-0.5.2.dist-info/RECORD` & `olive_ai-0.6.0.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,244 +1,261 @@
-olive/__init__.py,sha256=rMh3IndQNs7Kpguw0x6VP4CDSLbFKe3MEmhVwBAJ9po,608
-olive/cache.py,sha256=8fTz93_iPpzM6UGr0y04fhVw-Xpip4dBLxVKxHM_2kQ,9998
+olive/__init__.py,sha256=UVgBoZjtviTnsu-88Bnn2VjJmtk7D31RujQITLCTEv8,608
+olive/__main__.py,sha256=Ll8pwEp35R43A4ZvM8glzkONJN81ho5XilOfkB-BddY,488
+olive/cache.py,sha256=hQgmUOwe1DtxJoLSZlsYe5pbIC70w78gkJ6WM3T5OO8,10695
 olive/constants.py,sha256=vHZgfVTreESqTShRFI9dmx9IfdLlfHL3fegwmYQzNE0,1162
 olive/logging.py,sha256=VcJnHwDqDsWuw46HqgMOCfCgCNi2axFQYaxVFhrd8lI,2626
-olive/olive_config.json,sha256=cZQv-qU4CA2A36QHHxqKpN-pXGUKKJdFMMHjuvlJ_Dw,8038
+olive/olive_config.json,sha256=hYBYhVdwUg0qd6ovYBGNB12CTUHku5qIUbVxWt-2XI8,8567
 olive/package_config.py,sha256=ZsgHwNHGwjh0zIzlZn7qBmLiz8yB9nXXfA6azwh_S28,1406
-olive/resource_path.py,sha256=dPBcwg9KqYib7N75O8-ZT-_MxlXqGdHC2kiY2oDzLiU,22999
-olive/auto_optimizer/__init__.py,sha256=DC-U5sReV5weVF-A6Rn2-OA9BGxeBpYpg1VBpNrygCw,5181
-olive/auto_optimizer/regulate_mixins.py,sha256=X7G3UOOSH7Z9ZhD3QfCVpfIMtWksP_84UlK6ijItjJQ,5871
+olive/resource_path.py,sha256=yKfx0lvIfqB4JZZDkDZBw-vkvn7LqhsP2yvi1FDZ6_E,23380
+olive/auto_optimizer/__init__.py,sha256=_sS6KXyC1jEUr7k3B4ZJlfhrBam9MoaAPvVuzY0nH-M,5170
+olive/auto_optimizer/regulate_mixins.py,sha256=_rj-xOfQR35Wmez1VjH4VfezL7oCo0JFeCYaQIR_jrY,5918
 olive/auto_optimizer/template_mapping.py,sha256=6wgYD_X61GilGYRVCEvkwcYXSuhEWokgsdBKNxujaiQ,3615
 olive/auto_optimizer/config_template/opt_level_passes.yaml,sha256=A2ZE_u8mrWQ1I30tcHuft7FdY70eWFxuD6r_VMEgn90,1171
 olive/auto_optimizer/config_template/pass_capability.yaml,sha256=FfmafalzQSkImDnqCnJvZCgqXaDdZlMh9J2VIClWhOo,2062
 olive/azureml/__init__.py,sha256=WSNxt3l4lkWA_0vhw1ED4I7KOO0mnAuHwSgFYqbq0Lg,247
 olive/azureml/azureml_client.py,sha256=8IpXgGImz9WLNHTyjHbnK4DjXR_vkDXLVfFtaWNwbrw,6699
+olive/cli/__init__.py,sha256=WSNxt3l4lkWA_0vhw1ED4I7KOO0mnAuHwSgFYqbq0Lg,247
+olive/cli/base.py,sha256=Uw60B0JEcK4e7E3TRosMcCMGL_Qan29GSa0zeiQ4GS4,630
+olive/cli/configure_qualcomm_sdk.py,sha256=_uV8RiwUSIuD-Mwc-NBMfKXneTbmxDc9qKXWia4i66g,1256
+olive/cli/export_adapters.py,sha256=lX7DC3t1gFce4rB8YGowVqFVaBUr4Oi_284UK3BfQ88,6236
+olive/cli/launcher.py,sha256=t8E4CsHbIX1m_qLDYeXwRF5abdKMa5PjPvS9B7bM48U,2348
+olive/cli/manage_aml_compute.py,sha256=CcW0JLPRDxMZ-MdSXuuhirETFpazTx5uaBjwJ0o4zi0,7275
+olive/cli/run.py,sha256=UDFTEv4sQ4hhRDQwgWHtgUXitV80qH76o0T9ecLtpiE,1831
 olive/common/__init__.py,sha256=WSNxt3l4lkWA_0vhw1ED4I7KOO0mnAuHwSgFYqbq0Lg,247
 olive/common/auto_config.py,sha256=yNfcSrh1z_gQLSsiYFn63k5x-qT33t-S1y97J42uvnA,3430
-olive/common/config_utils.py,sha256=57gPIim-aDFScw3AamYnRZccXz8sc4KC_uOAUfvTObQ,10881
+olive/common/config_utils.py,sha256=bcrYy3wsEDvLb2r-rchw0tCHF9cy4Z6foG9CeGAWGkw,10422
 olive/common/import_lib.py,sha256=KrWnGR2Pe1RWfOqe3DL96Aq0O8zXzYHxJc0d2zgMdlU,1488
-olive/common/ort_inference.py,sha256=oI1swvgxWi4BR_ENKiOnn030GFcCTge7MIto414mZN4,18360
+olive/common/ort_inference.py,sha256=8q6L-WRanufedENEEitVWM1U8rEyTK3uf2sK_Gt4Hms,18372
 olive/common/pydantic_v1.py,sha256=vNddf08_5YT58wfDL3A38TaniE6xku-CMa7rIdesOZ8,765
 olive/common/user_module_loader.py,sha256=FfRLFiEvGw2yT9EKULc4eIr4a0CP_lGms2SkXNg0xa0,1809
-olive/common/utils.py,sha256=tG0WIdwp0Y0FUkHwQlfKIduP5YdOHp76mDYEmd2XS_Y,11789
+olive/common/utils.py,sha256=DkswFFJaYAcbrq4QQnoPHW_fYYkJjq7XOhORnQeEH4c,13009
 olive/data/__init__.py,sha256=e6E8AVlCoJ-LNfbshkiyOVopkfgUmg6dRo9LH51Mafw,345
-olive/data/config.py,sha256=Ro9bPuIHe6V1mhm9DcdHggq2gdu1_2bbAJ8krwewOIc,10680
+olive/data/config.py,sha256=rLNW5f4i16ZWvAQLoWolglCuMvAGb-a0po8Rlpbc-PI,10636
 olive/data/constants.py,sha256=v4_EcRT473PBqIJDJW54HiMWP_OboMKILUd7cf4MwR4,1443
 olive/data/registry.py,sha256=hZi_GKCKWu9SbxpMiJ9OR7q-yNKIunpTUzdXY9cPipI,8119
 olive/data/template.py,sha256=wJQGctfoMiJGIf5gB1Kp2kbJlofYujSg9vl3KGO-47E,3573
 olive/data/component/__init__.py,sha256=fo0PIFNXx16c4CMOTlxaIj8UlZvApJ3-Pca18AK3qQY,444
 olive/data/component/dataloader.py,sha256=beCT0mojWX09OGPyL2cR2pUSXMRv_kHohHDv4tJwj1s,1955
-olive/data/component/dataset.py,sha256=aNlwrIEJPplJcJaRKHX7P0EByfU4PxBHh2dgA1J-mxo,10679
+olive/data/component/dataset.py,sha256=t6XuLYvcUvHm1R6Aci2tNRti81PpD7SC_Yuj4T1fLFU,10505
 olive/data/component/load_dataset.py,sha256=rVZM2ZlZcu_o48-TtEV9kL_55G_K72_6CBcgWSnNWp4,1928
 olive/data/component/post_process_data.py,sha256=mUNokrUnKH_2GrQpLtXUSbDRWHosHC29kC0IpfbbCU8,2256
 olive/data/component/pre_process_data.py,sha256=nrzmMxKHlRu8V3C4E88sqyVrtCe3_99R_Q-vFv8aXss,11446
 olive/data/component/text_generation.py,sha256=gxaKqJAoUpR84WVJUUuBFsSkXRV6MBgIX9pAkV03Vck,29278
 olive/data/container/__init__.py,sha256=LDGROQwmhlEeOzEtSRG0UWushVKko-gu_EvHw0g6XJg,480
 olive/data/container/data_container.py,sha256=CJ8HBjcoDPAOX-zVUaOtS7wJGSnrkvNK5-QkSjSho1E,3385
 olive/data/container/dummy_data_container.py,sha256=4C_mhjK1qUKaytBrCzHR3TUfYYvQxDtgOXP2iRMhPwk,1159
 olive/data/container/huggingface_container.py,sha256=C1nMtdmVkDDviL-jyY5_lK9aN2dzRMcAKASoQ9Iysjk,1690
 olive/data/container/raw_data_container.py,sha256=YqjbFWH6KI51_TEI_YFBjjDMFKwKMx2M7SN8jbbBZYI,1721
 olive/engine/__init__.py,sha256=sK_oyURVPbwXYIzb3PcUG3Lh0dUZJ-Ot7SWL9laJojk,442
 olive/engine/config.py,sha256=LBDTo3OtIu__EMl3xKys0C-FRO1QKX92rf0Q7Ognyew,1199
-olive/engine/engine.py,sha256=LQvsYIqYhEQzE5CNQ-kw39KQ5_e8vOeJqy8ozedwths,45969
-olive/engine/footprint.py,sha256=C_s1OyI9yt8pal76WQ13WbHfu-B1oD0oKb3pvjzdvJI,17410
+olive/engine/engine.py,sha256=m2nw7ZtSiQP0qNDaB7YsgKlddRrTXk9P5owyslXQgto,46570
+olive/engine/footprint.py,sha256=WKXOVnXPv2dsMT4ANNd4WU7f87GrqE07SPA41B3CADk,17415
 olive/engine/packaging/__init__.py,sha256=WSNxt3l4lkWA_0vhw1ED4I7KOO0mnAuHwSgFYqbq0Lg,247
-olive/engine/packaging/packaging_config.py,sha256=LImhOApwoSPlKNV7dbVC1BenR2I_-M9H6td5T4TZAzo,1642
-olive/engine/packaging/packaging_generator.py,sha256=y9we8MVWV5H3V6uIZ0NR5f63Am27YFVmt_ZbUx5r3DA,19748
+olive/engine/packaging/packaging_config.py,sha256=DkTLy3_irN7_txSvqmleD_vdHCAnN9mZcGoLm19IH2o,3285
+olive/engine/packaging/packaging_generator.py,sha256=YgK4NH49W6uVH35gs1vv1VHkUmxUo08YI68L91ZLvUk,32569
+olive/engine/packaging/sample_code/GenAIOnnxModel/cpp/CMakeLists.txt,sha256=CV7bun569HXhDiLeJjH4LXhnCodNCwNTK1YymCHITeI,1325
+olive/engine/packaging/sample_code/GenAIOnnxModel/cpp/README.md,sha256=VcLdE6k_uc4rlVafQLt1R3LfGWFL1HLk2P0hmW-55zA,438
+olive/engine/packaging/sample_code/GenAIOnnxModel/cpp/code_sample.cpp,sha256=MODhjkL7GfMLOWyD5tU2Q0EDHGABctN1JGBcqjY6330,4097
+olive/engine/packaging/sample_code/GenAIOnnxModel/cs/README.md,sha256=oQvE5t4dGGtzjoMxJaCoymMkP6x87-Y6-gIpsrtB2bY,184
+olive/engine/packaging/sample_code/GenAIOnnxModel/cs/code_sample.cs,sha256=tWlmrZN6ItD5hyy0OI23G9xOz35blicIjovXLrLi_es,3587
+olive/engine/packaging/sample_code/GenAIOnnxModel/cs/olive-genai-cs-sample.csproj,sha256=8dX31jwpNoMYYgSWbn0704b15-Ywf6-zPRsQHFkUNQk,652
+olive/engine/packaging/sample_code/GenAIOnnxModel/cs/olive-genai-cs-sample.sln,sha256=SKbePeUn_Rj6Kygxl6l1C6X-ZKwt1HHFnO7igRpN8n8,1122
+olive/engine/packaging/sample_code/GenAIOnnxModel/python/README.md,sha256=BV_4NS_tMW7aWLCDQ8JIlafIgi65yNIpXx3DTlZn6_g,840
+olive/engine/packaging/sample_code/GenAIOnnxModel/python/code_sample.py,sha256=92ygY6qq1V0jh9HVHrs5YwE3niYlJ_jHRCV0KAe9x18,5570
 olive/engine/packaging/sample_code/ONNXModel/cpp/README.md,sha256=JnLAiNYgEZCvsP0rwG5rTOwn_px6XeLFjrchXUDWO4s,1588
 olive/engine/packaging/sample_code/ONNXModel/cpp/code_sample.cpp,sha256=4FejpIKRXN9-9LuWvkoFGMCgnuhRZxFA6m_9E6yrNQs,4990
 olive/engine/packaging/sample_code/ONNXModel/cs/README.md,sha256=V7tDnmXiisTAbiCec7Us-pUvI3XuJEc6EE1cO2WXt0A,1590
 olive/engine/packaging/sample_code/ONNXModel/cs/code_sample.cs,sha256=eZhEe9P2psAFeT_3Kz-WqHjkNRD-raaW3eILw2Gs1Cw,4991
 olive/engine/packaging/sample_code/ONNXModel/python/README.md,sha256=z2awTxd97vnQwNuQ08WOid4MiuGQghTJ3EI4Fo5Zb38,2296
-olive/engine/packaging/sample_code/ONNXModel/python/code_sample.py,sha256=HYIiEfvQObTDI6Bh3DP3fSbwvEp9PQ7YcdX8YGTGzw8,2545
+olive/engine/packaging/sample_code/ONNXModel/python/code_sample.py,sha256=HJf4eDxWRTxfZgau9g9kUvFz0ObKXpZEbRT1LnRsc0w,2557
 olive/evaluator/__init__.py,sha256=WSNxt3l4lkWA_0vhw1ED4I7KOO0mnAuHwSgFYqbq0Lg,247
-olive/evaluator/accuracy.py,sha256=HV17zTBx2U-H9BkM9cF7EbLWkOUyzHkySWX77mb9DaU,6473
-olive/evaluator/metric.py,sha256=yE3_zK_JanrxKM5LBhPb1zNJwgIt1sofW-4BxhjT6n0,8723
-olive/evaluator/metric_backend.py,sha256=2Trmgtcet7bmJTCKb3jDYzNYdLBwtY4xqnpDGG-O6po,4461
-olive/evaluator/metric_config.py,sha256=HDA9Ek4PgtY3QQj5tMGVHjqu-2d64cUEIOscTLqQkoI,4395
-olive/evaluator/olive_evaluator.py,sha256=QRrora4pTGWP62H020g2dm4c40T6GwdzbNnbWoqmfKg,47694
+olive/evaluator/accuracy.py,sha256=1gXrwujIz9EMa0v_cCKQNvPhq9kQ31rCqtObrTrqBQ4,6368
+olive/evaluator/metric.py,sha256=upJD_00t2Il8ffKQd-S0nlNmDetLHRG2G3GLLgh3elU,7343
+olive/evaluator/metric_backend.py,sha256=e-29m8LGm0C1HTjY-09MPPyEmJncR1PF-4bh30EXvPQ,4548
+olive/evaluator/metric_config.py,sha256=tqSYI5D14lDY0GWpQbqmBTwHkoQjfrHxDLAfvn6UYjo,4523
+olive/evaluator/metric_result.py,sha256=5xYQJNjhnUL36QoNYFlvSX4vhP7XGJMG24kvpFSDVbg,1702
+olive/evaluator/olive_evaluator.py,sha256=zrtlV9gt1bDFluqnizYHfulHVNGsmvJ11pK17pnz7tw,47925
 olive/exception/__init__.py,sha256=ycjIjR_iwg4ZcCuRtbHZpEbIw-4RzlurOa6o5tz8NA0,592
 olive/hardware/__init__.py,sha256=89KKeZDoW0jvqeOOrgaLoGFKZxVhh2jFLbAioi0hEi0,621
-olive/hardware/accelerator.py,sha256=2i_qGlWhxCsVVmRTnclDr7X_4jkgGDnjRQLFSBQuk6g,15059
-olive/hardware/constants.py,sha256=ZzHG-NRYy6L_XM-CSKSxv7pxcGLyXrKzLapqtafKmV0,1273
+olive/hardware/accelerator.py,sha256=ijmxkMbR29cJrnK4Anq7xRsucqAGmB6mbxkDllGAoWU,6688
+olive/hardware/constants.py,sha256=cZuJFFPgLoyOD5dcO7JtNPmqZWJeeZ-MdxJQBQefhnY,1304
 olive/model/__init__.py,sha256=ogykDHRcG2bcvxHJMYLzJb30SbpNmtDpzbIBfboVVV4,451
-olive/model/config/__init__.py,sha256=HqUlWk6oUdFksNgoz9z77mgE8r8Xlb2DkZl2iub40yw,482
-olive/model/config/hf_config.py,sha256=ZGMo6BnTMs7M4WfqcDmqTO-Wbuj-NgG8S6IKcvBZuPw,10950
-olive/model/config/io_config.py,sha256=NF3LMWwwaNkSnT7iShk04aISRVJ3T4g_5odt-t8l08A,4843
+olive/model/config/__init__.py,sha256=09QoAcTzAZ4f5lw9vwf9LloKmQ3W7SNUIsmsxgl_vR4,758
+olive/model/config/hf_config.py,sha256=XFLFblNZtw25al2sfiI1IF1SZ64X61Hs6H9VeXtzjnA,11244
+olive/model/config/io_config.py,sha256=ZEdoQdSMHgJPRXLg_IqATnnPeF-jOwn5Pc5jVAU8A-A,9113
+olive/model/config/kv_cache_config.py,sha256=p1Eql0S9hBRUhvppNgN_f1DJ-Xk1QLz53oUbLCQgknU,4567
 olive/model/config/model_config.py,sha256=X-kPWyMmHjB3WI6KUV7fgze2o3sS93SpiMsVpyqCbJk,3943
 olive/model/config/registry.py,sha256=PFa1p9xVBRHduXDa8UyzjXH8M6YSJ91nSyXa5e7Z8aE,1045
 olive/model/handler/__init__.py,sha256=dAx_DTEF4JOGePcPECDBqFWnkh1lHxAU7pYBrsxa9Ko,1139
-olive/model/handler/base.py,sha256=lPZOI9fAkCXpXZp4Yzi8xIhAtqDbR-Izccq5UYqtNiQ,3190
+olive/model/handler/base.py,sha256=j4MLbjtyENNUN0Xd5dZfckmQ1FFvrstgMTlU_iluUGk,3533
 olive/model/handler/composite.py,sha256=HaKW30CPj6G_nqFbWDQoo-DEHnBBSk1e4vS550Adc68,4461
-olive/model/handler/onnx.py,sha256=NOl-g6T2lIuInehFFdO88b8__TzzkCCkzcylyOqvd7c,10069
+olive/model/handler/onnx.py,sha256=GGNQmpVl75m3gGmOSR2BePFyKtfStDCufTU98OB8ZcM,10053
 olive/model/handler/openvino.py,sha256=JIcZsjZ1wrsUgHVE4sYb8mwXnoS2zN2wGV4OZdE7Ajw,3556
-olive/model/handler/pytorch.py,sha256=6WunjjQElAa1iW_sOeIpbv0mUtWrgXhqinHjePBJOCo,16898
-olive/model/handler/qnn.py,sha256=77nhGBAa1KL5mxGWOOmNJcV7vkCqsLoina_5YWrq23M,4704
-olive/model/handler/snpe.py,sha256=QRxfGSQ6FrPCZGtQXjfRKhHHMvvFbuGq_j1Y_AL-IVE,2597
+olive/model/handler/pytorch.py,sha256=rDs4gwQwew1qAGQ1pqMFFIhZDmNTenS2qdHy-49xcs0,17284
+olive/model/handler/qnn.py,sha256=NxekEPdEZ-4V42LGQlm8CXnLLu6ZPkR6nckpcMVtJ2M,4489
+olive/model/handler/snpe.py,sha256=XCEJVw_NeENFNaOR8nHSGau9XoUNWR5rMNm5_o9CeDM,2898
 olive/model/handler/tensorflow.py,sha256=dLLkfXrpuxG0ab93p7k1c3M0c_Kjjub78Rde__lox2o,1474
-olive/model/handler/mixin/__init__.py,sha256=HnupHTH3k-xB5XlpRjx8uuRQdKTiRX1tFu_vhb-xN4w,936
+olive/model/handler/mixin/__init__.py,sha256=i1x6_5o_XKdxoy5EdXVOoEKdtFrOvXt7I0jO0dixgdU,1106
 olive/model/handler/mixin/composite.py,sha256=qpQ41-7XsIz2l5X8ab2-gt6OZJDPZUInacW-1H9HopQ,418
-olive/model/handler/mixin/dummy_inputs.py,sha256=U-e257lcwqEkLgNTMPO5VczLU92Le7w-CXdBvZh5DDw,3021
-olive/model/handler/mixin/hf_config.py,sha256=hiffIeyfFDJ1klhOwJ8dgRgq6-5ivOMtB2Lio1PLNXc,3967
-olive/model/handler/mixin/io_config.py,sha256=hOIOJjeEhXxGgfUeKovKKS4NjpOm5tX4T2QnZntzPxE,613
+olive/model/handler/mixin/dummy_inputs.py,sha256=7gDrYWdW6VyhbX1zizbXxx6CMB9w9ZL3JrlTqePrlJk,3010
+olive/model/handler/mixin/hf_config.py,sha256=VM-LZV4Ed7RPF8gkWJk2H38FfBiUR2k4Kv8j59IQM_0,5993
+olive/model/handler/mixin/io_config.py,sha256=ul5VbjOb0SvsrefgcoWZmj8qOSEjAKn4Hd71GVI8pi8,625
 olive/model/handler/mixin/json.py,sha256=LnMzqAbDK7MBJucxVXxq400WxFq9pO6Xe5u69UQ73QI,1472
+olive/model/handler/mixin/kv_cache.py,sha256=qauQejGCAB_fbXqeJFG99ZGOGAdHb4rNlMOMNuoXLwU,4183
+olive/model/handler/mixin/mlflow.py,sha256=cRz9vi5ne45lpefI14oF6DTrS3u5eN7CL48C-nifB1s,2242
 olive/model/handler/mixin/onnx_ep.py,sha256=bZ4xKLSDpdR-AZaB2w_785IRU_qStLqs-G9eTPNQeJA,1402
 olive/model/handler/mixin/onnx_graph.py,sha256=PwVntvtKZuxFTPjssee_Hbc-xUrLTUBkbsDEtozuyHA,3946
 olive/model/handler/mixin/resource.py,sha256=VvVsto2k1AfNSzH7zxdgpYvt6gDiTcWlFsaPelA3M_M,2998
-olive/model/utils/__init__.py,sha256=OViqJhejw6VYFg7BO_zhp2WeCJzr9YPjUXumynwhARs,609
-olive/model/utils/hf_mappings.py,sha256=HJLxWMhTXSCmYW9NnCsn4Wr9PmGO39i2H9xEdrZ4L4U,3091
+olive/model/utils/__init__.py,sha256=cCA3Oi_yBKPqbtB2QSLJWlRgAKEfm5Vv7DM0MOFXDV4,690
+olive/model/utils/hf_mappings.py,sha256=mNW6gnTeZMnbqyPZqSswyMJZezEqhSA2vW2fM4TwxPs,3228
 olive/model/utils/hf_onnx_config.py,sha256=5njt4Ko5NCL_3Ipy0wdUwvjmaxLmwdACT5iuNWXnw9g,4517
-olive/model/utils/hf_utils.py,sha256=8LPvDe50b_Eaf6qdmawaGdLOVFwE7eKvmtTXlVUsBo0,8183
+olive/model/utils/hf_utils.py,sha256=teY55fzD0ENy_AtKE7nZ568TJwHkqMVbfefa_PgtCPU,10817
 olive/model/utils/onnx_utils.py,sha256=zo0CtDRWOyStOKMHJZdL7Ad5ocMgN9vuui2CFtY-dM0,3467
 olive/model/utils/path_utils.py,sha256=lu4r8V_PjCyFrlzxfAUZrRKAa3VhV67o9_4noYE1V2g,1510
-olive/passes/__init__.py,sha256=kzwYdsbpTo9ipqKgoTRf1hV-Jr2OnJlqdg_3-3iiECM,499
-olive/passes/olive_pass.py,sha256=GjmwtSVu8ZXuJxmyESxczmvs6ALpR58lm6qadIj-7QI,19895
-olive/passes/pass_config.py,sha256=Ijdjp_1NAtMkhrM7jE-024aTdJF98CQsRTtb0xHp8hw,6139
+olive/passes/__init__.py,sha256=fwEb793gSNRrN1TN7d2Bnp0iwhBARvrFK7EXL1lamiA,515
+olive/passes/olive_pass.py,sha256=iiexIsmL5cGByp4SXsxxEiix4niLO6yICNSpNHUd8WI,23315
+olive/passes/pass_config.py,sha256=gDExIGFaY6A7CZxn8fUdm9Wi1C6VeNRKgt6J9aumZog,6143
 olive/passes/onnx/__init__.py,sha256=WSNxt3l4lkWA_0vhw1ED4I7KOO0mnAuHwSgFYqbq0Lg,247
 olive/passes/onnx/append_pre_post_processing_ops.py,sha256=pYwd1LeAFym37hLknAIi90UqLTeCCzLRuzhbJVfUifQ,8408
 olive/passes/onnx/bnb_quantization.py,sha256=s9SfMEHXizkwP85VBpmPYxPiqTnCgyMA-7Sj0FqzXmI,5524
 olive/passes/onnx/common.py,sha256=lmPktG3KFd9b_akPtnvUXgkEr7lKtlANkv4zHMxXmXE,7639
-olive/passes/onnx/conversion.py,sha256=v2lDq-_T3P7R0_mxSDsOJieMtPd6ZAUjGMIr65i7hn8,27526
+olive/passes/onnx/conversion.py,sha256=50FGDch9McyhPdozmmP3DjCx776-LhW0OLqON1723vs,28894
 olive/passes/onnx/dynamic_to_fixed_shape.py,sha256=Qf9WEa088IZgFddNX-aFANEy_2N6aWaHXg9-Bwo5Qqc,4862
-olive/passes/onnx/extract_adapters.py,sha256=cG4nuifwAXOSSDu6EC2GxcPksbRcYytjzsoQ6dMRXx4,14055
-olive/passes/onnx/float16_conversion.py,sha256=zzBB4q8I_MXExjwVJTFD_W4KGMtAJRxowwU5sEqKrRY,3090
-olive/passes/onnx/genai_model_exporter.py,sha256=IMhlvLHuOB_LLiLHrp2aKgFWCpK1eoqMoOtNIY8bl4k,4556
-olive/passes/onnx/inc_quantization.py,sha256=hHKslRJsbxCemHQDtAqIKfldVRl4E25sOaglbEcCIzE,27096
+olive/passes/onnx/extract_adapters.py,sha256=uko20_qdTAjGKqZqUp0OMe3Q87aP6q8lZaR0yIEZpFI,15977
+olive/passes/onnx/float16_conversion.py,sha256=J37zcKVXKB4Cyieb5r9waMyT9ZmTVSRVLIk6C2MlxPA,3209
+olive/passes/onnx/float32_conversion.py,sha256=ACC43rOK6afXTLV8hwP_tiRfXe8y81aLN-fDCTs9HlE,4646
+olive/passes/onnx/inc_quantization.py,sha256=ucNHJNKdO6iRJ_cKK8XBcmvURTVpMvfZVIWaw-nfYLw,27158
 olive/passes/onnx/insert_beam_search.py,sha256=6hEavIrzEK8VoSzhrFp05hprSCKzNn6UFdjyHg_bkJU,15972
 olive/passes/onnx/merge_decoders.py,sha256=NNKKa0-FVa1vog_g-4LPSf916Zk3aFVA1wEVUhnj6tw,18495
 olive/passes/onnx/mixed_precision.py,sha256=RS7Rmaoknc76_0qdMw_tEnIdJxvlAIku7LHunjjj4oU,9054
+olive/passes/onnx/model_builder.py,sha256=PmEJK2Y2f9AXhoCbgRssDk-xCYoZgW_86LtLiO21bHg,10432
 olive/passes/onnx/model_optimizer.py,sha256=0l2BmghwWBCK-08F90TO7VY1swU6_AY3-LqVXyQCH-Q,10011
 olive/passes/onnx/moe_experts_distributor.py,sha256=GBdDgDpiTjWCVwHFnwmubZGxNJP8smz6KCqzTraJHiw,15752
-olive/passes/onnx/onnx_dag.py,sha256=P6_tPFH6zFxx2xxkjJYQK0uFDG6Q0EHMDBeny9enUrA,18666
+olive/passes/onnx/nvmo_quantization.py,sha256=rV7pC1aTNHWRbx2v_Rm6HbG1nV72AWRywxBmmfAFGBs,4749
+olive/passes/onnx/onnx_dag.py,sha256=4I1d_a0a9c3oMWJwhULj7GczQPPrztROmtkAhtD0dHI,18912
 olive/passes/onnx/optimum_conversion.py,sha256=HDcMkyrfeIFSvuQbD33YGzqS7A2JDn_B1zKJGUbDedk,6162
 olive/passes/onnx/optimum_merging.py,sha256=OSh2gSAOjXj_BIFX_NfRMWWlDPTHlKWmEjYIcAXhSps,3709
-olive/passes/onnx/perf_tuning.py,sha256=HaEHnIkQK5nVJe2dVwfhAvLi0jRE0LtQaznDj9tKKRc,29003
+olive/passes/onnx/perf_tuning.py,sha256=tM0BbKPzqcvxXwXeseuCytrBCCD6wvQarxZ5b-rW9y0,29116
 olive/passes/onnx/qnn_preprocess.py,sha256=C3KsKo7DpJP-L030LvVnoCzW1ax4CDefn03yRiCy8BM,5375
-olive/passes/onnx/quantization.py,sha256=JL971yrSgwuiTMPwgwQNPfuWb7F6TJrYTWzjZu-ZYcA,37566
-olive/passes/onnx/transformer_optimization.py,sha256=t-4W-l1NNENerO33IVFimZWaOnMkaYnabSZpiYnwTME,19292
-olive/passes/onnx/vitis_ai_quantization.py,sha256=Y6cZexKW6cLAaJ3Ii1L9cXdNwN0zeMIdsXiRFCJys8c,15105
+olive/passes/onnx/quantization.py,sha256=8eqTTDphviqRGxHTLNuU7zHalN5mnn7LA2H3g_pqGOs,37593
+olive/passes/onnx/transformer_optimization.py,sha256=9o3fI_eq6rUBruEyYRB6eeG2gZHA-PqiAeFfporxVys,19890
+olive/passes/onnx/vitis_ai_quantization.py,sha256=YzBDGuGDpxP3BaqCd2Stlj6fk3aGbhijlVAnclxhC2E,15135
 olive/passes/onnx/pipeline/__init__.py,sha256=hy6ZqdDw4q53FSvRAM5nh7dCOGt1ESZagOqThowBZAI,3239
 olive/passes/onnx/pipeline/step_utils.py,sha256=YxajZp5gVU0UVpHrbonNJwZL8CHiNI5TVpye0WGpIVw,8457
 olive/passes/onnx/vitis_ai/__init__.py,sha256=WcngHdIXOp4kglwsc_G4qqBKU-wsyNk94ibGQkSv-eU,508
-olive/passes/onnx/vitis_ai/calibrate.py,sha256=IXLi6rSAwJ4fX-POa9dwHSlwPYSKsXN62g7tdUat5CY,7762
-olive/passes/onnx/vitis_ai/quant_utils.py,sha256=5YrlKa3QLpCd8rgZ1uSnRFApXlH9tQ68J4RPASX73U0,15332
-olive/passes/onnx/vitis_ai/quantize.py,sha256=2p6fpiJ8WGxeMhH9h1rWo83ocfc9lHtp2fcrCnf3A2w,13580
-olive/passes/onnx/vitis_ai/quantizer.py,sha256=n8IK8jb3b7PIFDmBK1WCxzsq3LvWxCUUgoxgg2td4LI,36359
-olive/passes/onnx/vitis_ai/refine.py,sha256=BcB69YUImoFVaafwzrjG4wEd3xGbQyyCA-wF007Hs8c,18700
+olive/passes/onnx/vitis_ai/calibrate.py,sha256=o0InW6pWTQvbdewqhYFYTWiOr0o7SPQktAkBfrQqx-0,7778
+olive/passes/onnx/vitis_ai/quant_utils.py,sha256=wbEDKByWe1CDfjvnFwY594NwiiB7bnUqvF7T3_lYlCg,15723
+olive/passes/onnx/vitis_ai/quantize.py,sha256=_r4DjhuAaH4FyWtZTtkuhNCRrpU9fSd6efIWLYYTQGw,13588
+olive/passes/onnx/vitis_ai/quantizer.py,sha256=AikdRLH-KmBO5TymP5P9LaAIVWsE3VdZUPhySj6uSqk,66718
+olive/passes/onnx/vitis_ai/refine.py,sha256=f6sJxvuCCQa3bmOPzxPj0GEGqSsxc8gwRZR_65iA4yw,18750
 olive/passes/openvino/__init__.py,sha256=WSNxt3l4lkWA_0vhw1ED4I7KOO0mnAuHwSgFYqbq0Lg,247
 olive/passes/openvino/conversion.py,sha256=qFxo55aCHtIIe2w8TWU403QORZsr55BdgcJLxPbd9Fs,4555
-olive/passes/openvino/quantization.py,sha256=s-zPf2zId_ucfKwV3mhbP7bwKda6d6CY5XQ0IZ_WgAU,12610
+olive/passes/openvino/quantization.py,sha256=Yyqbf_U-OFcT0hc8WnO_L04y8b_qIEd8z6NAuGcpUMA,12637
 olive/passes/pytorch/__init__.py,sha256=WSNxt3l4lkWA_0vhw1ED4I7KOO0mnAuHwSgFYqbq0Lg,247
+olive/passes/pytorch/autoawq.py,sha256=bMfuSQSKCAr-GV816EH17vYWQNO5mMTAGt9dKopubv8,10184
 olive/passes/pytorch/cluster.py,sha256=wPZilm6bpu8_KvhVYUdy4fM9b1US3bE-3IWPqDqi9gs,7058
-olive/passes/pytorch/gptq.py,sha256=Ytq51gMdHVfOVJR0SCFlGnBMhvuH35CtIBNF9twgFJQ,9842
-olive/passes/pytorch/gptq_utils.py,sha256=oCTV62B4jmffUDVQm2ceBN4iY91cAhSntLn8EKF6jEM,11528
-olive/passes/pytorch/lora.py,sha256=ljq2FmlNvjL1asoZZtXhn-oWpfNEJFUTkgbHb5ZsHYI,48812
+olive/passes/pytorch/gptq.py,sha256=rYRiuSekFifxv9kvsQ7nO9PDZYQDMICd9C5sw0czAog,9834
+olive/passes/pytorch/lora.py,sha256=bqCL-FQjuU32kFZISuH45-7BWEV1Ys_SoPBe98MclBU,50163
 olive/passes/pytorch/pytorch_lightning_utils.py,sha256=JyHsdwapI9Z1d7b95MMCEGqpT3FvwzPMT8iOO84CsZU,1021
 olive/passes/pytorch/qat_utils.py,sha256=f08zUGQTvEMsSTDKmIl1Aa2VkRjAW4_sFxhrGZOMp_o,8038
+olive/passes/pytorch/quant_utils.py,sha256=r4WnIiFZJyc3_xaGeFsYTVy15iMmm37KI4m1suAz3fI,11630
 olive/passes/pytorch/quantization_aware_training.py,sha256=dl2YSOJoXuTWG8vQM_uQqvnrqBu86IGXEQrH9J4UPU4,6444
-olive/passes/pytorch/slicegpt.py,sha256=CP0HlDxEvMWcoUUIDg2DsnsTdLiPqROX_C229nVfcHk,7085
+olive/passes/pytorch/slicegpt.py,sha256=kbBBz0Q3IOgY_IJZqN9wyTYF6RvRSGEnmyHVQPbZsOw,6868
 olive/passes/pytorch/sparsegpt.py,sha256=96vnAWMe4KMcG4-LcdNlxluyUBuO9fIpH2mjx4s5JPE,9021
 olive/passes/pytorch/sparsegpt_utils.py,sha256=PgqZh_HYV9DTzURT0T269r984KxDNhKZQ10sfDDEjpc,10774
 olive/passes/pytorch/tensor_parallel.py,sha256=Ft798VoHjXKLlDItvwydPnvF9ak2FKyOYbVPg7rWkiU,7032
 olive/passes/pytorch/tensor_parallel_layers.py,sha256=91Cc4y_xfP_TNBg83izDXxD7Ot8g4zWkc-ajMc-8AmM,5372
 olive/passes/pytorch/tensor_parallel_llama2.py,sha256=X3lbqPif5VoVia03lma5AuLYrx8SCp5NGXKXh6DS7Zw,17239
 olive/passes/pytorch/torch_trt_conversion.py,sha256=lEJcNC-gXR_xXBps7R-HBAu3qlqMdSkWONe9Gb63v4s,8172
 olive/passes/pytorch/trt_utils.py,sha256=yXqmVoRruHl8raI3ySj8GItaPEbRstqbZo7G-HLZiBI,3185
 olive/passes/qnn/__init__.py,sha256=WSNxt3l4lkWA_0vhw1ED4I7KOO0mnAuHwSgFYqbq0Lg,247
 olive/passes/qnn/context_binary_generator.py,sha256=2EEBfThotk2288WXsU-eTjZWq410sv8bMfdqG_ICBx0,3192
-olive/passes/qnn/conversion.py,sha256=atW7a7OsXL3YvxeeOr7q1X0hx5QnSkN5RwMCs4QGRys,5268
+olive/passes/qnn/conversion.py,sha256=QAXCc2EPcui5518tchQdAeGKZTabeV_BZAf9XqZoYa4,5448
 olive/passes/qnn/model_lib_generator.py,sha256=aDjHkUZ4To8JEu-9wo7RHbF2j278dCPwhSSiGnrG0RQ,3298
 olive/passes/snpe/__init__.py,sha256=WSNxt3l4lkWA_0vhw1ED4I7KOO0mnAuHwSgFYqbq0Lg,247
 olive/passes/snpe/conversion.py,sha256=0zUfbIP_3NKgyDxK5bKrm4AA5lSbJAF0yVXO-R8n7S8,4802
 olive/passes/snpe/quantization.py,sha256=bTkAnbP4DhJk24FmV_TzsBCWM771nSVZq-NH-X7eK5I,5254
 olive/passes/snpe/snpe_to_onnx.py,sha256=-K11FhE31t3LFb6hzjFn0NRK4y6lU5DlgJ7Umo30uzY,2637
 olive/passes/utils/__init__.py,sha256=WSNxt3l4lkWA_0vhw1ED4I7KOO0mnAuHwSgFYqbq0Lg,247
 olive/passes/utils/whisper_prepost.py,sha256=8osxHqa0wt6qY-EyG3hfEeBXH6v-QRsYZ_FH7MrPQ-Y,1619
 olive/platform_sdk/__init__.py,sha256=WSNxt3l4lkWA_0vhw1ED4I7KOO0mnAuHwSgFYqbq0Lg,247
 olive/platform_sdk/qualcomm/__init__.py,sha256=4AO2N1wSJzJPtPuEk2eWpRE3LrSybtJqep1vs0RPUPY,341
-olive/platform_sdk/qualcomm/configure.py,sha256=JbkQn71ClNhNAkvO0BoEPgS0qPaODwaXYY9QIL7J7i8,3740
 olive/platform_sdk/qualcomm/constants.py,sha256=rmj27zwJFo7k2yirMbpE876eGW7brw7MFlSSFOI3PA0,1348
 olive/platform_sdk/qualcomm/copy_libcdsprpc.ps1,sha256=uJfKdyPWGWZyVHy_pvjhGzYK1pKUocI5LTAo9_QkkX0,1046
 olive/platform_sdk/qualcomm/create_python_env.ps1,sha256=UjbVZ9q9QnKYZUzjFkjBelTG4INyIu8-mq5GRd2uK_4,2387
 olive/platform_sdk/qualcomm/create_python_env.sh,sha256=MBEu4cyIltBIKMxgP27cPMgJCMVMjX_njV5h1zPWZ-I,2431
 olive/platform_sdk/qualcomm/env.py,sha256=iGRpJt6rxXxKVFjHLEfh-z5RFNecyc30aK4yvb-NsTQ,4034
-olive/platform_sdk/qualcomm/runner.py,sha256=pgC1iuUOmGLGn1wPbETwqObgP1ERJBXyETFKzY6OU9w,3652
+olive/platform_sdk/qualcomm/runner.py,sha256=gWJ1G2fKK1dlsqFoiP59n-YdD_1i6cDgS7y-MpWN3Qk,3869
+olive/platform_sdk/qualcomm/configure/__init__.py,sha256=AHp6BEMajHr0T8ueQAckETIti7K0Slw2obzQXPrMHF0,380
+olive/platform_sdk/qualcomm/configure/__main__.py,sha256=9GWjy-M3M69F-qcB-PZECAcMhmcrmF4wcZrjrUVZx64,533
+olive/platform_sdk/qualcomm/configure/configure.py,sha256=lGQ7B52nkbxpN_fx5WVZZyC8xo0N3i15m92Hul3l_E8,3486
 olive/platform_sdk/qualcomm/qnn/__init__.py,sha256=WSNxt3l4lkWA_0vhw1ED4I7KOO0mnAuHwSgFYqbq0Lg,247
-olive/platform_sdk/qualcomm/qnn/env.py,sha256=AgrAnb8XAvyNvAXypZc98MicwJA9sW7Bv49ZlY3tIEQ,2034
+olive/platform_sdk/qualcomm/qnn/env.py,sha256=Pd_dCn7gh6Z1PtniX_zLYJV-DOxxnOgV8DRddrLPXLs,2015
 olive/platform_sdk/qualcomm/qnn/qnn.py,sha256=_XOE8eByRsEGxuRebctpr9jcPZeyVrbIwalEtsh3d3w,7269
 olive/platform_sdk/qualcomm/qnn/utils/__init__.py,sha256=WSNxt3l4lkWA_0vhw1ED4I7KOO0mnAuHwSgFYqbq0Lg,247
 olive/platform_sdk/qualcomm/snpe/__init__.py,sha256=IWmOScWKUAm6utpxkEbcDzqQd9JTJ9c39_g3wZW_RiE,396
-olive/platform_sdk/qualcomm/snpe/env.py,sha256=Ma9k7CCeuUDeSgDBEcugcPXIwzWv1T2o23MkVdbdFjI,2117
+olive/platform_sdk/qualcomm/snpe/env.py,sha256=7zHEhb_V2uKafcVUbpT8LWoJqoHjbpDq4jUaSgBgSJk,2079
 olive/platform_sdk/qualcomm/snpe/snpe.py,sha256=0Abgu0BAYKawvSpP6mWIQMCuHNdosUnh9dZv7wOTC8s,3969
 olive/platform_sdk/qualcomm/snpe/tools/__init__.py,sha256=WSNxt3l4lkWA_0vhw1ED4I7KOO0mnAuHwSgFYqbq0Lg,247
 olive/platform_sdk/qualcomm/snpe/tools/dev.py,sha256=wO4sEHbtH0fWJMo6606lzhXUrAOxfbYfMIVu8GZUvaQ,10951
-olive/platform_sdk/qualcomm/snpe/tools/inference.py,sha256=W0Om9Z203cISj38813WuVXuP8Wif0DWOYwtcTEJZ_qg,19039
+olive/platform_sdk/qualcomm/snpe/tools/inference.py,sha256=jUFcxccZOq1jntmg_D6yy3IfCWZ-RunU-OuwRXLiULI,19075
 olive/platform_sdk/qualcomm/snpe/utils/__init__.py,sha256=WSNxt3l4lkWA_0vhw1ED4I7KOO0mnAuHwSgFYqbq0Lg,247
 olive/platform_sdk/qualcomm/snpe/utils/adb.py,sha256=fW9nG-7YARNAglJIRry4t-9UwcycbFhSYWoByNHKxhE,6978
-olive/platform_sdk/qualcomm/utils/__init__.py,sha256=nU7Vcr7_IqPRj7pYSd2ApPT_KRQxpQUapEQAlVR3yG8,374
-olive/platform_sdk/qualcomm/utils/data_loader.py,sha256=BAWOMxoDKKZESo0Owlegae3gtBl8WWnDvGgDSSt1YSs,14746
+olive/platform_sdk/qualcomm/utils/__init__.py,sha256=WSNxt3l4lkWA_0vhw1ED4I7KOO0mnAuHwSgFYqbq0Lg,247
+olive/platform_sdk/qualcomm/utils/data_loader.py,sha256=nU_20AVrqhJfnK7GknmeZVUqe-ZaEOFJslJpYkDjyHU,16573
 olive/platform_sdk/qualcomm/utils/input_list.py,sha256=mvQQlu154du1f4iawpw-FwxPWEHMfSXR-2EPxDtlUCs,8878
-olive/scripts/__init__.py,sha256=WSNxt3l4lkWA_0vhw1ED4I7KOO0mnAuHwSgFYqbq0Lg,247
-olive/scripts/export_adapters.py,sha256=tJuteakhOnkQjjLL71vmqoQFjwN-uQAycCElAOLR-Ac,3130
-olive/scripts/manage_compute_instance.py,sha256=9yRsfSbIQDMrlI90wUMk1SWr8-yFnxRm9vLwKg8710I,6435
 olive/strategy/__init__.py,sha256=WSNxt3l4lkWA_0vhw1ED4I7KOO0mnAuHwSgFYqbq0Lg,247
-olive/strategy/search_parameter.py,sha256=FmKvyblJHZbS1gAh1S7589WE6yL2MbIKL38-io_yDyQ,11837
-olive/strategy/search_results.py,sha256=fD0uXHefoLDWdRzM5I36yGyM8OBLHrY9NFqGqBiTTs0,5631
-olive/strategy/search_space.py,sha256=jYGOECHWZkkVahQVTUbPe09cXoiSIxcr4iZBCoWbOFs,4702
-olive/strategy/search_strategy.py,sha256=nO9T1dy06O4-yZ0FX_9c-j8eRgr3syREF1R5GmpDg8c,12873
+olive/strategy/search_parameter.py,sha256=B1sAF2zhOYU6ZhXMe9D0idJ_g7luYVsZm0N_FrWQe4A,11993
+olive/strategy/search_results.py,sha256=O1iGt1wKby4Gb2Qy3S3qnVWzQcSg58uILU9cWf3mr3s,5638
+olive/strategy/search_space.py,sha256=jR6gOYhhZX55F4-n-XIxS69D-hI7RpLnYXIridtvNiw,4781
+olive/strategy/search_strategy.py,sha256=gJZMKFbRTETcMXzlzg_L4AB5IHShbpEPwMApW4ssfYs,13016
 olive/strategy/utils.py,sha256=5_JB0POwrCN30LFehSafjzeK6I5AJUT0Qfm0xznjZV0,2817
-olive/strategy/search_algorithm/__init__.py,sha256=K5eStkEgcBM1yNTvOAqk042RO44JO7bwYvwaoqTDG74,705
-olive/strategy/search_algorithm/exhaustive.py,sha256=YXu2iXFfsf8SdzlN_G0yjpMopIrAWn5oFWY08xUJ6Gw,1091
-olive/strategy/search_algorithm/optuna_sampler.py,sha256=kwc1eKIHalLK6pTdYmIKor1LLCdMlFd3QWQaO_303GI,4334
-olive/strategy/search_algorithm/random_sampler.py,sha256=zbZ63YzQ9AwSF5zp-l55kWpH5Ab-oxAy-5rMSW8B2NU,2421
-olive/strategy/search_algorithm/search_algorithm.py,sha256=SA51NjNp4-fI3o0a4hwk2Shgq_T-jIZuLzpZqnUp1ds,2306
-olive/strategy/search_algorithm/tpe_sampler.py,sha256=_8mksflxg3pSsPWUK-5xZoa1Za9ve3oDnlxN9YbCjsM,1841
+olive/strategy/search_algorithm/__init__.py,sha256=5C_OqoRxJ-Zl2jDu13zzb5WydijQw6qjgdauFcz3-y8,717
+olive/strategy/search_algorithm/exhaustive.py,sha256=fHVvYKkyo_MwEiAdjgWIbc8ZsNfd-sXs76r1AQ31y5w,1148
+olive/strategy/search_algorithm/optuna_sampler.py,sha256=cQGdKjGsEIQwl6iEGBpHyb9_WapWQC8-mZZ1vLlDTkI,4407
+olive/strategy/search_algorithm/random_sampler.py,sha256=yH64C_swywa5BA1s-Ia5_R-pm2LyQ7GwJSk0plfmuOA,2473
+olive/strategy/search_algorithm/search_algorithm.py,sha256=KxwYY6mPH8-rdaE3m7jTpnjDfutH7mDZWvnNAxemZ9c,2160
+olive/strategy/search_algorithm/tpe_sampler.py,sha256=GYSejFQLdPMIZcgnlny2RDtZc0HuNv9nwPuNLBugZMA,1838
 olive/systems/__init__.py,sha256=WSNxt3l4lkWA_0vhw1ED4I7KOO0mnAuHwSgFYqbq0Lg,247
-olive/systems/common.py,sha256=QqZoabZxxSLdxCuAlnALlzLYYc9n2uu4I-DqMw8M0qA,2227
-olive/systems/local.py,sha256=kWfHWzfPLxybq35FqchqJ7v2PuKIpPzG23qekTH8mUU,2300
-olive/systems/olive_system.py,sha256=guo9D784bL9k9Va9tWOfmtHDDhytrEe0A8Hplnoruvs,2158
+olive/systems/accelerator_creator.py,sha256=oqflXcBHRx8S0o0Q5_ruccyaiJKBN-VlmX9vNGtJF6s,12276
+olive/systems/common.py,sha256=en5OlcDTK-YkRxJVcq6GuzpZfnw-VYzd9acA5yMf-Wc,2288
+olive/systems/local.py,sha256=3WK9J-HMRTS_TG9YhcIrEfivPklY9bsDmmCA642kxvw,2345
+olive/systems/olive_system.py,sha256=MuSG2PuMW5_V_bFrrJWENzi5BFbxH8nL39jz9wauKJg,2203
 olive/systems/system_alias.py,sha256=rqDxUPiJZNFArMX_mg5No3W7MWOlyppiyG0pk1SmITE,3140
-olive/systems/system_config.py,sha256=M6axCyIKodee8bBYvBJHEaIQRXO4AW9fIZ2aAbJQq0o,7048
+olive/systems/system_config.py,sha256=9fTpnYG1Zdw96TEZsQb2AobujxrKRi3O3vwUFK7wtlM,7969
 olive/systems/azureml/__init__.py,sha256=XMk00ngVPkLq8SAjhtDDXDUC6FDin5K_s_eu1FGi3qA,411
 olive/systems/azureml/aml_evaluation_runner.py,sha256=nI6kKyA9xsV7oJO5jd_B9h2zZ_5Ez0lknwGyXiZQrZQ,2883
-olive/systems/azureml/aml_pass_runner.py,sha256=rb4KVQS_23l-ogpiV-0TjuOnlRyUI1jJSW8eIXzxEC4,8763
-olive/systems/azureml/aml_system.py,sha256=Nt89vRaJjjHJe7acyDKb05fMa-7LDaaVciaUFm-GCXU,32108
+olive/systems/azureml/aml_pass_runner.py,sha256=MXijGqsd56GzTY9ExXGMnOEhx_nCBHBtvbR2lvK6oeI,8466
+olive/systems/azureml/aml_system.py,sha256=fbhqrOuNM7R8IFLNiSA97XX-VMwKsTW5hWulB_7Un8s,31865
 olive/systems/docker/Dockerfile,sha256=XAQOT_ruAGlgmeoXG2E7n6clsjMEV03BSwyVps5njpo,717
 olive/systems/docker/Dockerfile.cpu,sha256=o5F5Pc2J_FhtZZT2YrXnLDb1vwhx0OYlTQ_m6LqV7VQ,464
 olive/systems/docker/Dockerfile.gpu,sha256=GdrY3B1IZVB-PADSXF2cEwJWwXjxomJP-qG29a1G45w,1006
 olive/systems/docker/Dockerfile.openvino,sha256=kFtqfQys13L0hx66YxuCMY9XXx-i0D0jtgSL5bASOng,2531
 olive/systems/docker/__init__.py,sha256=nrCMDPi17qCk3iGuH-Hbpq9JIOYkR8nOdvWsfXy9uqM,407
-olive/systems/docker/docker_system.py,sha256=eHFtKIIp8GhtLoCRe4QOKGgUkOzFH4TEA3DYhv-KDzM,18244
+olive/systems/docker/docker_system.py,sha256=rcU_xP0fwjtl22ZjrucbVc1MTyE_y5gyJbi2zLh6NAc,18295
 olive/systems/docker/eval.py,sha256=bfeDsxCb6H3P8EqtQGzlzHWpE10D_gUyoZzAZlo4sds,2187
 olive/systems/docker/runner.py,sha256=E9bahyiRo56ZfADz9iiF1FbDDlHwpk1QlEdlRu1IxkQ,1956
-olive/systems/docker/utils.py,sha256=eU0Khr8nvn_BO9j3z6Kp3JRPZpSXVxRSs9qu2Om3XvY,6200
+olive/systems/docker/utils.py,sha256=ScD5PUcggnkZ9e6syJiqlizQLvzG7bxlTjR6f3yZsYM,6258
 olive/systems/isolated_ort/__init__.py,sha256=vITx_9_O5lJ6lVD-Eh8f0mbLB5d5sYHX__HgjpAYOLg,357
 olive/systems/isolated_ort/inference_runner.py,sha256=Ob69cZe_nFbM0SKj0CaUBVuLhftprHZyQ_yr8RMdDvw,3600
-olive/systems/isolated_ort/isolated_ort_system.py,sha256=GPD97K3VXhZXgbA8BrSUJ9Ao_iDbZ4QAZYYlg7A_dqs,11269
+olive/systems/isolated_ort/isolated_ort_system.py,sha256=JtoWLxFP9MKooZzFgJf919QU55BikHjo0vsXJXZXhTk,11296
 olive/systems/python_environment/__init__.py,sha256=cu6jFeXKLees7MkoNddzPVre_eE-FwXwA3pihv4yWi4,381
 olive/systems/python_environment/common_requirements.txt,sha256=chggo_d82Zdffa3G3ZKCCpI27wcCn2f17Cziy-x4f0Q,37
 olive/systems/python_environment/evaluation_runner.py,sha256=isVzvA2aHVuCK-qfIyAqjnS03c7vzIXmYIhFjGtiCME,2279
 olive/systems/python_environment/pass_runner.py,sha256=IdvBa0Nd3D8WspdWj8ops3OVJl8b6SDnFYfVVtAlbSM,2037
-olive/systems/python_environment/python_environment_system.py,sha256=PTNWHKu8CJ8KqnUHxpqYLhjVwi-xktz4m5aCGTBLAkY,7892
+olive/systems/python_environment/python_environment_system.py,sha256=rclQbDwsJtNeRyyXHU8tGjXVNOSkjwtiIJnuBn5Muy4,7899
 olive/systems/utils/__init__.py,sha256=VCiDPtACqpIXj-k-8rpHv2xsW4JYiRVfylM5qkF36RY,705
 olive/systems/utils/arg_parser.py,sha256=ZyFvQ9o6i7SqrNffnmuYvn_jjnGlWcRNSkGkZk9HZhE,2082
 olive/systems/utils/available_providers_runner.py,sha256=0A2C61-D5r9ke5ya2hOBEp1RP_6jgeG67cJC4NlqTH8,913
-olive/systems/utils/misc.py,sha256=YFgTeaBiKXx3ibnDMpORj3U4-dwsqqQ4mkEtJ-sKx-A,7419
+olive/systems/utils/misc.py,sha256=-t3lJMfo4fdwYKbHRSFvf_fQhQHTofB6uan-YtiOlNE,7680
 olive/workflows/__init__.py,sha256=2mLegObegOEd5p6MDGX_4-Eto2XvWBFPyr3HIrz4D0g,306
 olive/workflows/run/__init__.py,sha256=WSNxt3l4lkWA_0vhw1ED4I7KOO0mnAuHwSgFYqbq0Lg,247
-olive/workflows/run/__main__.py,sha256=6awG6OZneIa769QDU6X86X5BxSzBtFByd0K5YQ671RY,1418
-olive/workflows/run/config.py,sha256=t2c2vMli_hVcBpjikrGAll1ddAnE8fPlULALg8Ox2EU,13473
-olive/workflows/run/run.py,sha256=5N4_KMuALfyvPz3PcVelDBGvFTZNgfktab2smuiMg4w,13365
-olive/workflows/snpe/__init__.py,sha256=wqFn-4s3Sxzuy0Oa2euleTB7qUO-4g63bV2h7TW5XGU,431
-olive/workflows/snpe/convertquantize/__init__.py,sha256=WSNxt3l4lkWA_0vhw1ED4I7KOO0mnAuHwSgFYqbq0Lg,247
-olive/workflows/snpe/convertquantize/__main__.py,sha256=re1UWNmJI_E9ubcrAEs4JeP_A4C3LBQMnVofw9TvI40,1339
-olive/workflows/snpe/convertquantize/convertquantize.py,sha256=GaM0LpjcZVgi89vh8r0losJDltNC6sKZtRB1rUVxXbU,4445
-olive/workflows/snpe/evaluate/__init__.py,sha256=WSNxt3l4lkWA_0vhw1ED4I7KOO0mnAuHwSgFYqbq0Lg,247
-olive/workflows/snpe/evaluate/__main__.py,sha256=UAmzVqOnC90Ns3l8oBhHPheyEC2kncFgC-Gl7qXAoEQ,955
-olive/workflows/snpe/evaluate/evaluate.py,sha256=NGRS_9whYc4wvSola46jLiQduSb4mVr1AKlpCr-bmB0,2974
-olive_ai-0.5.2.dist-info/LICENSE,sha256=ws_MuBL-SCEBqPBFl9_FqZkaaydIJmxHrJG2parhU4M,1141
-olive_ai-0.5.2.dist-info/METADATA,sha256=8RMPQHAhHYlX5c6ggbq1era2aQ5BVuVv3z63AcC5lWA,3438
-olive_ai-0.5.2.dist-info/NOTICE.txt,sha256=h7RtTa8A8uYhoKJ-nO_kScaD8qHLYj0en8UYEqpy5_E,764423
-olive_ai-0.5.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-olive_ai-0.5.2.dist-info/entry_points.txt,sha256=XVTpnzIsU7uElE03r2zsuqXrvUKWbMw-ndKgwSBYAoM,101
-olive_ai-0.5.2.dist-info/top_level.txt,sha256=V9j-sv9fsgSHbZLD-a-cxoocQvfzNaWA8w_3snFQbhQ,6
-olive_ai-0.5.2.dist-info/RECORD,,
+olive/workflows/run/__main__.py,sha256=3DmHb_yyOuTFCWdrMUkimAe3neTwjjn2NqfE_rctWCk,399
+olive/workflows/run/config.py,sha256=a28a3ojX5q4KNCnQ3GpG6O9RBHLUj7NfC11u3FWlUCA,11708
+olive/workflows/run/run.py,sha256=zDm457NzjnVUoFrhcczM8GIQ808plE48g4l7bxEWyFo,15359
+olive_ai-0.6.0.dist-info/LICENSE,sha256=ws_MuBL-SCEBqPBFl9_FqZkaaydIJmxHrJG2parhU4M,1141
+olive_ai-0.6.0.dist-info/METADATA,sha256=faz44-NJ_tl2u1wxT4xLQ6Cr1EluVecnifkTI8zSvTA,3568
+olive_ai-0.6.0.dist-info/NOTICE.txt,sha256=h7RtTa8A8uYhoKJ-nO_kScaD8qHLYj0en8UYEqpy5_E,764423
+olive_ai-0.6.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+olive_ai-0.6.0.dist-info/entry_points.txt,sha256=aHNsskT6XbNGHRzJyxWrLOpCWCpqAL8CBIakQxqpKE0,50
+olive_ai-0.6.0.dist-info/top_level.txt,sha256=V9j-sv9fsgSHbZLD-a-cxoocQvfzNaWA8w_3snFQbhQ,6
+olive_ai-0.6.0.dist-info/RECORD,,
```

