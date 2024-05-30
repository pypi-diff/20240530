# Comparing `tmp/careamics-0.1.0rc4.tar.gz` & `tmp/careamics-0.1.0rc5.tar.gz`

## Comparing `careamics-0.1.0rc4.tar` & `careamics-0.1.0rc5.tar`

### file list

```diff
@@ -1,173 +1,175 @@
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/.github/PR_TEMPLATE/pull_request.md
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/.github/workflows/ci.yml
--rw-r--r--   0        0        0     5493 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/examples/2D/n2n/example_SEM_careamist.ipynb
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/examples/2D/n2n/n2n_2D_SEM.yml
--rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/examples/2D/n2v/example_BSD68_careamist.ipynb
--rw-r--r--   0        0        0     9737 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/examples/2D/n2v/example_BSD68_lightning.ipynb
--rw-r--r--   0        0        0     7129 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/examples/2D/n2v/example_SEM_lightning.ipynb
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/examples/2D/n2v/n2v_2D_BSD.yml
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/examples/2D/pn2v/pN2V_Convallaria.yml
--rw-r--r--   0        0        0     7882 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/examples/3D/example_flywing_3D.ipynb
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/examples/3D/n2v_flywing_3D.yml
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/__init__.py
--rw-r--r--   0        0        0    28409 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/careamist.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/conftest.py
--rw-r--r--   0        0        0    31915 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/lightning_datamodule.py
--rw-r--r--   0        0        0    10174 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/lightning_module.py
--rw-r--r--   0        0        0    15364 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/lightning_prediction_datamodule.py
--rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/lightning_prediction_loop.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/py.typed
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/callbacks/__init__.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/callbacks/hyperparameters_callback.py
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/callbacks/progress_bar_callback.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/__init__.py
--rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/algorithm_model.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/callback_model.py
--rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/configuration_example.py
--rw-r--r--   0        0        0    18793 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/configuration_factory.py
--rw-r--r--   0        0        0    18754 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/configuration_model.py
--rw-r--r--   0        0        0    16809 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/data_model.py
--rw-r--r--   0        0        0     8127 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/inference_model.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/noise_models.py
--rw-r--r--   0        0        0     5266 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/optimizer_models.py
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/tile_information.py
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/training_model.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/architectures/__init__.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/architectures/architecture_model.py
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/architectures/custom_model.py
--rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/architectures/register_model.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/architectures/unet_model.py
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/architectures/vae_model.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/references/__init__.py
--rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/references/algorithm_descriptions.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/references/references.py
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/support/__init__.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/support/supported_activations.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/support/supported_algorithms.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/support/supported_architectures.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/support/supported_data.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/support/supported_extraction_strategies.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/support/supported_loggers.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/support/supported_losses.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/support/supported_optimizers.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/support/supported_pixel_manipulations.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/support/supported_struct_axis.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/support/supported_transforms.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/transformations/__init__.py
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/transformations/n2v_manipulate_model.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/transformations/nd_flip_model.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/transformations/normalize_model.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/transformations/transform_model.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/transformations/xy_random_rotate90_model.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/validators/__init__.py
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/validators/validator_utils.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/dataset/__init__.py
--rw-r--r--   0        0        0    12213 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/dataset/in_memory_dataset.py
--rw-r--r--   0        0        0    15035 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/dataset/iterable_dataset.py
--rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/dataset/zarr_dataset.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/dataset/dataset_utils/__init__.py
--rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/dataset/dataset_utils/dataset_utils.py
--rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/dataset/dataset_utils/file_utils.py
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/dataset/dataset_utils/read_tiff.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/dataset/dataset_utils/read_utils.py
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/dataset/dataset_utils/read_zarr.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/dataset/patching/__init__.py
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/dataset/patching/patch_transform.py
--rw-r--r--   0        0        0     6258 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/dataset/patching/patching.py
--rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/dataset/patching/random_patching.py
--rw-r--r--   0        0        0     5688 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/dataset/patching/sequential_patching.py
--rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/dataset/patching/tiled_patching.py
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/dataset/patching/validate_patch_dimension.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/losses/__init__.py
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/losses/loss_factory.py
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/losses/losses.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/losses/noise_model_factory.py
--rw-r--r--   0        0        0    17801 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/losses/noise_models.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/model_io/__init__.py
--rw-r--r--   0        0        0     6955 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/model_io/bmz_io.py
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/model_io/model_io_utils.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/model_io/bioimage/__init__.py
--rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/model_io/bioimage/_readme_factory.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/model_io/bioimage/bioimage_utils.py
--rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/model_io/bioimage/model_description.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/models/__init__.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/models/activation.py
--rw-r--r--   0        0        0    11557 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/models/layers.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/models/model_factory.py
--rw-r--r--   0        0        0    10925 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/models/unet.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/prediction/__init__.py
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/prediction/stitch_prediction.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/transforms/__init__.py
--rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/transforms/n2v_manipulate.py
--rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/transforms/nd_flip.py
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/transforms/normalize.py
--rw-r--r--   0        0        0    12776 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/transforms/pixel_manipulation.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/transforms/struct_mask_parameters.py
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/transforms/tta.py
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/transforms/xy_random_rotate90.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/utils/__init__.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/utils/base_enum.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/utils/context.py
--rw-r--r--   0        0        0    10321 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/utils/logging.py
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/utils/metrics.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/utils/path_utils.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/utils/ram.py
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/utils/receptive_field.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/utils/running_stats.py
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/utils/torch_utils.py
--rw-r--r--   0        0        0     6602 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/conftest.py
--rw-r--r--   0        0        0    22382 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/test_careamist.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/test_conftest.py
--rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/test_lightning_datamodule.py
--rw-r--r--   0        0        0     7262 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/test_lightning_module.py
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/test_lightning_prediction_datamodule.py
--rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/config/test_algorithm_model.py
--rw-r--r--   0        0        0     6483 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/config/test_configuration_factory.py
--rw-r--r--   0        0        0     6180 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/config/test_configuration_model.py
--rw-r--r--   0        0        0    12328 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/config/test_data_model.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/config/test_full_config_example.py
--rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/config/test_inference_model.py
--rw-r--r--   0        0        0     4267 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/config/test_optimizers_model.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/config/test_tile_information.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/config/test_training_model.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/config/architectures/test_architecture_model.py
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/config/architectures/test_custom_model.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/config/architectures/test_register_model.py
--rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/config/architectures/test_unet_model.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/config/support/test_supported_data.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/config/support/test_supported_optimizers.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/config/transformations/test_n2v_manipulate_model.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/config/transformations/test_normalize_model.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/config/validators/test_validator_utils.py
--rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/dataset/test_in_memory_dataset.py
--rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/dataset/test_iterable_dataset.py
--rw-r--r--   0        0        0     6203 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/dataset/dataset_utils/test_list_files.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/dataset/dataset_utils/test_read_tiff.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/dataset/patching/test_patching_utils.py
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/dataset/patching/test_random_patching.py
--rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/dataset/patching/test_sequential_patching.py
--rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/dataset/patching/test_tiled_patching.py
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/model_io/test_bmz_io.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/models/test_model_factory.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/models/test_unet.py
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/prediction/test_stitch_prediction.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/transforms/test_manipulate_n2v.py
--rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/transforms/test_nd_flip.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/transforms/test_normalize.py
--rw-r--r--   0        0        0     8954 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/transforms/test_pixel_manipulation.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/transforms/test_supported_transforms.py
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/transforms/test_xy_random_rotate90.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/utils/test_base_enum.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/utils/test_context.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/utils/test_logging.py
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/utils/test_metrics.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/utils/test_torch_utils.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/utils/test_wandb.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/.gitignore
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/LICENSE
--rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/README.md
--rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/pyproject.toml
--rw-r--r--   0        0        0     4631 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/PKG-INFO
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/.github/pull_request_template.md
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     5493 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/examples/2D/n2n/example_SEM_careamist.ipynb
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/examples/2D/n2n/n2n_2D_SEM.yml
+-rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/examples/2D/n2v/example_BSD68_careamist.ipynb
+-rw-r--r--   0        0        0     9737 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/examples/2D/n2v/example_BSD68_lightning.ipynb
+-rw-r--r--   0        0        0     7129 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/examples/2D/n2v/example_SEM_lightning.ipynb
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/examples/2D/n2v/n2v_2D_BSD.yml
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/examples/2D/pn2v/pN2V_Convallaria.yml
+-rw-r--r--   0        0        0     7882 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/examples/3D/example_flywing_3D.ipynb
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/examples/3D/n2v_flywing_3D.yml
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/__init__.py
+-rw-r--r--   0        0        0    28755 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/careamist.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/conftest.py
+-rw-r--r--   0        0        0    31661 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/lightning_datamodule.py
+-rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/lightning_module.py
+-rw-r--r--   0        0        0    15517 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/lightning_prediction_datamodule.py
+-rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/lightning_prediction_loop.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/py.typed
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/callbacks/__init__.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/callbacks/hyperparameters_callback.py
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/callbacks/progress_bar_callback.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/__init__.py
+-rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/algorithm_model.py
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/callback_model.py
+-rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/configuration_example.py
+-rw-r--r--   0        0        0    21734 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/configuration_factory.py
+-rw-r--r--   0        0        0    18494 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/configuration_model.py
+-rw-r--r--   0        0        0    12946 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/data_model.py
+-rw-r--r--   0        0        0     7909 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/inference_model.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/noise_models.py
+-rw-r--r--   0        0        0     5266 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/optimizer_models.py
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/tile_information.py
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/training_model.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/architectures/__init__.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/architectures/architecture_model.py
+-rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/architectures/custom_model.py
+-rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/architectures/register_model.py
+-rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/architectures/unet_model.py
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/architectures/vae_model.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/references/__init__.py
+-rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/references/algorithm_descriptions.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/references/references.py
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/support/__init__.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/support/supported_activations.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/support/supported_algorithms.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/support/supported_architectures.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/support/supported_data.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/support/supported_extraction_strategies.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/support/supported_loggers.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/support/supported_losses.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/support/supported_optimizers.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/support/supported_pixel_manipulations.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/support/supported_struct_axis.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/support/supported_transforms.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/transformations/__init__.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/transformations/n2v_manipulate_model.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/transformations/nd_flip_model.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/transformations/normalize_model.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/transformations/transform_model.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/transformations/xy_random_rotate90_model.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/validators/__init__.py
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/config/validators/validator_utils.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/dataset/__init__.py
+-rw-r--r--   0        0        0    10900 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/dataset/in_memory_dataset.py
+-rw-r--r--   0        0        0    12333 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/dataset/iterable_dataset.py
+-rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/dataset/zarr_dataset.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/dataset/dataset_utils/__init__.py
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/dataset/dataset_utils/dataset_utils.py
+-rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/dataset/dataset_utils/file_utils.py
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/dataset/dataset_utils/read_tiff.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/dataset/dataset_utils/read_utils.py
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/dataset/dataset_utils/read_zarr.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/dataset/patching/__init__.py
+-rw-r--r--   0        0        0     6259 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/dataset/patching/patching.py
+-rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/dataset/patching/random_patching.py
+-rw-r--r--   0        0        0     5651 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/dataset/patching/sequential_patching.py
+-rw-r--r--   0        0        0     5814 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/dataset/patching/tiled_patching.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/dataset/patching/validate_patch_dimension.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/losses/__init__.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/losses/loss_factory.py
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/losses/losses.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/losses/noise_model_factory.py
+-rw-r--r--   0        0        0    17801 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/losses/noise_models.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/model_io/__init__.py
+-rw-r--r--   0        0        0     6967 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/model_io/bmz_io.py
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/model_io/model_io_utils.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/model_io/bioimage/__init__.py
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/model_io/bioimage/_readme_factory.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/model_io/bioimage/bioimage_utils.py
+-rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/model_io/bioimage/model_description.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/models/__init__.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/models/activation.py
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/models/layers.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/models/model_factory.py
+-rw-r--r--   0        0        0    13431 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/models/unet.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/prediction/__init__.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/prediction/stitch_prediction.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/transforms/__init__.py
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/transforms/compose.py
+-rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/transforms/n2v_manipulate.py
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/transforms/nd_flip.py
+-rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/transforms/normalize.py
+-rw-r--r--   0        0        0    12693 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/transforms/pixel_manipulation.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/transforms/struct_mask_parameters.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/transforms/transform.py
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/transforms/tta.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/transforms/xy_random_rotate90.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/utils/__init__.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/utils/base_enum.py
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/utils/context.py
+-rw-r--r--   0        0        0    10322 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/utils/logging.py
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/utils/metrics.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/utils/path_utils.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/utils/ram.py
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/utils/receptive_field.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/utils/running_stats.py
+-rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/src/careamics/utils/torch_utils.py
+-rw-r--r--   0        0        0     6602 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/conftest.py
+-rw-r--r--   0        0        0    22558 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/test_careamist.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/test_conftest.py
+-rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/test_lightning_datamodule.py
+-rw-r--r--   0        0        0     8251 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/test_lightning_module.py
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/test_lightning_prediction_datamodule.py
+-rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/config/test_algorithm_model.py
+-rw-r--r--   0        0        0    17140 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/config/test_configuration_factory.py
+-rw-r--r--   0        0        0     6180 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/config/test_configuration_model.py
+-rw-r--r--   0        0        0    10966 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/config/test_data_model.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/config/test_full_config_example.py
+-rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/config/test_inference_model.py
+-rw-r--r--   0        0        0     4267 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/config/test_optimizers_model.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/config/test_tile_information.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/config/test_training_model.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/config/architectures/test_architecture_model.py
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/config/architectures/test_custom_model.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/config/architectures/test_register_model.py
+-rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/config/architectures/test_unet_model.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/config/support/test_supported_data.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/config/support/test_supported_optimizers.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/config/transformations/test_n2v_manipulate_model.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/config/transformations/test_normalize_model.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/config/validators/test_validator_utils.py
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/dataset/test_in_memory_dataset.py
+-rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/dataset/test_iterable_dataset.py
+-rw-r--r--   0        0        0     6203 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/dataset/dataset_utils/test_list_files.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/dataset/dataset_utils/test_read_tiff.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/dataset/patching/test_patching_utils.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/dataset/patching/test_random_patching.py
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/dataset/patching/test_sequential_patching.py
+-rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/dataset/patching/test_tiled_patching.py
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/model_io/test_bmz_io.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/models/test_model_factory.py
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/models/test_unet.py
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/prediction/test_stitch_prediction.py
+-rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/transforms/test_compose.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/transforms/test_manipulate_n2v.py
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/transforms/test_nd_flip.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/transforms/test_normalize.py
+-rw-r--r--   0        0        0     8954 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/transforms/test_pixel_manipulation.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/transforms/test_supported_transforms.py
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/transforms/test_xy_random_rotate90.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/utils/test_base_enum.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/utils/test_context.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/utils/test_logging.py
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/utils/test_metrics.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/utils/test_torch_utils.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/tests/utils/test_wandb.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/.gitignore
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/LICENSE
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/README.md
+-rw-r--r--   0        0        0     4759 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/pyproject.toml
+-rw-r--r--   0        0        0     3413 2020-02-02 00:00:00.000000 careamics-0.1.0rc5/PKG-INFO
```

### Comparing `careamics-0.1.0rc4/.pre-commit-config.yaml` & `careamics-0.1.0rc5/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -5,52 +5,52 @@
 ci:
   autoupdate_schedule: monthly
   autofix_commit_msg: "style(pre-commit.ci): auto fixes [...]"
   autoupdate_commit_msg: "ci(pre-commit.ci): autoupdate"
 
 repos:
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.14
+    rev: v0.16
     hooks:
       - id: validate-pyproject
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.0.292
+    rev: v0.4.3
     hooks:
       - id: ruff
         args: [--fix, --target-version, py38]
 
   - repo: https://github.com/psf/black
-    rev: 23.9.1
+    rev: 24.4.2
     hooks:
       - id: black
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.5.1
+    rev: v1.10.0
     hooks:
       - id: mypy
         files: "^src/"
         additional_dependencies:
           - numpy
           - types-PyYAML
           - types-setuptools
 
   # check docstrings
   - repo: https://github.com/numpy/numpydoc
-    rev: v1.6.0
+    rev: v1.7.0
     hooks:
       - id: numpydoc-validation
 
   # jupyter linting and formatting
   - repo: https://github.com/nbQA-dev/nbQA
-    rev: 1.7.0
+    rev: 1.8.5
     hooks:
       - id: nbqa-ruff
         args: [--fix]
       - id: nbqa-black
       #- id: nbqa-mypy
 
   # strip out jupyter notebooks
   - repo: https://github.com/kynan/nbstripout
-    rev: 0.6.1
+    rev: 0.7.1
     hooks:
       - id: nbstripout
```

### Comparing `careamics-0.1.0rc4/.github/ISSUE_TEMPLATE/bug_report.md` & `careamics-0.1.0rc5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/.github/ISSUE_TEMPLATE/feature_request.md` & `careamics-0.1.0rc5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/.github/workflows/ci.yml` & `careamics-0.1.0rc5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/examples/2D/n2n/example_SEM_careamist.ipynb` & `careamics-0.1.0rc5/examples/2D/n2n/example_SEM_careamist.ipynb`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/examples/2D/n2n/n2n_2D_SEM.yml` & `careamics-0.1.0rc5/examples/2D/n2n/n2n_2D_SEM.yml`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/examples/2D/n2v/example_BSD68_careamist.ipynb` & `careamics-0.1.0rc5/examples/2D/n2v/example_BSD68_careamist.ipynb`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/examples/2D/n2v/example_BSD68_lightning.ipynb` & `careamics-0.1.0rc5/examples/2D/n2v/example_BSD68_lightning.ipynb`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/examples/2D/n2v/example_SEM_lightning.ipynb` & `careamics-0.1.0rc5/examples/2D/n2v/example_SEM_lightning.ipynb`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/examples/2D/n2v/n2v_2D_BSD.yml` & `careamics-0.1.0rc5/examples/2D/n2v/n2v_2D_BSD.yml`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/examples/2D/pn2v/pN2V_Convallaria.yml` & `careamics-0.1.0rc5/examples/2D/pn2v/pN2V_Convallaria.yml`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/examples/3D/example_flywing_3D.ipynb` & `careamics-0.1.0rc5/examples/3D/example_flywing_3D.ipynb`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/examples/3D/n2v_flywing_3D.yml` & `careamics-0.1.0rc5/examples/3D/n2v_flywing_3D.yml`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/src/careamics/__init__.py` & `careamics-0.1.0rc5/src/careamics/__init__.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/src/careamics/careamist.py` & `careamics-0.1.0rc5/src/careamics/careamist.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,25 +69,23 @@
 
     @overload
     def __init__(  # numpydoc ignore=GL08
         self,
         source: Union[Path, str],
         work_dir: Optional[str] = None,
         experiment_name: str = "CAREamics",
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @overload
     def __init__(  # numpydoc ignore=GL08
         self,
         source: Configuration,
         work_dir: Optional[str] = None,
         experiment_name: str = "CAREamics",
-    ) -> None:
-        ...
+    ) -> None: ...
 
     def __init__(
         self,
         source: Union[Path, str, Configuration],
         work_dir: Optional[Union[Path, str]] = None,
         experiment_name: str = "CAREamics",
     ) -> None:
@@ -474,16 +472,15 @@
 
     @overload
     def predict(  # numpydoc ignore=GL08
         self,
         source: CAREamicsPredictData,
         *,
         checkpoint: Optional[Literal["best", "last"]] = None,
-    ) -> Union[list, np.ndarray]:
-        ...
+    ) -> Union[list, np.ndarray]: ...
 
     @overload
     def predict(  # numpydoc ignore=GL08
         self,
         source: Union[Path, str],
         *,
         batch_size: int = 1,
@@ -493,16 +490,15 @@
         data_type: Optional[Literal["tiff", "custom"]] = None,
         transforms: Optional[List[TRANSFORMS_UNION]] = None,
         tta_transforms: bool = True,
         dataloader_params: Optional[Dict] = None,
         read_source_func: Optional[Callable] = None,
         extension_filter: str = "",
         checkpoint: Optional[Literal["best", "last"]] = None,
-    ) -> Union[list, np.ndarray]:
-        ...
+    ) -> Union[list, np.ndarray]: ...
 
     @overload
     def predict(  # numpydoc ignore=GL08
         self,
         source: np.ndarray,
         *,
         batch_size: int = 1,
@@ -510,16 +506,15 @@
         tile_overlap: Tuple[int, ...] = (48, 48),
         axes: Optional[str] = None,
         data_type: Optional[Literal["array"]] = None,
         transforms: Optional[List[TRANSFORMS_UNION]] = None,
         tta_transforms: bool = True,
         dataloader_params: Optional[Dict] = None,
         checkpoint: Optional[Literal["best", "last"]] = None,
-    ) -> Union[list, np.ndarray]:
-        ...
+    ) -> Union[list, np.ndarray]: ...
 
     def predict(
         self,
         source: Union[CAREamicsPredictData, Path, str, np.ndarray],
         *,
         batch_size: int = 1,
         tile_size: Optional[Tuple[int, ...]] = None,
@@ -544,14 +539,20 @@
         `tile_size`.
 
         The default transforms are defined in the `InferenceModel` Pydantic model.
 
         Test-time augmentation (TTA) can be switched off using the `tta_transforms`
         parameter.
 
+        Note that if you are using a UNet model and tiling, the tile size must be
+        divisible in every dimension by 2**d, where d is the depth of the model. This
+        avoids artefacts arising from the broken shift invariance induced by the
+        pooling layers of the UNet. If your image has less dimensions, as it may
+        happen in the Z dimension, consider padding your image.
+
         Parameters
         ----------
         source : Union[CAREamicsClay, Path, str, np.ndarray]
             Data to predict on.
         batch_size : int, optional
             Batch size for prediction, by default 1.
         tile_size : Optional[Tuple[int, ...]], optional
@@ -598,15 +599,15 @@
             if self.cfg is None:
                 raise ValueError(
                     "No configuration found. Train a model or load from a "
                     "checkpoint before predicting."
                 )
             # create predict config, reuse training config if parameters missing
             prediction_config = create_inference_configuration(
-                training_configuration=self.cfg,
+                configuration=self.cfg,
                 tile_size=tile_size,
                 tile_overlap=tile_overlap,
                 data_type=data_type,
                 axes=axes,
                 transforms=transforms,
                 tta_transforms=tta_transforms,
                 batch_size=batch_size,
```

### Comparing `careamics-0.1.0rc4/src/careamics/conftest.py` & `careamics-0.1.0rc5/src/careamics/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """File used to discover python modules and run doctest.
 
 See https://sybil.readthedocs.io/en/latest/use.html#pytest
 """
+
 from pathlib import Path
 
 import pytest
 from pytest import TempPathFactory
 from sybil import Sybil
 from sybil.parsers.codeblock import PythonCodeBlockParser
 from sybil.parsers.doctest import DocTestParser
```

### Comparing `careamics-0.1.0rc4/src/careamics/lightning_datamodule.py` & `careamics-0.1.0rc5/src/careamics/lightning_datamodule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Training and validation Lightning data modules."""
+
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Literal, Optional, Union
 
 import numpy as np
 import pytorch_lightning as L
-from albumentations import Compose
 from torch.utils.data import DataLoader
 
 from careamics.config import DataConfig
 from careamics.config.data_model import TRANSFORMS_UNION
 from careamics.config.support import SupportedData
 from careamics.dataset.dataset_utils import (
     get_files_size,
@@ -337,28 +337,28 @@
             # we run the training in memory, otherwise we switch to iterable dataset
             # The switch is deactivated if use_in_memory is False
             if self.use_in_memory and self.train_files_size < get_ram_size() * 0.8:
                 # train dataset
                 self.train_dataset = InMemoryDataset(
                     data_config=self.data_config,
                     inputs=self.train_files,
-                    data_target=self.train_target_files
-                    if self.train_data_target
-                    else None,
+                    data_target=(
+                        self.train_target_files if self.train_data_target else None
+                    ),
                     read_source_func=self.read_source_func,
                 )
 
                 # validation dataset
                 if self.val_data is not None:
                     self.val_dataset = InMemoryDataset(
                         data_config=self.data_config,
                         inputs=self.val_files,
-                        data_target=self.val_target_files
-                        if self.val_data_target
-                        else None,
+                        data_target=(
+                            self.val_target_files if self.val_data_target else None
+                        ),
                         read_source_func=self.read_source_func,
                     )
                 else:
                     # split dataset
                     self.val_dataset = self.train_dataset.split_dataset(
                         percentage=self.val_percentage,
                         minimum_patches=self.val_minimum_split,
@@ -366,29 +366,29 @@
 
             # else if the data is too large, load file by file during training
             else:
                 # create training dataset
                 self.train_dataset = PathIterableDataset(
                     data_config=self.data_config,
                     src_files=self.train_files,
-                    target_files=self.train_target_files
-                    if self.train_data_target
-                    else None,
+                    target_files=(
+                        self.train_target_files if self.train_data_target else None
+                    ),
                     read_source_func=self.read_source_func,
                 )
 
                 # create validation dataset
                 if self.val_files is not None:
                     # create its own dataset
                     self.val_dataset = PathIterableDataset(
                         data_config=self.data_config,
                         src_files=self.val_files,
-                        target_files=self.val_target_files
-                        if self.val_data_target
-                        else None,
+                        target_files=(
+                            self.val_target_files if self.val_data_target else None
+                        ),
                         read_source_func=self.read_source_func,
                     )
                 elif len(self.train_files) <= self.val_minimum_split:
                     raise ValueError(
                         f"Not enough files to split a minimum of "
                         f"{self.val_minimum_split} files, got {len(self.train_files)} "
                         f"files."
@@ -448,16 +448,15 @@
 
     To use array data, set `data_type` to `array` and pass a numpy array to
     `train_data`.
 
     In particular, N2V requires a specific transformation (N2V manipulates), which is
     not compatible with supervised training. The default transformations applied to the
     training patches are defined in `careamics.config.data_model`. To use different
-    transformations, pass a list of transforms or an albumentation `Compose` as
-    `transforms` parameter. See examples for more details.
+    transformations, pass a list of transforms. See examples for more details.
 
     By default, CAREamics only supports types defined in
     `careamics.config.support.SupportedData`. To read custom data types, you can set
     `data_type` to `custom` and provide a function that returns a numpy array from a
     path. Additionally, pass a `fnmatch` and `Path.rglob` compatible expression (e.g.
     "*.jpeg") to filter the files extension using `extension_filter`.
 
@@ -484,15 +483,15 @@
         Patch size, 2D or 3D patch size.
     axes : str
         Axes of the data, choosen amongst SCZYX.
     batch_size : int
         Batch size.
     val_data : Optional[Union[str, Path]], optional
         Validation data, by default None.
-    transforms : Optional[Union[List[TRANSFORMS_UNION], Compose]], optional
+    transforms : List[TRANSFORMS_UNION], optional
         List of transforms to apply to training patches. If None, default transforms
         are applied.
     train_target_data : Optional[Union[str, Path]], optional
         Training target data, by default None.
     val_target_data : Optional[Union[str, Path]], optional
         Validation target data, by default None.
     read_source_func : Optional[Callable], optional
@@ -580,15 +579,15 @@
         self,
         train_data: Union[str, Path, np.ndarray],
         data_type: Union[Literal["array", "tiff", "custom"], SupportedData],
         patch_size: List[int],
         axes: str,
         batch_size: int,
         val_data: Optional[Union[str, Path]] = None,
-        transforms: Optional[Union[List[TRANSFORMS_UNION], Compose]] = None,
+        transforms: Optional[List[TRANSFORMS_UNION]] = None,
         train_target_data: Optional[Union[str, Path]] = None,
         val_target_data: Optional[Union[str, Path]] = None,
         read_source_func: Optional[Callable] = None,
         extension_filter: str = "",
         val_percentage: float = 0.1,
         val_minimum_patches: int = 5,
         dataloader_params: Optional[dict] = None,
@@ -613,16 +612,16 @@
 
         To use array data, set `data_type` to `array` and pass a numpy array to
         `train_data`.
 
         In particular, N2V requires a specific transformation (N2V manipulates), which
         is not compatible with supervised training. The default transformations applied
         to the training patches are defined in `careamics.config.data_model`. To use
-        different transformations, pass a list of transforms or an albumentation
-        `Compose` as `transforms` parameter. See examples for more details.
+        different transformations, pass a list of transforms. See examples for more
+        details.
 
         By default, CAREamics only supports types defined in
         `careamics.config.support.SupportedData`. To read custom data types, you can set
         `data_type` to `custom` and provide a function that returns a numpy array from a
         path. Additionally, pass a `fnmatch` and `Path.rglob` compatible expression
         (e.g. "*.jpeg") to filter the files extension using `extension_filter`.
 
@@ -651,15 +650,15 @@
             Patch size, 2D or 3D patch size.
         axes : str
             Axes of the data, choosen amongst SCZYX.
         batch_size : int
             Batch size.
         val_data : Optional[Union[str, Path]], optional
             Validation data, by default None.
-        transforms : Optional[Union[List[TRANSFORMS_UNION], Compose]], optional
+        transforms : Optional[List[TRANSFORMS_UNION]], optional
             List of transforms to apply to training patches. If None, default transforms
             are applied.
         train_target_data : Optional[Union[str, Path]], optional
             Training target data, by default None.
         val_target_data : Optional[Union[str, Path]], optional
             Validation target data, by default None.
         read_source_func : Optional[Callable], optional
@@ -705,18 +704,15 @@
         if transforms is not None:
             data_dict["transforms"] = transforms
 
         # validate configuration
         self.data_config = DataConfig(**data_dict)
 
         # N2V specific checks, N2V, structN2V, and transforms
-        if (
-            self.data_config.has_transform_list()
-            and self.data_config.has_n2v_manipulate()
-        ):
+        if self.data_config.has_n2v_manipulate():
             # there is not target, n2v2 and structN2V can be changed
             if train_target_data is None:
                 self.data_config.set_N2V2(use_n2v2)
                 self.data_config.set_structN2V_mask(struct_n2v_axis, struct_n2v_span)
             else:
                 raise ValueError(
                     "Cannot have both supervised training (target data) and "
```

### Comparing `careamics-0.1.0rc4/src/careamics/lightning_module.py` & `careamics-0.1.0rc5/src/careamics/lightning_module.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
             output = self.model(x)
 
         # Denormalize the output
         denorm = Denormalize(
             mean=self._trainer.datamodule.predict_dataset.mean,
             std=self._trainer.datamodule.predict_dataset.std,
         )
-        denormalized_output = denorm(image=output)["image"]
+        denormalized_output, _ = denorm(patch=output)
 
         if len(aux) > 0:
             return denormalized_output, aux
         else:
             return denormalized_output
 
     def configure_optimizers(self) -> Any:
```

### Comparing `careamics-0.1.0rc4/src/careamics/lightning_prediction_datamodule.py` & `careamics-0.1.0rc5/src/careamics/lightning_prediction_datamodule.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Prediction Lightning data modules."""
+
 from pathlib import Path
 from typing import Any, Callable, List, Literal, Optional, Tuple, Union
 
 import numpy as np
 import pytorch_lightning as L
-from albumentations import Compose
 from torch.utils.data import DataLoader
 from torch.utils.data.dataloader import default_collate
 
 from careamics.config import InferenceConfig
 from careamics.config.support import SupportedData
 from careamics.config.tile_information import TileInformation
 from careamics.dataset.dataset_utils import (
@@ -35,15 +35,15 @@
     CAREamics prediction dataloader returns tuples of arrays and TileInformation. In
     case of non-tiled data, this function will return the arrays. In case of tiled data,
     it will return the arrays, the last tile flag, the overlap crop coordinates and the
     stitch coordinates.
 
     Parameters
     ----------
-    batch : Tuple[Tuple[np.ndarray, TileInformation], ...]
+    batch : List[Tuple[np.ndarray, TileInformation], ...]
         Batch of tiles.
 
     Returns
     -------
     Any
         Collated batch.
     """
@@ -253,33 +253,38 @@
     and are coherent.
 
     The data module can be used with Path, str or numpy arrays. To use array data, set
     `data_type` to `array` and pass a numpy array to `train_data`.
 
     The default transformations applied to the images are defined in
     `careamics.config.inference_model`. To use different transformations, pass a list
-    of transforms or an albumentation `Compose` as `transforms` parameter. See examples
+    of transforms. See examples
     for more details.
 
     The `mean` and `std` parameters are only used if Normalization is defined either
-    in the default transformations or in the `transforms` parameter, but not with
-    a `Compose` object. If you pass a `Normalization` transform in a list as
-    `transforms`, then the mean and std parameters will be overwritten by those passed
-    to this method.
+    in the default transformations or in the `transforms` parameter. If you pass a
+    `Normalization` transform in a list as `transforms`, then the mean and std
+    parameters will be overwritten by those passed to this method.
 
     By default, CAREamics only supports types defined in
     `careamics.config.support.SupportedData`. To read custom data types, you can set
     `data_type` to `custom` and provide a function that returns a numpy array from a
     path. Additionally, pass a `fnmatch` and `Path.rglob` compatible expression
     (e.g. "*.jpeg") to filter the files extension using `extension_filter`.
 
     In `dataloader_params`, you can pass any parameter accepted by PyTorch
     dataloaders, except for `batch_size`, which is set by the `batch_size`
     parameter.
 
+    Note that if you are using a UNet model and tiling, the tile size must be
+    divisible in every dimension by 2**d, where d is the depth of the model. This
+    avoids artefacts arising from the broken shift invariance induced by the
+    pooling layers of the UNet. If your image has less dimensions, as it may
+    happen in the Z dimension, consider padding your image.
+
     Parameters
     ----------
     pred_data : Union[str, Path, np.ndarray]
         Prediction data.
     data_type : Union[Literal["array", "tiff", "custom"], SupportedData]
         Data type, see `SupportedData` for available options.
     mean : float
@@ -294,15 +299,15 @@
         Tile overlap, 2D or 3D tile overlap.
     axes : str
         Axes of the data, choosen amongst SCZYX.
     batch_size : int
         Batch size.
     tta_transforms : bool, optional
         Use test time augmentation, by default True.
-    transforms : Optional[Union[List[TRANSFORMS_UNION], Compose]], optional
+    transforms : List, optional
         List of transforms to apply to prediction patches. If None, default
         transforms are applied.
     read_source_func : Optional[Callable], optional
         Function to read the source data, used if `data_type` is `custom`, by
         default None.
     extension_filter : str, optional
         Filter for file extensions, used if `data_type` is `custom`, by default "".
@@ -317,15 +322,15 @@
         mean: float,
         std: float,
         tile_size: Optional[Tuple[int, ...]] = None,
         tile_overlap: Optional[Tuple[int, ...]] = None,
         axes: str = "YX",
         batch_size: int = 1,
         tta_transforms: bool = True,
-        transforms: Optional[Union[List, Compose]] = None,
+        transforms: Optional[List] = None,
         read_source_func: Optional[Callable] = None,
         extension_filter: str = "",
         dataloader_params: Optional[dict] = None,
     ) -> None:
         """
         Constructor.
 
@@ -347,15 +352,15 @@
             Tile overlap, 2D or 3D tile overlap.
         axes : str
             Axes of the data, choosen amongst SCZYX.
         batch_size : int
             Batch size.
         tta_transforms : bool, optional
             Use test time augmentation, by default True.
-        transforms : Optional[Union[List[TRANSFORMS_UNION], Compose]], optional
+        transforms : Optional[List], optional
             List of transforms to apply to prediction patches. If None, default
             transforms are applied.
         read_source_func : Optional[Callable], optional
             Function to read the source data, used if `data_type` is `custom`, by
             default None.
         extension_filter : str, optional
             Filter for file extensions, used if `data_type` is `custom`, by default "".
```

### Comparing `careamics-0.1.0rc4/src/careamics/lightning_prediction_loop.py` & `careamics-0.1.0rc5/src/careamics/lightning_prediction_loop.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/src/careamics/callbacks/hyperparameters_callback.py` & `careamics-0.1.0rc5/src/careamics/callbacks/hyperparameters_callback.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/src/careamics/callbacks/progress_bar_callback.py` & `careamics-0.1.0rc5/src/careamics/callbacks/progress_bar_callback.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/src/careamics/config/__init__.py` & `careamics-0.1.0rc5/src/careamics/config/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Configuration module."""
 
-
 __all__ = [
     "AlgorithmConfig",
     "DataConfig",
     "Configuration",
     "CheckpointModel",
     "InferenceConfig",
     "load_configuration",
```

### Comparing `careamics-0.1.0rc4/src/careamics/config/algorithm_model.py` & `careamics-0.1.0rc5/src/careamics/config/algorithm_model.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/src/careamics/config/callback_model.py` & `careamics-0.1.0rc5/src/careamics/config/callback_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Checkpoint saving configuration."""
+
 from __future__ import annotations
 
 from datetime import timedelta
 from typing import Literal, Optional
 
 from pydantic import (
     BaseModel,
```

### Comparing `careamics-0.1.0rc4/src/careamics/config/configuration_example.py` & `careamics-0.1.0rc5/src/careamics/config/configuration_example.py`

 * *Files 19% similar despite different names*

```diff
@@ -53,19 +53,17 @@
         axes="YX",
         transforms=[
             {
                 "name": SupportedTransform.NORMALIZE.value,
             },
             {
                 "name": SupportedTransform.NDFLIP.value,
-                "is_3D": False,
             },
             {
                 "name": SupportedTransform.XY_RANDOM_ROTATE90.value,
-                "is_3D": False,
             },
             {
                 "name": SupportedTransform.N2V_MANIPULATE.value,
                 "roi_size": 11,
                 "masked_pixel_percentage": 0.2,
                 "strategy": SupportedPixelManipulation.MEDIAN.value,
             },
```

### Comparing `careamics-0.1.0rc4/src/careamics/config/configuration_factory.py` & `careamics-0.1.0rc5/src/careamics/config/configuration_factory.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 """Convenience functions to create configurations for training and inference."""
 
 from typing import Any, Dict, List, Literal, Optional, Tuple, Union
 
-from albumentations import Compose
-
 from .algorithm_model import AlgorithmConfig
 from .architectures import UNetModel
 from .configuration_model import Configuration
 from .data_model import DataConfig
 from .inference_model import InferenceConfig
 from .support import (
     SupportedAlgorithm,
@@ -24,16 +22,18 @@
     experiment_name: str,
     data_type: Literal["array", "tiff", "custom"],
     axes: str,
     patch_size: List[int],
     batch_size: int,
     num_epochs: int,
     use_augmentations: bool = True,
+    independent_channels: bool = False,
     loss: Literal["mae", "mse"] = "mae",
-    n_channels: int = -1,
+    n_channels_in: int = 1,
+    n_channels_out: int = 1,
     logger: Literal["wandb", "tensorboard", "none"] = "none",
     model_kwargs: Optional[dict] = None,
 ) -> Configuration:
     """
     Create a configuration for training CARE or Noise2Noise.
 
     Parameters
@@ -50,46 +50,51 @@
         Size of the patches along the spatial dimensions (e.g. [64, 64]).
     batch_size : int
         Batch size.
     num_epochs : int
         Number of epochs.
     use_augmentations : bool, optional
         Whether to use augmentations, by default True.
+    independent_channels : bool, optional
+        Whether to train all channels independently, by default False.
     loss : Literal["mae", "mse"], optional
         Loss function to use, by default "mae".
-    n_channels : int, optional
-        Number of channels (in and out), by default -1.
+    n_channels_in : int, optional
+        Number of channels in, by default 1.
+    n_channels_out : int, optional
+        Number of channels out, by default 1.
     logger : Literal["wandb", "tensorboard", "none"], optional
         Logger to use, by default "none".
     model_kwargs : dict, optional
         UNetModel parameters, by default {}.
 
     Returns
     -------
     Configuration
         Configuration for training CARE or Noise2Noise.
     """
     # if there are channels, we need to specify their number
-    if "C" in axes and n_channels == 1:
+    if "C" in axes and n_channels_in == 1:
         raise ValueError(
-            f"Number of channels must be specified when using channels "
-            f"(got {n_channels} channel)."
+            f"Number of channels in must be specified when using channels "
+            f"(got {n_channels_in} channel)."
         )
-    elif "C" not in axes and n_channels > 1:
+    elif "C" not in axes and n_channels_in > 1:
         raise ValueError(
             f"C is not present in the axes, but number of channels is specified "
-            f"(got {n_channels} channel)."
+            f"(got {n_channels_in} channels)."
         )
 
     # model
     if model_kwargs is None:
         model_kwargs = {}
     model_kwargs["conv_dims"] = 3 if "Z" in axes else 2
-    model_kwargs["in_channels"] = n_channels
-    model_kwargs["num_classes"] = n_channels
+    model_kwargs["in_channels"] = n_channels_in
+    model_kwargs["num_classes"] = n_channels_out
+    model_kwargs["independent_channels"] = independent_channels
 
     unet_model = UNetModel(
         architecture=SupportedArchitecture.UNET.value,
         **model_kwargs,
     )
 
     # algorithm model
@@ -150,29 +155,37 @@
     experiment_name: str,
     data_type: Literal["array", "tiff", "custom"],
     axes: str,
     patch_size: List[int],
     batch_size: int,
     num_epochs: int,
     use_augmentations: bool = True,
+    independent_channels: bool = False,
     loss: Literal["mae", "mse"] = "mae",
-    n_channels: int = 1,
+    n_channels_in: int = 1,
+    n_channels_out: int = -1,
     logger: Literal["wandb", "tensorboard", "none"] = "none",
     model_kwargs: Optional[dict] = None,
 ) -> Configuration:
     """
     Create a configuration for training CARE.
 
     If "Z" is present in `axes`, then `path_size` must be a list of length 3, otherwise
     2.
 
-    If "C" is present in `axes`, then you need to set `n_channels` to the number of
+    If "C" is present in `axes`, then you need to set `n_channels_in` to the number of
     channels. Likewise, if you set the number of channels, then "C" must be present in
     `axes`.
 
+    To set the number of output channels, use the `n_channels_out` parameter. If it is
+    not specified, it will be assumed to be equal to `n_channels_in`.
+
+    By default, all channels are trained together. To train all channels independently,
+    set `independent_channels` to True.
+
     By setting `use_augmentations` to False, the only transformation applied will be
     normalization.
 
     Parameters
     ----------
     experiment_name : str
         Name of the experiment.
@@ -184,53 +197,62 @@
         Size of the patches along the spatial dimensions (e.g. [64, 64]).
     batch_size : int
         Batch size.
     num_epochs : int
         Number of epochs.
     use_augmentations : bool, optional
         Whether to use augmentations, by default True.
+    independent_channels : bool, optional
+        Whether to train all channels independently, by default False.
     loss : Literal["mae", "mse"], optional
         Loss function to use, by default "mae".
-    n_channels : int, optional
-        Number of channels (in and out), by default 1.
+    n_channels_in : int, optional
+        Number of channels in, by default 1.
+    n_channels_out : int, optional
+        Number of channels out, by default -1.
     logger : Literal["wandb", "tensorboard", "none"], optional
         Logger to use, by default "none".
     model_kwargs : dict, optional
         UNetModel parameters, by default {}.
 
     Returns
     -------
     Configuration
         Configuration for training CARE.
     """
+    if n_channels_out == -1:
+        n_channels_out = n_channels_in
+
     return _create_supervised_configuration(
         algorithm="care",
         experiment_name=experiment_name,
         data_type=data_type,
         axes=axes,
         patch_size=patch_size,
         batch_size=batch_size,
         num_epochs=num_epochs,
         use_augmentations=use_augmentations,
+        independent_channels=independent_channels,
         loss=loss,
-        # TODO in the future we might support different in and out channels for CARE
-        n_channels=n_channels,
+        n_channels_in=n_channels_in,
+        n_channels_out=n_channels_out,
         logger=logger,
         model_kwargs=model_kwargs,
     )
 
 
 def create_n2n_configuration(
     experiment_name: str,
     data_type: Literal["array", "tiff", "custom"],
     axes: str,
     patch_size: List[int],
     batch_size: int,
     num_epochs: int,
     use_augmentations: bool = True,
+    independent_channels: bool = False,
     loss: Literal["mae", "mse"] = "mae",
     n_channels: int = 1,
     logger: Literal["wandb", "tensorboard", "none"] = "none",
     model_kwargs: Optional[dict] = None,
 ) -> Configuration:
     """
     Create a configuration for training Noise2Noise.
@@ -238,14 +260,17 @@
     If "Z" is present in `axes`, then `path_size` must be a list of length 3, otherwise
     2.
 
     If "C" is present in `axes`, then you need to set `n_channels` to the number of
     channels. Likewise, if you set the number of channels, then "C" must be present in
     `axes`.
 
+    By default, all channels are trained together. To train all channels independently,
+    set `independent_channels` to True.
+
     By setting `use_augmentations` to False, the only transformation applied will be
     normalization.
 
     Parameters
     ----------
     experiment_name : str
         Name of the experiment.
@@ -257,14 +282,16 @@
         Size of the patches along the spatial dimensions (e.g. [64, 64]).
     batch_size : int
         Batch size.
     num_epochs : int
         Number of epochs.
     use_augmentations : bool, optional
         Whether to use augmentations, by default True.
+    independent_channels : bool, optional
+        Whether to train all channels independently, by default False.
     loss : Literal["mae", "mse"], optional
         Loss function to use, by default "mae".
     n_channels : int, optional
         Number of channels (in and out), by default 1.
     logger : Literal["wandb", "tensorboard", "none"], optional
         Logger to use, by default "none".
     model_kwargs : dict, optional
@@ -280,29 +307,32 @@
         experiment_name=experiment_name,
         data_type=data_type,
         axes=axes,
         patch_size=patch_size,
         batch_size=batch_size,
         num_epochs=num_epochs,
         use_augmentations=use_augmentations,
+        independent_channels=independent_channels,
         loss=loss,
-        n_channels=n_channels,
+        n_channels_in=n_channels,
+        n_channels_out=n_channels,
         logger=logger,
         model_kwargs=model_kwargs,
     )
 
 
 def create_n2v_configuration(
     experiment_name: str,
     data_type: Literal["array", "tiff", "custom"],
     axes: str,
     patch_size: List[int],
     batch_size: int,
     num_epochs: int,
     use_augmentations: bool = True,
+    independent_channels: bool = True,
     use_n2v2: bool = False,
     n_channels: int = 1,
     roi_size: int = 11,
     masked_pixel_percentage: float = 0.2,
     struct_n2v_axis: Literal["horizontal", "vertical", "none"] = "none",
     struct_n2v_span: int = 5,
     logger: Literal["wandb", "tensorboard", "none"] = "none",
@@ -316,19 +346,22 @@
     (structN2V) parameters, or set `use_n2v2` to True (N2V2).
 
     N2V2 modifies the UNet architecture by adding blur pool layers and removes the skip
     connections, thus removing checkboard artefacts. StructN2V is used when vertical
     or horizontal correlations are present in the noise; it applies an additional mask
     to the manipulated pixel neighbors.
 
+    If "Z" is present in `axes`, then `path_size` must be a list of length 3, otherwise
+    2.
+
     If "C" is present in `axes`, then you need to set `n_channels` to the number of
     channels.
 
-    If "Z" is present in `axes`, then `path_size` must be a list of length 3, otherwise
-    2.
+    By default, all channels are trained independently. To train all channels together,
+    set `independent_channels` to False.
 
     By setting `use_augmentations` to False, the only transformations applied will be
     normalization and N2V manipulation.
 
     The `roi_size` parameter specifies the size of the area around each pixel that will
     be manipulated by N2V. The `masked_pixel_percentage` parameter specifies how many
     pixels per patch will be manipulated.
@@ -352,14 +385,16 @@
         Size of the patches along the spatial dimensions (e.g. [64, 64]).
     batch_size : int
         Batch size.
     num_epochs : int
         Number of epochs.
     use_augmentations : bool, optional
         Whether to use augmentations, by default True.
+    independent_channels : bool, optional
+        Whether to train all channels together, by default True.
     use_n2v2 : bool, optional
         Whether to use N2V2, by default False.
     n_channels : int, optional
         Number of channels (in and out), by default 1.
     roi_size : int, optional
         N2V pixel manipulation area, by default 11.
     masked_pixel_percentage : float, optional
@@ -410,23 +445,36 @@
     ...     patch_size=[64, 64],
     ...     batch_size=32,
     ...     num_epochs=100,
     ...     struct_n2v_axis="horizontal",
     ...     struct_n2v_span=7
     ... )
 
-    If you are training multiple channels together, then you need to specify the number
-    of channels:
+    If you are training multiple channels independently, then you need to specify the
+    number of channels:
+    >>> config = create_n2v_configuration(
+    ...     experiment_name="n2v_experiment",
+    ...     data_type="array",
+    ...     axes="YXC",
+    ...     patch_size=[64, 64],
+    ...     batch_size=32,
+    ...     num_epochs=100,
+    ...     n_channels=3
+    ... )
+
+    If instead you want to train multiple channels together, you need to turn off the
+    `independent_channels` parameter:
     >>> config = create_n2v_configuration(
     ...     experiment_name="n2v_experiment",
     ...     data_type="array",
     ...     axes="YXC",
     ...     patch_size=[64, 64],
     ...     batch_size=32,
     ...     num_epochs=100,
+    ...     independent_channels=False,
     ...     n_channels=3
     ... )
 
     To turn off the augmentations, except normalization and N2V manipulation, use the
     relevant keyword argument:
     >>> config = create_n2v_configuration(
     ...     experiment_name="n2v_experiment",
@@ -453,14 +501,15 @@
     # model
     if model_kwargs is None:
         model_kwargs = {}
     model_kwargs["n2v2"] = use_n2v2
     model_kwargs["conv_dims"] = 3 if "Z" in axes else 2
     model_kwargs["in_channels"] = n_channels
     model_kwargs["num_classes"] = n_channels
+    model_kwargs["independent_channels"] = independent_channels
 
     unet_model = UNetModel(
         architecture=SupportedArchitecture.UNET.value,
         **model_kwargs,
     )
 
     # algorithm model
@@ -489,17 +538,19 @@
                 "name": SupportedTransform.NORMALIZE.value,
             },
         ]
 
     # n2v2 and structn2v
     nv2_transform = {
         "name": SupportedTransform.N2V_MANIPULATE.value,
-        "strategy": SupportedPixelManipulation.MEDIAN.value
-        if use_n2v2
-        else SupportedPixelManipulation.UNIFORM.value,
+        "strategy": (
+            SupportedPixelManipulation.MEDIAN.value
+            if use_n2v2
+            else SupportedPixelManipulation.UNIFORM.value
+        ),
         "roi_size": roi_size,
         "masked_pixel_percentage": masked_pixel_percentage,
         "struct_mask_axis": struct_n2v_axis,
         "struct_mask_span": struct_n2v_span,
     }
     transforms.append(nv2_transform)
 
@@ -526,72 +577,91 @@
         data_config=data,
         training_config=training,
     )
 
     return configuration
 
 
-# TODO add tests
 def create_inference_configuration(
-    training_configuration: Configuration,
+    configuration: Configuration,
     tile_size: Optional[Tuple[int, ...]] = None,
     tile_overlap: Optional[Tuple[int, ...]] = None,
     data_type: Optional[Literal["array", "tiff", "custom"]] = None,
     axes: Optional[str] = None,
-    transforms: Optional[Union[List[Dict[str, Any]], Compose]] = None,
+    transforms: Optional[Union[List[Dict[str, Any]]]] = None,
     tta_transforms: bool = True,
     batch_size: Optional[int] = 1,
 ) -> InferenceConfig:
     """
     Create a configuration for inference with N2V.
 
     If not provided, `data_type` and `axes` are taken from the training
     configuration. If `transforms` are not provided, only normalization is applied.
 
     Parameters
     ----------
-    training_configuration : Configuration
-        Configuration used for training.
+    configuration : Configuration
+        Global configuration.
     tile_size : Tuple[int, ...], optional
         Size of the tiles.
     tile_overlap : Tuple[int, ...], optional
         Overlap of the tiles.
     data_type : str, optional
         Type of the data, by default "tiff".
     axes : str, optional
         Axes of the data, by default "YX".
-    transforms : List[Dict[str, Any]] or Compose, optional
+    transforms : List[Dict[str, Any]], optional
         Transformations to apply to the data, by default None.
     tta_transforms : bool, optional
         Whether to apply test-time augmentations, by default True.
     batch_size : int, optional
         Batch size, by default 1.
 
     Returns
     -------
     InferenceConfiguration
-        Configuration for inference with N2V.
+        Configuration used to configure CAREamicsPredictData.
     """
-    if (
-        training_configuration.data_config.mean is None
-        or training_configuration.data_config.std is None
-    ):
-        raise ValueError("Mean and std must be provided in the training configuration.")
+    if configuration.data_config.mean is None or configuration.data_config.std is None:
+        raise ValueError("Mean and std must be provided in the configuration.")
 
+    # minimum transform
     if transforms is None:
         transforms = [
             {
                 "name": SupportedTransform.NORMALIZE.value,
             },
         ]
 
+    # tile size for UNets
+    if tile_size is not None:
+        model = configuration.algorithm_config.model
+
+        if model.architecture == SupportedArchitecture.UNET.value:
+            # tile size must be equal to k*2^n, where n is the number of pooling layers
+            # (equal to the depth) and k is an integer
+            depth = model.depth
+            tile_increment = 2**depth
+
+            for i, t in enumerate(tile_size):
+                if t % tile_increment != 0:
+                    raise ValueError(
+                        f"Tile size must be divisible by {tile_increment} along all "
+                        f"axes (got {t} for axis {i}). If your image size is smaller "
+                        f"along one axis (e.g. Z), consider padding the image."
+                    )
+
+        # tile overlaps must be specified
+        if tile_overlap is None:
+            raise ValueError("Tile overlap must be specified.")
+
     return InferenceConfig(
-        data_type=data_type or training_configuration.data_config.data_type,
+        data_type=data_type or configuration.data_config.data_type,
         tile_size=tile_size,
         tile_overlap=tile_overlap,
-        axes=axes or training_configuration.data_config.axes,
-        mean=training_configuration.data_config.mean,
-        std=training_configuration.data_config.std,
+        axes=axes or configuration.data_config.axes,
+        mean=configuration.data_config.mean,
+        std=configuration.data_config.std,
         transforms=transforms,
         tta_transforms=tta_transforms,
         batch_size=batch_size,
     )
```

### Comparing `careamics-0.1.0rc4/src/careamics/config/configuration_model.py` & `careamics-0.1.0rc5/src/careamics/config/configuration_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Pydantic CAREamics configuration."""
+
 from __future__ import annotations
 
 import re
 from pathlib import Path
 from pprint import pformat
 from typing import Dict, List, Literal, Union
 
@@ -234,33 +235,30 @@
 
         Returns
         -------
         Self
             Validated configuration.
         """
         if self.algorithm_config.algorithm == SupportedAlgorithm.N2V:
-            # if we have a list of transform (as opposed to Compose)
-            if self.data_config.has_transform_list():
-                # missing N2V_MANIPULATE
-                if not self.data_config.has_n2v_manipulate():
-                    self.data_config.transforms.append(
-                        N2VManipulateModel(
-                            name=SupportedTransform.N2V_MANIPULATE.value,
-                        )
+            # missing N2V_MANIPULATE
+            if not self.data_config.has_n2v_manipulate():
+                self.data_config.transforms.append(
+                    N2VManipulateModel(
+                        name=SupportedTransform.N2V_MANIPULATE.value,
                     )
+                )
 
-                median = SupportedPixelManipulation.MEDIAN.value
-                uniform = SupportedPixelManipulation.UNIFORM.value
-                strategy = median if self.algorithm_config.model.n2v2 else uniform
-                self.data_config.set_N2V2_strategy(strategy)
+            median = SupportedPixelManipulation.MEDIAN.value
+            uniform = SupportedPixelManipulation.UNIFORM.value
+            strategy = median if self.algorithm_config.model.n2v2 else uniform
+            self.data_config.set_N2V2_strategy(strategy)
         else:
-            # if we have a list of transform, remove N2V manipulate if present
-            if self.data_config.has_transform_list():
-                if self.data_config.has_n2v_manipulate():
-                    self.data_config.remove_n2v_manipulate()
+            # remove N2V manipulate if present
+            if self.data_config.has_n2v_manipulate():
+                self.data_config.remove_n2v_manipulate()
 
         return self
 
     def __str__(self) -> str:
         """
         Pretty string reprensenting the configuration.
```

### Comparing `careamics-0.1.0rc4/src/careamics/config/data_model.py` & `careamics-0.1.0rc5/src/careamics/config/data_model.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Data configuration."""
+
 from __future__ import annotations
 
 from pprint import pformat
 from typing import Any, List, Literal, Optional, Union
 
-from albumentations import Compose
 from pydantic import (
     BaseModel,
     ConfigDict,
     Discriminator,
     Field,
     field_validator,
     model_validator,
@@ -67,38 +67,35 @@
     ...         {
     ...             "name": SupportedTransform.NORMALIZE.value,
     ...             "mean": 167.6,
     ...             "std": 47.2,
     ...         },
     ...         {
     ...             "name": "NDFlip",
-    ...             "is_3D": True,
-    ...             "flip_z": True,
     ...         }
     ...     ]
     ... )
     """
 
     # Pydantic class configuration
     model_config = ConfigDict(
         validate_assignment=True,
-        arbitrary_types_allowed=True,  # Allow Compose declaration
     )
 
     # Dataset configuration
     data_type: Literal["array", "tiff", "custom"]  # As defined in SupportedData
     patch_size: Union[List[int]] = Field(..., min_length=2, max_length=3)
     batch_size: int = Field(default=1, ge=1, validate_default=True)
     axes: str
 
     # Optional fields
     mean: Optional[float] = None
     std: Optional[float] = None
 
-    transforms: Union[List[TRANSFORMS_UNION], Compose] = Field(
+    transforms: List[TRANSFORMS_UNION] = Field(
         default=[
             {
                 "name": SupportedTransform.NORMALIZE.value,
             },
             {
                 "name": SupportedTransform.NDFLIP.value,
             },
@@ -177,51 +174,50 @@
         check_axes_validity(axes)
 
         return axes
 
     @field_validator("transforms")
     @classmethod
     def validate_prediction_transforms(
-        cls, transforms: Union[List[TRANSFORMS_UNION], Compose]
-    ) -> Union[List[TRANSFORMS_UNION], Compose]:
+        cls, transforms: List[TRANSFORMS_UNION]
+    ) -> List[TRANSFORMS_UNION]:
         """
         Validate N2VManipulate transform position in the transform list.
 
         Parameters
         ----------
-        transforms : Union[List[Transformations_Union], Compose]
+        transforms : List[Transformations_Union]
             Transforms.
 
         Returns
         -------
-        Union[List[Transformations_Union], Compose]
+        List[TRANSFORMS_UNION]
             Validated transforms.
 
         Raises
         ------
         ValueError
             If multiple instances of N2VManipulate are found.
         """
-        if not isinstance(transforms, Compose):
-            transform_list = [t.name for t in transforms]
+        transform_list = [t.name for t in transforms]
+
+        if SupportedTransform.N2V_MANIPULATE in transform_list:
+            # multiple N2V_MANIPULATE
+            if transform_list.count(SupportedTransform.N2V_MANIPULATE) > 1:
+                raise ValueError(
+                    f"Multiple instances of "
+                    f"{SupportedTransform.N2V_MANIPULATE} transforms "
+                    f"are not allowed."
+                )
 
-            if SupportedTransform.N2V_MANIPULATE in transform_list:
-                # multiple N2V_MANIPULATE
-                if transform_list.count(SupportedTransform.N2V_MANIPULATE) > 1:
-                    raise ValueError(
-                        f"Multiple instances of "
-                        f"{SupportedTransform.N2V_MANIPULATE} transforms "
-                        f"are not allowed."
-                    )
-
-                # N2V_MANIPULATE not the last transform
-                elif transform_list[-1] != SupportedTransform.N2V_MANIPULATE:
-                    index = transform_list.index(SupportedTransform.N2V_MANIPULATE)
-                    transform = transforms.pop(index)
-                    transforms.append(transform)
+            # N2V_MANIPULATE not the last transform
+            elif transform_list[-1] != SupportedTransform.N2V_MANIPULATE:
+                index = transform_list.index(SupportedTransform.N2V_MANIPULATE)
+                transform = transforms.pop(index)
+                transforms.append(transform)
 
         return transforms
 
     @model_validator(mode="after")
     def std_only_with_mean(self: Self) -> Self:
         """
         Check that mean and std are either both None, or both specified.
@@ -252,19 +248,18 @@
         Returns
         -------
         Self
             Data model with mean and std added to the Normalize transform.
         """
         if self.mean is not None or self.std is not None:
             # search in the transforms for Normalize and update parameters
-            if self.has_transform_list():
-                for transform in self.transforms:
-                    if transform.name == SupportedTransform.NORMALIZE.value:
-                        transform.mean = self.mean
-                        transform.std = self.std
+            for transform in self.transforms:
+                if transform.name == SupportedTransform.NORMALIZE.value:
+                    transform.mean = self.mean
+                    transform.std = self.std
 
         return self
 
     @model_validator(mode="after")
     def validate_dimensions(self: Self) -> Self:
         """
         Validate 2D/3D dimensions between axes, patch size and transforms.
@@ -282,35 +277,21 @@
         if "Z" in self.axes:
             if len(self.patch_size) != 3:
                 raise ValueError(
                     f"Patch size must have 3 dimensions if the data is 3D "
                     f"({self.axes})."
                 )
 
-            if self.has_transform_list():
-                for transform in self.transforms:
-                    if transform.name == SupportedTransform.NDFLIP:
-                        transform.is_3D = True
-                    elif transform.name == SupportedTransform.XY_RANDOM_ROTATE90:
-                        transform.is_3D = True
-
         else:
             if len(self.patch_size) != 2:
                 raise ValueError(
                     f"Patch size must have 3 dimensions if the data is 3D "
                     f"({self.axes})."
                 )
 
-            if self.has_transform_list():
-                for transform in self.transforms:
-                    if transform.name == SupportedTransform.NDFLIP:
-                        transform.is_3D = False
-                    elif transform.name == SupportedTransform.XY_RANDOM_ROTATE90:
-                        transform.is_3D = False
-
         return self
 
     def __str__(self) -> str:
         """
         Pretty string reprensenting the configuration.
 
         Returns
@@ -328,92 +309,39 @@
         ----------
         **kwargs : Any
             Keyword arguments to update.
         """
         self.__dict__.update(kwargs)
         self.__class__.model_validate(self.__dict__)
 
-    def has_transform_list(self) -> bool:
-        """
-        Check if the transforms are a list, as opposed to a Compose object.
-
-        Returns
-        -------
-        bool
-            True if the transforms are a list, False otherwise.
-        """
-        return isinstance(self.transforms, list)
-
     def has_n2v_manipulate(self) -> bool:
         """
         Check if the transforms contain N2VManipulate.
 
-        Use `has_transform_list` to check if the transforms are a list.
-
         Returns
         -------
         bool
             True if the transforms contain N2VManipulate, False otherwise.
-
-        Raises
-        ------
-        ValueError
-            If the transforms are a Compose object.
         """
-        if self.has_transform_list():
-            return any(
-                transform.name == SupportedTransform.N2V_MANIPULATE.value
-                for transform in self.transforms
-            )
-        else:
-            raise ValueError(
-                "Checking for N2VManipulate with Compose transforms is not allowed. "
-                "Check directly in the Compose."
-            )
+        return any(
+            transform.name == SupportedTransform.N2V_MANIPULATE.value
+            for transform in self.transforms
+        )
 
     def add_n2v_manipulate(self) -> None:
-        """
-        Add N2VManipulate to the transforms.
-
-        Use `has_transform_list` to check if the transforms are a list.
-
-        Raises
-        ------
-        ValueError
-            If the transforms are a Compose object.
-        """
-        if self.has_transform_list():
-            if not self.has_n2v_manipulate():
-                self.transforms.append(
-                    N2VManipulateModel(name=SupportedTransform.N2V_MANIPULATE.value)
-                )
-        else:
-            raise ValueError(
-                "Adding N2VManipulate with Compose transforms is not allowed. Add "
-                "N2VManipulate directly to the transform in the Compose."
+        """Add N2VManipulate to the transforms."""
+        if not self.has_n2v_manipulate():
+            self.transforms.append(
+                N2VManipulateModel(name=SupportedTransform.N2V_MANIPULATE.value)
             )
 
     def remove_n2v_manipulate(self) -> None:
-        """
-        Remove N2VManipulate from the transforms.
-
-        Use `has_transform_list` to check if the transforms are a list.
-
-        Raises
-        ------
-        ValueError
-            If the transforms are a Compose object.
-        """
-        if self.has_transform_list() and self.has_n2v_manipulate():
+        """Remove N2VManipulate from the transforms."""
+        if self.has_n2v_manipulate():
             self.transforms.pop(-1)
-        else:
-            raise ValueError(
-                "Removing N2VManipulate with Compose transforms is not allowed. Remove "
-                "N2VManipulate directly from the transform in the Compose."
-            )
 
     def set_mean_and_std(self, mean: float, std: float) -> None:
         """
         Set mean and standard deviation of the data.
 
         This method should be used instead setting the fields directly, as it would
         otherwise trigger a validation error.
@@ -424,24 +352,18 @@
             Mean of the data.
         std : float
             Standard deviation of the data.
         """
         self._update(mean=mean, std=std)
 
         # search in the transforms for Normalize and update parameters
-        if self.has_transform_list():
-            for transform in self.transforms:
-                if transform.name == SupportedTransform.NORMALIZE.value:
-                    transform.mean = mean
-                    transform.std = std
-        else:
-            raise ValueError(
-                "Setting mean and std with Compose transforms is not allowed. Add "
-                "mean and std parameters directly to the transform in the Compose."
-            )
+        for transform in self.transforms:
+            if transform.name == SupportedTransform.NORMALIZE.value:
+                transform.mean = mean
+                transform.std = std
 
     def set_3D(self, axes: str, patch_size: List[int]) -> None:
         """
         Set 3D parameters.
 
         Parameters
         ----------
@@ -461,16 +383,14 @@
         use_n2v2 : bool
             Whether to use N2V2.
 
         Raises
         ------
         ValueError
             If the N2V pixel manipulate transform is not found in the transforms.
-        ValueError
-            If the transforms are a Compose object.
         """
         if use_n2v2:
             self.set_N2V2_strategy("median")
         else:
             self.set_N2V2_strategy("uniform")
 
     def set_N2V2_strategy(self, strategy: Literal["uniform", "median"]) -> None:
@@ -482,36 +402,27 @@
         strategy : Literal["uniform", "median"]
             Strategy to use for N2V2.
 
         Raises
         ------
         ValueError
             If the N2V pixel manipulate transform is not found in the transforms.
-        ValueError
-            If the transforms are a Compose object.
         """
-        if isinstance(self.transforms, list):
-            found_n2v = False
+        found_n2v = False
 
-            for transform in self.transforms:
-                if transform.name == SupportedTransform.N2V_MANIPULATE.value:
-                    transform.strategy = strategy
-                    found_n2v = True
-
-            if not found_n2v:
-                transforms = [t.name for t in self.transforms]
-                raise ValueError(
-                    f"N2V_Manipulate transform not found in the transforms list "
-                    f"({transforms})."
-                )
+        for transform in self.transforms:
+            if transform.name == SupportedTransform.N2V_MANIPULATE.value:
+                transform.strategy = strategy
+                found_n2v = True
 
-        else:
+        if not found_n2v:
+            transforms = [t.name for t in self.transforms]
             raise ValueError(
-                "Setting N2V2 strategy with Compose transforms is not allowed. Add "
-                "N2V2 strategy parameters directly to the transform in the Compose."
+                f"N2V_Manipulate transform not found in the transforms list "
+                f"({transforms})."
             )
 
     def set_structN2V_mask(
         self, mask_axis: Literal["horizontal", "vertical", "none"], mask_span: int
     ) -> None:
         """
         Set structN2V mask parameters.
@@ -525,31 +436,22 @@
         mask_span : int
             Total span of the mask in pixels.
 
         Raises
         ------
         ValueError
             If the N2V pixel manipulate transform is not found in the transforms.
-        ValueError
-            If the transforms are a Compose object.
         """
-        if isinstance(self.transforms, list):
-            found_n2v = False
+        found_n2v = False
 
-            for transform in self.transforms:
-                if transform.name == SupportedTransform.N2V_MANIPULATE.value:
-                    transform.struct_mask_axis = mask_axis
-                    transform.struct_mask_span = mask_span
-                    found_n2v = True
+        for transform in self.transforms:
+            if transform.name == SupportedTransform.N2V_MANIPULATE.value:
+                transform.struct_mask_axis = mask_axis
+                transform.struct_mask_span = mask_span
+                found_n2v = True
 
-            if not found_n2v:
-                transforms = [t.name for t in self.transforms]
-                raise ValueError(
-                    f"N2V pixel manipulate transform not found in the transforms "
-                    f"({transforms})."
-                )
-
-        else:
+        if not found_n2v:
+            transforms = [t.name for t in self.transforms]
             raise ValueError(
-                "Setting structN2VMask with Compose transforms is not allowed. Add "
-                "structN2VMask parameters directly to the transform in the Compose."
+                f"N2V pixel manipulate transform not found in the transforms "
+                f"({transforms})."
             )
```

### Comparing `careamics-0.1.0rc4/src/careamics/config/inference_model.py` & `careamics-0.1.0rc5/src/careamics/config/inference_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Pydantic model representing CAREamics prediction configuration."""
+
 from __future__ import annotations
 
 from typing import Any, List, Literal, Optional, Union
 
-from albumentations import Compose
 from pydantic import BaseModel, ConfigDict, Field, field_validator, model_validator
 from typing_extensions import Self
 
 from .support import SupportedTransform
 from .transformations.normalize_model import NormalizeModel
 from .validators import check_axes_validity, patch_size_ge_than_8_power_of_2
 
@@ -29,15 +29,15 @@
     )
 
     axes: str
 
     mean: float
     std: float = Field(..., ge=0.0)
 
-    transforms: Union[List[TRANSFORMS_UNION], Compose] = Field(
+    transforms: List[TRANSFORMS_UNION] = Field(
         default=[
             {
                 "name": SupportedTransform.NORMALIZE.value,
             },
         ],
         validate_default=True,
     )
@@ -47,49 +47,49 @@
 
     # Dataloader parameters
     batch_size: int = Field(default=1, ge=1)
 
     @field_validator("tile_overlap")
     @classmethod
     def all_elements_non_zero_even(
-        cls, patch_list: Optional[Union[List[int]]]
+        cls, tile_overlap: Optional[Union[List[int]]]
     ) -> Optional[Union[List[int]]]:
         """
-        Validate patch size.
+        Validate tile overlap.
 
-        Patch size must be non-zero, positive and even.
+        Overlaps must be non-zero, positive and even.
 
         Parameters
         ----------
-        patch_list : Optional[Union[List[int]]]
+        tile_overlap : Optional[Union[List[int]]]
             Patch size.
 
         Returns
         -------
         Optional[Union[List[int]]]
-            Validated patch size.
+            Validated tile overlap.
 
         Raises
         ------
         ValueError
             If the patch size is 0.
         ValueError
             If the patch size is not even.
         """
-        if patch_list is not None:
-            for dim in patch_list:
+        if tile_overlap is not None:
+            for dim in tile_overlap:
                 if dim < 1:
                     raise ValueError(
                         f"Patch size must be non-zero positive (got {dim})."
                     )
 
                 if dim % 2 != 0:
                     raise ValueError(f"Patch size must be even (got {dim}).")
 
-        return patch_list
+        return tile_overlap
 
     @field_validator("tile_size")
     @classmethod
     def tile_min_8_power_of_2(
         cls, tile_list: Optional[Union[List[int]]]
     ) -> Optional[Union[List[int]]]:
         """
@@ -148,35 +148,35 @@
         check_axes_validity(axes)
 
         return axes
 
     @field_validator("transforms")
     @classmethod
     def validate_transforms(
-        cls, transforms: Union[List[TRANSFORMS_UNION], Compose]
-    ) -> Union[List[TRANSFORMS_UNION], Compose]:
+        cls, transforms: List[TRANSFORMS_UNION]
+    ) -> List[TRANSFORMS_UNION]:
         """
         Validate that transforms do not have N2V pixel manipulate transforms.
 
         Parameters
         ----------
-        transforms : Union[List[TransformModel], Compose]
+        transforms : List[TRANSFORMS_UNION]
             Transforms.
 
         Returns
         -------
-        Union[List[Transformations_Union], Compose]
+        List[TRANSFORMS_UNION]
             Validated transforms.
 
         Raises
         ------
         ValueError
             If transforms contain N2V pixel manipulate transforms.
         """
-        if not isinstance(transforms, Compose) and transforms is not None:
+        if transforms is not None:
             for transform in transforms:
                 if transform.name == SupportedTransform.N2V_MANIPULATE.value:
                     raise ValueError(
                         "N2V_Manipulate transform is not allowed in "
                         "prediction transforms."
                     )
 
@@ -243,19 +243,18 @@
         Returns
         -------
         Self
             Inference model with mean and std added to the Normalize transform.
         """
         if self.mean is not None or self.std is not None:
             # search in the transforms for Normalize and update parameters
-            if not isinstance(self.transforms, Compose):
-                for transform in self.transforms:
-                    if transform.name == SupportedTransform.NORMALIZE.value:
-                        transform.mean = self.mean
-                        transform.std = self.std
+            for transform in self.transforms:
+                if transform.name == SupportedTransform.NORMALIZE.value:
+                    transform.mean = self.mean
+                    transform.std = self.std
 
         return self
 
     def _update(self, **kwargs: Any) -> None:
         """
         Update multiple arguments at once.
```

### Comparing `careamics-0.1.0rc4/src/careamics/config/noise_models.py` & `careamics-0.1.0rc5/src/careamics/config/noise_models.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/src/careamics/config/optimizer_models.py` & `careamics-0.1.0rc5/src/careamics/config/optimizer_models.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/src/careamics/config/tile_information.py` & `careamics-0.1.0rc5/src/careamics/config/tile_information.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/src/careamics/config/training_model.py` & `careamics-0.1.0rc5/src/careamics/config/training_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Training configuration."""
+
 from __future__ import annotations
 
 from pprint import pformat
 from typing import Literal, Optional
 
 from pydantic import (
     BaseModel,
```

### Comparing `careamics-0.1.0rc4/src/careamics/config/architectures/architecture_model.py` & `careamics-0.1.0rc5/src/careamics/config/architectures/architecture_model.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/src/careamics/config/architectures/custom_model.py` & `careamics-0.1.0rc5/src/careamics/config/architectures/custom_model.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/src/careamics/config/architectures/register_model.py` & `careamics-0.1.0rc5/src/careamics/config/architectures/register_model.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/src/careamics/config/architectures/unet_model.py` & `careamics-0.1.0rc5/src/careamics/config/architectures/unet_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     in_channels: int = Field(default=1, ge=1, validate_default=True)
     depth: int = Field(default=2, ge=1, le=10, validate_default=True)
     num_channels_init: int = Field(default=32, ge=8, le=1024, validate_default=True)
     final_activation: Literal[
         "None", "Sigmoid", "Softmax", "Tanh", "ReLU", "LeakyReLU"
     ] = Field(default="None", validate_default=True)
     n2v2: bool = Field(default=False, validate_default=True)
+    independent_channels: bool = Field(default=True, validate_default=True)
 
     @field_validator("num_channels_init")
     @classmethod
     def validate_num_channels_init(cls, num_channels_init: int) -> int:
         """
         Validate that num_channels_init is even.
```

### Comparing `careamics-0.1.0rc4/src/careamics/config/architectures/vae_model.py` & `careamics-0.1.0rc5/src/careamics/config/architectures/vae_model.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/src/careamics/config/references/__init__.py` & `careamics-0.1.0rc5/src/careamics/config/references/__init__.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/src/careamics/config/references/algorithm_descriptions.py` & `careamics-0.1.0rc5/src/careamics/config/references/algorithm_descriptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Descriptions of the algorithms used in CAREmics."""
+
 from pydantic import BaseModel
 
 CUSTOM = "Custom"
 N2V = "Noise2Void"
 N2V2 = "N2V2"
 STRUCT_N2V = "StructN2V"
 STRUCT_N2V2 = "StructN2V2"
```

### Comparing `careamics-0.1.0rc4/src/careamics/config/references/references.py` & `careamics-0.1.0rc5/src/careamics/config/references/references.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """References for the CAREamics algorithms."""
+
 from bioimageio.spec.generic.v0_3 import CiteEntry
 
 N2VRef = CiteEntry(
     text='Krull, A., Buchholz, T.O. and Jug, F., 2019. "Noise2Void - Learning '
     'denoising from single noisy images". In Proceedings of the IEEE/CVF '
     "conference on computer vision and pattern recognition (pp. 2129-2137).",
     doi="10.1109/cvpr.2019.00223",
```

### Comparing `careamics-0.1.0rc4/src/careamics/config/support/__init__.py` & `careamics-0.1.0rc5/src/careamics/config/support/__init__.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/src/careamics/config/support/supported_data.py` & `careamics-0.1.0rc5/src/careamics/config/support/supported_data.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/src/careamics/config/support/supported_extraction_strategies.py` & `careamics-0.1.0rc5/src/careamics/config/support/supported_extraction_strategies.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Extraction strategy module.
 
 This module defines the various extraction strategies available in CAREamics.
 """
+
 from careamics.utils import BaseEnum
 
 
 class SupportedExtractionStrategy(str, BaseEnum):
     """
     Available extraction strategies.
```

### Comparing `careamics-0.1.0rc4/src/careamics/config/support/supported_optimizers.py` & `careamics-0.1.0rc5/src/careamics/config/support/supported_optimizers.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/src/careamics/config/support/supported_transforms.py` & `careamics-0.1.0rc5/src/careamics/config/support/supported_transforms.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/src/careamics/config/transformations/n2v_manipulate_model.py` & `careamics-0.1.0rc5/src/careamics/config/transformations/n2v_manipulate_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Pydantic model for the N2VManipulate transform."""
+
 from typing import Literal
 
 from pydantic import ConfigDict, Field, field_validator
 
 from .transform_model import TransformModel
```

### Comparing `careamics-0.1.0rc4/src/careamics/config/transformations/normalize_model.py` & `careamics-0.1.0rc5/src/careamics/config/transformations/normalize_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Pydantic model for the Normalize transform."""
+
 from typing import Literal
 
 from pydantic import ConfigDict, Field
 
 from .transform_model import TransformModel
```

### Comparing `careamics-0.1.0rc4/src/careamics/config/transformations/transform_model.py` & `careamics-0.1.0rc5/src/careamics/config/transformations/transform_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Parent model for the transforms."""
+
 from typing import Any, Dict
 
 from pydantic import BaseModel, ConfigDict
 
 
 class TransformModel(BaseModel):
     """
```

### Comparing `careamics-0.1.0rc4/src/careamics/config/transformations/xy_random_rotate90_model.py` & `careamics-0.1.0rc5/src/careamics/config/transformations/xy_random_rotate90_model.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 """Pydantic model for the XYRandomRotate90 transform."""
-from typing import Literal
 
-from pydantic import ConfigDict, Field
+from typing import Literal, Optional
+
+from pydantic import ConfigDict
 
 from .transform_model import TransformModel
 
 
 class XYRandomRotate90Model(TransformModel):
     """
     Pydantic model used to represent NDFlip transformation.
 
     Attributes
     ----------
     name : Literal["XYRandomRotate90"]
         Name of the transformation.
-    p : float
-        Probability of applying the transformation, by default 0.5.
-    is_3D : bool
-        Whether the transformation should be applied in 3D, by default False.
+    seed : Optional[int]
+        Seed for the random number generator.
     """
 
     model_config = ConfigDict(
         validate_assignment=True,
     )
 
     name: Literal["XYRandomRotate90"] = "XYRandomRotate90"
-    p: float = Field(default=0.5, ge=0.0, le=1.0)
-    is_3D: bool = Field(default=False)
+    seed: Optional[int] = None
```

### Comparing `careamics-0.1.0rc4/src/careamics/config/validators/validator_utils.py` & `careamics-0.1.0rc5/src/careamics/config/validators/validator_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Validator functions.
 
 These functions are used to validate dimensions and axes of inputs.
 """
+
 from typing import List, Optional, Tuple, Union
 
 _AXES = "STCZYX"
 
 
 def check_axes_validity(axes: str) -> None:
     """
```

### Comparing `careamics-0.1.0rc4/src/careamics/dataset/in_memory_dataset.py` & `careamics-0.1.0rc5/src/careamics/dataset/in_memory_dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """In-memory dataset module."""
+
 from __future__ import annotations
 
 import copy
 from pathlib import Path
 from typing import Any, Callable, List, Optional, Tuple, Union
 
 import numpy as np
 from torch.utils.data import Dataset
 
+from careamics.transforms import Compose
+
 from ..config import DataConfig, InferenceConfig
 from ..config.tile_information import TileInformation
 from ..utils.logging import get_logger
 from .dataset_utils import read_tiff, reshape_array
-from .patching.patch_transform import get_patch_transform
 from .patching.patching import (
     prepare_patches_supervised,
     prepare_patches_supervised_array,
     prepare_patches_unsupervised,
     prepare_patches_unsupervised_array,
 )
 from .patching.tiled_patching import extract_tiles
@@ -56,26 +58,23 @@
         # Add results to members
         self.data, self.data_targets, computed_mean, computed_std = patches
 
         if not self.data_config.mean or not self.data_config.std:
             self.mean, self.std = computed_mean, computed_std
             logger.info(f"Computed dataset mean: {self.mean}, std: {self.std}")
 
-            # if the transforms are not an instance of Compose
-            if self.data_config.has_transform_list():
-                # update mean and std in configuration
-                # the object is mutable and should then be recorded in the CAREamist obj
-                self.data_config.set_mean_and_std(self.mean, self.std)
+            # update mean and std in configuration
+            # the object is mutable and should then be recorded in the CAREamist obj
+            self.data_config.set_mean_and_std(self.mean, self.std)
         else:
             self.mean, self.std = self.data_config.mean, self.data_config.std
 
         # get transforms
-        self.patch_transform = get_patch_transform(
-            patch_transforms=self.data_config.transforms,
-            with_target=self.data_target is not None,
+        self.patch_transform = Compose(
+            transform_list=self.data_config.transforms,
         )
 
     def _prepare_patches(
         self, supervised: bool
     ) -> Tuple[np.ndarray, Optional[np.ndarray], float, float]:
         """
         Iterate over data source and create an array of patches.
@@ -162,41 +161,18 @@
         patch = self.data[index]
 
         # if there is a target
         if self.data_target is not None:
             # get target
             target = self.data_targets[index]
 
-            # Albumentations requires Channel last
-            c_patch = np.moveaxis(patch, 0, -1)
-            c_target = np.moveaxis(target, 0, -1)
-
-            # Apply transforms
-            transformed = self.patch_transform(image=c_patch, target=c_target)
-
-            # move axes back
-            patch = np.moveaxis(transformed["image"], -1, 0)
-            target = np.moveaxis(transformed["target"], -1, 0)
-
-            return patch, target
+            return self.patch_transform(patch=patch, target=target)
 
         elif self.data_config.has_n2v_manipulate():
-            # Albumentations requires Channel last
-            patch = np.moveaxis(patch, 0, -1)
-
-            # Apply transforms
-            transformed_patch = self.patch_transform(image=patch)["image"]
-            manip_patch, patch, mask = transformed_patch
-
-            # move C axes back
-            manip_patch = np.moveaxis(manip_patch, -1, 0)
-            patch = np.moveaxis(patch, -1, 0)
-            mask = np.moveaxis(mask, -1, 0)
-
-            return (manip_patch, patch, mask)
+            return self.patch_transform(patch=patch)
         else:
             raise ValueError(
                 "Something went wrong! No target provided (not supervised training) "
                 "and no N2V manipulation (no N2V training)."
             )
 
     def split_dataset(
@@ -314,17 +290,16 @@
         self.read_source_func = read_source_func
 
         # Generate patches
         self.data = self._prepare_tiles()
         self.mean, self.std = self.pred_config.mean, self.pred_config.std
 
         # get transforms
-        self.patch_transform = get_patch_transform(
-            patch_transforms=self.pred_config.transforms,
-            with_target=self.data_target is not None,
+        self.patch_transform = Compose(
+            transform_list=self.pred_config.transforms,
         )
 
     def _prepare_tiles(self) -> List[Tuple[np.ndarray, TileInformation]]:
         """
         Iterate over data source and create an array of patches.
 
         Returns
@@ -375,17 +350,11 @@
         Returns
         -------
         Tuple[np.ndarray, TileInformation]
             Transformed patch.
         """
         tile_array, tile_info = self.data[index]
 
-        # Albumentations requires channel last, use the XArrayTile array
-        patch = np.moveaxis(tile_array, 0, -1)
-
         # Apply transforms
-        transformed_patch = self.patch_transform(image=patch)["image"]
-
-        # move C axes back
-        transformed_patch = np.moveaxis(transformed_patch, -1, 0)
+        transformed_tile, _ = self.patch_transform(patch=tile_array)
 
-        return transformed_patch, tile_info
+        return transformed_tile, tile_info
```

### Comparing `careamics-0.1.0rc4/src/careamics/dataset/iterable_dataset.py` & `careamics-0.1.0rc5/src/careamics/dataset/iterable_dataset.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,21 +3,20 @@
 import copy
 from pathlib import Path
 from typing import Any, Callable, Generator, List, Optional, Tuple, Union
 
 import numpy as np
 from torch.utils.data import IterableDataset, get_worker_info
 
+from careamics.transforms import Compose
+
 from ..config import DataConfig, InferenceConfig
 from ..config.tile_information import TileInformation
 from ..utils.logging import get_logger
 from .dataset_utils import read_tiff, reshape_array
-from .patching import (
-    get_patch_transform,
-)
 from .patching.random_patching import extract_patches_random
 from .patching.tiled_patching import extract_tiles
 
 logger = get_logger(__name__)
 
 
 class PathIterableDataset(IterableDataset):
@@ -57,34 +56,23 @@
         self.data_config = data_config
         self.read_source_func = read_source_func
 
         # compute mean and std over the dataset
         if not data_config.mean or not data_config.std:
             self.mean, self.std = self._calculate_mean_and_std()
 
-            # if the transforms are not an instance of Compose
-            # Check if the data_config is an instance of DataModel or InferenceModel
-            # isinstance isn't working properly here
-            if hasattr(data_config, "has_transform_list"):
-                if data_config.has_transform_list():
-                    # update mean and std in configuration
-                    # the object is mutable and should then be recorded in the CAREamist
-                    data_config.set_mean_and_std(self.mean, self.std)
-            else:
-                data_config.set_mean_and_std(self.mean, self.std)
-
+            # update mean and std in configuration
+            # the object is mutable and should then be recorded in the CAREamist
+            data_config.set_mean_and_std(self.mean, self.std)
         else:
             self.mean = data_config.mean
             self.std = data_config.std
 
         # get transforms
-        self.patch_transform = get_patch_transform(
-            patch_transforms=data_config.transforms,
-            with_target=target_files is not None,
-        )
+        self.patch_transform = Compose(transform_list=data_config.transforms)
 
     def _calculate_mean_and_std(self) -> Tuple[float, float]:
         """
         Calculate mean and std of the dataset.
 
         Returns
         -------
@@ -188,57 +176,18 @@
             )
 
             # iterate over patches
             # patches are tuples of (patch, target) if target is available
             # or (patch, None) only if no target is available
             # patch is of dimensions (C)ZYX
             for patch_data in patches:
-                # if there is a target
-                if self.target_files is not None:
-                    # Albumentations expects the channel dimension to be last
-                    # Taking the first element because patch_data can include target
-                    c_patch = np.moveaxis(patch_data[0], 0, -1)
-                    c_target = np.moveaxis(patch_data[1], 0, -1)
-
-                    # apply the transform to the patch and the target
-                    transformed = self.patch_transform(
-                        image=c_patch,
-                        target=c_target,
-                    )
-
-                    # move the axes back to the original position
-                    c_patch = np.moveaxis(transformed["image"], -1, 0)
-                    c_target = np.moveaxis(transformed["target"], -1, 0)
-
-                    yield (c_patch, c_target)
-                elif self.data_config.has_n2v_manipulate():
-                    # Albumentations expects the channel dimension to be last
-                    # Taking the first element because patch_data can include target
-                    patch = np.moveaxis(patch_data[0], 0, -1)
-
-                    # apply transform
-                    transformed = self.patch_transform(image=patch)
-
-                    # retrieve the output of ManipulateN2V
-                    results = transformed["image"]
-                    masked_patch: np.ndarray = results[0]
-                    original_patch: np.ndarray = results[1]
-                    mask: np.ndarray = results[2]
-
-                    # move C axes back
-                    masked_patch = np.moveaxis(masked_patch, -1, 0)
-                    original_patch = np.moveaxis(original_patch, -1, 0)
-                    mask = np.moveaxis(mask, -1, 0)
-
-                    yield (masked_patch, original_patch, mask)
-                else:
-                    raise ValueError(
-                        "Something went wrong! Not target file (no supervised "
-                        "training) and no N2V transform (no n2v training either)."
-                    )
+                yield self.patch_transform(
+                    patch=patch_data[0],
+                    target=patch_data[1],
+                )
 
     def get_number_of_files(self) -> int:
         """
         Return the number of files in the dataset.
 
         Returns
         -------
@@ -363,17 +312,16 @@
         self.tile_overlap = self.prediction_config.tile_overlap
         self.read_source_func = read_source_func
 
         # tile only if both tile size and overlaps are provided
         self.tile = self.tile_size is not None and self.tile_overlap is not None
 
         # get tta transforms
-        self.patch_transform = get_patch_transform(
-            patch_transforms=prediction_config.transforms,
-            with_target=False,
+        self.patch_transform = Compose(
+            transform_list=prediction_config.transforms,
         )
 
     def __iter__(
         self,
     ) -> Generator[Tuple[np.ndarray, TileInformation], None, None]:
         """
         Iterate over data source and yield single patch.
@@ -404,13 +352,10 @@
                 patch_gen = (
                     (reshaped_sample, TileInformation(array_shape=array_shape))
                     for _ in range(1)
                 )
 
             # apply transform to patches
             for patch_array, tile_info in patch_gen:
-                # albumentations expects the channel dimension to be last
-                patch = np.moveaxis(patch_array, 0, -1)
-                transformed_patch = self.patch_transform(image=patch)
-                transformed_patch = np.moveaxis(transformed_patch["image"], -1, 0)
+                transformed_patch, _ = self.patch_transform(patch=patch_array)
 
                 yield transformed_patch, tile_info
```

### Comparing `careamics-0.1.0rc4/src/careamics/dataset/zarr_dataset.py` & `careamics-0.1.0rc5/src/careamics/dataset/zarr_dataset.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/src/careamics/dataset/dataset_utils/dataset_utils.py` & `careamics-0.1.0rc5/src/careamics/dataset/dataset_utils/dataset_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Convenience methods for datasets."""
+
 from typing import List, Tuple
 
 import numpy as np
 
 from careamics.utils.logging import get_logger
 
 logger = get_logger(__name__)
```

### Comparing `careamics-0.1.0rc4/src/careamics/dataset/dataset_utils/file_utils.py` & `careamics-0.1.0rc5/src/careamics/dataset/dataset_utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/src/careamics/dataset/dataset_utils/read_tiff.py` & `careamics-0.1.0rc5/src/careamics/dataset/dataset_utils/read_tiff.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/src/careamics/dataset/dataset_utils/read_utils.py` & `careamics-0.1.0rc5/src/careamics/dataset/dataset_utils/read_utils.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/src/careamics/dataset/dataset_utils/read_zarr.py` & `careamics-0.1.0rc5/src/careamics/dataset/dataset_utils/read_zarr.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/src/careamics/dataset/patching/patching.py` & `careamics-0.1.0rc5/src/careamics/dataset/patching/patching.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Tiling submodule.
 
 These functions are used to tile images into patches or tiles.
 """
+
 from pathlib import Path
 from typing import Callable, List, Tuple, Union
 
 import numpy as np
 
 from ...utils.logging import get_logger
 from ..dataset_utils import reshape_array
```

### Comparing `careamics-0.1.0rc4/src/careamics/dataset/patching/random_patching.py` & `careamics-0.1.0rc5/src/careamics/dataset/patching/random_patching.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/src/careamics/dataset/patching/sequential_patching.py` & `careamics-0.1.0rc5/src/careamics/dataset/patching/sequential_patching.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,23 +131,20 @@
     """
     rng = np.random.default_rng()
 
     if target is not None:
         arr = np.stack([arr, target], axis=0)
         window_shape = [arr.shape[0], *window_shape]
         step = (arr.shape[0], *step)
-        output_shape = [arr.shape[0], -1, arr.shape[2], *output_shape[2:]]
+        output_shape = [-1, arr.shape[0], arr.shape[2], *output_shape[2:]]
 
     patches = view_as_windows(arr, window_shape=window_shape, step=step).reshape(
         *output_shape
     )
-    if target is not None:
-        rng.shuffle(patches, axis=1)
-    else:
-        rng.shuffle(patches, axis=0)
+    rng.shuffle(patches, axis=0)
     return patches
 
 
 def extract_patches_sequential(
     arr: np.ndarray,
     patch_size: Union[List[int], Tuple[int, ...]],
     target: Optional[np.ndarray] = None,
@@ -197,10 +194,13 @@
         step=window_steps,
         output_shape=output_shape,
         target=target,
     )
 
     if target is not None:
         # target was concatenated to patches in _compute_reshaped_view
-        return (patches[0, ...], patches[1, ...])  # TODO  in _compute_reshaped_view?
+        return (
+            patches[:, 0, ...],
+            patches[:, 1, ...],
+        )  # TODO  in _compute_reshaped_view?
     else:
         return patches, None
```

### Comparing `careamics-0.1.0rc4/src/careamics/dataset/patching/tiled_patching.py` & `careamics-0.1.0rc5/src/careamics/dataset/patching/tiled_patching.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,27 +39,31 @@
             # Add the coordinates to crop one tile
             crop_coords.append((i, i + tile_size))
 
             # Add the pixel coordinates of the cropped tile in the original image space
             stitch_coords.append(
                 (
                     i + overlap // 2 if i > 0 else 0,
-                    i + tile_size - overlap // 2
-                    if crop_coords[-1][1] < axis_size
-                    else axis_size,
+                    (
+                        i + tile_size - overlap // 2
+                        if crop_coords[-1][1] < axis_size
+                        else axis_size
+                    ),
                 )
             )
 
             # Add the coordinates to crop the overlap from the prediction.
             overlap_crop_coords.append(
                 (
                     overlap // 2 if i > 0 else 0,
-                    tile_size - overlap // 2
-                    if crop_coords[-1][1] < axis_size
-                    else tile_size,
+                    (
+                        tile_size - overlap // 2
+                        if crop_coords[-1][1] < axis_size
+                        else tile_size
+                    ),
                 )
             )
 
         # If the tile does not fit within the axis, perform the abovementioned
         # operations starting from the end of the axis
         else:
             # if (axis_size - tile_size, axis_size) not in crop_coords:
```

### Comparing `careamics-0.1.0rc4/src/careamics/dataset/patching/validate_patch_dimension.py` & `careamics-0.1.0rc5/src/careamics/dataset/patching/validate_patch_dimension.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/src/careamics/losses/loss_factory.py` & `careamics-0.1.0rc5/src/careamics/losses/loss_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Loss factory module.
 
 This module contains a factory function for creating loss functions.
 """
+
 from typing import Callable, Union
 
 from ..config.support import SupportedLoss
 from .losses import mae_loss, mse_loss, n2v_loss
 
 
 # TODO add tests
```

### Comparing `careamics-0.1.0rc4/src/careamics/losses/losses.py` & `careamics-0.1.0rc5/src/careamics/losses/losses.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/src/careamics/losses/noise_model_factory.py` & `careamics-0.1.0rc5/src/careamics/losses/noise_model_factory.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/src/careamics/losses/noise_models.py` & `careamics-0.1.0rc5/src/careamics/losses/noise_models.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/src/careamics/model_io/bmz_io.py` & `careamics-0.1.0rc5/src/careamics/model_io/bmz_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Function to export to the BioImage Model Zoo format."""
+
 import tempfile
 from pathlib import Path
 from typing import List, Optional, Tuple, Union
 
 import numpy as np
 import pkg_resources
 from bioimageio.core import load_description, test_model
@@ -173,15 +174,15 @@
             config_path=config_path,
             env_path=env_path,
             channel_names=channel_names,
             data_description=data_description,
         )
 
         # test model description
-        summary: ValidationSummary = test_model(model_description)
+        summary: ValidationSummary = test_model(model_description, decimal=0)
         if summary.status == "failed":
             raise ValueError(f"Model description test failed: {summary}")
 
         # save bmz model
         save_bioimageio_package(model_description, output_path=path)
```

### Comparing `careamics-0.1.0rc4/src/careamics/model_io/model_io_utils.py` & `careamics-0.1.0rc5/src/careamics/model_io/model_io_utils.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/src/careamics/model_io/bioimage/_readme_factory.py` & `careamics-0.1.0rc5/src/careamics/model_io/bioimage/_readme_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Functions used to create a README.md file for BMZ export."""
+
 from pathlib import Path
 from typing import Optional
 
 import yaml
 
 from careamics.config import Configuration
 from careamics.utils import cwd, get_careamics_home
@@ -113,8 +114,8 @@
             "## Links\n\n"
             "- [CAREamics repository](https://github.com/CAREamics/careamics)\n"
             "- [CAREamics documentation](https://careamics.github.io/latest/)\n"
         )
 
         readme.write_text("".join(description))
 
-    return readme
+        return readme.absolute()
```

### Comparing `careamics-0.1.0rc4/src/careamics/model_io/bioimage/bioimage_utils.py` & `careamics-0.1.0rc5/src/careamics/model_io/bioimage/bioimage_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Bioimage.io utils."""
+
 from pathlib import Path
 from typing import Union
 
 
 def get_unzip_path(zip_path: Union[Path, str]) -> Path:
     """Generate unzipped folder path from the bioimage.io model path.
```

### Comparing `careamics-0.1.0rc4/src/careamics/model_io/bioimage/model_description.py` & `careamics-0.1.0rc5/src/careamics/model_io/bioimage/model_description.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module use to build BMZ model description."""
+
 from pathlib import Path
 from typing import List, Optional, Tuple, Union
 
 import numpy as np
 from bioimageio.spec.model.v0_5 import (
     ArchitectureFromLibraryDescr,
     Author,
```

### Comparing `careamics-0.1.0rc4/src/careamics/models/activation.py` & `careamics-0.1.0rc5/src/careamics/models/activation.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/src/careamics/models/layers.py` & `careamics-0.1.0rc5/src/careamics/models/layers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Layer module.
 
 This submodule contains layers used in the CAREamics models.
 """
+
 from typing import List, Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
 from torch.nn import functional as F
```

### Comparing `careamics-0.1.0rc4/src/careamics/models/model_factory.py` & `careamics-0.1.0rc5/src/careamics/models/model_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Model factory.
 
 Model creation factory functions.
 """
+
 from typing import Union
 
 import torch
 
 from ..config.architectures import CustomModel, UNetModel, VAEModel, get_custom_model
 from ..config.support import SupportedArchitecture
 from ..utils import get_logger
```

### Comparing `careamics-0.1.0rc4/src/careamics/models/unet.py` & `careamics-0.1.0rc5/src/careamics/models/unet.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 UNet model.
 
 A UNet encoder, decoder and complete model.
 """
-from typing import Any, List, Union
+
+from typing import Any, List, Tuple, Union
 
 import torch
 import torch.nn as nn
 
 from ..config.support import SupportedActivation
 from .activation import get_activation
 from .layers import Conv_Block, MaxBlurPool
@@ -29,26 +30,30 @@
         Number of channels in the first encoder block, by default 64.
     use_batch_norm : bool, optional
         Whether to use batch normalization, by default True.
     dropout : float, optional
         Dropout probability, by default 0.0.
     pool_kernel : int, optional
         Kernel size for the max pooling layers, by default 2.
+    groups: int, optional
+        Number of blocked connections from input channels to output
+        channels, by default 1.
     """
 
     def __init__(
         self,
         conv_dim: int,
         in_channels: int = 1,
         depth: int = 3,
         num_channels_init: int = 64,
         use_batch_norm: bool = True,
         dropout: float = 0.0,
         pool_kernel: int = 2,
         n2v2: bool = False,
+        groups: int = 1,
     ) -> None:
         """
         Constructor.
 
         Parameters
         ----------
         conv_dim : int
@@ -61,35 +66,39 @@
             Number of channels in the first encoder block, by default 64.
         use_batch_norm : bool, optional
             Whether to use batch normalization, by default True.
         dropout : float, optional
             Dropout probability, by default 0.0.
         pool_kernel : int, optional
             Kernel size for the max pooling layers, by default 2.
+        groups: int, optional
+            Number of blocked connections from input channels to output
+            channels, by default 1.
         """
         super().__init__()
 
         self.pooling = (
             getattr(nn, f"MaxPool{conv_dim}d")(kernel_size=pool_kernel)
             if not n2v2
             else MaxBlurPool(dim=conv_dim, kernel_size=3, max_pool_size=pool_kernel)
         )
 
         encoder_blocks = []
 
         for n in range(depth):
-            out_channels = num_channels_init * (2**n)
+            out_channels = num_channels_init * (2**n) * groups
             in_channels = in_channels if n == 0 else out_channels // 2
             encoder_blocks.append(
                 Conv_Block(
                     conv_dim,
                     in_channels=in_channels,
                     out_channels=out_channels,
                     dropout_perc=dropout,
                     use_batch_norm=use_batch_norm,
+                    groups=groups,
                 )
             )
             encoder_blocks.append(self.pooling)
         self.encoder_blocks = nn.ModuleList(encoder_blocks)
 
     def forward(self, x: torch.Tensor) -> List[torch.Tensor]:
         """
@@ -127,24 +136,28 @@
         Number of decoder blocks, by default 3.
     num_channels_init : int, optional
         Number of channels in the first encoder block, by default 64.
     use_batch_norm : bool, optional
         Whether to use batch normalization, by default True.
     dropout : float, optional
         Dropout probability, by default 0.0.
+    groups: int, optional
+        Number of blocked connections from input channels to output
+        channels, by default 1.
     """
 
     def __init__(
         self,
         conv_dim: int,
         depth: int = 3,
         num_channels_init: int = 64,
         use_batch_norm: bool = True,
         dropout: float = 0.0,
         n2v2: bool = False,
+        groups: int = 1,
     ) -> None:
         """
         Constructor.
 
         Parameters
         ----------
         conv_dim : int
@@ -153,59 +166,61 @@
             Number of decoder blocks, by default 3.
         num_channels_init : int, optional
             Number of channels in the first encoder block, by default 64.
         use_batch_norm : bool, optional
             Whether to use batch normalization, by default True.
         dropout : float, optional
             Dropout probability, by default 0.0.
+        groups: int, optional
+            Number of blocked connections from input channels to output
+            channels, by default 1.
         """
         super().__init__()
 
         upsampling = nn.Upsample(
             scale_factor=2, mode="bilinear" if conv_dim == 2 else "trilinear"
         )
-        in_channels = out_channels = num_channels_init * 2 ** (depth - 1)
+        in_channels = out_channels = num_channels_init * groups * (2 ** (depth - 1))
 
         self.n2v2 = n2v2
+        self.groups = groups
 
         self.bottleneck = Conv_Block(
             conv_dim,
             in_channels=in_channels,
             out_channels=out_channels,
             intermediate_channel_multiplier=2,
             use_batch_norm=use_batch_norm,
             dropout_perc=dropout,
+            groups=self.groups,
         )
 
-        decoder_blocks = []
+        decoder_blocks: List[nn.Module] = []
         for n in range(depth):
             decoder_blocks.append(upsampling)
-            in_channels = (
-                num_channels_init ** (depth - n)
-                if (self.n2v2 and n == depth - 1)
-                else num_channels_init * 2 ** (depth - n)
-            )
+            in_channels = (num_channels_init * 2 ** (depth - n)) * groups
             out_channels = in_channels // 2
             decoder_blocks.append(
                 Conv_Block(
                     conv_dim,
-                    in_channels=in_channels + in_channels // 2
-                    if n > 0
-                    else in_channels,
+                    in_channels=(
+                        in_channels + in_channels // 2 if n > 0 else in_channels
+                    ),
                     out_channels=out_channels,
                     intermediate_channel_multiplier=2,
                     dropout_perc=dropout,
                     activation="ReLU",
                     use_batch_norm=use_batch_norm,
+                    groups=groups,
                 )
             )
 
         self.decoder_blocks = nn.ModuleList(decoder_blocks)
 
-    def forward(self, *features: List[torch.Tensor]) -> torch.Tensor:
+    def forward(self, *features: torch.Tensor) -> torch.Tensor:
         """
         Forward pass.
 
         Parameters
         ----------
         *features :  List[torch.Tensor]
             List containing the output of each encoder block(skip connections) and final
@@ -213,28 +228,78 @@
 
         Returns
         -------
         torch.Tensor
             Output of the decoder.
         """
         x: torch.Tensor = features[0]
-        skip_connections: torch.Tensor = features[1:][::-1]
+        skip_connections: Tuple[torch.Tensor, ...] = features[-1:0:-1]
 
         x = self.bottleneck(x)
 
         for i, module in enumerate(self.decoder_blocks):
             x = module(x)
             if isinstance(module, nn.Upsample):
+                # divide index by 2 because of upsampling layers
+                skip_connection: torch.Tensor = skip_connections[i // 2]
                 if self.n2v2:
                     if x.shape != skip_connections[-1].shape:
-                        x = torch.cat([x, skip_connections[i // 2]], axis=1)
+                        x = self._interleave(x, skip_connection, self.groups)
                 else:
-                    x = torch.cat([x, skip_connections[i // 2]], axis=1)
+                    x = self._interleave(x, skip_connection, self.groups)
         return x
 
+    @staticmethod
+    def _interleave(A: torch.Tensor, B: torch.Tensor, groups: int) -> torch.Tensor:
+        """
+        Splits the tensors `A` and `B` into equally sized groups along the
+        channel axis (axis=1); then concatenates the groups in alternating
+        order along the channel axis, starting with the first group from tensor
+        A.
+
+        Parameters
+        ----------
+        A: torch.Tensor
+        B: torch.Tensor
+        groups: int
+            The number of groups.
+
+        Returns
+        -------
+        torch.Tensor
+
+        Raises
+        ------
+        ValueError:
+            If either of `A` or `B`'s channel axis is not divisible by `groups`.
+        """
+        if (A.shape[1] % groups != 0) or (B.shape[1] % groups != 0):
+            raise ValueError(f"Number of channels not divisible by {groups} groups.")
+
+        m = A.shape[1] // groups
+        n = B.shape[1] // groups
+
+        A_groups: List[torch.Tensor] = [
+            A[:, i * m : (i + 1) * m] for i in range(groups)
+        ]
+        B_groups: List[torch.Tensor] = [
+            B[:, i * n : (i + 1) * n] for i in range(groups)
+        ]
+
+        interleaved = torch.cat(
+            [
+                tensor_list[i]
+                for i in range(groups)
+                for tensor_list in [A_groups, B_groups]
+            ],
+            dim=1,
+        )
+
+        return interleaved
+
 
 class UNet(nn.Module):
     """
     UNet model.
 
     Adapted for PyTorch from:
     https://github.com/juglab/n2v/blob/main/n2v/nets/unet_blocks.py.
@@ -269,14 +334,15 @@
         depth: int = 3,
         num_channels_init: int = 64,
         use_batch_norm: bool = True,
         dropout: float = 0.0,
         pool_kernel: int = 2,
         final_activation: Union[SupportedActivation, str] = SupportedActivation.NONE,
         n2v2: bool = False,
+        independent_channels: bool = True,
         **kwargs: Any,
     ) -> None:
         """
         Constructor.
 
         Parameters
         ----------
@@ -294,40 +360,48 @@
             Whether to use batch normalization, by default True.
         dropout : float, optional
             Dropout probability, by default 0.0.
         pool_kernel : int, optional
             Kernel size of the pooling layers, by default 2.
         last_activation : Optional[Callable], optional
             Activation function to use for the last layer, by default None.
+        independent_channels : bool
+            Whether to train parallel independent networks for each channel, by
+            default True.
         """
         super().__init__()
 
+        groups = in_channels if independent_channels else 1
+
         self.encoder = UnetEncoder(
             conv_dims,
             in_channels=in_channels,
             depth=depth,
             num_channels_init=num_channels_init,
             use_batch_norm=use_batch_norm,
             dropout=dropout,
             pool_kernel=pool_kernel,
             n2v2=n2v2,
+            groups=groups,
         )
 
         self.decoder = UnetDecoder(
             conv_dims,
             depth=depth,
             num_channels_init=num_channels_init,
             use_batch_norm=use_batch_norm,
             dropout=dropout,
             n2v2=n2v2,
+            groups=groups,
         )
         self.final_conv = getattr(nn, f"Conv{conv_dims}d")(
-            in_channels=num_channels_init,
+            in_channels=num_channels_init * groups,
             out_channels=num_classes,
             kernel_size=1,
+            groups=groups,
         )
         self.final_activation = get_activation(final_activation)
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         """
         Forward pass.
```

### Comparing `careamics-0.1.0rc4/src/careamics/prediction/stitch_prediction.py` & `careamics-0.1.0rc5/src/careamics/prediction/stitch_prediction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Prediction convenience functions.
 
 These functions are used during prediction.
 """
+
 from typing import List
 
 import numpy as np
 import torch
 
 
 def stitch_prediction(
```

### Comparing `careamics-0.1.0rc4/src/careamics/transforms/n2v_manipulate.py` & `careamics-0.1.0rc5/src/careamics/transforms/n2v_manipulate.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import Any, Literal, Optional, Tuple
 
 import numpy as np
-from albumentations import ImageOnlyTransform
 
 from careamics.config.support import SupportedPixelManipulation, SupportedStructAxis
+from careamics.transforms.transform import Transform
 
 from .pixel_manipulation import median_manipulate, uniform_manipulate
 from .struct_mask_parameters import StructMaskParameters
 
 
-class N2VManipulate(ImageOnlyTransform):
+class N2VManipulate(Transform):
     """
     Default augmentation for the N2V model.
 
-    This transform expects (Z)YXC dimensions.
+    This transform expects C(Z)YX dimensions.
 
     Parameters
     ----------
     mask_pixel_percentage : float
         Approximate percentage of pixels to be masked.
     roi_size : int
         Size of the ROI the new pixel value is sampled from, by default 11.
@@ -29,14 +29,15 @@
         masked_pixel_percentage: float = 0.2,
         strategy: Literal[
             "uniform", "median"
         ] = SupportedPixelManipulation.UNIFORM.value,
         remove_center: bool = True,
         struct_mask_axis: Literal["horizontal", "vertical", "none"] = "none",
         struct_mask_span: int = 5,
+        seed: Optional[int] = None,  # TODO use in pixel manipulation
     ):
         """Constructor.
 
         Parameters
         ----------
         roi_size : int, optional
             Size of the replacement area, by default 11
@@ -46,68 +47,62 @@
             Replaccement strategy, uniform or median, by default uniform
         remove_center : bool, optional
             Whether to remove central pixel from patch, by default True
         struct_mask_axis : Literal["horizontal", "vertical", "none"], optional
             StructN2V mask axis, by default "none"
         struct_mask_span : int, optional
             StructN2V mask span, by default 5
+        seed : Optional[int], optional
+            Random seed, by default None
         """
-        super().__init__(p=1)
         self.masked_pixel_percentage = masked_pixel_percentage
         self.roi_size = roi_size
         self.strategy = strategy
         self.remove_center = remove_center
 
         if struct_mask_axis == SupportedStructAxis.NONE:
             self.struct_mask: Optional[StructMaskParameters] = None
         else:
             self.struct_mask = StructMaskParameters(
                 axis=0 if struct_mask_axis == SupportedStructAxis.HORIZONTAL else 1,
                 span=struct_mask_span,
             )
 
-    def apply(
-        self, patch: np.ndarray, **kwargs: Any
+        # numpy random generator
+        self.rng = np.random.default_rng(seed=seed)
+
+    def __call__(
+        self, patch: np.ndarray, *args: Any, **kwargs: Any
     ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
         """Apply the transform to the image.
 
         Parameters
         ----------
         image : np.ndarray
-            Image or image patch, 2D or 3D, shape (y, x, c) or (z, y, x, c).
+            Image or image patch, 2D or 3D, shape C(Z)YX.
         """
         masked = np.zeros_like(patch)
         mask = np.zeros_like(patch)
         if self.strategy == SupportedPixelManipulation.UNIFORM:
             # Iterate over the channels to apply manipulation separately
-            for c in range(patch.shape[-1]):
-                masked[..., c], mask[..., c] = uniform_manipulate(
-                    patch=patch[..., c],
+            for c in range(patch.shape[0]):
+                masked[c, ...], mask[c, ...] = uniform_manipulate(
+                    patch=patch[c, ...],
                     mask_pixel_percentage=self.masked_pixel_percentage,
                     subpatch_size=self.roi_size,
                     remove_center=self.remove_center,
                     struct_params=self.struct_mask,
                 )
         elif self.strategy == SupportedPixelManipulation.MEDIAN:
             # Iterate over the channels to apply manipulation separately
-            for c in range(patch.shape[-1]):
-                masked[..., c], mask[..., c] = median_manipulate(
-                    patch=patch[..., c],
+            for c in range(patch.shape[0]):
+                masked[c, ...], mask[c, ...] = median_manipulate(
+                    patch=patch[c, ...],
                     mask_pixel_percentage=self.masked_pixel_percentage,
                     subpatch_size=self.roi_size,
                     struct_params=self.struct_mask,
                 )
         else:
             raise ValueError(f"Unknown masking strategy ({self.strategy}).")
 
         # TODO why return patch?
         return masked, patch, mask
-
-    def get_transform_init_args_names(self) -> Tuple[str, ...]:
-        """Get the transform parameters.
-
-        Returns
-        -------
-        Tuple[str, ...]
-            Transform parameters.
-        """
-        return ("roi_size", "masked_pixel_percentage", "strategy", "struct_mask")
```

### Comparing `careamics-0.1.0rc4/src/careamics/transforms/pixel_manipulation.py` & `careamics-0.1.0rc5/src/careamics/transforms/pixel_manipulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Pixel manipulation methods.
 
 Pixel manipulation is used in N2V and similar algorithm to replace the value of
 masked pixels.
 """
+
 from typing import Optional, Tuple, Union
 
 import numpy as np
 
 from .struct_mask_parameters import StructMaskParameters
 
 
@@ -242,16 +243,15 @@
     patch : np.ndarray
         Image patch, 2D or 3D, shape (y, x) or (z, y, x).
     mask_pixel_percentage : float
         Approximate percentage of pixels to be masked.
     subpatch_size : int
         Size of the subpatch the new pixel value is sampled from, by default 11.
     remove_center : bool
-        Whether to remove the center pixel from the subpatch, by default False. See
-        uniform with/without central pixel in the documentation. #TODO add link
+        Whether to remove the center pixel from the subpatch, by default False.
     struct_params: Optional[StructMaskParameters]
         Parameters for the structN2V mask (axis and span).
 
     Returns
     -------
     Tuple[np.ndarray]
         Tuple containing the manipulated patch and the corresponding mask.
```

### Comparing `careamics-0.1.0rc4/src/careamics/transforms/tta.py` & `careamics-0.1.0rc5/src/careamics/transforms/tta.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Test-time augmentations."""
+
 from typing import List
 
-import numpy as np
 from torch import Tensor, flip, mean, rot90, stack
 
 
 # TODO add tests
 class ImageRestorationTTA:
     """
     Test-time augmentation for image restoration tasks.
@@ -44,15 +44,15 @@
             rot90(x, 3, dims=(-2, -1)),
         ]
         augmented_flip = augmented.copy()
         for x_ in augmented:
             augmented_flip.append(flip(x_, dims=(-3, -1)))
         return augmented_flip
 
-    def backward(self, x: List[Tensor]) -> np.ndarray:
+    def backward(self, x: List[Tensor]) -> Tensor:
         """Undo the test-time augmentation.
 
         Parameters
         ----------
         x : Any
             List of augmented tensors.
```

### Comparing `careamics-0.1.0rc4/src/careamics/utils/base_enum.py` & `careamics-0.1.0rc5/src/careamics/utils/base_enum.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/src/careamics/utils/context.py` & `careamics-0.1.0rc5/src/careamics/utils/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Context submodule.
 
 A convenience function to change the working directory in order to save data.
 """
+
 import os
 from contextlib import contextmanager
 from pathlib import Path
 from typing import Iterator, Union
 
 
 def get_careamics_home() -> Path:
```

### Comparing `careamics-0.1.0rc4/src/careamics/utils/logging.py` & `careamics-0.1.0rc5/src/careamics/utils/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Logging submodule.
 
 The methods are responsible for the in-console logger.
 """
+
 import logging
 import sys
 import time
 from pathlib import Path
 from typing import Any, Dict, Generator, List, Optional, Union
 
 LOGGERS: dict = {}
```

### Comparing `careamics-0.1.0rc4/src/careamics/utils/metrics.py` & `careamics-0.1.0rc5/src/careamics/utils/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Metrics submodule.
 
 This module contains various metrics and a metrics tracking class.
 """
+
 from typing import Union
 
 import numpy as np
 import torch
 from skimage.metrics import peak_signal_noise_ratio
```

### Comparing `careamics-0.1.0rc4/src/careamics/utils/path_utils.py` & `careamics-0.1.0rc5/src/careamics/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/src/careamics/utils/receptive_field.py` & `careamics-0.1.0rc5/src/careamics/utils/receptive_field.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/src/careamics/utils/running_stats.py` & `careamics-0.1.0rc5/src/careamics/utils/running_stats.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/src/careamics/utils/torch_utils.py` & `careamics-0.1.0rc5/src/careamics/utils/torch_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Convenience functions using torch.
 
 These functions are used to control certain aspects and behaviours of PyTorch.
 """
+
 import inspect
 from typing import Dict, Union
 
 import torch
 
 from careamics.config.support import SupportedOptimizer, SupportedScheduler
```

### Comparing `careamics-0.1.0rc4/tests/conftest.py` & `careamics-0.1.0rc5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/tests/test_careamist.py` & `careamics-0.1.0rc5/tests/test_careamist.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,26 +132,30 @@
         name="TopModel",
         general_description="A model that just walked in.",
         authors=[{"name": "Amod", "affiliation": "El"}],
     )
     assert (tmp_path / "model.zip").exists()
 
 
-def test_train_array_channel(tmp_path: Path, minimum_configuration: dict):
+@pytest.mark.parametrize("independent_channels", [False, True])
+def test_train_array_channel(
+    tmp_path: Path, minimum_configuration: dict, independent_channels: bool
+):
     """Test that CAREamics can be trained on arrays with channels."""
     # training data
     train_array = np.random.rand(32, 32, 3)
     val_array = np.random.rand(32, 32, 3)
 
     # create configuration
     config = Configuration(**minimum_configuration)
     config.training_config.num_epochs = 1
     config.data_config.axes = "YXC"
     config.algorithm_config.model.in_channels = 3
     config.algorithm_config.model.num_classes = 3
+    config.algorithm_config.model.independent_channels = independent_channels
     config.data_config.batch_size = 2
     config.data_config.data_type = SupportedData.ARRAY.value
     config.data_config.patch_size = (8, 8)
 
     # instantiate CAREamist
     careamist = CAREamist(source=config, work_dir=tmp_path)
```

### Comparing `careamics-0.1.0rc4/tests/test_conftest.py` & `careamics-0.1.0rc5/tests/test_conftest.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/tests/test_lightning_datamodule.py` & `careamics-0.1.0rc5/tests/test_lightning_datamodule.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/tests/test_lightning_module.py` & `careamics-0.1.0rc5/tests/test_lightning_module.py`

 * *Files 8% similar despite different names*

```diff
@@ -163,14 +163,48 @@
     model.model.eval()
     # test forward pass
     x = torch.rand((1, 1, *shape))
     y: torch.Tensor = model.forward(x)
     assert y.shape == x.shape
 
 
+@pytest.mark.parametrize(
+    "shape",
+    [
+        (8, 64, 64),
+        (16, 64, 64),
+        (16, 128, 128),
+        (32, 128, 128),
+    ],
+)
+def test_careamics_kiln_unet_depth_3_3D_n2v2(shape):
+    algo_dict = {
+        "algorithm": "n2v",
+        "model": {
+            "architecture": "UNet",
+            "conv_dims": 3,
+            "in_channels": 1,
+            "num_classes": 1,
+            "depth": 3,
+            "n2v2": True,
+        },
+        "loss": "n2v",
+    }
+    algo_config = AlgorithmConfig(**algo_dict)
+
+    # instantiate CAREamicsKiln
+    model = CAREamicsModule(algo_config)
+    # set model to evaluation mode to avoid batch dimension error
+    model.model.eval()
+    # test forward pass
+    x = torch.rand((1, 1, *shape))
+    y: torch.Tensor = model.forward(x)
+    assert y.shape == x.shape
+
+
 @pytest.mark.parametrize("n_channels", [1, 3, 4])
 def test_careamics_kiln_unet_depth_2_channels_2D(n_channels):
     algo_dict = {
         "algorithm": "n2n",
         "model": {
             "architecture": "UNet",
             "conv_dims": 2,
@@ -188,24 +222,28 @@
     model.model.eval()
     # test forward pass
     x = torch.rand((1, n_channels, 32, 32))
     y: torch.Tensor = model.forward(x)
     assert y.shape == x.shape
 
 
-@pytest.mark.parametrize("n_channels", [1, 3, 4])
-def test_careamics_kiln_unet_depth_3_channels_2D(n_channels):
+@pytest.mark.parametrize(
+    "n_channels,independent_channels",
+    [(1, False), (1, True), (3, False), (3, True), (4, False), (4, True)],
+)
+def test_careamics_kiln_unet_depth_3_channels_2D(n_channels, independent_channels):
     algo_dict = {
         "algorithm": "n2n",
         "model": {
             "architecture": "UNet",
             "conv_dims": 2,
             "in_channels": n_channels,
             "num_classes": n_channels,
             "depth": 3,
+            "independent_channels": independent_channels,
         },
         "loss": "mae",
     }
     algo_config = AlgorithmConfig(**algo_dict)
 
     # instantiate CAREamicsKiln
     model = CAREamicsModule(algo_config)
```

### Comparing `careamics-0.1.0rc4/tests/test_lightning_prediction_datamodule.py` & `careamics-0.1.0rc5/tests/test_lightning_prediction_datamodule.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/tests/config/test_algorithm_model.py` & `careamics-0.1.0rc5/tests/config/test_algorithm_model.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/tests/config/test_configuration_model.py` & `careamics-0.1.0rc5/tests/config/test_configuration_model.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/tests/config/test_data_model.py` & `careamics-0.1.0rc5/tests/config/test_data_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-from albumentations import Compose
 
 from careamics.config.data_model import DataConfig
 from careamics.config.support import (
     SupportedPixelManipulation,
     SupportedStructAxis,
     SupportedTransform,
 )
@@ -250,26 +249,14 @@
     model = DataConfig(**minimum_data)
 
     # Normalize
     params = model.transforms[0].model_dump()
     assert "mean" in params
     assert "std" in params
 
-    # NDFlip
-    params = model.transforms[1].model_dump()
-    assert "p" in params
-    assert "is_3D" in params
-    assert "flip_z" in params
-
-    # XYRandomRotate90
-    params = model.transforms[2].model_dump()
-    assert "p" in params
-    assert "is_3D" in params
-    assert isinstance(model.transforms[2], XYRandomRotate90Model)
-
     # N2VManipulate
     params = model.transforms[3].model_dump()
     assert "roi_size" in params
     assert "masked_pixel_percentage" in params
     assert "strategy" in params
     assert "struct_mask_axis" in params
     assert "struct_mask_span" in params
@@ -287,48 +274,14 @@
     minimum_data["transforms"] = [
         {"name": get_all_transforms()[SupportedTransform.NDFLIP.value]()},
     ]
     with pytest.raises(ValueError):
         DataConfig(**minimum_data)
 
 
-def test_passing_compose_transform(minimum_data: dict):
-    """Test that Compose transform can be passed."""
-    minimum_data["transforms"] = Compose(
-        [
-            get_all_transforms()[SupportedTransform.NDFLIP](),
-            get_all_transforms()[SupportedTransform.N2V_MANIPULATE](),
-        ]
-    )
-    DataConfig(**minimum_data)
-
-
-def test_3D_and_transforms(minimum_data: dict):
-    """Test that NDFlip is corrected if the data is 3D."""
-    minimum_data["transforms"] = [
-        {
-            "name": SupportedTransform.NDFLIP.value,
-            "is_3D": True,
-            "flip_z": True,
-        },
-        {
-            "name": SupportedTransform.XY_RANDOM_ROTATE90.value,
-            "is_3D": True,
-        },
-    ]
-    data = DataConfig(**minimum_data)
-    assert data.transforms[0].is_3D is False
-    assert data.transforms[1].is_3D is False
-
-    # change to 3D
-    data.set_3D("ZYX", [64, 64, 64])
-    data.transforms[0].is_3D = True
-    data.transforms[1].is_3D = True
-
-
 def test_set_n2v_strategy(minimum_data: dict):
     """Test that the N2V strategy can be set."""
     uniform = SupportedPixelManipulation.UNIFORM.value
     median = SupportedPixelManipulation.MEDIAN.value
 
     data = DataConfig(**minimum_data)
     assert data.transforms[-1].name == SupportedTransform.N2V_MANIPULATE.value
```

### Comparing `careamics-0.1.0rc4/tests/config/test_inference_model.py` & `careamics-0.1.0rc5/tests/config/test_inference_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-from albumentations import Compose
 
 from careamics.config.inference_model import InferenceConfig
 from careamics.config.support import (
     SupportedTransform,
 )
 from careamics.transforms import get_all_transforms
 
@@ -157,25 +156,14 @@
     minimum_inference["transforms"] = [
         {"name": get_all_transforms()[SupportedTransform.NDFLIP.value]()},
     ]
     with pytest.raises(ValueError):
         InferenceConfig(**minimum_inference)
 
 
-def test_passing_compose_transform(minimum_inference: dict):
-    """Test that Compose transform can be passed."""
-    minimum_inference["transforms"] = Compose(
-        [
-            get_all_transforms()[SupportedTransform.NORMALIZE](mean=10.4, std=3.2),
-            get_all_transforms()[SupportedTransform.NDFLIP](),
-        ]
-    )
-    InferenceConfig(**minimum_inference)
-
-
 def test_mean_and_std_in_normalize(minimum_inference: dict):
     """Test that mean and std are added to the Normalize transform."""
     minimum_inference["mean"] = 10.4
     minimum_inference["std"] = 3.2
     minimum_inference["transforms"] = [
         {"name": SupportedTransform.NORMALIZE.value},
     ]
```

### Comparing `careamics-0.1.0rc4/tests/config/test_optimizers_model.py` & `careamics-0.1.0rc5/tests/config/test_optimizers_model.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/tests/config/test_tile_information.py` & `careamics-0.1.0rc5/tests/config/test_tile_information.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/tests/config/architectures/test_custom_model.py` & `careamics-0.1.0rc5/tests/config/architectures/test_custom_model.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/tests/config/architectures/test_register_model.py` & `careamics-0.1.0rc5/tests/config/architectures/test_register_model.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/tests/config/architectures/test_unet_model.py` & `careamics-0.1.0rc5/tests/config/architectures/test_unet_model.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/tests/config/support/test_supported_data.py` & `careamics-0.1.0rc5/tests/config/support/test_supported_data.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/tests/config/support/test_supported_optimizers.py` & `careamics-0.1.0rc5/tests/config/support/test_supported_optimizers.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/tests/config/transformations/test_n2v_manipulate_model.py` & `careamics-0.1.0rc5/tests/config/transformations/test_n2v_manipulate_model.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/tests/config/validators/test_validator_utils.py` & `careamics-0.1.0rc5/tests/config/validators/test_validator_utils.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/tests/dataset/test_in_memory_dataset.py` & `careamics-0.1.0rc5/tests/dataset/test_in_memory_dataset.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/tests/dataset/test_iterable_dataset.py` & `careamics-0.1.0rc5/tests/dataset/test_iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/tests/dataset/dataset_utils/test_list_files.py` & `careamics-0.1.0rc5/tests/dataset/dataset_utils/test_list_files.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/tests/dataset/dataset_utils/test_read_tiff.py` & `careamics-0.1.0rc5/tests/dataset/dataset_utils/test_read_tiff.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/tests/dataset/patching/test_patching_utils.py` & `careamics-0.1.0rc5/tests/dataset/patching/test_patching_utils.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/tests/dataset/patching/test_random_patching.py` & `careamics-0.1.0rc5/tests/dataset/patching/test_random_patching.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/tests/dataset/patching/test_sequential_patching.py` & `careamics-0.1.0rc5/tests/dataset/patching/test_sequential_patching.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,31 @@
     The 3D array is a fixture of shape (1, 8, 16, 16)."""
     # TODO changed the fixture to (1, 8, 16, 16), uneven shape doesnt work. We need to
     # discuss the function or the test cases
     check_extract_patches_sequential(array_3D, patch_size)
 
 
 @pytest.mark.parametrize(
+    "patch_size",
+    [
+        (4, 4),
+        (8, 8),
+    ],
+)
+def test_extract_patches_sequential_2d_supervised(array_2D, patch_size):
+    """Test extracting patches sequentially in 2D with target."""
+    patches, targets = extract_patches_sequential(
+        array_2D, patch_size=patch_size, target=array_2D
+    )
+
+    # Check that the same region is extracted in the patches and targets
+    assert np.array_equal(patches, targets)
+
+
+@pytest.mark.parametrize(
     "shape, patch_sizes, expected",
     [
         ((1, 3, 10, 10), (1, 3, 10, 5), (1, 1, 1, 2)),
         ((1, 1, 9, 9), (1, 1, 4, 3), (1, 1, 3, 3)),
         ((1, 3, 10, 9), (1, 3, 3, 5), (1, 1, 4, 2)),
         ((1, 1, 5, 9, 10), (1, 1, 2, 3, 5), (1, 1, 3, 3, 2)),
     ],
```

### Comparing `careamics-0.1.0rc4/tests/dataset/patching/test_tiled_patching.py` & `careamics-0.1.0rc5/tests/dataset/patching/test_tiled_patching.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/tests/model_io/test_bmz_io.py` & `careamics-0.1.0rc5/tests/model_io/test_bmz_io.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/tests/models/test_model_factory.py` & `careamics-0.1.0rc5/tests/models/test_model_factory.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/tests/prediction/test_stitch_prediction.py` & `careamics-0.1.0rc5/tests/prediction/test_stitch_prediction.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/tests/transforms/test_manipulate_n2v.py` & `careamics-0.1.0rc5/tests/transforms/test_manipulate_n2v.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 import numpy as np
 import pytest
-from albumentations import Compose
 
 from careamics.config.support import SupportedPixelManipulation
 from careamics.transforms import N2VManipulate
 
 
 @pytest.mark.parametrize(
     "strategy",
     [SupportedPixelManipulation.UNIFORM.value, SupportedPixelManipulation.MEDIAN.value],
 )
 def test_manipulate_n2v(strategy):
     """Test the N2V augmentation."""
     # create array, adding a channel to simulate a 2D image with channel last
-    array = np.arange(16 * 16).reshape((16, 16))[..., np.newaxis]
+    array = np.arange(16 * 16).reshape((16, 16))[np.newaxis, ...]
 
     # create augmentation
-    aug = Compose(
-        [N2VManipulate(roi_size=5, masked_pixel_percentage=5, strategy=strategy)]
-    )
+    aug = N2VManipulate(roi_size=5, masked_pixel_percentage=5, strategy=strategy)
 
     # apply augmentation
-    augmented = aug(image=array)
-    assert "image" in augmented
-    assert len(augmented["image"]) == 3  # transformed_patch, original_patch, mask
+    augmented = aug(array)
+    assert len(augmented) == 3  # transformed_patch, original_patch, mask
 
     # assert that the difference between the original and transformed patch are the
     # same pixels that are selected by the mask
-    tr_path, orig_patch, mask = augmented["image"]
+    tr_path, orig_patch, mask = augmented
     diff_coords = np.array(np.where(tr_path != orig_patch))
     mask_coords = np.array(np.where(mask == 1))
     assert np.array_equal(diff_coords, mask_coords)
```

### Comparing `careamics-0.1.0rc4/tests/transforms/test_normalize.py` & `careamics-0.1.0rc5/tests/transforms/test_normalize.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 
 from careamics.transforms import Denormalize, Normalize
 
 
 def test_normalize_denormalize():
     """Test the Normalize transform."""
     # Create data
-    array = np.arange(100).reshape((1, 1, 10, 10))
+    array = np.arange(100).reshape((1, 10, 10))
 
     # Create the transform
     norm = Normalize(
         mean=50,
         std=25,
     )
 
     # Apply the transform
-    normalized: np.array = norm(image=array)["image"]
+    normalized, _ = norm(patch=array)
     assert np.abs(normalized.mean()) < 0.02
     assert np.abs(normalized.std() - 1) < 0.2
 
     # Create the denormalize transform
     denorm = Denormalize(
         mean=50,
         std=25,
     )
 
     # Apply the denormalize transform
-    denormalized: np.array = denorm(image=normalized)["image"]
+    denormalized, _ = denorm(patch=normalized)
     assert np.isclose(denormalized, array).all()
```

### Comparing `careamics-0.1.0rc4/tests/transforms/test_pixel_manipulation.py` & `careamics-0.1.0rc5/tests/transforms/test_pixel_manipulation.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/tests/utils/test_context.py` & `careamics-0.1.0rc5/tests/utils/test_context.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/tests/utils/test_logging.py` & `careamics-0.1.0rc5/tests/utils/test_logging.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/tests/utils/test_metrics.py` & `careamics-0.1.0rc5/tests/utils/test_metrics.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/tests/utils/test_torch_utils.py` & `careamics-0.1.0rc5/tests/utils/test_torch_utils.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/tests/utils/test_wandb.py` & `careamics-0.1.0rc5/tests/utils/test_wandb.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/LICENSE` & `careamics-0.1.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc4/pyproject.toml` & `careamics-0.1.0rc5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: BSD License",
     "Typing :: Typed",
 ]
 dependencies = [
     'torch>=2.0.0',
-    'albumentations',
     'bioimageio.core>=0.6.0',
     'tifffile',
     'psutil',
     'pydantic>=2.5',
     'pytorch_lightning>=2.2.0',
     'pyyaml',
     'scikit-image',
```

