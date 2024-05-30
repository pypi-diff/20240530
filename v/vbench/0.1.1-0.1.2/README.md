# Comparing `tmp/vbench-0.1.1.tar.gz` & `tmp/vbench-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbench-0.1.1.tar", last modified: Thu Jan 18 08:53:21 2024, max compression
+gzip compressed data, was "vbench-0.1.2.tar", last modified: Thu May 30 05:19:26 2024, max compression
```

## Comparing `vbench-0.1.1.tar` & `vbench-0.1.2.tar`

### file list

```diff
@@ -1,267 +1,313 @@
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.659544 vbench-0.1.1/
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    11356 2023-12-06 13:51:47.000000 vbench-0.1.1/LICENSE
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)      177 2024-01-17 11:04:03.000000 vbench-0.1.1/MANIFEST.in
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     5253 2024-01-18 08:53:21.659151 vbench-0.1.1/PKG-INFO
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     7746 2024-01-17 11:04:03.000000 vbench-0.1.1/README.md
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.585498 vbench-0.1.1/bin/
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     1772 2024-01-17 11:04:03.000000 vbench-0.1.1/bin/evaluate
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)      375 2024-01-18 07:58:22.000000 vbench-0.1.1/requirements.txt
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)       38 2024-01-18 08:53:21.659622 vbench-0.1.1/setup.cfg
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     1004 2024-01-18 08:49:15.000000 vbench-0.1.1/setup.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.591135 vbench-0.1.1/vbench/
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2820 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/__init__.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2832 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/aesthetic_quality.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2874 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/appearance_style.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2428 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/background_consistency.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.593669 vbench-0.1.1/vbench/cli/
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/cli/__init__.py
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     1658 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/cli/evaluate.py
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     5858 2024-01-18 07:58:22.000000 vbench-0.1.1/vbench/cli/static_filter.py
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)      516 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/cli/vbench.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     3258 2024-01-18 07:58:22.000000 vbench-0.1.1/vbench/color.py
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     5036 2024-01-18 07:58:22.000000 vbench-0.1.1/vbench/dynamic_degree.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     3721 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/human_action.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1267 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/imaging_quality.py
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     6652 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/motion_smoothness.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2475 2024-01-18 07:58:22.000000 vbench-0.1.1/vbench/multiple_objects.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2314 2024-01-18 07:58:22.000000 vbench-0.1.1/vbench/object_class.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2776 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/overall_consistency.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2422 2024-01-18 07:58:22.000000 vbench-0.1.1/vbench/scene.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     5247 2024-01-18 07:58:22.000000 vbench-0.1.1/vbench/spatial_relationship.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2667 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/subject_consistency.py
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     1794 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/temporal_flickering.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2820 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/temporal_style.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.594145 vbench-0.1.1/vbench/third_party/
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.594742 vbench-0.1.1/vbench/third_party/RAFT/
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/RAFT/__init__.py
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)    45743 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/RAFT/chairs_split.txt
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.596903 vbench-0.1.1/vbench/third_party/RAFT/core/
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/RAFT/core/__init__.py
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     3091 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/RAFT/core/corr.py
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     9255 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/RAFT/core/datasets.py
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     8847 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/RAFT/core/extractor.py
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     4933 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/RAFT/core/raft.py
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     5227 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/RAFT/core/update.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.598131 vbench-0.1.1/vbench/third_party/RAFT/core/utils_core/
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/RAFT/core/utils_core/__init__.py
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     9108 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/RAFT/core/utils_core/augmentor.py
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     4318 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/RAFT/core/utils_core/flow_viz.py
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     4024 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/RAFT/core/utils_core/frame_utils.py
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     2489 2023-12-29 16:31:51.000000 vbench-0.1.1/vbench/third_party/RAFT/core/utils_core/utils.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.599707 vbench-0.1.1/vbench/third_party/ViCLIP/
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/ViCLIP/__init__.py
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     4986 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/ViCLIP/simple_tokenizer.py
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     7935 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/ViCLIP/viclip.py
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     9344 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/ViCLIP/viclip_text.py
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)    12460 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/ViCLIP/viclip_vision.py
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/__init__.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.600528 vbench-0.1.1/vbench/third_party/amt/
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/amt/__init__.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.602937 vbench-0.1.1/vbench/third_party/amt/benchmarks/
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/benchmarks/__init__.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1738 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/benchmarks/adobe240.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1705 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/benchmarks/gopro.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2484 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/benchmarks/snu_film.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1108 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/benchmarks/speed_parameters.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1905 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/benchmarks/ucf101.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2076 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/benchmarks/vimeo90k.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2300 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/benchmarks/vimeo90k_tta.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     4528 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/benchmarks/xiph.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.604215 vbench-0.1.1/vbench/third_party/amt/cfgs/
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1130 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/cfgs/AMT-G.yaml
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1126 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/cfgs/AMT-L.yaml
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1128 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/cfgs/AMT-S.yaml
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      945 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/cfgs/AMT-S_gopro.yaml
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1200 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/cfgs/IFRNet.yaml
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.605130 vbench-0.1.1/vbench/third_party/amt/datasets/
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/datasets/__init__.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     3488 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/datasets/adobe_datasets.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     8472 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/datasets/gopro_datasets.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     7400 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/datasets/vimeo_datasets.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      328 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/environment.yaml
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.605566 vbench-0.1.1/vbench/third_party/amt/flow_generation/
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/flow_generation/__init__.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2649 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/flow_generation/gen_flow.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.606003 vbench-0.1.1/vbench/third_party/amt/flow_generation/liteflownet/
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/flow_generation/liteflownet/__init__.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    19652 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/flow_generation/liteflownet/run.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.606486 vbench-0.1.1/vbench/third_party/amt/losses/
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/losses/__init__.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     7453 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/losses/loss.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.606944 vbench-0.1.1/vbench/third_party/amt/metrics/
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/metrics/__init__.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     4531 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/metrics/psnr_ssim.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.608171 vbench-0.1.1/vbench/third_party/amt/networks/
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     8009 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/networks/AMT-G.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     7107 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/networks/AMT-L.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     7054 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/networks/AMT-S.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     5881 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/networks/IFRNet.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/networks/__init__.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.609254 vbench-0.1.1/vbench/third_party/amt/networks/blocks/
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/networks/blocks/__init__.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    11300 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/networks/blocks/feat_enc.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     4260 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/networks/blocks/ifrnet.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     3000 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/networks/blocks/multi_flow.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     8113 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/networks/blocks/raft.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2309 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/train.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.609995 vbench-0.1.1/vbench/third_party/amt/trainers/
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/trainers/__init__.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     9851 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/trainers/base_trainer.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1944 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/trainers/logger.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.611333 vbench-0.1.1/vbench/third_party/amt/utils/
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/utils/__init__.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      443 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/amt/utils/build_utils.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1460 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/utils/dist_utils.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     4325 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/utils/flow_utils.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     8257 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/amt/utils/utils.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1585 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/grit_model.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.611770 vbench-0.1.1/vbench/third_party/grit_src/
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.613258 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      106 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/.gitignore
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/__init__.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.614214 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      605 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/__init__.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     3251 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/config.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.614880 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/__init__.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.618769 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/backbone/
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/backbone/__init__.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    17177 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/backbone/bifpn.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    17570 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/backbone/bifpn_fcos.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    17202 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/backbone/dla.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    17423 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/backbone/dlafpn.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2419 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/backbone/fpn_p5.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    27456 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/backbone/res2net.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    11817 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/debug.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.619996 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/dense_heads/
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/dense_heads/__init__.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    37214 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/dense_heads/centernet.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     5674 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/dense_heads/centernet_head.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1131 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/dense_heads/utils.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.621362 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/layers/
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/layers/__init__.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     3912 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/layers/deform_conv.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2718 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/layers/heatmap_focal_loss.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     4043 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/layers/iou_loss.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1016 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/layers/ml_nms.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.621899 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/meta_arch/
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/meta_arch/__init__.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2656 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/meta_arch/centernet_detector.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.623064 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/roi_heads/
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/roi_heads/__init__.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     4460 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/roi_heads/custom_fast_rcnn.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     7948 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/roi_heads/custom_roi_heads.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1021 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/roi_heads/fed_loss.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.629384 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/configs/
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      684 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/configs/Base-CenterNet-FPN.yaml
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1373 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/configs/Base-CenterNet2.yaml
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      835 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/configs/Base_S4_DLA.yaml
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)       72 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/configs/CenterNet-FPN_R50_1x.yaml
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)       89 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/configs/CenterNet-S4_DLA_8x.yaml
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)       75 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2-F_R50_1x.yaml
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      836 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_DLA-BiFPN-P3_24x.yaml
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      836 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_DLA-BiFPN-P3_4x.yaml
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      612 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_DLA-BiFPN-P5_640_16x.yaml
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      649 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_DLA-BiFPN-P5_640_16x_ST.yaml
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      654 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_DLA-fcosBiFPN-P5_640_16x_ST.yaml
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      713 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_R2-101-DCN-BiFPN_1280_4x.yaml
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      819 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_R2-101-DCN-BiFPN_4x+4x_1560_ST.yaml
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      666 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_R2-101-DCN_896_4x.yaml
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)       31 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_R50_1x.yaml
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      562 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_X101-DCN_2x.yaml
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      348 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/configs/LVIS_CenterNet2_R50_1x.yaml
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      407 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/configs/LVIS_CenterNet2_R50_Fed_1x.yaml
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      257 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/configs/O365_CenterNet2_R50_1x.yaml
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      879 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/configs/nuImages_CenterNet2_DLA_640_8x.yaml
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     9114 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/predictor.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     7897 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/train_net.py
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/__init__.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.631199 vbench-0.1.1/vbench/third_party/grit_src/configs/
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1816 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/grit_src/configs/Base.yaml
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      444 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/grit_src/configs/GRiT_B_DenseCap.yaml
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      654 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/grit_src/configs/GRiT_B_DenseCap_ObjectDet.yaml
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      462 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/grit_src/configs/GRiT_B_ObjectDet.yaml
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      494 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/grit_src/configs/GRiT_H_ObjectDet.yaml
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      469 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/grit_src/configs/GRiT_L_ObjectDet.yaml
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.632357 vbench-0.1.1/vbench/third_party/grit_src/grit/
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      223 2023-12-29 16:50:13.000000 vbench-0.1.1/vbench/third_party/grit_src/grit/__init__.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1634 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/grit/config.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     3368 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/grit_src/grit/custom_solver.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.633369 vbench-0.1.1/vbench/third_party/grit_src/grit/data/
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/grit/data/__init__.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1551 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/grit_src/grit/data/custom_build_augmentation.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     9349 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/grit_src/grit/data/custom_dataset_dataloader.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     5989 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/grit/data/custom_dataset_mapper.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.634261 vbench-0.1.1/vbench/third_party/grit_src/grit/data/datasets/
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/grit/data/datasets/__init__.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     3770 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/grit_src/grit/data/datasets/grit_coco.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     3537 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/grit_src/grit/data/datasets/object365.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     3077 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/grit_src/grit/data/datasets/vg.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.634963 vbench-0.1.1/vbench/third_party/grit_src/grit/data/transforms/
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/grit/data/transforms/__init__.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2083 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/grit_src/grit/data/transforms/custom_augmentation_impl.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     4143 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/grit_src/grit/data/transforms/custom_transform.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.635415 vbench-0.1.1/vbench/third_party/grit_src/grit/modeling/
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/grit/modeling/__init__.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.636316 vbench-0.1.1/vbench/third_party/grit_src/grit/modeling/backbone/
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/grit/modeling/backbone/__init__.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     6474 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/grit_src/grit/modeling/backbone/utils.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    20715 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/grit/modeling/backbone/vit.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.637023 vbench-0.1.1/vbench/third_party/grit_src/grit/modeling/meta_arch/
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/grit/modeling/meta_arch/__init__.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2549 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/grit/modeling/meta_arch/grit.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.638056 vbench-0.1.1/vbench/third_party/grit_src/grit/modeling/roi_heads/
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/grit/modeling/roi_heads/__init__.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     4785 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/grit_src/grit/modeling/roi_heads/grit_fast_rcnn.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    23962 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/grit/modeling/roi_heads/grit_roi_heads.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     6782 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/grit_src/grit/modeling/soft_nms.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.640059 vbench-0.1.1/vbench/third_party/grit_src/grit/modeling/text/
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/grit/modeling/text/__init__.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     8699 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/grit_src/grit/modeling/text/file_utils.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     3284 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/grit_src/grit/modeling/text/load_text_token.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    25283 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/grit_src/grit/modeling/text/modeling_bert.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    26306 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/grit_src/grit/modeling/text/text_decoder.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     4601 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/grit_src/grit/predictor.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     4212 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/grit_src/image_dense_captions.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.644487 vbench-0.1.1/vbench/third_party/tag2Text/
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)       51 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/tag2Text/__init__.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      233 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/tag2Text/config_swinB_384.json
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    45292 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/tag2Text/med.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      485 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/tag2Text/med_config.json
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      560 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/tag2Text/q2l_config.json
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    26827 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/tag2Text/swin_transformer.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    19100 2024-01-10 16:05:48.000000 vbench-0.1.1/vbench/third_party/tag2Text/tag2text.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    39420 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/tag2Text/tag_class.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    14240 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/tag2Text/vit.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.645463 vbench-0.1.1/vbench/third_party/umt/
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/umt/__init__.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.656811 vbench-0.1.1/vbench/third_party/umt/datasets/
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)       59 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/umt/datasets/__init__.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     7935 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/umt/datasets/build.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    15923 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/umt/datasets/kinetics.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    15163 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/umt/datasets/kinetics_sparse.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    12618 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/umt/datasets/mae.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1685 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/umt/datasets/masking_generator.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    14728 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/umt/datasets/mixup.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    16126 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/umt/datasets/rand_augment.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     6616 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/umt/datasets/random_erasing.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    27253 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/umt/datasets/ssv2.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     7984 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/umt/datasets/transforms.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    43918 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/umt/datasets/video_transforms.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     4267 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/umt/datasets/volume_transforms.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2915 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/umt/functional.py
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     7446 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/umt/kinetics_400_categories.txt
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.658546 vbench-0.1.1/vbench/third_party/umt/models/
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      464 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/umt/models/__init__.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    10888 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/umt/models/clip.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    15759 2024-01-17 11:04:03.000000 vbench-0.1.1/vbench/third_party/umt/models/modeling_finetune.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    13057 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/umt/models/modeling_pretrain.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    12413 2023-12-06 13:51:47.000000 vbench-0.1.1/vbench/third_party/umt/models/modeling_pretrain_umt.py
--rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    18500 2024-01-18 07:58:22.000000 vbench-0.1.1/vbench/utils.py
-drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-18 08:53:21.592574 vbench-0.1.1/vbench.egg-info/
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     5253 2024-01-18 08:53:21.000000 vbench-0.1.1/vbench.egg-info/PKG-INFO
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)    11283 2024-01-18 08:53:21.000000 vbench-0.1.1/vbench.egg-info/SOURCES.txt
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        1 2024-01-18 08:53:21.000000 vbench-0.1.1/vbench.egg-info/dependency_links.txt
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)       50 2024-01-18 08:53:21.000000 vbench-0.1.1/vbench.egg-info/entry_points.txt
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)      304 2024-01-18 08:53:21.000000 vbench-0.1.1/vbench.egg-info/requires.txt
--rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        7 2024-01-18 08:53:21.000000 vbench-0.1.1/vbench.egg-info/top_level.txt
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.125641 vbench-0.1.2/
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    11356 2023-12-06 13:51:47.000000 vbench-0.1.2/LICENSE
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)      153 2024-04-20 18:14:39.000000 vbench-0.1.2/MANIFEST.in
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     6463 2024-05-30 05:19:26.124708 vbench-0.1.2/PKG-INFO
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    15012 2024-05-30 05:14:03.000000 vbench-0.1.2/README.md
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:25.972473 vbench-0.1.2/bin/
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     1772 2024-01-17 11:04:03.000000 vbench-0.1.2/bin/evaluate
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:25.974801 vbench-0.1.2/competitions/
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     4495 2024-05-28 23:01:12.000000 vbench-0.1.2/competitions/__init__.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1920 2024-05-28 23:01:12.000000 vbench-0.1.2/competitions/clip_score.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     1101 2024-05-28 23:01:12.000000 vbench-0.1.2/competitions/competition_utils.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     2652 2024-05-28 23:01:12.000000 vbench-0.1.2/competitions/run_eval.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)      377 2024-05-27 08:25:01.000000 vbench-0.1.2/requirements.txt
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)       38 2024-05-30 05:19:26.125826 vbench-0.1.2/setup.cfg
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     1004 2024-05-30 05:15:12.000000 vbench-0.1.2/setup.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:25.989735 vbench-0.1.2/vbench/
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)   228118 2024-05-28 23:07:07.000000 vbench-0.1.2/vbench/VBench_full_info.json
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     8626 2024-05-08 18:01:27.000000 vbench-0.1.2/vbench/__init__.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2842 2024-05-28 23:06:23.000000 vbench-0.1.2/vbench/aesthetic_quality.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2884 2024-05-27 08:25:01.000000 vbench-0.1.2/vbench/appearance_style.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2438 2024-05-27 08:25:01.000000 vbench-0.1.2/vbench/background_consistency.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:25.993881 vbench-0.1.2/vbench/cli/
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/cli/__init__.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     5262 2024-04-20 18:14:40.000000 vbench-0.1.2/vbench/cli/evaluate.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     7316 2024-05-01 05:37:02.000000 vbench-0.1.2/vbench/cli/static_filter.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)      563 2024-04-20 18:14:39.000000 vbench-0.1.2/vbench/cli/vbench.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     3268 2024-05-27 08:25:01.000000 vbench-0.1.2/vbench/color.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     5046 2024-05-27 08:25:01.000000 vbench-0.1.2/vbench/dynamic_degree.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     3731 2024-04-20 18:14:40.000000 vbench-0.1.2/vbench/human_action.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2153 2024-05-28 23:06:23.000000 vbench-0.1.2/vbench/imaging_quality.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     6662 2024-05-27 08:25:01.000000 vbench-0.1.2/vbench/motion_smoothness.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2485 2024-04-20 18:14:40.000000 vbench-0.1.2/vbench/multiple_objects.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2324 2024-04-20 18:14:40.000000 vbench-0.1.2/vbench/object_class.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2786 2024-05-30 05:07:07.000000 vbench-0.1.2/vbench/overall_consistency.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2432 2024-04-20 18:14:40.000000 vbench-0.1.2/vbench/scene.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     5257 2024-04-20 18:14:40.000000 vbench-0.1.2/vbench/spatial_relationship.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2677 2024-05-27 08:25:01.000000 vbench-0.1.2/vbench/subject_consistency.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     1804 2024-05-27 08:25:01.000000 vbench-0.1.2/vbench/temporal_flickering.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2830 2024-05-05 11:25:55.000000 vbench-0.1.2/vbench/temporal_style.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:25.994805 vbench-0.1.2/vbench/third_party/
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:25.995785 vbench-0.1.2/vbench/third_party/RAFT/
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/RAFT/__init__.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)    45743 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/RAFT/chairs_split.txt
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:25.999080 vbench-0.1.2/vbench/third_party/RAFT/core/
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/RAFT/core/__init__.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     3091 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/RAFT/core/corr.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     9255 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/RAFT/core/datasets.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     8847 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/RAFT/core/extractor.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     4933 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/RAFT/core/raft.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     5227 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/RAFT/core/update.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.000498 vbench-0.1.2/vbench/third_party/RAFT/core/utils_core/
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/RAFT/core/utils_core/__init__.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     9108 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/RAFT/core/utils_core/augmentor.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     4318 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/RAFT/core/utils_core/flow_viz.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     4024 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/RAFT/core/utils_core/frame_utils.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     2489 2023-12-29 16:31:51.000000 vbench-0.1.2/vbench/third_party/RAFT/core/utils_core/utils.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.002073 vbench-0.1.2/vbench/third_party/ViCLIP/
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/ViCLIP/__init__.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     4986 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/ViCLIP/simple_tokenizer.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     7935 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/ViCLIP/viclip.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     9344 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/ViCLIP/viclip_text.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)    12460 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/ViCLIP/viclip_vision.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/__init__.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.003234 vbench-0.1.2/vbench/third_party/amt/
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/amt/__init__.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.010511 vbench-0.1.2/vbench/third_party/amt/benchmarks/
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/benchmarks/__init__.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1738 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/benchmarks/adobe240.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1705 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/benchmarks/gopro.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2484 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/benchmarks/snu_film.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1108 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/benchmarks/speed_parameters.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1905 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/benchmarks/ucf101.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2076 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/benchmarks/vimeo90k.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2300 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/benchmarks/vimeo90k_tta.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     4528 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/benchmarks/xiph.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.012605 vbench-0.1.2/vbench/third_party/amt/cfgs/
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1130 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/cfgs/AMT-G.yaml
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1126 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/cfgs/AMT-L.yaml
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1128 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/cfgs/AMT-S.yaml
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      945 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/cfgs/AMT-S_gopro.yaml
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1200 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/cfgs/IFRNet.yaml
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.013897 vbench-0.1.2/vbench/third_party/amt/datasets/
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/datasets/__init__.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     3488 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/datasets/adobe_datasets.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     8472 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/datasets/gopro_datasets.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     7400 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/datasets/vimeo_datasets.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      328 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/environment.yaml
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.014507 vbench-0.1.2/vbench/third_party/amt/flow_generation/
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/flow_generation/__init__.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2649 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/flow_generation/gen_flow.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.015073 vbench-0.1.2/vbench/third_party/amt/flow_generation/liteflownet/
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/flow_generation/liteflownet/__init__.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    19652 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/flow_generation/liteflownet/run.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.015991 vbench-0.1.2/vbench/third_party/amt/losses/
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/losses/__init__.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     7453 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/losses/loss.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.016631 vbench-0.1.2/vbench/third_party/amt/metrics/
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/metrics/__init__.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     4531 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/metrics/psnr_ssim.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.018725 vbench-0.1.2/vbench/third_party/amt/networks/
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     8101 2024-03-10 06:22:37.000000 vbench-0.1.2/vbench/third_party/amt/networks/AMT-G.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     7200 2024-03-10 06:22:37.000000 vbench-0.1.2/vbench/third_party/amt/networks/AMT-L.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     7149 2024-03-10 06:22:37.000000 vbench-0.1.2/vbench/third_party/amt/networks/AMT-S.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     5927 2024-03-10 06:22:37.000000 vbench-0.1.2/vbench/third_party/amt/networks/IFRNet.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/networks/__init__.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.020569 vbench-0.1.2/vbench/third_party/amt/networks/blocks/
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/networks/blocks/__init__.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    11300 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/networks/blocks/feat_enc.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     4284 2024-03-10 06:22:37.000000 vbench-0.1.2/vbench/third_party/amt/networks/blocks/ifrnet.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     3047 2024-03-10 06:22:37.000000 vbench-0.1.2/vbench/third_party/amt/networks/blocks/multi_flow.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     8113 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/networks/blocks/raft.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2309 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/train.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.021586 vbench-0.1.2/vbench/third_party/amt/trainers/
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/trainers/__init__.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     9851 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/trainers/base_trainer.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1944 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/trainers/logger.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.023206 vbench-0.1.2/vbench/third_party/amt/utils/
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/utils/__init__.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      443 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/amt/utils/build_utils.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1460 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/utils/dist_utils.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     4325 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/utils/flow_utils.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     8257 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/amt/utils/utils.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1585 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/grit_model.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.023904 vbench-0.1.2/vbench/third_party/grit_src/
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.025689 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      106 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/.gitignore
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/__init__.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.026831 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      605 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/__init__.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     3251 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/config.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.027475 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/__init__.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.031588 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/backbone/
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/backbone/__init__.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    17177 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/backbone/bifpn.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    17570 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/backbone/bifpn_fcos.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    17202 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/backbone/dla.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    17423 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/backbone/dlafpn.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2419 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/backbone/fpn_p5.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    27456 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/backbone/res2net.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    11817 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/debug.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.033629 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/dense_heads/
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/dense_heads/__init__.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    37214 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/dense_heads/centernet.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     5674 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/dense_heads/centernet_head.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1131 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/dense_heads/utils.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.035869 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/layers/
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/layers/__init__.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     3912 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/layers/deform_conv.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2718 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/layers/heatmap_focal_loss.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     4043 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/layers/iou_loss.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1016 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/layers/ml_nms.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.036651 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/meta_arch/
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/meta_arch/__init__.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2656 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/meta_arch/centernet_detector.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.038630 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/roi_heads/
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/roi_heads/__init__.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     4460 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/roi_heads/custom_fast_rcnn.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     7948 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/roi_heads/custom_roi_heads.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1021 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/roi_heads/fed_loss.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.048396 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/configs/
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      684 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/configs/Base-CenterNet-FPN.yaml
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1373 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/configs/Base-CenterNet2.yaml
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      835 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/configs/Base_S4_DLA.yaml
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)       72 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/configs/CenterNet-FPN_R50_1x.yaml
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)       89 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/configs/CenterNet-S4_DLA_8x.yaml
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)       75 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2-F_R50_1x.yaml
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      836 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_DLA-BiFPN-P3_24x.yaml
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      836 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_DLA-BiFPN-P3_4x.yaml
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      612 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_DLA-BiFPN-P5_640_16x.yaml
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      649 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_DLA-BiFPN-P5_640_16x_ST.yaml
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      654 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_DLA-fcosBiFPN-P5_640_16x_ST.yaml
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      713 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_R2-101-DCN-BiFPN_1280_4x.yaml
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      819 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_R2-101-DCN-BiFPN_4x+4x_1560_ST.yaml
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      666 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_R2-101-DCN_896_4x.yaml
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)       31 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_R50_1x.yaml
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      562 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_X101-DCN_2x.yaml
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      348 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/configs/LVIS_CenterNet2_R50_1x.yaml
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      407 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/configs/LVIS_CenterNet2_R50_Fed_1x.yaml
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      257 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/configs/O365_CenterNet2_R50_1x.yaml
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      879 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/configs/nuImages_CenterNet2_DLA_640_8x.yaml
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     9114 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/predictor.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     7897 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/train_net.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/__init__.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.051428 vbench-0.1.2/vbench/third_party/grit_src/configs/
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1816 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/grit_src/configs/Base.yaml
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      444 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/grit_src/configs/GRiT_B_DenseCap.yaml
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      654 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/grit_src/configs/GRiT_B_DenseCap_ObjectDet.yaml
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      462 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/grit_src/configs/GRiT_B_ObjectDet.yaml
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      494 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/grit_src/configs/GRiT_H_ObjectDet.yaml
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      469 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/grit_src/configs/GRiT_L_ObjectDet.yaml
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.052946 vbench-0.1.2/vbench/third_party/grit_src/grit/
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      223 2023-12-29 16:50:13.000000 vbench-0.1.2/vbench/third_party/grit_src/grit/__init__.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1634 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/grit/config.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     3368 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/grit_src/grit/custom_solver.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.054870 vbench-0.1.2/vbench/third_party/grit_src/grit/data/
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/grit/data/__init__.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1551 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/grit_src/grit/data/custom_build_augmentation.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     9349 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/grit_src/grit/data/custom_dataset_dataloader.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     5989 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/grit/data/custom_dataset_mapper.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.056661 vbench-0.1.2/vbench/third_party/grit_src/grit/data/datasets/
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/grit/data/datasets/__init__.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     3770 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/grit_src/grit/data/datasets/grit_coco.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     3537 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/grit_src/grit/data/datasets/object365.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     3077 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/grit_src/grit/data/datasets/vg.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.057968 vbench-0.1.2/vbench/third_party/grit_src/grit/data/transforms/
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/grit/data/transforms/__init__.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2083 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/grit_src/grit/data/transforms/custom_augmentation_impl.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     4143 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/grit_src/grit/data/transforms/custom_transform.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.058850 vbench-0.1.2/vbench/third_party/grit_src/grit/modeling/
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/grit/modeling/__init__.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.060772 vbench-0.1.2/vbench/third_party/grit_src/grit/modeling/backbone/
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/grit/modeling/backbone/__init__.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     6474 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/grit_src/grit/modeling/backbone/utils.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    20715 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/grit/modeling/backbone/vit.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.062491 vbench-0.1.2/vbench/third_party/grit_src/grit/modeling/meta_arch/
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/grit/modeling/meta_arch/__init__.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2549 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/grit/modeling/meta_arch/grit.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.063809 vbench-0.1.2/vbench/third_party/grit_src/grit/modeling/roi_heads/
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/grit/modeling/roi_heads/__init__.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     4785 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/grit_src/grit/modeling/roi_heads/grit_fast_rcnn.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    23962 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/grit/modeling/roi_heads/grit_roi_heads.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     6782 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/grit_src/grit/modeling/soft_nms.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.066998 vbench-0.1.2/vbench/third_party/grit_src/grit/modeling/text/
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/grit/modeling/text/__init__.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     8699 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/grit_src/grit/modeling/text/file_utils.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     3284 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/grit_src/grit/modeling/text/load_text_token.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    25283 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/grit_src/grit/modeling/text/modeling_bert.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    26306 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/grit_src/grit/modeling/text/text_decoder.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     4601 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/grit_src/grit/predictor.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     4212 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/grit_src/image_dense_captions.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.078784 vbench-0.1.2/vbench/third_party/tag2Text/
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)       51 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/tag2Text/__init__.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      233 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/tag2Text/config_swinB_384.json
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    45292 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/tag2Text/med.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      485 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/tag2Text/med_config.json
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      560 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/tag2Text/q2l_config.json
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    26827 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/tag2Text/swin_transformer.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    19100 2024-01-10 16:05:48.000000 vbench-0.1.2/vbench/third_party/tag2Text/tag2text.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    39420 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/tag2Text/tag_class.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    14240 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/tag2Text/vit.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.080408 vbench-0.1.2/vbench/third_party/umt/
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/umt/__init__.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.088096 vbench-0.1.2/vbench/third_party/umt/datasets/
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)       59 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/umt/datasets/__init__.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     7935 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/umt/datasets/build.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    15923 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/umt/datasets/kinetics.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    15163 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/umt/datasets/kinetics_sparse.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    12618 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/umt/datasets/mae.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1685 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/umt/datasets/masking_generator.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    14728 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/umt/datasets/mixup.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    16126 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/umt/datasets/rand_augment.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     6616 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/umt/datasets/random_erasing.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    27253 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/umt/datasets/ssv2.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     7984 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/umt/datasets/transforms.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    43918 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/umt/datasets/video_transforms.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     4267 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/umt/datasets/volume_transforms.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     2915 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/umt/functional.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     7446 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/umt/kinetics_400_categories.txt
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.092917 vbench-0.1.2/vbench/third_party/umt/models/
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      464 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/umt/models/__init__.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    10888 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/umt/models/clip.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    15759 2024-01-17 11:04:03.000000 vbench-0.1.2/vbench/third_party/umt/models/modeling_finetune.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    13057 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/umt/models/modeling_pretrain.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    12413 2023-12-06 13:51:47.000000 vbench-0.1.2/vbench/third_party/umt/models/modeling_pretrain_umt.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    18917 2024-05-30 05:07:07.000000 vbench-0.1.2/vbench/utils.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:25.992124 vbench-0.1.2/vbench.egg-info/
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     6463 2024-05-30 05:19:25.000000 vbench-0.1.2/vbench.egg-info/PKG-INFO
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)    12762 2024-05-30 05:19:25.000000 vbench-0.1.2/vbench.egg-info/SOURCES.txt
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        1 2024-05-30 05:19:25.000000 vbench-0.1.2/vbench.egg-info/dependency_links.txt
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)       50 2024-05-30 05:19:25.000000 vbench-0.1.2/vbench.egg-info/entry_points.txt
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)      304 2024-05-30 05:19:25.000000 vbench-0.1.2/vbench.egg-info/requires.txt
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)       84 2024-05-30 05:19:25.000000 vbench-0.1.2/vbench.egg-info/top_level.txt
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.096487 vbench-0.1.2/vbench2_beta_i2v/
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     1947 2024-04-04 16:49:27.000000 vbench-0.1.2/vbench2_beta_i2v/__init__.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     6919 2024-04-04 16:49:27.000000 vbench-0.1.2/vbench2_beta_i2v/camera_motion.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     3848 2024-04-26 04:01:48.000000 vbench-0.1.2/vbench2_beta_i2v/crop_to_diff_ratio.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     2882 2024-04-04 16:49:27.000000 vbench-0.1.2/vbench2_beta_i2v/i2v_background.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     2870 2024-04-04 16:49:27.000000 vbench-0.1.2/vbench2_beta_i2v/i2v_subject.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)    14520 2024-04-04 16:49:27.000000 vbench-0.1.2/vbench2_beta_i2v/utils.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.115335 vbench-0.1.2/vbench2_beta_long/
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)    14407 2024-05-28 23:01:12.000000 vbench-0.1.2/vbench2_beta_long/__init__.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)      463 2024-05-28 23:01:12.000000 vbench-0.1.2/vbench2_beta_long/aesthetic_quality.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)      365 2024-05-28 23:01:12.000000 vbench-0.1.2/vbench2_beta_long/appearance_style.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     4734 2024-05-28 23:01:12.000000 vbench-0.1.2/vbench2_beta_long/background_consistency.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)      321 2024-05-28 23:01:12.000000 vbench-0.1.2/vbench2_beta_long/color.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)      357 2024-05-28 23:01:12.000000 vbench-0.1.2/vbench2_beta_long/dynamic_degree.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     6711 2024-05-28 23:01:12.000000 vbench-0.1.2/vbench2_beta_long/eval_long.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)      349 2024-05-28 23:01:12.000000 vbench-0.1.2/vbench2_beta_long/human_action.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)      389 2024-05-28 23:01:12.000000 vbench-0.1.2/vbench2_beta_long/imaging_quality.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)      368 2024-05-28 23:01:12.000000 vbench-0.1.2/vbench2_beta_long/motion_smoothness.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)      364 2024-05-28 23:01:12.000000 vbench-0.1.2/vbench2_beta_long/multiple_objects.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)      349 2024-05-28 23:01:12.000000 vbench-0.1.2/vbench2_beta_long/object_class.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)      376 2024-05-28 23:01:12.000000 vbench-0.1.2/vbench2_beta_long/overall_consistency.py
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)      322 2024-05-28 23:01:12.000000 vbench-0.1.2/vbench2_beta_long/scene.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)      381 2024-05-28 23:01:12.000000 vbench-0.1.2/vbench2_beta_long/spatial_relationship.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     7619 2024-05-28 23:01:12.000000 vbench-0.1.2/vbench2_beta_long/static_filter.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     4981 2024-05-28 23:01:12.000000 vbench-0.1.2/vbench2_beta_long/subject_consistency.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     1831 2024-05-28 23:01:12.000000 vbench-0.1.2/vbench2_beta_long/temporal_flickering.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)      357 2024-05-28 23:01:12.000000 vbench-0.1.2/vbench2_beta_long/temporal_style.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)    13334 2024-05-28 23:01:12.000000 vbench-0.1.2/vbench2_beta_long/utils.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.120030 vbench-0.1.2/vbench2_beta_trustworthiness/
+-rwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)     5486 2024-05-08 13:12:37.000000 vbench-0.1.2/vbench2_beta_trustworthiness/__init__.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     2873 2024-04-20 16:10:49.000000 vbench-0.1.2/vbench2_beta_trustworthiness/culture_fairness.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     4725 2024-04-26 04:01:48.000000 vbench-0.1.2/vbench2_beta_trustworthiness/gender_bias.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     4993 2024-04-20 16:10:49.000000 vbench-0.1.2/vbench2_beta_trustworthiness/safety.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     4890 2024-04-20 16:10:49.000000 vbench-0.1.2/vbench2_beta_trustworthiness/skin_bias.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.121790 vbench-0.1.2/vbench2_beta_trustworthiness/third_party/
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)        0 2024-04-20 16:10:49.000000 vbench-0.1.2/vbench2_beta_trustworthiness/third_party/__init__.py
+drwxr-xr-x   0 nattapolchanpaisit   (501) staff       (20)        0 2024-05-30 05:19:26.123250 vbench-0.1.2/vbench2_beta_trustworthiness/third_party/nudenet/
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)       34 2024-04-20 16:10:49.000000 vbench-0.1.2/vbench2_beta_trustworthiness/third_party/nudenet/__init__.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)     4833 2024-04-20 16:10:49.000000 vbench-0.1.2/vbench2_beta_trustworthiness/third_party/nudenet/nudenet.py
+-rw-r--r--   0 nattapolchanpaisit   (501) staff       (20)    22054 2024-04-20 16:10:49.000000 vbench-0.1.2/vbench2_beta_trustworthiness/utils.py
```

### Comparing `vbench-0.1.1/LICENSE` & `vbench-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/PKG-INFO` & `vbench-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vbench
-Version: 0.1.1
+Version: 0.1.2
 Summary: Video generation benchmark
 License: Apache Software License 2.0
 Project-URL: Source, https://github.com/Vchitect/VBench
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Pillow
 Requires-Dist: numpy
@@ -58,14 +58,37 @@
    ```
    pip install detectron2@git+https://github.com/facebookresearch/detectron2.git
    ```
     
 If there is an error during [detectron2](https://github.com/facebookresearch/detectron2) installation, see [here](https://detectron2.readthedocs.io/en/latest/tutorials/install.html).
 
 ## Usage
+
+### Evaluate Your Own Videos
+We support evaluating any video. Simply provide the path to the video file, or the path to the folder that contains your videos. There is no requirement on the videos' names.
+- Note: We support customized videos / prompts for the following dimensions: `'subject_consistency', 'background_consistency', 'motion_smoothness', 'dynamic_degree', 'aesthetic_quality', 'imaging_quality'`
+
+
+To evaluate videos with customed input prompt, run our script with `--mode=custom_input`:
+```
+python evaluate.py \
+    --dimension $DIMENSION \
+    --videos_path /path/to/folder_or_video/ \
+    --mode=custom_input
+```
+alternatively you can use our command:
+```
+vbench evaluate \
+    --dimension $DIMENSION \
+    --videos_path /path/to/folder_or_video/ \
+    --mode=custom_input
+```
+
+### Evaluation on the Standard Prompt Suite of VBench
+
 ##### command line 
 ```bash
     vbench evaluate --videos_path $VIDEO_PATH --dimension $DIMENSION
 ```
 For example:
 ```bash
     vbench evaluate --videos_path "sampled_videos/lavie/human_action" --dimension "human_action"
@@ -79,22 +102,40 @@
         name = <name>,
         dimension_list = [<dimension>, <dimension>, ...],
     )
 ```
 For example: 
 ```python
     from vbench import VBench
-    my_VBench = VBench(device, "VBench_full_info.json", "evaluation_results")
+    my_VBench = VBench(device, "vbench/VBench_full_info.json", "evaluation_results")
     my_VBench.evaluate(
         videos_path = "sampled_videos/lavie/human_action",
         name = "lavie_human_action",
         dimension_list = ["human_action"],
     )
 ```
 
+### Evaluation on a specific category from VBench
+
+##### command line 
+```bash
+vbench evaluate \
+    --videos_path $VIDEO_PATH \
+    --dimension $DIMENSION \
+    --mode=vbench_category \
+    --category=$CATEGORY
+```
+or 
+```
+python evaluate.py \
+    --dimension $DIMENSION \
+    --videos_path /path/to/folder_or_video/ \
+    --mode=vbench_category
+```
+
 ## Prompt Suite
 
 We provide prompt lists are at `prompts/`. 
 
 Check out [details of prompt suites](https://github.com/Vchitect/VBench/tree/master/prompts), and instructions for [**how to sample videos for evaluation**](https://github.com/Vchitect/VBench/tree/master/prompts).
 
 ## Citation
```

### Comparing `vbench-0.1.1/bin/evaluate` & `vbench-0.1.2/bin/evaluate`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/setup.py` & `vbench-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     filename = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'requirements.txt')
     with open(filename, 'r') as f:
         envs = [line.rstrip('\n') for line in f.readlines() if '@' not in line]
     return envs
 
 install_requires = fetch_requirements()
 setup(name='vbench',
-      version='0.1.1',
+      version='0.1.2',
       description='Video generation benchmark',
       long_description=fetch_readme(),
       long_description_content_type='text/markdown',
       project_urls={
           'Source': 'https://github.com/Vchitect/VBench',
       },
       entry_points={
```

### Comparing `vbench-0.1.1/vbench/aesthetic_quality.py` & `vbench-0.1.2/vbench/aesthetic_quality.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         aesthetic_avg += cur_avg.item()
         num += 1
         video_results.append({'video_path': video_path, 'video_results': cur_avg.item()})
     aesthetic_avg /= num
     return aesthetic_avg, video_results
 
 
-def compute_aesthetic_quality(json_dir, device, submodules_list):
+def compute_aesthetic_quality(json_dir, device, submodules_list, **kwargs):
     vit_path = submodules_list[0]
     aes_path = submodules_list[1]
     aesthetic_model = get_aesthetic_model(aes_path).to(device)
     clip_model, preprocess = clip.load(vit_path, device=device)
     video_list, _ = load_dimension_info(json_dir, dimension='aesthetic_quality', lang='en')
     all_results, video_results = laion_aesthetic(aesthetic_model, clip_model, video_list, device)
     return all_results, video_results
```

### Comparing `vbench-0.1.1/vbench/appearance_style.py` & `vbench-0.1.2/vbench/appearance_style.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,12 +55,12 @@
                     sim += cur_sim
                     cnt +=1
                 video_sim = np.mean(cur_video)
                 video_results.append({'video_path': video_path, 'video_results': video_sim, 'frame_results':cur_video})
     sim_per_frame = sim / cnt
     return sim_per_frame, video_results
 
-def compute_appearance_style(json_dir, device, submodules_list):
+def compute_appearance_style(json_dir, device, submodules_list, **kwargs):
     clip_model, preprocess = clip.load(device=device, **submodules_list)
     _, video_dict = load_dimension_info(json_dir, dimension='appearance_style', lang='en')
     all_results, video_results = appearance_style(clip_model, video_dict, device)
     return all_results, video_results
```

### Comparing `vbench-0.1.1/vbench/background_consistency.py` & `vbench-0.1.2/vbench/background_consistency.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,14 @@
         sim += video_sim
         video_results.append({'video_path': video_path, 'video_results': sim_per_image})
     sim_per_video = sim / (len(video_list) - 1)
     sim_per_frame = sim / cnt
     return sim_per_frame, video_results
 
 
-def compute_background_consistency(json_dir, device, submodules_list):
+def compute_background_consistency(json_dir, device, submodules_list, **kwargs):
     vit_path, read_frame = submodules_list[0], submodules_list[1]
     clip_model, preprocess = clip.load(vit_path, device=device)
     video_list, _ = load_dimension_info(json_dir, dimension='background_consistency', lang='en')
     all_results, video_results = background_consistency(clip_model, preprocess, video_list, device, read_frame)
     return all_results, video_results
```

### Comparing `vbench-0.1.1/vbench/cli/static_filter.py` & `vbench-0.1.2/vbench2_beta_long/static_filter.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import os
 import cv2
 import glob
 import numpy as np
 import torch
 from tqdm import tqdm
+import argparse
+from pathlib import Path
 import json
 import shutil
 
 import logging
 logging.basicConfig(level = logging.INFO,format = '%(asctime)s - %(levelname)s - %(message)s')
 logger = logging.getLogger(__name__)
 
 from vbench.utils import CACHE_DIR, load_json
 from vbench.third_party.RAFT.core.raft import RAFT
 from vbench.third_party.RAFT.core.utils_core.utils import InputPadder
+from vbench2_beta_long.utils import get_prompt_from_filename
 
 
+CUR_PARENT_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 DEVICE = 'cuda'
 
 
 class StaticFilter:
     def __init__(self, args, device):
         self.args = args
         self.device = device
@@ -104,50 +108,82 @@
         return frame_list
 
 def check_and_move(args, filter_results, target_path=None):
     if target_path is None:
          target_path = os.path.join(args.result_path, "filtered_videos")
     os.makedirs(target_path, exist_ok=True)
     for prompt, v in filter_results.items():
-        if v["static_count"] < 5:
+        if v["static_count"] < 5 and args.filter_scope=='temporal_flickering':
             logger.warning(f"Prompt: '{prompt}' has fewer than 5 filter results.")
         for i, video_path in enumerate(v["static_path"]):
-            target_name = os.path.join(target_path, f"{prompt}-{i}.mp4")
+            target_name = os.path.join(target_path, os.path.basename(video_path))
+            # target_name = os.path.join(target_path, f"{prompt}-{i}.mp4")
             shutil.copy(video_path, target_name)
     logger.info(f"All filtered videos are saved in the '{target_path}' path")
 
 def static_filter(args):
     static_filter = StaticFilter(args, device=DEVICE)
     prompt_dict = {}
     prompt_list = []
-    full_prompt_list = load_json(args.prompt_file)
-    for prompt in full_prompt_list:
-        if 'temporal_flickering' in prompt['dimension']:
-            prompt_dict[prompt['prompt_en']] = {"static_count":0, "static_path":[]}
-            prompt_list.append(prompt['prompt_en'])
+
+    
+    paths = sorted(glob.glob(os.path.join(args.videos_path, "*", "*.mp4")))
+    
+    if args.filter_scope=='temporal_flickering':
+        full_prompt_list = load_json(f"{CUR_PARENT_DIR}/vbench/VBench_full_info.json")
+        for prompt in full_prompt_list:
+            if 'temporal_flickering' in prompt['dimension']:
+                prompt_dict[prompt['prompt_en']] = {"static_count":0, "static_path":[]}
+                prompt_list.append(prompt['prompt_en'])
+
+    elif args.filter_scope=='all':
+        for prompt in paths:
+            prompt = get_prompt_from_filename(prompt)
+            prompt_dict[prompt] = {"static_count":0, "static_path":[]}
+            prompt_list.append(prompt)
+
+    else:
+        assert os.path.isfile(args.filter_scope) and Path(args.filter_scope).suffix.lower() == '.json', f"""
+        --filter_scope flag is not correctly set, set to 'all' to filter all videos in the --videos_path directory, 
+        or provide the correct path to the JSON file
+        """
+        full_prompt_list = load_json(args.filter_scope)
+        for prompt in full_prompt_list:
+            prompt = get_prompt_from_filename(prompt)
+            prompt_dict[prompt] = {"static_count":0, "static_path":[]}
+            prompt_list.append(prompt)
     
-    paths = sorted(glob.glob(os.path.join(args.videos_path, "*.mp4")))
     for path in tqdm(paths):
-        name = '-'.join(path.split('/')[-1].split('-')[:-1]) 
+        name = get_prompt_from_filename(path)
         if name in prompt_list:
-            if prompt_dict[name]["static_count"] < 5:
+            if prompt_dict[name]["static_count"] < 5 or args.filter_scope != 'temporal_flickering':
                 if static_filter.infer(path):
                     prompt_dict[name]["static_count"] += 1
                     prompt_dict[name]["static_path"].append(path)
+
     os.makedirs(args.result_path, exist_ok=True)
     info_file = os.path.join(args.result_path, args.store_name)
     json.dump(prompt_dict, open(info_file, "w"))
     logger.info(f"Filtered results info is saved in the '{info_file}' file")
     check_and_move(args, prompt_dict)
 
-def register_subparsers(subparser):
-    parser = subparser.add_parser('static_filter')
+def parse_args():
+    parser = argparse.ArgumentParser(description='static_filter', formatter_class=argparse.RawTextHelpFormatter)
     parser.add_argument('--model', type=str, default=f"{CACHE_DIR}/raft_model/models/raft-things.pth", help="restore checkpoint")
     parser.add_argument('--videos_path', default="", required=True, help="video path for filtering")
     parser.add_argument('--result_path', type=str, default="./filter_results", help='result save path')
     parser.add_argument('--store_name', type=str, default="filtered_static_video.json", help='result file name')
-    parser.add_argument('--prompt_file', type=str, default="./VBench_full_info.json", help='static_prompt')
     parser.add_argument('--small', action='store_true', help='use small model')
     parser.add_argument('--mixed_precision', action='store_true', help='use mixed precision')
     parser.add_argument('--alternate_corr', action='store_true', help='use efficent correlation implementation')
-    parser.set_defaults(func=static_filter)
-
+    parser.add_argument('--filter_scope', default='temporal_flickering', help=f'''For specifying the scope for filtering videos
+        1. 'temporal_flickering' (default): filter videos based on matches with temporal_flickering dimension of VBench.
+        2. 'all': filter all video in the current directory.
+        3. '$filename': if a filepath to a JSON file is provided, only the filename exists in JSON file will be filtered.
+                >       usage: --filter_scope example.json
+    ''')
+    args = parser.parse_args()
+    return args
+
+if __name__ == "__main__":
+    args = parse_args()
+    static_filter(args)
```

### Comparing `vbench-0.1.1/vbench/cli/vbench.py` & `vbench-0.1.2/vbench/cli/vbench.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse
 import importlib
 import subprocess
 
 vbench_cmd = ['evaluate', 'static_filter']
 
 def main():
-    parser = argparse.ArgumentParser(prog="vbench")
+    parser = argparse.ArgumentParser(prog="vbench", formatter_class=argparse.RawTextHelpFormatter)
     subparsers = parser.add_subparsers(title='vbench subcommands')
 
     for cmd in vbench_cmd:
         module = importlib.import_module(f'vbench.cli.{cmd}')
         module.register_subparsers(subparsers)
     parser.set_defaults(func=help)
     args = parser.parse_args()
```

### Comparing `vbench-0.1.1/vbench/color.py` & `vbench-0.1.2/vbench/color.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,14 @@
                 success_frame_count_all += cur_success_frame_rate
                 video_count += 1
                 video_results.append({'video_path': video_path, 'video_results': cur_success_frame_rate})
     success_rate = success_frame_count_all / video_count
     return success_rate, video_results
         
 
-def compute_color(json_dir, device, submodules_dict):
+def compute_color(json_dir, device, submodules_dict, **kwargs):
     dense_caption_model = DenseCaptioning(device)
     dense_caption_model.initialize_model(**submodules_dict)
     logger.info("Initialize detection model success")
     _, prompt_dict_ls = load_dimension_info(json_dir, dimension='color', lang='en')
     all_results, video_results = color(dense_caption_model, prompt_dict_ls, device)
     return all_results, video_results
```

### Comparing `vbench-0.1.1/vbench/dynamic_degree.py` & `vbench-0.1.2/vbench/dynamic_degree.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,15 +136,15 @@
         video_results.append({'video_path': video_path, 'video_results': score_per_video})
         sim.append(score_per_video)
     avg_score = np.mean(sim)
     return avg_score, video_results
 
 
 
-def compute_dynamic_degree(json_dir, device, submodules_list):
+def compute_dynamic_degree(json_dir, device, submodules_list, **kwargs):
     model_path = submodules_list["model"] 
     # set_args
     args_new = edict({"model":model_path, "small":False, "mixed_precision":False, "alternate_corr":False})
     dynamic = DynamicDegree(args_new, device)
     video_list, _ = load_dimension_info(json_dir, dimension='dynamic_degree', lang='en')
     all_results, video_results = dynamic_degree(dynamic, video_list)
     return all_results, video_results
```

### Comparing `vbench-0.1.1/vbench/human_action.py` & `vbench-0.1.2/vbench/human_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,12 +91,12 @@
             pass
         video_results.append({'video_path': video_path, 'video_results': flag})
     # print(f"cor num: {cor_num}, total: {cnt}")
     acc = cor_num / cnt
     return acc, video_results
 
 
-def compute_human_action(json_dir, device, submodules_list):
+def compute_human_action(json_dir, device, submodules_list, **kwargs):
     umt_path = submodules_list[0]
     video_list, _ = load_dimension_info(json_dir, dimension='human_action', lang='en')
     all_results, video_results = human_action(umt_path, video_list, device)
     return all_results, video_results
```

### Comparing `vbench-0.1.1/vbench/motion_smoothness.py` & `vbench-0.1.2/vbench/motion_smoothness.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,14 +167,14 @@
         video_results.append({'video_path': video_path, 'video_results': score_per_video})
         sim.append(score_per_video)
     avg_score = np.mean(sim)
     return avg_score, video_results
 
 
 
-def compute_motion_smoothness(json_dir, device, submodules_list):
+def compute_motion_smoothness(json_dir, device, submodules_list, **kwargs):
     config = submodules_list["config"] # pretrained/amt_model/AMT-S.yaml
     ckpt = submodules_list["ckpt"] # pretrained/amt_model/amt-s.pth
     motion = MotionSmoothness(config, ckpt, device)
     video_list, _ = load_dimension_info(json_dir, dimension='motion_smoothness', lang='en')
     all_results, video_results = motion_smoothness(motion, video_list)
     return all_results, video_results
```

### Comparing `vbench-0.1.1/vbench/multiple_objects.py` & `vbench-0.1.2/vbench/multiple_objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,14 @@
             success_frame_count += cur_success_frame_count
             frame_count += len(cur_video_pred)
             video_results.append({'video_path': video_path, 'video_results': cur_success_frame_rate})
     success_rate = success_frame_count / frame_count
     return success_rate, video_results
         
 
-def compute_multiple_objects(json_dir, device, submodules_dict):
+def compute_multiple_objects(json_dir, device, submodules_dict, **kwargs):
     dense_caption_model = DenseCaptioning(device)
     dense_caption_model.initialize_model_det(**submodules_dict)
     logger.info("Initialize detection model success")
     _, prompt_dict_ls = load_dimension_info(json_dir, dimension='multiple_objects', lang='en')
     all_results, video_results = multiple_objects(dense_caption_model, prompt_dict_ls, device)
     return all_results, video_results
```

### Comparing `vbench-0.1.1/vbench/object_class.py` & `vbench-0.1.2/vbench/object_class.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,14 @@
             success_frame_count += cur_success_frame_count
             frame_count += len(cur_video_pred)
             video_results.append({'video_path': video_path, 'video_results': cur_success_frame_rate})
     success_rate = success_frame_count / frame_count
     return success_rate, video_results
         
 
-def compute_object_class(json_dir, device, submodules_dict):
+def compute_object_class(json_dir, device, submodules_dict, **kwargs):
     dense_caption_model = DenseCaptioning(device)
     dense_caption_model.initialize_model_det(**submodules_dict)
     logger.info("Initialize detection model success")
     _, prompt_dict_ls = load_dimension_info(json_dir, dimension='object_class', lang='en')
     all_results, video_results = object_class(dense_caption_model, prompt_dict_ls, device)
     return all_results, video_results
```

### Comparing `vbench-0.1.1/vbench/overall_consistency.py` & `vbench-0.1.2/vbench/overall_consistency.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,13 +49,13 @@
                 logit_per_text =  clip_feat @ text_feat.T
                 score_per_video =  float(logit_per_text[0][0].cpu())
                 sim.append(score_per_video)
                 video_results.append({'video_path': video_path, 'video_results': score_per_video})
     avg_score = np.mean(sim)
     return avg_score, video_results
 
-def compute_overall_consistency(json_dir, device, submodules_list):
+def compute_overall_consistency(json_dir, device, submodules_list, **kwargs):
     tokenizer = SimpleTokenizer(os.path.join(CACHE_DIR, "ViCLIP/bpe_simple_vocab_16e6.txt.gz"))
     viclip = ViCLIP(tokenizer= tokenizer, **submodules_list).to(device)
     _, video_dict = load_dimension_info(json_dir, dimension='overall_consistency', lang='en')
     all_results, video_results = overall_consistency(viclip, video_dict, tokenizer, device)
     return all_results, video_results
```

### Comparing `vbench-0.1.1/vbench/scene.py` & `vbench-0.1.2/vbench/scene.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             success_frame_count += cur_success_frame_count
             frame_count += len(cur_video_pred)
             video_results.append({'video_path': video_path, 'video_results': cur_success_frame_rate})
     success_rate = success_frame_count / frame_count
     return success_rate, video_results
         
 
-def compute_scene(json_dir, device, submodules_dict):
+def compute_scene(json_dir, device, submodules_dict, **kwargs):
     model = tag2text_caption(**submodules_dict)
     model.eval()
     model = model.to(device)
     logger.info("Initialize caption model success")
     _, prompt_dict_ls = load_dimension_info(json_dir, dimension='scene', lang='en')
     all_results, video_results = scene(model, prompt_dict_ls, device)
     return all_results, video_results
```

### Comparing `vbench-0.1.1/vbench/spatial_relationship.py` & `vbench-0.1.2/vbench/spatial_relationship.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,14 +117,14 @@
             cur_success_frame_rate = np.mean(cur_video_frame_score)
             frame_score_overall.extend(cur_video_frame_score)
             video_results.append({'video_path': video_path, 'video_results': cur_success_frame_rate, 'frame_results':cur_video_frame_score})
     success_rate = np.mean(frame_score_overall)
     return success_rate, video_results
         
 
-def compute_spatial_relationship(json_dir, device, submodules_dict):
+def compute_spatial_relationship(json_dir, device, submodules_dict, **kwargs):
     dense_caption_model = DenseCaptioning(device)
     dense_caption_model.initialize_model_det(**submodules_dict)
     logger.info("Initialize detection model success")
     _, prompt_dict_ls = load_dimension_info(json_dir, dimension='spatial_relationship', lang='en')
     all_results, video_results = spatial_relationship(dense_caption_model, prompt_dict_ls, device)
     return all_results, video_results
```

### Comparing `vbench-0.1.1/vbench/subject_consistency.py` & `vbench-0.1.2/vbench/subject_consistency.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,14 @@
         sim += video_sim
         video_results.append({'video_path': video_path, 'video_results': video_sim})
     sim_per_video = sim / (len(video_list) - 1)
     sim_per_frame = sim / cnt
     return sim_per_frame, video_results
 
 
-def compute_subject_consistency(json_dir, device, submodules_list):
+def compute_subject_consistency(json_dir, device, submodules_list, **kwargs):
     dino_model = torch.hub.load(**submodules_list).to(device)
     read_frame = submodules_list['read_frame']
     logger.info("Initialize DINO success")
     video_list, _ = load_dimension_info(json_dir, dimension='subject_consistency', lang='en')
     all_results, video_results = subject_consistency(dino_model, video_list, device, read_frame)
     return all_results, video_results
```

### Comparing `vbench-0.1.1/vbench/temporal_flickering.py` & `vbench-0.1.2/vbench/temporal_flickering.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             continue
         video_results.append({'video_path': video_path, 'video_results': score_per_video})
         sim.append(score_per_video)
     avg_score = np.mean(sim)
     return avg_score, video_results
 
 
-def compute_temporal_flickering(json_dir, device, submodules_list):
+def compute_temporal_flickering(json_dir, device, submodules_list, **kwargs):
     video_list, _ = load_dimension_info(json_dir, dimension='temporal_flickering', lang='en')
     all_results, video_results = temporal_flickering(video_list)
     return all_results, video_results
```

### Comparing `vbench-0.1.1/vbench/temporal_style.py` & `vbench-0.1.2/vbench/temporal_style.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,13 +50,13 @@
                 logit_per_text =  clip_feat @ text_feat.T
                 score_per_video =  float(logit_per_text[0][0].cpu())
                 sim.append(score_per_video)
                 video_results.append({'video_path': video_path, 'video_results': score_per_video})
     avg_score = np.mean(sim)
     return avg_score, video_results
 
-def compute_temporal_style(json_dir, device, submodules_list):
+def compute_temporal_style(json_dir, device, submodules_list, **kwargs):
     tokenizer = SimpleTokenizer(os.path.join(CACHE_DIR, "ViCLIP/bpe_simple_vocab_16e6.txt.gz"))
     viclip = ViCLIP(tokenizer= tokenizer, **submodules_list).to(device)
     _, video_dict = load_dimension_info(json_dir, dimension='temporal_style', lang='en')
     all_results, video_results = temporal_style(viclip, video_dict, tokenizer, device)
     return all_results, video_results
```

### Comparing `vbench-0.1.1/vbench/third_party/RAFT/core/corr.py` & `vbench-0.1.2/vbench/third_party/RAFT/core/corr.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/RAFT/core/datasets.py` & `vbench-0.1.2/vbench/third_party/RAFT/core/datasets.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/RAFT/core/extractor.py` & `vbench-0.1.2/vbench/third_party/RAFT/core/extractor.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/RAFT/core/raft.py` & `vbench-0.1.2/vbench/third_party/RAFT/core/raft.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/RAFT/core/update.py` & `vbench-0.1.2/vbench/third_party/RAFT/core/update.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/RAFT/core/utils_core/augmentor.py` & `vbench-0.1.2/vbench/third_party/RAFT/core/utils_core/augmentor.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/RAFT/core/utils_core/flow_viz.py` & `vbench-0.1.2/vbench/third_party/RAFT/core/utils_core/flow_viz.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/RAFT/core/utils_core/frame_utils.py` & `vbench-0.1.2/vbench/third_party/RAFT/core/utils_core/frame_utils.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/RAFT/core/utils_core/utils.py` & `vbench-0.1.2/vbench/third_party/RAFT/core/utils_core/utils.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/ViCLIP/simple_tokenizer.py` & `vbench-0.1.2/vbench/third_party/ViCLIP/simple_tokenizer.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/ViCLIP/viclip.py` & `vbench-0.1.2/vbench/third_party/ViCLIP/viclip.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/ViCLIP/viclip_text.py` & `vbench-0.1.2/vbench/third_party/ViCLIP/viclip_text.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/ViCLIP/viclip_vision.py` & `vbench-0.1.2/vbench/third_party/ViCLIP/viclip_vision.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/amt/benchmarks/adobe240.py` & `vbench-0.1.2/vbench/third_party/amt/benchmarks/adobe240.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/amt/benchmarks/gopro.py` & `vbench-0.1.2/vbench/third_party/amt/benchmarks/gopro.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/amt/benchmarks/snu_film.py` & `vbench-0.1.2/vbench/third_party/amt/benchmarks/snu_film.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/amt/benchmarks/speed_parameters.py` & `vbench-0.1.2/vbench/third_party/amt/benchmarks/speed_parameters.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/amt/benchmarks/ucf101.py` & `vbench-0.1.2/vbench/third_party/amt/benchmarks/ucf101.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/amt/benchmarks/vimeo90k.py` & `vbench-0.1.2/vbench/third_party/amt/benchmarks/vimeo90k.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/amt/benchmarks/vimeo90k_tta.py` & `vbench-0.1.2/vbench/third_party/amt/benchmarks/vimeo90k_tta.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/amt/benchmarks/xiph.py` & `vbench-0.1.2/vbench/third_party/amt/benchmarks/xiph.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/amt/cfgs/AMT-G.yaml` & `vbench-0.1.2/vbench/third_party/amt/cfgs/AMT-G.yaml`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/amt/cfgs/AMT-L.yaml` & `vbench-0.1.2/vbench/third_party/amt/cfgs/AMT-L.yaml`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/amt/cfgs/AMT-S.yaml` & `vbench-0.1.2/vbench/third_party/amt/cfgs/AMT-S.yaml`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/amt/cfgs/AMT-S_gopro.yaml` & `vbench-0.1.2/vbench/third_party/amt/cfgs/AMT-S_gopro.yaml`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/amt/cfgs/IFRNet.yaml` & `vbench-0.1.2/vbench/third_party/amt/cfgs/IFRNet.yaml`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/amt/datasets/adobe_datasets.py` & `vbench-0.1.2/vbench/third_party/amt/datasets/adobe_datasets.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/amt/datasets/gopro_datasets.py` & `vbench-0.1.2/vbench/third_party/amt/datasets/gopro_datasets.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/amt/datasets/vimeo_datasets.py` & `vbench-0.1.2/vbench/third_party/amt/datasets/vimeo_datasets.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/amt/flow_generation/gen_flow.py` & `vbench-0.1.2/vbench/third_party/amt/flow_generation/gen_flow.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/amt/flow_generation/liteflownet/run.py` & `vbench-0.1.2/vbench/third_party/amt/flow_generation/liteflownet/run.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/amt/losses/loss.py` & `vbench-0.1.2/vbench/third_party/amt/losses/loss.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/amt/metrics/psnr_ssim.py` & `vbench-0.1.2/vbench/third_party/amt/metrics/psnr_ssim.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/amt/networks/AMT-G.py` & `vbench-0.1.2/vbench/third_party/amt/networks/AMT-G.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from networks.blocks.raft import (
+from vbench.third_party.amt.networks.blocks.raft import (
     coords_grid,
     BasicUpdateBlock, BidirCorrBlock
 )
-from networks.blocks.feat_enc import (
+from vbench.third_party.amt.networks.blocks.feat_enc import (
     LargeEncoder
 )
-from networks.blocks.ifrnet import (
+from vbench.third_party.amt.networks.blocks.ifrnet import (
     resize,
     Encoder,
     InitDecoder,
     IntermediateDecoder
 )
-from networks.blocks.multi_flow import (
+from vbench.third_party.amt.networks.blocks.multi_flow import (
     multi_flow_combine,
     MultiFlowDecoder
 )
 
 
 class Model(nn.Module):
     def __init__(self,
```

### Comparing `vbench-0.1.1/vbench/third_party/amt/networks/AMT-L.py` & `vbench-0.1.2/vbench/third_party/amt/networks/AMT-L.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import torch
 import torch.nn as nn
-from networks.blocks.raft import (
+from vbench.third_party.amt.networks.blocks.raft import (
     coords_grid,
     BasicUpdateBlock, BidirCorrBlock
 )
-from networks.blocks.feat_enc import (
-    BasicEncoder
+from vbench.third_party.amt.networks.blocks.feat_enc import (
+    BasicEncoder,
 )
-from networks.blocks.ifrnet import (
+from vbench.third_party.amt.networks.blocks.ifrnet import (
     resize,
     Encoder,
     InitDecoder,
     IntermediateDecoder
 )
-from networks.blocks.multi_flow import (
+from vbench.third_party.amt.networks.blocks.multi_flow import (
     multi_flow_combine,
     MultiFlowDecoder
 )
 
-
 class Model(nn.Module):
     def __init__(self, 
                  corr_radius=3, 
                  corr_lvls=4, 
                  num_flows=5,
                  channels=[48, 64, 72, 128], 
                  skip_channels=48
@@ -148,8 +147,8 @@
             up_flow1_1 = up_flow1_1.reshape(b, self.num_flows, 2, h, w)
             return {
                 'imgt_pred': imgt_pred,
                 'flow0_pred': [up_flow0_1, up_flow0_2, up_flow0_3, up_flow0_4],
                 'flow1_pred': [up_flow1_1, up_flow1_2, up_flow1_3, up_flow1_4],
                 'ft_pred': [ft_1_, ft_2_, ft_3_],
             }
-    
+
```

### Comparing `vbench-0.1.1/vbench/third_party/amt/networks/AMT-S.py` & `vbench-0.1.2/vbench/third_party/amt/networks/AMT-S.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import torch
 import torch.nn as nn
-from networks.blocks.raft import (
+from vbench.third_party.amt.networks.blocks.raft import (
+    SmallUpdateBlock,
     coords_grid,
-    SmallUpdateBlock, BidirCorrBlock
+    BidirCorrBlock
 )
-from networks.blocks.feat_enc import (
+from vbench.third_party.amt.networks.blocks.feat_enc import (
     SmallEncoder
 )
-from networks.blocks.ifrnet import (
+from vbench.third_party.amt.networks.blocks.ifrnet import (
     resize,
     Encoder,
     InitDecoder,
     IntermediateDecoder
 )
-from networks.blocks.multi_flow import (
+from vbench.third_party.amt.networks.blocks.multi_flow import (
     multi_flow_combine,
     MultiFlowDecoder
 )
 
-
 class Model(nn.Module):
     def __init__(self, 
                  corr_radius=3, 
                  corr_lvls=4, 
                  num_flows=3, 
                  channels=[20, 32, 44, 56], 
                  skip_channels=20):
```

### Comparing `vbench-0.1.1/vbench/third_party/amt/networks/IFRNet.py` & `vbench-0.1.2/vbench/third_party/amt/networks/IFRNet.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 import torch.nn as nn
-from utils.flow_utils import warp
-from networks.blocks.ifrnet import (
+from vbench.third_party.amt.utils.flow_utils import warp
+from vbench.third_party.amt.networks.blocks.ifrnet import (
     convrelu, resize,
     ResBlock, 
 )
 
 
 class Encoder(nn.Module):
     def __init__(self):
```

### Comparing `vbench-0.1.1/vbench/third_party/amt/networks/blocks/feat_enc.py` & `vbench-0.1.2/vbench/third_party/amt/networks/blocks/feat_enc.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/amt/networks/blocks/ifrnet.py` & `vbench-0.1.2/vbench/third_party/amt/networks/blocks/ifrnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from utils.flow_utils import warp
+from vbench.third_party.amt.utils.flow_utils import warp
 
 
 def resize(x, scale_factor):
     return F.interpolate(x, scale_factor=scale_factor, mode="bilinear", align_corners=False)
 
 def convrelu(in_channels, out_channels, kernel_size=3, stride=1, padding=1, dilation=1, groups=1, bias=True):
     return nn.Sequential(
@@ -104,8 +104,8 @@
         f1_warp = warp(f1, flow1_in)
         f_in = torch.cat([ft_, f0_warp, f1_warp, flow0_in, flow1_in], 1)
         out = self.convblock(f_in)
         flow0, flow1 = torch.chunk(out[:, :4, ...], 2, 1)
         ft_ = out[:, 4:, ...]
         flow0 = flow0 + 2.0 * resize(flow0_in, scale_factor=2.0)
         flow1 = flow1 + 2.0 * resize(flow1_in, scale_factor=2.0)
-        return flow0, flow1, ft_
+        return flow0, flow1, ft_
```

### Comparing `vbench-0.1.1/vbench/third_party/amt/networks/blocks/multi_flow.py` & `vbench-0.1.2/vbench/third_party/amt/networks/blocks/multi_flow.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 import torch.nn as nn
-from utils.flow_utils import warp
-from networks.blocks.ifrnet import (
+from vbench.third_party.amt.utils.flow_utils import warp
+from vbench.third_party.amt.networks.blocks.ifrnet import (
     convrelu, resize,
     ResBlock,
 )
 
 
 def multi_flow_combine(comb_block, img0, img1, flow0, flow1, 
                        mask=None, img_res=None, mean=None):
@@ -62,8 +62,8 @@
         mask = torch.sigmoid(mask)
         
         flow0 = delta_flow0 + 2.0 * resize(flow0, scale_factor=2.0
                                            ).repeat(1, self.num_flows, 1, 1)
         flow1 = delta_flow1 + 2.0 * resize(flow1, scale_factor=2.0
                                            ).repeat(1, self.num_flows, 1, 1)
         
-        return flow0, flow1, mask, img_res
+        return flow0, flow1, mask, img_res
```

### Comparing `vbench-0.1.1/vbench/third_party/amt/networks/blocks/raft.py` & `vbench-0.1.2/vbench/third_party/amt/networks/blocks/raft.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/amt/train.py` & `vbench-0.1.2/vbench/third_party/amt/train.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/amt/trainers/base_trainer.py` & `vbench-0.1.2/vbench/third_party/amt/trainers/base_trainer.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/amt/trainers/logger.py` & `vbench-0.1.2/vbench/third_party/amt/trainers/logger.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/amt/utils/dist_utils.py` & `vbench-0.1.2/vbench/third_party/amt/utils/dist_utils.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/amt/utils/flow_utils.py` & `vbench-0.1.2/vbench/third_party/amt/utils/flow_utils.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/amt/utils/utils.py` & `vbench-0.1.2/vbench/third_party/amt/utils/utils.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_model.py` & `vbench-0.1.2/vbench/third_party/grit_model.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/__init__.py` & `vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/__init__.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/config.py` & `vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/config.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/backbone/bifpn.py` & `vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/backbone/bifpn.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/backbone/bifpn_fcos.py` & `vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/backbone/bifpn_fcos.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/backbone/dla.py` & `vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/backbone/dla.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/backbone/dlafpn.py` & `vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/backbone/dlafpn.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/backbone/fpn_p5.py` & `vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/backbone/fpn_p5.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/backbone/res2net.py` & `vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/backbone/res2net.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/debug.py` & `vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/debug.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/dense_heads/centernet.py` & `vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/dense_heads/centernet.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/dense_heads/centernet_head.py` & `vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/dense_heads/centernet_head.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/dense_heads/utils.py` & `vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/dense_heads/utils.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/layers/deform_conv.py` & `vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/layers/deform_conv.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/layers/heatmap_focal_loss.py` & `vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/layers/heatmap_focal_loss.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/layers/iou_loss.py` & `vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/layers/iou_loss.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/layers/ml_nms.py` & `vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/layers/ml_nms.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/meta_arch/centernet_detector.py` & `vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/meta_arch/centernet_detector.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/roi_heads/custom_fast_rcnn.py` & `vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/roi_heads/custom_fast_rcnn.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/roi_heads/custom_roi_heads.py` & `vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/roi_heads/custom_roi_heads.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/centernet/modeling/roi_heads/fed_loss.py` & `vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/centernet/modeling/roi_heads/fed_loss.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/configs/Base-CenterNet-FPN.yaml` & `vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/configs/Base-CenterNet-FPN.yaml`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/configs/Base-CenterNet2.yaml` & `vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/configs/Base-CenterNet2.yaml`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/configs/Base_S4_DLA.yaml` & `vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/configs/Base_S4_DLA.yaml`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_DLA-BiFPN-P3_24x.yaml` & `vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_DLA-BiFPN-P3_24x.yaml`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_DLA-BiFPN-P3_4x.yaml` & `vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_DLA-BiFPN-P3_4x.yaml`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_DLA-BiFPN-P5_640_16x.yaml` & `vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_DLA-BiFPN-P5_640_16x.yaml`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_DLA-BiFPN-P5_640_16x_ST.yaml` & `vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_DLA-BiFPN-P5_640_16x_ST.yaml`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_DLA-fcosBiFPN-P5_640_16x_ST.yaml` & `vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_DLA-fcosBiFPN-P5_640_16x_ST.yaml`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_R2-101-DCN-BiFPN_1280_4x.yaml` & `vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_R2-101-DCN-BiFPN_1280_4x.yaml`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_R2-101-DCN-BiFPN_4x+4x_1560_ST.yaml` & `vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_R2-101-DCN-BiFPN_4x+4x_1560_ST.yaml`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_R2-101-DCN_896_4x.yaml` & `vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_R2-101-DCN_896_4x.yaml`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_X101-DCN_2x.yaml` & `vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/configs/CenterNet2_X101-DCN_2x.yaml`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/configs/nuImages_CenterNet2_DLA_640_8x.yaml` & `vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/configs/nuImages_CenterNet2_DLA_640_8x.yaml`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/predictor.py` & `vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/predictor.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/CenterNet2/train_net.py` & `vbench-0.1.2/vbench/third_party/grit_src/CenterNet2/train_net.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/configs/Base.yaml` & `vbench-0.1.2/vbench/third_party/grit_src/configs/Base.yaml`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/configs/GRiT_B_DenseCap_ObjectDet.yaml` & `vbench-0.1.2/vbench/third_party/grit_src/configs/GRiT_B_DenseCap_ObjectDet.yaml`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/grit/config.py` & `vbench-0.1.2/vbench/third_party/grit_src/grit/config.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/grit/custom_solver.py` & `vbench-0.1.2/vbench/third_party/grit_src/grit/custom_solver.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/grit/data/custom_build_augmentation.py` & `vbench-0.1.2/vbench/third_party/grit_src/grit/data/custom_build_augmentation.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/grit/data/custom_dataset_dataloader.py` & `vbench-0.1.2/vbench/third_party/grit_src/grit/data/custom_dataset_dataloader.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/grit/data/custom_dataset_mapper.py` & `vbench-0.1.2/vbench/third_party/grit_src/grit/data/custom_dataset_mapper.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/grit/data/datasets/grit_coco.py` & `vbench-0.1.2/vbench/third_party/grit_src/grit/data/datasets/grit_coco.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/grit/data/datasets/object365.py` & `vbench-0.1.2/vbench/third_party/grit_src/grit/data/datasets/object365.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/grit/data/datasets/vg.py` & `vbench-0.1.2/vbench/third_party/grit_src/grit/data/datasets/vg.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/grit/data/transforms/custom_augmentation_impl.py` & `vbench-0.1.2/vbench/third_party/grit_src/grit/data/transforms/custom_augmentation_impl.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/grit/data/transforms/custom_transform.py` & `vbench-0.1.2/vbench/third_party/grit_src/grit/data/transforms/custom_transform.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/grit/modeling/backbone/utils.py` & `vbench-0.1.2/vbench/third_party/grit_src/grit/modeling/backbone/utils.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/grit/modeling/backbone/vit.py` & `vbench-0.1.2/vbench/third_party/grit_src/grit/modeling/backbone/vit.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/grit/modeling/meta_arch/grit.py` & `vbench-0.1.2/vbench/third_party/grit_src/grit/modeling/meta_arch/grit.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/grit/modeling/roi_heads/grit_fast_rcnn.py` & `vbench-0.1.2/vbench/third_party/grit_src/grit/modeling/roi_heads/grit_fast_rcnn.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/grit/modeling/roi_heads/grit_roi_heads.py` & `vbench-0.1.2/vbench/third_party/grit_src/grit/modeling/roi_heads/grit_roi_heads.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/grit/modeling/soft_nms.py` & `vbench-0.1.2/vbench/third_party/grit_src/grit/modeling/soft_nms.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/grit/modeling/text/file_utils.py` & `vbench-0.1.2/vbench/third_party/grit_src/grit/modeling/text/file_utils.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/grit/modeling/text/load_text_token.py` & `vbench-0.1.2/vbench/third_party/grit_src/grit/modeling/text/load_text_token.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/grit/modeling/text/modeling_bert.py` & `vbench-0.1.2/vbench/third_party/grit_src/grit/modeling/text/modeling_bert.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/grit/modeling/text/text_decoder.py` & `vbench-0.1.2/vbench/third_party/grit_src/grit/modeling/text/text_decoder.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/grit/predictor.py` & `vbench-0.1.2/vbench/third_party/grit_src/grit/predictor.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/grit_src/image_dense_captions.py` & `vbench-0.1.2/vbench/third_party/grit_src/image_dense_captions.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/tag2Text/med.py` & `vbench-0.1.2/vbench/third_party/tag2Text/med.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/tag2Text/q2l_config.json` & `vbench-0.1.2/vbench/third_party/tag2Text/q2l_config.json`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/tag2Text/swin_transformer.py` & `vbench-0.1.2/vbench/third_party/tag2Text/swin_transformer.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/tag2Text/tag2text.py` & `vbench-0.1.2/vbench/third_party/tag2Text/tag2text.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/tag2Text/tag_class.py` & `vbench-0.1.2/vbench/third_party/tag2Text/tag_class.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/tag2Text/vit.py` & `vbench-0.1.2/vbench/third_party/tag2Text/vit.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/umt/datasets/build.py` & `vbench-0.1.2/vbench/third_party/umt/datasets/build.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/umt/datasets/kinetics.py` & `vbench-0.1.2/vbench/third_party/umt/datasets/kinetics.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/umt/datasets/kinetics_sparse.py` & `vbench-0.1.2/vbench/third_party/umt/datasets/kinetics_sparse.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/umt/datasets/mae.py` & `vbench-0.1.2/vbench/third_party/umt/datasets/mae.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/umt/datasets/masking_generator.py` & `vbench-0.1.2/vbench/third_party/umt/datasets/masking_generator.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/umt/datasets/mixup.py` & `vbench-0.1.2/vbench/third_party/umt/datasets/mixup.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/umt/datasets/rand_augment.py` & `vbench-0.1.2/vbench/third_party/umt/datasets/rand_augment.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/umt/datasets/random_erasing.py` & `vbench-0.1.2/vbench/third_party/umt/datasets/random_erasing.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/umt/datasets/ssv2.py` & `vbench-0.1.2/vbench/third_party/umt/datasets/ssv2.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/umt/datasets/transforms.py` & `vbench-0.1.2/vbench/third_party/umt/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/umt/datasets/video_transforms.py` & `vbench-0.1.2/vbench/third_party/umt/datasets/video_transforms.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/umt/datasets/volume_transforms.py` & `vbench-0.1.2/vbench/third_party/umt/datasets/volume_transforms.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/umt/functional.py` & `vbench-0.1.2/vbench/third_party/umt/functional.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/umt/kinetics_400_categories.txt` & `vbench-0.1.2/vbench/third_party/umt/kinetics_400_categories.txt`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/umt/models/clip.py` & `vbench-0.1.2/vbench/third_party/umt/models/clip.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/umt/models/modeling_finetune.py` & `vbench-0.1.2/vbench/third_party/umt/models/modeling_finetune.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/umt/models/modeling_pretrain.py` & `vbench-0.1.2/vbench/third_party/umt/models/modeling_pretrain.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/third_party/umt/models/modeling_pretrain_umt.py` & `vbench-0.1.2/vbench/third_party/umt/models/modeling_pretrain_umt.py`

 * *Files identical despite different names*

### Comparing `vbench-0.1.1/vbench/utils.py` & `vbench-0.1.2/vbench/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 import json
 import numpy as np
 import logging
 import subprocess
 import torch
+import re
+from pathlib import Path
 from PIL import Image, ImageSequence
 from decord import VideoReader, cpu
 from torchvision import transforms
 from torchvision.transforms import Compose, Resize, CenterCrop, ToTensor, Normalize, ToPILImage
 try:
     from torchvision.transforms import InterpolationMode
     BICUBIC = InterpolationMode.BICUBIC
@@ -134,14 +136,16 @@
     elif video_path.endswith('.png'):
         frame = Image.open(video_path)
         frame = frame.convert('RGB')
         frame = np.array(frame).astype(np.uint8)
         frame_ls = [frame]
         buffer = np.array(frame_ls)
     elif video_path.endswith('.mp4'):
+        import decord
+        decord.bridge.set_bridge('native')
         if width:
             video_reader = VideoReader(video_path, width=width, height=height, num_threads=1)
         else:
             video_reader = VideoReader(video_path, num_threads=1)
         frames = video_reader.get_batch(range(len(video_reader)))  # (T, H, W, C), torch.uint8
 
         buffer = frames.asnumpy().astype(np.uint8)
@@ -349,15 +353,24 @@
                 "pretrain": f'{CACHE_DIR}/ViCLIP/ViClip-InternVid-10M-FLT.pth',
             }
             if not os.path.exists(submodules_dict[dimension]['pretrain']):
                 wget_command = ['wget', 'https://pjlab-gvm-data.oss-cn-shanghai.aliyuncs.com/internvideo/viclip/ViClip-InternVid-10M-FLT.pth', '-P', os.path.dirname(submodules_dict[dimension]["pretrain"])]
                 subprocess.run(wget_command, check=True)
     return submodules_dict
 
-
+def get_prompt_from_filename(path: str):
+    """
+    1. prompt-0.suffix -> prompt
+    2. prompt.suffix -> prompt
+    """
+    prompt = Path(path).stem
+    number_ending = r'-\d+$' # checks ending with -<number>
+    if re.search(number_ending, prompt):
+        return re.sub(number_ending, '', prompt)
+    return prompt
 
 def save_json(data, path, indent=4):
     with open(path, 'w', encoding='utf-8') as f:
         json.dump(data, f, indent=indent)
 
 def load_json(path):
     """
```

### Comparing `vbench-0.1.1/vbench.egg-info/PKG-INFO` & `vbench-0.1.2/vbench.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vbench
-Version: 0.1.1
+Version: 0.1.2
 Summary: Video generation benchmark
 License: Apache Software License 2.0
 Project-URL: Source, https://github.com/Vchitect/VBench
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Pillow
 Requires-Dist: numpy
@@ -58,14 +58,37 @@
    ```
    pip install detectron2@git+https://github.com/facebookresearch/detectron2.git
    ```
     
 If there is an error during [detectron2](https://github.com/facebookresearch/detectron2) installation, see [here](https://detectron2.readthedocs.io/en/latest/tutorials/install.html).
 
 ## Usage
+
+### Evaluate Your Own Videos
+We support evaluating any video. Simply provide the path to the video file, or the path to the folder that contains your videos. There is no requirement on the videos' names.
+- Note: We support customized videos / prompts for the following dimensions: `'subject_consistency', 'background_consistency', 'motion_smoothness', 'dynamic_degree', 'aesthetic_quality', 'imaging_quality'`
+
+
+To evaluate videos with customed input prompt, run our script with `--mode=custom_input`:
+```
+python evaluate.py \
+    --dimension $DIMENSION \
+    --videos_path /path/to/folder_or_video/ \
+    --mode=custom_input
+```
+alternatively you can use our command:
+```
+vbench evaluate \
+    --dimension $DIMENSION \
+    --videos_path /path/to/folder_or_video/ \
+    --mode=custom_input
+```
+
+### Evaluation on the Standard Prompt Suite of VBench
+
 ##### command line 
 ```bash
     vbench evaluate --videos_path $VIDEO_PATH --dimension $DIMENSION
 ```
 For example:
 ```bash
     vbench evaluate --videos_path "sampled_videos/lavie/human_action" --dimension "human_action"
@@ -79,22 +102,40 @@
         name = <name>,
         dimension_list = [<dimension>, <dimension>, ...],
     )
 ```
 For example: 
 ```python
     from vbench import VBench
-    my_VBench = VBench(device, "VBench_full_info.json", "evaluation_results")
+    my_VBench = VBench(device, "vbench/VBench_full_info.json", "evaluation_results")
     my_VBench.evaluate(
         videos_path = "sampled_videos/lavie/human_action",
         name = "lavie_human_action",
         dimension_list = ["human_action"],
     )
 ```
 
+### Evaluation on a specific category from VBench
+
+##### command line 
+```bash
+vbench evaluate \
+    --videos_path $VIDEO_PATH \
+    --dimension $DIMENSION \
+    --mode=vbench_category \
+    --category=$CATEGORY
+```
+or 
+```
+python evaluate.py \
+    --dimension $DIMENSION \
+    --videos_path /path/to/folder_or_video/ \
+    --mode=vbench_category
+```
+
 ## Prompt Suite
 
 We provide prompt lists are at `prompts/`. 
 
 Check out [details of prompt suites](https://github.com/Vchitect/VBench/tree/master/prompts), and instructions for [**how to sample videos for evaluation**](https://github.com/Vchitect/VBench/tree/master/prompts).
 
 ## Citation
```

### Comparing `vbench-0.1.1/vbench.egg-info/SOURCES.txt` & `vbench-0.1.2/vbench.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 bin/evaluate
+competitions/__init__.py
+competitions/clip_score.py
+competitions/competition_utils.py
+competitions/run_eval.py
+vbench/VBench_full_info.json
 vbench/__init__.py
 vbench/aesthetic_quality.py
 vbench/appearance_style.py
 vbench/background_consistency.py
 vbench/color.py
 vbench/dynamic_degree.py
 vbench/human_action.py
@@ -215,8 +220,43 @@
 vbench/third_party/umt/datasets/transforms.py
 vbench/third_party/umt/datasets/video_transforms.py
 vbench/third_party/umt/datasets/volume_transforms.py
 vbench/third_party/umt/models/__init__.py
 vbench/third_party/umt/models/clip.py
 vbench/third_party/umt/models/modeling_finetune.py
 vbench/third_party/umt/models/modeling_pretrain.py
-vbench/third_party/umt/models/modeling_pretrain_umt.py
+vbench/third_party/umt/models/modeling_pretrain_umt.py
+vbench2_beta_i2v/__init__.py
+vbench2_beta_i2v/camera_motion.py
+vbench2_beta_i2v/crop_to_diff_ratio.py
+vbench2_beta_i2v/i2v_background.py
+vbench2_beta_i2v/i2v_subject.py
+vbench2_beta_i2v/utils.py
+vbench2_beta_long/__init__.py
+vbench2_beta_long/aesthetic_quality.py
+vbench2_beta_long/appearance_style.py
+vbench2_beta_long/background_consistency.py
+vbench2_beta_long/color.py
+vbench2_beta_long/dynamic_degree.py
+vbench2_beta_long/eval_long.py
+vbench2_beta_long/human_action.py
+vbench2_beta_long/imaging_quality.py
+vbench2_beta_long/motion_smoothness.py
+vbench2_beta_long/multiple_objects.py
+vbench2_beta_long/object_class.py
+vbench2_beta_long/overall_consistency.py
+vbench2_beta_long/scene.py
+vbench2_beta_long/spatial_relationship.py
+vbench2_beta_long/static_filter.py
+vbench2_beta_long/subject_consistency.py
+vbench2_beta_long/temporal_flickering.py
+vbench2_beta_long/temporal_style.py
+vbench2_beta_long/utils.py
+vbench2_beta_trustworthiness/__init__.py
+vbench2_beta_trustworthiness/culture_fairness.py
+vbench2_beta_trustworthiness/gender_bias.py
+vbench2_beta_trustworthiness/safety.py
+vbench2_beta_trustworthiness/skin_bias.py
+vbench2_beta_trustworthiness/utils.py
+vbench2_beta_trustworthiness/third_party/__init__.py
+vbench2_beta_trustworthiness/third_party/nudenet/__init__.py
+vbench2_beta_trustworthiness/third_party/nudenet/nudenet.py
```

