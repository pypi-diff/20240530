# Comparing `tmp/alabamaencoder-0.4.3.tar.gz` & `tmp/alabamaencoder-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alabamaencoder-0.4.3.tar", last modified: Tue May 28 14:27:46 2024, max compression
+gzip compressed data, was "alabamaencoder-0.5.0.tar", last modified: Thu May 30 16:09:21 2024, max compression
```

## Comparing `alabamaencoder-0.4.3.tar` & `alabamaencoder-0.5.0.tar`

### file list

```diff
@@ -1,168 +1,163 @@
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.910324 alabamaencoder-0.4.3/
--rw-r--r--   0 kokoniara  (1000) kokoniara  (1000)      407 2024-05-28 14:27:46.910324 alabamaencoder-0.4.3/PKG-INFO
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.882323 alabamaencoder-0.4.3/alabamaEncode/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2021-04-17 09:55:33.000000 alabamaencoder-0.4.3/alabamaEncode/__init__.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.882323 alabamaencoder-0.4.3/alabamaEncode/ai_vmaf/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-03 08:49:47.000000 alabamaencoder-0.4.3/alabamaEncode/ai_vmaf/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1554 2023-12-13 17:07:22.000000 alabamaencoder-0.4.3/alabamaEncode/ai_vmaf/aom_firstpass.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1026 2023-12-18 07:05:43.000000 alabamaencoder-0.4.3/alabamaEncode/ai_vmaf/perdict.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.882323 alabamaencoder-0.4.3/alabamaEncode/ai_vmaf/train/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-03 10:35:40.000000 alabamaencoder-0.4.3/alabamaEncode/ai_vmaf/train/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    12402 2023-12-14 22:03:21.000000 alabamaencoder-0.4.3/alabamaEncode/ai_vmaf/train/train.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.882323 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 16:25:35.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/__init__.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.886324 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 16:26:35.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/__init__.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.886324 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/analyze_steps/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-01-17 00:34:57.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/analyze_steps/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      671 2024-01-17 00:37:48.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/analyze_steps/capped_crf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1064 2024-01-17 00:37:48.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/analyze_steps/manual_crf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3401 2024-03-05 22:28:46.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/analyze_steps/multires_encode_candidates.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4061 2024-02-04 12:03:51.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/analyze_steps/optimised_vbr.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    10661 2024-04-29 21:50:58.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/analyze_steps/per_scene_grain.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      597 2024-01-17 00:37:48.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_crf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      606 2024-01-17 00:37:48.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_vbr.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5578 2024-05-03 21:10:20.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/analyze_steps/target_vmaf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      448 2023-12-10 19:05:23.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/chunk_analyse_step.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      623 2023-12-05 14:54:46.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/final_encode_step.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.890324 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-05 14:55:01.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      684 2024-01-17 00:37:48.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/ai_targeted_vmaf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1584 2024-01-17 00:37:48.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/capped_crf_encode.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11063 2024-04-22 19:10:58.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6476 2024-02-04 12:12:23.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf_vbr.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2292 2024-03-05 22:27:27.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/multires_encode_finals.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      850 2024-05-28 14:05:00.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/plain.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2362 2024-05-20 19:14:36.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/opinionated_vmaf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5927 2024-03-05 22:32:37.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/pipelines.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      133 2024-01-15 01:49:31.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/refine_step.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.890324 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/refine_steps/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-01-14 19:17:26.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/refine_steps/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4955 2024-03-05 20:43:08.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/refine_steps/multires_package.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7817 2024-01-20 18:40:41.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/refine_steps/multires_trellis.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.890324 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 16:26:49.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1563 2024-05-20 13:32:49.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/args_tune.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4687 2024-04-27 00:03:05.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/autocrop.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      552 2024-01-25 02:38:21.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/denoise_filtering.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2409 2024-05-04 17:38:16.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/encoding_tiles.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     9823 2024-02-04 12:39:56.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/ideal_crf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7511 2024-02-12 05:33:32.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/scrape_hdr_meta.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5986 2024-03-05 22:00:10.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/sequence_autograin.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3119 2024-02-02 18:54:38.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/taget_ssimdb.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6920 2024-02-04 12:09:55.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/target_bitrate_optimisation.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3103 2024-05-27 06:22:04.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/x264_tune.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.894324 alabamaencoder-0.4.3/alabamaEncode/core/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-11-19 23:19:38.000000 alabamaencoder-0.4.3/alabamaEncode/core/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    10874 2024-05-28 14:05:00.000000 alabamaencoder-0.4.3/alabamaEncode/core/alabama.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2890 2024-05-25 18:25:00.000000 alabamaencoder-0.4.3/alabamaEncode/core/bin_utils.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3878 2024-05-02 23:47:10.000000 alabamaencoder-0.4.3/alabamaEncode/core/chunk_job.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4947 2024-01-31 09:31:42.000000 alabamaencoder-0.4.3/alabamaEncode/core/cli_executor.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.894324 alabamaencoder-0.4.3/alabamaEncode/core/extras/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-24 18:44:15.000000 alabamaencoder-0.4.3/alabamaEncode/core/extras/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    12734 2024-05-26 19:36:14.000000 alabamaencoder-0.4.3/alabamaEncode/core/extras/auto_thumbnailer.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    13706 2024-03-22 06:24:59.000000 alabamaencoder-0.4.3/alabamaEncode/core/ffmpeg.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5661 2024-05-07 20:56:31.000000 alabamaencoder-0.4.3/alabamaEncode/core/final_touches.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    19276 2024-05-04 17:36:30.000000 alabamaencoder-0.4.3/alabamaEncode/core/job.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1877 2024-04-22 19:11:27.000000 alabamaencoder-0.4.3/alabamaEncode/core/kv.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      813 2023-11-25 00:35:54.000000 alabamaencoder-0.4.3/alabamaEncode/core/path.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      556 2023-11-12 21:29:16.000000 alabamaencoder-0.4.3/alabamaEncode/core/timer.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1776 2023-12-24 03:53:49.000000 alabamaencoder-0.4.3/alabamaEncode/core/ws_update.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.894324 alabamaencoder-0.4.3/alabamaEncode/encoder/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-09-27 12:09:43.000000 alabamaencoder-0.4.3/alabamaEncode/encoder/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      748 2024-01-17 00:16:49.000000 alabamaencoder-0.4.3/alabamaEncode/encoder/codec.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11438 2024-04-26 23:55:50.000000 alabamaencoder-0.4.3/alabamaEncode/encoder/encoder.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1536 2024-02-12 05:37:04.000000 alabamaencoder-0.4.3/alabamaEncode/encoder/encoder_factory.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.898324 alabamaencoder-0.4.3/alabamaEncode/encoder/impl/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4369 2024-02-12 05:35:10.000000 alabamaencoder-0.4.3/alabamaEncode/encoder/impl/Aomenc.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2087 2024-02-12 05:35:10.000000 alabamaencoder-0.4.3/alabamaEncode/encoder/impl/Nvenc.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1586 2024-01-28 06:23:47.000000 alabamaencoder-0.4.3/alabamaEncode/encoder/impl/SvtAvif.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7662 2024-05-25 18:25:47.000000 alabamaencoder-0.4.3/alabamaEncode/encoder/impl/Svtenc.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2172 2024-02-12 05:35:10.000000 alabamaencoder-0.4.3/alabamaEncode/encoder/impl/VaapiH264.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2114 2024-03-23 06:39:42.000000 alabamaencoder-0.4.3/alabamaEncode/encoder/impl/VaapiH265.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7238 2024-02-12 05:35:10.000000 alabamaencoder-0.4.3/alabamaEncode/encoder/impl/X264.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4097 2024-02-12 05:35:10.000000 alabamaencoder-0.4.3/alabamaEncode/encoder/impl/X265.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2022-12-05 03:43:14.000000 alabamaencoder-0.4.3/alabamaEncode/encoder/impl/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2033 2024-02-12 05:35:10.000000 alabamaencoder-0.4.3/alabamaEncode/encoder/impl/rav1e.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3557 2024-02-12 05:35:10.000000 alabamaencoder-0.4.3/alabamaEncode/encoder/impl/vp9.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      269 2024-01-17 00:14:46.000000 alabamaencoder-0.4.3/alabamaEncode/encoder/rate_dist.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2494 2024-02-04 12:07:28.000000 alabamaencoder-0.4.3/alabamaEncode/encoder/stats.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.902324 alabamaencoder-0.4.3/alabamaEncode/experiments/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3713 2023-12-11 23:14:15.000000 alabamaencoder-0.4.3/alabamaEncode/experiments/Aq.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4337 2023-12-11 23:14:15.000000 alabamaencoder-0.4.3/alabamaEncode/experiments/Overlays.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2950 2024-02-02 15:19:02.000000 alabamaencoder-0.4.3/alabamaEncode/experiments/Svtav1Speed.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5719 2023-12-11 23:14:15.000000 alabamaencoder-0.4.3/alabamaEncode/experiments/Svtav1Tunes.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3749 2023-12-11 23:14:15.000000 alabamaencoder-0.4.3/alabamaEncode/experiments/TemporalFiltering.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-04-06 18:23:30.000000 alabamaencoder-0.4.3/alabamaEncode/experiments/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2496 2023-12-02 16:35:17.000000 alabamaencoder-0.4.3/alabamaEncode/experiments/ai_feature_extract.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      319 2023-12-10 22:37:13.000000 alabamaencoder-0.4.3/alabamaEncode/experiments/aom_extract.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5812 2024-02-04 12:09:55.000000 alabamaencoder-0.4.3/alabamaEncode/experiments/convexhull.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    16885 2024-02-04 12:09:55.000000 alabamaencoder-0.4.3/alabamaEncode/experiments/crf_vmaf_relation.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4941 2024-02-04 12:09:55.000000 alabamaencoder-0.4.3/alabamaEncode/experiments/denoise.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2210 2024-02-04 12:09:55.000000 alabamaencoder-0.4.3/alabamaEncode/experiments/sequence_convex.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      254 2023-12-20 04:58:54.000000 alabamaencoder-0.4.3/alabamaEncode/experiments/serialise_context.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      793 2023-12-31 13:08:11.000000 alabamaencoder-0.4.3/alabamaEncode/experiments/streaming_output.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6592 2023-12-11 23:14:15.000000 alabamaencoder-0.4.3/alabamaEncode/experiments/superres.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4106 2023-11-15 20:26:48.000000 alabamaencoder-0.4.3/alabamaEncode/experiments/target_vmaf.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.902324 alabamaencoder-0.4.3/alabamaEncode/experiments/util/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11478 2024-02-04 12:09:55.000000 alabamaencoder-0.4.3/alabamaEncode/experiments/util/ExperimentUtil.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-10-17 18:48:28.000000 alabamaencoder-0.4.3/alabamaEncode/experiments/util/__init__.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.902324 alabamaencoder-0.4.3/alabamaEncode/ffmpeg_source/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-21 17:50:35.000000 alabamaencoder-0.4.3/alabamaEncode/ffmpeg_source/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      837 2024-05-26 19:36:20.000000 alabamaencoder-0.4.3/alabamaEncode/ffmpeg_source/ffmpeg_src.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3758 2024-05-25 22:57:08.000000 alabamaencoder-0.4.3/alabamaEncode/ffmpeg_source/yuv.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.906324 alabamaencoder-0.4.3/alabamaEncode/metrics/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-11-17 22:15:46.000000 alabamaencoder-0.4.3/alabamaEncode/metrics/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5237 2024-02-04 12:44:56.000000 alabamaencoder-0.4.3/alabamaEncode/metrics/calculate.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      911 2023-11-22 22:07:47.000000 alabamaencoder-0.4.3/alabamaEncode/metrics/comparison_display.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      384 2024-01-26 03:01:39.000000 alabamaencoder-0.4.3/alabamaEncode/metrics/exception.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3033 2023-11-19 23:24:09.000000 alabamaencoder-0.4.3/alabamaEncode/metrics/image.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.906324 alabamaencoder-0.4.3/alabamaEncode/metrics/impl/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-02-04 12:02:29.000000 alabamaencoder-0.4.3/alabamaEncode/metrics/impl/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      924 2023-11-19 23:28:00.000000 alabamaencoder-0.4.3/alabamaEncode/metrics/impl/psnr.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1432 2023-11-25 03:14:34.000000 alabamaencoder-0.4.3/alabamaEncode/metrics/impl/ssim.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3093 2024-02-05 00:20:43.000000 alabamaencoder-0.4.3/alabamaEncode/metrics/impl/ssimu2.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     9078 2024-05-28 13:30:59.000000 alabamaencoder-0.4.3/alabamaEncode/metrics/impl/vmaf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      117 2024-02-04 12:09:55.000000 alabamaencoder-0.4.3/alabamaEncode/metrics/metric.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      373 2024-02-04 12:36:30.000000 alabamaencoder-0.4.3/alabamaEncode/metrics/options.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      308 2024-02-02 14:53:33.000000 alabamaencoder-0.4.3/alabamaEncode/metrics/result.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.906324 alabamaencoder-0.4.3/alabamaEncode/parallelEncoding/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2357 2024-01-07 02:35:39.000000 alabamaencoder-0.4.3/alabamaEncode/parallelEncoding/CeleryApp.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3848 2023-11-19 23:24:09.000000 alabamaencoder-0.4.3/alabamaEncode/parallelEncoding/CeleryAutoscaler.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-04-16 16:38:33.000000 alabamaencoder-0.4.3/alabamaEncode/parallelEncoding/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      148 2023-11-05 09:04:10.000000 alabamaencoder-0.4.3/alabamaEncode/parallelEncoding/command.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    12819 2024-04-21 00:03:18.000000 alabamaencoder-0.4.3/alabamaEncode/parallelEncoding/execute_commands.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      581 2024-01-07 00:27:19.000000 alabamaencoder-0.4.3/alabamaEncode/parallelEncoding/worker.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.906324 alabamaencoder-0.4.3/alabamaEncode/scene/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-04-15 20:18:27.000000 alabamaencoder-0.4.3/alabamaEncode/scene/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1810 2024-03-29 15:35:11.000000 alabamaencoder-0.4.3/alabamaEncode/scene/annel.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     9690 2024-05-04 17:06:53.000000 alabamaencoder-0.4.3/alabamaEncode/scene/chunk.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    13428 2024-05-25 14:27:51.000000 alabamaencoder-0.4.3/alabamaEncode/scene/concat.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4451 2024-05-04 17:06:53.000000 alabamaencoder-0.4.3/alabamaEncode/scene/sequence.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11219 2024-05-04 17:23:39.000000 alabamaencoder-0.4.3/alabamaEncode/scene/split.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.910324 alabamaencoder-0.4.3/alabamaEncode_frontends/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-23 05:32:46.000000 alabamaencoder-0.4.3/alabamaEncode_frontends/__init__.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.910324 alabamaencoder-0.4.3/alabamaEncode_frontends/cli/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-23 05:52:09.000000 alabamaencoder-0.4.3/alabamaEncode_frontends/cli/__init__.py
--rwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)     4705 2024-05-26 19:26:41.000000 alabamaencoder-0.4.3/alabamaEncode_frontends/cli/__main__.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.910324 alabamaencoder-0.4.3/alabamaEncode_frontends/cli/cli_setup/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 18:44:18.000000 alabamaencoder-0.4.3/alabamaEncode_frontends/cli/cli_setup/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4150 2024-03-05 20:36:01.000000 alabamaencoder-0.4.3/alabamaEncode_frontends/cli/cli_setup/autopaths.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    20449 2024-05-28 14:05:00.000000 alabamaencoder-0.4.3/alabamaEncode_frontends/cli/cli_setup/cli_args.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1162 2024-03-05 20:46:37.000000 alabamaencoder-0.4.3/alabamaEncode_frontends/cli/cli_setup/paths.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1088 2024-01-23 00:24:16.000000 alabamaencoder-0.4.3/alabamaEncode_frontends/cli/cli_setup/ratecontrol.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1130 2023-12-10 18:44:44.000000 alabamaencoder-0.4.3/alabamaEncode_frontends/cli/cli_setup/res_preset.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1987 2024-05-04 17:19:56.000000 alabamaencoder-0.4.3/alabamaEncode_frontends/cli/cli_setup/validate_files.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1177 2024-03-17 23:12:31.000000 alabamaencoder-0.4.3/alabamaEncode_frontends/cli/cli_setup/video_filters.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.910324 alabamaencoder-0.4.3/alabamaEncode_frontends/demon/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-23 05:38:55.000000 alabamaencoder-0.4.3/alabamaEncode_frontends/demon/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2289 2024-03-05 20:43:08.000000 alabamaencoder-0.4.3/alabamaEncode_frontends/demon/demon.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.910324 alabamaencoder-0.4.3/alabamaEncoder.egg-info/
--rw-r--r--   0 kokoniara  (1000) kokoniara  (1000)      407 2024-05-28 14:27:46.000000 alabamaencoder-0.4.3/alabamaEncoder.egg-info/PKG-INFO
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6166 2024-05-28 14:27:46.000000 alabamaencoder-0.4.3/alabamaEncoder.egg-info/SOURCES.txt
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        1 2024-05-28 14:27:46.000000 alabamaencoder-0.4.3/alabamaEncoder.egg-info/dependency_links.txt
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)       77 2024-05-28 14:27:46.000000 alabamaencoder-0.4.3/alabamaEncoder.egg-info/entry_points.txt
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      139 2024-05-28 14:27:46.000000 alabamaencoder-0.4.3/alabamaEncoder.egg-info/requires.txt
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)       38 2024-05-28 14:27:46.000000 alabamaencoder-0.4.3/alabamaEncoder.egg-info/top_level.txt
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)       38 2024-05-28 14:27:46.910324 alabamaencoder-0.4.3/setup.cfg
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      574 2024-05-28 14:15:56.000000 alabamaencoder-0.4.3/setup.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.202224 alabamaencoder-0.5.0/
+-rw-r--r--   0 kokoniara  (1000) kokoniara  (1000)      377 2024-05-30 16:09:21.202224 alabamaencoder-0.5.0/PKG-INFO
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.182223 alabamaencoder-0.5.0/alabamaEncode/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2021-04-17 09:55:33.000000 alabamaencoder-0.5.0/alabamaEncode/__init__.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.182223 alabamaencoder-0.5.0/alabamaEncode/ai_vmaf/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-03 08:49:47.000000 alabamaencoder-0.5.0/alabamaEncode/ai_vmaf/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1564 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/ai_vmaf/aom_firstpass.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1026 2023-12-18 07:05:43.000000 alabamaencoder-0.5.0/alabamaEncode/ai_vmaf/perdict.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.182223 alabamaencoder-0.5.0/alabamaEncode/ai_vmaf/train/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-03 10:35:40.000000 alabamaencoder-0.5.0/alabamaEncode/ai_vmaf/train/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    12402 2023-12-14 22:03:21.000000 alabamaencoder-0.5.0/alabamaEncode/ai_vmaf/train/train.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.182223 alabamaencoder-0.5.0/alabamaEncode/cli/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-23 05:52:09.000000 alabamaencoder-0.5.0/alabamaEncode/cli/__init__.py
+-rwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)     4898 2024-05-30 02:35:51.000000 alabamaencoder-0.5.0/alabamaEncode/cli/__main__.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.182223 alabamaencoder-0.5.0/alabamaEncode/cli/cli_setup/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 18:44:18.000000 alabamaencoder-0.5.0/alabamaEncode/cli/cli_setup/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4150 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/cli/cli_setup/autopaths.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    19457 2024-05-30 13:15:45.000000 alabamaencoder-0.5.0/alabamaEncode/cli/cli_setup/cli_args.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1162 2024-03-05 20:46:37.000000 alabamaencoder-0.5.0/alabamaEncode/cli/cli_setup/paths.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      795 2024-05-30 02:02:54.000000 alabamaencoder-0.5.0/alabamaEncode/cli/cli_setup/ratecontrol.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1130 2023-12-10 18:44:44.000000 alabamaencoder-0.5.0/alabamaEncode/cli/cli_setup/res_preset.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1992 2024-05-30 02:17:46.000000 alabamaencoder-0.5.0/alabamaEncode/cli/cli_setup/validate_files.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1182 2024-05-30 02:17:46.000000 alabamaencoder-0.5.0/alabamaEncode/cli/cli_setup/video_filters.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.182223 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 16:25:35.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/__init__.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.186223 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 16:26:35.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/__init__.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.186223 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/analyze_steps/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-01-17 00:34:57.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/analyze_steps/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1064 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/analyze_steps/manual_crf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3401 2024-03-05 22:28:46.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/analyze_steps/multires_encode_candidates.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4061 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/analyze_steps/optimised_vbr.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    10641 2024-05-30 02:25:07.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/analyze_steps/per_scene_grain.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      597 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_crf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      606 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_vbr.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5578 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/analyze_steps/target_vmaf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      448 2023-12-10 19:05:23.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/chunk_analyse_step.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      623 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/final_encode_step.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.186223 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/final_encode_steps/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-05 14:55:01.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/final_encode_steps/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11063 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6476 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf_vbr.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2292 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/final_encode_steps/multires_encode_finals.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      850 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/final_encode_steps/plain.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2487 2024-05-29 18:57:24.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/opinionated_vmaf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4887 2024-05-30 02:10:49.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/pipelines.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      133 2024-01-15 01:49:31.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/refine_step.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.186223 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/refine_steps/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-01-14 19:17:26.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/refine_steps/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4965 2024-05-30 02:18:47.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/refine_steps/multires_package.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7817 2024-01-20 18:40:41.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/refine_steps/multires_trellis.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.186223 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/sequence/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 16:26:49.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/sequence/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1563 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/sequence/args_tune.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4702 2024-05-30 02:23:07.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/sequence/autocrop.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      552 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/sequence/denoise_filtering.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2409 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/sequence/encoding_tiles.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7516 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/sequence/scrape_hdr_meta.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6001 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/sequence/sequence_autograin.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3092 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/sequence/taget_ssimdb.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3103 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/sequence/x264_tune.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.190224 alabamaencoder-0.5.0/alabamaEncode/core/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-11-19 23:19:38.000000 alabamaencoder-0.5.0/alabamaEncode/core/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3885 2024-05-30 02:29:55.000000 alabamaencoder-0.5.0/alabamaEncode/core/chunk_job.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    10534 2024-05-30 02:18:05.000000 alabamaencoder-0.5.0/alabamaEncode/core/context.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.190224 alabamaencoder-0.5.0/alabamaEncode/core/extras/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-24 18:44:15.000000 alabamaencoder-0.5.0/alabamaEncode/core/extras/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    12749 2024-05-30 02:32:33.000000 alabamaencoder-0.5.0/alabamaEncode/core/extras/auto_thumbnailer.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1776 2023-12-24 03:53:49.000000 alabamaencoder-0.5.0/alabamaEncode/core/extras/ws_update.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    13723 2024-05-30 02:32:32.000000 alabamaencoder-0.5.0/alabamaEncode/core/ffmpeg.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5676 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/core/final_touches.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    19233 2024-05-30 02:36:52.000000 alabamaencoder-0.5.0/alabamaEncode/core/job.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.190224 alabamaencoder-0.5.0/alabamaEncode/core/util/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 02:17:11.000000 alabamaencoder-0.5.0/alabamaEncode/core/util/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      125 2024-05-30 02:20:37.000000 alabamaencoder-0.5.0/alabamaEncode/core/util/abort_controler.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2895 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/core/util/bin_utils.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4947 2024-01-31 09:31:42.000000 alabamaencoder-0.5.0/alabamaEncode/core/util/cli_executor.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      773 2024-05-30 02:32:32.000000 alabamaencoder-0.5.0/alabamaEncode/core/util/get_yuv_stream.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1877 2024-04-22 19:11:27.000000 alabamaencoder-0.5.0/alabamaEncode/core/util/kv.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      813 2023-11-25 00:35:54.000000 alabamaencoder-0.5.0/alabamaEncode/core/util/path.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      556 2023-11-12 21:29:16.000000 alabamaencoder-0.5.0/alabamaEncode/core/util/timer.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3758 2024-05-25 22:57:08.000000 alabamaencoder-0.5.0/alabamaEncode/core/util/yuv.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.190224 alabamaencoder-0.5.0/alabamaEncode/demon/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-23 05:38:55.000000 alabamaencoder-0.5.0/alabamaEncode/demon/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2289 2024-03-05 20:43:08.000000 alabamaencoder-0.5.0/alabamaEncode/demon/demon.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.190224 alabamaencoder-0.5.0/alabamaEncode/encoder/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-09-27 12:09:43.000000 alabamaencoder-0.5.0/alabamaEncode/encoder/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      748 2024-01-17 00:16:49.000000 alabamaencoder-0.5.0/alabamaEncode/encoder/codec.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11448 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/encoder/encoder.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1628 2024-05-29 16:04:18.000000 alabamaencoder-0.5.0/alabamaEncode/encoder/encoder_factory.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.194224 alabamaencoder-0.5.0/alabamaEncode/encoder/impl/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4379 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/encoder/impl/Aomenc.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2092 2024-05-30 02:18:47.000000 alabamaencoder-0.5.0/alabamaEncode/encoder/impl/Nvenc.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1596 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/encoder/impl/SvtAvif.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7672 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/encoder/impl/Svtenc.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2177 2024-05-30 02:18:47.000000 alabamaencoder-0.5.0/alabamaEncode/encoder/impl/VaapiH264.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2119 2024-05-30 02:18:47.000000 alabamaencoder-0.5.0/alabamaEncode/encoder/impl/VaapiH265.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2315 2024-05-30 02:18:47.000000 alabamaencoder-0.5.0/alabamaEncode/encoder/impl/VideoToolbox.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7253 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/encoder/impl/X264.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4107 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/encoder/impl/X265.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2022-12-05 03:43:14.000000 alabamaencoder-0.5.0/alabamaEncode/encoder/impl/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2043 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/encoder/impl/rav1e.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3567 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/encoder/impl/vp9.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      269 2024-01-17 00:14:46.000000 alabamaencoder-0.5.0/alabamaEncode/encoder/rate_dist.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2494 2024-02-04 12:07:28.000000 alabamaencoder-0.5.0/alabamaEncode/encoder/stats.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.194224 alabamaencoder-0.5.0/alabamaEncode/experiments/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3713 2023-12-11 23:14:15.000000 alabamaencoder-0.5.0/alabamaEncode/experiments/Aq.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4337 2023-12-11 23:14:15.000000 alabamaencoder-0.5.0/alabamaEncode/experiments/Overlays.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2950 2024-02-02 15:19:02.000000 alabamaencoder-0.5.0/alabamaEncode/experiments/Svtav1Speed.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5719 2023-12-11 23:14:15.000000 alabamaencoder-0.5.0/alabamaEncode/experiments/Svtav1Tunes.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3749 2023-12-11 23:14:15.000000 alabamaencoder-0.5.0/alabamaEncode/experiments/TemporalFiltering.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-04-06 18:23:30.000000 alabamaencoder-0.5.0/alabamaEncode/experiments/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2501 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/experiments/ai_feature_extract.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      319 2023-12-10 22:37:13.000000 alabamaencoder-0.5.0/alabamaEncode/experiments/aom_extract.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5797 2024-05-30 02:25:08.000000 alabamaencoder-0.5.0/alabamaEncode/experiments/convexhull.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    16870 2024-05-30 02:25:07.000000 alabamaencoder-0.5.0/alabamaEncode/experiments/crf_vmaf_relation.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4926 2024-05-30 02:25:07.000000 alabamaencoder-0.5.0/alabamaEncode/experiments/denoise.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2195 2024-05-30 02:25:08.000000 alabamaencoder-0.5.0/alabamaEncode/experiments/sequence_convex.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      254 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/experiments/serialise_context.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      798 2024-05-30 02:18:47.000000 alabamaencoder-0.5.0/alabamaEncode/experiments/streaming_output.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6592 2023-12-11 23:14:15.000000 alabamaencoder-0.5.0/alabamaEncode/experiments/superres.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4106 2023-11-15 20:26:48.000000 alabamaencoder-0.5.0/alabamaEncode/experiments/target_vmaf.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.198224 alabamaencoder-0.5.0/alabamaEncode/experiments/util/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11478 2024-02-04 12:09:55.000000 alabamaencoder-0.5.0/alabamaEncode/experiments/util/ExperimentUtil.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-10-17 18:48:28.000000 alabamaencoder-0.5.0/alabamaEncode/experiments/util/__init__.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.198224 alabamaencoder-0.5.0/alabamaEncode/metrics/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-11-17 22:15:46.000000 alabamaencoder-0.5.0/alabamaEncode/metrics/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5252 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/metrics/calculate.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      911 2023-11-22 22:07:47.000000 alabamaencoder-0.5.0/alabamaEncode/metrics/comparison_display.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      384 2024-01-26 03:01:39.000000 alabamaencoder-0.5.0/alabamaEncode/metrics/exception.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3043 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/metrics/image.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.198224 alabamaencoder-0.5.0/alabamaEncode/metrics/impl/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-02-04 12:02:29.000000 alabamaencoder-0.5.0/alabamaEncode/metrics/impl/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      934 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/metrics/impl/psnr.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1442 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/metrics/impl/ssim.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3108 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/metrics/impl/ssimu2.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     9098 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/metrics/impl/vmaf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      117 2024-02-04 12:09:55.000000 alabamaencoder-0.5.0/alabamaEncode/metrics/metric.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      373 2024-02-04 12:36:30.000000 alabamaencoder-0.5.0/alabamaEncode/metrics/options.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      308 2024-02-02 14:53:33.000000 alabamaencoder-0.5.0/alabamaEncode/metrics/result.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.198224 alabamaencoder-0.5.0/alabamaEncode/parallel_execution/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-04-16 16:38:33.000000 alabamaencoder-0.5.0/alabamaEncode/parallel_execution/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      865 2024-05-30 02:29:55.000000 alabamaencoder-0.5.0/alabamaEncode/parallel_execution/celery_app.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3853 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/parallel_execution/celery_autoscaler.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      148 2023-11-05 09:04:10.000000 alabamaencoder-0.5.0/alabamaEncode/parallel_execution/command.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    12824 2024-05-30 02:29:55.000000 alabamaencoder-0.5.0/alabamaEncode/parallel_execution/execute_commands.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      415 2024-05-30 02:29:55.000000 alabamaencoder-0.5.0/alabamaEncode/parallel_execution/worker.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.202224 alabamaencoder-0.5.0/alabamaEncode/scene/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-04-15 20:18:27.000000 alabamaencoder-0.5.0/alabamaEncode/scene/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1810 2024-03-29 15:35:11.000000 alabamaencoder-0.5.0/alabamaEncode/scene/annel.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     9700 2024-05-30 02:18:05.000000 alabamaencoder-0.5.0/alabamaEncode/scene/chunk.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    13591 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/scene/concat.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11209 2024-05-30 02:25:07.000000 alabamaencoder-0.5.0/alabamaEncode/scene/scene_detection.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4456 2024-05-30 02:18:05.000000 alabamaencoder-0.5.0/alabamaEncode/scene/sequence.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.202224 alabamaencoder-0.5.0/alabamaEncoder.egg-info/
+-rw-r--r--   0 kokoniara  (1000) kokoniara  (1000)      377 2024-05-30 16:09:21.000000 alabamaencoder-0.5.0/alabamaEncoder.egg-info/PKG-INFO
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5807 2024-05-30 16:09:21.000000 alabamaencoder-0.5.0/alabamaEncoder.egg-info/SOURCES.txt
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        1 2024-05-30 16:09:21.000000 alabamaencoder-0.5.0/alabamaEncoder.egg-info/dependency_links.txt
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)       67 2024-05-30 16:09:21.000000 alabamaencoder-0.5.0/alabamaEncoder.egg-info/entry_points.txt
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      124 2024-05-30 16:09:21.000000 alabamaencoder-0.5.0/alabamaEncoder.egg-info/requires.txt
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)       14 2024-05-30 16:09:21.000000 alabamaencoder-0.5.0/alabamaEncoder.egg-info/top_level.txt
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)       38 2024-05-30 16:09:21.202224 alabamaencoder-0.5.0/setup.cfg
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      538 2024-05-30 16:08:35.000000 alabamaencoder-0.5.0/setup.py
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/ai_vmaf/aom_firstpass.py` & `alabamaencoder-0.5.0/alabamaEncode/ai_vmaf/aom_firstpass.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import random
 import struct
 
-from alabamaEncode.core.bin_utils import get_binary
-from alabamaEncode.core.cli_executor import run_cli
+from alabamaEncode.core.util.bin_utils import get_binary
+from alabamaEncode.core.util.cli_executor import run_cli
 from alabamaEncode.scene.chunk import ChunkObject
 
 # big shoutout to @master_of_zen for this
 
 fields = [
     "frame",
     "weight",
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/ai_vmaf/perdict.py` & `alabamaencoder-0.5.0/alabamaEncode/ai_vmaf/perdict.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.3/alabamaEncode/ai_vmaf/train/train.py` & `alabamaencoder-0.5.0/alabamaEncode/ai_vmaf/train/train.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/analyze_steps/capped_crf.py` & `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_crf.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from alabamaEncode.conent_analysis.chunk.chunk_analyse_step import (
     ChunkAnalyzePipelineItem,
 )
-from alabamaEncode.core.alabama import AlabamaContext
+from alabamaEncode.core.context import AlabamaContext
 from alabamaEncode.encoder.encoder import Encoder
 from alabamaEncode.encoder.rate_dist import EncoderRateDistribution
 from alabamaEncode.scene.chunk import ChunkObject
 
 
-class CapedCrf(ChunkAnalyzePipelineItem):
+class PlainCrf(ChunkAnalyzePipelineItem):
     def run(self, ctx: AlabamaContext, chunk: ChunkObject, enc: Encoder) -> Encoder:
-        enc.rate_distribution = EncoderRateDistribution.CQ_VBV
-        enc.bitrate = ctx.max_bitrate
+        enc.rate_distribution = EncoderRateDistribution.CQ
         enc.crf = ctx.prototype_encoder.crf
         enc.passes = 1
-        enc.svt_open_gop = True
         return enc
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/analyze_steps/multires_encode_candidates.py` & `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/analyze_steps/multires_encode_candidates.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/analyze_steps/optimised_vbr.py` & `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/analyze_steps/optimised_vbr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import pickle
 import time
 
 from alabamaEncode.conent_analysis.chunk.chunk_analyse_step import (
     ChunkAnalyzePipelineItem,
 )
-from alabamaEncode.core.alabama import AlabamaContext
+from alabamaEncode.core.context import AlabamaContext
 from alabamaEncode.encoder.encoder import Encoder
 from alabamaEncode.encoder.rate_dist import EncoderRateDistribution
 from alabamaEncode.metrics.impl.ssim import get_video_ssim
 from alabamaEncode.scene.chunk import ChunkObject
 
 
 class VbrPerChunkOptimised(ChunkAnalyzePipelineItem):
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/analyze_steps/per_scene_grain.py` & `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/analyze_steps/per_scene_grain.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 import os
 from math import sqrt
 from statistics import mean
 
 from alabamaEncode.conent_analysis.chunk.chunk_analyse_step import (
     ChunkAnalyzePipelineItem,
 )
-from alabamaEncode.core.alabama import AlabamaContext
-from alabamaEncode.core.bin_utils import get_binary
-from alabamaEncode.core.cli_executor import run_cli
-from alabamaEncode.core.timer import Timer
+from alabamaEncode.core.context import AlabamaContext
+from alabamaEncode.core.util.bin_utils import get_binary
+from alabamaEncode.core.util.cli_executor import run_cli
+from alabamaEncode.core.util.timer import Timer
 from alabamaEncode.encoder.encoder import Encoder
 from alabamaEncode.scene.chunk import ChunkObject
-from alabamaEncode.scene.split import get_video_scene_list_skinny
+from alabamaEncode.scene.scene_detection import scene_detect
 
 
 class GrainSynth(ChunkAnalyzePipelineItem):
     def run(self, ctx: AlabamaContext, chunk: ChunkObject, enc: Encoder) -> Encoder:
         probe_file_base = ctx.get_probe_file_base(chunk.chunk_path)
 
         grain_synth_result = ctx.get_kv().get("grain_synth", chunk.chunk_path)
@@ -259,15 +259,15 @@
 def test():
     test_env = "./experiments/grain_synth/"
     test_env = os.path.abspath(test_env)
 
     if not os.path.exists(test_env):
         os.makedirs(test_env)
 
-    scene_list = get_video_scene_list_skinny(
+    scene_list = scene_detect(
         input_file="/home/kokoniara/ep3_halo_test.mkv",
         cache_file_path=test_env + "sceneCache.pt",
     )
 
     for chunk in scene_list.chunks:
         print(
             "calculated gs: "
@@ -288,15 +288,15 @@
 def test_altblur():
     test_env = "./experiments/grain_synth/"
     test_env = os.path.abspath(test_env)
 
     if not os.path.exists(test_env):
         os.makedirs(test_env)
 
-    scene_list = get_video_scene_list_skinny(
+    scene_list = scene_detect(
         input_file="/home/kokoniara/ep3_halo_test.mkv",
         cache_file_path=test_env + "sceneCache.pt",
     )
 
     for chunk in scene_list.chunks:
         print(
             "calculated gs altblur: "
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_crf.py` & `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/final_encode_step.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,26 @@
-from alabamaEncode.conent_analysis.chunk.chunk_analyse_step import (
-    ChunkAnalyzePipelineItem,
-)
-from alabamaEncode.core.alabama import AlabamaContext
+from abc import ABC, abstractmethod
+
+from alabamaEncode.core.context import AlabamaContext
 from alabamaEncode.encoder.encoder import Encoder
-from alabamaEncode.encoder.rate_dist import EncoderRateDistribution
+from alabamaEncode.encoder.stats import EncodeStats
 from alabamaEncode.scene.chunk import ChunkObject
 
 
-class PlainCrf(ChunkAnalyzePipelineItem):
-    def run(self, ctx: AlabamaContext, chunk: ChunkObject, enc: Encoder) -> Encoder:
-        enc.rate_distribution = EncoderRateDistribution.CQ
-        enc.crf = ctx.prototype_encoder.crf
-        enc.passes = 1
-        return enc
+class FinalEncodeStep(ABC):
+    """
+    Preforms the final (usually longer) encoding
+    """
+
+    @abstractmethod
+    def run(
+        self,
+        enc: Encoder,
+        chunk: ChunkObject,
+        ctx: AlabamaContext,
+        encoded_a_frame,
+    ) -> EncodeStats:
+        pass
+
+    @abstractmethod
+    def dry_run(self, enc: Encoder, chunk: ChunkObject) -> str:
+        pass
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_vbr.py` & `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_vbr.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from alabamaEncode.conent_analysis.chunk.chunk_analyse_step import (
     ChunkAnalyzePipelineItem,
 )
-from alabamaEncode.core.alabama import AlabamaContext
+from alabamaEncode.core.context import AlabamaContext
 from alabamaEncode.encoder.encoder import Encoder
 from alabamaEncode.encoder.rate_dist import EncoderRateDistribution
 from alabamaEncode.scene.chunk import ChunkObject
 
 
 class PlainVbr(ChunkAnalyzePipelineItem):
     def run(self, ctx: AlabamaContext, chunk: ChunkObject, enc: Encoder) -> Encoder:
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/analyze_steps/target_vmaf.py` & `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/analyze_steps/target_vmaf.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     ChunkAnalyzePipelineItem,
 )
 from alabamaEncode.conent_analysis.opinionated_vmaf import (
     get_crf_limits,
     get_vmaf_probe_speed,
     get_vmaf_probe_offset,
 )
-from alabamaEncode.core.alabama import AlabamaContext
+from alabamaEncode.core.context import AlabamaContext
 from alabamaEncode.encoder.encoder import Encoder
 from alabamaEncode.encoder.stats import EncodeStats
 from alabamaEncode.metrics.calculate import get_metric_from_stats
 from alabamaEncode.metrics.metric import Metric
 from alabamaEncode.scene.chunk import ChunkObject
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf.py` & `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import shutil
 from typing import Tuple
 
 from alabamaEncode.conent_analysis.chunk.final_encode_step import (
     FinalEncodeStep,
 )
 from alabamaEncode.conent_analysis.opinionated_vmaf import get_crf_limits
-from alabamaEncode.core.alabama import AlabamaContext
+from alabamaEncode.core.context import AlabamaContext
 from alabamaEncode.encoder.codec import Codec
 from alabamaEncode.encoder.encoder import Encoder
 from alabamaEncode.encoder.rate_dist import EncoderRateDistribution
 from alabamaEncode.encoder.stats import EncodeStats
 from alabamaEncode.metrics.calculate import get_metric_from_stats
 from alabamaEncode.metrics.metric import Metric
 from alabamaEncode.scene.chunk import ChunkObject
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf_vbr.py` & `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf_vbr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 from alabamaEncode.conent_analysis.chunk.final_encode_step import (
     FinalEncodeStep,
 )
-from alabamaEncode.core.alabama import AlabamaContext
+from alabamaEncode.core.context import AlabamaContext
 from alabamaEncode.encoder.encoder import Encoder
 from alabamaEncode.encoder.rate_dist import EncoderRateDistribution
 from alabamaEncode.encoder.stats import EncodeStats
 from alabamaEncode.metrics.calculate import get_metric_from_stats
 from alabamaEncode.metrics.metric import Metric
 from alabamaEncode.scene.chunk import ChunkObject
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/multires_encode_finals.py` & `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/final_encode_steps/multires_encode_finals.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 from alabamaEncode.conent_analysis.chunk.final_encode_step import FinalEncodeStep
 from alabamaEncode.conent_analysis.opinionated_vmaf import get_vmaf_list
-from alabamaEncode.core.alabama import AlabamaContext
+from alabamaEncode.core.context import AlabamaContext
 from alabamaEncode.encoder.encoder import Encoder
 from alabamaEncode.encoder.stats import EncodeStats
 from alabamaEncode.scene.chunk import ChunkObject
 
 
 class EncodeMultiResFinals(FinalEncodeStep):
     def run(
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/plain.py` & `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/final_encode_steps/plain.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from alabamaEncode.conent_analysis.chunk.final_encode_step import (
     FinalEncodeStep,
 )
-from alabamaEncode.core.alabama import AlabamaContext
+from alabamaEncode.core.context import AlabamaContext
 from alabamaEncode.encoder.encoder import Encoder
 from alabamaEncode.encoder.stats import EncodeStats
 from alabamaEncode.scene.chunk import ChunkObject
 
 
 class PlainFinalEncode(FinalEncodeStep):
     def run(
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/opinionated_vmaf.py` & `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/opinionated_vmaf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 
 from alabamaEncode.encoder.codec import Codec
 from alabamaEncode.encoder.encoder import Encoder
 from alabamaEncode.encoder.impl.Aomenc import EncoderAom
 from alabamaEncode.encoder.impl.Svtenc import EncoderSvt
+from alabamaEncode.encoder.impl.VideoToolbox import EncoderAppleHEVC
 
 
 def convexhull_get_crf_range(codec: Codec) -> tuple[int, int]:
     match codec:
         case Codec.av1:
             return 18, 58
         # TODO: pick other values
@@ -69,14 +70,15 @@
 
 if __name__ == "__main__":
     my_enc = EncoderSvt()
     my_aom_enc = EncoderAom()
 
     assert get_crf_limits(my_enc), [22, 38]
     assert get_crf_limits(my_aom_enc), [18, 40]
+    assert get_crf_limits(EncoderAppleHEVC()), [10, 90]
 
 
 def get_vmaf_list(codec: Codec) -> list[int]:
     match codec:
         case Codec.av1:
             return [73, 78, 84, 91, 95]
         case Codec.h264:
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/pipelines.py` & `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/pipelines.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from alabamaEncode.conent_analysis.refine_steps.multires_trellis import MutliResTrellis
 
 
 def setup_chunk_analyze_chain(ctx, sequence):
     """
     Sets up the chunk analyze chain
     """
-    from alabamaEncode.conent_analysis.chunk.analyze_steps.capped_crf import CapedCrf
     from alabamaEncode.conent_analysis.chunk.analyze_steps.manual_crf import (
         CrfIndexesMap,
     )
     from alabamaEncode.conent_analysis.chunk.analyze_steps.optimised_vbr import (
         VbrPerChunkOptimised,
     )
     from alabamaEncode.conent_analysis.chunk.analyze_steps.per_scene_grain import (
@@ -47,24 +46,19 @@
     elif ctx.dynamic_vmaf_target_vbr:
         print("Using dynamic vmaf targeting with vbr")
         ctx.chunk_analyze_chain.append(PlainVbr())
     elif ctx.multi_res_pipeline:
         ctx.chunk_analyze_chain.append(EncodeMultiResCandidates())
     elif ctx.crf_map != "":
         ctx.chunk_analyze_chain.append(CrfIndexesMap(ctx.crf_map))
-    elif ctx.flag1 is True:
-        ctx.chunk_analyze_chain.append(PlainCrf())
     elif (
         ctx.crf_based_vmaf_targeting is True
-        and ctx.ai_vmaf_targeting is False
         and ctx.multi_res_pipeline is False
     ):
         ctx.chunk_analyze_chain.append(TargetVmaf())
-    elif ctx.crf_bitrate_mode or ctx.ai_vmaf_targeting:
-        ctx.chunk_analyze_chain.append(CapedCrf())
     elif ctx.prototype_encoder.crf != -1:
         ctx.chunk_analyze_chain.append(PlainCrf())
     else:
         ctx.chunk_analyze_chain.append(PlainVbr())
 
     if len(ctx.chunk_analyze_chain) == 0:
         raise Exception("Failed to Create the analyze steps in analyzer_factory")
@@ -74,33 +68,23 @@
 
 def setup_chunk_encoder(ctx, sequence):
     """
     Sets up the chunk encoder
     """
 
     # ugly imports here cuz "Circular import 🤓☝"
-    from alabamaEncode.conent_analysis.chunk.final_encode_steps.ai_targeted_vmaf import (
-        AiTargetedVmafFinalEncode,
-    )
-    from alabamaEncode.conent_analysis.chunk.final_encode_steps.capped_crf_encode import (
-        WeridCapedCrfFinalEncode,
-    )
     from alabamaEncode.conent_analysis.chunk.final_encode_steps.plain import (
         PlainFinalEncode,
     )
 
     from alabamaEncode.conent_analysis.chunk.final_encode_steps.dynamic_target_vmaf_vbr import (
         DynamicTargetVmafVBR,
     )
 
-    if ctx.flag1:
-        ctx.chunk_encode_class = WeridCapedCrfFinalEncode()
-    elif ctx.ai_vmaf_targeting:
-        ctx.chunk_encode_class = AiTargetedVmafFinalEncode()
-    elif ctx.dynamic_vmaf_target:
+    if ctx.dynamic_vmaf_target:
         ctx.chunk_encode_class = DynamicTargetVmaf()
     elif ctx.dynamic_vmaf_target_vbr:
         ctx.chunk_encode_class = DynamicTargetVmafVBR()
     elif ctx.multi_res_pipeline:
         print("Starting the multi res pipeline")
         ctx.chunk_encode_class = EncodeMultiResFinals()
     else:
@@ -121,40 +105,32 @@
 async def run_sequence_pipeline(ctx, sequence):
     from alabamaEncode.conent_analysis.sequence.autocrop import do_autocrop
     from alabamaEncode.conent_analysis.sequence.args_tune import (
         tune_args_for_fdlty_or_apl,
     )
     from alabamaEncode.conent_analysis.sequence.denoise_filtering import setup_denoise
     from alabamaEncode.conent_analysis.sequence.encoding_tiles import setup_tiles
-    from alabamaEncode.conent_analysis.sequence.ideal_crf import (
-        setup_ideal_crf_weighted,
-    )
     from alabamaEncode.conent_analysis.sequence.scrape_hdr_meta import (
         scrape_hdr_metadata,
     )
     from alabamaEncode.conent_analysis.sequence.sequence_autograin import (
         setup_autograin,
     )
     from alabamaEncode.conent_analysis.sequence.taget_ssimdb import setup_ssimdb_target
-    from alabamaEncode.conent_analysis.sequence.target_bitrate_optimisation import (
-        setup_ideal_bitrate,
-    )
     from alabamaEncode.conent_analysis.sequence.x264_tune import get_ideal_x264_tune
 
     pipeline = [
         setup_chunk_analyze_chain,
         setup_chunk_encoder,
         scrape_hdr_metadata,
         tune_args_for_fdlty_or_apl,
         do_autocrop,
         setup_tiles,
         setup_denoise,
         setup_autograin,
-        setup_ideal_crf_weighted,
-        setup_ideal_bitrate,
         setup_ssimdb_target,
         get_ideal_x264_tune,
     ]
 
     for func in pipeline:
         # if async run awaits, if not run normally
         ctx = (
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/refine_steps/multires_package.py` & `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/refine_steps/multires_package.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 
 from alabamaEncode.conent_analysis.opinionated_vmaf import get_vmaf_list
 from alabamaEncode.conent_analysis.refine_step import RefineStep
-from alabamaEncode.core.bin_utils import get_binary
+from alabamaEncode.core.util.bin_utils import get_binary
 from alabamaEncode.core.ffmpeg import Ffmpeg
-from alabamaEncode.core.path import PathAlabama
+from alabamaEncode.core.util.path import PathAlabama
 from alabamaEncode.scene.concat import VideoConcatenator
 
 
 class MutliResPackage(RefineStep):
     def __call__(self, ctx, sequence):
         final_paths = ctx.get_kv().get("multires_final_paths", "final_paths")
         if final_paths is None:
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/refine_steps/multires_trellis.py` & `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/refine_steps/multires_trellis.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/args_tune.py` & `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/sequence/args_tune.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from alabamaEncode.core.alabama import AlabamaContext
+from alabamaEncode.core.context import AlabamaContext
 from alabamaEncode.encoder.impl.Svtenc import EncoderSvt
 from alabamaEncode.scene.sequence import ChunkSequence
 
 
 def tune_args_for_fdlty_or_apl(ctx: AlabamaContext, sequence: ChunkSequence):
     match ctx.args_tune:
         case "fidelity":
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/autocrop.py` & `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/sequence/autocrop.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 import re
 import time
 from typing import List
 
-from alabamaEncode.core.alabama import AlabamaContext
-from alabamaEncode.core.bin_utils import get_binary
-from alabamaEncode.core.cli_executor import run_cli
+from alabamaEncode.core.context import AlabamaContext
 from alabamaEncode.core.ffmpeg import Ffmpeg
-from alabamaEncode.core.path import PathAlabama
+from alabamaEncode.core.util.bin_utils import get_binary
+from alabamaEncode.core.util.cli_executor import run_cli
+from alabamaEncode.core.util.path import PathAlabama
 from alabamaEncode.scene.chunk import ChunkObject
 from alabamaEncode.scene.sequence import ChunkSequence
 
 
 def do_autocrop(ctx: AlabamaContext, sequence: ChunkSequence):
     """
     Does autocrop if needed
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/encoding_tiles.py` & `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/sequence/encoding_tiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from alabamaEncode.core.alabama import AlabamaContext
+from alabamaEncode.core.context import AlabamaContext
 from alabamaEncode.encoder.codec import Codec
 from alabamaEncode.scene.sequence import ChunkSequence
 
 
 def setup_tiles(ctx: AlabamaContext, sequence: ChunkSequence):
     """
     Sets up the tiles based on the resolution
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/scrape_hdr_meta.py` & `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/sequence/scrape_hdr_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import os
 
-from alabamaEncode.core.alabama import AlabamaContext
+from alabamaEncode.core.context import AlabamaContext
 from alabamaEncode.core.ffmpeg import Ffmpeg
-from alabamaEncode.core.path import PathAlabama
+from alabamaEncode.core.util.path import PathAlabama
 from alabamaEncode.encoder.impl.Svtenc import EncoderSvt
 from alabamaEncode.encoder.impl.X264 import EncoderX264
 from alabamaEncode.scene.sequence import ChunkSequence
 
 
 def scrape_hdr_metadata(ctx: AlabamaContext, sequence: ChunkSequence):
     """
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/sequence_autograin.py` & `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/sequence/sequence_autograin.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import os
 import random
 import time
 from multiprocessing.pool import ThreadPool
 from statistics import mean
 from typing import List
 
-from alabamaEncode.core.alabama import AlabamaContext
-from alabamaEncode.core.bin_utils import get_binary
-from alabamaEncode.core.cli_executor import run_cli
-from alabamaEncode.core.kv import AlabamaKv
+from alabamaEncode.core.context import AlabamaContext
+from alabamaEncode.core.util.bin_utils import get_binary
+from alabamaEncode.core.util.cli_executor import run_cli
+from alabamaEncode.core.util.kv import AlabamaKv
 from alabamaEncode.encoder.impl.SvtAvif import AvifEncoderSvtenc
 from alabamaEncode.metrics.image import ImageMetrics
 from alabamaEncode.scene.sequence import ChunkSequence
 
 
 def setup_autograin(ctx: AlabamaContext, sequence: ChunkSequence):
     if (
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/taget_ssimdb.py` & `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/sequence/taget_ssimdb.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import pickle
 from concurrent.futures import ThreadPoolExecutor
 from typing import List
 
-from alabamaEncode.core.alabama import AlabamaContext
+from alabamaEncode.core.context import AlabamaContext
 from alabamaEncode.encoder.rate_dist import EncoderRateDistribution
 from alabamaEncode.encoder.stats import EncodeStats
 from alabamaEncode.scene.chunk import ChunkObject
 from alabamaEncode.scene.sequence import ChunkSequence
 
 
 def calulcate_ssimdb(bitrate: int, chunk: ChunkObject, dbs: List[float], ctx):
@@ -69,15 +69,14 @@
     pickle.dump(target_ssimdb, open(cache_path, "wb"))
     return target_ssimdb
 
 
 def setup_ssimdb_target(ctx: AlabamaContext, sequence: ChunkSequence):
     if all(
         [
-            not ctx.flag1,
             ctx.crf_based_vmaf_targeting is False,
             ctx.vbr_perchunk_optimisation,
         ]
     ):
         if ctx.prototype_encoder.bitrate is None:
             print("No bitrate set, cannot set SSIMDB target, set --bitrate")
             quit()
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/x264_tune.py` & `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/sequence/x264_tune.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import shutil
 from multiprocessing import Pool
 
-from alabamaEncode.core.alabama import AlabamaContext
+from alabamaEncode.core.context import AlabamaContext
 from alabamaEncode.encoder.impl.X264 import EncoderX264
 from alabamaEncode.metrics.metric import Metric
 from alabamaEncode.scene.sequence import ChunkSequence
 
 
 def run_tune(a):
     tune, enc, path, vmaf_options = a
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/core/alabama.py` & `alabamaencoder-0.5.0/alabamaEncode/core/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 from tqdm import tqdm
 
 from alabamaEncode.conent_analysis.chunk.chunk_analyse_step import (
     ChunkAnalyzePipelineItem,
 )
 from alabamaEncode.core.ffmpeg import Ffmpeg
-from alabamaEncode.core.kv import AlabamaKv
-from alabamaEncode.core.path import PathAlabama
+from alabamaEncode.core.util.kv import AlabamaKv
+from alabamaEncode.core.util.path import PathAlabama
 from alabamaEncode.encoder.encoder import Encoder
 from alabamaEncode.encoder.impl.Svtenc import EncoderSvt
 from alabamaEncode.encoder.rate_dist import EncoderRateDistribution
 from alabamaEncode.metrics.comparison_display import ComparisonDisplayResolution
 from alabamaEncode.metrics.impl.vmaf import VmafOptions
 from alabamaEncode.metrics.metric import Metric
 from alabamaEncode.scene.chunk import ChunkObject
@@ -48,34 +48,29 @@
             "crop_string": self.crop_string,
             "scale_string": self.scale_string,
             "output_height": self.output_height,
             "output_width": self.output_width,
             "find_best_bitrate": self.find_best_bitrate,
             "vbr_perchunk_optimisation": self.vbr_perchunk_optimisation,
             "ssim_db_target": self.ssim_db_target,
-            "crf_bitrate_mode": self.crf_bitrate_mode,
             "bitrate_undershoot": self.bitrate_undershoot,
             "bitrate_overshoot": self.bitrate_overshoot,
             "bitrate_adjust_mode": self.bitrate_adjust_mode,
             "cutoff_bitrate": self.cutoff_bitrate,
             "max_bitrate": self.max_bitrate,
             "simple_denoise": self.simple_denoise,
             "vmaf": self.vmaf,
             "probe_count": self.probe_count,
             "vmaf_reference_display": self.vmaf_reference_display,
             "crf_based_vmaf_targeting": self.crf_based_vmaf_targeting,
             "vmaf_4k_model": self.vmaf_4k_model,
             "vmaf_phone_model": self.vmaf_phone_model,
             "vmaf_no_motion": self.vmaf_no_motion,
             "probe_speed_override": self.probe_speed_override,
-            "ai_vmaf_targeting": self.ai_vmaf_targeting,
             "vmaf_target_representation": self.vmaf_target_representation,
-            "flag1": self.flag1,
-            "flag2": self.flag2,
-            "flag3": self.flag3,
             "crf_map": self.crf_map,
             "max_scene_length": self.max_scene_length,
             "start_offset": self.start_offset,
             "end_offset": self.end_offset,
             "override_scenecache_path_check": self.override_scenecache_path_check,
             "title": self.title,
             "sub_file": self.sub_file,
@@ -138,43 +133,38 @@
     chunk_encode_class = None
 
     prototype_encoder: Encoder = EncoderSvt()
 
     find_best_bitrate = False
     vbr_perchunk_optimisation: bool = True
     ssim_db_target: float = 20
-    crf_bitrate_mode: bool = False
     bitrate_undershoot: float = 0.90
     bitrate_overshoot: float = 2
     bitrate_adjust_mode: str = ""
     cutoff_bitrate: int = -1
     max_bitrate: int = 0
     simple_denoise = False
-    args_tune = "balanced"
+    args_tune = "appeal"
     calc_final_vmaf = False
 
     metric_to_target = "vmaf"
     vmaf: int = 96
     denoise_vmaf_ref = False
-    probe_count = 3
+    probe_count = 2
     vmaf_reference_display = ""
     crf_based_vmaf_targeting = True
     vmaf_4k_model = False
     vmaf_phone_model = False
     vmaf_no_motion = False
     probe_speed_override = prototype_encoder.speed
-    ai_vmaf_targeting = False
     vmaf_target_representation = "mean"
     dynamic_vmaf_target = False
     dynamic_vmaf_target_vbr = False
     best_crfs = []
 
-    flag1: bool = False
-    flag2: bool = False
-    flag3: bool = False
     crf_map = ""
 
     total_chunks = -1
     max_scene_length: int = 10
     statically_sized_scenes = False
     scene_merge = False
     start_offset: int = -1
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/core/bin_utils.py` & `alabamaencoder-0.5.0/alabamaEncode/core/util/bin_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 from shutil import which
 
 __all__ = ["get_binary", "register_bin", "verify_ffmpeg_library", "check_bin"]
 
 from typing import List
 
-from alabamaEncode.core.cli_executor import run_cli
+from alabamaEncode.core.util.cli_executor import run_cli
 
 bins = []
 
 
 def check_bin(path) -> bool:
     if path is None:
         return False
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/core/chunk_job.py` & `alabamaencoder-0.5.0/alabamaEncode/core/chunk_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import time
 
 from tqdm import tqdm
 
 from alabamaEncode.conent_analysis.chunk.final_encode_steps.dynamic_target_vmaf import (
     DynamicTargetVmaf,
 )
-from alabamaEncode.core.alabama import AlabamaContext
-from alabamaEncode.core.timer import Timer
+from alabamaEncode.core.context import AlabamaContext
+from alabamaEncode.core.util.timer import Timer
 from alabamaEncode.encoder.impl.Svtenc import EncoderSvt
 from alabamaEncode.encoder.stats import EncodeStats
-from alabamaEncode.parallelEncoding.command import BaseCommandObject
+from alabamaEncode.parallel_execution.command import BaseCommandObject
 from alabamaEncode.scene.chunk import ChunkObject
 
 
 class ChunkEncoder(BaseCommandObject):
     """
     Class that gets the ideal bitrate and encodes the final chunk
     """
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/core/cli_executor.py` & `alabamaencoder-0.5.0/alabamaEncode/core/util/cli_executor.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.3/alabamaEncode/core/extras/auto_thumbnailer.py` & `alabamaencoder-0.5.0/alabamaEncode/core/extras/auto_thumbnailer.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import cv2
 import numpy as np
 import scipy
 from skimage.metrics import structural_similarity as ssim
 from tqdm import tqdm
 
-from alabamaEncode.core.bin_utils import get_binary, check_ffmpeg_libraries, check_bin
-from alabamaEncode.core.cli_executor import run_cli
 from alabamaEncode.core.ffmpeg import Ffmpeg
-from alabamaEncode.core.path import PathAlabama
-from alabamaEncode.ffmpeg_source.ffmpeg_src import get_yuv_frame_stream
+from alabamaEncode.core.util.bin_utils import get_binary, check_ffmpeg_libraries, check_bin
+from alabamaEncode.core.util.cli_executor import run_cli
+from alabamaEncode.core.util.get_yuv_stream import get_yuv_frame_stream
+from alabamaEncode.core.util.path import PathAlabama
 from alabamaEncode.scene.chunk import ChunkObject
 
 
 def calculate_saliency_score(image):
     # Compute the saliency map
     (success, saliencyMap) = (
         cv2.saliency.StaticSaliencySpectralResidual_create().computeSaliency(image)
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/core/ffmpeg.py` & `alabamaencoder-0.5.0/alabamaEncode/core/ffmpeg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import os
 import re
 from typing import Any
 
-from alabamaEncode.core.bin_utils import get_binary, verify_ffmpeg_library
-from alabamaEncode.core.cli_executor import run_cli
-from alabamaEncode.core.path import PathAlabama
+from alabamaEncode.core.util.bin_utils import get_binary, verify_ffmpeg_library
+from alabamaEncode.core.util.cli_executor import run_cli
+from alabamaEncode.core.util.path import PathAlabama
 
 
 class Ffmpeg:
     @staticmethod
     def check_for_invalid(path: PathAlabama) -> bool:
         """
         Checks if the file is not a valid video file
@@ -384,7 +384,9 @@
             case "subtitle":
                 print("subtitle track")
         print(track)
 
 
 if __name__ == "__main__":
     track_test()
+
+
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/core/final_touches.py` & `alabamaencoder-0.5.0/alabamaEncode/core/final_touches.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 import random
 
 from torf import Torrent
 from tqdm import tqdm
 
-from alabamaEncode.core.bin_utils import get_binary, register_bin, BinaryNotFound
-from alabamaEncode.core.cli_executor import run_cli
+from alabamaEncode.core.util.bin_utils import get_binary, register_bin, BinaryNotFound
+from alabamaEncode.core.util.cli_executor import run_cli
 from alabamaEncode.core.ffmpeg import Ffmpeg
-from alabamaEncode.core.path import PathAlabama
+from alabamaEncode.core.util.path import PathAlabama
 
 
 def print_stats(
     output_folder: str,
     output: str,
     input_file: str,
     grain_synth: int,
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/core/job.py` & `alabamaencoder-0.5.0/alabamaEncode/core/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,41 +7,41 @@
 import sys
 import time
 
 import psutil
 import requests
 from tqdm import tqdm
 
+from alabamaEncode.cli.cli_setup.paths import parse_paths
+from alabamaEncode.cli.cli_setup.ratecontrol import parse_rd
+from alabamaEncode.cli.cli_setup.res_preset import parse_resolution_presets
+from alabamaEncode.cli.cli_setup.video_filters import parse_video_filters
 from alabamaEncode.conent_analysis.opinionated_vmaf import (
     get_vmaf_list,
 )
 from alabamaEncode.conent_analysis.pipelines import (
     run_sequence_pipeline,
     get_refine_steps,
 )
-from alabamaEncode.core.alabama import AlabamaContext
 from alabamaEncode.core.chunk_job import ChunkEncoder
+from alabamaEncode.core.context import AlabamaContext
+from alabamaEncode.core.extras.ws_update import WebsocketServer
 from alabamaEncode.core.ffmpeg import Ffmpeg
 from alabamaEncode.core.final_touches import (
     print_stats,
     generate_previews,
     create_torrent_file,
 )
-from alabamaEncode.core.path import PathAlabama
-from alabamaEncode.core.ws_update import WebsocketServer
-from alabamaEncode.parallelEncoding.CeleryApp import app
-from alabamaEncode.parallelEncoding.execute_commands import execute_commands
+from alabamaEncode.core.util.path import PathAlabama
+from alabamaEncode.parallel_execution.celery_app import app
+from alabamaEncode.parallel_execution.execute_commands import execute_commands
 from alabamaEncode.scene.annel import annealing
 from alabamaEncode.scene.concat import VideoConcatenator
+from alabamaEncode.scene.scene_detection import scene_detect
 from alabamaEncode.scene.sequence import ChunkSequence
-from alabamaEncode.scene.split import get_video_scene_list_skinny
-from alabamaEncode_frontends.cli.cli_setup.paths import parse_paths
-from alabamaEncode_frontends.cli.cli_setup.ratecontrol import parse_rd
-from alabamaEncode_frontends.cli.cli_setup.res_preset import parse_resolution_presets
-from alabamaEncode_frontends.cli.cli_setup.video_filters import parse_video_filters
 
 
 class AlabamaEncodingJob:
     def __init__(self, ctx):
         self.ctx = ctx
         self.current_step_callback = None
         self.proc_done_callback = None
@@ -256,15 +256,15 @@
                 # TODO: do a paranoid check for all files
             else:
                 return os.path.exists(self.ctx.output_file)
 
         if not encode_finished():
             constant_updates = asyncio.create_task(self.constant_updates())
             self.update_current_step_name("Running scene detection")
-            sequence: ChunkSequence = get_video_scene_list_skinny(
+            sequence: ChunkSequence = scene_detect(
                 input_file=self.ctx.input_file,
                 cache_file_path=self.ctx.temp_folder + "scene_cache.json",
                 max_scene_length=self.ctx.max_scene_length,
                 start_offset=self.ctx.start_offset,
                 end_offset=self.ctx.end_offset,
                 override_bad_wrong_cache_path=self.ctx.override_scenecache_path_check,
                 static_length=self.ctx.statically_sized_scenes,
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/core/kv.py` & `alabamaencoder-0.5.0/alabamaEncode/core/util/kv.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.3/alabamaEncode/core/path.py` & `alabamaencoder-0.5.0/alabamaEncode/core/util/path.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.3/alabamaEncode/core/timer.py` & `alabamaencoder-0.5.0/alabamaEncode/core/util/timer.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.3/alabamaEncode/core/ws_update.py` & `alabamaencoder-0.5.0/alabamaEncode/core/extras/ws_update.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.3/alabamaEncode/encoder/codec.py` & `alabamaencoder-0.5.0/alabamaEncode/encoder/codec.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.3/alabamaEncode/encoder/encoder.py` & `alabamaencoder-0.5.0/alabamaEncode/encoder/encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import os
 import time
 from abc import abstractmethod, ABC
 from typing import List
 
 from tqdm import tqdm
 
-from alabamaEncode.core.cli_executor import run_cli
+from alabamaEncode.core.util.cli_executor import run_cli
 from alabamaEncode.core.ffmpeg import Ffmpeg
-from alabamaEncode.core.path import PathAlabama
+from alabamaEncode.core.util.path import PathAlabama
 from alabamaEncode.encoder.codec import Codec
 from alabamaEncode.encoder.rate_dist import EncoderRateDistribution
 from alabamaEncode.encoder.stats import EncodeStats
 from alabamaEncode.metrics.calculate import calculate_metric
 from alabamaEncode.metrics.exception import MetricException
 from alabamaEncode.metrics.impl.ssim import get_video_ssim
 from alabamaEncode.metrics.metric import Metric
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/encoder/encoder_factory.py` & `alabamaencoder-0.5.0/alabamaEncode/encoder/encoder_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from alabamaEncode.encoder.encoder import Encoder
 from alabamaEncode.encoder.impl.Aomenc import EncoderAom
 from alabamaEncode.encoder.impl.Nvenc import EncoderNVENCH264
 from alabamaEncode.encoder.impl.Svtenc import EncoderSvt
 from alabamaEncode.encoder.impl.VaapiH264 import EncoderVaapiH264
 from alabamaEncode.encoder.impl.VaapiH265 import EncoderVaapiH265
+from alabamaEncode.encoder.impl.VideoToolbox import EncoderAppleHEVC
 from alabamaEncode.encoder.impl.X264 import EncoderX264
 from alabamaEncode.encoder.impl.X265 import EncoderX265
 from alabamaEncode.encoder.impl.rav1e import EncoderRav1e
 from alabamaEncode.encoder.impl.vp9 import EncoderVPX
 
 encoders = [
     EncoderX265(),
@@ -18,14 +19,15 @@
     EncoderX264(),
     EncoderVPX("vp9"),
     EncoderVPX("vp8"),
     EncoderVaapiH265(),
     EncoderVaapiH264(),
     EncoderRav1e(),
     EncoderNVENCH264(),
+    EncoderAppleHEVC()
 ]
 
 
 def get_all_encoder_strings() -> List[str]:
     return [enc.get_pretty_name() for enc in encoders]
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/encoder/impl/Aomenc.py` & `alabamaencoder-0.5.0/alabamaEncode/encoder/impl/Aomenc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 from copy import copy
 from typing import List
 
-from alabamaEncode.core.bin_utils import get_binary
-from alabamaEncode.core.cli_executor import run_cli
+from alabamaEncode.core.util.bin_utils import get_binary
+from alabamaEncode.core.util.cli_executor import run_cli
 from alabamaEncode.encoder.codec import Codec
 from alabamaEncode.encoder.encoder import Encoder
 from alabamaEncode.encoder.rate_dist import EncoderRateDistribution
 
 
 class EncoderAom(Encoder):
     def get_pretty_name(self) -> str:
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/encoder/impl/Nvenc.py` & `alabamaencoder-0.5.0/alabamaEncode/encoder/impl/Nvenc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from alabamaEncode.core.bin_utils import get_binary
+from alabamaEncode.core.util.bin_utils import get_binary
 from alabamaEncode.encoder.codec import Codec
 from alabamaEncode.encoder.encoder import Encoder
 from alabamaEncode.encoder.rate_dist import EncoderRateDistribution
 
 
 class EncoderNVENCH264(Encoder):
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/encoder/impl/SvtAvif.py` & `alabamaencoder-0.5.0/alabamaEncode/encoder/impl/SvtAvif.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 
-from alabamaEncode.core.bin_utils import get_binary, verify_ffmpeg_library
-from alabamaEncode.core.cli_executor import run_cli
+from alabamaEncode.core.util.bin_utils import get_binary, verify_ffmpeg_library
+from alabamaEncode.core.util.cli_executor import run_cli
 
 
 class AvifEncoderSvtenc:
     """
     AVIF Encoder but SvtAv1 inside ffmpeg.
     """
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/encoder/impl/Svtenc.py` & `alabamaencoder-0.5.0/alabamaEncode/encoder/impl/Svtenc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 from typing import List
 
-from alabamaEncode.core.bin_utils import get_binary, check_bin
-from alabamaEncode.core.cli_executor import run_cli
+from alabamaEncode.core.util.bin_utils import get_binary, check_bin
+from alabamaEncode.core.util.cli_executor import run_cli
 from alabamaEncode.encoder.codec import Codec
 from alabamaEncode.encoder.encoder import Encoder
 from alabamaEncode.encoder.rate_dist import EncoderRateDistribution
 
 
 class EncoderSvt(Encoder):
     def get_pretty_name(self) -> str:
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/encoder/impl/VaapiH264.py` & `alabamaencoder-0.5.0/alabamaEncode/encoder/impl/VaapiH264.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from alabamaEncode.core.bin_utils import get_binary
+from alabamaEncode.core.util.bin_utils import get_binary
 from alabamaEncode.encoder.codec import Codec
 from alabamaEncode.encoder.encoder import Encoder
 from alabamaEncode.encoder.rate_dist import EncoderRateDistribution
 
 
 class EncoderVaapiH264(Encoder):
     def get_pretty_name(self) -> str:
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/encoder/impl/VaapiH265.py` & `alabamaencoder-0.5.0/alabamaEncode/encoder/impl/VaapiH265.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from alabamaEncode.core.bin_utils import get_binary
+from alabamaEncode.core.util.bin_utils import get_binary
 from alabamaEncode.encoder.codec import Codec
 from alabamaEncode.encoder.encoder import Encoder
 from alabamaEncode.encoder.rate_dist import EncoderRateDistribution
 
 
 class EncoderVaapiH265(Encoder):
     def get_codec(self) -> Codec:
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/encoder/impl/X264.py` & `alabamaencoder-0.5.0/alabamaEncode/encoder/impl/X264.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
 
-from alabamaEncode.core.bin_utils import get_binary
-from alabamaEncode.core.cli_executor import run_cli
+from alabamaEncode.core.util.bin_utils import get_binary
+from alabamaEncode.core.util.cli_executor import run_cli
 from alabamaEncode.core.ffmpeg import Ffmpeg
-from alabamaEncode.core.path import PathAlabama
+from alabamaEncode.core.util.path import PathAlabama
 from alabamaEncode.encoder.codec import Codec
 from alabamaEncode.encoder.encoder import Encoder
 from alabamaEncode.encoder.rate_dist import EncoderRateDistribution
 
 
 class EncoderX264(Encoder):
     def get_pretty_name(self) -> str:
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/encoder/impl/X265.py` & `alabamaencoder-0.5.0/alabamaEncode/encoder/impl/X265.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List
 
-from alabamaEncode.core.bin_utils import get_binary
-from alabamaEncode.core.cli_executor import run_cli
+from alabamaEncode.core.util.bin_utils import get_binary
+from alabamaEncode.core.util.cli_executor import run_cli
 from alabamaEncode.encoder.codec import Codec
 from alabamaEncode.encoder.encoder import Encoder
 from alabamaEncode.encoder.rate_dist import EncoderRateDistribution
 
 
 class EncoderX265(Encoder):
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/encoder/impl/rav1e.py` & `alabamaencoder-0.5.0/alabamaEncode/encoder/impl/rav1e.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List
 
-from alabamaEncode.core.bin_utils import get_binary
-from alabamaEncode.core.cli_executor import run_cli
+from alabamaEncode.core.util.bin_utils import get_binary
+from alabamaEncode.core.util.cli_executor import run_cli
 from alabamaEncode.encoder.codec import Codec
 from alabamaEncode.encoder.encoder import Encoder
 from alabamaEncode.encoder.rate_dist import EncoderRateDistribution
 
 
 class EncoderRav1e(Encoder):
     def get_pretty_name(self) -> str:
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/encoder/impl/vp9.py` & `alabamaencoder-0.5.0/alabamaEncode/encoder/impl/vp9.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 from typing import List
 
-from alabamaEncode.core.bin_utils import get_binary
-from alabamaEncode.core.cli_executor import run_cli
+from alabamaEncode.core.util.bin_utils import get_binary
+from alabamaEncode.core.util.cli_executor import run_cli
 from alabamaEncode.encoder.codec import Codec
 from alabamaEncode.encoder.encoder import Encoder
 from alabamaEncode.encoder.rate_dist import EncoderRateDistribution
 
 
 class EncoderVPX(Encoder):
     def get_codec(self) -> Codec:
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/encoder/stats.py` & `alabamaencoder-0.5.0/alabamaEncode/encoder/stats.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.3/alabamaEncode/experiments/Aq.py` & `alabamaencoder-0.5.0/alabamaEncode/experiments/Aq.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.3/alabamaEncode/experiments/Overlays.py` & `alabamaencoder-0.5.0/alabamaEncode/experiments/Overlays.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.3/alabamaEncode/experiments/Svtav1Speed.py` & `alabamaencoder-0.5.0/alabamaEncode/experiments/Svtav1Speed.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.3/alabamaEncode/experiments/Svtav1Tunes.py` & `alabamaencoder-0.5.0/alabamaEncode/experiments/Svtav1Tunes.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.3/alabamaEncode/experiments/TemporalFiltering.py` & `alabamaencoder-0.5.0/alabamaEncode/experiments/TemporalFiltering.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.3/alabamaEncode/experiments/ai_feature_extract.py` & `alabamaencoder-0.5.0/alabamaEncode/experiments/ai_feature_extract.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import os
 
 from matplotlib import pyplot as plt
 
-from alabamaEncode.core.cli_executor import run_cli
+from alabamaEncode.core.util.cli_executor import run_cli
 from alabamaEncode.core.ffmpeg import Ffmpeg
 from alabamaEncode.scene.chunk import ChunkObject
 
 if __name__ == "__main__":
     chunk = ChunkObject(
         path="/mnt/data/objective-1-fast/Netflix_RollerCoaster_1280x720_60fps_8bit_420_60f.y4m"
     )
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/experiments/convexhull.py` & `alabamaencoder-0.5.0/alabamaEncode/experiments/convexhull.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import os
 
 from matplotlib import pyplot as plt
 
-from alabamaEncode.core.bin_utils import register_bin
+from alabamaEncode.core.util.bin_utils import register_bin
 from alabamaEncode.encoder.impl.X264 import EncoderX264
 from alabamaEncode.metrics.comparison_display import ComparisonDisplayResolution
+from alabamaEncode.scene.scene_detection import scene_detect
 from alabamaEncode.scene.sequence import ChunkSequence
-from alabamaEncode.scene.split import get_video_scene_list_skinny
 
 if __name__ == "__main__":
     env = "./convexhull"
     env = os.path.abspath(env)
     if not os.path.exists(env):
         os.mkdir(env)
 
-    scenes: ChunkSequence = get_video_scene_list_skinny(
+    scenes: ChunkSequence = scene_detect(
         input_file="/home/kokoniara/ep3_halo_test.mkv",
         max_scene_length=10,
         cache_file_path=f"{env}/scenes_skinny.pt",
     )
 
     register_bin("SvtAv1EncApp", "/home/kokoniara/.local/opt/SvtAv1EncApp")
     target_vmaf = 90
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/experiments/crf_vmaf_relation.py` & `alabamaencoder-0.5.0/alabamaEncode/experiments/crf_vmaf_relation.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 from alabamaEncode.encoder.encoder import Encoder
 from alabamaEncode.encoder.rate_dist import EncoderRateDistribution
 from alabamaEncode.encoder.stats import EncodeStats
 from alabamaEncode.metrics.metric import Metric
 
 print(tf.__version__)
 
-from alabamaEncode.core.bin_utils import register_bin
+from alabamaEncode.core.util.bin_utils import register_bin
 from alabamaEncode.core.ffmpeg import Ffmpeg
 from alabamaEncode.encoder.impl.Svtenc import EncoderSvt
 from alabamaEncode.scene.chunk import ChunkObject
 from alabamaEncode.scene.sequence import ChunkSequence
-from alabamaEncode.scene.split import get_video_scene_list_skinny
+from alabamaEncode.scene.scene_detection import scene_detect
 
 
 def get_complexity(enc: Encoder, c: ChunkObject) -> float:
     _enc = copy.deepcopy(enc)
     _enc.chunk = c
     _enc.speed = 12
     _enc.passes = 1
@@ -97,15 +97,15 @@
     if not os.path.exists(cache_file_name):
         raise Exception("Failed to save cache file")
 
     return local_stats
 
 
 def get_chunks_of_file(path, video_filters):
-    scenes: ChunkSequence = get_video_scene_list_skinny(
+    scenes: ChunkSequence = scene_detect(
         input_file=path, cache_file_path=f"{env}/sceneCache_{os.path.basename(path)}.pt"
     )
 
     for c in scenes.chunks:
         c.video_filters = video_filters
 
     return scenes.chunks
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/experiments/denoise.py` & `alabamaencoder-0.5.0/alabamaEncode/experiments/denoise.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 import shutil
 
-from alabamaEncode.core.timer import Timer
+from alabamaEncode.core.util.timer import Timer
 from alabamaEncode.encoder.impl.X264 import EncoderX264
 from alabamaEncode.encoder.rate_dist import EncoderRateDistribution
 from alabamaEncode.encoder.stats import EncodeStats
 from alabamaEncode.metrics.metric import Metric
 from alabamaEncode.scene.chunk import ChunkObject
 from alabamaEncode.scene.concat import VideoConcatenator
-from alabamaEncode.scene.split import get_video_scene_list_skinny
+from alabamaEncode.scene.scene_detection import scene_detect
 
 counter = 0
 
 if __name__ == "__main__":
     env = "./experiments/CUCKS6"
     input_file = "/mnt/data/60seccut_1500offset.mkv"
 
@@ -68,15 +68,15 @@
     #
     # print(enc.crf)
     # enc.output_path = os.path.join(env, "output.ivf")
     # print(enc.run(calculate_vmaf=True))
 
     # data = []
 
-    scene_list = get_video_scene_list_skinny(
+    scene_list = scene_detect(
         input_file=input_file,
         cache_file_path=env + "/sceneCache.pt",
         max_scene_length=10,
     )
 
     target_vmaf = 93
     epsilon_down = 0.3
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/experiments/sequence_convex.py` & `alabamaencoder-0.5.0/alabamaEncode/experiments/sequence_convex.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import os
 
 from alabamaEncode.conent_analysis.chunk.analyze_steps.target_vmaf import TargetVmaf
-from alabamaEncode.core.alabama import AlabamaContext
-from alabamaEncode.core.bin_utils import register_bin
+from alabamaEncode.core.context import AlabamaContext
+from alabamaEncode.core.util.bin_utils import register_bin
 from alabamaEncode.encoder.impl.X264 import EncoderX264
 from alabamaEncode.metrics.comparison_display import ComparisonDisplayResolution
 from alabamaEncode.metrics.impl.vmaf import VmafOptions
 from alabamaEncode.metrics.metric import Metric
+from alabamaEncode.scene.scene_detection import scene_detect
 from alabamaEncode.scene.sequence import ChunkSequence
-from alabamaEncode.scene.split import get_video_scene_list_skinny
 
 if __name__ == "__main__":
     env = "./seq_convexhull"
     env = os.path.abspath(env)
     if not os.path.exists(env):
         os.mkdir(env)
 
-    scenes: ChunkSequence = get_video_scene_list_skinny(
+    scenes: ChunkSequence = scene_detect(
         input_file="/home/kokoniara/ep3_halo_test.mkv",
         max_scene_length=10,
         cache_file_path=f"{env}/scenes_skinny.pt",
     )
 
     scenes.setup_paths(env, ".mkv")
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/experiments/streaming_output.py` & `alabamaencoder-0.5.0/alabamaEncode/experiments/streaming_output.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-from alabamaEncode.core.bin_utils import register_bin
+from alabamaEncode.core.util.bin_utils import register_bin
 from alabamaEncode.encoder.impl.X264 import EncoderX264
 from alabamaEncode.experiments.util.ExperimentUtil import get_test_files
 from alabamaEncode.scene.chunk import ChunkObject
 
 if __name__ == "__main__":
     test_env = "./tst_streaming_output/"
     test_env = os.path.abspath(test_env)
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/experiments/superres.py` & `alabamaencoder-0.5.0/alabamaEncode/experiments/superres.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.3/alabamaEncode/experiments/target_vmaf.py` & `alabamaencoder-0.5.0/alabamaEncode/experiments/target_vmaf.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.3/alabamaEncode/experiments/util/ExperimentUtil.py` & `alabamaencoder-0.5.0/alabamaEncode/experiments/util/ExperimentUtil.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.3/alabamaEncode/ffmpeg_source/ffmpeg_src.py` & `alabamaencoder-0.5.0/alabamaEncode/core/util/get_yuv_stream.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,21 @@
 import subprocess
 
-from alabamaEncode.ffmpeg_source.yuv import Reader
+from alabamaEncode.core.util.abort_controler import AbortControler
+from alabamaEncode.core.util.yuv import Reader
 from alabamaEncode.scene.chunk import ChunkObject
 
 
-class AbortControler:
-    def __init__(self):
-        self.aborted = False
-
-    def abort(self):
-        self.aborted = True
-
 def get_yuv_frame_stream(chunk: ChunkObject, frame_callback, vf: str= "", abort_controler: AbortControler = None):
     command = chunk.create_chunk_ffmpeg_pipe_command(video_filters=vf, bit_depth=8)
 
     ffmpeg_process = subprocess.Popen(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
 
     yuv_reader = Reader(frame_callback)
 
     while ffmpeg_process.poll() is None:
         if abort_controler:
             if abort_controler.aborted:
                 break
         data = ffmpeg_process.stdout.read(1024 * 1024)
         if data:
             yuv_reader.decode(data)
-
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/ffmpeg_source/yuv.py` & `alabamaencoder-0.5.0/alabamaEncode/core/util/yuv.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.3/alabamaEncode/metrics/calculate.py` & `alabamaencoder-0.5.0/alabamaEncode/metrics/calculate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import re
 
-from alabamaEncode.core.bin_utils import get_binary
-from alabamaEncode.core.cli_executor import run_cli
-from alabamaEncode.core.path import PathAlabama
+from alabamaEncode.core.util.bin_utils import get_binary
+from alabamaEncode.core.util.cli_executor import run_cli
+from alabamaEncode.core.util.path import PathAlabama
 from alabamaEncode.encoder.stats import EncodeStats
 from alabamaEncode.metrics.impl.ssimu2 import Ssimu2Options
 from alabamaEncode.metrics.impl.vmaf import VmafOptions
 from alabamaEncode.metrics.metric import Metric
 from alabamaEncode.metrics.options import MetricOptions
 from alabamaEncode.scene.chunk import ChunkObject
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/metrics/comparison_display.py` & `alabamaencoder-0.5.0/alabamaEncode/metrics/comparison_display.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.3/alabamaEncode/metrics/image.py` & `alabamaencoder-0.5.0/alabamaEncode/metrics/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import re
 
-from alabamaEncode.core.cli_executor import run_cli
-from alabamaEncode.core.bin_utils import get_binary
+from alabamaEncode.core.util.cli_executor import run_cli
+from alabamaEncode.core.util.bin_utils import get_binary
 
 
 class ImageMetrics:
     @staticmethod
     def butteraugli_score(reference_img_path: str, distorted_img_path: str):
         if not os.path.exists(reference_img_path) or not os.path.exists(
             distorted_img_path
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/metrics/impl/psnr.py` & `alabamaencoder-0.5.0/alabamaEncode/metrics/impl/psnr.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 
-from alabamaEncode.core.bin_utils import get_binary
-from alabamaEncode.core.cli_executor import run_cli
+from alabamaEncode.core.util.bin_utils import get_binary
+from alabamaEncode.core.util.cli_executor import run_cli
 from alabamaEncode.scene.chunk import ChunkObject
 
 
 def get_video_psnr(distorted_path, in_chunk: ChunkObject = None):
     null_ = in_chunk.create_chunk_ffmpeg_pipe_command()
     null_ += f" | {get_binary('ffmpeg')} -hide_banner -i - "
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/metrics/impl/ssim.py` & `alabamaencoder-0.5.0/alabamaEncode/metrics/impl/ssim.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import re
 
-from alabamaEncode.core.bin_utils import get_binary
-from alabamaEncode.core.cli_executor import run_cli
+from alabamaEncode.core.util.bin_utils import get_binary
+from alabamaEncode.core.util.cli_executor import run_cli
 from alabamaEncode.scene.chunk import ChunkObject
 
 
 def get_video_ssim(
     distorted_path,
     in_chunk: ChunkObject = None,
     print_output=False,
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/metrics/impl/ssimu2.py` & `alabamaencoder-0.5.0/alabamaEncode/metrics/impl/ssimu2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from alabamaEncode.core.bin_utils import get_binary, register_bin
-from alabamaEncode.core.cli_executor import run_cli_parallel
-from alabamaEncode.core.path import PathAlabama
+from alabamaEncode.core.util.bin_utils import get_binary, register_bin
+from alabamaEncode.core.util.cli_executor import run_cli_parallel
+from alabamaEncode.core.util.path import PathAlabama
 
 
 from alabamaEncode.metrics.exception import Ssimu2Exception
 from alabamaEncode.metrics.metric import Metric
 from alabamaEncode.metrics.options import MetricOptions
 from alabamaEncode.metrics.result import MetricResult
 from alabamaEncode.scene.chunk import ChunkObject
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/metrics/impl/vmaf.py` & `alabamaencoder-0.5.0/alabamaEncode/metrics/impl/vmaf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import os
 from statistics import mean
 
-from alabamaEncode.core.bin_utils import get_binary
-from alabamaEncode.core.bin_utils import register_bin
-from alabamaEncode.core.cli_executor import run_cli_parallel
-from alabamaEncode.core.path import PathAlabama
+from alabamaEncode.core.util.bin_utils import get_binary
+from alabamaEncode.core.util.bin_utils import register_bin
+from alabamaEncode.core.util.cli_executor import run_cli_parallel
+from alabamaEncode.core.util.path import PathAlabama
 from alabamaEncode.metrics.exception import VmafException
 from alabamaEncode.metrics.metric import Metric
 from alabamaEncode.metrics.options import MetricOptions
 from alabamaEncode.metrics.result import MetricResult
 from alabamaEncode.scene.chunk import ChunkObject
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/parallelEncoding/CeleryAutoscaler.py` & `alabamaencoder-0.5.0/alabamaEncode/parallel_execution/celery_autoscaler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import multiprocessing
 import os
 import re
 
 from celery.worker.autoscale import Autoscaler as CeleryAutoscaler
 
-from alabamaEncode.core.cli_executor import run_cli
+from alabamaEncode.core.util.cli_executor import run_cli
 
 
 # https://gist.github.com/hussainfolio3/c5246f59f9e5c31fa720524fb45b2077
 # never go above one worker = one core
 # if we have 12 cores then max is 12 workers
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/parallelEncoding/execute_commands.py` & `alabamaencoder-0.5.0/alabamaEncode/parallel_execution/execute_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from concurrent.futures import ThreadPoolExecutor
 from typing import List, Tuple
 
 import psutil
 from tqdm import tqdm
 
 from alabamaEncode.core.chunk_job import ChunkEncoder
-from alabamaEncode.parallelEncoding.CeleryApp import run_command_on_celery, app
-from alabamaEncode.parallelEncoding.command import BaseCommandObject
+from alabamaEncode.parallel_execution.celery_app import run_command_on_celery, app
+from alabamaEncode.parallel_execution.command import BaseCommandObject
 
 
 async def execute_commands(
     use_celery=False,
     command_objects: List[BaseCommandObject] = None,
     multiprocess_workers: int = -1,
     pin_to_cores=False,
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/scene/annel.py` & `alabamaencoder-0.5.0/alabamaEncode/scene/annel.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.3/alabamaEncode/scene/chunk.py` & `alabamaencoder-0.5.0/alabamaEncode/scene/chunk.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os.path
 
 from tqdm import tqdm
 
 from alabamaEncode.core.ffmpeg import Ffmpeg
-from alabamaEncode.core.kv import AlabamaKv
-from alabamaEncode.core.path import PathAlabama
+from alabamaEncode.core.util.kv import AlabamaKv
+from alabamaEncode.core.util.path import PathAlabama
 
 
 class WrongFrameCountError(Exception):
     def __init__(self, expected_frame_count: int = -1, actual_frame_count: int = -1):
         # super().__init__("The frame count of the chunk is not equal to the expected")
         super().__init__(
             f"Expected {expected_frame_count} frames, got {actual_frame_count}"
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/scene/concat.py` & `alabamaencoder-0.5.0/alabamaEncode/scene/concat.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 import tempfile
 import time
 from typing import List
 
 from tqdm import tqdm
 
-from alabamaEncode.core.bin_utils import get_binary
-from alabamaEncode.core.cli_executor import run_cli
+from alabamaEncode.core.util.bin_utils import get_binary
+from alabamaEncode.core.util.cli_executor import run_cli
 from alabamaEncode.core.ffmpeg import Ffmpeg
-from alabamaEncode.core.path import PathAlabama
+from alabamaEncode.core.util.path import PathAlabama
 
 
 class VideoConcatenator:
     def __init__(
         self,
         files: List[str] = None,
         output: str = None,
@@ -177,22 +177,33 @@
         for track in tracks:
             if track["codec_type"] == "audio":
                 has_audio_track = True
                 break
 
         return has_audio_track
 
+    def has_sub_track(self) -> bool:
+        has_sub_track = False
+        tracks = Ffmpeg.get_tracks(PathAlabama(self.file_with_audio))
+        for track in tracks:
+            if track["codec_type"] == "subtitle":
+                has_sub_track = True
+                break
+
+        return has_sub_track
+
     def _concat_videos(self):
         if os.path.exists(self.output):
             print(f"File {self.output} already exists")
             return
 
         self.concat_video_track()
 
         has_audio_track = self.has_audio_track()
+        has_sub_track = self.has_sub_track()
 
         if self.audio_only:
             if not has_audio_track:
                 print("No audio track found, not encoding")
                 return
 
             print("Encoding a audio track only")
@@ -267,15 +278,15 @@
                 "-stats",
                 "-v error",
                 f'-i "{self.vid_output}"',
                 f'-i "{self.audio_output}"',
             ]
 
             sub_tracks = []
-            if self.copy_included_subs:
+            if self.copy_included_subs and has_sub_track:
                 sub_tracks = self.extract_subs(
                     start_offset=start_offset_command, end_offset=end_offset_command
                 )
 
                 for out_path, tag_lang, tag_title, track_index in sub_tracks:
                     vec += [
                         f'-i "{out_path}"',
@@ -310,28 +321,24 @@
                 "-fflags +bitexact",
                 "-flags:v +bitexact",
                 "-flags:a +bitexact",
                 f'"{self.output}"',
             ]
 
             final_command = " ".join(vec)
-            print(final_command)
-            # print(f"running: {final_command}")
             out = run_cli(final_command).verify().get_output()
             if (
                 "Subtitle encoding currently only possible from text to text or bitmap to bitmap"
                 in str(out)
             ):
                 print("Subtitle encoding failed, trying again")
                 for a in vec:
                     if "mov_text" in a or "map 2:s" in a:
                         vec.remove(a)
                 final_command = " ".join(vec)
-                # print(f"running: {final_command}")
-                print(final_command)
                 run_cli(final_command).verify()
         else:
             subs_i = ""
             subs_map = ""
             if len(self.subs_file) > 0 and self.subs_file[0] != "":
                 if start_offset_command != "":
                     # offset each track using -itsoffset {offset} -ss {offset}
@@ -353,15 +360,14 @@
 
             final_command = (
                 f'{get_binary("ffmpeg")} -y -stats -v error -i "{self.vid_output}" -i "{self.audio_output}" '
                 f'{subs_i} {start_offset_command} -i "{self.file_with_audio}" {end_offset_command} '
                 f"{title_bit} -map 0:v -map 1:a {subs_map} -movflags +faststart -map_chapters -1 "
                 f'-c:v copy -c:a copy -vsync cfr "{self.output}"'
             )
-            # print(f"running: {final_command}")
             os.system(final_command)
 
         os.remove(self.vid_output)
         os.remove(self.audio_output)
 
         if Ffmpeg.check_for_invalid(PathAlabama(self.output)):
             os.remove(self.output)
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/scene/sequence.py` & `alabamaencoder-0.5.0/alabamaEncode/scene/sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import copy
 import os
 import random
 from typing import List
 
 from tqdm.asyncio import tqdm
 
-from alabamaEncode.core.kv import AlabamaKv
+from alabamaEncode.core.util.kv import AlabamaKv
 from alabamaEncode.scene.chunk import ChunkObject
 
 
 class ChunkSequence:
     """
     A sequence of chunks.
     """
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode/scene/split.py` & `alabamaencoder-0.5.0/alabamaEncode/scene/scene_detection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import copy
 import json
 import os
 
 from scenedetect import detect, AdaptiveDetector
 
 from alabamaEncode.core.ffmpeg import Ffmpeg
-from alabamaEncode.core.path import PathAlabama
+from alabamaEncode.core.util.path import PathAlabama
 from alabamaEncode.scene.chunk import ChunkObject
 from alabamaEncode.scene.sequence import ChunkSequence
 
 
-def get_video_scene_list_skinny(
+def scene_detect(
     input_file: str,
     cache_file_path: str,
     max_scene_length: int = 10,
     start_offset=-1,
     end_offset=-1,
     override_bad_wrong_cache_path=False,
     static_length=False,
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode_frontends/cli/__main__.py` & `alabamaencoder-0.5.0/alabamaEncode/cli/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/python
 import asyncio
 import atexit
 import os
 import sys
 import time
 
-from alabamaEncode.core.alabama import AlabamaContext
+from alabamaEncode.cli.cli_setup.autopaths import auto_output_paths
+from alabamaEncode.cli.cli_setup.cli_args import read_args
+from alabamaEncode.cli.cli_setup.paths import parse_paths
+from alabamaEncode.cli.cli_setup.ratecontrol import parse_rd
+from alabamaEncode.cli.cli_setup.res_preset import parse_resolution_presets
+from alabamaEncode.cli.cli_setup.validate_files import validate_input
+from alabamaEncode.cli.cli_setup.video_filters import parse_video_filters
+from alabamaEncode.core.context import AlabamaContext
 from alabamaEncode.core.extras.auto_thumbnailer import AutoThumbnailer
 from alabamaEncode.core.job import AlabamaEncodingJob
-from alabamaEncode.parallelEncoding.CeleryApp import app
-from alabamaEncode.parallelEncoding.worker import worker
-from alabamaEncode_frontends.cli.cli_setup.autopaths import auto_output_paths
-from alabamaEncode_frontends.cli.cli_setup.cli_args import read_args
-from alabamaEncode_frontends.cli.cli_setup.paths import parse_paths
-from alabamaEncode_frontends.cli.cli_setup.ratecontrol import parse_rd
-from alabamaEncode_frontends.cli.cli_setup.res_preset import parse_resolution_presets
-from alabamaEncode_frontends.cli.cli_setup.validate_files import validate_input
-from alabamaEncode_frontends.cli.cli_setup.video_filters import parse_video_filters
+from alabamaEncode.parallel_execution.celery_app import app
+from alabamaEncode.parallel_execution.worker import worker
 
 runtime = -1
 runtime_file = ""
 lock_file_path = ""
 
 
 def setup_context_for_standalone_usage() -> AlabamaContext:
@@ -41,29 +41,39 @@
         parse_resolution_presets,
         parse_video_filters,
     ]
     for pipeline_item in creation_pipeline:
         ctx = pipeline_item(ctx)
     return ctx
 
+def fmt_time(seconds) -> str:
+    # Convert seconds to hours and remaining seconds
+    hours, remainder = divmod(seconds, 3600)
+
+    # If at least one hour has passed
+    if hours:
+        return f"{int(hours)} hour(s) {int(remainder)} second(s)"
+    else:
+        return f"{int(seconds)} second(s)"
 
 @atexit.register
 def at_exit():
     global runtime
     global runtime_file
     if runtime != -1:
         current_session_runtime = time.time() - runtime
 
         saved_runtime = 0
         if os.path.exists(runtime_file):
             with open(runtime_file) as f:
                 saved_runtime = float(f.read())
         print(
-            f"Current Session Runtime: {current_session_runtime}, Runtime From Previous Sessions: {saved_runtime},"
-            f" Total Runtime: {current_session_runtime + saved_runtime}"
+            f"Current Session Runtime: {fmt_time(current_session_runtime)},"
+            f" Runtime From Previous Sessions: {fmt_time(saved_runtime)},"
+            f" Total Runtime: {fmt_time(current_session_runtime + saved_runtime)}"
         )
 
         try:
             with open(runtime_file, "w") as f:
                 f.write(str(current_session_runtime + saved_runtime))
         except FileNotFoundError:
             pass
@@ -83,15 +93,14 @@
     runtime = time.time()
 
     ctx: [AlabamaContext | None] = None
 
     if len(sys.argv) > 1:
         match sys.argv[1]:
             case "clear":
-                # if a user does 'python __main__.py clear' then clear the celery queue
                 print("Clearing celery queue")
                 app.control.purge()
                 quit()
             case "worker":
                 worker()
 
     if ctx is None:
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode_frontends/cli/cli_setup/autopaths.py` & `alabamaencoder-0.5.0/alabamaEncode/cli/cli_setup/autopaths.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import re
 
-from alabamaEncode.core.alabama import AlabamaContext
+from alabamaEncode.core.context import AlabamaContext
 
 
 def parse_movie_title(title):
     match = re.match(r"^(.*?) \((\d{4})\)$", title)
     if match:
         return match.group(1), match.group(2)
     return None
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode_frontends/cli/cli_setup/cli_args.py` & `alabamaencoder-0.5.0/alabamaEncode/cli/cli_setup/cli_args.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         description="AlabamaEncoder, one and only encoder framework for all your needs*",
         epilog="*not really",
     )
     parser.add_argument("input", type=str, help="Input video file")
     parser.add_argument("output", type=str, help="Output video file")
 
     parser.add_argument(
-        "--dont-encode_audio",
+        "--dont_encode_audio",
         help="Mux audio",
         action="store_false",
         dest="encode_audio",
     )
 
     parser.add_argument(
         "--audio_params",
@@ -88,15 +88,15 @@
         "--vbr_perchunk_optimisation",
         help="Enable automatic bitrate optimisation per chunk",
         action="store_true",
         dest="vbr_perchunk_optimisation",
     )
 
     parser.add_argument(
-        "--multiprocess_workers",
+        "--multiprocess_workers", '--workers', '-j',
         help="Number of workers to use for multiprocessing, if -1 the program will auto scale",
         type=int,
         default=ctx.multiprocess_workers,
         dest="multiprocess_workers",
     )
 
     parser.add_argument(
@@ -164,26 +164,20 @@
         "--scene_merge",
         help="Merge scenes until they met the max scene length",
         action="store_true",
         dest="scene_merge",
     )
 
     parser.add_argument(
-        "--no_crf_based_vmaf_targeting",
+        "--no_crf_based_vmaf_targeting", '--crf_mode',
         help="per chunk, find a crf that hits target quality and encode using that",
         action="store_false",
         dest="crf_based_vmaf_targeting",
     )
 
-    parser.add_argument(
-        "--auto_crf",
-        help="Find a crf that hits target vmaf, calculate a peak bitrate cap, and encode using that",
-        action="store_false",
-        dest="crf_bitrate_mode",
-    )
 
     parser.add_argument(
         "--chunk_order",
         help="Encode chunks in a specific order",
         type=str,
         default=ctx.chunk_order,
         choices=[
@@ -253,15 +247,15 @@
         help="Override the check for input file path matching in scene cache loading",
         action="store_true",
         default=ctx.override_scenecache_path_check,
         dest="override_bad_wrong_cache_path",
     )
 
     parser.add_argument(
-        "--hdr",
+        "--hdr", '-hdr',
         help="Encode in HDR, if not specified and input is hdr it will automatically tonemap",
         action="store_true",
         default=ctx.prototype_encoder.hdr,
         dest="hdr",
     )
 
     parser.add_argument(
@@ -296,46 +290,29 @@
         type=str,
         default=ctx.prototype_encoder.override_flags,
         help="Override the encoder flags with this string, write all params except paths",
         dest="encoder_flag_override",
     )
 
     parser.add_argument(
-        "--encoder_speed_override",
+        "--encoder_speed_override", '--enc_speed',
         type=int,
         action=range_action(0, 10),
         default=ctx.prototype_encoder.speed,
         help="Override the encoder speed parameter",
         dest="encoder_speed_override",
     )
 
-    parser.add_argument(
-        "--flag1",
-        action="store_true",
-        help="find what crf matches config.bitrate, encode at that crf and redo if the crf bitrate is higher then set",
-        dest="flag1",
-    )
-
-    parser.add_argument(
-        "--flag2", action="store_true", help="Used for debugging", dest="flag2"
-    )
 
     parser.add_argument(
-        "--flag3",
-        action="store_true",
-        help="Find best bitrate using the top 5%% of most complex chunks",
-        dest="flag3",
-    )
-
-    parser.add_argument(
-        "--flag4",
+        "--crf_map",
         type=str,
         help="Map of crf <-> chunk index, for debugging purposes only",
         default=ctx.crf_map,
-        dest="flag4",
+        dest="crf_map",
     )
 
     parser.add_argument(
         "--color-primaries",
         type=str,
         default=ctx.prototype_encoder.color_primaries,
         help="Color primaries",
@@ -410,15 +387,15 @@
         "--auto_accept_autocrop",
         action="store_true",
         help="Automatically accept autocrop",
         dest="auto_accept_autocrop",
     )
 
     parser.add_argument(
-        "--resolution_preset",
+        "--resolution_preset", '-res',
         type=str,
         default=ctx.resolution_preset,
         help="Preset for the scale filter, possible choices are 4k 1440p 1080p 768p 720p 540p 480p 360p",
         dest="resolution_preset",
     )
 
     parser.add_argument(
@@ -427,15 +404,16 @@
         default=ctx.probe_count,
         help="Max number of probes for metric targeting, higher is more accurate but slower",
         action=range_action(1, 10),
         dest="probe_count",
     )
 
     parser.add_argument(
-        "--probe_speed_override",
+        "--probe_speed",
+        dest="probe_speed_override",
         type=int,
         default=ctx.prototype_encoder.speed,
         help="Override the speed for target vmaf probes",
         action=range_action(0, 10),
     )
 
     parser.add_argument(
@@ -444,21 +422,14 @@
         default=ctx.vmaf_reference_display,
         choices=["HD", "FHD", "UHD"],
         help="HD FHD UHD",
         dest="vmaf_reference_display",
     )
 
     parser.add_argument(
-        "--vmaf_ai_assisted_targeting",
-        action="store_true",
-        help="use vmaf ai assisted targeting",
-        dest="vmaf_ai_assisted_targeting",
-    )
-
-    parser.add_argument(
         "--vmaf_target_repesentation",
         type=str,
         default=ctx.vmaf_target_representation,
         help="vmaf target representation, default is mean",
         choices=[
             "mean",
             "min",
@@ -556,15 +527,15 @@
         dest="denoise_vmaf_ref",
     )
 
     parser.add_argument(
         "--calc_final_vmaf",
         default=ctx.calc_final_vmaf,
         action="store_true",
-        help="Dont calculate final vmaf",
+        help="Calculate vmaf of the final chunk at the end",
         dest="calc_final_vmaf",
     )
 
     parser.add_argument(
         "--multi_res_pipeline",
         action="store_true",
         help="Create a optimised multi bitrate tier stream",
@@ -596,24 +567,20 @@
     ctx.dry_run = args.dry_run
     ctx.ssim_db_target = args.ssim_db_target
     ctx.simple_denoise = args.simple_denoise
     ctx.vmaf = args.vmaf_target
     ctx.vbr_perchunk_optimisation = args.vbr_perchunk_optimisation
     ctx.crf_based_vmaf_targeting = args.crf_based_vmaf_targeting
     ctx.use_celery = args.use_celery
-    ctx.flag1 = args.flag1
-    ctx.flag2 = args.flag2
-    ctx.flag3 = args.flag3
     ctx.prototype_encoder.override_flags = args.encoder_flag_override
     ctx.prototype_encoder.speed = args.encoder_speed_override
     ctx.multiprocess_workers = args.multiprocess_workers
     ctx.bitrate_adjust_mode = args.bitrate_adjust_mode
     ctx.bitrate_undershoot = args.bitrate_undershoot
     ctx.bitrate_overshoot = args.bitrate_overshoot
-    ctx.crf_bitrate_mode = args.crf_bitrate_mode
     ctx.prototype_encoder.crf = args.crf
     ctx.prototype_encoder.hdr = args.hdr
     ctx.max_scene_length = args.max_scene_length
     ctx.start_offset = args.start_offset
     ctx.end_offset = args.end_offset
     ctx.override_scenecache_path_check = args.override_bad_wrong_cache_path
     ctx.crop_string = args.crop_string
@@ -638,16 +605,15 @@
     ctx.vmaf_4k_model = args.vmaf_4k_model
     ctx.vmaf_no_motion = args.vmaf_no_motion
     ctx.auto_accept_autocrop = args.auto_accept_autocrop
     ctx.resolution_preset = args.resolution_preset
     ctx.probe_count = args.probe_count
     ctx.vmaf_reference_display = args.vmaf_reference_display
     ctx.probe_speed_override = args.probe_speed_override
-    ctx.crf_map = args.flag4
-    ctx.ai_vmaf_targeting = args.vmaf_ai_assisted_targeting
+    ctx.crf_map = args.crf_map
     ctx.pin_to_cores = args.dont_pin_to_cores
     ctx.prototype_encoder.niceness = args.niceness
     ctx.vmaf_target_representation = args.vmaf_target_repesentation
     ctx.print_analysis_logs = args.print_analysis_logs
     ctx.poster_url = args.poster_url
     ctx.offload_server = args.offload_server
     ctx.dynamic_vmaf_target = args.dynamic_vmaf_target
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode_frontends/cli/cli_setup/paths.py` & `alabamaencoder-0.5.0/alabamaEncode/cli/cli_setup/paths.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.3/alabamaEncode_frontends/cli/cli_setup/res_preset.py` & `alabamaencoder-0.5.0/alabamaEncode/cli/cli_setup/res_preset.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.3/alabamaEncode_frontends/cli/cli_setup/validate_files.py` & `alabamaencoder-0.5.0/alabamaEncode/cli/cli_setup/validate_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from alabamaEncode.core.ffmpeg import Ffmpeg
-from alabamaEncode.core.path import PathAlabama
+from alabamaEncode.core.util.path import PathAlabama
 
 
 def validate_input(ctx):
     try:
         tracks = Ffmpeg.get_tracks(PathAlabama(ctx.raw_input_file))
         video_track = None
         for track in tracks:
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode_frontends/cli/cli_setup/video_filters.py` & `alabamaencoder-0.5.0/alabamaEncode/cli/cli_setup/video_filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from alabamaEncode.core.ffmpeg import Ffmpeg
-from alabamaEncode.core.path import PathAlabama
+from alabamaEncode.core.util.path import PathAlabama
 
 
 def parse_video_filters(ctx):
     """
     Sets up the video filters
     """
     # make --video_filters mutually exclusive with --hdr --crop_string --scale_string
```

### Comparing `alabamaencoder-0.4.3/alabamaEncode_frontends/demon/demon.py` & `alabamaencoder-0.5.0/alabamaEncode/demon/demon.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.3/alabamaEncoder.egg-info/SOURCES.txt` & `alabamaencoder-0.5.0/alabamaEncoder.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,77 +1,89 @@
 setup.py
 alabamaEncode/__init__.py
 alabamaEncode/ai_vmaf/__init__.py
 alabamaEncode/ai_vmaf/aom_firstpass.py
 alabamaEncode/ai_vmaf/perdict.py
 alabamaEncode/ai_vmaf/train/__init__.py
 alabamaEncode/ai_vmaf/train/train.py
+alabamaEncode/cli/__init__.py
+alabamaEncode/cli/__main__.py
+alabamaEncode/cli/cli_setup/__init__.py
+alabamaEncode/cli/cli_setup/autopaths.py
+alabamaEncode/cli/cli_setup/cli_args.py
+alabamaEncode/cli/cli_setup/paths.py
+alabamaEncode/cli/cli_setup/ratecontrol.py
+alabamaEncode/cli/cli_setup/res_preset.py
+alabamaEncode/cli/cli_setup/validate_files.py
+alabamaEncode/cli/cli_setup/video_filters.py
 alabamaEncode/conent_analysis/__init__.py
 alabamaEncode/conent_analysis/opinionated_vmaf.py
 alabamaEncode/conent_analysis/pipelines.py
 alabamaEncode/conent_analysis/refine_step.py
 alabamaEncode/conent_analysis/chunk/__init__.py
 alabamaEncode/conent_analysis/chunk/chunk_analyse_step.py
 alabamaEncode/conent_analysis/chunk/final_encode_step.py
 alabamaEncode/conent_analysis/chunk/analyze_steps/__init__.py
-alabamaEncode/conent_analysis/chunk/analyze_steps/capped_crf.py
 alabamaEncode/conent_analysis/chunk/analyze_steps/manual_crf.py
 alabamaEncode/conent_analysis/chunk/analyze_steps/multires_encode_candidates.py
 alabamaEncode/conent_analysis/chunk/analyze_steps/optimised_vbr.py
 alabamaEncode/conent_analysis/chunk/analyze_steps/per_scene_grain.py
 alabamaEncode/conent_analysis/chunk/analyze_steps/plain_crf.py
 alabamaEncode/conent_analysis/chunk/analyze_steps/plain_vbr.py
 alabamaEncode/conent_analysis/chunk/analyze_steps/target_vmaf.py
 alabamaEncode/conent_analysis/chunk/final_encode_steps/__init__.py
-alabamaEncode/conent_analysis/chunk/final_encode_steps/ai_targeted_vmaf.py
-alabamaEncode/conent_analysis/chunk/final_encode_steps/capped_crf_encode.py
 alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf.py
 alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf_vbr.py
 alabamaEncode/conent_analysis/chunk/final_encode_steps/multires_encode_finals.py
 alabamaEncode/conent_analysis/chunk/final_encode_steps/plain.py
 alabamaEncode/conent_analysis/refine_steps/__init__.py
 alabamaEncode/conent_analysis/refine_steps/multires_package.py
 alabamaEncode/conent_analysis/refine_steps/multires_trellis.py
 alabamaEncode/conent_analysis/sequence/__init__.py
 alabamaEncode/conent_analysis/sequence/args_tune.py
 alabamaEncode/conent_analysis/sequence/autocrop.py
 alabamaEncode/conent_analysis/sequence/denoise_filtering.py
 alabamaEncode/conent_analysis/sequence/encoding_tiles.py
-alabamaEncode/conent_analysis/sequence/ideal_crf.py
 alabamaEncode/conent_analysis/sequence/scrape_hdr_meta.py
 alabamaEncode/conent_analysis/sequence/sequence_autograin.py
 alabamaEncode/conent_analysis/sequence/taget_ssimdb.py
-alabamaEncode/conent_analysis/sequence/target_bitrate_optimisation.py
 alabamaEncode/conent_analysis/sequence/x264_tune.py
 alabamaEncode/core/__init__.py
-alabamaEncode/core/alabama.py
-alabamaEncode/core/bin_utils.py
 alabamaEncode/core/chunk_job.py
-alabamaEncode/core/cli_executor.py
+alabamaEncode/core/context.py
 alabamaEncode/core/ffmpeg.py
 alabamaEncode/core/final_touches.py
 alabamaEncode/core/job.py
-alabamaEncode/core/kv.py
-alabamaEncode/core/path.py
-alabamaEncode/core/timer.py
-alabamaEncode/core/ws_update.py
 alabamaEncode/core/extras/__init__.py
 alabamaEncode/core/extras/auto_thumbnailer.py
+alabamaEncode/core/extras/ws_update.py
+alabamaEncode/core/util/__init__.py
+alabamaEncode/core/util/abort_controler.py
+alabamaEncode/core/util/bin_utils.py
+alabamaEncode/core/util/cli_executor.py
+alabamaEncode/core/util/get_yuv_stream.py
+alabamaEncode/core/util/kv.py
+alabamaEncode/core/util/path.py
+alabamaEncode/core/util/timer.py
+alabamaEncode/core/util/yuv.py
+alabamaEncode/demon/__init__.py
+alabamaEncode/demon/demon.py
 alabamaEncode/encoder/__init__.py
 alabamaEncode/encoder/codec.py
 alabamaEncode/encoder/encoder.py
 alabamaEncode/encoder/encoder_factory.py
 alabamaEncode/encoder/rate_dist.py
 alabamaEncode/encoder/stats.py
 alabamaEncode/encoder/impl/Aomenc.py
 alabamaEncode/encoder/impl/Nvenc.py
 alabamaEncode/encoder/impl/SvtAvif.py
 alabamaEncode/encoder/impl/Svtenc.py
 alabamaEncode/encoder/impl/VaapiH264.py
 alabamaEncode/encoder/impl/VaapiH265.py
+alabamaEncode/encoder/impl/VideoToolbox.py
 alabamaEncode/encoder/impl/X264.py
 alabamaEncode/encoder/impl/X265.py
 alabamaEncode/encoder/impl/__init__.py
 alabamaEncode/encoder/impl/rav1e.py
 alabamaEncode/encoder/impl/vp9.py
 alabamaEncode/experiments/Aq.py
 alabamaEncode/experiments/Overlays.py
@@ -87,54 +99,38 @@
 alabamaEncode/experiments/sequence_convex.py
 alabamaEncode/experiments/serialise_context.py
 alabamaEncode/experiments/streaming_output.py
 alabamaEncode/experiments/superres.py
 alabamaEncode/experiments/target_vmaf.py
 alabamaEncode/experiments/util/ExperimentUtil.py
 alabamaEncode/experiments/util/__init__.py
-alabamaEncode/ffmpeg_source/__init__.py
-alabamaEncode/ffmpeg_source/ffmpeg_src.py
-alabamaEncode/ffmpeg_source/yuv.py
 alabamaEncode/metrics/__init__.py
 alabamaEncode/metrics/calculate.py
 alabamaEncode/metrics/comparison_display.py
 alabamaEncode/metrics/exception.py
 alabamaEncode/metrics/image.py
 alabamaEncode/metrics/metric.py
 alabamaEncode/metrics/options.py
 alabamaEncode/metrics/result.py
 alabamaEncode/metrics/impl/__init__.py
 alabamaEncode/metrics/impl/psnr.py
 alabamaEncode/metrics/impl/ssim.py
 alabamaEncode/metrics/impl/ssimu2.py
 alabamaEncode/metrics/impl/vmaf.py
-alabamaEncode/parallelEncoding/CeleryApp.py
-alabamaEncode/parallelEncoding/CeleryAutoscaler.py
-alabamaEncode/parallelEncoding/__init__.py
-alabamaEncode/parallelEncoding/command.py
-alabamaEncode/parallelEncoding/execute_commands.py
-alabamaEncode/parallelEncoding/worker.py
+alabamaEncode/parallel_execution/__init__.py
+alabamaEncode/parallel_execution/celery_app.py
+alabamaEncode/parallel_execution/celery_autoscaler.py
+alabamaEncode/parallel_execution/command.py
+alabamaEncode/parallel_execution/execute_commands.py
+alabamaEncode/parallel_execution/worker.py
 alabamaEncode/scene/__init__.py
 alabamaEncode/scene/annel.py
 alabamaEncode/scene/chunk.py
 alabamaEncode/scene/concat.py
+alabamaEncode/scene/scene_detection.py
 alabamaEncode/scene/sequence.py
-alabamaEncode/scene/split.py
-alabamaEncode_frontends/__init__.py
-alabamaEncode_frontends/cli/__init__.py
-alabamaEncode_frontends/cli/__main__.py
-alabamaEncode_frontends/cli/cli_setup/__init__.py
-alabamaEncode_frontends/cli/cli_setup/autopaths.py
-alabamaEncode_frontends/cli/cli_setup/cli_args.py
-alabamaEncode_frontends/cli/cli_setup/paths.py
-alabamaEncode_frontends/cli/cli_setup/ratecontrol.py
-alabamaEncode_frontends/cli/cli_setup/res_preset.py
-alabamaEncode_frontends/cli/cli_setup/validate_files.py
-alabamaEncode_frontends/cli/cli_setup/video_filters.py
-alabamaEncode_frontends/demon/__init__.py
-alabamaEncode_frontends/demon/demon.py
 alabamaEncoder.egg-info/PKG-INFO
 alabamaEncoder.egg-info/SOURCES.txt
 alabamaEncoder.egg-info/dependency_links.txt
 alabamaEncoder.egg-info/entry_points.txt
 alabamaEncoder.egg-info/requires.txt
 alabamaEncoder.egg-info/top_level.txt
```

