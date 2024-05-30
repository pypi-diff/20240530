# Comparing `tmp/ethos-u-vela-3.8.0.tar.gz` & `tmp/ethos-u-vela-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ethos-u-vela-3.8.0.tar", last modified: Wed May 24 15:05:53 2023, max compression
+gzip compressed data, was "ethos-u-vela-3.9.0.tar", last modified: Thu Aug 24 09:43:38 2023, max compression
```

## Comparing `ethos-u-vela-3.8.0.tar` & `ethos-u-vela-3.9.0.tar`

### file list

```diff
@@ -1,319 +1,319 @@
-drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-05-24 15:05:53.093833 ethos-u-vela-3.8.0/
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)       94 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/.gitignore
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2119 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/.pre-commit-config.yaml
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4268 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/API.md
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     7925 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/BUGS.md
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3245 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/CONTRIBUTIONS.md
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4115 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/DEBUG_DB.md
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    11357 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/LICENSE.txt
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    27430 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/OPTIONS.md
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    13706 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/PERFORMANCE.md
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    12381 2023-05-24 15:05:53.093833 ethos-u-vela-3.8.0/PKG-INFO
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    10280 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/README.md
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    14105 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/RELEASES.md
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     5176 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/SECURITY.md
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    19014 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/SUPPORTED_OPS.md
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3209 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/TESTING.md
-drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-05-24 15:05:53.049833 ethos-u-vela-3.8.0/ethos_u_vela.egg-info/
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    12381 2023-05-24 15:05:52.000000 ethos-u-vela-3.8.0/ethos_u_vela.egg-info/PKG-INFO
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    10736 2023-05-24 15:05:53.000000 ethos-u-vela-3.8.0/ethos_u_vela.egg-info/SOURCES.txt
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)        1 2023-05-24 15:05:52.000000 ethos-u-vela-3.8.0/ethos_u_vela.egg-info/dependency_links.txt
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)       47 2023-05-24 15:05:52.000000 ethos-u-vela-3.8.0/ethos_u_vela.egg-info/entry_points.txt
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)      176 2023-05-24 15:05:52.000000 ethos-u-vela-3.8.0/ethos_u_vela.egg-info/requires.txt
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)        7 2023-05-24 15:05:52.000000 ethos-u-vela-3.8.0/ethos_u_vela.egg-info/top_level.txt
-drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-05-24 15:05:53.045832 ethos-u-vela-3.8.0/ethosu/
-drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-05-24 15:05:53.045832 ethos-u-vela-3.8.0/ethosu/config_files/
-drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-05-24 15:05:53.049833 ethos-u-vela-3.8.0/ethosu/config_files/Arm/
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3862 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/config_files/Arm/vela.ini
-drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-05-24 15:05:53.053833 ethos-u-vela-3.8.0/ethosu/mlw_codec/
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1291 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/mlw_codec/makefile
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     9389 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/mlw_codec/mlw_codecmodule.c
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)      958 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/mlw_codec/mlw_common.h
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    11109 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/mlw_codec/mlw_decode.c
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1089 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/mlw_codec/mlw_decode.h
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    41192 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/mlw_codec/mlw_encode.c
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1568 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/mlw_codec/mlw_encode.h
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     5347 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/mlw_codec/mlw_main.c
-drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-05-24 15:05:53.053833 ethos-u-vela-3.8.0/ethosu/mlw_codec/test/
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3234 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/mlw_codec/test/test_mlw_codec.py
-drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-05-24 15:05:53.061833 ethos-u-vela-3.8.0/ethosu/vela/
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)      742 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/__init__.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)      759 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/__main__.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)      766 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/_version.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    18665 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/api.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    17490 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/architecture_allocator.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    35247 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/architecture_features.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    15473 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/cascade_builder.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    11098 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/compiler_driver.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4845 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/data_type.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     6269 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/debug_database.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     5010 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/driver_actions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2725 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/errors.py
-drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-05-24 15:05:53.061833 ethos-u-vela-3.8.0/ethosu/vela/ethos_u55_regs/
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)        0 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/ethos_u55_regs/__init__.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)   133784 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/ethos_u55_regs/ethos_u55_regs.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    10290 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/extract_npu_subgraphs.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     7626 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/fp_math.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1986 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/graph_optimiser.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    13005 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/graph_optimiser_util.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2858 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/greedy_allocation.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    11920 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/high_level_command_stream.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    11652 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/high_level_command_stream_generator.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    29622 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/high_level_command_to_npu_op.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    15685 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/hillclimb_allocation.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    15911 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/live_range.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    17919 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/lstm.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    10255 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/lut.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4607 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/mark_tensors.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2544 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/model_reader.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    21118 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/nn_graph.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    38217 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/npu_performance.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     6711 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/npu_serialisation.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2444 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/numeric_util.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    37513 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/operation.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    11505 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/operation_util.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    20676 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/pass_packing.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     5022 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/range_set.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3261 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/rawdata_writer.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3098 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/reader_util.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    47761 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/register_command_stream_generator.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    23842 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/register_command_stream_util.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4546 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/rewrite_graph.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3672 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/scaling.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    76797 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/scheduler.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     6802 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/shape4d.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    31094 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/softmax.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    13943 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/stats_writer.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1101 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/supported_operators_util.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    33552 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tensor.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    10993 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tensor_allocation.py
-drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-05-24 15:05:53.065833 ethos-u-vela-3.8.0/ethosu/vela/test/
-drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-05-24 15:05:53.065833 ethos-u-vela-3.8.0/ethosu/vela/test/extapi/
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1834 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/extapi/test_extapi_create_payload.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1470 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/extapi/test_extapi_encode_bias.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2456 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/extapi/test_extapi_encode_weights.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4473 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/extapi/test_extapi_find_block_configs.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    19536 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/extapi/test_extapi_generate_commands.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1061 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/extapi/test_extapi_get_version.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4335 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/test_architecture_allocator.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2826 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/test_build.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1868 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/test_compiler_driver.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    13053 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/test_fp_math.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    24795 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/test_graph_optimiser.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1929 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/test_hillclimb_allocation.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2311 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/test_live_range.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     8952 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/test_lut.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1314 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/test_model_reader.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3032 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/test_new_performance.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1621 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/test_nng_mapping.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     9963 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/test_register_command_stream_util.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2122 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/test_scaling.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1775 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/test_tensor_allocation.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    27177 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/test_tflite_model_semantic.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     5272 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/test_tflite_reader.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    28590 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/test_tflite_supported_operators.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     6645 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/testutil.py
-drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-05-24 15:05:53.089833 ethos-u-vela-3.8.0/ethosu/vela/tflite/
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1157 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/ATan2Options.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1139 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/AbsOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)      220 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/ActivationFunctionType.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1148 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/AddNOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2148 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/AddOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1611 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/ArgMaxOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1611 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/ArgMinOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1238 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/AssignVariableOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2637 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/BatchMatMulOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1238 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/BatchToSpaceNDOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4593 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/BidirectionalSequenceLSTMOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3579 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/BidirectionalSequenceRNNOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1211 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/BroadcastToOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2641 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/BucketizeOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2383 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/Buffer.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3350 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/BuiltinOperator.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3381 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/BuiltinOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1693 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/CallOnceOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1575 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/CallOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2034 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/CastOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)      158 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/CombinerType.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     5049 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/ConcatEmbeddingsOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2219 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/ConcatenationOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3959 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/Conv2DOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4871 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/Conv3DOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1139 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/CosOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2044 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/CumsumOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)      146 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/CustomOptionsFormat.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2615 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/CustomQuantization.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1175 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/DensifyOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1677 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/DepthToSpaceOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4717 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/DepthwiseConv2DOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1202 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/DequantizeOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4301 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/DimensionMetadata.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)      153 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/DimensionType.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1679 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/DivOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1274 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/DynamicUpdateSliceOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1775 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/EmbeddingLookupSparseOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1157 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/EqualOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1139 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/ExpOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1202 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/ExpandDimsOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2914 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/FakeQuantOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1148 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/FillOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1184 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/FloorDivOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1184 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/FloorModOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3383 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/FullyConnectedOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)      182 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/FullyConnectedOptionsWeightsFormat.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1184 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/GatherNdOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2004 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/GatherOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1605 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/GeluOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1220 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/GreaterEqualOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1175 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/GreaterOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1193 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/HardSwishOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1229 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/HashtableFindOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1247 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/HashtableImportOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2517 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/HashtableOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1229 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/HashtableSizeOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2112 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/IfOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2496 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/Int32Vector.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1715 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/L2NormOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1647 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/LSHProjectionOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)      169 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/LSHProjectionType.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)      148 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/LSTMKernelType.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3559 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/LSTMOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1617 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/LeakyReluOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1193 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/LessEqualOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1148 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/LessOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3231 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/LocalResponseNormalizationOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1202 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/LogSoftmaxOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1202 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/LogicalAndOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1202 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/LogicalNotOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1193 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/LogicalOrOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1202 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/MatrixDiagOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1229 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/MatrixSetDiagOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1238 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/MaximumMinimumOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1935 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/Metadata.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)      154 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/MirrorPadMode.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1599 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/MirrorPadOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     9533 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/Model.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1679 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/MulOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1139 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/NegOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1283 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/NonMaxSuppressionV4Options.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1283 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/NonMaxSuppressionV5Options.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1184 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/NotEqualOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1565 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/OneHotOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    10212 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/Operator.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3032 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/OperatorCode.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1990 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/PackOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1139 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/PadOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1157 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/PadV2Options.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)      141 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/Padding.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3903 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/Pool2DOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1139 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/PowOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)      166 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/QuantizationDetails.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     8544 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/QuantizationParameters.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1184 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/QuantizeOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2237 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/RNNOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1972 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/RandomOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1157 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/RangeOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1148 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/RankOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1220 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/ReadVariableOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1617 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/ReducerOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2575 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/ReshapeOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2261 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/ResizeBilinearOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2365 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/ResizeNearestNeighborOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2147 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/ReverseSequenceOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1193 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/ReverseV2Options.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1166 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/Rfft2dOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2645 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SVDFOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1193 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/ScatterNdOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1202 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SegmentSumOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1166 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SelectOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1184 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SelectV2Options.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2819 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SequenceRNNOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1575 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/ShapeOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1148 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SignOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4583 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SignatureDef.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2599 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SkipGramOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1157 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SliceOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1585 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SoftmaxOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1238 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SpaceToBatchNDOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1677 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SpaceToDepthOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)      198 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SparseIndexVector.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1745 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SparseToDenseOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     5517 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SparsityParameters.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1593 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SplitOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1605 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SplitVOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1166 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SquareOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1265 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SquaredDifferenceOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2617 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SqueezeOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3571 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/StridedSliceOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     6637 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SubGraph.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2148 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SubOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     8406 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/Tensor.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1990 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/TensorMap.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)      398 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/TensorType.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1148 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/TileOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1166 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/TopKV2Options.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3130 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/TransposeConvOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1193 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/TransposeOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2515 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/Uint16Vector.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2496 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/Uint8Vector.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4089 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/UnidirectionalSequenceLSTMOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1611 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/UniqueOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1956 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/UnpackOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1274 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/UnsortedSegmentMaxOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1274 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/UnsortedSegmentMinOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1283 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/UnsortedSegmentProdOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1274 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/UnsortedSegmentSumOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2153 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/VarHandleOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3367 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/VariantSubType.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1157 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/WhereOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2157 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/WhileOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1193 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/ZerosLikeOptions.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)        0 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/__init__.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)   100599 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite_graph_optimiser.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    46097 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite_mapping.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    32755 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite_model_semantic.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    16397 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite_reader.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    39946 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite_supported_operators.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    22790 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite_writer.py
-drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-05-24 15:05:53.093833 ethos-u-vela-3.8.0/ethosu/vela/tosa/
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1068 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/ArithmeticRightShiftAttribute.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)      506 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/Attribute.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)      928 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/AxisAttribute.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1955 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/ClampAttribute.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1376 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/CondIfAttribute.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3706 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/ConvAttribute.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1280 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/ConvQuantInfo.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)      236 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/DType.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1264 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/MatMulQuantInfo.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)      924 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/MulAttribute.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1333 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/Op.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)      932 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/PadQuantInfo.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3692 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/PoolAttribute.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)      218 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/QuantInfo.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1282 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/ReluNAttribute.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4499 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/RescaleAttribute.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1657 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/ReshapeAttribute.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     6535 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/ResizeAttribute.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)      165 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/ResizeMode.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2653 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/SliceAttribute.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1652 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/TileAttribute.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4304 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/TosaBasicBlock.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1964 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/TosaGraph.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4042 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/TosaOperator.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3258 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/TosaTensor.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4998 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/TransposeConvAttribute.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1290 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/UnaryQuantInfo.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1879 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/Version.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1406 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/WhileLoopAttribute.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)        0 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/__init__.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    37007 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa_graph_optimiser.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    12356 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa_mapping.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2008 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa_model_semantic.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    12661 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa_reader.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    11180 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa_supported_operators.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3481 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/utils.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    26621 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/vela.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)    20790 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/weight_compressor.py
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2095 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/pyproject.toml
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)      220 2023-05-24 15:05:53.093833 ethos-u-vela-3.8.0/setup.cfg
--rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2735 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/setup.py
+drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-08-24 09:43:38.635177 ethos-u-vela-3.9.0/
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)       94 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/.gitignore
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2117 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4268 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/API.md
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     7925 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/BUGS.md
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3245 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/CONTRIBUTIONS.md
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4115 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/DEBUG_DB.md
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    11357 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/LICENSE.txt
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    29004 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/OPTIONS.md
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    13706 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/PERFORMANCE.md
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    13213 2023-08-24 09:43:38.635177 ethos-u-vela-3.9.0/PKG-INFO
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    11111 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/README.md
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    14725 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/RELEASES.md
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     5176 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/SECURITY.md
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    20505 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/SUPPORTED_OPS.md
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3209 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/TESTING.md
+drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-08-24 09:43:38.575176 ethos-u-vela-3.9.0/ethos_u_vela.egg-info/
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    13213 2023-08-24 09:43:38.000000 ethos-u-vela-3.9.0/ethos_u_vela.egg-info/PKG-INFO
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    10736 2023-08-24 09:43:38.000000 ethos-u-vela-3.9.0/ethos_u_vela.egg-info/SOURCES.txt
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)        1 2023-08-24 09:43:38.000000 ethos-u-vela-3.9.0/ethos_u_vela.egg-info/dependency_links.txt
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)       47 2023-08-24 09:43:38.000000 ethos-u-vela-3.9.0/ethos_u_vela.egg-info/entry_points.txt
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      176 2023-08-24 09:43:38.000000 ethos-u-vela-3.9.0/ethos_u_vela.egg-info/requires.txt
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)        7 2023-08-24 09:43:38.000000 ethos-u-vela-3.9.0/ethos_u_vela.egg-info/top_level.txt
+drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-08-24 09:43:38.571176 ethos-u-vela-3.9.0/ethosu/
+drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-08-24 09:43:38.571176 ethos-u-vela-3.9.0/ethosu/config_files/
+drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-08-24 09:43:38.575176 ethos-u-vela-3.9.0/ethosu/config_files/Arm/
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3862 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/config_files/Arm/vela.ini
+drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-08-24 09:43:38.579176 ethos-u-vela-3.9.0/ethosu/mlw_codec/
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1291 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/mlw_codec/makefile
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     9389 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/mlw_codec/mlw_codecmodule.c
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      958 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/mlw_codec/mlw_common.h
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    11109 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/mlw_codec/mlw_decode.c
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1089 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/mlw_codec/mlw_decode.h
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    41192 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/mlw_codec/mlw_encode.c
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1568 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/mlw_codec/mlw_encode.h
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     5347 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/mlw_codec/mlw_main.c
+drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-08-24 09:43:38.579176 ethos-u-vela-3.9.0/ethosu/mlw_codec/test/
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3234 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/mlw_codec/test/test_mlw_codec.py
+drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-08-24 09:43:38.591176 ethos-u-vela-3.9.0/ethosu/vela/
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      742 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/__init__.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      759 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/__main__.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      766 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/_version.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    18665 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/api.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    17490 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/architecture_allocator.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    35247 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/architecture_features.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    15414 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/cascade_builder.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    11098 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/compiler_driver.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4845 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/data_type.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     6269 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/debug_database.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     5016 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/driver_actions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3051 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/errors.py
+drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-08-24 09:43:38.591176 ethos-u-vela-3.9.0/ethosu/vela/ethos_u55_regs/
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)        0 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/ethos_u55_regs/__init__.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)   133784 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/ethos_u55_regs/ethos_u55_regs.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    11106 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/extract_npu_subgraphs.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     7626 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/fp_math.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1986 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/graph_optimiser.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    13168 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/graph_optimiser_util.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2858 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/greedy_allocation.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    11955 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/high_level_command_stream.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    11704 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/high_level_command_stream_generator.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    29982 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/high_level_command_to_npu_op.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    15685 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/hillclimb_allocation.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    16057 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/live_range.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    17919 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/lstm.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    15258 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/lut.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4607 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/mark_tensors.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2544 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/model_reader.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    20410 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/nn_graph.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    38381 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/npu_performance.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     6711 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/npu_serialisation.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2444 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/numeric_util.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    37473 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/operation.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    11505 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/operation_util.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    20666 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/pass_packing.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     5022 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/range_set.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3261 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/rawdata_writer.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3098 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/reader_util.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    49197 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/register_command_stream_generator.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    25018 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/register_command_stream_util.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4546 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/rewrite_graph.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3672 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/scaling.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    78012 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/scheduler.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     6802 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/shape4d.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    31094 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/softmax.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    13943 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/stats_writer.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1101 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/supported_operators_util.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    33552 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tensor.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    10993 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tensor_allocation.py
+drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-08-24 09:43:38.595176 ethos-u-vela-3.9.0/ethosu/vela/test/
+drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-08-24 09:43:38.595176 ethos-u-vela-3.9.0/ethosu/vela/test/extapi/
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1834 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/test/extapi/test_extapi_create_payload.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1470 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/test/extapi/test_extapi_encode_bias.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2456 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/test/extapi/test_extapi_encode_weights.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4473 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/test/extapi/test_extapi_find_block_configs.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    42025 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/test/extapi/test_extapi_generate_commands.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1061 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/test/extapi/test_extapi_get_version.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4335 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/test/test_architecture_allocator.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2826 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/test/test_build.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1868 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/test/test_compiler_driver.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    13053 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/test/test_fp_math.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    24795 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/test/test_graph_optimiser.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1929 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/test/test_hillclimb_allocation.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2311 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/test/test_live_range.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     8952 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/test/test_lut.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1314 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/test/test_model_reader.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3032 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/test/test_new_performance.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1621 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/test/test_nng_mapping.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     9963 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/test/test_register_command_stream_util.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2122 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/test/test_scaling.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1775 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/test/test_tensor_allocation.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    28897 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/test/test_tflite_model_semantic.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     5272 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/test/test_tflite_reader.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    31069 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/test/test_tflite_supported_operators.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     6645 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/test/testutil.py
+drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-08-24 09:43:38.631176 ethos-u-vela-3.9.0/ethosu/vela/tflite/
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1157 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/ATan2Options.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1139 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/AbsOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      220 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/ActivationFunctionType.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1148 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/AddNOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2148 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/AddOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1611 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/ArgMaxOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1611 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/ArgMinOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1238 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/AssignVariableOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2637 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/BatchMatMulOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1238 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/BatchToSpaceNDOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4593 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/BidirectionalSequenceLSTMOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3579 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/BidirectionalSequenceRNNOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1211 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/BroadcastToOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2641 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/BucketizeOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2383 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/Buffer.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3350 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/BuiltinOperator.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3381 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/BuiltinOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1693 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/CallOnceOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1575 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/CallOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2034 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/CastOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      158 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/CombinerType.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     5049 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/ConcatEmbeddingsOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2219 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/ConcatenationOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3959 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/Conv2DOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4871 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/Conv3DOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1139 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/CosOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2044 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/CumsumOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      146 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/CustomOptionsFormat.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2615 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/CustomQuantization.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1175 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/DensifyOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1677 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/DepthToSpaceOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4717 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/DepthwiseConv2DOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1202 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/DequantizeOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4301 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/DimensionMetadata.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      153 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/DimensionType.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1679 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/DivOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1274 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/DynamicUpdateSliceOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1775 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/EmbeddingLookupSparseOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1157 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/EqualOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1139 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/ExpOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1202 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/ExpandDimsOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2914 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/FakeQuantOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1148 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/FillOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1184 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/FloorDivOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1184 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/FloorModOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3383 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/FullyConnectedOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      182 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/FullyConnectedOptionsWeightsFormat.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1184 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/GatherNdOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2004 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/GatherOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1605 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/GeluOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1220 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/GreaterEqualOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1175 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/GreaterOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1193 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/HardSwishOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1229 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/HashtableFindOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1247 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/HashtableImportOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2517 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/HashtableOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1229 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/HashtableSizeOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2112 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/IfOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2496 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/Int32Vector.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1715 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/L2NormOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1647 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/LSHProjectionOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      169 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/LSHProjectionType.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      148 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/LSTMKernelType.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3559 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/LSTMOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1617 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/LeakyReluOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1193 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/LessEqualOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1148 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/LessOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3231 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/LocalResponseNormalizationOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1202 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/LogSoftmaxOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1202 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/LogicalAndOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1202 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/LogicalNotOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1193 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/LogicalOrOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1202 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/MatrixDiagOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1229 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/MatrixSetDiagOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1238 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/MaximumMinimumOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1935 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/Metadata.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      154 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/MirrorPadMode.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1599 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/MirrorPadOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     9533 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/Model.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1679 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/MulOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1139 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/NegOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1283 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/NonMaxSuppressionV4Options.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1283 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/NonMaxSuppressionV5Options.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1184 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/NotEqualOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1565 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/OneHotOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    10212 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/Operator.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3032 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/OperatorCode.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1990 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/PackOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1139 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/PadOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1157 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/PadV2Options.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      141 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/Padding.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3903 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/Pool2DOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1139 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/PowOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      166 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/QuantizationDetails.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     8544 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/QuantizationParameters.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1184 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/QuantizeOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2237 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/RNNOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1972 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/RandomOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1157 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/RangeOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1148 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/RankOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1220 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/ReadVariableOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1617 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/ReducerOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2575 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/ReshapeOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2261 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/ResizeBilinearOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2365 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/ResizeNearestNeighborOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2147 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/ReverseSequenceOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1193 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/ReverseV2Options.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1166 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/Rfft2dOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2645 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/SVDFOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1193 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/ScatterNdOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1202 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/SegmentSumOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1166 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/SelectOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1184 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/SelectV2Options.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2819 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/SequenceRNNOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1575 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/ShapeOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1148 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/SignOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4583 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/SignatureDef.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2599 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/SkipGramOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1157 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/SliceOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1585 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/SoftmaxOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1238 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/SpaceToBatchNDOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1677 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/SpaceToDepthOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      198 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/SparseIndexVector.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1745 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/SparseToDenseOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     5517 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/SparsityParameters.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1593 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/SplitOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1605 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/SplitVOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1166 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/SquareOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1265 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/SquaredDifferenceOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2617 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/SqueezeOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3571 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/StridedSliceOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     6637 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/SubGraph.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2148 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/SubOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     8406 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/Tensor.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1990 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/TensorMap.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      398 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/TensorType.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1148 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/TileOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1166 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/TopKV2Options.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3130 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/TransposeConvOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1193 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/TransposeOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2515 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/Uint16Vector.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2496 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/Uint8Vector.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4717 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/UnidirectionalSequenceLSTMOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1611 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/UniqueOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1956 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/UnpackOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1274 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/UnsortedSegmentMaxOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1274 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/UnsortedSegmentMinOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1283 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/UnsortedSegmentProdOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1274 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/UnsortedSegmentSumOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2153 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/VarHandleOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3367 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/VariantSubType.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1157 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/WhereOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2157 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/WhileOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1193 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/ZerosLikeOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)        0 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite/__init__.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)   114614 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite_graph_optimiser.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    46239 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite_mapping.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    36165 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite_model_semantic.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    16397 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite_reader.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    43725 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite_supported_operators.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    22993 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tflite_writer.py
+drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-08-24 09:43:38.635177 ethos-u-vela-3.9.0/ethosu/vela/tosa/
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1068 2023-08-24 09:42:02.000000 ethos-u-vela-3.9.0/ethosu/vela/tosa/ArithmeticRightShiftAttribute.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      506 2023-08-24 09:42:02.000000 ethos-u-vela-3.9.0/ethosu/vela/tosa/Attribute.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      928 2023-08-24 09:42:02.000000 ethos-u-vela-3.9.0/ethosu/vela/tosa/AxisAttribute.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1955 2023-08-24 09:42:02.000000 ethos-u-vela-3.9.0/ethosu/vela/tosa/ClampAttribute.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1376 2023-08-24 09:42:02.000000 ethos-u-vela-3.9.0/ethosu/vela/tosa/CondIfAttribute.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3706 2023-08-24 09:42:02.000000 ethos-u-vela-3.9.0/ethosu/vela/tosa/ConvAttribute.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1280 2023-08-24 09:42:02.000000 ethos-u-vela-3.9.0/ethosu/vela/tosa/ConvQuantInfo.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      236 2023-08-24 09:42:02.000000 ethos-u-vela-3.9.0/ethosu/vela/tosa/DType.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1264 2023-08-24 09:42:02.000000 ethos-u-vela-3.9.0/ethosu/vela/tosa/MatMulQuantInfo.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      924 2023-08-24 09:42:02.000000 ethos-u-vela-3.9.0/ethosu/vela/tosa/MulAttribute.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1333 2023-08-24 09:42:02.000000 ethos-u-vela-3.9.0/ethosu/vela/tosa/Op.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      932 2023-08-24 09:42:02.000000 ethos-u-vela-3.9.0/ethosu/vela/tosa/PadQuantInfo.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3692 2023-08-24 09:42:02.000000 ethos-u-vela-3.9.0/ethosu/vela/tosa/PoolAttribute.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      218 2023-08-24 09:42:02.000000 ethos-u-vela-3.9.0/ethosu/vela/tosa/QuantInfo.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1282 2023-08-24 09:42:02.000000 ethos-u-vela-3.9.0/ethosu/vela/tosa/ReluNAttribute.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4499 2023-08-24 09:42:02.000000 ethos-u-vela-3.9.0/ethosu/vela/tosa/RescaleAttribute.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1657 2023-08-24 09:42:02.000000 ethos-u-vela-3.9.0/ethosu/vela/tosa/ReshapeAttribute.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     6535 2023-08-24 09:42:02.000000 ethos-u-vela-3.9.0/ethosu/vela/tosa/ResizeAttribute.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      165 2023-08-24 09:42:02.000000 ethos-u-vela-3.9.0/ethosu/vela/tosa/ResizeMode.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2653 2023-08-24 09:42:02.000000 ethos-u-vela-3.9.0/ethosu/vela/tosa/SliceAttribute.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1652 2023-08-24 09:42:02.000000 ethos-u-vela-3.9.0/ethosu/vela/tosa/TileAttribute.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4304 2023-08-24 09:42:02.000000 ethos-u-vela-3.9.0/ethosu/vela/tosa/TosaBasicBlock.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1964 2023-08-24 09:42:02.000000 ethos-u-vela-3.9.0/ethosu/vela/tosa/TosaGraph.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4042 2023-08-24 09:42:02.000000 ethos-u-vela-3.9.0/ethosu/vela/tosa/TosaOperator.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3258 2023-08-24 09:42:02.000000 ethos-u-vela-3.9.0/ethosu/vela/tosa/TosaTensor.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4998 2023-08-24 09:42:02.000000 ethos-u-vela-3.9.0/ethosu/vela/tosa/TransposeConvAttribute.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1290 2023-08-24 09:42:02.000000 ethos-u-vela-3.9.0/ethosu/vela/tosa/UnaryQuantInfo.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1879 2023-08-24 09:42:02.000000 ethos-u-vela-3.9.0/ethosu/vela/tosa/Version.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1406 2023-08-24 09:42:02.000000 ethos-u-vela-3.9.0/ethosu/vela/tosa/WhileLoopAttribute.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)        0 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tosa/__init__.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    37007 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tosa_graph_optimiser.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    12356 2023-08-24 09:42:02.000000 ethos-u-vela-3.9.0/ethosu/vela/tosa_mapping.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2008 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tosa_model_semantic.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    12661 2023-08-24 09:42:02.000000 ethos-u-vela-3.9.0/ethosu/vela/tosa_reader.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    11180 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/tosa_supported_operators.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4957 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/utils.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    26621 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/vela.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    20790 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/ethosu/vela/weight_compressor.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2320 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/pyproject.toml
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      220 2023-08-24 09:43:38.635177 ethos-u-vela-3.9.0/setup.cfg
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2735 2023-08-24 09:41:53.000000 ethos-u-vela-3.9.0/setup.py
```

### Comparing `ethos-u-vela-3.8.0/.pre-commit-config.yaml` & `ethos-u-vela-3.9.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 -   repo: local
     hooks:
     -   id: pytest
         name: pytest
         stages: [commit]
         language: system
-        entry: pytest -s -v .
+        entry: pytest -s -v
         types: [python]
         pass_filenames: false
         always_run: true
 
     -   id: pytest-cov
         name: pytest-cov
         stages: [push]
```

### Comparing `ethos-u-vela-3.8.0/API.md` & `ethos-u-vela-3.9.0/API.md`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/BUGS.md` & `ethos-u-vela-3.9.0/BUGS.md`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/CONTRIBUTIONS.md` & `ethos-u-vela-3.9.0/CONTRIBUTIONS.md`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/DEBUG_DB.md` & `ethos-u-vela-3.9.0/DEBUG_DB.md`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/LICENSE.txt` & `ethos-u-vela-3.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/OPTIONS.md` & `ethos-u-vela-3.9.0/OPTIONS.md`

 * *Files 4% similar despite different names*

```diff
@@ -394,16 +394,16 @@
 vela network.tflite --verbose-performance
 ```
 
 ### Verbose Tensor Purpose
 
 Displays a list of all operators and the tensors that are connected to them.
 Additional information is shown about the tensors. The format is:
-`<num> <op_type> <op_name>`, where;  
-`  <direction> <idx> <purpose> <mem_area> <mem_type> <tens>`, where;  
+`<num> <op_type> <op_name> <direction> <idx> <purpose> <mem_area> <mem_type>
+<tens>`, where;  
 num = an increasing operator count  
 op_type = the Graph IR Operator Type  
 op_name = the Graph IR Operator Name (this may have been derived from the
 corresponding TFLite operator name)  
 direction = either *Input* or *Output* and indicates the connection direction of
 the tensor with respect 
 idx = the index position where on each operator  
@@ -462,26 +462,59 @@
 
 ```bash
 vela network.tflite --verbose-allocation
 ```
 
 ### Verbose High Level Command Stream
 
-Display a high level command stream with one command per DMA or NPU stripe. The
-commands contain information about block configuration as well as IFM-, OFM-
-and weight boxes.  
+Display an enumerated list of High-Level (HL) commands in execution
+order.  There are three types of command and each one displays individual
+information:
+
+* NPU Stripe = `<name> <ifm_box> <ifm2_box> <ofm_box> <weight_box>
+<block_config>`, represents a data processing operation that maps directly to
+a single Ethos-U operation where;  
+name = name of the pass that corresponds to this HL command (not unique)  
+ifm_box = part of the IFM in NHWC format  
+ifm2_box = part of the IFM2 in NHWC format (is empty [] when not present)  
+ofm_box = part of the OFM in NHWC format  
+weight_box = part of the filter kernel in NHWC format  
+block_config = block processing size in HWIO format
+
+* DMA = `<in> <out> <box>`, represents a memory copy operation from source to
+destination where;  
+name = name of the pass that corresponds to this HL command (not unique)  
+in = name of the source tensor  
+out = name of the destination tensor  
+box = part of the source tensor in NHWC format
+
+* NOP = `<in> <out>`, represents a memory copy operation that has source equal
+to destination and therefore does nothing, where;  
+name = name of the pass that corresponds to this HL command (not unique)  
+in = name of the input tensor  
+out = name of the output tensor
 
 ```bash
 vela network.tflite --verbose-high-level-command-stream
 ```
 
 ### Verbose Register Command Stream
 
-Display all NPU operations and a register level (low level) command stream with
-all register settings for the network execution on the NPU.  
+Display two groups of information.  The first group is the input to the register
+command stream generator.  The second group is the output of the register
+command stream generator:
+
+* Input = an enumerated list of the High-Level commands that are the input to
+the generator.  Each command details all of its attributes.
+
+* Output = a disassembly of the Ethos-U command stream (referred to as the
+register command stream).  More information about the commands listed in the
+register command stream can be found in the Arm Ethos-U NPU Technical Reference
+Manuals that are available from the Arm Developer website (see
+[README - Resources](README.md#resources)).
 
 ```bash
 vela network.tflite --verbose-register-command-stream
 ```
 
 ### Verbose Operators
```

### Comparing `ethos-u-vela-3.8.0/PERFORMANCE.md` & `ethos-u-vela-3.9.0/PERFORMANCE.md`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/PKG-INFO` & `ethos-u-vela-3.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: ethos-u-vela
-Version: 3.8.0
+Version: 3.9.0
 Summary: Neural network model compiler for Arm Ethos-U NPUs
 Author-email: Arm Ltd <mlg-vela@arm.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://git.mlplatform.org/ml/ethos-u/ethos-u-vela.git/
 Keywords: ethos-u,vela compiler,tflite,npu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Compilers
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 <!--
 SPDX-FileCopyrightText: Copyright 2020-2023 Arm Limited and/or its affiliates <open-source-office@arm.com>
 
@@ -64,39 +64,57 @@
 compiled model.
 
 The tool has limited functionality for compiling a
 [TOSA](https://git.mlplatform.org/tosa/specification.git/) neural network
 (EXPERIMENTAL).
 
 ## TensorFlow Support
-* Vela 3.8.0 to current supports TensorFlow 2.11
+Vela is tested by comparing the numerical behaviour of the optimised operators
+against that of the corresponding TensorFlow Lite reference kernels.  The
+following list indicates which version is used for comparison:
+
+* Vela 3.9.0 to current supports TensorFlow 2.12
+* Vela 3.8.0 supports TensorFlow 2.11
 * Vela 3.6.0 to 3.7.0 supports TensorFlow 2.10
 * Vela 3.5.0 supports TensorFlow 2.9
 * Vela 3.4.0 supports TensorFlow 2.8
 * Vela 3.3.0 supports TensorFlow 2.7
 * Vela 3.1.0 to 3.2.0 supports TensorFlow 2.5
 * Vela 2.1.0 to 3.0.0 supports TensorFlow 2.4
 * Vela 2.0.0 to 2.0.1 supports TensorFlow 2.3
 * Vela 0.1.0 to 1.2.0 supports TensorFlow 2.1
 
+## Python Version Support
+The majority of Vela's testing is done using a single version of Python, as
+indicated by the first version in the list below.  However, some additional
+testing is also performed across a range of newer versions starting at the
+minimum version (pyproject.toml:project.requires-python) indicated in the
+brackets:
+
+* Vela 3.9.0 to current supports Python 3.10 (3.8)
+* Vela 3.8.0 supports Python 3.9 (3.8)
+* Vela 3.4.0 to 3.7.0 supports Python 3.7 (3.8)
+* Vela 3.3.0 supports Python 3.8 (3.7)
+* Vela 0.1.0 to 3.2.0 supports Python 3.6 (3.7)
+
 ## Environment
 
 Vela runs on Linux and Microsoft Windows 10 operating systems.
 
 ## Prerequisites
 
 The following should be installed prior to the installation of Vela:
 
-* Python 3.9 or compatible
+* Python 3.10 or compatible
    - Development version containing the Python/C API header files
-   - e.g. `apt install python3.9-dev` or `yum install python39-devel`
+   - e.g. `apt install python3.10-dev` or `yum install python310-devel`
 * Pip3
-* A C99 capable compiler and associated toolchain
+* C99 capable compiler and associated toolchain
     - For Linux operating systems, a GNU toolchain is recommended.
-    - For Microsoft Windows 10, Microsoft Visual C++ 14.2 Build Tools is recommended.
+    - For Microsoft Windows 10, the Microsoft Visual C++ 14.2 Build Tools are recommended.
       See <https://wiki.python.org/moin/WindowsCompilers>
 
 ## Installation
 
 Vela is available to install as a package from
 [PyPi](https://pypi.org/project/ethos-u-vela/), or as
 source code from
@@ -132,29 +150,29 @@
 #### Advanced Installation for Developers
 
 If you plan to modify the Vela codebase then it is recommended to install Vela
 as an editable package to avoid the need to re-install after every modification.
 This is done by adding the `-e` option to the install command like so:
 
 ```bash
-pip3 install -e .
+pip3 install -e .[dev]
 ```
 
 If you plan to contribute to the Vela project (highly encouraged!) then it is
 recommended to install Vela with the development dependencies (see
-[Vela Testing](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/TESTING.md) for more details).
+[Vela Testing](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.9.0/TESTING.md) for more details).
 
 ## Running
 
 Vela is run with an input `.tflite` or `.tosa` (EXPERIMENTAL) file passed on the
 command line. This file contains the neural network to be compiled. The tool then
 outputs an optimised `.tflite` file with a `_vela` suffix in the file name, along
 with performance estimate (EXPERIMENTAL) CSV files, all to the output directory.
 It also prints a performance estimation summary back to the console, see
-[Vela Performance Estimation Summary](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/PERFORMANCE.md).
+[Vela Performance Estimation Summary](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.9.0/PERFORMANCE.md).
 
 Example usage:
 
 1) Compile the network `my_model.tflite`.  The optimised version will be output
 to `./output/my_network_vela.tflite`.
 
 ```bash
@@ -241,15 +259,15 @@
 the mlw_codec and the current version of NumPy.
 
 **Example scenario:**
 
 In the ethos-u-vela source directory, run:
 
 ```bash
-virtualenv -p 3.9 venv
+virtualenv -p 3.10 venv
 . venv/bin/activate
 pip install ethos-u-vela
 ```
 
 Next, install a different NumPy version (e.g. 1.21.3)
 
 ```bash
@@ -287,66 +305,66 @@
    in mlw_codec during the build process.
    ```
    pip install ethos-u-vela --no-build-isolation --no-cache-dir
    ```
 
 ## APIs
 
-Please see [Vela External APIs](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/API.md).
+Please see [Vela External APIs](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.9.0/API.md).
 
 ## Bug Reporting
 
-Please see [Vela Community Bug Reporting](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/BUGS.md) for a description of how to
+Please see [Vela Community Bug Reporting](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.9.0/BUGS.md) for a description of how to
 report bugs.
 
 ## Contributions
 
-Please see [Vela Contributions](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/CONTRIBUTIONS.md).
+Please see [Vela Contributions](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.9.0/CONTRIBUTIONS.md).
 
 ## Debug Database
 
-Please see [Vela Debug Database](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/DEBUG_DB.md).
+Please see [Vela Debug Database](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.9.0/DEBUG_DB.md).
 
 ## Inclusive language commitment
 
 This product conforms to Arm’s inclusive language policy and, to the best of
 our knowledge, does not contain any non-inclusive language. If you find
 something that concerns you, email terms@arm.com.
 
 ## Options
 
-Please see [Vela CLI Options](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/OPTIONS.md).  This includes a description of the
+Please see [Vela CLI Options](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.9.0/OPTIONS.md).  This includes a description of the
 system configuration file format.
 
 ## Performance
 
-Please see [Vela Performance Estimation Summary](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/PERFORMANCE.md).
+Please see [Vela Performance Estimation Summary](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.9.0/PERFORMANCE.md).
 
 ## Releases
 
-Please see [Vela Releases](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/RELEASES.md).
+Please see [Vela Releases](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.9.0/RELEASES.md).
 
 ## Resources
 
 Additional useful information:
 
 * [Arm Products: Ethos-U55 NPU](https://www.arm.com/products/silicon-ip-cpu/ethos/ethos-u55)
 * [Arm Products: Ethos-U65 NPU](https://www.arm.com/products/silicon-ip-cpu/ethos/ethos-u65)
 * [Arm Developer: Ethos-U55 NPU](https://developer.arm.com/ip-products/processors/machine-learning/arm-ethos-u/ethos-u55)
 * [Arm Developer: Ethos-U65 NPU](https://developer.arm.com/ip-products/processors/machine-learning/arm-ethos-u/ethos-u65)
 
 ## Security
 
-Please see [Vela Security](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/SECURITY.md).
+Please see [Vela Security](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.9.0/SECURITY.md).
 
 ## Supported Operators
 
-Please see [Vela Supported Operators](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/SUPPORTED_OPS.md) for the list of
+Please see [Vela Supported Operators](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.9.0/SUPPORTED_OPS.md) for the list of
 operators supported in this release.
 
 ## Testing
 
-Please see [Vela Testing](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/TESTING.md).
+Please see [Vela Testing](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.9.0/TESTING.md).
 
 ## License
 
-Vela is licensed under [Apache License 2.0](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/LICENSE.txt).
+Vela is licensed under [Apache License 2.0](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.9.0/LICENSE.txt).
```

### Comparing `ethos-u-vela-3.8.0/README.md` & `ethos-u-vela-3.9.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -41,39 +41,57 @@
 compiled model.
 
 The tool has limited functionality for compiling a
 [TOSA](https://git.mlplatform.org/tosa/specification.git/) neural network
 (EXPERIMENTAL).
 
 ## TensorFlow Support
-* Vela 3.8.0 to current supports TensorFlow 2.11
+Vela is tested by comparing the numerical behaviour of the optimised operators
+against that of the corresponding TensorFlow Lite reference kernels.  The
+following list indicates which version is used for comparison:
+
+* Vela 3.9.0 to current supports TensorFlow 2.12
+* Vela 3.8.0 supports TensorFlow 2.11
 * Vela 3.6.0 to 3.7.0 supports TensorFlow 2.10
 * Vela 3.5.0 supports TensorFlow 2.9
 * Vela 3.4.0 supports TensorFlow 2.8
 * Vela 3.3.0 supports TensorFlow 2.7
 * Vela 3.1.0 to 3.2.0 supports TensorFlow 2.5
 * Vela 2.1.0 to 3.0.0 supports TensorFlow 2.4
 * Vela 2.0.0 to 2.0.1 supports TensorFlow 2.3
 * Vela 0.1.0 to 1.2.0 supports TensorFlow 2.1
 
+## Python Version Support
+The majority of Vela's testing is done using a single version of Python, as
+indicated by the first version in the list below.  However, some additional
+testing is also performed across a range of newer versions starting at the
+minimum version (pyproject.toml:project.requires-python) indicated in the
+brackets:
+
+* Vela 3.9.0 to current supports Python 3.10 (3.8)
+* Vela 3.8.0 supports Python 3.9 (3.8)
+* Vela 3.4.0 to 3.7.0 supports Python 3.7 (3.8)
+* Vela 3.3.0 supports Python 3.8 (3.7)
+* Vela 0.1.0 to 3.2.0 supports Python 3.6 (3.7)
+
 ## Environment
 
 Vela runs on Linux and Microsoft Windows 10 operating systems.
 
 ## Prerequisites
 
 The following should be installed prior to the installation of Vela:
 
-* Python 3.9 or compatible
+* Python 3.10 or compatible
    - Development version containing the Python/C API header files
-   - e.g. `apt install python3.9-dev` or `yum install python39-devel`
+   - e.g. `apt install python3.10-dev` or `yum install python310-devel`
 * Pip3
-* A C99 capable compiler and associated toolchain
+* C99 capable compiler and associated toolchain
     - For Linux operating systems, a GNU toolchain is recommended.
-    - For Microsoft Windows 10, Microsoft Visual C++ 14.2 Build Tools is recommended.
+    - For Microsoft Windows 10, the Microsoft Visual C++ 14.2 Build Tools are recommended.
       See <https://wiki.python.org/moin/WindowsCompilers>
 
 ## Installation
 
 Vela is available to install as a package from
 [PyPi](https://pypi.org/project/ethos-u-vela/), or as
 source code from
@@ -109,15 +127,15 @@
 #### Advanced Installation for Developers
 
 If you plan to modify the Vela codebase then it is recommended to install Vela
 as an editable package to avoid the need to re-install after every modification.
 This is done by adding the `-e` option to the install command like so:
 
 ```bash
-pip3 install -e .
+pip3 install -e .[dev]
 ```
 
 If you plan to contribute to the Vela project (highly encouraged!) then it is
 recommended to install Vela with the development dependencies (see
 [Vela Testing](TESTING.md) for more details).
 
 ## Running
@@ -218,15 +236,15 @@
 the mlw_codec and the current version of NumPy.
 
 **Example scenario:**
 
 In the ethos-u-vela source directory, run:
 
 ```bash
-virtualenv -p 3.9 venv
+virtualenv -p 3.10 venv
 . venv/bin/activate
 pip install ethos-u-vela
 ```
 
 Next, install a different NumPy version (e.g. 1.21.3)
 
 ```bash
```

### Comparing `ethos-u-vela-3.8.0/RELEASES.md` & `ethos-u-vela-3.9.0/RELEASES.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,36 @@
 # Vela Releases
 
 These are the release notes for all Vela releases.  They document all of the
 main feature changes, interface changes and reported defects that have been
 fixed.  The version numbering adheres to the
 [semantic versioning](https://semver.org/) scheme.
 
+## Release 3.9.0 - 15/08/2023
+
+**Main feature changes:**
+
+* New operator support: RSQRT
+* Extended Mean operator support
+* Enabled weight buffering for the Size optimisation strategy (CLI option "--optimise Size")
+* Improved documentation of verbose CLI options
+* Upgrade TensorFlow Lite support to version 2.12
+
+**Interface changes:**
+
+* None
+
+**Reported defect fixes:**
+
+* Fixed crash when rewriting Slice operator (MLCE-918)
+* Fixed issues with faulty memory overwrite for reshape operator (MLCE-1003)
+* Fixed runtime issues for grouped convolutions (MLCE-1076)
+* Enabled cascading for resize operators (MLCE-1058)
+
+
 ## Release 3.8.0 - 17/05/2023
 
 **Main feature changes:**
 
 * New operator support: ARG_MAX, UNIDIRECTIONAL_SEQUENCE_LSTM, EXP
 * Improved CONV_2D striding support
 * Upgrade TensorFlow Lite support to version 2.11
```

### Comparing `ethos-u-vela-3.8.0/SECURITY.md` & `ethos-u-vela-3.9.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/SUPPORTED_OPS.md` & `ethos-u-vela-3.9.0/SUPPORTED_OPS.md`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 -->
 
 # Supported Ops
 
 This file was automatically generated by Vela using the `--supported-ops-report` parameter.  
-Vela version: `3.8.0`
+Vela version: `3.9.0`
 
 This file complies with
 [**Gitiles Markdown syntax**](https://github.com/google/gitiles/blob/master/Documentation/markdown.md)
 
 Summary table of constraints for:
 - [TFLite](#tflite-summary-table)
 
@@ -60,16 +60,17 @@
 | QUANTIZE | [Generic](#tflite-generic-constraints) |
 | RELU | [Generic](#tflite-generic-constraints) |
 | RELU6 | [Generic](#tflite-generic-constraints) |
 | RELU_N1_TO_1 | [Generic](#tflite-generic-constraints) |
 | RESHAPE | [Generic](#tflite-generic-constraints), [Specific](#tflite-reshape-constraints) |
 | RESIZE_BILINEAR | [Generic](#tflite-generic-constraints), [Specific](#tflite-resize_bilinear-constraints) |
 | RESIZE_NEAREST_NEIGHBOR | [Generic](#tflite-generic-constraints), [Specific](#tflite-resize_nearest_neighbor-constraints) |
+| RSQRT | [Generic](#tflite-generic-constraints), [Specific](#tflite-rsqrt-constraints) |
 | SHAPE | [Generic](#tflite-generic-constraints) |
-| SLICE | [Generic](#tflite-generic-constraints) |
+| SLICE | [Generic](#tflite-generic-constraints), [Specific](#tflite-slice-constraints) |
 | SOFTMAX | [Generic](#tflite-generic-constraints), [Specific](#tflite-softmax-constraints) |
 | SPLIT | [Generic](#tflite-generic-constraints), [Specific](#tflite-split-constraints) |
 | SPLIT_V | [Generic](#tflite-generic-constraints), [Specific](#tflite-split_v-constraints) |
 | SQUEEZE | [Generic](#tflite-generic-constraints), [Specific](#tflite-squeeze-constraints) |
 | STRIDED_SLICE | [Generic](#tflite-generic-constraints), [Specific](#tflite-strided_slice-constraints) |
 | SUB | [Generic](#tflite-generic-constraints), [Specific](#tflite-sub-constraints) |
 | TANH | [Generic](#tflite-generic-constraints) |
@@ -129,15 +130,16 @@
 ### TFLite AVERAGE_POOL_2D Constraints
 
 This is a list of constraints that the AVERAGE_POOL_2D operator must satisfy in order to be scheduled on the NPU.
 
 - Stride values for both width and height must be integer types
 - IFM and OFM data types must match
 - Kernel filter values for both width and height must be integer types
-- Stride values for both width and height must be in the range [1, 3]
+- Stride width must be greater than or equal to 1.  
+        For stride width greater than 3, valid padding needs to be used.
 - Kernel filter values for both width and height must be in the range [1, 8]
 - VALID padding: Kernel filter height must be in the range [1, 256]
 - VALID padding: Product of kernel filter width and height must be in the range [1, 65536]
 
 ### TFLite CONCATENATION Constraints
 
 This is a list of constraints that the CONCATENATION operator must satisfy in order to be scheduled on the NPU.
@@ -149,16 +151,20 @@
 - The size of the OFM axis must match the sum of all IFM axis defined by the axis attribute
 
 ### TFLite CONV_2D Constraints
 
 This is a list of constraints that the CONV_2D operator must satisfy in order to be scheduled on the NPU.
 
 - Stride values for both width and height must be integer types
+- IFM depth must be a whole multiple of the filter kernel depth
+- Number of filter kernels must be equally divisible by the number of convolution groups
 - Dilation factor values for both width and height must be integer types
-- Stride width must be greater than or equal to 1 and stride height must be between 1 and 3
+- Stride width must be greater than or equal to 1.  
+        For stride widths greater than 3, the post-optimization stride needs to be less than or equal to 3.  
+        Stride height must be between 1 and 3.
 - Dilated kernel height must be in the range [1, 64]
 - Product of dilated kernel width and height must be in the range [1, 4096]
 - Weight tensor must be 8-bit
 - Weight tensor must be constant
 - The sum of the weights cannot exceed 8323072
 - Optional Bias tensor must be of shape: 1D
 - Optional Bias tensor must be of type: int32, int64
@@ -243,18 +249,27 @@
 - Product of kernel filter width and height must be in the range [1, 65536]
 
 ### TFLite MEAN Constraints
 
 This is a list of constraints that the MEAN operator must satisfy in order to be scheduled on the NPU.
 
 - Input tensor must be at least 2D
-- Axis indices must correspond to height and width axes
-- Product of height and width must be no greater than 4096
-- For single axis averages across the height dimension:  
-        IFM height must be no greater than 64
+- Requirements for axis parameter:  
+        When IFM tensor is 2D:  
+          - Reduction in both axes is supported.  
+        When IFM tensor is 3D or 4D:  
+          - Reduction in Batch axis is only supported if batch size is 1.  
+          - Reduction in both Height and Width axes is supported.  
+          - Reduction in Depth axis is supported if at least one of H,W,C are of size 1.
+- Product of reduced axes must be no greater than:  
+        - 16777216 for signed 8-bit inputs.  
+        - 8388608 for unsigned 8-bit inputs.  
+        - 65536 for signed 16-bit inputs.
+- If Width axis is reduced its shape must be no greater than 4096.
+- If Depth axis is reduced its shape must be no greater than 4096.
 
 ### TFLite MINIMUM Constraints
 
 This is a list of constraints that the MINIMUM operator must satisfy in order to be scheduled on the NPU.
 
 - At least one Input's shape must match the OFM's shape
 - IFM and OFM data types must match
@@ -273,14 +288,15 @@
 
 ### TFLite PAD Constraints
 
 This is a list of constraints that the PAD operator must satisfy in order to be scheduled on the NPU.
 
 - Number of input tensors must be exactly 2
 - The padding tensor must be constant
+- Shape of output tensor must equal to size of input tensor plus padding
 - The padding tensor must have the shape [3,2] or [4,2]
 - The pad tensor can only pad width and height
 - Pad tensor must be of type: int32, int64
 
 ### TFLite RESHAPE Constraints
 
 This is a list of constraints that the RESHAPE operator must satisfy in order to be scheduled on the NPU.
@@ -312,14 +328,28 @@
         IFM W and H must both be 1  
         IFM must match OFM  
         W and H scaling must be equal and OFM W-1 and H-1 must be 2x/4x/8x IFM W-1 and H-1, if align_corners is True  
         W and H scaling must be equal and OFM W and H must be 2x/4x/8x IFM W and H, if align_corners is False
 - The size tensor must match the output tensor shape
 - Both align_corners and half_pixel_centers can't be True
 
+### TFLite RSQRT Constraints
+
+This is a list of constraints that the RSQRT operator must satisfy in order to be scheduled on the NPU.
+
+- At least one Input's shape must match the OFM's shape
+- IFM and OFM data types must match
+- IFM must be int8
+
+### TFLite SLICE Constraints
+
+This is a list of constraints that the SLICE operator must satisfy in order to be scheduled on the NPU.
+
+- Begin and Size Input tensors must be constant
+
 ### TFLite SOFTMAX Constraints
 
 This is a list of constraints that the SOFTMAX operator must satisfy in order to be scheduled on the NPU.
 
 - IFM and OFM shapes must match
 - IFM and OFM data types must match
 - Beta value needs to be positive
@@ -394,7 +424,8 @@
 - Must have 5 intermediate tensors
 - State tensors must be variable
 - Must not use CIFG
 - Must not use Peephole
 - Must not use Projection
 - Must not use Normalisation
 - All input and recurrent weights must be available
+- All recurrent weights must be 2D
```

### Comparing `ethos-u-vela-3.8.0/TESTING.md` & `ethos-u-vela-3.9.0/TESTING.md`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethos_u_vela.egg-info/PKG-INFO` & `ethos-u-vela-3.9.0/ethos_u_vela.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: ethos-u-vela
-Version: 3.8.0
+Version: 3.9.0
 Summary: Neural network model compiler for Arm Ethos-U NPUs
 Author-email: Arm Ltd <mlg-vela@arm.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://git.mlplatform.org/ml/ethos-u/ethos-u-vela.git/
 Keywords: ethos-u,vela compiler,tflite,npu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Compilers
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 <!--
 SPDX-FileCopyrightText: Copyright 2020-2023 Arm Limited and/or its affiliates <open-source-office@arm.com>
 
@@ -64,39 +64,57 @@
 compiled model.
 
 The tool has limited functionality for compiling a
 [TOSA](https://git.mlplatform.org/tosa/specification.git/) neural network
 (EXPERIMENTAL).
 
 ## TensorFlow Support
-* Vela 3.8.0 to current supports TensorFlow 2.11
+Vela is tested by comparing the numerical behaviour of the optimised operators
+against that of the corresponding TensorFlow Lite reference kernels.  The
+following list indicates which version is used for comparison:
+
+* Vela 3.9.0 to current supports TensorFlow 2.12
+* Vela 3.8.0 supports TensorFlow 2.11
 * Vela 3.6.0 to 3.7.0 supports TensorFlow 2.10
 * Vela 3.5.0 supports TensorFlow 2.9
 * Vela 3.4.0 supports TensorFlow 2.8
 * Vela 3.3.0 supports TensorFlow 2.7
 * Vela 3.1.0 to 3.2.0 supports TensorFlow 2.5
 * Vela 2.1.0 to 3.0.0 supports TensorFlow 2.4
 * Vela 2.0.0 to 2.0.1 supports TensorFlow 2.3
 * Vela 0.1.0 to 1.2.0 supports TensorFlow 2.1
 
+## Python Version Support
+The majority of Vela's testing is done using a single version of Python, as
+indicated by the first version in the list below.  However, some additional
+testing is also performed across a range of newer versions starting at the
+minimum version (pyproject.toml:project.requires-python) indicated in the
+brackets:
+
+* Vela 3.9.0 to current supports Python 3.10 (3.8)
+* Vela 3.8.0 supports Python 3.9 (3.8)
+* Vela 3.4.0 to 3.7.0 supports Python 3.7 (3.8)
+* Vela 3.3.0 supports Python 3.8 (3.7)
+* Vela 0.1.0 to 3.2.0 supports Python 3.6 (3.7)
+
 ## Environment
 
 Vela runs on Linux and Microsoft Windows 10 operating systems.
 
 ## Prerequisites
 
 The following should be installed prior to the installation of Vela:
 
-* Python 3.9 or compatible
+* Python 3.10 or compatible
    - Development version containing the Python/C API header files
-   - e.g. `apt install python3.9-dev` or `yum install python39-devel`
+   - e.g. `apt install python3.10-dev` or `yum install python310-devel`
 * Pip3
-* A C99 capable compiler and associated toolchain
+* C99 capable compiler and associated toolchain
     - For Linux operating systems, a GNU toolchain is recommended.
-    - For Microsoft Windows 10, Microsoft Visual C++ 14.2 Build Tools is recommended.
+    - For Microsoft Windows 10, the Microsoft Visual C++ 14.2 Build Tools are recommended.
       See <https://wiki.python.org/moin/WindowsCompilers>
 
 ## Installation
 
 Vela is available to install as a package from
 [PyPi](https://pypi.org/project/ethos-u-vela/), or as
 source code from
@@ -132,29 +150,29 @@
 #### Advanced Installation for Developers
 
 If you plan to modify the Vela codebase then it is recommended to install Vela
 as an editable package to avoid the need to re-install after every modification.
 This is done by adding the `-e` option to the install command like so:
 
 ```bash
-pip3 install -e .
+pip3 install -e .[dev]
 ```
 
 If you plan to contribute to the Vela project (highly encouraged!) then it is
 recommended to install Vela with the development dependencies (see
-[Vela Testing](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/TESTING.md) for more details).
+[Vela Testing](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.9.0/TESTING.md) for more details).
 
 ## Running
 
 Vela is run with an input `.tflite` or `.tosa` (EXPERIMENTAL) file passed on the
 command line. This file contains the neural network to be compiled. The tool then
 outputs an optimised `.tflite` file with a `_vela` suffix in the file name, along
 with performance estimate (EXPERIMENTAL) CSV files, all to the output directory.
 It also prints a performance estimation summary back to the console, see
-[Vela Performance Estimation Summary](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/PERFORMANCE.md).
+[Vela Performance Estimation Summary](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.9.0/PERFORMANCE.md).
 
 Example usage:
 
 1) Compile the network `my_model.tflite`.  The optimised version will be output
 to `./output/my_network_vela.tflite`.
 
 ```bash
@@ -241,15 +259,15 @@
 the mlw_codec and the current version of NumPy.
 
 **Example scenario:**
 
 In the ethos-u-vela source directory, run:
 
 ```bash
-virtualenv -p 3.9 venv
+virtualenv -p 3.10 venv
 . venv/bin/activate
 pip install ethos-u-vela
 ```
 
 Next, install a different NumPy version (e.g. 1.21.3)
 
 ```bash
@@ -287,66 +305,66 @@
    in mlw_codec during the build process.
    ```
    pip install ethos-u-vela --no-build-isolation --no-cache-dir
    ```
 
 ## APIs
 
-Please see [Vela External APIs](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/API.md).
+Please see [Vela External APIs](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.9.0/API.md).
 
 ## Bug Reporting
 
-Please see [Vela Community Bug Reporting](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/BUGS.md) for a description of how to
+Please see [Vela Community Bug Reporting](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.9.0/BUGS.md) for a description of how to
 report bugs.
 
 ## Contributions
 
-Please see [Vela Contributions](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/CONTRIBUTIONS.md).
+Please see [Vela Contributions](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.9.0/CONTRIBUTIONS.md).
 
 ## Debug Database
 
-Please see [Vela Debug Database](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/DEBUG_DB.md).
+Please see [Vela Debug Database](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.9.0/DEBUG_DB.md).
 
 ## Inclusive language commitment
 
 This product conforms to Arm’s inclusive language policy and, to the best of
 our knowledge, does not contain any non-inclusive language. If you find
 something that concerns you, email terms@arm.com.
 
 ## Options
 
-Please see [Vela CLI Options](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/OPTIONS.md).  This includes a description of the
+Please see [Vela CLI Options](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.9.0/OPTIONS.md).  This includes a description of the
 system configuration file format.
 
 ## Performance
 
-Please see [Vela Performance Estimation Summary](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/PERFORMANCE.md).
+Please see [Vela Performance Estimation Summary](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.9.0/PERFORMANCE.md).
 
 ## Releases
 
-Please see [Vela Releases](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/RELEASES.md).
+Please see [Vela Releases](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.9.0/RELEASES.md).
 
 ## Resources
 
 Additional useful information:
 
 * [Arm Products: Ethos-U55 NPU](https://www.arm.com/products/silicon-ip-cpu/ethos/ethos-u55)
 * [Arm Products: Ethos-U65 NPU](https://www.arm.com/products/silicon-ip-cpu/ethos/ethos-u65)
 * [Arm Developer: Ethos-U55 NPU](https://developer.arm.com/ip-products/processors/machine-learning/arm-ethos-u/ethos-u55)
 * [Arm Developer: Ethos-U65 NPU](https://developer.arm.com/ip-products/processors/machine-learning/arm-ethos-u/ethos-u65)
 
 ## Security
 
-Please see [Vela Security](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/SECURITY.md).
+Please see [Vela Security](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.9.0/SECURITY.md).
 
 ## Supported Operators
 
-Please see [Vela Supported Operators](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/SUPPORTED_OPS.md) for the list of
+Please see [Vela Supported Operators](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.9.0/SUPPORTED_OPS.md) for the list of
 operators supported in this release.
 
 ## Testing
 
-Please see [Vela Testing](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/TESTING.md).
+Please see [Vela Testing](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.9.0/TESTING.md).
 
 ## License
 
-Vela is licensed under [Apache License 2.0](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/LICENSE.txt).
+Vela is licensed under [Apache License 2.0](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.9.0/LICENSE.txt).
```

### Comparing `ethos-u-vela-3.8.0/ethos_u_vela.egg-info/SOURCES.txt` & `ethos-u-vela-3.9.0/ethos_u_vela.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/config_files/Arm/vela.ini` & `ethos-u-vela-3.9.0/ethosu/config_files/Arm/vela.ini`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/mlw_codec/makefile` & `ethos-u-vela-3.9.0/ethosu/mlw_codec/makefile`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/mlw_codec/mlw_codecmodule.c` & `ethos-u-vela-3.9.0/ethosu/mlw_codec/mlw_codecmodule.c`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/mlw_codec/mlw_common.h` & `ethos-u-vela-3.9.0/ethosu/mlw_codec/mlw_common.h`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/mlw_codec/mlw_decode.c` & `ethos-u-vela-3.9.0/ethosu/mlw_codec/mlw_decode.c`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/mlw_codec/mlw_decode.h` & `ethos-u-vela-3.9.0/ethosu/mlw_codec/mlw_decode.h`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/mlw_codec/mlw_encode.c` & `ethos-u-vela-3.9.0/ethosu/mlw_codec/mlw_encode.c`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/mlw_codec/mlw_encode.h` & `ethos-u-vela-3.9.0/ethosu/mlw_codec/mlw_encode.h`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/mlw_codec/mlw_main.c` & `ethos-u-vela-3.9.0/ethosu/mlw_codec/mlw_main.c`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/mlw_codec/test/test_mlw_codec.py` & `ethos-u-vela-3.9.0/ethosu/mlw_codec/test/test_mlw_codec.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/__init__.py` & `ethos-u-vela-3.9.0/ethosu/vela/__init__.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/__main__.py` & `ethos-u-vela-3.9.0/ethosu/vela/__main__.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/_version.py` & `ethos-u-vela-3.9.0/ethosu/vela/_version.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/api.py` & `ethos-u-vela-3.9.0/ethosu/vela/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright 2020-2022 Arm Limited and/or its affiliates <open-source-office@arm.com>
+# SPDX-FileCopyrightText: Copyright 2020-2023 Arm Limited and/or its affiliates <open-source-office@arm.com>
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 # Licensed under the Apache License, Version 2.0 (the License); you may
 # not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -23,15 +23,15 @@
 from typing import Optional
 from typing import Tuple
 
 import numpy
 
 
 API_VERSION_MAJOR = 1
-API_VERSION_MINOR = 3
+API_VERSION_MINOR = 4
 API_VERSION = f"{API_VERSION_MAJOR}.{API_VERSION_MINOR}"
 
 
 class NpuAccelerator(Enum):
     """
     Supported accelerators
     """
```

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/architecture_allocator.py` & `ethos-u-vela-3.9.0/ethosu/vela/architecture_allocator.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/architecture_features.py` & `ethos-u-vela-3.9.0/ethosu/vela/architecture_features.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/cascade_builder.py` & `ethos-u-vela-3.9.0/ethosu/vela/cascade_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,14 @@
 
         return (
             sched_op.op_type.npu_block_type not in non_cascadable_blocks
             and cost.stripe.height < sched_op.ofm.shape.height
             and sched_op.parent_op.read_offsets[0] is None
             and sched_op.parent_op.read_offsets[1] is None
             and self.elementwise_cascadable(sched_op)
-            and not sched_op.parent_op.type.is_resize_op()
             and not sched_op.parent_op.type == Op.Conv2DBackpropInputSwitchedBias
             and sched_op.parent_op.attrs.get("padding", None) != Padding.TILE
         )
 
     def _estimate_sram_usage(self, sched_op, cost) -> int:
         """Estimate the SRAM required for the Op if all FeatureMaps are in SRAM"""
         if sched_op.parent_op.type.is_binary_elementwise_op():
```

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/compiler_driver.py` & `ethos-u-vela-3.9.0/ethosu/vela/compiler_driver.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/data_type.py` & `ethos-u-vela-3.9.0/ethosu/vela/data_type.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/debug_database.py` & `ethos-u-vela-3.9.0/ethosu/vela/debug_database.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/driver_actions.py` & `ethos-u-vela-3.9.0/ethosu/vela/driver_actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright 2020-2022 Arm Limited and/or its affiliates <open-source-office@arm.com>
+# SPDX-FileCopyrightText: Copyright 2020-2023 Arm Limited and/or its affiliates <open-source-office@arm.com>
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 # Licensed under the Apache License, Version 2.0 (the License); you may
 # not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -75,15 +75,15 @@
     macs_cc = arch.ncores * arch.config.macs
     log2_macs_cc = int(np.log2(macs_cc) + 0.5)
     shram_size = arch.ncores * int(arch.shram_size_bytes / 1024)
     n = config_r()
     if arch.is_ethos_u65_system:
         n.set_product(1)
     else:
-        n.set_product(0)  # U55
+        n.set_product(0)  # Ethos-U55
     n.set_shram_size(shram_size)
     n.set_cmd_stream_version(0)  # may be incremented in the future
     n.set_macs_per_cc(log2_macs_cc)
     return n.word
 
 
 def emit_config(data: List[int], rel: int, patch: int, arch):
```

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/errors.py` & `ethos-u-vela-3.9.0/ethosu/vela/errors.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright 2020-2021 Arm Limited and/or its affiliates <open-source-office@arm.com>
+# SPDX-FileCopyrightText: Copyright 2020-2021, 2023 Arm Limited and/or its affiliates <open-source-office@arm.com>
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 # Licensed under the Apache License, Version 2.0 (the License); you may
 # not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -71,7 +71,21 @@
 
 
 class AllocationError(VelaError):
     """Raised when allocation fails"""
 
     def __init__(self, msg):
         super().__init__(f"Allocation failed: {msg}")
+
+
+class ByteAlignmentError(VelaError):
+    """Raised when value is unaligned"""
+
+    def __init__(self, msg):
+        super().__init__(f"Unaligned Value: {msg}")
+
+
+class ByteSizeError(VelaError):
+    """Raised when size has illegal value"""
+
+    def __init__(self, msg):
+        super().__init__(f"Illegal Size: {msg}")
```

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/ethos_u55_regs/ethos_u55_regs.py` & `ethos-u-vela-3.9.0/ethosu/vela/ethos_u55_regs/ethos_u55_regs.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/extract_npu_subgraphs.py` & `ethos-u-vela-3.9.0/ethosu/vela/extract_npu_subgraphs.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,25 +106,29 @@
             new_tens.consumer_list.append(op)
 
     # Deal with output tensors for the NPU graph. These are special.
     npu_subgraph.output_tensors = [new_tens if tens == orig_tens else tens for tens in npu_subgraph.output_tensors]
 
 
 def rewrite_tensor_npu_producer_cpu_consumers(
-    orig_tens, call_ps, startup_init_ps, npu_subgraph, cpu_subgraph, subgraph_for_pass
+    orig_tens, call_ps, npu_subgraph, cpu_subgraph, subgraph_for_pass, multiple_npu_sg_have_same_cpu_out_tens
 ):
+    if multiple_npu_sg_have_same_cpu_out_tens:
+        new_tens = orig_tens
+        orig_tens = orig_tens.src_tensor
+    else:
+        new_tens = orig_tens.clone("")
+        orig_tens.name = orig_tens.name + "_cpu"
+        new_tens.ops = []
 
-    new_tens = orig_tens.clone("")
-    orig_tens.name = orig_tens.name + "_cpu"
     npu_subgraph.output_tensors.append(orig_tens)
 
     call_ps.outputs.append(new_tens)
     call_ps.primary_op.outputs.append(new_tens)
-    new_tens.ops = [call_ps.primary_op]
-
+    new_tens.ops.append(call_ps.primary_op)
     # Elementwise op can not overwrite ifm if input is used by many consumers
     if orig_tens in npu_subgraph.input_tensors and len(orig_tens.consumers()) > 1:
         new_tens.ifm_write_protected = True
 
     # Elementwise op can not overwrite ifm if tensor is used as output from sub graph
     if orig_tens in npu_subgraph.output_tensors:
         new_tens.ifm_write_protected = True
@@ -231,24 +235,37 @@
                         tens, call_pass[curr_sg], startup_init_passes[curr_sg], curr_sg, orig_sg, subgraph_for_pass
                     )
 
             for tens in ps.outputs:
 
                 dest_sgs = [subgraph_for_pass[op.scheduled_pass] for op in tens.consumers() if op is not None]
                 need_rewrite = False
+                multiple_npu_sg_have_same_cpu_out_tens = False
+                output_tensor = tens
                 for sg in dest_sgs:
                     if sg != curr_sg:
                         need_rewrite = True
                         break
-                if tens in orig_sg.output_tensors:
-                    need_rewrite = True
+                for orig_out_tens in orig_sg.output_tensors:
+                    if tens not in curr_sg.output_tensors:
+                        if tens == orig_out_tens:
+                            need_rewrite = True
+                        elif tens.equivalence_id == orig_out_tens.equivalence_id:
+                            need_rewrite = True
+                            multiple_npu_sg_have_same_cpu_out_tens = True
+                            output_tensor = orig_out_tens
 
                 if need_rewrite:
                     rewrite_tensor_npu_producer_cpu_consumers(
-                        tens, call_pass[curr_sg], startup_init_passes[curr_sg], curr_sg, orig_sg, subgraph_for_pass
+                        output_tensor,
+                        call_pass[curr_sg],
+                        curr_sg,
+                        orig_sg,
+                        subgraph_for_pass,
+                        multiple_npu_sg_have_same_cpu_out_tens,
                     )
 
         for tens in curr_sg.output_tensors:
             # ofm can depend on multiple ops. These ops can be divided into different NPU
             # nodes due to CPU nodes. If that is the case the ofm must be NHWC.
             tens.force_linear_format = True
```

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/fp_math.py` & `ethos-u-vela-3.9.0/ethosu/vela/fp_math.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/graph_optimiser.py` & `ethos-u-vela-3.9.0/ethosu/vela/graph_optimiser.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/graph_optimiser_util.py` & `ethos-u-vela-3.9.0/ethosu/vela/graph_optimiser_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 from .architecture_features import Accelerator
 from .data_type import DataType
 from .debug_database import DebugDatabase
 from .errors import UnsupportedFeatureError
 from .errors import VelaError
 from .operation import Op
+from .operation import Operation
 from .operation_util import create_avgpool_nop
 from .shape4d import Shape4D
 from .tensor import Tensor
 
 memory_only_ops = (
     Op.Reshape,
     Op.QuantizedReshape,
@@ -181,22 +182,23 @@
     output_pad_after = pad_after
     while output_pad_after > 0 and output_pad_after % stride != total_minus_before % stride:
         output_pad_after -= 1
     return pad_before, output_pad_after
 
 
 def needed_total_padding(input_size, stride, filter_size):
-    out_size = (input_size + stride - 1) // stride
-    needed_input = (out_size - 1) * stride + filter_size
-    total_padding = max(0, needed_input - input_size)
-    return total_padding
+    """Compute hardware padding."""
+    if input_size % stride == 0:
+        return max(filter_size - stride, 0)
 
+    return max(filter_size - (input_size % stride), 0)
 
-# Set input/output tensor equivalence to the same id for memory operations
-def set_tensor_equivalence(op, arch, nng):
+
+def set_tensor_equivalence(op: Operation, arch, nng) -> Operation:
+    """Set input/output tensor equivalence to the same id for memory operations."""
     if op.type in memory_only_ops:
         eid = op.outputs[0].equivalence_id
         for inp in op.inputs:
             inp.equivalence_id = eid
     return op
 
 
@@ -295,37 +297,37 @@
         for prev_op in ifm.ops:
             prev_op.outputs = [ofm]
             ofm.ops.append(prev_op)
 
     return op
 
 
-def convert_depthwise_to_conv(op, arch, nng):
-    # Depthwise is equivalent to a single conv2d if the ifm depth is 1 and
-    # the ofm depth equals the depth multipler.
-    # If those conditions are true, then we can perform a simple
-    # switch of the operator type (and weight order)
-
+def convert_depthwise_to_conv(op: Operation, arch, nng) -> Operation:
+    """Convert DepthwiseConv2DBias to Conv2D to allow support for DepthwiseConv2DBias ops with 'depth multiplier' > 1,
+    as long as IFM depth = 1 and OFM depth is equal to the depth multiplier.
+    """
     if op.type == Op.DepthwiseConv2DBias and (op.attrs["depth_multiplier"] != 1):
         ifm_shape = op.ifm_shapes[0]
         weight_tensor = op.inputs[1]
         ofm_shape = op.ofm_shapes[0]
+        # Depthwise is equivalent to a single conv2d if the ifm depth is 1 and
+        # the ofm depth equals the depth multipler.
         if (ifm_shape.depth == 1) and (ofm_shape.depth == op.attrs["depth_multiplier"]):
             # Change op type to Conv2d
             op.type = Op.Conv2DBias
             del op.attrs["channel_multiplier"]
             del op.attrs["depth_multiplier"]
 
             weight_tensor.values = np.transpose(weight_tensor.values, (0, 1, 3, 2))
             weight_tensor.set_all_shapes(list(weight_tensor.values.shape))
             DebugDatabase.add_optimised(op, op)
         else:
             raise UnsupportedFeatureError(
-                f"Unsupported 'DEPTHWISE_CONV_2D' with depth_multiplier = {op.attrs['depth_multiplier']},",
-                f" ifm channels = {ifm_shape.depth}, ofm channels = {ofm_shape.depth}",
+                f"Unsupported 'DEPTHWISE_CONV_2D' with depth_multiplier = {op.attrs['depth_multiplier']},"
+                f" ifm channels = {ifm_shape.depth}, ofm channels = {ofm_shape.depth}"
             )
     return op
 
 
 def create_avg_pool_for_concat(concat_op, name, ifm, ifm_shape: Shape4D, write_offset: Shape4D):
     """Creates an average pool for the given concat op/input feature map"""
     ofm = concat_op.ofm
```

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/greedy_allocation.py` & `ethos-u-vela-3.9.0/ethosu/vela/greedy_allocation.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/high_level_command_stream.py` & `ethos-u-vela-3.9.0/ethosu/vela/high_level_command_stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,15 +232,15 @@
         for i in range(len(self.ofm_box.end_coord)):
             assert self.ofm_box.end_coord[i] <= ps.ofm_shapes[0][i]
 
     def is_npu_pass_command(self):
         return True
 
     def __str__(self):
-        return "<NPUStripe: ps=%s, ifm_box=%s, ifm2_box=%s, ofm_box=%s, weight_box=%s, block_config=%s>" % (
+        return "<NpuStripe: name=%s, ifm_box=%s, ifm2_box=%s, ofm_box=%s, weight_box=%s, block_config=%s>" % (
             self.ps.name,
             self.ifm_box,
             self.ifm2_box,
             self.ofm_box,
             self.weight_box,
             self.block_config,
         )
@@ -282,15 +282,15 @@
     def __init__(self, ps, in_tensor, out_tensor, box):
         self.ps = ps
         self.in_tensor = in_tensor
         self.out_tensor = out_tensor
         self.box = box
 
     def __str__(self):
-        return "<DMA: in=%s, out=%s, box=%s>" % (self.in_tensor.name, self.out_tensor.name, self.box)
+        return f"<DMA: name={self.ps.name}, in={self.in_tensor.name}, out={self.out_tensor.name} box={self.box}>"
 
     __repr__ = __str__
 
     def get_operation_count(self):
         # returns numpy array of (DPU blocks, dma_ops)
         return np.array((0, 1))
 
@@ -298,14 +298,14 @@
 class NOP(Command):
     def __init__(self, ps, in_tensor, out_tensor):
         self.ps = ps
         self.in_tensor = in_tensor
         self.out_tensor = out_tensor
 
     def __str__(self):
-        return f"<NOP: in={self.in_tensor.name}, out={self.out_tensor.name}>"
+        return f"<NOP: name={self.ps.name}, in={self.in_tensor.name}, out={self.out_tensor.name}>"
 
     __repr__ = __str__
 
     def get_operation_count(self):
         # returns numpy array of (DPU blocks, dma_ops)
         return np.array((0, 0))
```

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/high_level_command_stream_generator.py` & `ethos-u-vela-3.9.0/ethosu/vela/high_level_command_stream_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # distributed under the License is distributed on an AS IS BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # Description:
 # Generate a high-level command stream from a schedule
+from .architecture_allocator import is_nearest
 from .high_level_command_stream import Box
 from .high_level_command_stream import DMA
 from .high_level_command_stream import NOP
 from .high_level_command_stream import NpuStripe
 from .numeric_util import round_up_divide
 from .operation import create_activation_function
 from .operation import NpuBlockType
@@ -98,15 +99,15 @@
     # Get Kernel strides and upscaling factor
     kernel_stride = sched_op.kernel.stride
     strides = [1, kernel_stride.y, kernel_stride.x, 1]
     skirt = parent_op.attrs.get("skirt", None)
     upscaling = 1
     if sched_op.op_type == Op.Conv2DBackpropInputSwitchedBias:
         upscaling = ofm_shape.height // ifm.shape.height
-    elif sched_op.op_type.is_resize_op():
+    elif is_nearest(sched_op.resampling_mode):
         upscaling = round_up_divide(ofm_shape.height, ifm.shape.height)
 
     # Get kernel height and height dilation
     k_height = 1
     if npu_block_type in (NpuBlockType.Pooling, NpuBlockType.ReduceSum):
         if parent_op is not None:
             k_height = parent_op.attrs["ksize"][1]
```

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/high_level_command_to_npu_op.py` & `ethos-u-vela-3.9.0/ethosu/vela/high_level_command_to_npu_op.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,14 +304,22 @@
 
 
 def use_zero_point_0(ps, tens: Tensor, is_ifm_tensor: bool) -> bool:
     """Checks if quantization should use 0 as zero point"""
     if tens.dtype == DataType.int32 and is_ifm_tensor:
         return True
     if ps.primary_op.rounding_mode == RoundingMode.AwayZero:
+        if (
+            ps.primary_op.original_type == Op.AvgPool
+            and ps.primary_op.type == Op.Conv2DBias
+            and ps.primary_op.attrs.get("padding", None) == Padding.VALID
+        ):
+            # Force zero point to 0 for AveragePool operators converted to a Conv2DBias with rounding away from
+            # zero.
+            return True
         if ps.primary_op.original_type == Op.ResizeBilinear and ps.primary_op.type == Op.DepthwiseConv2DBias:
             # Force zero point to 0 for ResizeBilinear operators converted to a DepthwiseConv with rounding away from
             # zero. This is because the reference kernel ignores the zero points.
             return True
         if (
             not is_ifm_tensor
             and ps.primary_op.original_type == Op.AvgPool
```

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/hillclimb_allocation.py` & `ethos-u-vela-3.9.0/ethosu/vela/hillclimb_allocation.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/live_range.py` & `ethos-u-vela-3.9.0/ethosu/vela/live_range.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,16 +204,19 @@
         # Check if possible to merge ifm/ofm live ranges of dma op
         dma_op = sched_op.parent_op
         ifm = dma_op.ifm
         ofm = dma_op.ofm
         if not (
             tensor_should_be_ignored(ifm, target_mem_area, target_mem_type_set)
             or tensor_should_be_ignored(ofm, target_mem_area, target_mem_type_set)
+            # input tensor only allowed to have one consumer
+            or len(ifm.consumer_list) > 1
         ):
             # Currently DMA only used when bypassing memory only ops so ok to reuse ifm
+            # if ifm has only one consumer
             ifm_tens = ifm
 
     return ifm_tens
 
 
 def ofm_can_reuse_ifm(sched_op, target_mem_area=None, target_mem_type_set=None):
     ifm = _get_ifm_to_fuse(sched_op, target_mem_area, target_mem_type_set)
```

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/lstm.py` & `ethos-u-vela-3.9.0/ethosu/vela/lstm.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/mark_tensors.py` & `ethos-u-vela-3.9.0/ethosu/vela/mark_tensors.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/model_reader.py` & `ethos-u-vela-3.9.0/ethosu/vela/model_reader.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/nn_graph.py` & `ethos-u-vela-3.9.0/ethosu/vela/nn_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -334,49 +334,29 @@
                 visit_op(op)
 
         for tens in self.output_tensors:
             visit_tensor(tens)
 
         return all_ops
 
-    def print_operators(self):
-        print("print_operators()", self.name)
-        all_ops = self.get_all_ops()
-        unique_ops = []
-        for op in all_ops:
-            if op.type in (Op.Const, Op.Identity, Op.Placeholder):
-                continue
-
-            attrs = op.attrs.copy()
-            if op.type in (Op.Conv2D, Op.Conv2DBias, Op.DepthwiseConv2DBias):
-                kshape = op.inputs[1].shape
-                attrs["kshape"] = [kshape[0], kshape[1]]
-            attrs["type"] = op.type.name
-            attrs.pop("use_cudnn_on_gpu", None)
-            custom_options = attrs.pop("custom_options", None)
-            if attrs not in unique_ops:
-                unique_ops.append(attrs)
-                # print attributes in human readable format
-                a = attrs.copy()
-                if custom_options is not None:
-                    a["custom_options"] = custom_options
-                s = a.pop("type")
-                data_format = a.pop("data_format", None)
-                if data_format and data_format != b"NHWC":
-                    s += " " + str(data_format)
-                t = a.pop("T", None)
-                if t:
-                    s += " " + str(t)[9:-2]
-                srct = a.pop("SrcT", None)
-                if srct:
-                    s += " " + str(srct)[9:-2]
-                dstt = a.pop("DstT", None)
-                if dstt:
-                    s += "->" + str(dstt)[9:-2]
-                print(s + " " + str(a))
+    def print_operators(self, ignore_placeholder_const=True, show_attributes=True):
+        print(f"Operators of Subgraph {self.name}")
+
+        ignore_ops = (Op.Const, Op.Identity, Op.Placeholder) if ignore_placeholder_const else ()
+        all_ops = [op for op in self.get_all_ops() if op.type not in ignore_ops]
+
+        if len(all_ops) > 0:
+            max_op_type_len = max([len(op.type.name) for op in all_ops])
+
+            for idx, op in enumerate(all_ops):
+                attrs_str = f" - {op.attrs}" if show_attributes else ""
+                print(f"{idx:3}: {op.type:{max_op_type_len}}{attrs_str} - {op.name}")
+
+        else:
+            print("No Operators")
 
     def print_graph(self, label=None):
         if label:
             print(f"\n[ {label} ]")
         print("print_graph()", self.name)
         all_ops = self.get_all_ops()
         for idx, op in enumerate(all_ops):
@@ -558,17 +538,17 @@
         for sg in self.subgraphs:
             sg.update_consumers()
 
     def refresh_after_modification(self):
         for sg in self.subgraphs:
             sg.refresh_after_modification()
 
-    def print_operators(self):
+    def print_operators(self, ignore_placeholder_const=True, show_attributes=True):
         for sg in self.subgraphs:
-            sg.print_operators()
+            sg.print_operators(ignore_placeholder_const, show_attributes)
 
     def print_graph(self, label=None):
         for sg in self.subgraphs:
             sg.print_graph(label)
 
     def print_graph_with_tensors(self):
         for sg in self.subgraphs:
```

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/npu_performance.py` & `ethos-u-vela-3.9.0/ethosu/vela/npu_performance.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,27 +100,27 @@
             PassCycles.Total,
         )
 
 
 class PerformanceQuery:
     def __init__(self, npu_block_type=0):
         self.npu_block_type = npu_block_type
-        self.ifm_shape = Shape4D(0)
+        self.ifm_shape = Shape4D(0, 0, 0, 0)
         self.ifm_format = TensorFormat.NHWC
         self.ifm_memory_area = MemArea.Unknown
         self.ifm2_memory_area = MemArea.Unknown
         self.ifm_bits = 0
         self.ifm2_bits = 0
         self.ifm2_shape = None
         self.ifm2_format = TensorFormat.NHWC
-        self.ofm_shape = Shape4D(0)
+        self.ofm_shape = Shape4D(0, 0, 0, 0)
         self.ofm_format = TensorFormat.NHWC
         self.ofm_memory_area = MemArea.Unknown
         self.ofm_bits = 0
-        self.const_shape = Shape4D(0)
+        self.const_shape = Shape4D(0, 0, 0, 0)
         self.const_memory_area = MemArea.Unknown
         self.kernel = Kernel(1, 1)
         self.config = ArchitectureBlockConfig()
 
 
 class CycleCost:
     def __init__(self):
@@ -190,15 +190,15 @@
         strides[1] = (element_bits * shape.width * shape.depth) / 8  # +Y
         strides[0] = (element_bits * shape.width * shape.depth) / 8  # +N
 
     return strides
 
 
 def _estimate_memory_transfer_efficiency(
-    arch, is_read, mem_area, format: TensorFormat, element_bits, block_size, shape4D, to_transfer
+    arch, is_read, mem_area, format, element_bits, block_size, shape4D, to_transfer
 ):
     burst_len = 8
 
     strides = _strides_for_shape(shape4D, format, element_bits)
 
     if format == TensorFormat.NHCWB16:
         if strides[2] == block_size.depth:  # TODO is this check corrrect for non 8-bit
@@ -614,24 +614,24 @@
 ):
     cycles_a = make_cycles_array()
     bws = make_bandwidth_array()
     scaled_bws = make_bandwidth_array()  # scaled bw with memory transfer efficiency
     macs = 0
 
     query = PerformanceQuery(op.op_type.npu_block_type)
-    query.ifm_shape = op.ifm.shape
+    query.ifm_shape = op.ifm_read_shape
     query.ifm_format = op.ifm.format
-    query.ifm_memory_area = op.ifm.mem_area
+    query.ifm_memory_area = op.ifm.connection.parent_tens.mem_area  # Mem Area is set directly on parent_tens
     query.ifm_bits = op.ifm.dtype.size_in_bits()
-    query.ifm2_shape = op.ifm2 and op.ifm2.shape
+    query.ifm2_shape = op.ifm2_read_shape
     query.ifm2_format = op.ifm2 and op.ifm2.format
-    query.ifm2_memory_area = op.ifm2 and op.ifm2.mem_area
+    query.ifm2_memory_area = op.ifm2 and op.ifm2.connection.parent_tens.mem_area
     query.ifm2_bits = op.ifm2 and op.ifm2.dtype.size_in_bits()
-    query.ofm_shape = op.ofm.shape
-    query.ofm_memory_area = op.ofm.mem_area
+    query.ofm_shape = op.ofm_write_shape
+    query.ofm_memory_area = op.ofm.connection.parent_tens.mem_area
     query.ofm_bits = op.ofm.dtype.size_in_bits()
     query.ofm_format = op.ofm.format
     query.kernel = op.kernel
     query.config = block_config
 
     cost = schedule.cost_map[op]
     prev_cost = schedule.cost_map[prev_op] if prev_op else None
@@ -711,39 +711,46 @@
         # Add cycles for LUT + mempcy op Transfer
         cycles_a[PassCycles.Npu] += dma_transfer_cycles
     else:
         # Add cycles for LUT + mempcy op Transfer
         cycles_a[PassCycles.Npu] += max(dma_transfer_cycles - slack_cycles, 0)
 
     # OFM write
-    ofm = op.parent_op.ofm
+    ofm = op.ofm.connection.parent_tens
     bw = access.ofm_write * ofm.element_size()
     bws[query.ofm_memory_area][ofm.purpose][BandwidthDirection.Write] += bw
-    scaled_bws[ofm.mem_area][ofm.purpose][BandwidthDirection.Write] += _estimate_memory_transfer_efficiency(
-        arch, False, query.ofm_memory_area, ofm.format, query.ofm_bits, query.config.ofm_block, query.ofm_shape, bw
+    scaled_bws[query.ofm_memory_area][ofm.purpose][BandwidthDirection.Write] += _estimate_memory_transfer_efficiency(
+        arch,
+        False,
+        query.ofm_memory_area,
+        query.ofm_format,
+        query.ofm_bits,
+        query.config.ofm_block,
+        query.ofm_shape,
+        bw,
     )
 
     # IFM read
-    ifm = op.parent_op.ifm2 if op.reversed_operands else op.parent_op.ifm
+    ifm = op.ifm.connection.parent_tens
     bw = access.ifm_read[0] * ifm.element_size()
-    bws[ifm.mem_area][ifm.purpose][BandwidthDirection.Read] += bw
-    scaled_bws[ifm.mem_area][ifm.purpose][BandwidthDirection.Read] += _estimate_memory_transfer_efficiency(
-        arch, True, query.ifm_memory_area, ifm.format, query.ifm_bits, query.config.ifm_block, query.ifm_shape, bw
+    bws[query.ifm_memory_area][ifm.purpose][BandwidthDirection.Read] += bw
+    scaled_bws[query.ifm_memory_area][ifm.purpose][BandwidthDirection.Read] += _estimate_memory_transfer_efficiency(
+        arch, True, query.ifm_memory_area, query.ifm_format, query.ifm_bits, query.config.ifm_block, query.ifm_shape, bw
     )
 
     if query.ifm2_shape:
-        ifm2 = op.parent_op.ifm if op.reversed_operands else op.parent_op.ifm2
+        ifm2 = op.ifm2.connection.parent_tens
         bw = access.ifm_read[1] * ifm2.element_size()
         bws[ifm2.mem_area][ifm2.purpose][BandwidthDirection.Read] += bw
         scaled_bws[ifm2.mem_area][ifm2.purpose][BandwidthDirection.Read] += _estimate_memory_transfer_efficiency(
             arch,
             True,
             query.ifm2_memory_area,
-            ifm2.format,
-            op.ifm2.dtype.size_in_bits(),
+            query.ifm2_format,
+            query.ifm2_bits,
             query.config.ifm_block,
             query.ifm2_shape,
             bw,
         )
 
     # Weight read
     if access.const_read[0] > 0:
```

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/npu_serialisation.py` & `ethos-u-vela-3.9.0/ethosu/vela/npu_serialisation.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/numeric_util.py` & `ethos-u-vela-3.9.0/ethosu/vela/numeric_util.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/operation.py` & `ethos-u-vela-3.9.0/ethosu/vela/operation.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,16 +144,16 @@
     Any = OperatorInfo()
     ArgMax = OperatorInfo(indices=NNG_IFM_INDICES)
     ArgMin = OperatorInfo()
     AvgPool = OperatorInfo(block_type=NpuBlockType.Pooling, indices=NNG_IFM_INDICES)
     Atan2 = OperatorInfo(indices=NNG_IFM_IFM2_INDICES)
     BatchMatMul = OperatorInfo()
     BatchToSpaceND = OperatorInfo()
-    BidirectionalSequenceLstm = OperatorInfo(block_type=NpuBlockType.VectorProduct, indices=NNG_IFM_WEIGHTS_INDICES)
-    BidirectionalSequenceRnn = OperatorInfo(block_type=NpuBlockType.VectorProduct, indices=NNG_IFM_WEIGHTS_INDICES)
+    BidirectionalSequenceLstm = OperatorInfo(indices=NNG_IFM_WEIGHTS_INDICES)
+    BidirectionalSequenceRnn = OperatorInfo(indices=NNG_IFM_WEIGHTS_INDICES)
     CLZ = OperatorInfo(
         block_type=NpuBlockType.ElementWise, indices=NNG_IFM_INDICES, is_unary=True
     )  # NPU specific operation
     Call = OperatorInfo()
     Cast = OperatorInfo()
     Ceil = OperatorInfo()
     Clamp = OperatorInfo(indices=NNG_IFM_INDICES)  # TOSA specific
@@ -210,17 +210,17 @@
     Less = OperatorInfo()
     LessEqual = OperatorInfo()
     Log = OperatorInfo()
     LogSoftmax = OperatorInfo()
     LogicalAnd = OperatorInfo()
     LogicalNot = OperatorInfo()
     LogicalOr = OperatorInfo()
-    Lstm = OperatorInfo(block_type=NpuBlockType.VectorProduct, indices=NNG_IFM_WEIGHTS_INDICES)
+    Lstm = OperatorInfo(indices=NNG_IFM_WEIGHTS_INDICES)
     LUT = OperatorInfo()  # NPU specific, operator has LUT, only used in fused activation functions
-    MatMul = OperatorInfo(block_type=NpuBlockType.VectorProduct, indices=NNG_IFM_WEIGHTS_INDICES)
+    MatMul = OperatorInfo(indices=NNG_IFM_WEIGHTS_INDICES)
     MatrixDiag = OperatorInfo()
     MatrixSetDiag = OperatorInfo()
     Max = OperatorInfo()
     MaxPool = OperatorInfo(block_type=NpuBlockType.Pooling, indices=NNG_IFM_INDICES)
     Maximum = OperatorInfo(block_type=NpuBlockType.ElementWise, indices=NNG_IFM_IFM2_INDICES)
     Mean = OperatorInfo(indices=NNG_IFM_INDICES)
     Min = OperatorInfo()
@@ -257,17 +257,17 @@
     Rescale = OperatorInfo(indices=NNG_IFM_INDICES)  # TOSA specific
     Reshape = OperatorInfo(indices=NNG_IFM_INDICES)
     # resize ops map to pooling operations unless explicitly converted to other operations in the graph optimiser
     ResizeBilinear = OperatorInfo(block_type=NpuBlockType.Pooling, indices=NNG_IFM_INDICES)
     ResizeNearestNeighbor = OperatorInfo(block_type=NpuBlockType.Pooling, indices=NNG_IFM_INDICES)
     ReverseSequence = OperatorInfo()
     ReverseV2 = OperatorInfo()
-    Rnn = OperatorInfo(block_type=NpuBlockType.VectorProduct, indices=NNG_IFM_WEIGHTS_INDICES)
+    Rnn = OperatorInfo(indices=NNG_IFM_WEIGHTS_INDICES)
     Round = OperatorInfo()
-    Rsqrt = OperatorInfo()
+    Rsqrt = OperatorInfo(block_type=NpuBlockType.ElementWise, indices=NNG_IFM_INDICES, is_unary=True)
     SHL = OperatorInfo(block_type=NpuBlockType.ElementWise, indices=NNG_IFM_IFM2_INDICES)  # NPU specific operation
     SHR = OperatorInfo(block_type=NpuBlockType.ElementWise, indices=NNG_IFM_IFM2_INDICES)  # NPU specific operation
     ScatterNd = OperatorInfo()
     SegmentSum = OperatorInfo()
     Select = OperatorInfo()
     SelectV2 = OperatorInfo()
     Shape = OperatorInfo(indices=NNG_IFM_INDICES)
@@ -294,16 +294,16 @@
     Sum = OperatorInfo()
     Svdf = OperatorInfo()
     Table = OperatorInfo(indices=NNG_IFM_INDICES)
     Tanh = OperatorInfo(indices=NNG_IFM_INDICES)
     Tile = OperatorInfo()
     TopKV2 = OperatorInfo()
     Transpose = OperatorInfo(indices=NNG_IFM_IFM2_INDICES)
-    UnidirectionalSequenceLstm = OperatorInfo(block_type=NpuBlockType.VectorProduct, indices=NNG_IFM_WEIGHTS_INDICES)
-    UnidirectionalSequenceRnn = OperatorInfo(block_type=NpuBlockType.VectorProduct, indices=NNG_IFM_WEIGHTS_INDICES)
+    UnidirectionalSequenceLstm = OperatorInfo(indices=NNG_IFM_WEIGHTS_INDICES)
+    UnidirectionalSequenceRnn = OperatorInfo(indices=NNG_IFM_WEIGHTS_INDICES)
     Unique = OperatorInfo()
     Unpack = OperatorInfo(indices=NNG_IFM_INDICES)
     UnpackReshaped = OperatorInfo(indices=NNG_IFM_INDICES)
     VariableTensorWrite = OperatorInfo()
     Where = OperatorInfo()
     While = OperatorInfo()
     ZerosLike = OperatorInfo()
@@ -611,15 +611,15 @@
             # is done by slightly adjusting the scale and shift on the ofm tensor using the scale and bias tensor,
             # it has no affect on global scaling (i.e. the ofm_scale register). In addition, the zero points of the
             # input and/or output tensors may also require forcing to zero but the exact behaviour also depends upon the
             # corresponding optimisation performed in graph_optimisation.py where the rounding mode is set
             is_supported = False
             if self.original_type == Op.ResizeBilinear and self.type == Op.DepthwiseConv2DBias:
                 is_supported = True
-            if self.original_type == Op.AvgPool and self.type == Op.DepthwiseConv2DBias:
+            if self.original_type == Op.AvgPool and self.type in (Op.DepthwiseConv2DBias, Op.Conv2DBias):
                 is_supported = True
 
         if is_supported:
             self._rounding_mode = mode
         else:
             assert (
                 False
@@ -848,14 +848,19 @@
             tens.consumer_list.append(self)
 
     def get_input_quantization(self):
         if self.forced_input_quantization is not None:
             return self.forced_input_quantization
         return self.ifm.quantization
 
+    def add_output_tensor(self, tens):
+        self.outputs.append(tens)
+        if self not in tens.ops:
+            tens.ops.append(self)
+
     def set_output_tensor(self, tens):
         tens.ops = [self]
         self.outputs = [tens]
 
     def get_output_quantization(self):
         if self.forced_output_quantization is not None:
             return self.forced_output_quantization
```

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/operation_util.py` & `ethos-u-vela-3.9.0/ethosu/vela/operation_util.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/pass_packing.py` & `ethos-u-vela-3.9.0/ethosu/vela/pass_packing.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,15 +267,15 @@
                                 assert len(curr_op.inputs) >= 1
                                 ifm_tensor = curr_op.ifm
                                 ifm_shapes = curr_op.ifm_shapes.copy()
                                 assert ifm_tensor is not None, "IFM missing in {}".format(curr_op)
                                 assert ifm_tensor.purpose == TensorPurpose.FeatureMap
 
                         if operation_set is None:
-                            print("Warning:", curr_op.type, "operation is unknown or unsupported, placing on CPU")
+                            assert not curr_op.run_on_npu  # operator should have been placed on the CPU
 
                         for inp in reversed(curr_op.inputs):
                             if inp is None:
                                 continue
                             if can_pack(inp, curr_op):
                                 to_process.append((inp.ops[0], inp))
                             else:
```

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/range_set.py` & `ethos-u-vela-3.9.0/ethosu/vela/range_set.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/rawdata_writer.py` & `ethos-u-vela-3.9.0/ethosu/vela/rawdata_writer.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/reader_util.py` & `ethos-u-vela-3.9.0/ethosu/vela/reader_util.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/register_command_stream_generator.py` & `ethos-u-vela-3.9.0/ethosu/vela/register_command_stream_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright 2020-2022 Arm Limited and/or its affiliates <open-source-office@arm.com>
+# SPDX-FileCopyrightText: Copyright 2020-2023 Arm Limited and/or its affiliates <open-source-office@arm.com>
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 # Licensed under the Apache License, Version 2.0 (the License); you may
 # not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -56,14 +56,16 @@
 from .api import NpuTileBox
 from .architecture_allocator import ArchitectureBlockConfig
 from .architecture_allocator import try_block_config
 from .architecture_features import Accelerator
 from .architecture_features import ArchitectureFeatures
 from .architecture_features import create_default_arch
 from .architecture_features import SHRAMElements
+from .errors import ByteAlignmentError
+from .errors import ByteSizeError
 from .errors import VelaError
 from .ethos_u55_regs.ethos_u55_regs import acc_format
 from .ethos_u55_regs.ethos_u55_regs import activation
 from .ethos_u55_regs.ethos_u55_regs import cmd0
 from .ethos_u55_regs.ethos_u55_regs import cmd1
 from .ethos_u55_regs.ethos_u55_regs import elementwise_mode
 from .ethos_u55_regs.ethos_u55_regs import pooling_mode
@@ -72,14 +74,19 @@
 from .numeric_util import round_away_zero
 from .numeric_util import round_up_to_int
 from .operation import ExplicitScaling
 from .operation import NpuBlockType
 from .range_set import MemoryAccessSet
 from .register_command_stream_util import BASE_PTR_INDEX_MEM2MEM
 from .register_command_stream_util import calc_blockdep
+from .register_command_stream_util import check_addresses
+from .register_command_stream_util import check_alignment
+from .register_command_stream_util import check_dma_op
+from .register_command_stream_util import check_size
+from .register_command_stream_util import check_strides
 from .register_command_stream_util import get_dma_memory_accesses
 from .register_command_stream_util import get_op_memory_accesses
 from .register_command_stream_util import get_strides
 from .register_command_stream_util import get_wait_dependency
 from .register_command_stream_util import get_zero_point
 from .register_command_stream_util import has_ifm2
 from .register_command_stream_util import quantise
@@ -331,19 +338,24 @@
     else:
         activation_value = cast(int, activation_op_map[act.op_type])
     emit.cmd0_with_param(cmd0.NPU_SET_ACTIVATION, activation_value)
     emit.cmd0_with_param(cmd0.NPU_SET_ACTIVATION_MIN, quantized_min)
     emit.cmd0_with_param(cmd0.NPU_SET_ACTIVATION_MAX, quantized_max)
 
 
-def generate_addresses(emit: CommandStreamEmitter, ptr_cmds: List[cmd1], addresses: List[int], layout: NpuLayout):
+def generate_addresses(
+    emit: CommandStreamEmitter,
+    ptr_cmds: List[cmd1],
+    addresses: List[int],
+    layout: NpuLayout,
+    element_size,
+    arch: ArchitectureFeatures,
+):
     """Generates xFM_BASE registers"""
-    if layout == NpuLayout.NHCWB16:
-        # Check that all BasePointer addresses are aligned to 16 bytes
-        assert all((int(addr) % 16) == 0 for addr in addresses)
+    check_addresses(addresses, layout, element_size, arch)
     for i in range(4):
         emit.cmd1_with_address(ptr_cmds[i], addresses[i])
 
 
 def generate_tiles(emit: CommandStreamEmitter, tile_cmds: List[cmd0], tiles: NpuTileBox):
     """Generates xFM_HEIGHT0/HEIGHT1/WIDTH0 registers"""
     emit.cmd0_with_param(tile_cmds[0], tiles.height_0 - 1)
@@ -352,14 +364,16 @@
 
 
 def generate_strides(
     emit: CommandStreamEmitter, fm: NpuFeatureMap, stride_c_cmd: cmd1, stride_y_cmd: cmd1, stride_x_cmd: cmd1
 ):
     """Generates STRIDE_C/Y/X registers"""
     strides = get_strides(fm)
+    check_strides(fm, strides)
+
     emit.cmd1_with_address(stride_c_cmd, strides.depth)  # stride between 16-byte channel blocks (C)
     emit.cmd1_with_address(stride_y_cmd, strides.height)  # stride between vertical values (H)
     emit.cmd1_with_address(stride_x_cmd, strides.width)  # stride between horisontal values (W)
 
 
 def generate_ifm_precision(emit: CommandStreamEmitter, fm: NpuFeatureMap, op_to_scale: int, precision_cmd: cmd0):
     """Generates IFM/IFM2_PRECISION register"""
@@ -416,56 +430,62 @@
             # Broadcast in 'C' dimension
             assert ifm2.shape.depth == 1
             ifm2_broadcast |= IFM2Broadcast.BroadcastCdim
 
     emit.cmd0_with_param(cmd0.NPU_SET_IFM2_BROADCAST, ifm2_broadcast)
 
 
-def generate_ifm(emit: CommandStreamEmitter, ifm: NpuFeatureMap):
+def generate_ifm(emit: CommandStreamEmitter, ifm: NpuFeatureMap, arch: ArchitectureFeatures):
     """Generates general IFM registers"""
     emit.cmd0_with_param(cmd0.NPU_SET_IFM_REGION, ifm.region)
     generate_addresses(
         emit,
         [cmd1.NPU_SET_IFM_BASE0, cmd1.NPU_SET_IFM_BASE1, cmd1.NPU_SET_IFM_BASE2, cmd1.NPU_SET_IFM_BASE3],
         ifm.tiles.addresses,
         ifm.layout,
+        ifm.data_type.size_in_bytes(),
+        arch,
     )
     generate_tiles(
         emit, [cmd0.NPU_SET_IFM_HEIGHT0_M1, cmd0.NPU_SET_IFM_HEIGHT1_M1, cmd0.NPU_SET_IFM_WIDTH0_M1], ifm.tiles
     )
     emit.cmd0_with_param(cmd0.NPU_SET_IFM_DEPTH_M1, ifm.shape.depth - 1)
     generate_strides(emit, ifm, cmd1.NPU_SET_IFM_STRIDE_C, cmd1.NPU_SET_IFM_STRIDE_Y, cmd1.NPU_SET_IFM_STRIDE_X)
     emit.cmd0_with_param(cmd0.NPU_SET_IFM_ZERO_POINT, get_zero_point(ifm))
 
 
-def generate_ifm2(emit: CommandStreamEmitter, ifm2: NpuFeatureMap, has_scalar: bool):
+def generate_ifm2(emit: CommandStreamEmitter, ifm2: NpuFeatureMap, has_scalar: bool, arch: ArchitectureFeatures):
     """Generates general IFM2 registers"""
     if not has_scalar:
         emit.cmd0_with_param(cmd0.NPU_SET_IFM2_REGION, ifm2.region)
         generate_addresses(
             emit,
             [cmd1.NPU_SET_IFM2_BASE0, cmd1.NPU_SET_IFM2_BASE1, cmd1.NPU_SET_IFM2_BASE2, cmd1.NPU_SET_IFM2_BASE3],
             ifm2.tiles.addresses,
             ifm2.layout,
+            ifm2.data_type.size_in_bytes(),
+            arch,
         )
         generate_tiles(
             emit, [cmd0.NPU_SET_IFM2_HEIGHT0_M1, cmd0.NPU_SET_IFM2_HEIGHT1_M1, cmd0.NPU_SET_IFM2_WIDTH0_M1], ifm2.tiles
         )
         generate_strides(emit, ifm2, cmd1.NPU_SET_IFM2_STRIDE_C, cmd1.NPU_SET_IFM2_STRIDE_Y, cmd1.NPU_SET_IFM2_STRIDE_X)
     emit.cmd0_with_param(cmd0.NPU_SET_IFM2_ZERO_POINT, get_zero_point(ifm2))
 
 
-def generate_ofm(emit: CommandStreamEmitter, ofm: NpuFeatureMap):
+def generate_ofm(emit: CommandStreamEmitter, ofm: NpuFeatureMap, arch: ArchitectureFeatures):
     """Generates general OFM registers"""
     emit.cmd0_with_param(cmd0.NPU_SET_OFM_REGION, ofm.region)
     generate_addresses(
         emit,
         [cmd1.NPU_SET_OFM_BASE0, cmd1.NPU_SET_OFM_BASE1, cmd1.NPU_SET_OFM_BASE2, cmd1.NPU_SET_OFM_BASE3],
         ofm.tiles.addresses,
         ofm.layout,
+        ofm.data_type.size_in_bytes(),
+        arch,
     )
     generate_tiles(
         emit, [cmd0.NPU_SET_OFM_HEIGHT0_M1, cmd0.NPU_SET_OFM_HEIGHT1_M1, cmd0.NPU_SET_OFM_WIDTH0_M1], ofm.tiles
     )
     emit.cmd0_with_param(cmd0.NPU_SET_OFM_HEIGHT_M1, ofm.shape.height - 1)
     emit.cmd0_with_param(cmd0.NPU_SET_OFM_WIDTH_M1, ofm.shape.width - 1)
     emit.cmd0_with_param(cmd0.NPU_SET_OFM_DEPTH_M1, ofm.shape.depth - 1)
@@ -501,17 +521,20 @@
     for core, (addr, length) in enumerate(
         [
             (cmd1.NPU_SET_WEIGHT_BASE, cmd1.NPU_SET_WEIGHT_LENGTH),
             (cmd1.NPU_SET_WEIGHT1_BASE, cmd1.NPU_SET_WEIGHT1_LENGTH),
         ]
     ):
         if core < len(weights):
+            check_alignment(weights[core].address, 16)
+            check_size(weights[core].length, 16)
             emit.cmd1_with_address(addr, weights[core].address)
             emit.cmd1_with_offset(length, weights[core].length)
         elif core < arch.ncores:
+            check_alignment(weights[0].address, 16)
             emit.cmd1_with_address(addr, weights[0].address)
             emit.cmd1_with_offset(length, 0)
 
 
 def generate_biases(emit: CommandStreamEmitter, biases: List[NpuAddressRange], arch: ArchitectureFeatures):
     """Generates SCALE registers"""
     if len(biases) == 0:
@@ -519,14 +542,15 @@
     emit.cmd0_with_param(cmd0.NPU_SET_SCALE_REGION, biases[0].region)
     # Set weights sources for active and present cores
     for core, (addr, length) in enumerate(
         [(cmd1.NPU_SET_SCALE_BASE, cmd1.NPU_SET_SCALE_LENGTH), (cmd1.NPU_SET_SCALE1_BASE, cmd1.NPU_SET_SCALE1_LENGTH)]
     ):
         if core < len(biases):
             emit.cmd1_with_address(addr, biases[core].address)
+            check_size(biases[core].length, 16)
             emit.cmd1_with_offset(length, biases[core].length)
         elif core < arch.ncores:
             emit.cmd1_with_address(addr, biases[0].address)
             emit.cmd1_with_offset(length, 0)
 
 
 def generate_block_config(
@@ -627,20 +651,20 @@
     block_traversal: NpuBlockTraversal,
     arch: ArchitectureFeatures,
     use_global_scale: bool = False,
     op_to_scale: int = 0,
 ):
     """Generate registers that are common to most operations"""
     assert npu_op.ifm is not None and npu_op.ofm is not None
-    generate_ifm(emit, npu_op.ifm)
+    generate_ifm(emit, npu_op.ifm, arch)
     generate_ifm_precision(emit, npu_op.ifm, op_to_scale, cmd0.NPU_SET_IFM_PRECISION)
     emit.cmd0_with_param(cmd0.NPU_SET_IFM_UPSCALE, resampling_mode_map[npu_op.ifm_upscale])
     if npu_op.padding is not None:
         generate_padding(emit, npu_op.padding)
-    generate_ofm(emit, npu_op.ofm)
+    generate_ofm(emit, npu_op.ofm, arch)
     generate_ofm_precision(emit, npu_op, use_global_scale)
     if npu_op.op_type != NpuOperationType.ElementWise:
         assert npu_op.kernel is not None
         generate_kernel(emit, npu_op.kernel, block_traversal)
     generate_weights(emit, npu_op.weights, arch)
     generate_biases(emit, npu_op.biases, arch)
     generate_activation(emit, npu_op.activation, npu_op.ofm)
@@ -970,25 +994,27 @@
         emit, npu_op, NpuBlockTraversal.DEPTH_FIRST, arch, use_global_scale=use_global_scale, op_to_scale=op_to_scale
     )
     # Elementwise op specific
     if npu_op.sub_op_type not in UNARY_ELEMWISE_OPS:
         # Binary operation; generate IFM2 registers
         assert npu_op.ifm2 is not None
         has_scalar = npu_op.ifm2_scalar is not None
-        generate_ifm2(emit, npu_op.ifm2, has_scalar)
+        generate_ifm2(emit, npu_op.ifm2, has_scalar, arch)
         generate_ifm_precision(emit, npu_op.ifm2, 0, cmd0.NPU_SET_IFM2_PRECISION)
         generate_ifm2_broadcast(emit, npu_op)
         if has_scalar:
             quantized_scalar = quantise(npu_op.ifm2_scalar, npu_op.ifm2.quantization)
             assert npu_op.ifm2.data_type.min_value() <= quantized_scalar <= npu_op.ifm2.data_type.max_value()
             emit.cmd0_with_param(cmd0.NPU_SET_IFM2_SCALAR, quantized_scalar)
 
 
-def generate_dma_op(emit: CommandStreamEmitter, dma_op: NpuDmaOperation):
+def generate_dma_op(emit: CommandStreamEmitter, dma_op: NpuDmaOperation, arch: ArchitectureFeatures):
     """Generates register commands for DMA operations"""
+    check_dma_op(dma_op, arch)
+
     emit.cmd0_with_param(cmd0.NPU_SET_DMA0_SRC_REGION, dma_op.src.region)
     emit.cmd1_with_address(cmd1.NPU_SET_DMA0_SRC, dma_op.src.address)
     emit.cmd0_with_param(cmd0.NPU_SET_DMA0_DST_REGION, dma_op.dest.region)
 
     emit.cmd1_with_address(cmd1.NPU_SET_DMA0_DST, dma_op.dest.address)
     emit.cmd1_with_address(cmd1.NPU_SET_DMA0_LEN, dma_op.src.length)
 
@@ -1003,15 +1029,15 @@
     elif isinstance(npu_op, NpuConvDepthWiseOperation):
         generate_conv_depthwise_op(emit, npu_op, arch)
     elif isinstance(npu_op, NpuPoolingOperation):
         generate_pooling_op(emit, npu_op, arch)
     elif isinstance(npu_op, NpuElementWiseOperation):
         generate_elementwise_op(emit, npu_op, arch)
     elif isinstance(npu_op, NpuDmaOperation):
-        generate_dma_op(emit, npu_op)
+        generate_dma_op(emit, npu_op, arch)
     else:
         assert 0, "Unsupported operation"
 
 
 def generate_command_stream(
     npu_op_list: List[NpuOperation],
     arch: ArchitectureFeatures,
@@ -1022,37 +1048,44 @@
 ) -> List[int]:
     """
     Generates register commands for the given list of NPU operations.
     Returns Ethos-U instructions, as a list of 32-bit integers.
     """
     emit = CommandStreamEmitter()
     if verbose:
+        print("Register-Level Command Stream: Input")
         print_operations(npu_op_list, npu_op_to_cmd)
     # Calculate memory accesses for every operation
     memory_accesses: Dict[NpuOperation, MemoryAccessSet] = {}
     for npu_op in npu_op_list:
         if isinstance(npu_op, NpuDmaOperation):
             memory_accesses[npu_op] = get_dma_memory_accesses(npu_op)
         elif isinstance(npu_op, NpuBlockOperation):
             memory_accesses[npu_op] = get_op_memory_accesses(npu_op, arch)
         else:
             assert 0, "Invalid operation type"
 
     if arch.is_ethos_u65_system:
         emit.cmd0_with_param(cmd0.NPU_SET_PARALLEL_MODE, arch.ncores - 1)
-    dep_watermark = Watermark(0, 0)
     prev_op = None
     # Generate register commands for all operations
+    outstanding_dma_ops: List[NpuOperation] = list()
+    outstanding_npu_ops: List[NpuOperation] = list()
     for op_index, npu_op in enumerate(npu_op_list):
         try:
             check_mem_limits(memory_accesses[npu_op], mem_limits)
-            dep_watermark, cmd_waits = get_wait_dependency(arch, npu_op_list, memory_accesses, op_index, dep_watermark)
+            cmd_waits = get_wait_dependency(arch, npu_op, memory_accesses, outstanding_dma_ops, outstanding_npu_ops)
             generate_registers_for_op(emit, npu_op, arch)
+        except ByteAlignmentError as e:
+            # Enables testing for ByteAlignmentErrors specifically
+            raise ByteAlignmentError(f"{e.error_msg}, in operation {op_index}:{npu_op.op_type.name}") from None
+        except ByteSizeError as e:
+            # Enables testing for ByteSizeErrors specifically
+            raise ByteSizeError(f"{e.error_msg}, in operation {op_index}:{npu_op.op_type.name}") from None
         except VelaError as e:
-            # Add operation info and rethrow
             raise VelaError(f"{e.error_msg}, in operation {op_index}:{npu_op.op_type.name}") from None
         if not isinstance(npu_op, NpuDmaOperation) and isinstance(npu_op, NpuBlockOperation):
             # Generate BLOCKDEP
             blockdep = calc_blockdep(arch, prev_op, npu_op)
             blockdep = min(blockdep, arch.max_blockdep)
             emit.cmd0_with_param(cmd0.NPU_SET_BLOCKDEP, blockdep)
             prev_op = npu_op
@@ -1069,14 +1102,15 @@
     if emit.size_in_bytes() >= 1 << 24:
         raise VelaError(
             f"The command stream size exceeds the hardware limit of 16 MiB. "
             f"The current stream size is {emit.size_in_bytes()/2**20:.2F} MiB."
         )
 
     if verbose:
+        print("Register-Level Command Stream: Output")
         emit.print_cmds()
         print(f"Number of commands = {len(emit.cmd_stream)}")
         print(f"Command stream length = {emit.size_in_bytes()} bytes")
     return res
 
 
 def generate_register_command_stream(npu_op_list: List[NpuOperation], npu_accelerator: NpuAccelerator) -> List[int]:
```

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/register_command_stream_util.py` & `ethos-u-vela-3.9.0/ethosu/vela/register_command_stream_util.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright 2020-2022 Arm Limited and/or its affiliates <open-source-office@arm.com>
+# SPDX-FileCopyrightText: Copyright 2020-2023 Arm Limited and/or its affiliates <open-source-office@arm.com>
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 # Licensed under the Apache License, Version 2.0 (the License); you may
 # not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -33,27 +33,43 @@
 from .api import NpuOperationType
 from .api import NpuPadding
 from .api import NpuQuantization
 from .api import NpuShape3D
 from .architecture_features import ArchitectureFeatures
 from .architecture_features import Block
 from .architecture_features import Rect
+from .errors import ByteAlignmentError
+from .errors import ByteSizeError
 from .operation import Kernel
 from .operation import PointXYZ
+from .tensor import TensorFormat
 from ethosu.vela.range_set import AccessDirection
 from ethosu.vela.range_set import MemoryAccessSet
 from ethosu.vela.range_set import MemoryRangeSet
 
+
 # base address slot for memory to memory transfer
 BASE_PTR_INDEX_MEM2MEM = int((1 << 8) | (3 << 0))
 
 
 UNARY_ELEMWISE_OPS = (NpuElementWiseOp.ABS, NpuElementWiseOp.LRELU, NpuElementWiseOp.CLZ)
 
 
+def check_alignment(payload, required_alignment):
+    # assuming payload is defined in bytes
+    if payload % required_alignment != 0:
+        raise ByteAlignmentError(f"Cmd1 payload of size: {payload} Bytes is not {required_alignment}-byte aligned")
+
+
+def check_size(payload, required_multiple):
+    # assuming payload is defined in bytes
+    if payload % required_multiple != 0:
+        raise ByteSizeError(f"Cmd1 payload of size: {payload} Bytes is not a multiple of {required_multiple}")
+
+
 def to_npu_kernel(kernel: Kernel) -> NpuKernel:
     """Converts the given internally used kernel object to NpuKernel (of public API)"""
     return NpuKernel(
         kernel.width, kernel.height, kernel.stride.x, kernel.stride.y, kernel.dilation.x, kernel.dilation.y
     )
 
 
@@ -237,14 +253,37 @@
     if t1 is not None and t2 is not None:
         t3 = get_address_range(fm, strides, height_1, width_0, 0, height - 1, width - 1, depth - 1)
     else:
         t3 = None
     return [t0, t1, t2, t3]
 
 
+def check_strides(fm: NpuFeatureMap, strides: NpuShape3D):
+
+    element_size_in_bytes = fm.data_type.size_in_bytes()
+
+    if fm.layout == NpuLayout.NHCWB16:
+        strides_to_check = [strides.depth, strides.height]
+        required_multiple = 16 * element_size_in_bytes
+    else:
+        strides_to_check = [strides.height, strides.width]
+        required_multiple = element_size_in_bytes
+    for stride in strides_to_check:
+        check_size(stride, required_multiple)
+
+
+def check_addresses(addresses: List[int], layout: NpuLayout, element_size, arch: ArchitectureFeatures):
+    if layout == NpuLayout.NHCWB16:
+        required_alignment = arch.storage_rounding_quantums[TensorFormat.NHCWB16][-1]
+    else:
+        required_alignment = element_size
+    for addr in addresses:
+        check_alignment(addr, required_alignment)
+
+
 # -------------------------------------------------------------------
 # DMA_WAIT/KERNEL_WAIT
 # -------------------------------------------------------------------
 
 
 class Watermark(NamedTuple):
     npu: int
@@ -290,70 +329,70 @@
     for write_range in write_ranges:
         if write_range is not None:
             res.add(memory_range_set(write_range), AccessDirection.Write)
     return res
 
 
 def get_wait_dependency(
-    arch: ArchitectureFeatures, npu_op_list: List[NpuOperation], memory_accesses, op_index: int, watermark: Watermark
+    arch: ArchitectureFeatures,
+    npu_op: NpuOperation,
+    memory_accesses,
+    outstanding_dma_ops: List[NpuOperation],
+    outstanding_npu_ops: List[NpuOperation],
 ):
     """Used to calculate whether DMA wait or kernel wait operations are needed"""
-    npu_op = npu_op_list[op_index]
-    op_access = memory_accesses[npu_op]
-    index = op_index - 1
-
-    # NPU dependency tracking
-    npu_outstanding = -1
-    npu_ops = 0
-    npu_index = watermark.npu
-
-    # DMA dependency tracking
-    dma_outstanding = -1
-    dma_ops = 0
-    dma_index = watermark.dma
-
-    # Seek back in the command stream looking for NPU or DMA dependencies
-    # but only as far as the first dependency or the watermarks (dependencies
-    # before this point have been satisfied already).
-    # The watermark moves to after the latest element we must wait for, not
-    # the command that issues the wait.
-    # NPU->NPU dependency is handled via blockdep.
-    while (index >= npu_index) or (index >= dma_index):
-        prev_op = npu_op_list[index]
-        prev_access = memory_accesses[prev_op]
-
-        # Check NPU consuming DMA output
-        if isinstance(prev_op, NpuDmaOperation):
-            if index >= dma_index:
-                if not isinstance(npu_op, NpuDmaOperation):
-                    if (dma_outstanding == -1) and prev_access.conflicts(op_access):
-                        dma_outstanding = dma_ops
-                dma_ops += 1  # Count DMA ops in the pipeline
-                if dma_ops >= arch.max_outstanding_dma:
-                    dma_index = max(index + 1, dma_index)
-        # Check DMA consuming NPU output
-        else:
-            if index >= npu_index:
-                if isinstance(npu_op, NpuDmaOperation) and npu_outstanding == -1 and prev_access.conflicts(op_access):
-                    npu_outstanding = npu_ops
-                npu_ops += 1  # Count NPU ops in the pipeline
-                if npu_ops >= arch.max_outstanding_kernels:
-                    npu_index = max(index + 1, npu_index)
-
-        index -= 1
-
-    # Update DMA watermark if we didn't see any and the NPU pipeline is full
-    if (dma_ops == 0) and (npu_ops >= arch.max_outstanding_kernels):
-        dma_index = op_index
-
-    # Bring the search watermark forwards as we complete for those dependencies
-    watermark = Watermark(npu_index, dma_index)
-    outstanding = Watermark(npu_outstanding, dma_outstanding)
-
-    return watermark, outstanding
+    kern_wait = -1
+    dma_wait = -1
+    op_accesses = memory_accesses[npu_op]
+
+    if isinstance(npu_op, NpuDmaOperation):
+        outstanding_ops = outstanding_npu_ops
+        outstanding_dma_ops.append(npu_op)
+        if len(outstanding_dma_ops) > arch.max_outstanding_dma:
+            outstanding_dma_ops.pop(0)
+    else:
+        outstanding_ops = outstanding_dma_ops
+        outstanding_npu_ops.append(npu_op)
+        if len(outstanding_npu_ops) > arch.max_outstanding_kernels:
+            outstanding_npu_ops.pop(0)
+
+    waits = -1
+    for idx in range(len(outstanding_ops) - 1, -1, -1):
+        waits += 1
+        other_op = outstanding_ops[idx]
+        other_accesses = memory_accesses[other_op]
+        if other_accesses.conflicts(op_accesses):
+            if isinstance(npu_op, NpuDmaOperation):
+                kern_wait = waits
+            else:
+                dma_wait = waits
+            # Current op needs to wait, and after it has waited,
+            # outstanding_ops[0..idx] are not outstanding any longer
+            for i in range(idx + 1):
+                outstanding_ops.pop(0)
+            break
+
+    cmd_waits = Watermark(kern_wait, dma_wait)
+    return cmd_waits
+
+
+def check_dma_op(dma_op: NpuDmaOperation, arch: ArchitectureFeatures):
+
+    # For Ethos-U65 only internal addresses have to be aligned, and if the internal address is the destination
+    # then the length has to be aligned also.
+    if arch.is_ethos_u65_system:
+        if dma_op.src.region == BASE_PTR_INDEX_MEM2MEM:
+            check_alignment(dma_op.src.address, 16)
+        if dma_op.dest.region == BASE_PTR_INDEX_MEM2MEM:
+            check_alignment(dma_op.dest.address, 16)
+            check_size(dma_op.src.length, 16)
+    else:
+        check_alignment(dma_op.src.address, 16)
+        check_alignment(dma_op.dest.address, 16)
+        check_size(dma_op.src.length, 16)
 
 
 # -------------------------------------------------------------------
 # BLOCKDEP
 # -------------------------------------------------------------------
```

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/rewrite_graph.py` & `ethos-u-vela-3.9.0/ethosu/vela/rewrite_graph.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/scaling.py` & `ethos-u-vela-3.9.0/ethosu/vela/scaling.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/scheduler.py` & `ethos-u-vela-3.9.0/ethosu/vela/scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -256,14 +256,35 @@
                 self.parent_ps.ifm_shapes = self.parent_ps.ifm_shapes[::-1]
                 self.parent_ps.inputs = self.parent_ps.inputs[::-1]
                 self.parent_ps.ifm_tensor, self.parent_ps.ifm2_tensor = (
                     self.parent_ps.ifm2_tensor,
                     self.parent_ps.ifm_tensor,
                 )
 
+    @property
+    def ofm_write_shape(self):
+        if self.ofm:
+            ofm_write_shape = self.parent_op.write_shape
+            return ofm_write_shape if ofm_write_shape else self.ofm.shape
+        return None
+
+    @property
+    def ifm_read_shape(self):
+        if self.ifm:
+            ifm_read_shape = self.parent_op.read_shapes[1] if self.reversed_operands else self.parent_op.read_shapes[0]
+            return ifm_read_shape if ifm_read_shape else self.ifm.shape
+        return None
+
+    @property
+    def ifm2_read_shape(self):
+        if self.ifm2:
+            ifm2_read_shape = self.parent_op.read_shapes[0] if self.reversed_operands else self.parent_op.read_shapes[1]
+            return ifm2_read_shape if ifm2_read_shape else self.ifm2.shape
+        return None
+
     def add_ifm_connection(self, conn: "Connection"):
         """Add input connection to another SchedulerOperation or Subgraph Input"""
         conn.consumers.append(self)
         self.ifm.connection = conn
 
     def add_ifm2_connection(self, conn: "Connection"):
         """Add input connection to another SchedulerOperation or Subgraph Input"""
@@ -412,14 +433,17 @@
         self.nng = nng
         self.sg = sg
         self.arch = arch
         self.sched_ops: List[SchedulerOperation] = []
         self.max_schedule: Optional[Schedule] = None
         self.scheduler_options = options
 
+        # sram limit can be changed when scheduling for Size
+        self.sram_limit = options.optimization_sram_limit
+
         self.scratched_fms: Dict[Tensor, Any] = {}
         self.evicted_fms: List[live_range.LiveRange] = []
 
     def avoid_nhcwb16_for_ofm(self, tens, ps, arch):
         """For elementwise ops when ifm is in nhwc format and not brick format aligned (16),
         then if the ofm can overwrite the ifm it is better to enforce ofm format to nhwc in
         order to reduce memory transactions"""
@@ -558,47 +582,47 @@
         schedule.memory_snapshot = temporal_usage
 
         # Set the peak memory usage
         schedule.fast_storage_peak_usage = max(temporal_usage, default=0)
 
     def estimate_op_performance(self, op: SchedulerOperation, block_config, ofm_depth):
         query = npu_performance.PerformanceQuery(op.op_type.npu_block_type)
-        query.ifm_shape = op.ifm.shape
-        query.ifm_memory_area = op.ifm.mem_area
+        query.ifm_shape = op.ifm_read_shape
+        query.ifm_memory_area = op.ifm.connection.parent_tens.mem_area
         query.ifm_bits = op.ifm.dtype.size_in_bits()
         query.ifm_format = op.ifm.format
-        query.ifm2_shape = op.ifm2 and op.ifm2.shape
-        query.ifm2_memory_area = op.ifm2 and op.ifm2.mem_area
+        query.ifm2_shape = op.ifm2_read_shape
+        query.ifm2_memory_area = op.ifm2 and op.ifm2.connection.parent_tens.mem_area
         query.ifm2_bits = op.ifm2 and op.ifm2.dtype.size_in_bits()
         query.ifm2_format = op.ifm2 and op.ifm2.format
-        query.ofm_shape = op.ofm.shape.with_depth(ofm_depth)
-        query.ofm_memory_area = op.ofm.mem_area
+        query.ofm_shape = op.ofm_write_shape.with_depth(ofm_depth)
+        query.ofm_memory_area = op.ofm.connection.parent_tens.mem_area
         query.ofm_bits = op.ofm.dtype.size_in_bits()
         query.ofm_format = op.ofm.format
         if op.parent_op.bias:
             query.const_shape = Shape4D(1, 1, 1, op.ofm.shape.depth)
             query.const_memory_area = self.arch.fast_storage_mem_area
 
         query.kernel = op.kernel
         query.config = block_config
 
         return npu_performance.measure_cycle_cost(self.arch, op.op_type, op.activation and op.activation.op_type, query)
 
     def estimate_element_access(self, op: SchedulerOperation, block_config, ofm_depth):
         query = npu_performance.PerformanceQuery(op.op_type.npu_block_type)
-        query.ifm_shape = op.ifm.shape
-        query.ifm_memory_area = op.ifm.mem_area
+        query.ifm_shape = op.ifm_read_shape
+        query.ifm_memory_area = op.ifm.connection.parent_tens.mem_area
         query.ifm_bits = op.ifm.dtype.size_in_bits()
         query.ifm_format = op.ifm.format
-        query.ifm2_shape = op.ifm2 and op.ifm2.shape
-        query.ifm2_memory_area = op.ifm2 and op.ifm2.mem_area
+        query.ifm2_shape = op.ifm2_read_shape
+        query.ifm2_memory_area = op.ifm2 and op.ifm2.connection.parent_tens.mem_area
         query.ifm2_bits = op.ifm2 and op.ifm2.dtype.size_in_bits()
         query.ifm2_format = op.ifm2 and op.ifm2.format
-        query.ofm_shape = op.ofm.shape.with_depth(ofm_depth)
-        query.ofm_memory_area = op.ofm.mem_area
+        query.ofm_shape = op.ofm_write_shape.with_depth(ofm_depth)
+        query.ofm_memory_area = op.ofm.connection.parent_tens.mem_area
         query.ofm_bits = op.ofm.dtype.size_in_bits()
         query.ofm_format = op.ofm.format
         if op.parent_op.bias:
             query.const_shape = Shape4D(1, 1, 1, op.ofm.shape.depth)
             query.const_memory_area = self.arch.fast_storage_mem_area
 
         query.kernel = op.kernel
@@ -876,14 +900,17 @@
         cost_map = min_schedule.cost_map
         verbose_progress = self.scheduler_options.verbose_progress
         # Keep track of the previous Op - which consumes the current Op's OFM
         prev_op: Optional[SchedulerOperation] = None
         for index, sched_op in enumerate(reversed(self.sched_ops)):
             progress_print(verbose_progress, "Processing SchedulerOp", index, self.sched_ops)
             min_stripe_height = prev_op.kernel.stride.y if prev_op else 1
+            if is_nearest(sched_op.resampling_mode):
+                # is nearest requires even stripes
+                min_stripe_height += min_stripe_height % 2
             min_stripe = sched_op.ofm.shape.with_height(min_stripe_height)
 
             cost = sched_op.create_scheduler_info(self.nng, min_stripe)
             cost.cycles = self.estimate_op_performance(sched_op, cost.block_config, sched_op.ofm.shape.depth)
             cost_map[sched_op] = cost
 
             prev_op = sched_op
@@ -1038,17 +1065,15 @@
             non_local_mem_usage[sched_op] = mem_usage_parallel_to_sub_schedule
             if idx != 0:
                 non_local_mem_usage[sched_op] += persistent_initial_ifm
 
         cascade_builder = CascadeBuilder(sub_schedule_ops, self.arch.is_spilling_enabled(), non_local_mem_usage)
 
         # Start by adding buffering
-        buffered_sub_schedule = self.propose_schedule_buffering(
-            sub_schedule, self.scheduler_options.optimization_sram_limit
-        )
+        buffered_sub_schedule = self.propose_schedule_buffering(sub_schedule, self.sram_limit)
         # Copy the cascades over from the unbuffered-schedule
         buffered_sub_schedule.cascades = sub_schedule.cascades
 
         # Generate the possible stripings for the final Op in the sub-schedule
         final_ofm_shape = sub_schedule_ops[-1].ofm.shape
 
         # Skip testing the min stripe used in the MIN schedule since that will be used
@@ -1088,51 +1113,48 @@
         return best_schedule
 
     def optimize_schedule(
         self,
         schedule: Schedule,
         max_sched: Schedule,
         max_template: Schedule,
-        options: SchedulerOptions,
     ) -> Schedule:
         """Extracts sub-schedules based on the cascades and optimizes them and applies them to the final schedule"""
-        verbose_progress = options.verbose_progress
-        sram_limit = options.optimization_sram_limit
-        if max_sched.fast_storage_peak_usage < sram_limit and not self.arch.is_spilling_enabled():
+        verbose_progress = self.scheduler_options.verbose_progress
+        if max_sched.fast_storage_peak_usage < self.sram_limit and not self.arch.is_spilling_enabled():
             # Maximum performance schedule fits within the SRAM target
             return max_sched
 
         # Iterate over a copy of the cascades since they may change during the loop
         cascades = list(schedule.cascades.values())
         for index, cascade_info in enumerate(cascades):
             progress_print(verbose_progress, "Processing cascade", index, cascades)
             # Optimize the sub-schedule in this cascade
-            opt_sub_schedule = self.optimize_sub_schedule(cascade_info, schedule, max_template, sram_limit)
+            opt_sub_schedule = self.optimize_sub_schedule(cascade_info, schedule, max_template, self.sram_limit)
             if opt_sub_schedule:
                 # Remove the existing cascade
                 del schedule.cascades[cascade_info.end]
                 # Update the sub-schedule Op and cascade costs to the full schedule
                 schedule.cost_map.update(opt_sub_schedule.cost_map)
                 schedule.cascades.update(opt_sub_schedule.cascades)
 
         # Update memory snapshot
         self.sg.schedule = schedule
         self.update_op_memory_snapshot(schedule)
         # Propose schedule buffering to the optimized schedule
-        optimized_sched = self.propose_schedule_buffering(schedule, self.scheduler_options.optimization_sram_limit)
+        optimized_sched = self.propose_schedule_buffering(schedule, self.sram_limit)
         # Copy the cascade's metadata from the unbuffered schedule
         optimized_sched.cascades = schedule.cascades
         return optimized_sched
 
     def optimize_weight_buffering_size(
         self,
         min_schedule: Schedule,
-        options: SchedulerOptions,
     ):
-        verbose_progress = options.verbose_progress
+        verbose_progress = self.scheduler_options.verbose_progress
         default_schedule = self.sg.schedule
         npu_performance.calc_new_performance_for_network(self.nng, self.arch, None, False)
         default_tot_cycles = self.nng.cycles[npu_performance.PassCycles.Total]
         default_dram_cycles = self.nng.cycles[npu_performance.PassCycles.DramAccess]
 
         # Restore mem/type for scratched_fms
         for tens in self.scratched_fms:
@@ -1174,22 +1196,22 @@
                             sched_op.evicted_fms_size += lr.size
                             break
 
         self.sg.schedule = min_schedule
         self.update_op_memory_snapshot(self.sg.schedule)
 
         # Run schedule buffering - with weight buffer size reduction
-        schedule = self.propose_schedule_buffering(self.sg.schedule, options.optimization_sram_limit)
+        schedule = self.propose_schedule_buffering(self.sg.schedule, self.sram_limit)
         schedule.cascades = self.sg.schedule.cascades
         self.sg.schedule = schedule
 
         # Apply new buffer schdule and calc new performance
         self.update_op_memory_snapshot(self.sg.schedule)
         self.apply_schedule(self.sg.schedule)
-        self.use_fast_storage_for_feature_maps(self.sg.schedule, options.optimization_sram_limit)
+        self.use_fast_storage_for_feature_maps(self.sg.schedule, self.sram_limit)
 
         npu_performance.calc_new_performance_for_network(self.nng, self.arch, None, False)
         new_tot_cycles = self.nng.cycles[npu_performance.PassCycles.Total]
         new_dram_cycles = self.nng.cycles[npu_performance.PassCycles.DramAccess]
 
         improvement_tot = (
             round((default_tot_cycles - new_tot_cycles) / default_tot_cycles, 2) if default_tot_cycles != 0 else 0
@@ -1207,15 +1229,15 @@
             for tens in self.scratched_fms:
                 tens.mem_area = self.scratched_fms[tens][0]
                 tens.mem_type = self.scratched_fms[tens][1]
 
             self.sg.schedule = default_schedule
             self.update_op_memory_snapshot(self.sg.schedule)
             self.apply_schedule(self.sg.schedule)
-            self.use_fast_storage_for_feature_maps(self.sg.schedule, options.optimization_sram_limit)
+            self.use_fast_storage_for_feature_maps(self.sg.schedule, self.sram_limit)
 
     def apply_schedule(self, sched: Schedule):
         """Applies the given schedule as a final solution"""
         for sched_op in self.sched_ops:
             op_info = sched.cost_map[sched_op]
             cascade_info = sched.cascades.get(op_info.cascade, None)
             if cascade_info and sched_op in cascade_info.buffers:
@@ -1621,40 +1643,43 @@
             opt_max_schedule = scheduler.propose_schedule_buffering(max_schedule_template, 1 << 32)
             sg.schedule = opt_max_schedule
             scheduler.update_op_memory_snapshot(opt_max_schedule)
 
             progress_print(verbose_progress, "Creating minimal schedule")
             # Create Min schedule
             min_schedule = scheduler.propose_minimal_schedule()
-            initial_sram_limit = scheduler_options.optimization_sram_limit
+            initial_sram_limit = scheduler.sram_limit
             if scheduler_options.optimization_strategy == OptimizationStrategy.Size:
                 initial_sram_limit = scheduler.min_memory_req
 
             # Build cascades for Min schedule
             progress_print(verbose_progress, "Building cascades for minimal schedule")
             scheduler.build_cascades_for_min_schedule(min_schedule, max_schedule_template, initial_sram_limit)
             sg.schedule = min_schedule
             scheduler.update_op_memory_snapshot(min_schedule)
 
-            if scheduler_options.optimization_strategy == OptimizationStrategy.Performance:
+            if scheduler_options.optimization_strategy == OptimizationStrategy.Size:
                 progress_print(verbose_progress, "Creating schedule optimized for performance")
-                # Create an optimized schedule
-                sg.schedule = scheduler.optimize_schedule(
-                    min_schedule, opt_max_schedule, max_schedule_template, scheduler_options
-                )
-                scheduler.update_op_memory_snapshot(sg.schedule)
+                # Update sram limit to peak usage from the minimum scheduler when optimizing for Size.
+                # Then optimize schedule can be called for both OptimizationStrategy Performance and Size
+                # as long the max sram usage is <= scheduler.sram_limit
+                scheduler.sram_limit = min_schedule.fast_storage_peak_usage
+
+            # Create an optimized schedule
+            sg.schedule = scheduler.optimize_schedule(min_schedule, opt_max_schedule, max_schedule_template)
+            scheduler.update_op_memory_snapshot(sg.schedule)
 
             scheduler.apply_schedule(sg.schedule)
-            scheduler.use_fast_storage_for_feature_maps(sg.schedule, scheduler_options.optimization_sram_limit)
+            scheduler.use_fast_storage_for_feature_maps(sg.schedule, scheduler.sram_limit)
 
             if scheduler_options.optimization_strategy == OptimizationStrategy.Performance and scheduler.evicted_fms:
                 progress_print(verbose_progress, "Optimizing weight buffering size")
                 # It might be possible to gain performance by reducing
                 # weight buffer size and instead fit fms in fast storage
-                scheduler.optimize_weight_buffering_size(min_schedule, scheduler_options)
+                scheduler.optimize_weight_buffering_size(min_schedule)
 
             if scheduler_options.verbose_schedule:
                 scheduler.print_schedule(sg.schedule)
 
     progress_print(verbose_progress, "Update memory snapshot for all NPU graphs")
     # Make a full live range calculation starting from the root sg
     _update_memory_snapshot_for_all_npu_graphs(nng, arch, schedulers, verbose_progress)
```

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/shape4d.py` & `ethos-u-vela-3.9.0/ethosu/vela/shape4d.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/softmax.py` & `ethos-u-vela-3.9.0/ethosu/vela/softmax.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/stats_writer.py` & `ethos-u-vela-3.9.0/ethosu/vela/stats_writer.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/supported_operators_util.py` & `ethos-u-vela-3.9.0/ethosu/vela/supported_operators_util.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tensor.py` & `ethos-u-vela-3.9.0/ethosu/vela/tensor.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tensor_allocation.py` & `ethos-u-vela-3.9.0/ethosu/vela/tensor_allocation.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/test/extapi/test_extapi_create_payload.py` & `ethos-u-vela-3.9.0/ethosu/vela/test/extapi/test_extapi_create_payload.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/test/extapi/test_extapi_encode_bias.py` & `ethos-u-vela-3.9.0/ethosu/vela/test/extapi/test_extapi_encode_bias.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/test/extapi/test_extapi_encode_weights.py` & `ethos-u-vela-3.9.0/ethosu/vela/test/extapi/test_extapi_encode_weights.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/test/extapi/test_extapi_find_block_configs.py` & `ethos-u-vela-3.9.0/ethosu/vela/test/extapi/test_extapi_find_block_configs.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/test/extapi/test_extapi_get_version.py` & `ethos-u-vela-3.9.0/ethosu/vela/test/extapi/test_extapi_get_version.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/test/test_architecture_allocator.py` & `ethos-u-vela-3.9.0/ethosu/vela/test/test_architecture_allocator.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/test/test_build.py` & `ethos-u-vela-3.9.0/ethosu/vela/test/test_build.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/test/test_compiler_driver.py` & `ethos-u-vela-3.9.0/ethosu/vela/test/test_compiler_driver.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/test/test_fp_math.py` & `ethos-u-vela-3.9.0/ethosu/vela/test/test_fp_math.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/test/test_graph_optimiser.py` & `ethos-u-vela-3.9.0/ethosu/vela/test/test_graph_optimiser.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/test/test_hillclimb_allocation.py` & `ethos-u-vela-3.9.0/ethosu/vela/test/test_hillclimb_allocation.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/test/test_live_range.py` & `ethos-u-vela-3.9.0/ethosu/vela/test/test_live_range.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/test/test_lut.py` & `ethos-u-vela-3.9.0/ethosu/vela/test/test_lut.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/test/test_model_reader.py` & `ethos-u-vela-3.9.0/ethosu/vela/test/test_model_reader.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/test/test_new_performance.py` & `ethos-u-vela-3.9.0/ethosu/vela/test/test_new_performance.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/test/test_nng_mapping.py` & `ethos-u-vela-3.9.0/ethosu/vela/test/test_nng_mapping.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/test/test_register_command_stream_util.py` & `ethos-u-vela-3.9.0/ethosu/vela/test/test_register_command_stream_util.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/test/test_scaling.py` & `ethos-u-vela-3.9.0/ethosu/vela/test/test_scaling.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/test/test_tensor_allocation.py` & `ethos-u-vela-3.9.0/ethosu/vela/test/test_tensor_allocation.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/test/test_tflite_model_semantic.py` & `ethos-u-vela-3.9.0/ethosu/vela/test/test_tflite_model_semantic.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,22 +117,40 @@
     op = testutil.create_op_with_quant_tensors(Op.Conv2DBias, [1, 1, 1, 1], [1, 1, 1, 1], weights_shape=[1, 1, 1, 1])
     op.attrs = {"stride_w": 1, "stride_h": 1}
     assert semantic_checker.is_operator_semantic_valid(op)
 
 
 def test_constraint_stride_type():
     # Stride width and height must be integer types
-    op = testutil.create_op_with_quant_tensors(Op.Conv2DBias, [1, 8, 8, 8], [1, 8, 8, 8])
+    op = testutil.create_op_with_quant_tensors(Op.Conv2DBias, [1, 8, 8, 8], [1, 8, 8, 8], weights_shape=[1, 1, 1, 1])
     op.attrs = {"stride_w": 1.5, "stride_h": "1"}
     assert not semantic_checker.is_operator_semantic_valid(op)
 
 
+def test_constraint_conv_groups_ifm_depth():
+    # Test IFM depth is a whole multiple of the filter kernel depth
+    op = testutil.create_op_with_quant_tensors(Op.Conv2DBias, [1, 8, 8, 15], [1, 8, 8, 5], weights_shape=[1, 1, 3, 5])
+    assert semantic_checker.is_operator_semantic_valid(op)
+
+    op = testutil.create_op_with_quant_tensors(Op.Conv2DBias, [1, 8, 8, 15], [1, 8, 8, 5], weights_shape=[1, 1, 4, 5])
+    assert not semantic_checker.is_operator_semantic_valid(op)
+
+
+def test_constraint_conv_groups_num_filters():
+    # Test number of filter kernels is equally divisible by the number of convolution groups
+    op = testutil.create_op_with_quant_tensors(Op.Conv2DBias, [1, 8, 8, 15], [1, 8, 8, 20], weights_shape=[1, 1, 3, 20])
+    assert semantic_checker.is_operator_semantic_valid(op)
+
+    op = testutil.create_op_with_quant_tensors(Op.Conv2DBias, [1, 8, 8, 15], [1, 8, 8, 21], weights_shape=[1, 1, 3, 21])
+    assert not semantic_checker.is_operator_semantic_valid(op)
+
+
 def test_constraint_dilation_type():
     # Dilation width and height must be integer types
-    op = testutil.create_op_with_quant_tensors(Op.Conv2DBias, [1, 8, 8, 8], [1, 8, 8, 8])
+    op = testutil.create_op_with_quant_tensors(Op.Conv2DBias, [1, 8, 8, 8], [1, 8, 8, 8], weights_shape=[1, 1, 1, 1])
     op.attrs = {"stride_w": 1, "stride_h": 1, "dilation_w_factor": 1.5, "dilation_h_factor": "1"}
     assert not semantic_checker.is_operator_semantic_valid(op)
 
 
 def test_constraint_quant_scale_inf():
     # Test handling IFM scale/OFM scale is infinite
     op = testutil.create_op_with_quant_tensors(Op.Relu, [1, 8, 8, 8], [1, 8, 8, 8])
@@ -334,14 +352,26 @@
         padding=[[0, 0], [1, 1], [1, 1], [0, 0]],
     )
     assert semantic_checker.is_operator_semantic_valid(op)
     op.add_input_tensor(op.inputs[0].clone())
     assert not semantic_checker.is_operator_semantic_valid(op)
 
 
+def test_constraint_pad_output_shape():
+    # Incorrect output tensor shape
+    op = create_pad_op(
+        in_shape=[1, 1, 1, 1],
+        out_shape=[1, 3, 3, 1],
+        padding=[[0, 0], [1, 1], [1, 1], [0, 0]],
+    )
+    assert semantic_checker.is_operator_semantic_valid(op)
+    op.outputs[0].shape = [1, 1, 1, 1]
+    assert not semantic_checker.is_operator_semantic_valid(op)
+
+
 def create_strided_slice():
     # Creates a valid strided slice operator with some valid inputs/outputs
     op = create_strided_slice_op([1, 10, 10, 10], [1, 5, 5, 10], [127, 2, 2, 0], [0, 7, -3, 0])
     op.attrs["begin_mask"] = 1
     op.attrs["end_mask"] = 9
     assert semantic_checker.is_operator_semantic_valid(op)
     return op
@@ -502,22 +532,29 @@
     assert semantic_checker.is_operator_semantic_valid(op)
     op.ifm.dtype = DataType.int16
     op.ofm.dtype = DataType.int16
     assert semantic_checker.is_operator_semantic_valid(op)
 
 
 def test_mean_axis():
-    op = create_mean([1, 6, 6, 16], [1, 1, 1, 16], 0, DataType.int8, {"keep_dims": True})
-    assert not semantic_checker.is_operator_semantic_valid(op)
     op = create_mean([1, 6, 6, 16], [1, 1, 1, 16], [3], DataType.int8, {"keep_dims": True})
     assert not semantic_checker.is_operator_semantic_valid(op)
-    op = create_mean([1, 6, 6, 16], [1, 1, 1, 16], [1, 3], DataType.int8, {"keep_dims": True})
+    op = create_mean([1, 6, 6, 1], [1, 1, 1, 1], [3], DataType.int8, {"keep_dims": True})
+    assert semantic_checker.is_operator_semantic_valid(op)
+
+    op = create_mean([2, 6, 6, 16], [2, 1, 1, 16], [0], DataType.int8, {"keep_dims": True})
     assert not semantic_checker.is_operator_semantic_valid(op)
-    op = create_mean([1, 6, 6, 16], [1, 1, 1, 16], [0, 1], DataType.int8, {"keep_dims": True})
+    op = create_mean([1, 6, 6, 16], [1, 1, 1, 16], 0, DataType.int8, {"keep_dims": True})
+    assert semantic_checker.is_operator_semantic_valid(op)
+
+    op = create_mean([2, 6, 6, 16], [2, 1, 1, 16], [0, 1], DataType.int8, {"keep_dims": True})
     assert not semantic_checker.is_operator_semantic_valid(op)
+    op = create_mean([1, 6, 6, 16], [1, 1, 1, 16], [0, 1], DataType.int8, {"keep_dims": True})
+    assert semantic_checker.is_operator_semantic_valid(op)
+
     op = create_mean([1, 6, 6, 16], [1, 1, 1, 16], [1, 2], DataType.int8, {"keep_dims": True})
     assert semantic_checker.is_operator_semantic_valid(op)
     op = create_mean([1, 6, 6, 16], [1, 1, 1, 16], [1], DataType.int8, {"keep_dims": True})
     assert semantic_checker.is_operator_semantic_valid(op)
     op = create_mean([1, 6, 6, 16], [1, 1, 1, 16], 2, DataType.int8, {"keep_dims": True})
     assert semantic_checker.is_operator_semantic_valid(op)
     op = create_mean([1, 6, 6, 16], [1, 1, 1, 16], [2, 1], DataType.int8, {"keep_dims": True})
```

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/test/test_tflite_reader.py` & `ethos-u-vela-3.9.0/ethosu/vela/test/test_tflite_reader.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/test/test_tflite_supported_operators.py` & `ethos-u-vela-3.9.0/ethosu/vela/test/test_tflite_supported_operators.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 # distributed under the License is distributed on an AS IS BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # Description:
 # Unit tests for tflite support_operators
+from typing import List
+
 import numpy as np
 import pytest
 
 from ethosu.vela.data_type import DataType
 from ethosu.vela.operation import ActivationFunction
 from ethosu.vela.operation import Op
 from ethosu.vela.operation import Padding
@@ -102,31 +104,32 @@
     # First test a simple conv passes
     op = testutil.create_op_with_quant_tensors(Op.Conv2DBias, [1, 1, 1, 1], [1, 1, 1, 1], weights_shape=[1, 1, 1, 1])
     op.attrs = {"stride_w": 1, "stride_h": 1}
     assert support.is_operator_supported(op)
 
 
 @pytest.mark.parametrize(
-    "stride_w, stride_h, supported",
+    "ifm_shape, stride_w, stride_h, supported",
     [
-        [0, 20, False],
-        [20, 0, False],
-        [4, 3, True],
-        [4, 5, False],
-        [4, 9, False],
-        [3, 3, True],
-        [1, 1, True],
-        [20, 2, True],
-        [6, 3, True],
-        [8, 1, True],
+        [[1, 8, 8, 8], 0, 20, False],
+        [[1, 8, 8, 8], 20, 0, False],
+        [[1, 8, 8, 8], 4, 3, True],
+        [[1, 8, 8, 8], 4, 5, False],
+        [[1, 8, 8, 8], 4, 9, False],
+        [[1, 8, 8, 8], 3, 3, True],
+        [[1, 8, 8, 8], 1, 1, True],
+        [[1, 8, 8, 8], 20, 2, False],
+        [[1, 8, 40, 8], 20, 2, True],
+        [[1, 8, 40, 8], 6, 3, True],
+        [[1, 8, 40, 8], 8, 1, True],
     ],
 )
-def test_constraint_stride_range(stride_w: int, stride_h: int, supported: bool):
+def test_constraint_stride_range(ifm_shape: List[int], stride_w: int, stride_h: int, supported: bool):
     # Stride width and height must lie within a certain range
-    op = testutil.create_op_with_quant_tensors(Op.Conv2DBias, [1, 8, 8, 8], [1, 8, 8, 8], [1, 1, 1, 1])
+    op = testutil.create_op_with_quant_tensors(Op.Conv2DBias, ifm_shape, [1, 8, 8, 8], [1, 1, 1, 1])
     op.attrs = {"stride_w": stride_w, "stride_h": stride_h}
     assert support.is_operator_supported(op) == supported
 
 
 def test_constraint_dilated_height_range():
     # Dilated kernel height must lie within a certain range
     op = testutil.create_op_with_quant_tensors(Op.Conv2DBias, [1, 8, 8, 8], [1, 8, 8, 8], weights_shape=[65, 64, 1, 1])
@@ -608,17 +611,34 @@
     elif type(axis) is int:
         indices = create_const_tensor("indices", [], DataType.int32, axis)
     op = testutil.create_op(Op.Mean, [ifm, indices], ofm, attrs)
     return op
 
 
 def test_mean_hw_product():
-    op = create_mean([1, 64, 64, 16], [1, 16], [1, 2], DataType.uint8, {})
+    # max kernel size checks
+    op = create_mean([1, 4096, 4096, 16], [1, 1, 1, 16], [1, 2], DataType.int8, {})
+    assert support.is_operator_supported(op)
+    op = create_mean([1, 4097, 4096, 16], [1, 1, 1, 16], [1, 2], DataType.int8, {})
+    assert not support.is_operator_supported(op)
+
+    op = create_mean([1, 2048, 4096, 16], [1, 1, 1, 16], [1, 2], DataType.uint8, {})
+    assert support.is_operator_supported(op)
+    op = create_mean([1, 2049, 4096, 16], [1, 1, 1, 16], [1, 2], DataType.uint8, {})
+    assert not support.is_operator_supported(op)
+
+    op = create_mean([1, 16, 4096, 16], [1, 1, 1, 16], [1, 2], DataType.int16, {})
+    assert support.is_operator_supported(op)
+    op = create_mean([1, 17, 4096, 16], [1, 1, 1, 16], [1, 2], DataType.int16, {})
+    assert not support.is_operator_supported(op)
+
+    # h > 4096 is OK but w > 4096 is not
+    op = create_mean([1, 4097, 10, 16], [1, 1, 1, 16], [1, 2], DataType.uint8, {"keep_dims": True})
     assert support.is_operator_supported(op)
-    op = create_mean([1, 65, 64, 16], [1, 1, 1, 16], [1, 2], DataType.int8, {"keep_dims": True})
+    op = create_mean([1, 10, 4097, 16], [1, 1, 1, 16], [1, 2], DataType.int16, {"keep_dims": True})
     assert not support.is_operator_supported(op)
 
 
 def test_lstm_support():
     # Test valid configuration
     op = testutil.create_lstm_op(3, 12, 24, 20, DataType.int8)
     assert support.is_operator_supported(op)
@@ -658,7 +678,36 @@
     assert not support.is_operator_supported(op)
     op.inputs[22] = None
     op.inputs[23] = input_to_input_weights
     assert not support.is_operator_supported(op)
     op.inputs[23] = None
     # Test restored valid configuration
     assert support.is_operator_supported(op)
+
+
+def test_rsqrt_support():
+    # Test supported op (int8)
+    op = testutil.create_elemwise_op(Op.Rsqrt, "op", [1, 8, 8, 8], [1, 8, 8, 8], [1, 8, 8, 8], datatype=DataType.int8)
+    assert support.is_operator_supported(op)
+    # Test not supported op (uint8)
+    op = testutil.create_elemwise_op(Op.Rsqrt, "op", [1, 8, 8, 8], [1, 8, 8, 8], [1, 8, 8, 8], datatype=DataType.uint8)
+    assert not support.is_operator_supported(op)
+    # Test not supported op (int16)
+    op = testutil.create_elemwise_op(Op.Rsqrt, "op", [1, 8, 8, 8], [1, 8, 8, 8], [1, 8, 8, 8], datatype=DataType.int16)
+    assert not support.is_operator_supported(op)
+
+
+def test_constraint_slice_inputs_const():
+    # Begin and Size tensor cannot be non-const tensors
+    # Test not supported op
+    ifm = Tensor([3, 1, 256], DataType.int8, "in")
+    begin = Tensor([3], DataType.int32, "begin")
+    size = Tensor([3], DataType.int32, "size")
+    ofm = Tensor([1, 1, 256], DataType.int8, "size")
+    op = testutil.create_op(Op.Slice, [ifm, begin, size], ofm)
+    assert not support.is_operator_supported(op)
+    # Test supported op
+    begin = create_const_tensor("begin", [3], DataType.int32, [0, 0, 0])
+    size = create_const_tensor("size", [3], DataType.int32, [2, 1, 256])
+    op.set_input_tensor(begin, 1)
+    op.set_input_tensor(begin, 2)
+    assert support.is_operator_supported(op)
```

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/test/testutil.py` & `ethos-u-vela-3.9.0/ethosu/vela/test/testutil.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/ATan2Options.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/ATan2Options.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/AbsOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/AbsOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/AddNOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/AddNOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/AddOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/AddOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/ArgMaxOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/ArgMaxOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/ArgMinOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/ArgMinOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/AssignVariableOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/AssignVariableOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/BatchMatMulOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/BatchMatMulOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/BatchToSpaceNDOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/BatchToSpaceNDOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/BidirectionalSequenceLSTMOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/BidirectionalSequenceLSTMOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/BidirectionalSequenceRNNOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/BidirectionalSequenceRNNOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/BroadcastToOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/BroadcastToOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/BucketizeOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/BucketizeOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/Buffer.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/Buffer.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/BuiltinOperator.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/BuiltinOperator.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/BuiltinOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/BuiltinOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/CallOnceOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/CallOnceOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/CallOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/CallOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/CastOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/CastOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/ConcatEmbeddingsOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/ConcatEmbeddingsOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/ConcatenationOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/ConcatenationOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/Conv2DOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/Conv2DOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/Conv3DOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/Conv3DOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/CosOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/CosOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/CumsumOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/CumsumOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/CustomQuantization.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/CustomQuantization.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/DensifyOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/DensifyOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/DepthToSpaceOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/DepthToSpaceOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/DepthwiseConv2DOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/DepthwiseConv2DOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/DequantizeOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/DequantizeOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/DimensionMetadata.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/DimensionMetadata.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/DivOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/DivOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/DynamicUpdateSliceOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/DynamicUpdateSliceOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/EmbeddingLookupSparseOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/EmbeddingLookupSparseOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/EqualOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/EqualOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/ExpOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/ExpOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/ExpandDimsOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/ExpandDimsOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/FakeQuantOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/FakeQuantOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/FillOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/FillOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/FloorDivOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/FloorDivOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/FloorModOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/FloorModOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/FullyConnectedOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/FullyConnectedOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/GatherNdOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/GatherNdOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/GatherOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/GatherOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/GeluOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/GeluOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/GreaterEqualOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/GreaterEqualOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/GreaterOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/GreaterOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/HardSwishOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/HardSwishOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/HashtableFindOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/HashtableFindOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/HashtableImportOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/HashtableImportOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/HashtableOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/HashtableOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/HashtableSizeOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/HashtableSizeOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/IfOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/IfOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/Int32Vector.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/Int32Vector.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/L2NormOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/L2NormOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/LSHProjectionOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/LSHProjectionOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/LSTMOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/LSTMOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/LeakyReluOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/LeakyReluOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/LessEqualOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/LessEqualOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/LessOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/LessOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/LocalResponseNormalizationOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/LocalResponseNormalizationOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/LogSoftmaxOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/LogSoftmaxOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/LogicalAndOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/LogicalAndOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/LogicalNotOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/LogicalNotOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/LogicalOrOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/LogicalOrOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/MatrixDiagOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/MatrixDiagOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/MatrixSetDiagOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/MatrixSetDiagOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/MaximumMinimumOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/MaximumMinimumOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/Metadata.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/Metadata.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/MirrorPadOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/MirrorPadOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/Model.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/Model.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/MulOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/MulOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/NegOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/NegOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/NonMaxSuppressionV4Options.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/NonMaxSuppressionV4Options.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/NonMaxSuppressionV5Options.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/NonMaxSuppressionV5Options.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/NotEqualOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/NotEqualOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/OneHotOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/OneHotOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/Operator.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/Operator.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/OperatorCode.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/OperatorCode.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/PackOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/PackOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/PadOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/PadOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/PadV2Options.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/PadV2Options.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/Pool2DOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/Pool2DOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/PowOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/PowOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/QuantizationParameters.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/QuantizationParameters.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/QuantizeOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/QuantizeOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/RNNOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/RNNOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/RandomOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/RandomOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/RangeOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/RangeOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/RankOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/RankOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/ReadVariableOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/ReadVariableOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/ReducerOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/ReducerOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/ReshapeOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/ReshapeOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/ResizeBilinearOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/ResizeBilinearOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/ResizeNearestNeighborOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/ResizeNearestNeighborOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/ReverseSequenceOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/ReverseSequenceOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/ReverseV2Options.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/ReverseV2Options.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/Rfft2dOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/Rfft2dOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/SVDFOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/SVDFOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/ScatterNdOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/ScatterNdOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/SegmentSumOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/SegmentSumOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/SelectOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/SelectOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/SelectV2Options.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/SelectV2Options.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/SequenceRNNOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/SequenceRNNOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/ShapeOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/ShapeOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/SignOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/SignOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/SignatureDef.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/SignatureDef.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/SkipGramOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/SkipGramOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/SliceOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/SliceOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/SoftmaxOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/SoftmaxOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/SpaceToBatchNDOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/SpaceToBatchNDOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/SpaceToDepthOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/SpaceToDepthOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/SparseToDenseOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/SparseToDenseOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/SparsityParameters.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/SparsityParameters.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/SplitOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/SplitOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/SplitVOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/SplitVOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/SquareOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/SquareOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/SquaredDifferenceOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/SquaredDifferenceOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/SqueezeOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/SqueezeOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/StridedSliceOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/StridedSliceOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/SubGraph.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/SubGraph.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/SubOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/SubOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/Tensor.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/Tensor.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/TensorMap.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/TensorMap.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/TileOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/TileOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/TopKV2Options.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/TopKV2Options.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/TransposeConvOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/TransposeConvOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/TransposeOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/TransposeOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/Uint16Vector.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/Uint16Vector.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/Uint8Vector.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/Uint8Vector.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/UnidirectionalSequenceLSTMOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/UnidirectionalSequenceLSTMOptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -59,15 +59,22 @@
     # UnidirectionalSequenceLSTMOptions
     def AsymmetricQuantizeInputs(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(12))
         if o != 0:
             return bool(self._tab.Get(flatbuffers.number_types.BoolFlags, o + self._tab.Pos))
         return False
 
-def UnidirectionalSequenceLSTMOptionsStart(builder): builder.StartObject(5)
+    # UnidirectionalSequenceLSTMOptions
+    def DiagonalRecurrentTensors(self):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(14))
+        if o != 0:
+            return bool(self._tab.Get(flatbuffers.number_types.BoolFlags, o + self._tab.Pos))
+        return False
+
+def UnidirectionalSequenceLSTMOptionsStart(builder): builder.StartObject(6)
 def Start(builder):
     return UnidirectionalSequenceLSTMOptionsStart(builder)
 def UnidirectionalSequenceLSTMOptionsAddFusedActivationFunction(builder, fusedActivationFunction): builder.PrependInt8Slot(0, fusedActivationFunction, 0)
 def AddFusedActivationFunction(builder, fusedActivationFunction):
     return UnidirectionalSequenceLSTMOptionsAddFusedActivationFunction(builder, fusedActivationFunction)
 def UnidirectionalSequenceLSTMOptionsAddCellClip(builder, cellClip): builder.PrependFloat32Slot(1, cellClip, 0.0)
 def AddCellClip(builder, cellClip):
@@ -77,10 +84,13 @@
     return UnidirectionalSequenceLSTMOptionsAddProjClip(builder, projClip)
 def UnidirectionalSequenceLSTMOptionsAddTimeMajor(builder, timeMajor): builder.PrependBoolSlot(3, timeMajor, 0)
 def AddTimeMajor(builder, timeMajor):
     return UnidirectionalSequenceLSTMOptionsAddTimeMajor(builder, timeMajor)
 def UnidirectionalSequenceLSTMOptionsAddAsymmetricQuantizeInputs(builder, asymmetricQuantizeInputs): builder.PrependBoolSlot(4, asymmetricQuantizeInputs, 0)
 def AddAsymmetricQuantizeInputs(builder, asymmetricQuantizeInputs):
     return UnidirectionalSequenceLSTMOptionsAddAsymmetricQuantizeInputs(builder, asymmetricQuantizeInputs)
+def UnidirectionalSequenceLSTMOptionsAddDiagonalRecurrentTensors(builder, diagonalRecurrentTensors): builder.PrependBoolSlot(5, diagonalRecurrentTensors, 0)
+def AddDiagonalRecurrentTensors(builder, diagonalRecurrentTensors):
+    return UnidirectionalSequenceLSTMOptionsAddDiagonalRecurrentTensors(builder, diagonalRecurrentTensors)
 def UnidirectionalSequenceLSTMOptionsEnd(builder): return builder.EndObject()
 def End(builder):
     return UnidirectionalSequenceLSTMOptionsEnd(builder)
```

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/UniqueOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/UniqueOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/UnpackOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/UnpackOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/UnsortedSegmentMaxOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/UnsortedSegmentMaxOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/UnsortedSegmentMinOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/UnsortedSegmentMinOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/UnsortedSegmentProdOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/UnsortedSegmentProdOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/UnsortedSegmentSumOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/UnsortedSegmentSumOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/VarHandleOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/VarHandleOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/VariantSubType.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/VariantSubType.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/WhereOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/WhereOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/WhileOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/WhileOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite/ZerosLikeOptions.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite/ZerosLikeOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite_graph_optimiser.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite_graph_optimiser.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,25 +41,27 @@
 from .graph_optimiser_util import needed_total_padding
 from .graph_optimiser_util import set_ifm_ofm_op_shapes
 from .graph_optimiser_util import set_tensor_equivalence
 from .lstm import Lstm
 from .lut import convert_to_lut
 from .lut import create_lut_8bit_op
 from .lut import create_lut_int16_op
+from .lut import create_lut_rsqrt_int8_op
 from .numeric_util import clamp_sigmoid
 from .numeric_util import full_shape
 from .numeric_util import round_away_zero
 from .numeric_util import round_down_log2
 from .operation import create_activation_function
 from .operation import ExplicitScaling
 from .operation import NpuBlockType
 from .operation import Op
 from .operation import Operation
 from .operation import Padding
 from .operation import RoundingMode
+from .operation_util import create_add
 from .operation_util import create_add_nop
 from .operation_util import create_avgpool_nop
 from .operation_util import create_cast_op
 from .operation_util import create_depthwise_maxpool
 from .operation_util import create_memcpy
 from .operation_util import get_pad_values_from_input
 from .scaling import quantise_scale
@@ -68,14 +70,15 @@
 from .tensor import check_quantized_tens_scaling_equal
 from .tensor import create_const_tensor
 from .tensor import create_equivalence_id
 from .tensor import QuantizationParameters
 from .tensor import Tensor
 from .tensor import TensorPurpose
 from .tflite_mapping import optype_to_builtintype
+from .utils import calc_resize_factor
 
 passthrough_nodes = (Op.Identity,)
 
 
 def remove_passthrough_tensor(tens, arch, nng):
     if len(tens.ops) == 1 and tens.ops[0].type in passthrough_nodes:
         assert len(tens.ops[0].inputs) == 1
@@ -143,15 +146,15 @@
         new_op = Operation(Op.SplitSliceRead, split_op.name)
         new_op.inputs = [inp]
         ofm_shape_idx = 0
         if None in (offset_end, offset_start):
             read_shape = None
         else:
             # the read shape is relative to each start offset
-            read_shape = [oe - os for oe, os in zip(offset_end, offset_start)]
+            read_shape = Shape4D([oe - os for oe, os in zip(offset_end, offset_start)])
 
         # For Split the offset cannot be extracted from the tensor so it has to
         # be calculated from the index of the output tensor
         if axis is not None:
             # Get the start and end of the split
             offset_start = [0] * 4
             axis_4D_list = split_op.attrs.get("split_axis_4D", None)  # Present for UnpackReshaped and some StridedSlice
@@ -257,15 +260,15 @@
     else:
         raise UnsupportedFeatureError(f"Unsupported padding = {padding_type} for up-scaled padding calculation")
     padding = (top_pad, left_pad, bottom_pad, right_pad)
     skirt = padding
     return padding, skirt
 
 
-def fixup_conv2d_backprop(op, arch, nng):
+def fixup_conv2d_backprop(op: Operation, arch, nng) -> Operation:
     if op.type == Op.Conv2DBackpropInput:
         # flip the inputs
         op.inputs[0], op.inputs[2] = op.inputs[2], op.inputs[0]
         op.type = Op.Conv2DBackpropInputSwitchedBias
         op.ifm_resampling_mode = resampling_mode.TRANSPOSE
 
         # Update strides
@@ -448,15 +451,15 @@
     scaled_op.outputs[0].ops = [scaled_op]
     scaled_op.set_ifm_ofm_shapes()
     DebugDatabase.add_optimised(op, scaled_op)
 
     return op
 
 
-def convert_argmax_to_depthwise_conv_and_max_pool(op, arch, nng):
+def convert_argmax_to_depthwise_conv_and_max_pool(op: Operation, arch, nng) -> Operation:
     """
     Convert ArgMax to DWConv2D->MaxPool->DWConv2D, see details below.
 
     Example:
     arr = [4,   [00000100,
            6, =  00000110,  # <-- This is the largest value, so we're expecting argmax(arr) = 1
            5]    00000101]
@@ -755,15 +758,16 @@
 
     kernels = _compute_kernels(input_height, input_width, output_height, output_width)
     op = _build_convolutions(op, kernels)
 
     return op
 
 
-def fixup_resize(op, arch, nng):
+def fixup_resize(op: Operation, arch, nng) -> Operation:
+    """Fixup resize ops to increase support for ResizeNearestNeighbor cases."""
     if op.type.is_resize_op() and op.run_on_npu:
         if op.ifm_shapes[0] == op.ofm_shapes[0]:
             # Bypass the resize op which is essentially a NOP
             op.inputs = op.inputs[:1]
             op.type = Op.Identity
         elif op.ifm_shapes[0].height == 1 and op.ifm_shapes[0].width == 1:
             convert_resize_1x1_to_add(op)
@@ -780,15 +784,16 @@
         # the list comprehension should return a list with a single tensor
         # if it shouldn't, remove_passthrough_tensor will fail appropriately
         op.inputs = [i for i in op.inputs if i.shape == op.outputs[0].shape]
         op.type = Op.Identity
     return op
 
 
-def rewrite_fully_connected_input(op: Operation, arch, nng):
+def rewrite_fully_connected_input(op: Operation, arch, nng) -> Operation:
+    """Rewrite FullyConnected shape as 2D to allow it to run on NPU."""
     # If the operation already have a read shape do not modify
     # the ifm shape, since that will already be correct
     if op.type == Op.FullyConnected and not op.read_shapes[0]:
         new_shape = op.ifm.get_shape_as_2d(op.weights.shape[-2])
         assert new_shape is not None, "Tensor can not be reshaped to 2D"
         op.ifm_shapes[0] = new_shape
 
@@ -796,15 +801,16 @@
             # If IFM is batching then also make sure OFM is batching
             h, w = op.ofm_shapes[0].height, op.ofm_shapes[0].width
             op.ofm_shapes[0] = Shape4D([h * w, 1, 1, op.ofm_shapes[0].depth])
 
     return op
 
 
-def convert_batched_fc_shape(op, arch, nng):
+def convert_batched_fc_shape(op: Operation, arch, nng) -> Operation:
+    """Convert batched FullyConnected op shape to allow for support on NPU."""
     if op.type == Op.FullyConnected:
         # Check if the first dimension indicates batching
         if op.ifm_shapes[0].batch > 1:
             batching_split = {4: (2, 2), 8: (2, 4), 16: (4, 4)}
             n = op.ifm_shapes[0].batch
             h, w = batching_split.get(n, (1, n))
             op.ifm_shapes[0] = Shape4D([1, h, w, op.ifm_shapes[0].depth])
@@ -933,25 +939,76 @@
 
             op.attrs["explicit_padding"] = padding
             op.attrs["skirt"] = skirt
 
     return op
 
 
-def reorder_depthwise_weights(op, arch, nng):
+def reorder_depthwise_weights(op: Operation, arch, nng) -> Operation:
     if op.type.is_depthwise_conv2d_op():
         weight_tensor = op.inputs[1]
-        weight_tensor.values = np.transpose(weight_tensor.values, (0, 1, 3, 2))
-        weight_tensor.set_all_shapes(list(weight_tensor.values.shape))
-        weight_tensor.weight_transpose_depthwise = True
+        if not weight_tensor.weight_transpose_depthwise:
+            weight_tensor.values = np.transpose(weight_tensor.values, (0, 1, 3, 2))
+            weight_tensor.set_all_shapes(list(weight_tensor.values.shape))
+            weight_tensor.weight_transpose_depthwise = True
+
+    return op
+
+
+def convert_avg_pool_to_conv2d(op: Operation, arch, nng) -> Operation:
+    """Convert strided Average Pools with stride >= 4 to Conv2D."""
+    if op.type != Op.AvgPool:
+        return op
 
+    stride_x, stride_y = op.get_kernel_stride()
+    # For strides <= 3 no optimization is needed
+    if stride_x <= 3:
+        return op
+    h, w = op.attrs["filter_height"], op.attrs["filter_width"]
+    inputs = op.inputs[0]
+    shape = inputs.shape
+
+    # Set necessary conv2d attributes
+    op.attrs.update(
+        {
+            "stride_h": stride_y,
+            "stride_w": stride_x,
+            "dilation_h_factor": 1,
+            "dilation_w_factor": 1,
+            "strides": (1, stride_y, stride_x, 1),
+            "dilation": (1, 1, 1, 1),
+        }
+    )
+
+    # Change op type
+    op.type = Op.Conv2DBias
+    op.name += "_conv2d"
+
+    op.rounding_mode = RoundingMode.AwayZero
+    shape = [h, w, 1, op.ofm.shape[-1]]
+    weights = np.full(shape, 1)
+    quant = QuantizationParameters(scale_f32=1 / (h * w), zero_point=0)
+    # Add unit weight tensor
+    op.add_input_tensor(
+        create_const_tensor(
+            "weights",
+            shape,
+            inputs.dtype,
+            weights,
+            quantization=quant,
+        ),
+    )
+    op.weights.values = np.reshape(op.inputs[1].values, shape)
+
+    # Set IFM/OFM shapes after changing op type
+    op.set_ifm_ofm_shapes()
     return op
 
 
-def fixup_strided_conv(op: Operation, arch, nng) -> Operation:
+def fixup_strided_conv(op: Operation, arch, nng):
     """Optimize or fixup strided Conv2DBias
     Optimization:
         Reduce, when possible, the Conv2DBias stride from N with 1 > N > 4 to 1
         by re-shaping both IFM and filter.
 
     Fixup:
         Introduce software support for Conv2DBias with stride_width > 4 by
@@ -965,45 +1022,23 @@
     ifm_shape = op.ifm_shapes[0]
 
     # Do not optimize if op is not the first in the network and stride is
     # supported by the hardware
     if op.op_index != 0 and stride_x < 4:
         return op
 
-    def calc_resize_factor(ifm_width: int, stride_x: int) -> tuple[int, int]:
-        """Compute resize factor for strided Conv2D optimization"""
-        # Define strides that are supported by HW
-        hw_supported_strides = (2, 3)
-        resize_factor = stride_x
-
-        if ifm_width % resize_factor != 0:
-            # In case it is not divisible, check if the resize factor is
-            # divisible by any of the hw_supported_strides. If it is, re-compute
-            # the resize factor to be the value that leads us to
-            # reach a hw supported stride.
-            # E.g.: IFM width = 133, stride = 14, filter width = 7 can be
-            #       optimised to IFM width = 19, stride = 2, filter width = 7 using
-            #       a resize factor of 7. The final stride is 2 which is
-            #       supported by the hardware.
-            supported_final_strides = (x for x in hw_supported_strides if resize_factor % x == 0)
-            new_resize_factor = resize_factor // next(supported_final_strides, 1)
-            resize_factor = new_resize_factor if resize_factor != new_resize_factor else 1
-
-        optimised_stride = stride_x // resize_factor
-
-        return resize_factor, optimised_stride
-
     resize_factor, final_stride = calc_resize_factor(ifm_shape.width, stride_x)
 
     def calc_filter_padding(
         ifm_padding_type: Padding | None,
         ifm_current_padding_x: int,
         post_op_stride: int,
         opt_resize_factor: int,
         filter_width: int,
+        ifm_width: int,
     ) -> tuple[int, int, int, int]:
         """Calculate zero padding to be added to the filter.
 
         Parameters
         ----------
         ifm_padding_type : Padding or None
             The padding type that is applied to the IFM.
@@ -1013,32 +1048,59 @@
             The final stride once optimization is performed.
         opt_resize_factor : int
             The factor by which the stride will be reduced.
             E.g. opt_resize_factor = 2 on a stride of 4 will produce
             a stride of 2 after the optimization
         filter_width : int
             Width of the filter before optimization.
+        ifm_width : int
+            Width of the IFM before optimization
 
         Returns
         -------
         padding : tuple[int, int, int, int]
             A tuple with the ammount of padding on each side (top, left, bottom, right)
         """
         padding_size = 0
         padding = (0, 0, 0, 0)
         if ifm_padding_type and ifm_padding_type != Padding.VALID:
-            padding_size = (ifm_current_padding_x + post_op_stride) * opt_resize_factor - filter_width
-            # Distribute padding between left and right side of the filter
-            padding_left = padding_size // 2
+            # Compute padding size for the filter that guarantees that HW padding added to IFM matches
+            # before and after the optimization is performed
+            expected_filter_size = 0
+            pre_opt_stride = post_op_stride * opt_resize_factor
+            post_opt_ifm_width = ifm_width // opt_resize_factor
+            # Compute the total expected filter size post optimization that ensures that the same HW padding
+            # is added to IFM.
+            # There are two ways of calculating required filter size depending on whether IFM width is divisible
+            # by stride width or not. These approaches match the cases used to calculate HW padding in
+            # needed_total_padding method.
+            if ifm_width % pre_opt_stride == 0:
+                expected_filter_size = ifm_current_padding_x + post_op_stride
+            else:
+                expected_filter_size = ifm_current_padding_x + (post_opt_ifm_width % post_op_stride)
+            # Compute padding size from expected filter size
+            padding_size = expected_filter_size * opt_resize_factor - filter_width
+
+            if ifm_current_padding_x == 0:
+                # If no HW padding is added to IFM, divide filter padding between left and right following
+                # the same strategy as the reference.
+                padding_left = padding_size // 2
+            else:
+                # If HW padding is added to IFM, split padding for the filter so that left padding and right padding
+                # are proportional to left and right HW padding.
+                left_hw_padding = ifm_current_padding_x // 2
+                # Compute filter padding
+                padding_left = padding_size // ifm_current_padding_x * left_hw_padding
             padding = (0, padding_left, 0, padding_size - padding_left)
 
         # Check if filter width is divisible by the stride width (required for optimization)
-        # If padding was already added above, the filter width is already divisible by
-        # resize factor, so this should be skipped.
-        if padding_size == 0 and filter_width % opt_resize_factor != 0:
+        # If filter width is not divisible by stride width and no HW padding is added to IFM, compute
+        # filter padding required for the filter width to be divisible by the stride width and apply it as right
+        # padding.
+        if filter_width % opt_resize_factor != 0 and (padding_size == 0 or ifm_current_padding_x == 0):
             padding_size = opt_resize_factor - (filter_width % opt_resize_factor)
             # Add padding zeros to the right
             padding = (0, 0, 0, padding_size)
 
         return padding
 
     # Compute the depth of the IFM once the strided Conv2D is optimised
@@ -1051,15 +1113,15 @@
         padding_type = op.attrs.get("padding", None)
         if padding_type in (None, Padding.EXPLICIT, Padding.TILE):
             return op
         # Compute current padding as if IFM padding is SAME
         curr_padding_x = needed_total_padding(ifm_shape.width, stride_x, k_w)
         # Compute the padding needed on the filter for the optimisation
         _, left_filter_padding, _, right_filter_padding = calc_filter_padding(
-            padding_type, curr_padding_x, final_stride, resize_factor, k_w
+            padding_type, curr_padding_x, final_stride, resize_factor, k_w, ifm_shape.width
         )
         total_horizontal_padding = left_filter_padding + right_filter_padding
         # If IFM padding is enabled, check if pre-opt and post-opt padding is
         # the same while taking into consideration the extra filter padding.
         if padding_type == Padding.SAME:
             optimised_padding_x = needed_total_padding(
                 ifm_shape.width // resize_factor, final_stride, (k_w + 1 + total_horizontal_padding) // resize_factor
@@ -1096,18 +1158,19 @@
         # Strides
         stride_x = final_stride
         op.attrs.update({"stride_w": stride_x, "stride_h": stride_y, "strides": (1, stride_y, stride_x, 1)})
 
     return op
 
 
-def convert_conv_to_fc(op, arch, nng):
+def convert_conv_to_fc(op: Operation, arch, nng) -> Operation:
+    """Convert 1x1 Conv2D that behave like FullyConnected to FullyConnected, since they don't need any weight
+    buffering.
+    """
     # Conv 1x1 can be equivalent to Fully Connected.
-    # By representing certain convs as fully connected layers, Vela can better determine wether or not to use
-    # caching/double buffering for the weights.
     # (Weights dont need to be reloaded for convs when IFM H and W are 1)
     if op.type == Op.Conv2DBias:
         h = op.ifm_shapes[0].height
         w = op.ifm_shapes[0].width
         kh, kw, _, _ = op.inputs[1].shape
         if h == 1 and w == 1 and kh == 1 and kw == 1:
             # Overwrite this op as a Fully Connected Op
@@ -1121,15 +1184,16 @@
             weight_tensor.values = weight_tensor.values.squeeze(axis=(0, 1))
             weight_tensor.set_all_shapes(list(weight_tensor.values.shape))
 
             DebugDatabase.add_optimised(op, op)
     return op
 
 
-def fixup_relus_with_differing_ifm_ofm_scaling(op, arch, nng):
+def fixup_relus_with_differing_ifm_ofm_scaling(op: Operation, arch, nng) -> Operation:
+    """Fixup Relu with different IFM and OFM to allow fusing by adding its own primary op."""
     if op.run_on_npu and op.type.is_relu_op():
         ifm = op.inputs[0]
         ofm = op.outputs[0]
         # Relu with differing IFM and OFM scaling cannot be fused with another primary op
         # and requires its own to be inserted
         if not check_quantized_tens_scaling_equal(ifm, ofm):
             # Override this op with its own primary op (avgpool)
@@ -1146,29 +1210,32 @@
             relu_fused_op.add_input_tensor(ifm)
             relu_fused_op.set_output_tensor(ofm)
             relu_fused_op.set_ifm_ofm_shapes()
             op = relu_fused_op
     return op
 
 
-def convert_lstm(op, arch, nng):
+def convert_lstm(op: Operation, arch, nng) -> Operation:
+    """Convert LSTM op into its basic opearations to allow for support on NPU."""
     if op.type == Op.UnidirectionalSequenceLstm:
         lstm = Lstm(op)
         op = lstm.get_graph()
     return op
 
 
-def convert_softmax(op, arch, nng):
+def convert_softmax(op: Operation, arch, nng) -> Operation:
+    """Convert Softmax op into its basic operations to allow for support on NPU."""
     if op.type == Op.Softmax and op.run_on_npu:
         softmax = SoftMax(op)
         op = softmax.get_graph()
     return op
 
 
-def convert_prelu(op, arch, nng):
+def convert_prelu(op: Operation, arch, nng) -> Operation:
+    """Convert PReLU op to other ops based on alpha values to allow for support on NPU."""
     if op.type == Op.Prelu:
         ifm, alpha, ofm = op.get_ifm_ifm2_ofm()
         if None in (ifm, alpha, ofm):
             return op
 
         if alpha.values is not None:
             # If const alpha check for possible optimisations
@@ -1277,15 +1344,15 @@
         DebugDatabase.add_optimised(op, add_op)
         ifm.consumer_list.remove(op)
         op = add_op
 
     return op
 
 
-def convert_mul_max_to_abs_or_lrelu(op, arch, nng):
+def convert_mul_max_to_abs_or_lrelu(op: Operation, arch, nng) -> Operation:
     r"""Whenever there is a subgraph with this topology:
 
     Input    X   For X = -1 or X > 0
     |   \   /    This subgraph can be replaced with either
     |    Mul     an Abs (if X = -1) or a LeakyReLU (if X > 0)
     |   /
     Max
@@ -1369,15 +1436,16 @@
 
         # Record optimisation in debug database
         DebugDatabase.add_optimised(op, op)
 
     return op
 
 
-def convert_hardswish_to_lut(op, arch, nng):
+def convert_hardswish_to_lut(op: Operation, arch, nng) -> Operation:
+    """Convert HardSwish to LUT to allow for support on NPU."""
     if op.type == Op.HardSwish:
         ifm, ofm = op.get_ifm_ofm()
         # Generate the LUT
         ifm_scale = np.double(ifm.quantization.scale_f32)
         ofm_scale = np.double(ofm.quantization.scale_f32)
         zp_in = ifm.quantization.zero_point
         zp_out = ofm.quantization.zero_point
@@ -1582,16 +1650,16 @@
         else:
             lut_result = zp_out + fp_math.multiply_by_quantized_multiplier(x - zp_in, identity_scale, identity_shift)
         lut_result = min(quantized_max, max(quantized_min, lut_result))
         values.append(lut_result)
     return convert_to_lut(op, values, "lrelu")
 
 
-def convert_lrelu(op, arch, nng):
-    # Converts LeakyRelu to a LUT based solution if possible, otherwise a mul + max
+def convert_lrelu(op: Operation, arch, nng) -> Operation:
+    """Convert LeakyRelu to a LUT based solution if possible, otherwise a mul + max."""
     if op.type != Op.LeakyRelu:
         return op
     ifm, ofm = op.get_ifm_ofm()
     if ifm is None or ofm is None:
         return op
     alpha = op.attrs["alpha"]
     if alpha == 0:
@@ -1604,16 +1672,16 @@
         return convert_lrelu_to_lut(op, arch)
     if check_quantized_tens_scaling_equal(ifm, ofm) and ifm.dtype == ofm.dtype == DataType.int16 and alpha > 0:
         # use LeakyRelu unmodified for int16 with equal input/output scaling and positive alpha
         return op
     return convert_lrelu_to_mul_max(op, arch)
 
 
-def convert_tanh_sigmoid_to_lut(op, arch, nng):
-    # Converts int8/uint8 Sigmoid and Tanh to a LUT based solution
+def convert_tanh_sigmoid_to_lut(op: Operation, arch, nng) -> Operation:
+    """Convert int8/uint8 Sigmoid and Tanh to a LUT based solution."""
     if op.type == Op.Sigmoid:
         return convert_to_lut8(op, clamp_sigmoid, "sigmoid")
     elif op.type == Op.Tanh:
         return convert_to_lut8(op, math.tanh, "tanh")
     return op
 
 
@@ -1654,15 +1722,15 @@
 def _leading_pad_ok(leading_pad, stride, kernel_size):
     # If kernel size // 2 > stride, then (left, top) padding must be a multiple of stride,
     # otherwise replacing PAD by hardware padding would iterate the wrong IFM rows/columns
     max_size = kernel_size // 2
     return leading_pad == max_size or max_size <= stride or leading_pad % stride == 0
 
 
-def replace_pad_by_hw_pad(op: Operation, arch, nng):
+def replace_pad_by_hw_pad(op: Operation, arch, nng) -> Operation:
     """
     Tries to completely remove a PAD operator by using hardware padding.
     E.g. a PAD operation that pads 1, followed by a CONV with VALID padding and kernel size 3
     is rewritten such that the PAD is removed, and the CONV uses SAME padding.
     Converts tens1 -> PAD -> tens2 -> CONV to tens1 -> CONV
     if both operations can be run on the NPU.
     This is the most efficient way to implement PAD, but cannot be done for all pad sizes.
@@ -1826,15 +1894,16 @@
             op, op.name + "_right", zero_tens, shape, shp_top.with_width(ofm_shape.width - right)
         )
 
     op.type = Op.ConcatTFLite
     return avgpool_op
 
 
-def fixup_bias_tensors(op, arch, nng, dtype=None):
+def fixup_bias_tensors(op: Operation, arch, nng, dtype=None) -> Operation:
+    """Fixup ops that require a bias and don't have one by adding a bias tensor filled with zeros."""
     if op.type.needs_bias() and op.bias is None:
         # Op has no bias, add bias tensor filled with zeros
         nr_biases = op.inputs[1].shape[-1]
         bias_values = [0] * nr_biases
         # The DataType of the bias tensor can be explicitly provided or deduced from the ifm
         # DataType. Default is int32 bias for 8-bit ifms and int64 for int16 ifms.
         # For int16 the selected bias DataType will have an impact on the scaling
@@ -1842,30 +1911,34 @@
         # refence with reduced scaling for int64 bias.
         # This means that in cases (in the graph optimiser) where DepthwiseConv2DBias
         # is used to emulate average pool int32 bias should be selected for full precision
         # int16 scaling.
         if dtype is None:
             dtype = DataType.int64 if op.ifm.dtype == DataType.int16 else DataType.int32
         bias_tensor = create_const_tensor(op.name + "_bias", [nr_biases], dtype, bias_values)
-        op.set_input_tensor(bias_tensor, op.type.info.indices.biases[0])
+        bias_index = op.type.info.indices.biases[0]
+        if bias_index < len(op.inputs):
+            op.set_input_tensor(bias_tensor, bias_index)
+        else:
+            op.add_input_tensor(bias_tensor)
 
     return op
 
 
 def detect_asymmetric_weights(op):
     # Check all ops (cpu and npu)
     if op.type.is_conv2d_op() or op.type.is_depthwise_conv2d_op():
         if op.ifm.dtype in (DataType.int8, DataType.int16):
             if not np.all(op.weights.quantization.zero_point == 0):
                 print(f"Warning: Op {op.type} '{op.name}' has asymmetric weights.", end=" ")
                 return True
     return False
 
 
-def fixup_asymmetric_weights(op, arch, nng):
+def fixup_asymmetric_weights(op: Operation, arch, nng) -> Operation:
     if detect_asymmetric_weights(op):
         if op.run_on_npu:
             print("Zero points have been adjusted.")
             op.weights.quantization.zero_point *= 0
     return op
 
 
@@ -1884,131 +1957,220 @@
     if force_symmetric_int_weights:
         return fixup_asymmetric_weights
     else:
         return check_asymmetric_weights
 
 
 def convert_mean_to_depthwise_conv(op, arch, nng):
+    """
+    When h x w <= 4096     When h x w > 4096 there is a need to split into several ops.
+                           Do this by splitting up h and change the read_offset/shape.
+                           Below is an example where ifm is 1x190x64x1
+           MEAN                                           MEAN
+             |                      |-----------------------|----------------------|
+    DepthwiseConv2DBias    1_DepthwiseConv2DBias   2_DepthwiseConv2DBias   3_DepthwiseConv2DBias
+             |                      |                       |                     |
+            MUL                     |---------ADD-----------|                     |
+                                               |                                  |
+                                               |----------------ADD---------------|
+                                                                 |
+                                                                MUL
+               1_DepthwiseConv2DBias: read_offset [0, 0, 0, 0]> read_shape [1,  64, 64, 1]>
+               2_DepthwiseConv2DBias: read_offset [0, 64, 0, 0]> read_shape [1,  64, 64, 1]>
+               3_DepthwiseConv2DBias: read_offset [0, 128, 0, 0]> read_shape [1,  62, 64, 1]>
+    """
     if op.type == Op.Mean and op.run_on_npu:
+        max_kernel_size = 4096
+        max_height = 64
         inp, axis = op.inputs
-        shape = inp.shape
-        ofm_shape = op.ofm.shape
-        dims = len(shape)
-        dims_ofm = len(ofm_shape)
-
-        # Height and width axes have different index depending on dimensions
-        if axis.shape == [] or axis.shape[0] == 1:  # single axis
-            axis = int(axis.values) if len(axis.shape) == 0 else int(axis.values[0])
-            if dims in (2, 3):
-                # If dims is 2 or 3, axis 0 refers to h-dimension
-                h, w = (shape[axis], 1) if axis == 0 else (1, shape[axis])
-            else:
-                # If dims is 4, axis 1 refers to h-dimension
-                h, w = (shape[axis], 1) if axis == 1 else (1, shape[axis])
-        else:  # multiple axes
-            axis = sorted(axis.values)
-            h, w = [shape[i] for i in axis]
-
-        # Set necessary depthwise attributes
-        op.attrs.update(
-            {
-                "padding": Padding.VALID,
-                "stride_h": 1,
-                "stride_w": 1,
-                "strides": (1, 1, 1, 1),
-                "depth_multiplier": 1,
-                "channel_multiplier": 1,
-                "dilation_h_factor": 1,
-                "dilation_w_factor": 1,
-                "dilation": (1, 1, 1, 1),
-            }
-        )
-        # Change op type
-        op.type = Op.DepthwiseConv2DBias
-        # Set IFM/OFM shapes after changing op type
-        op.set_ifm_ofm_shapes()
-
-        # Change dimensions to 4
-        def extend_dims(dim, in_shape):
-            if dim < 4:
-                in_shape = [1] + in_shape
-                if dim == 2:
-                    in_shape += [1]
-            return in_shape
-
-        if dims < 4 or dims_ofm < 4:
-            # Fix the ofm dimension when keep_dims is false
-            # e.g. IFM=1xHxWxC axis=2 OFM=1xHxC, the ofm_shape should be 1xHx1xC, not 1x1xHxC
-            if isinstance(axis, int) and dims_ofm + 1 == dims:
-                ofm_shape.insert(axis, 1)
-            elif isinstance(axis, list) and (dims_ofm + len(axis) == dims):
-                for i in axis:
-                    ofm_shape.insert(i, 1)
-            shape = extend_dims(dims, shape)
-            dims_ofm = len(ofm_shape)
-            ofm_shape = extend_dims(dims_ofm, ofm_shape)
-            op.set_ifm_ofm_shapes()
-
-        # If height is greater than max kernel height, reshape from HxW to 1x(HxW)
-        if h > 64:
-            # This can only happen and be done for multiple axes, and
-            # h * w <= 4096 for DepthwiseConv2DBias
-            # which is checked in supported ops
-            shape = [shape[0], 1, h * w, shape[3]]
-            op.ifm_shapes[0] = Shape4D(shape)
-            weight_shape = [1, h * w, shape[3], shape[0]]
+        dims = len(inp.shape)
+        dims_ofm = len(op.ofm.shape)
+        ofmq = op.ofm.quantization
+        ifmq = op.ifm.quantization
+
+        # reduce_axis[i] is true if axis i should be reduced
+        if axis.shape == []:
+            reduce_axis = [True if i == axis.values else False for i in range(dims)]
         else:
-            # Set weight shape to [H,W,C,B]
-            weight_shape = [h, w, shape[3], shape[0]]
+            reduce_axis = [True if i in axis.values else False for i in range(dims)]
 
-        op.rounding_mode = RoundingMode.HalfUp
-        identity_quant = QuantizationParameters(scale_f32=1.0, zero_point=0)
-        op.forced_input_quantization = identity_quant
-        op.forced_output_quantization = identity_quant
+        ifm_shape = inp.shape.copy()
+        intermediate_shape = op.ofm.shape.copy()
 
-        # Add unit weight tensor
-        op.set_input_tensor(
-            create_const_tensor(
-                "weights",
-                weight_shape,
-                inp.dtype,
-                np.ones(weight_shape),
-                quantization=identity_quant,
-            ),
-            1,
-        )
-        op.weights.values = np.reshape(op.inputs[1].values, weight_shape)
+        # Fix intermediate_shape when keep_dims is false
+        # e.g. IFM=1xHxWxC axis=2 OFM=1xHxC, the intermediate_shape should be 1xHx1xC
+        if dims_ofm < dims:
+            for i in range(dims):
+                if reduce_axis[i]:
+                    intermediate_shape.insert(i, 1)
+
+        # Reshape to 4D
+        reduce_axis = full_shape(4, reduce_axis, False)
+        ifm_shape = full_shape(4, ifm_shape, 1)
+        intermediate_shape = full_shape(4, intermediate_shape, 1)
+
+        # If all dimensions to reduce have shape 1, the operation is essentially a memcpy.
+        # We can then remove the whole op by propagating ofm to previous ops
+        if not any([reduce_axis[i] and ifm_shape[i] > 1 for i in range(4)]):
+            op.type = Op.Memcpy
+            op = bypass_memory_only_ops(op, arch, nng)
+            return op
 
-        # Input zero point is adjusted after the sum calculation, so we emulate that with a bias
-        ofmq, ifmq = op.ofm.quantization, inp.quantization
-        bias = -ifmq.zero_point * h * w
-        bias_shape = [shape[-1]]
-        op.inputs.append(create_const_tensor(op.name + "_bias", bias_shape, DataType.int32, np.ones(bias_shape) * bias))
-        DebugDatabase.add_optimised(op, op)
+        # Support mean over depth-axis by left-shifting the C channel
+        # From semantics checks we can assume that one of H,W,C has shape 1
+        if reduce_axis[3] and ifm_shape[3] > 1:
+            assert 1 in ifm_shape[1:], "Mean reduction over depth channel, but none of H,W,C has shape 1"
+            # If W=1 reshape NxHx1xC -> NxHxCx1, else reshape Nx1xWxC -> NxWxCx1
+            idx_to_del = 2 if ifm_shape[2] == 1 else 1
+
+            # Delete axis with size 1
+            del reduce_axis[idx_to_del]
+            del ifm_shape[idx_to_del]
+            del intermediate_shape[idx_to_del]
+
+            # Add another element to set channel-axis to one
+            reduce_axis.append(False)
+            ifm_shape.append(1)
+            intermediate_shape.append(1)
+
+        # Compute kernel sizes for our convolutions
+        # Batch axis is implicit as it is only supported if batch size is 1.
+        h = ifm_shape[1] if reduce_axis[1] else 1
+        w = ifm_shape[2] if reduce_axis[2] else 1
+
+        num_elements_in_axis = h * w
+
+        # If one convolution is enough, but height is greater than max kernel height
+        # reshape from HxW to 1x(HxW)
+        # This can only be done if the mean is computed over both H and W
+        if h > max_height and num_elements_in_axis <= max_kernel_size and reduce_axis[1] and reduce_axis[2]:
+            ifm_shape = [ifm_shape[0], 1, h * w, ifm_shape[3]]
+            w = h * w
+            h = 1
+
+        intermediate_op = None
+        height_per_conv = min(max_kernel_size // w, h)
+        height_per_conv = min(height_per_conv, max_height)
+        num_convs = math.ceil(h / height_per_conv)
+        convs = list()
+
+        for i in range(num_convs):
+            is_last_op = i == (num_convs - 1)
+
+            intermediate_op = op.clone(f"{op.name}_conv_{i}")
+
+            intermediate_op.type = Op.DepthwiseConv2DBias
+
+            # Set necessary depthwise attributes
+            intermediate_op.attrs.update(
+                {
+                    "padding": Padding.VALID,
+                    "stride_h": 1,
+                    "stride_w": 1,
+                    "strides": (1, 1, 1, 1),
+                    "depth_multiplier": 1,
+                    "channel_multiplier": 1,
+                    "dilation_h_factor": 1,
+                    "dilation_w_factor": 1,
+                    "dilation": (1, 1, 1, 1),
+                }
+            )
 
-        # Create intermediate tensor between depthwise conv and mul
-        intermediate = op.ofm.clone(suffix="_intermediate", set_unique=True)
-        intermediate.dtype = DataType.int32
-
-        # Multiply sum with 1/num_elements_in_axis to get the mean
-        mul_op = Operation(Op.Mul, op.name + "_mul")
-        mul_op.add_input_tensor(intermediate)
-        mul_op.set_output_tensor(op.ofm)
-        mul_op.forced_input_quantization = identity_quant
+            b, _, _, c = ifm_shape
 
-        # Set dw conv output to the intermediate tensor
-        op.set_output_tensor(intermediate)
+            intermediate_tensor = op.ofm.clone(suffix=f"_conv_sum_{i}", set_unique=True)
+            intermediate_tensor.dtype = DataType.int32
+            intermediate_tensor.shape = intermediate_shape
+            intermediate_op.set_output_tensor(intermediate_tensor)
+
+            # as we have several convs, scaling/rounding must be done after the sum has been calculated
+            intermediate_op.explicit_scaling = ExplicitScaling(False, shift=[0], multiplier=[1])
+
+            # compute height for the kernel
+            if is_last_op and h % height_per_conv != 0:
+                weight_h = h % height_per_conv
+            else:
+                weight_h = height_per_conv
 
-        # Move activation from original op to mean op
-        mul_op.activation = op.activation
-        op.activation = None
+            # compute ifm read offset and shape for the convolution
+            read_shape_h = weight_h if reduce_axis[1] else ifm_shape[1]
+            read_shape_w = w if reduce_axis[2] else ifm_shape[2]
+
+            intermediate_op.read_offsets[0] = Shape4D([0, i * height_per_conv, 0, 0])
+            intermediate_op.read_shapes[0] = Shape4D(ifm_shape).with_hw(read_shape_h, read_shape_w)
+
+            weight_quant = QuantizationParameters(0, 255, scale_f32=1.0, zero_point=0)
+            weight_shape = [weight_h, w, c, b]
+            weight_tensor = create_const_tensor(
+                f"{intermediate_op.name}_weights",
+                weight_shape,
+                DataType.uint8,
+                np.ones(weight_shape),
+                TensorPurpose.Weights,
+                quantization=weight_quant,
+            )
+
+            weights_1D = np.ones(np.prod(weight_shape))
+            weight_tensor.equivalence_id = create_equivalence_id(tuple(weights_1D))
+            weight_tensor.value_id = weight_tensor.equivalence_id
+
+            intermediate_op.set_input_tensor(weight_tensor, 1)
+
+            dtype = DataType.int64 if intermediate_op.ifm.dtype == DataType.int16 else DataType.int32
+            bias_values = [0] * c
+            bias = create_const_tensor(f"{intermediate_op.name}_bias", [c], dtype, bias_values)
+            bias.equivalence_id = create_equivalence_id(tuple(bias_values))
+            bias.value_id = bias.equivalence_id
+            intermediate_op.inputs.append(bias)
+            intermediate_op.set_ifm_ofm_shapes()
+
+            # We want to avoid reshaping the ifm tensor directly, to not affect other ops
+            # so we update the shape explicitly for this operation
+            intermediate_op.ifm_shapes[0] = Shape4D(ifm_shape)
+
+            convs.append(intermediate_op)
+            DebugDatabase.add_optimised(op, intermediate_op)
+
+        # If we have more than one convolution
+        # We use add operations to accumulate the intermediate tensors
+        if len(convs) > 1:
+            prev_add_op = None
+            idx = 0
+
+            while len(convs):
+                intermediate_tensor = op.ofm.clone(suffix=f"_add_sum_{idx}", set_unique=True)
+                intermediate_tensor.dtype = DataType.int32
+                intermediate_tensor.shape = intermediate_shape
+
+                one_scale_quant = QuantizationParameters(scale_f32=1.0, zero_point=0)
+
+                ifm = convs.pop().ofm
+                if not prev_add_op:
+                    ifm2 = convs.pop().ofm
+                else:
+                    ifm2 = prev_add_op.ofm
+                intermediate_op = create_add(f"{op.name}_add_{idx}", ifm, ifm2, one_scale_quant)
+                intermediate_op.explicit_scaling = ExplicitScaling(False, shift=[0], multiplier=[1])
+                intermediate_op.set_output_tensor(intermediate_tensor)
+                intermediate_op.set_ifm_ofm_shapes()
+
+                prev_add_op = intermediate_op
+                idx += 1
+
+                DebugDatabase.add_optimised(op, intermediate_op)
+
+        # Convert the original mean op to our final Mul operation
+        # Which scales and divides by num_elements_in_axis
+        op.type = Op.Mul
+        op.name = f"{op.name}_mul"
+        op.attrs = {}
+        op.set_input_tensor(intermediate_op.ofm, 0)
 
         # The multiplier is calculated in the same way as in the reference,
         # clamping the shift value at the price of some precision loss.
-        num_elements_in_axis = int(h * w)
         output_multiplier, output_shift_vela = quantise_scale(np.double(ifmq.scale_f32) / np.double(ofmq.scale_f32))
 
         # Convert to reference representation shift value
         output_shift = 31 - output_shift_vela
 
         # Reference calculation
         # round_down_log2 same as 63 - CountLeadingZeros(num_elements_in_axis)
@@ -2019,39 +2181,45 @@
         output_shift = output_shift - shift
 
         # Convert to vela representation shift
         output_shift_vela = 31 - output_shift
 
         # For int32 scaling is not supported so instead multiply with the scale
         # intermediate * scale -> round and shift.
+        identity_quant = QuantizationParameters(scale_f32=1.0, zero_point=0)
         scalar = create_const_tensor(
             op.name + "_scalar", [1, 1, 1, 1], DataType.int32, [output_multiplier], quantization=identity_quant
         )
-        mul_op.add_input_tensor(scalar)
-        mul_op.set_ifm_ofm_shapes()
+        op.set_input_tensor(scalar, 1)
+        op.set_ifm_ofm_shapes()
+        op.ofm_shapes[0] = Shape4D(intermediate_shape)
 
         # Reference using TFL rounding for the multiply
-        mul_op.rounding_mode = RoundingMode.TFLite
+        op.rounding_mode = RoundingMode.TFLite
 
         # Need to use explicit scaling to get the wanted shift
-        mul_op.explicit_scaling = ExplicitScaling(False, [output_shift_vela], [1])
-        DebugDatabase.add_optimised(op, mul_op)
+        op.explicit_scaling = ExplicitScaling(False, [output_shift_vela], [1])
+        DebugDatabase.add_optimised(op, op)
     return op
 
 
-def convert_ops_to_lut(op, arch, nng):
+def convert_ops_to_lut(op: Operation, arch, nng) -> Operation:
+    """Convert Exp to 8bit or 16bit LUT to allow for support on NPU."""
     if op.type == Op.Exp:
         if op.ifm.dtype == DataType.int8:
             return create_lut_8bit_op(op, math.exp, "exp")
         elif op.ifm.dtype == DataType.int16:
             return create_lut_int16_op(op, math.exp, "exp")
         else:
             # Should already be catched in tflite supported ops
             assert False, f"Unsupported data type {op.ifm.dtype} for {op.type}"
 
+    if op.type == Op.Rsqrt:
+        return create_lut_rsqrt_int8_op(op)
+
     return op
 
 
 def optimise_quantize(op: Operation, arch, nng):
 
     if op.type == Op.Quantize and op.run_on_npu:
 
@@ -2141,15 +2309,16 @@
 
         # Add size calculation to shape output tensors
         ofm.values = np.array(ifm.shape)
 
     return op
 
 
-def fixup_dilation_gt2(op, arch, nng):
+def fixup_dilation_gt2(op: Operation, arch, nng) -> Operation:
+    """Fixup Conv2DBias and DepthwiseConv2DBias to allow dilation greater than 2."""
     assert op.run_on_npu
     if op.type == Op.Conv2DBias or op.type == Op.DepthwiseConv2DBias:
         dilation_w, dilation_h = op.get_kernel_dilation()
 
         # if dilation in either axis is greater than that supported by the hardware then we must manually dilate the
         # kernel
         if dilation_w > 2 or dilation_h > 2:
@@ -2250,14 +2419,138 @@
 
         # force new_shape attribute to output shape
         op.attrs["new_shape"] = ofm_shape
 
     return op
 
 
+def convert_conv_groups(op: Operation, arch, nng):
+    """
+    Convert convolution groups to a split followed by separate convolutions and then a concat.
+    This needs to run before the concat and split handling functions"""
+    if not op.type.is_conv2d_op():
+        return op
+
+    num_conv_groups = op.attrs.get("num_conv_groups", 0)
+    if num_conv_groups > 1:
+        # convolution groups params
+        ifm_depth_cg = op.ifm.shape[-1] // num_conv_groups
+        num_filters_cg = op.weights.shape[-1] // num_conv_groups
+
+        # create split
+        split_op = Operation(Op.Split, f"{op.name}_split")
+        split_op.attrs.update(
+            {
+                "num_splits": num_conv_groups,
+            }
+        )
+        # first input is the split axis
+        split_op.add_input_tensor(
+            # split along the depth axis
+            create_const_tensor(f"{split_op.name}_axis", [0], DataType.int32, [-1])
+        )
+        # second input is the ifm
+        split_op.add_input_tensor(op.ifm)
+        # calculate shape of each ofm part
+        split_op_ofm_shape = op.ifm.shape[:-1] + [ifm_depth_cg]
+
+        # create concat. do this prior to each conv group so that the for-loop can reference the concat as it iterates
+        concat_op = Operation(Op.ConcatTFLite, f"{op.name}_concat")
+        concat_op.attrs.update(
+            {
+                "axis": -1,
+                "fused_activation_function": None,
+            }
+        )
+        # calculate shape of each ifm part
+        concat_op_ifm_shape = op.ofm.shape[:-1] + [num_filters_cg]
+        # output is the concatenated tensor
+        concat_op.set_output_tensor(op.ofm)  # will disconnect ofm from op
+
+        # for each conv group
+        for i in range(num_conv_groups):
+            # cg params
+            cg_oc_start = i * num_filters_cg
+            cg_oc_end = (i + 1) * num_filters_cg
+
+            # split has multiple outputs
+            split_op_ofm_part = Tensor(split_op_ofm_shape, op.ifm.dtype, f"{split_op.name}_out{i}")
+            split_op_ofm_part.quantization = op.ifm.quantization.clone()
+            split_op.add_output_tensor(split_op_ofm_part)
+
+            # concat has multiple inputs
+            concat_op_ifm_part = Tensor(concat_op_ifm_shape, op.ifm.dtype, f"{concat_op.name}_in{i}")
+            concat_op_ifm_part.quantization = op.ofm.quantization.clone()
+            concat_op.add_input_tensor(concat_op_ifm_part)
+
+            # create convolution group operator
+            conv_group_op = Operation(op.type, f"{op.name}_cg{i}")
+            conv_group_op.attrs = op.attrs.copy()
+            conv_group_op.attrs["num_conv_groups"] = 1
+            # first input is the ifm
+            conv_group_op.add_input_tensor(split_op_ofm_part)
+            # second input is weights. the number of filters (i.e. the output channels) need to be split equally
+            # across all of the convolution groups
+            conv_group_op_weights_shape = op.weights.shape[:-1] + [num_filters_cg]
+            conv_group_op_weights_quant = op.weights.quantization.clone()
+            conv_group_op_weights_quant.scale_f32 = op.weights.quantization.scale_f32[..., cg_oc_start:cg_oc_end]
+            conv_group_op_weights_quant.zero_point = op.weights.quantization.zero_point[..., cg_oc_start:cg_oc_end]
+            conv_group_op.add_input_tensor(
+                create_const_tensor(
+                    f"{op.weights.name}_cg{i}",
+                    conv_group_op_weights_shape,
+                    op.weights.dtype,
+                    op.weights.values[..., cg_oc_start:cg_oc_end],
+                    op.weights.purpose,
+                    conv_group_op_weights_quant,
+                )
+            )
+            # third input is bias. like the weights, the bias needs to be split equally across all of the convolution
+            # groups
+            if op.bias is None:
+                conv_group_op.add_input_tensor(None)
+            else:
+                conv_group_op_bias_shape = op.bias.shape[:-1] + [num_filters_cg]
+                conv_group_op_bias_quant = op.bias.quantization.clone()
+                conv_group_op_bias_quant.scale_f32 = op.bias.quantization.scale_f32[..., cg_oc_start:cg_oc_end]
+                conv_group_op_bias_quant.zero_point = op.bias.quantization.zero_point[..., cg_oc_start:cg_oc_end]
+                conv_group_op.add_input_tensor(
+                    create_const_tensor(
+                        f"{op.bias.name}_cg{i}",
+                        conv_group_op_bias_shape,
+                        op.bias.dtype,
+                        op.bias.values[..., cg_oc_start:cg_oc_end],
+                        op.bias.purpose,
+                        op.bias.quantization,
+                    )
+                )
+            # output goes to the concat
+            conv_group_op.set_output_tensor(concat_op_ifm_part)
+            # update the cg op shapes and debug db
+            conv_group_op.set_ifm_ofm_shapes()
+            DebugDatabase.add_optimised(op, conv_group_op)
+
+        # update the split/concat op shapes/debug db
+        split_op.set_ifm_ofm_shapes()
+        DebugDatabase.add_optimised(op, split_op)
+        concat_op.set_ifm_ofm_shapes()
+        DebugDatabase.add_optimised(op, concat_op)
+
+        # disconnect the original convolution operator.
+        # the ofm has already been disconnected by concat_op.set_output_tensor()
+        op.ifm.consumer_list.remove(op)
+        op.inputs = []
+        op.outputs = []
+
+        # return last op so that other graph optimiser functions can process the new operators
+        op = concat_op
+
+    return op
+
+
 def supported_operator_check(op, arch, nng):
     op.run_on_npu = arch.tflite_supported_operators.is_operator_supported(op)
     return op
 
 
 def tflite_optimise_graph(nng, arch, force_symmetric_int_weights):
     # Compile time static optimisations
@@ -2274,15 +2567,15 @@
             arch,
             [],
             optimisation_list,
             rewrite_unsupported=False,
         )
 
     # Pre-processing step
-    pre_process_list = [supported_operator_check, set_ifm_ofm_op_shapes, fixup_reshape]
+    pre_process_list = [supported_operator_check, set_ifm_ofm_op_shapes, fixup_reshape, convert_conv_groups]
 
     for idx, sg in enumerate(nng.subgraphs):
         nng.subgraphs[idx] = rewrite_graph.rewrite_graph_pre_order(
             nng,
             sg,
             arch,
             [],
@@ -2335,14 +2628,15 @@
         convert_depthwise_to_conv,
         convert_conv_to_fc,
         convert_lstm,
         convert_softmax,
         convert_prelu,
         convert_mul_max_to_abs_or_lrelu,
         convert_lrelu,
+        convert_avg_pool_to_conv2d,
         fixup_strided_conv,
         convert_hardswish_to_lut,
         rewrite_fully_connected_input,
         convert_batched_fc_shape,
         fixup_conv2d_backprop,
         fixup_relus_with_differing_ifm_ofm_scaling,
         reorder_depthwise_weights,
```

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite_mapping.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -712,15 +712,22 @@
         ),
         TFLITE_IFM_INDICES,
     ),
     BuiltinOperator.UNIDIRECTIONAL_SEQUENCE_LSTM: (
         Op.UnidirectionalSequenceLstm,
         OptionsSerializer(
             "UnidirectionalSequenceLSTMOptions",
-            ("asymmetric_quantize_inputs", "cell_clip", fused_act, "proj_clip", "time_major"),
+            (
+                "asymmetric_quantize_inputs",
+                "cell_clip",
+                "diagonal_recurrent_tensors",
+                fused_act,
+                "proj_clip",
+                "time_major",
+            ),
         ),
         TFLITE_IFM_WEIGHTS_INDICES,
     ),
     BuiltinOperator.STRIDED_SLICE: (
         Op.StridedSlice,
         OptionsSerializer(
             "StridedSliceOptions", ("begin_mask", "ellipsis_mask", "end_mask", "new_axis_mask", "shrink_axis_mask")
@@ -789,15 +796,15 @@
     BuiltinOperator.TILE: (Op.Tile, OptionsSerializer("TileOptions"), TFLITE_NO_INDICES),
     BuiltinOperator.EXPAND_DIMS: (Op.ExpandDims, OptionsSerializer("ExpandDimsOptions"), TFLITE_IFM_INDICES),
     BuiltinOperator.EQUAL: (Op.Equal, OptionsSerializer("EqualOptions"), TFLITE_NO_INDICES),
     BuiltinOperator.NOT_EQUAL: (Op.NotEqual, OptionsSerializer("NotEqualOptions"), TFLITE_NO_INDICES),
     BuiltinOperator.LOG: (Op.Log, None, TFLITE_NO_INDICES),
     BuiltinOperator.SUM: (Op.Sum, OptionsSerializer("ReducerOptions", ("keep_dims",)), TFLITE_NO_INDICES),
     BuiltinOperator.SQRT: (Op.Sqrt, None, TFLITE_NO_INDICES),
-    BuiltinOperator.RSQRT: (Op.Rsqrt, None, TFLITE_NO_INDICES),
+    BuiltinOperator.RSQRT: (Op.Rsqrt, None, TFLITE_IFM_INDICES),
     BuiltinOperator.SHAPE: (
         Op.Shape,
         OptionsSerializer("ShapeOptions", (("out_type", datatype_deserialize, datatype_serialize),)),
         TFLITE_IFM_INDICES,
     ),
     BuiltinOperator.POW: (Op.Pow, OptionsSerializer("PowOptions"), TFLITE_NO_INDICES),
     BuiltinOperator.ARG_MIN: (
```

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite_model_semantic.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite_model_semantic.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,14 +106,18 @@
 
         # Setup specific constraints. Note: the order matters
         self.specific_constraints = defaultdict(list)
 
         # Conv-like checks:
         for op_type in TFLiteSemantic.convolution_like_ops:
             self.specific_constraints[op_type].append(TFLiteSemantic.constraint_stride_type)
+            if op_type in TFLiteSemantic.convolution_ops:
+                # Only Conv has groups
+                self.specific_constraints[op_type].append(TFLiteSemantic.constraint_conv_groups_ifm_depth)
+                self.specific_constraints[op_type].append(TFLiteSemantic.constraint_conv_groups_num_filters)
             if op_type not in TFLiteSemantic.transpose_convolution_ops:
                 # Transpose Conv does not contain dilation
                 self.specific_constraints[op_type].append(TFLiteSemantic.constraint_dilation_type)
 
         # Pooling checks:
         for op_type in TFLiteSemantic.pooling_ops:
             self.specific_constraints[op_type].append(TFLiteSemantic.constraint_stride_type)
@@ -176,14 +180,15 @@
         # FullyConnected specific checks:
         self.specific_constraints[Op.FullyConnected].append(TFLiteSemantic.constraint_fc_output_2d)
         self.specific_constraints[Op.FullyConnected].append(TFLiteSemantic.constraint_keep_dim_ifm_ofm)
 
         # Pad specific checks:
         self.specific_constraints[Op.Pad].append(TFLiteSemantic.constraint_pad_input_count)
         self.specific_constraints[Op.Pad].append(TFLiteSemantic.constraint_pad_constant)
+        self.specific_constraints[Op.Pad].append(TFLiteSemantic.constraint_pad_output_shape)
 
         # HardSwish specific checks:
         self.specific_constraints[Op.HardSwish].append(TFLiteSemantic.constraint_input_8bit)
         self.specific_constraints[Op.HardSwish].append(TFLiteSemantic.constraint_matching_in_out_types)
 
         # Mean specific checks:
         self.specific_constraints[Op.Mean].append(TFLiteSemantic.constraint_mean_input_dims)
@@ -369,14 +374,44 @@
     def constraint_stride_type(op):
         "Stride values for both width and height must be integer types"
         w, h = op.get_kernel_stride()
         valid = is_integer(w) and is_integer(h)
         return valid, f"Op has stride WxH as: {repr(w)}x{repr(h)}"
 
     @staticmethod
+    def constraint_conv_groups_ifm_depth(op):
+        """IFM depth must be a whole multiple of the filter kernel depth"""
+        ifm_depth = op.ifm.shape[-1]  # nhwc
+        kernel_ic = op.weights.shape[-2]  # hwio
+        num_conv_groups = ifm_depth // kernel_ic
+
+        if ifm_depth % kernel_ic == 0:
+            op.attrs["num_conv_groups"] = num_conv_groups
+            valid = True
+        else:
+            valid = False
+
+        return valid, f"IFM depth = {ifm_depth} and filter kernel depth = {kernel_ic}"
+
+    @staticmethod
+    def constraint_conv_groups_num_filters(op):
+        """Number of filter kernels must be equally divisible by the number of convolution groups"""
+        ifm_depth = op.ifm.shape[-1]  # nhwc
+        kernel_ic = op.weights.shape[-2]  # hwio
+        kernel_oc = op.weights.shape[-1]  # hwio
+        num_conv_groups = ifm_depth // kernel_ic
+
+        if kernel_oc % num_conv_groups == 0:
+            valid = True
+        else:
+            valid = False
+
+        return valid, f"Filter kernels = {kernel_oc} and convolution groups = {num_conv_groups}"
+
+    @staticmethod
     def constraint_dilation_type(op):
         "Dilation factor values for both width and height must be integer types"
         w, h = op.get_kernel_dilation()
         valid = is_integer(w) and is_integer(h)
         return valid, f"Op has dilation factor WxH as: {repr(w)}x{repr(h)}"
 
     @staticmethod
@@ -432,27 +467,35 @@
 
     @staticmethod
     def constraint_split_axis(op):
         "Axis value must be in the range [-RANK(IFM) to +RANK(IFM))"
         axis_tens = op.inputs[0]
         input_tens = op.inputs[1]
         dims = len(input_tens.shape)
-        axis = int(axis_tens.values)
+        # handle axis being a scalar or 1-D array
+        if axis_tens.values.ndim == 0:
+            axis = int(axis_tens.values)
+        else:
+            axis = int(axis_tens.values[0])
         axis += dims if axis < 0 else 0
         valid = 0 <= axis < dims
         return valid, f"Op has ifm_dimensions={dims} and axis value is: {axis}"
 
     @staticmethod
     def constraint_split_num_splits(op):
         "Axis must be divisible by number of splits"
         num_splits = op.attrs.get("num_splits")
         axis_tens = op.inputs[0]
         input_tens = op.inputs[1]
         dims = len(input_tens.shape)
-        axis = int(axis_tens.values)
+        # handle axis being a scalar or 1-D array
+        if axis_tens.values.ndim == 0:
+            axis = int(axis_tens.values)
+        else:
+            axis = int(axis_tens.values[0])
         axis += dims if axis < 0 else 0
         valid = input_tens.shape[axis] % num_splits == 0
         return valid, f"Op has ifm shape={input_tens.shape} axis={axis} num_splits={num_splits}"
 
     @staticmethod
     def constraint_splitv_inferred(op):
         "Only one size is allowed to be inferred"
@@ -546,14 +589,24 @@
     def constraint_pad_constant(op):
         "The padding tensor must be constant"
         pad_tensor = op.inputs[1].values
         valid = pad_tensor is not None
         return valid, f"Op has non-constant padding tensor: {op.inputs[1].values}"
 
     @staticmethod
+    def constraint_pad_output_shape(op):
+        "Shape of output tensor must equal to size of input tensor plus padding"
+        input_shape = op.inputs[0].shape
+        expected_output_shape = op.outputs[0].shape
+        pad_tensor = op.inputs[1].values
+        actual_output_shape = input_shape + pad_tensor.T[0] + pad_tensor.T[1]
+        valid = np.array_equal(actual_output_shape, expected_output_shape)
+        return valid, f"Op has wrong output tensor shape: {expected_output_shape}, has shape: {actual_output_shape}"
+
+    @staticmethod
     def constraint_stridedslice_inputs_const(op):
         "Begin, End and Stride Input tensors must be constant"
         valid = True
         extra = []
         _, begin, end, strides = op.inputs
         if begin.values is None:
             valid = False
@@ -690,22 +743,52 @@
     def constraint_mean_input_dims(op):
         "Input tensor must be at least 2D"
         dims = len(op.inputs[0].shape)
         return 2 <= dims <= 4, f"Input is {dims}D"
 
     @staticmethod
     def constraint_mean_axis(op):
-        "Axis indices must correspond to height and width axes"
-        dims = len(op.inputs[0].shape)
-        axis = int(op.inputs[1].values) if op.inputs[1].shape == [] else list(op.inputs[1].values)
-        if dims == 2 or dims == 3:
-            valid = axis in (0, 1, [0], [1], [0, 1], [1, 0])
-        elif dims == 4:
-            valid = axis in (1, 2, [1], [2], [1, 2], [2, 1])
-        return valid, f"Axis is {axis}"
+        """Requirements for axis parameter:
+        When IFM tensor is 2D:
+          - Reduction in both axes is supported.
+        When IFM tensor is 3D or 4D:
+          - Reduction in Batch axis is only supported if batch size is 1.
+          - Reduction in both Height and Width axes is supported.
+          - Reduction in Depth axis is supported if at least one of H,W,C are of size 1."""
+        input_shape = op.inputs[0].shape
+        dims = len(input_shape)
+        if op.inputs[1].shape == []:
+            axis = [int(op.inputs[1].values)]
+        else:
+            axis = list(op.inputs[1].values)
+        valid = True
+
+        for ax in axis:
+            if ax < 0 or ax >= dims:
+                return False, "Axis parameter is out of bounds. axis: {axis}, dims: {dims}. "
+
+            # Batch is only supported if batch shape is 1
+            if dims == 4 and ax == 0:
+                if input_shape[0] != 1:
+                    valid = False
+                    break
+
+            # Depth is supported if any of h,w,c == 1
+            if dims == 3:
+                if ax == 2 and not any([s == 1 for s in input_shape]):
+                    valid = False
+                    break
+
+            # Depth is supported if any of h,w,c == 1
+            if dims == 4:
+                if ax == 3 and not any([s == 1 for s in input_shape[1:]]):
+                    valid = False
+                    break
+
+        return valid, f"Shape is {input_shape}, Axis is {axis}."
 
     @staticmethod
     def constraint_matching_in_out_quant(op):
         "Input and output quantisation must match."
         if not check_quantized_tens_scaling_equal(op.ifm, op.ofm):
             return False, "IFM and OFM quantisation parameters are not equal."
         return True, "IFM and OFM quantisation parameters matches."
```

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite_reader.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite_reader.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite_supported_operators.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite_supported_operators.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from .operation import Op
 from .operation import Padding
 from .supported_operators_util import docstring_format_args
 from .supported_operators_util import list_formatter
 from .tensor import check_quantized_tens_scaling_equal
 from .tflite_mapping import BUILTIN_OPERATOR_UNKNOWN
 from .tflite_mapping import optype_to_builtintype
+from .utils import calc_resize_factor
 
 
 def _optype_formatter(op_list):
     # Convert internal op types to external names
     output = map(optype_to_builtintype, op_list)
     # Remove UNKNOWNs
     output = (x for x in output if x is not BUILTIN_OPERATOR_UNKNOWN)
@@ -186,15 +187,18 @@
     stride_range = (1, 3)
     dilated_height_range = (1, 64)
     dilated_product_range = (1, 64 * 64)
     weights_limit = 127 * 65536
     filter_range = (1, 8)
     filter_height_range = (1, 256)
     filter_product_range = (1, 256 * 256)
-    mean_kernel_product = 64 * 64
+    mean_reduced_axis_max_size = 64 * 64
+    mean_kernel_product_int8 = 2 ** (24)
+    mean_kernel_product_uint8 = 2 ** (23)
+    mean_kernel_product_int16 = 2 ** (16)
 
     def __init__(self):
         # Setup the generic constraints. Note: the order matters
         self.generic_constraints = []
         self.generic_constraints.append(TFLiteSupportedOperators.constraint_tens_dtype)
         self.generic_constraints.append(TFLiteSupportedOperators.constraint_tens_int32_ops)
         self.generic_constraints.append(TFLiteSupportedOperators.constraint_tens_dimension)
@@ -215,15 +219,15 @@
             self.generic_constraints_exceptions[op_type].append(TFLiteSupportedOperators.constraint_batch_size)
 
         # Setup specific constraints. Note: the order matters
         self.specific_constraints = defaultdict(list)
 
         # Conv specific ops:
         for op_type in TFLiteSupportedOperators.convolution_ops:
-            self.specific_constraints[op_type].append(TFLiteSupportedOperators.constraint_conv_stride)
+            self.specific_constraints[op_type].append(TFLiteSupportedOperators.constraint_stride_width_no_upper_limit)
 
         # Conv-like checks:
         for op_type in TFLiteSupportedOperators.convolution_like_ops:
             self.specific_constraints[op_type].append(TFLiteSupportedOperators.constraint_dilated_height_range)
             self.specific_constraints[op_type].append(TFLiteSupportedOperators.constraint_dilated_product_range)
             self.specific_constraints[op_type].append(TFLiteSupportedOperators.constraint_weights_type)
             self.specific_constraints[op_type].append(TFLiteSupportedOperators.constraint_weights_const)
@@ -239,18 +243,19 @@
             self.specific_constraints[op_type].append(TFLiteSupportedOperators.constraint_tconv_valid)
         # Depthwise Conv specific checks:
         for op_type in TFLiteSupportedOperators.depthwise_convolution_ops:
             self.specific_constraints[op_type].append(TFLiteSupportedOperators.constraint_depthwise_conv_stride)
             self.specific_constraints[op_type].append(TFLiteSupportedOperators.constraint_depth_multiplier)
 
         # Pooling checks:
-        for op_type in TFLiteSupportedOperators.pooling_ops:
+        for op_type in TFLiteSupportedOperators.pooling_ops - TFLiteSupportedOperators.avg_pooling_ops:
             self.specific_constraints[op_type].append(TFLiteSupportedOperators.constraint_stride_range)
         # AVG pooling specific checks:
         for op_type in TFLiteSupportedOperators.avg_pooling_ops:
+            self.specific_constraints[op_type].append(TFLiteSupportedOperators.constraint_stride_range_no_padding)
             self.specific_constraints[op_type].append(TFLiteSupportedOperators.constraint_filter_range)
             self.specific_constraints[op_type].append(TFLiteSupportedOperators.constraint_filter_height_range_valid_pad)
             self.specific_constraints[op_type].append(
                 TFLiteSupportedOperators.constraint_filter_product_range_valid_pad
             )
         # MAX pooling specific checks:
         for op_type in TFLiteSupportedOperators.max_pooling_ops:
@@ -305,15 +310,16 @@
         # Pad specific checks:
         self.specific_constraints[Op.Pad].append(TFLiteSupportedOperators.constraint_pad_shape)
         self.specific_constraints[Op.Pad].append(TFLiteSupportedOperators.constraint_padding_dimensions)
         self.specific_constraints[Op.Pad].append(TFLiteSupportedOperators.constraint_pad_type)
 
         # Mean specific checks:
         self.specific_constraints[Op.Mean].append(TFLiteSupportedOperators.constraint_mean_height_width_product)
-        self.specific_constraints[Op.Mean].append(TFLiteSupportedOperators.constraint_mean_height_single_axis)
+        self.specific_constraints[Op.Mean].append(TFLiteSupportedOperators.constraint_mean_width)
+        self.specific_constraints[Op.Mean].append(TFLiteSupportedOperators.constraint_mean_depth)
 
         # Reshape specific checks:
         self.specific_constraints[Op.Reshape].append(TFLiteSupportedOperators.constraint_reshape_shape_constant)
 
         # ArgMax specific checks:
         self.specific_constraints[Op.ArgMax].append(TFLiteSupportedOperators.constraint_argmax_axis)
         self.specific_constraints[Op.ArgMax].append(TFLiteSupportedOperators.constraint_argmax_depth)
@@ -321,14 +327,21 @@
         # UnidirectionalSequenceLstm specific checks:
         op_type = Op.UnidirectionalSequenceLstm
         self.specific_constraints[op_type].append(TFLiteSupportedOperators.constraint_lstm_no_cifg)
         self.specific_constraints[op_type].append(TFLiteSupportedOperators.constraint_lstm_no_peep_hole)
         self.specific_constraints[op_type].append(TFLiteSupportedOperators.constraint_lstm_no_projection)
         self.specific_constraints[op_type].append(TFLiteSupportedOperators.constraint_lstm_no_normalisation)
         self.specific_constraints[op_type].append(TFLiteSupportedOperators.constraint_lstm_weights)
+        self.specific_constraints[op_type].append(TFLiteSupportedOperators.constraint_lstm_weight_dimensions)
+
+        # Rsqrt specific checks
+        self.specific_constraints[Op.Rsqrt].append(TFLiteSupportedOperators.constraint_rsqrt_input_int8)
+
+        # Slice specific checks:
+        self.specific_constraints[Op.Slice].append(TFLiteSupportedOperators.constraint_slice_inputs_const)
 
     def is_operator_supported(self, op):
         ext_type = optype_to_builtintype(op.type)
         if op.type not in TFLiteSupportedOperators.supported_operators:
             if op.type not in (Op.Placeholder, Op.SubgraphInput, Op.Const):
                 print(f"Info: {ext_type} '{op.name}' is a CPU only op")
             return False
@@ -537,23 +550,41 @@
                 f"Op has ifm_channels={ifm_channels}, ofm_channels={ofm_channels}"
                 f" and depth_multiplier={depth_multiplier}"
             )
             return valid, extra
         return True, "Op has depth_multiplier=1"
 
     @staticmethod
-    def constraint_conv_stride(op):
-        "Stride width must be greater than or equal to 1 and stride height must be between 1 and 3"
+    def constraint_stride_width_no_upper_limit(op):
+        """Stride width must be greater than or equal to 1.
+        For stride widths greater than 3, the post-optimization stride needs to be less than or equal to 3.
+        Stride height must be between 1 and 3."""
         w, h = op.get_kernel_stride()
         stride_min = 1
         stride_max_h = 3
-        valid = (stride_min <= w) and (stride_min <= h <= stride_max_h)
+        ifm_width = op.ifm.shape[2]
+        _, optimized_stride = calc_resize_factor(ifm_width, w) if w > 1 else (1, w)
+        # Optimized stride indicates the final Conv2D stride width after all optimizations are performed
+        can_optimize_stride_width_gt_3 = optimized_stride <= 3
+        valid = (stride_min <= w) and (stride_min <= h <= stride_max_h) and can_optimize_stride_width_gt_3
+
         return valid, f"Op has stride WxH as: {w}x{h}"
 
     @staticmethod
+    def constraint_stride_range_no_padding(op):
+        """Stride width must be greater than or equal to 1.
+        For stride width greater than 3, valid padding needs to be used."""
+        w, _ = op.get_kernel_stride()
+        valid, message = TFLiteSupportedOperators.constraint_stride_width_no_upper_limit(op)
+        padding = op.attrs.get("padding", None)
+        is_optimized_with_valid_padding = padding in (None, Padding.VALID) or w <= 3
+        valid = valid and is_optimized_with_valid_padding
+        return valid, f"{message}, padding: {padding}"
+
+    @staticmethod
     def constraint_depthwise_conv_stride(op):
         "Stride values for both width and height must be between 1 and 3"
         w, h = op.get_kernel_stride()
         stride_min, stride_max = 1, 3
         valid = (stride_min <= w <= stride_max) and (stride_min <= h <= stride_max)
         return valid, f"Op has stride WxH as: {w}x{h}"
 
@@ -599,18 +630,19 @@
         return True, "Op has padding=SAME"
 
     @classmethod
     @docstring_format_args(filter_range)
     def constraint_filter_range(cls, op):
         "Kernel filter values for both width and height must be in the range [{}, {}]"
         if op.attrs["padding"] == Padding.SAME:
+            sw, _ = op.get_kernel_stride()
             w = op.kernel.width
             h = op.kernel.height
             filter_min, filter_max = cls.filter_range
-            valid = (filter_min <= w <= filter_max) and (filter_min <= h <= filter_max)
+            valid = ((filter_min <= w <= filter_max) or sw == w) and (filter_min <= h <= filter_max)
             return valid, f"Op has kernel filter WxH as: {w}x{h}"
         return True, "Op has padding=VALID"
 
     @classmethod
     @docstring_format_args(filter_height_range)
     def constraint_filter_height_range(cls, op):
         "Kernel filter height must be in the range [{}, {}]"
@@ -807,47 +839,70 @@
                 if not (i == i2 or i == 1 or i2 == 1) or o != mi:
                     valid = False
                     break
 
         return valid, f"Op has ifm_shape={ifm_shape} and ifm2_shape={ifm2_shape}"
 
     @classmethod
-    @docstring_format_args([mean_kernel_product])
+    @docstring_format_args([mean_kernel_product_int8, mean_kernel_product_uint8, mean_kernel_product_int16])
     def constraint_mean_height_width_product(cls, op):
-        """Product of height and width must be no greater than {}"""
+        """Product of reduced axes must be no greater than:
+        - {} for signed 8-bit inputs.
+        - {} for unsigned 8-bit inputs.
+        - {} for signed 16-bit inputs."""
+        shape = op.inputs[0].shape
+        if op.inputs[1].shape == []:
+            axis = [int(op.inputs[1].values)]
+        else:
+            axis = list(op.inputs[1].values)
+
+        # compute the product of the shape of all reduced axes
+        axis_shapes = [shape[ax] for ax in axis]
+        prod = np.prod(axis_shapes)
+
+        if op.ifm.dtype == DataType.int16:
+            max_prod = cls.mean_kernel_product_int16
+            datatype = "int16"
+        elif op.ifm.dtype == DataType.uint8:
+            max_prod = cls.mean_kernel_product_uint8
+            datatype = "uint8"
+        else:
+            max_prod = cls.mean_kernel_product_int8
+            datatype = "int8"
+        return prod <= max_prod, f"Datatype is {datatype}, product of axes is {prod}"
+
+    @classmethod
+    @docstring_format_args([mean_reduced_axis_max_size])
+    def constraint_mean_width(cls, op):
+        """If Width axis is reduced its shape must be no greater than {}."""
         shape = op.inputs[0].shape
         hi = 0 if len(shape) < 4 else 1
         h, w = shape[hi : hi + 2]
-        max_prod = cls.mean_kernel_product
-        return h * w <= max_prod, f"Product of height and width is {h * w}"
+        max_width = cls.mean_reduced_axis_max_size
+        return w <= max_width, f"Width is {w}"
 
     @classmethod
-    @docstring_format_args([dilated_height_range[1]])
-    def constraint_mean_height_single_axis(cls, op):
-        """For single axis averages across the height dimension:
-        IFM height must be no greater than {}"""
-        inp, axis = op.inputs
-        if axis.shape == [] or axis.shape[0] == 1:  # single axis
-            axis = int(axis.values) if len(axis.shape) == 0 else int(axis.values[0])
+    @docstring_format_args([mean_reduced_axis_max_size])
+    def constraint_mean_depth(cls, op):
+        """If Depth axis is reduced its shape must be no greater than {}."""
+        max_depth = cls.mean_reduced_axis_max_size
+        shape = op.inputs[0].shape
+
+        if op.inputs[1].shape == []:
+            axis = [int(op.inputs[1].values)]
         else:
-            # Multiple axes
-            return True, ""
+            axis = list(op.inputs[1].values)
 
-        shape = inp.shape
-        if len(shape) < 3:
-            # No height dimension present in IFM
-            return True, ""
-        if axis != len(shape) - 3:
-            # Not averaging across the height dimension
-            return True, ""
+        depth_idx = len(shape) - 1
 
-        h = shape[axis]
-        ifm, ofm = op.get_ifm_ofm()
+        supported = True
+        if depth_idx in axis and shape[-1] > max_depth:
+            supported = False
 
-        return h <= cls.dilated_height_range[1], f"Height is {h}"
+        return supported, f"Depth is {shape[-1]}, shape is {shape}, axis is {axis}"
 
     @staticmethod
     def constraint_reshape_shape_constant(op):
         "Shape must be constant"
         valid = True
         extra = []
 
@@ -907,7 +962,35 @@
         return valid, "Op uses normalisation"
 
     @staticmethod
     def constraint_lstm_weights(op):
         "All input and recurrent weights must be available"
         valid = None not in op.inputs[1:9]
         return valid, "Op has missing weights"
+
+    @staticmethod
+    def constraint_lstm_weight_dimensions(op):
+        "All recurrent weights must be 2D"
+        valid = all([len(input.shape) == 2 for input in op.inputs[5:9]])
+        return valid, "Op recurrent weights are not 2D"
+
+    @staticmethod
+    def constraint_rsqrt_input_int8(op):
+        "IFM must be int8"
+        ifm_dtype = op.ifm.dtype
+        valid = ifm_dtype == DataType.int8
+        return valid, f"Op has ifm_dtype={ifm_dtype}"
+
+    @staticmethod
+    def constraint_slice_inputs_const(op):
+        "Begin and Size Input tensors must be constant"
+        valid = True
+        extra = []
+        _, begin, sizes = op.inputs
+        if begin.values is None:
+            valid = False
+            extra.append(f"Begin tensor '{begin.name}'")
+        if sizes.values is None:
+            valid = False
+            extra.append(f"Size tensor '{sizes.name}'")
+        extra = ", ".join(extra)
+        return valid, f"Op has non-constant tensors: {extra}"
```

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tflite_writer.py` & `ethos-u-vela-3.9.0/ethosu/vela/tflite_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 # Functions used to write to a TensorFlow Lite format file. Supports adding in file identifiers.
 import flatbuffers
 import flatbuffers.number_types as N
 import numpy as np
 from flatbuffers import encode
 from flatbuffers.builder import UOffsetTFlags
 
+from ._version import __version__
 from .errors import VelaError
 from .nn_graph import PassPlacement
 from .operation import Op
 from .reader_util import align_inputs_indices
 from .tensor import MemType
 from .tensor import shape_num_elements
 from .tensor import TensorPurpose
@@ -423,15 +424,18 @@
 
         return SubGraph.SubGraphEnd(builder)
 
     def write_aligned_bytes(self, buf):
         builder = self.builder
         builder.assertNotNested()
         builder.nested = True
-        data = bytes(buf)
+        if isinstance(buf, str):
+            data = bytes(buf, "utf-8")
+        else:
+            data = bytes(buf)
         length_bytes = UOffsetTFlags.py_type(len(data))
         builder.vectorNumElems = length_bytes
         builder.Prep(16, length_bytes)  # Reserve aligned storage
         builder.head = UOffsetTFlags.py_type(builder.Head() - length_bytes)  # Update FlatBuffer internal pointer
         builder.Bytes[builder.Head() : builder.Head() + length_bytes] = data  # Assign bytes to aligned area
         return builder.EndVector()
 
@@ -460,15 +464,16 @@
         operator_code_offset = self.write_offset_vector(
             [
                 self.serialise_operator_code(idx, optype, code, version)
                 for idx, (optype, code, version) in enumerate(self.operator_codes)
             ]
         )
 
-        description = builder.CreateString("Vela Optimised")
+        description = builder.CreateString(f"Vela {__version__} Optimised")
+        self.nng.metadata.append(("vela_version", __version__))
 
         subgraph_offset = self.write_offset_vector(
             [self.serialise_subgraph(sg, builder.CreateString(sg.name)) for sg in self.subgraphs_to_write]
         )
 
         # Fill the metadata buffer
         version = np.int32(0)
```

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tosa/ArithmeticRightShiftAttribute.py` & `ethos-u-vela-3.9.0/ethosu/vela/tosa/ArithmeticRightShiftAttribute.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tosa/AxisAttribute.py` & `ethos-u-vela-3.9.0/ethosu/vela/tosa/AxisAttribute.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tosa/ClampAttribute.py` & `ethos-u-vela-3.9.0/ethosu/vela/tosa/ClampAttribute.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tosa/CondIfAttribute.py` & `ethos-u-vela-3.9.0/ethosu/vela/tosa/CondIfAttribute.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tosa/ConvAttribute.py` & `ethos-u-vela-3.9.0/ethosu/vela/tosa/ConvAttribute.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tosa/ConvQuantInfo.py` & `ethos-u-vela-3.9.0/ethosu/vela/tosa/ConvQuantInfo.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tosa/MatMulQuantInfo.py` & `ethos-u-vela-3.9.0/ethosu/vela/tosa/MatMulQuantInfo.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tosa/MulAttribute.py` & `ethos-u-vela-3.9.0/ethosu/vela/tosa/MulAttribute.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tosa/Op.py` & `ethos-u-vela-3.9.0/ethosu/vela/tosa/Op.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tosa/PadQuantInfo.py` & `ethos-u-vela-3.9.0/ethosu/vela/tosa/PadQuantInfo.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tosa/PoolAttribute.py` & `ethos-u-vela-3.9.0/ethosu/vela/tosa/PoolAttribute.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tosa/ReluNAttribute.py` & `ethos-u-vela-3.9.0/ethosu/vela/tosa/ReluNAttribute.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tosa/RescaleAttribute.py` & `ethos-u-vela-3.9.0/ethosu/vela/tosa/RescaleAttribute.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tosa/ReshapeAttribute.py` & `ethos-u-vela-3.9.0/ethosu/vela/tosa/ReshapeAttribute.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tosa/ResizeAttribute.py` & `ethos-u-vela-3.9.0/ethosu/vela/tosa/ResizeAttribute.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tosa/SliceAttribute.py` & `ethos-u-vela-3.9.0/ethosu/vela/tosa/SliceAttribute.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tosa/TileAttribute.py` & `ethos-u-vela-3.9.0/ethosu/vela/tosa/TileAttribute.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tosa/TosaBasicBlock.py` & `ethos-u-vela-3.9.0/ethosu/vela/tosa/TosaBasicBlock.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tosa/TosaGraph.py` & `ethos-u-vela-3.9.0/ethosu/vela/tosa/TosaGraph.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tosa/TosaOperator.py` & `ethos-u-vela-3.9.0/ethosu/vela/tosa/TosaOperator.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tosa/TosaTensor.py` & `ethos-u-vela-3.9.0/ethosu/vela/tosa/TosaTensor.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tosa/TransposeConvAttribute.py` & `ethos-u-vela-3.9.0/ethosu/vela/tosa/TransposeConvAttribute.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tosa/UnaryQuantInfo.py` & `ethos-u-vela-3.9.0/ethosu/vela/tosa/UnaryQuantInfo.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tosa/Version.py` & `ethos-u-vela-3.9.0/ethosu/vela/tosa/Version.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tosa/WhileLoopAttribute.py` & `ethos-u-vela-3.9.0/ethosu/vela/tosa/WhileLoopAttribute.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tosa_graph_optimiser.py` & `ethos-u-vela-3.9.0/ethosu/vela/tosa_graph_optimiser.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tosa_mapping.py` & `ethos-u-vela-3.9.0/ethosu/vela/tosa_mapping.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tosa_model_semantic.py` & `ethos-u-vela-3.9.0/ethosu/vela/tosa_model_semantic.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tosa_reader.py` & `ethos-u-vela-3.9.0/ethosu/vela/tosa_reader.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/tosa_supported_operators.py` & `ethos-u-vela-3.9.0/ethosu/vela/tosa_supported_operators.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/vela.py` & `ethos-u-vela-3.9.0/ethosu/vela/vela.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/ethosu/vela/weight_compressor.py` & `ethos-u-vela-3.9.0/ethosu/vela/weight_compressor.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.8.0/pyproject.toml` & `ethos-u-vela-3.9.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 [project]
 name = "ethos-u-vela"
 description = "Neural network model compiler for Arm Ethos-U NPUs"
-requires-python = "~=3.7"
+requires-python = "~=3.8"
 authors = [{name = "Arm Ltd", email = "mlg-vela@arm.com"}]
 license = {text= "Apache License 2.0"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: POSIX :: Linux",
     "Operating System :: Microsoft :: Windows :: Windows 10",
     "Programming Language :: C",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Software Development :: Compilers",
 ]
 keywords = ["ethos-u", "vela compiler", "tflite", "npu"]
 dependencies = [
     "flatbuffers==2.0.7",
     "numpy<=1.21.3; python_version<='3.7'",
@@ -58,8 +58,15 @@
 
 [build-system]
 requires = [
     "numpy<=1.21.3; python_version<='3.7'",
     "numpy; python_version>'3.7'",
     "setuptools_scm[toml]~=7.1.0"
 ]
-build-backend = "setuptools.build_meta"
+build-backend = "setuptools.build_meta"
+
+[tool.pytest.ini_options]
+minversion = "6.0"
+addopts = ["-ra", "--showlocals", "--strict-markers", "--strict-config"]
+xfail_strict = true
+filterwarnings = ["error"]
+testpaths = ["ethosu/mlw_codec/test", "ethosu/vela/test"]
```

### Comparing `ethos-u-vela-3.8.0/setup.py` & `ethos-u-vela-3.9.0/setup.py`

 * *Files identical despite different names*

