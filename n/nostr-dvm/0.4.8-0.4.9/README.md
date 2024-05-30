# Comparing `tmp/nostr_dvm-0.4.8.tar.gz` & `tmp/nostr_dvm-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nostr_dvm-0.4.8.tar", last modified: Sat May 25 22:37:57 2024, max compression
+gzip compressed data, was "nostr_dvm-0.4.9.tar", last modified: Thu May 30 08:14:03 2024, max compression
```

## Comparing `nostr_dvm-0.4.8.tar` & `nostr_dvm-0.4.9.tar`

### file list

```diff
@@ -1,116 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:37:57.249195 nostr_dvm-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-25 22:37:57.249195 nostr_dvm-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:37:57.233195 nostr_dvm-0.4.8/nostr_dvm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:37:57.233195 nostr_dvm-0.4.8/nostr_dvm/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:37:57.233195 nostr_dvm-0.4.8/nostr_dvm/backends/mlx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/backends/mlx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:37:57.233195 nostr_dvm-0.4.8/nostr_dvm/backends/mlx/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/backends/mlx/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:37:57.233195 nostr_dvm-0.4.8/nostr_dvm/backends/mlx/modules/stable_diffusion/
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:37:57.233195 nostr_dvm-0.4.8/nostr_dvm/backends/nova_server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/backends/nova_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:37:57.233195 nostr_dvm-0.4.8/nostr_dvm/backends/nova_server/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/backends/nova_server/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:37:57.237195 nostr_dvm-0.4.8/nostr_dvm/backends/nova_server/modules/image_interrogator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/backends/nova_server/modules/image_interrogator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/backends/nova_server/modules/image_interrogator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:37:57.237195 nostr_dvm-0.4.8/nostr_dvm/backends/nova_server/modules/image_upscale/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/backends/nova_server/modules/image_upscale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py
--rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/backends/nova_server/modules/image_upscale/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:37:57.237195 nostr_dvm-0.4.8/nostr_dvm/backends/nova_server/modules/stablediffusionxl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/backends/nova_server/modules/stablediffusionxl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py
--rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/backends/nova_server/modules/stablediffusionxl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:37:57.237195 nostr_dvm-0.4.8/nostr_dvm/backends/nova_server/modules/whisperx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/backends/nova_server/modules/whisperx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/backends/nova_server/modules/whisperx/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/backends/nova_server/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    39902 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)    39789 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/dvm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:37:57.237195 nostr_dvm-0.4.8/nostr_dvm/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/interfaces/dvmtaskinterface.py
--rw-r--r--   0 runner    (1001) docker     (127)    23582 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:37:57.245195 nostr_dvm-0.4.8/nostr_dvm/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/tasks/advanced_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     7452 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/tasks/advanced_search_wine.py
--rw-r--r--   0 runner    (1001) docker     (127)    13185 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/tasks/content_discovery_currently_popular.py
--rw-r--r--   0 runner    (1001) docker     (127)    13703 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/tasks/content_discovery_currently_popular_followers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14107 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/tasks/content_discovery_currently_popular_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/tasks/convert_media.py
--rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/tasks/discovery_bot_farms.py
--rw-r--r--   0 runner    (1001) docker     (127)     8189 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/tasks/discovery_censor_wot.py
--rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/tasks/discovery_inactive_follows.py
--rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/tasks/discovery_nonfollowers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/tasks/discovery_trending_notes_nostrband.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/tasks/imagegeneration_openai_dalle.py
--rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/tasks/imagegeneration_sd21_mlx.py
--rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/tasks/imagegeneration_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/tasks/imageinterrogator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/tasks/imageupscale.py
--rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/tasks/search_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/tasks/summarization_huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/tasks/summarization_unleashed_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/tasks/textextraction_google.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/tasks/textextraction_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/tasks/textextraction_whisperx.py
--rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/tasks/textgeneration_huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/tasks/textgeneration_llmlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/tasks/textgeneration_unleashed_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/tasks/texttospeech.py
--rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/tasks/translation_google.py
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/tasks/translation_libretranslate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/tasks/videogeneration_replicate_svd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/tasks/videogeneration_svd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:37:57.249195 nostr_dvm-0.4.8/nostr_dvm/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/utils/admin_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/utils/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/utils/cashu_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/utils/database_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/utils/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/utils/dvmconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/utils/external_dvm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13406 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/utils/mediasource_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/utils/nip88_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/utils/nip89_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/utils/nostr_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/utils/nwc_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/utils/output_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:37:57.249195 nostr_dvm-0.4.8/nostr_dvm/utils/scrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/utils/scrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26119 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/utils/scrapper/media_scrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/utils/subscription_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15010 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/nostr_dvm/utils/zap_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:37:57.249195 nostr_dvm-0.4.8/nostr_dvm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-25 22:37:57.000000 nostr_dvm-0.4.8/nostr_dvm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-05-25 22:37:57.000000 nostr_dvm-0.4.8/nostr_dvm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 22:37:57.000000 nostr_dvm-0.4.8/nostr_dvm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-25 22:37:57.000000 nostr_dvm-0.4.8/nostr_dvm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-25 22:37:57.000000 nostr_dvm-0.4.8/nostr_dvm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 22:37:57.249195 nostr_dvm-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:37:57.249195 nostr_dvm-0.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    13764 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/tests/test_dvm_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-25 22:37:53.000000 nostr_dvm-0.4.8/tests/test_events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:14:03.665580 nostr_dvm-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-30 08:14:03.665580 nostr_dvm-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:14:03.645579 nostr_dvm-0.4.9/nostr_dvm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:14:03.645579 nostr_dvm-0.4.9/nostr_dvm/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:14:03.645579 nostr_dvm-0.4.9/nostr_dvm/backends/mlx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/backends/mlx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:14:03.645579 nostr_dvm-0.4.9/nostr_dvm/backends/mlx/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/backends/mlx/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:14:03.649579 nostr_dvm-0.4.9/nostr_dvm/backends/mlx/modules/stable_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:14:03.649579 nostr_dvm-0.4.9/nostr_dvm/backends/nova_server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/backends/nova_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:14:03.649579 nostr_dvm-0.4.9/nostr_dvm/backends/nova_server/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/backends/nova_server/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:14:03.649579 nostr_dvm-0.4.9/nostr_dvm/backends/nova_server/modules/image_interrogator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/backends/nova_server/modules/image_interrogator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/backends/nova_server/modules/image_interrogator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:14:03.649579 nostr_dvm-0.4.9/nostr_dvm/backends/nova_server/modules/image_upscale/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/backends/nova_server/modules/image_upscale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/backends/nova_server/modules/image_upscale/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:14:03.653580 nostr_dvm-0.4.9/nostr_dvm/backends/nova_server/modules/stablediffusionxl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/backends/nova_server/modules/stablediffusionxl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/backends/nova_server/modules/stablediffusionxl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:14:03.653580 nostr_dvm-0.4.9/nostr_dvm/backends/nova_server/modules/whisperx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/backends/nova_server/modules/whisperx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/backends/nova_server/modules/whisperx/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/backends/nova_server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39902 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39789 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/dvm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:14:03.653580 nostr_dvm-0.4.9/nostr_dvm/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/interfaces/dvmtaskinterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23582 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:14:03.657580 nostr_dvm-0.4.9/nostr_dvm/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/tasks/advanced_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7452 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/tasks/advanced_search_wine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/tasks/content_discovery_currently_popular.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13936 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/tasks/content_discovery_currently_popular_by_top_zaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13790 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/tasks/content_discovery_currently_popular_followers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13817 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/tasks/content_discovery_currently_popular_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/tasks/convert_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/tasks/discovery_bot_farms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8189 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/tasks/discovery_censor_wot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/tasks/discovery_inactive_follows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/tasks/discovery_nonfollowers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/tasks/discovery_trending_notes_nostrband.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/tasks/imagegeneration_openai_dalle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/tasks/imagegeneration_sd21_mlx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/tasks/imagegeneration_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/tasks/imageinterrogator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/tasks/imageupscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/tasks/search_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/tasks/summarization_huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/tasks/summarization_unleashed_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/tasks/textextraction_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/tasks/textextraction_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/tasks/textextraction_whisperx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/tasks/textgeneration_huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/tasks/textgeneration_llmlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/tasks/textgeneration_unleashed_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/tasks/texttospeech.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/tasks/translation_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/tasks/translation_libretranslate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/tasks/videogeneration_replicate_svd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/tasks/videogeneration_svd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:14:03.661579 nostr_dvm-0.4.9/nostr_dvm/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/utils/admin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/utils/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/utils/cashu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/utils/database_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/utils/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/utils/dvmconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/utils/external_dvm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13406 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/utils/mediasource_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/utils/nip88_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/utils/nip89_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/utils/nostr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/utils/nwc_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/utils/output_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:14:03.661579 nostr_dvm-0.4.9/nostr_dvm/utils/scrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/utils/scrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26119 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/utils/scrapper/media_scrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/utils/subscription_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15010 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/nostr_dvm/utils/zap_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:14:03.661579 nostr_dvm-0.4.9/nostr_dvm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-30 08:14:03.000000 nostr_dvm-0.4.9/nostr_dvm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-05-30 08:14:03.000000 nostr_dvm-0.4.9/nostr_dvm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 08:14:03.000000 nostr_dvm-0.4.9/nostr_dvm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-30 08:14:03.000000 nostr_dvm-0.4.9/nostr_dvm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 08:14:03.000000 nostr_dvm-0.4.9/nostr_dvm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 08:14:03.665580 nostr_dvm-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:14:03.661579 nostr_dvm-0.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13764 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/tests/test_dvm_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-30 08:13:58.000000 nostr_dvm-0.4.9/tests/test_events.py
```

### Comparing `nostr_dvm-0.4.8/LICENSE` & `nostr_dvm-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/PKG-INFO` & `nostr_dvm-0.4.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nostr-dvm
-Version: 0.4.8
+Version: 0.4.9
 Summary: A framework to build and run Nostr NIP90 Data Vending Machines
 Home-page: https://github.com/believethehype/nostrdvm
 Author: Believethehype
 Author-email: believethehypeonnostr@proton.me
 License: MIT
 Keywords: nostr,nip90,dvm,data vending machine
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nostr_dvm-0.4.8/README.md` & `nostr_dvm-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py` & `nostr_dvm-0.4.9/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py` & `nostr_dvm-0.4.9/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py` & `nostr_dvm-0.4.9/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py` & `nostr_dvm-0.4.9/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py` & `nostr_dvm-0.4.9/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py` & `nostr_dvm-0.4.9/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py` & `nostr_dvm-0.4.9/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py` & `nostr_dvm-0.4.9/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py` & `nostr_dvm-0.4.9/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py` & `nostr_dvm-0.4.9/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py` & `nostr_dvm-0.4.9/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py` & `nostr_dvm-0.4.9/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py` & `nostr_dvm-0.4.9/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py` & `nostr_dvm-0.4.9/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py` & `nostr_dvm-0.4.9/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/backends/nova_server/utils.py` & `nostr_dvm-0.4.9/nostr_dvm/backends/nova_server/utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/bot.py` & `nostr_dvm-0.4.9/nostr_dvm/bot.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/dvm.py` & `nostr_dvm-0.4.9/nostr_dvm/dvm.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/interfaces/dvmtaskinterface.py` & `nostr_dvm-0.4.9/nostr_dvm/interfaces/dvmtaskinterface.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/subscription.py` & `nostr_dvm-0.4.9/nostr_dvm/subscription.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/tasks/advanced_search.py` & `nostr_dvm-0.4.9/nostr_dvm/tasks/advanced_search.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/tasks/advanced_search_wine.py` & `nostr_dvm-0.4.9/nostr_dvm/tasks/advanced_search_wine.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/tasks/content_discovery_currently_popular.py` & `nostr_dvm-0.4.9/nostr_dvm/tasks/content_discovery_currently_popular_by_top_zaps.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,32 +8,33 @@
 from nostr_dvm.utils import definitions
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
 from nostr_dvm.utils.nip88_utils import NIP88Config, check_and_set_d_tag_nip88, check_and_set_tiereventid_nip88
 from nostr_dvm.utils.nip89_utils import NIP89Config, check_and_set_d_tag, create_amount_tag
 from nostr_dvm.utils.output_utils import post_process_list_to_events
+from nostr_dvm.utils.zap_utils import parse_zap_event_tags, parse_amount_from_bolt11_invoice
 
 """
-This File contains a Module to discover popular notes
+This File contains a Module to discover popular notes by amount of zaps
 Accepted Inputs: none
 Outputs: A list of events 
 Params:  None
 """
 
 
-class DicoverContentCurrentlyPopular(DVMTaskInterface):
+class DicoverContentCurrentlyPopularZaps(DVMTaskInterface):
     KIND: Kind = EventDefinitions.KIND_NIP90_CONTENT_DISCOVERY
     TASK: str = "discover-content"
     FIX_COST: float = 0
     dvm_config: DVMConfig
     last_schedule: int
     db_since = 3600
     db_name = "db/nostr_recent_notes.db"
-    min_reactions = 2
+    min_reactions = 1
     personalized = False
     result = ""
 
     def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
                  admin_config: AdminConfig = None, options=None):
         dvm_config.SCRIPT = os.path.abspath(__file__)
         super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
@@ -48,15 +49,14 @@
         self.last_schedule = Timestamp.now().as_secs()
 
         if self.options.get("db_name"):
             self.db_name = self.options.get("db_name")
         if self.options.get("db_since"):
             self.db_since = int(self.options.get("db_since"))
 
-
         use_logger = False
         if use_logger:
             init_logger(LogLevel.DEBUG)
 
         if self.dvm_config.UPDATE_DATABASE:
             self.sync_db()
 
@@ -128,20 +128,30 @@
         since = Timestamp.from_secs(timestamp_hour_ago)
 
         filter1 = Filter().kind(definitions.EventDefinitions.KIND_NOTE).since(since)
         events = cli.database().query([filter1])
         ns.finallist = {}
         for event in events:
             if event.created_at().as_secs() > timestamp_hour_ago:
-                filt = Filter().kinds([definitions.EventDefinitions.KIND_ZAP, definitions.EventDefinitions.KIND_REPOST,
-                                       definitions.EventDefinitions.KIND_REACTION,
-                                       definitions.EventDefinitions.KIND_NOTE]).event(event.id()).since(since)
+                filt = Filter().kinds([definitions.EventDefinitions.KIND_ZAP]).event(event.id()).since(since)
                 reactions = cli.database().query([filt])
+                invoice_amount = 0
+                haspreimage = False
                 if len(reactions) >= self.min_reactions:
-                    ns.finallist[event.id().to_hex()] = len(reactions)
+                    for reaction in reactions:
+                        for tag in reaction.tags():
+                            print(tag.as_vec())
+                            if tag.as_vec()[0] == 'bolt11':
+                                print(tag.as_vec()[1])
+                                invoice_amount = parse_amount_from_bolt11_invoice(tag.as_vec()[1])
+                                print(invoice_amount)
+                            if tag.as_vec()[0] == 'preimage':
+                                haspreimage = True # TODO further check preimage
+                    if haspreimage:
+                        ns.finallist[event.id().to_hex()] = invoice_amount
 
         result_list = []
         finallist_sorted = sorted(ns.finallist.items(), key=lambda x: x[1], reverse=True)[:int(options["max_results"])]
         for entry in finallist_sorted:
             # print(EventId.parse(entry[0]).to_bech32() + "/" + EventId.parse(entry[0]).to_hex() + ": " + str(entry[1]))
             e_tag = Tag.parse(["e", entry[0]])
             result_list.append(e_tag.as_vec())
@@ -198,34 +208,36 @@
         print(
             "[" + self.dvm_config.IDENTIFIER + "] Done Syncing Notes of the last " + str(self.db_since) + " seconds..")
 
 
 # We build an example here that we can call by either calling this file directly from the main directory,
 # or by adding it to our playground. You can call the example and adjust it to your needs or redefine it in the
 # playground or elsewhere
-def build_example(name, identifier, admin_config, options,  cost=0, update_rate=180,  processing_msg=None, update_db=True):
+def build_example(name, identifier, admin_config, options, cost=0, update_rate=180, processing_msg=None,
+                  update_db=True):
     dvm_config = build_default_config(identifier)
     dvm_config.USE_OWN_VENV = False
     dvm_config.SHOWLOG = True
     dvm_config.SCHEDULE_UPDATES_SECONDS = update_rate  # Every 10 minutes
     dvm_config.UPDATE_DATABASE = update_db
     # Activate these to use a subscription based model instead
     # dvm_config.SUBSCRIPTION_REQUIRED = True
     # dvm_config.SUBSCRIPTION_DAILY_COST = 1
     dvm_config.FIX_COST = cost
     dvm_config.CUSTOM_PROCESSING_MESSAGE = processing_msg
     admin_config.LUD16 = dvm_config.LN_ADDRESS
 
-
+    image = "https://image.nostr.build/c6879f458252641d04d0aa65fd7f1e005a4f7362fd407467306edc2f4acdb113.jpg",
 
     # Add NIP89
     nip89info = {
         "name": name,
-        "image": "https://image.nostr.build/b29b6ec4bf9b6184f69d33cb44862db0d90a2dd9a506532e7ba5698af7d36210.jpg",
-        "about": "I show notes that are currently popular",
+        "image": image,
+        "picture": image,
+        "about": "I show notes that are currently zapped the most.",
         "lud16": dvm_config.LN_ADDRESS,
         "encryptionSupported": True,
         "cashuAccepted": True,
         "personalized": False,
         "amount": create_amount_tag(cost),
         "nip90Params": {
             "max_results": {
@@ -236,39 +248,40 @@
         }
     }
 
     nip89config = NIP89Config()
     nip89config.DTAG = check_and_set_d_tag(identifier, name, dvm_config.PRIVATE_KEY, nip89info["image"])
     nip89config.CONTENT = json.dumps(nip89info)
 
-    #admin_config.UPDATE_PROFILE = False
-    #admin_config.REBROADCAST_NIP89 = False
+    # admin_config.UPDATE_PROFILE = False
+    # admin_config.REBROADCAST_NIP89 = False
 
-    return DicoverContentCurrentlyPopular(name=name, dvm_config=dvm_config, nip89config=nip89config,
-                                          admin_config=admin_config, options=options)
+    return DicoverContentCurrentlyPopularZaps(name=name, dvm_config=dvm_config, nip89config=nip89config,
+                                              admin_config=admin_config, options=options)
 
 
-def build_example_subscription(name, identifier, admin_config, options, update_rate=180, processing_msg=None, update_db=True):
+def build_example_subscription(name, identifier, admin_config, options, update_rate=180, processing_msg=None,
+                               update_db=True):
     dvm_config = build_default_config(identifier)
     dvm_config.USE_OWN_VENV = False
     dvm_config.SHOWLOG = True
     dvm_config.SCHEDULE_UPDATES_SECONDS = update_rate  # Every 3 minutes
     dvm_config.UPDATE_DATABASE = update_db
     # Activate these to use a subscription based model instead
     # dvm_config.SUBSCRIPTION_DAILY_COST = 1
     dvm_config.FIX_COST = 0
     dvm_config.CUSTOM_PROCESSING_MESSAGE = processing_msg
     admin_config.LUD16 = dvm_config.LN_ADDRESS
 
-
-
+    image = "https://image.nostr.build/c6879f458252641d04d0aa65fd7f1e005a4f7362fd407467306edc2f4acdb113.jpg",
     # Add NIP89
     nip89info = {
         "name": name,
-        "image": "https://image.nostr.build/b29b6ec4bf9b6184f69d33cb44862db0d90a2dd9a506532e7ba5698af7d36210.jpg",
+        "image": image,
+        "picture": image,
         "about": "I show notes that are currently popular all over Nostr. I'm also used for testing subscriptions.",
         "lud16": dvm_config.LN_ADDRESS,
         "encryptionSupported": True,
         "cashuAccepted": True,
         "subscription": True,
         "personalized": False,
         "nip90Params": {
@@ -293,22 +306,22 @@
     nip88config.AMOUNT_DAILY = 100
     nip88config.AMOUNT_MONTHLY = 2000
     nip88config.CONTENT = "Subscribe to the DVM for unlimited use during your subscription"
     nip88config.PERK1DESC = "Unlimited requests"
     nip88config.PERK2DESC = "Support NostrDVM & NostrSDK development"
     nip88config.PAYMENT_VERIFIER_PUBKEY = "5b5c045ecdf66fb540bdf2049fe0ef7f1a566fa427a4fe50d400a011b65a3a7e"
 
-    #admin_config.UPDATE_PROFILE = False
-    #admin_config.REBROADCAST_NIP89 = False
-    #admin_config.REBROADCAST_NIP88 = False
+    # admin_config.UPDATE_PROFILE = False
+    # admin_config.REBROADCAST_NIP89 = False
+    # admin_config.REBROADCAST_NIP88 = False
 
     # admin_config.FETCH_NIP88 = True
     # admin_config.EVENTID = ""
     # admin_config.PRIVKEY = dvm_config.PRIVATE_KEY
 
-    return DicoverContentCurrentlyPopular(name=name, dvm_config=dvm_config, nip89config=nip89config,
-                                          nip88config=nip88config, options=options,
-                                          admin_config=admin_config)
+    return DicoverContentCurrentlyPopularZaps(name=name, dvm_config=dvm_config, nip89config=nip89config,
+                                              nip88config=nip88config, options=options,
+                                              admin_config=admin_config)
 
 
 if __name__ == '__main__':
-    process_venv(DicoverContentCurrentlyPopular)
+    process_venv(DicoverContentCurrentlyPopularZaps)
```

### Comparing `nostr_dvm-0.4.8/nostr_dvm/tasks/content_discovery_currently_popular_followers.py` & `nostr_dvm-0.4.9/nostr_dvm/tasks/content_discovery_currently_popular_followers.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,19 +227,20 @@
     # Activate these to use a subscription based model instead
     # dvm_config.SUBSCRIPTION_REQUIRED = True
     # dvm_config.SUBSCRIPTION_DAILY_COST = 1
     dvm_config.FIX_COST = cost
     dvm_config.CUSTOM_PROCESSING_MESSAGE = processing_msg
     admin_config.LUD16 = dvm_config.LN_ADDRESS
 
-
+    image = "https://image.nostr.build/d92652a6a07677e051d647dcf9f0f59e265299b3335a939d008183a911513f4a.jpg"
     # Add NIP89
     nip89info = {
         "name": name,
-        "image": "https://image.nostr.build/d92652a6a07677e051d647dcf9f0f59e265299b3335a939d008183a911513f4a.jpg",
+        "image": image,
+        "picture": image,
         "about": "I show notes that are currently popular from people you follow",
         "lud16": dvm_config.LN_ADDRESS,
         "encryptionSupported": True,
         "cashuAccepted": True,
         "personalized": True,
         "amount": create_amount_tag(cost),
         "nip90Params": {
@@ -270,17 +271,19 @@
     dvm_config.UPDATE_DATABASE = update_db
     # Activate these to use a subscription based model instead
     # dvm_config.SUBSCRIPTION_DAILY_COST = 1
     dvm_config.FIX_COST = 0
     dvm_config.CUSTOM_PROCESSING_MESSAGE = processing_msg
 
     # Add NIP89
+    image = "https://image.nostr.build/d92652a6a07677e051d647dcf9f0f59e265299b3335a939d008183a911513f4a.jpg"
     nip89info = {
         "name": name,
-        "image": "https://image.nostr.build/b29b6ec4bf9b6184f69d33cb44862db0d90a2dd9a506532e7ba5698af7d36210.jpg",
+        "image": image,
+        "picture": image,
         "about": "I show notes that are currently popular, just like the free DVM, I'm also used for testing subscriptions. (beta)",
         "lud16": dvm_config.LN_ADDRESS,
         "encryptionSupported": True,
         "cashuAccepted": True,
         "personalized": True,
         "subscription": True,
         "nip90Params": {
```

### Comparing `nostr_dvm-0.4.8/nostr_dvm/tasks/content_discovery_currently_popular_topic.py` & `nostr_dvm-0.4.9/nostr_dvm/tasks/content_discovery_currently_popular_topic.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
 from nostr_dvm.utils.nip88_utils import NIP88Config, check_and_set_d_tag_nip88, check_and_set_tiereventid_nip88
 from nostr_dvm.utils.nip89_utils import NIP89Config, check_and_set_d_tag, create_amount_tag
 from nostr_dvm.utils.output_utils import post_process_list_to_events
 
 """
-This File contains a Module to discover popular notes
+This File contains a Module to discover popular notes by topic
 Accepted Inputs: none
 Outputs: A list of events 
 Params:  None
 """
 
 
 class DicoverContentCurrentlyPopularbyTopic(DVMTaskInterface):
@@ -205,18 +205,15 @@
         cli.add_relay("wss://relay.damus.io")
         cli.add_relay("wss://nostr.oxtr.dev")
         cli.add_relay("wss://relay.nostr.net")
         cli.add_relay("wss://relay.nostr.bg")
         cli.add_relay("wss://nostr.wine")
         cli.add_relay("wss://nostr21.com")
 
-        #RELAY_LIST = [ "wss://nostr.wine",
-        #              , "wss://relay.nostr.bg",
-        #              , "wss://relay.nostr.net"
-        #              ]
+
         cli.connect()
 
         timestamp_since = Timestamp.now().as_secs() - self.db_since
         since = Timestamp.from_secs(timestamp_since)
 
         filter1 = Filter().kinds([definitions.EventDefinitions.KIND_NOTE, definitions.EventDefinitions.KIND_REACTION, definitions.EventDefinitions.KIND_ZAP]).since(since)  # Notes, reactions, zaps
 
@@ -247,14 +244,15 @@
     admin_config.LUD16 = dvm_config.LN_ADDRESS
 
 
     # Add NIP89
     nip89info = {
         "name": name,
         "image": image,
+        "picture": image,
         "about": description,
         "lud16": dvm_config.LN_ADDRESS,
         "encryptionSupported": True,
         "cashuAccepted": True,
         "personalized": False,
         "amount": create_amount_tag(cost),
         "nip90Params": {
@@ -286,14 +284,15 @@
     admin_config.LUD16 = dvm_config.LN_ADDRESS
 
 
     # Add NIP89
     nip89info = {
         "name": name,
         "image": image,
+        "picture": image,
         "about": description,
         "lud16": dvm_config.LN_ADDRESS,
         "encryptionSupported": True,
         "cashuAccepted": True,
         "subscription": True,
         "personalized": False,
         "nip90Params": {
@@ -319,19 +318,14 @@
     nip88config.AMOUNT_MONTHLY = 2000
     nip88config.CONTENT = "Subscribe to the DVM for unlimited use during your subscription"
     nip88config.PERK1DESC = "Unlimited requests"
     nip88config.PERK2DESC = "Support NostrDVM & NostrSDK development"
     nip88config.PAYMENT_VERIFIER_PUBKEY = "5b5c045ecdf66fb540bdf2049fe0ef7f1a566fa427a4fe50d400a011b65a3a7e"
 
 
-   # admin_config.FETCH_NIP88 = True
-   # admin_config.EVENTID = "63a791cdc7bf78c14031616963105fce5793f532bb231687665b14fb6d805fdb"
-   # admin_config.PRIVKEY = dvm_config.PRIVATE_KEY
-
-
     return DicoverContentCurrentlyPopularbyTopic(name=name, dvm_config=dvm_config, nip89config=nip89config,
                                           nip88config=nip88config,
                                           admin_config=admin_config,
                                           options=options)
 
 
 if __name__ == '__main__':
```

### Comparing `nostr_dvm-0.4.8/nostr_dvm/tasks/convert_media.py` & `nostr_dvm-0.4.9/nostr_dvm/tasks/convert_media.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/tasks/discovery_bot_farms.py` & `nostr_dvm-0.4.9/nostr_dvm/tasks/discovery_bot_farms.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/tasks/discovery_censor_wot.py` & `nostr_dvm-0.4.9/nostr_dvm/tasks/discovery_censor_wot.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/tasks/discovery_inactive_follows.py` & `nostr_dvm-0.4.9/nostr_dvm/tasks/discovery_inactive_follows.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/tasks/discovery_nonfollowers.py` & `nostr_dvm-0.4.9/nostr_dvm/tasks/discovery_nonfollowers.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/tasks/discovery_trending_notes_nostrband.py` & `nostr_dvm-0.4.9/nostr_dvm/tasks/discovery_trending_notes_nostrband.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,14 @@
                 input_type = tag.as_vec()[2]
                 if input_type != "text":
                     return False
         return True
 
     def create_request_from_nostr_event(self, event, client=None, dvm_config=None):
         self.dvm_config = dvm_config
-        print(self.dvm_config.PRIVATE_KEY)
 
         request_form = {"jobID": event.id().to_hex()}
         max_results = 200
 
         for tag in event.tags():
             if tag.as_vec()[0] == 'i':
                 input_type = tag.as_vec()[2]
@@ -108,14 +107,15 @@
     dvm_config.CUSTOM_PROCESSING_MESSAGE = custom_processing_msg
     admin_config.LUD16 = dvm_config.LN_ADDRESS
     # Add NIP89
 
     nip89info = {
         "name": name,
         "image": "https://nostr.band/android-chrome-192x192.png",
+        "picture": "https://nostr.band/android-chrome-192x192.png",
         "about": "I show trending notes from nostr.band",
         "amount": "Free",
         "encryptionSupported": True,
         "cashuAccepted": True,
         "nip90Params": {}
     }
     nip89config = NIP89Config()
```

### Comparing `nostr_dvm-0.4.8/nostr_dvm/tasks/imagegeneration_openai_dalle.py` & `nostr_dvm-0.4.9/nostr_dvm/tasks/imagegeneration_openai_dalle.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py` & `nostr_dvm-0.4.9/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/tasks/imagegeneration_sd21_mlx.py` & `nostr_dvm-0.4.9/nostr_dvm/tasks/imagegeneration_sd21_mlx.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/tasks/imagegeneration_sdxl.py` & `nostr_dvm-0.4.9/nostr_dvm/tasks/imagegeneration_sdxl.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py` & `nostr_dvm-0.4.9/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/tasks/imageinterrogator.py` & `nostr_dvm-0.4.9/nostr_dvm/tasks/imageinterrogator.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/tasks/imageupscale.py` & `nostr_dvm-0.4.9/nostr_dvm/tasks/imageupscale.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/tasks/search_users.py` & `nostr_dvm-0.4.9/nostr_dvm/tasks/search_users.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/tasks/summarization_huggingchat.py` & `nostr_dvm-0.4.9/nostr_dvm/tasks/summarization_huggingchat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/tasks/summarization_unleashed_chat.py` & `nostr_dvm-0.4.9/nostr_dvm/tasks/summarization_unleashed_chat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/tasks/textextraction_google.py` & `nostr_dvm-0.4.9/nostr_dvm/tasks/textextraction_google.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/tasks/textextraction_pdf.py` & `nostr_dvm-0.4.9/nostr_dvm/tasks/textextraction_pdf.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/tasks/textextraction_whisperx.py` & `nostr_dvm-0.4.9/nostr_dvm/tasks/textextraction_whisperx.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/tasks/textgeneration_huggingchat.py` & `nostr_dvm-0.4.9/nostr_dvm/tasks/textgeneration_huggingchat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/tasks/textgeneration_llmlite.py` & `nostr_dvm-0.4.9/nostr_dvm/tasks/textgeneration_llmlite.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/tasks/textgeneration_unleashed_chat.py` & `nostr_dvm-0.4.9/nostr_dvm/tasks/textgeneration_unleashed_chat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/tasks/texttospeech.py` & `nostr_dvm-0.4.9/nostr_dvm/tasks/texttospeech.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/tasks/translation_google.py` & `nostr_dvm-0.4.9/nostr_dvm/tasks/translation_google.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/tasks/translation_libretranslate.py` & `nostr_dvm-0.4.9/nostr_dvm/tasks/translation_libretranslate.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/tasks/videogeneration_replicate_svd.py` & `nostr_dvm-0.4.9/nostr_dvm/tasks/videogeneration_replicate_svd.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/tasks/videogeneration_svd.py` & `nostr_dvm-0.4.9/nostr_dvm/tasks/videogeneration_svd.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/utils/admin_utils.py` & `nostr_dvm-0.4.9/nostr_dvm/utils/admin_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     UNWHITELISTUSER: bool = False
     BLACKLISTUSER: bool = False
     DELETEUSER: bool = False
     LISTDATABASE: bool = False
     ClEANDB: bool = False
     POW: bool = False
     INDEX: str = "1"
+    LUD16: str = ""
 
     USERNPUBS: list = []
 
     EVENTID: str = ""
     PRIVKEY: str = ""
```

### Comparing `nostr_dvm-0.4.8/nostr_dvm/utils/backend_utils.py` & `nostr_dvm-0.4.9/nostr_dvm/utils/backend_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/utils/cashu_utils.py` & `nostr_dvm-0.4.9/nostr_dvm/utils/cashu_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/utils/database_utils.py` & `nostr_dvm-0.4.9/nostr_dvm/utils/database_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/utils/definitions.py` & `nostr_dvm-0.4.9/nostr_dvm/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/utils/dvmconfig.py` & `nostr_dvm-0.4.9/nostr_dvm/utils/dvmconfig.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/utils/external_dvm_utils.py` & `nostr_dvm-0.4.9/nostr_dvm/utils/external_dvm_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/utils/mediasource_utils.py` & `nostr_dvm-0.4.9/nostr_dvm/utils/mediasource_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/utils/nip88_utils.py` & `nostr_dvm-0.4.9/nostr_dvm/utils/nip88_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/utils/nip89_utils.py` & `nostr_dvm-0.4.9/nostr_dvm/utils/nip89_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/utils/nostr_utils.py` & `nostr_dvm-0.4.9/nostr_dvm/utils/nostr_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/utils/nwc_tools.py` & `nostr_dvm-0.4.9/nostr_dvm/utils/nwc_tools.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/utils/output_utils.py` & `nostr_dvm-0.4.9/nostr_dvm/utils/output_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/utils/scrapper/media_scrapper.py` & `nostr_dvm-0.4.9/nostr_dvm/utils/scrapper/media_scrapper.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/utils/subscription_utils.py` & `nostr_dvm-0.4.9/nostr_dvm/utils/subscription_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm/utils/zap_utils.py` & `nostr_dvm-0.4.9/nostr_dvm/utils/zap_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/nostr_dvm.egg-info/PKG-INFO` & `nostr_dvm-0.4.9/nostr_dvm.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nostr-dvm
-Version: 0.4.8
+Version: 0.4.9
 Summary: A framework to build and run Nostr NIP90 Data Vending Machines
 Home-page: https://github.com/believethehype/nostrdvm
 Author: Believethehype
 Author-email: believethehypeonnostr@proton.me
 License: MIT
 Keywords: nostr,nip90,dvm,data vending machine
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nostr_dvm-0.4.8/nostr_dvm.egg-info/SOURCES.txt` & `nostr_dvm-0.4.9/nostr_dvm.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py
 nostr_dvm/interfaces/__init__.py
 nostr_dvm/interfaces/dvmtaskinterface.py
 nostr_dvm/tasks/__init__.py
 nostr_dvm/tasks/advanced_search.py
 nostr_dvm/tasks/advanced_search_wine.py
 nostr_dvm/tasks/content_discovery_currently_popular.py
+nostr_dvm/tasks/content_discovery_currently_popular_by_top_zaps.py
 nostr_dvm/tasks/content_discovery_currently_popular_followers.py
 nostr_dvm/tasks/content_discovery_currently_popular_topic.py
 nostr_dvm/tasks/convert_media.py
 nostr_dvm/tasks/discovery_bot_farms.py
 nostr_dvm/tasks/discovery_censor_wot.py
 nostr_dvm/tasks/discovery_inactive_follows.py
 nostr_dvm/tasks/discovery_nonfollowers.py
```

### Comparing `nostr_dvm-0.4.8/setup.py` & `nostr_dvm-0.4.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.4.8'
+VERSION = '0.4.9'
 DESCRIPTION = 'A framework to build and run Nostr NIP90 Data Vending Machines'
 LONG_DESCRIPTION = ('A framework to build and run Nostr NIP90 Data Vending Machines. See the github repository for more information')
 
 # Setting up
 setup(
     name="nostr-dvm",
     version=VERSION,
```

### Comparing `nostr_dvm-0.4.8/tests/test_dvm_client.py` & `nostr_dvm-0.4.9/tests/test_dvm_client.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.4.8/tests/test_events.py` & `nostr_dvm-0.4.9/tests/test_events.py`

 * *Files identical despite different names*

