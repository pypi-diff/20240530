# Comparing `tmp/webscout-2.9.tar.gz` & `tmp/webscout-3.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscout-2.9.tar", last modified: Sun May 26 12:43:50 2024, max compression
+gzip compressed data, was "webscout-3.0b0.tar", last modified: Thu May 30 06:49:41 2024, max compression
```

## Comparing `webscout-2.9.tar` & `webscout-3.0b0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 12:43:50.638272 webscout-2.9/
-drwxrwxrwx   0        0        0        0 2024-05-26 12:43:50.149661 webscout-2.9/DeepWEBS/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.9/DeepWEBS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 12:43:50.165669 webscout-2.9/DeepWEBS/documents/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.9/DeepWEBS/documents/__init__.py
--rw-rw-rw-   0        0        0     4049 2024-05-08 15:52:48.000000 webscout-2.9/DeepWEBS/documents/query_results_extractor.py
--rw-rw-rw-   0        0        0     5272 2024-05-08 15:52:48.000000 webscout-2.9/DeepWEBS/documents/webpage_content_extractor.py
-drwxrwxrwx   0        0        0        0 2024-05-26 12:43:50.191663 webscout-2.9/DeepWEBS/networks/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.9/DeepWEBS/networks/__init__.py
--rw-rw-rw-   0        0        0     3183 2024-05-08 15:52:48.000000 webscout-2.9/DeepWEBS/networks/filepath_converter.py
--rw-rw-rw-   0        0        0     1966 2024-05-08 15:52:48.000000 webscout-2.9/DeepWEBS/networks/google_searcher.py
--rw-rw-rw-   0        0        0      726 2024-05-08 15:52:48.000000 webscout-2.9/DeepWEBS/networks/network_configs.py
--rw-rw-rw-   0        0        0     3590 2024-05-08 15:52:48.000000 webscout-2.9/DeepWEBS/networks/webpage_fetcher.py
-drwxrwxrwx   0        0        0        0 2024-05-26 12:43:50.215361 webscout-2.9/DeepWEBS/utilsdw/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.9/DeepWEBS/utilsdw/__init__.py
--rw-rw-rw-   0        0        0     2472 2024-05-08 15:52:48.000000 webscout-2.9/DeepWEBS/utilsdw/enver.py
--rw-rw-rw-   0        0        0     8174 2024-05-08 15:52:48.000000 webscout-2.9/DeepWEBS/utilsdw/logger.py
--rw-rw-rw-   0        0        0     3150 2024-05-08 15:52:48.000000 webscout-2.9/LICENSE.md
--rw-rw-rw-   0        0        0    47775 2024-05-26 12:43:50.633263 webscout-2.9/PKG-INFO
--rw-rw-rw-   0        0        0    45203 2024-05-19 15:11:59.000000 webscout-2.9/README.md
--rw-rw-rw-   0        0        0       42 2024-05-26 12:43:50.638272 webscout-2.9/setup.cfg
--rw-rw-rw-   0        0        0     2816 2024-05-26 12:42:47.000000 webscout-2.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 12:43:50.398174 webscout-2.9/webscout/
--rw-rw-rw-   0        0        0    18246 2024-05-12 12:54:03.000000 webscout-2.9/webscout/AIauto.py
--rw-rw-rw-   0        0        0     4710 2024-05-08 15:52:48.000000 webscout-2.9/webscout/AIbase.py
--rw-rw-rw-   0        0        0    33256 2024-05-14 14:10:47.000000 webscout-2.9/webscout/AIutel.py
--rw-rw-rw-   0        0        0     7332 2024-05-08 15:52:48.000000 webscout-2.9/webscout/DWEBS.py
--rw-rw-rw-   0        0        0     4184 2024-05-19 17:29:05.000000 webscout-2.9/webscout/LLM.py
-drwxrwxrwx   0        0        0        0 2024-05-26 12:43:50.467443 webscout-2.9/webscout/Local/
--rw-rw-rw-   0        0        0      217 2024-05-14 07:50:22.000000 webscout-2.9/webscout/Local/__init__.py
--rw-rw-rw-   0        0        0       83 2024-05-26 12:42:35.000000 webscout-2.9/webscout/Local/_version.py
--rw-rw-rw-   0        0        0    18994 2024-05-19 14:40:00.000000 webscout-2.9/webscout/Local/formats.py
--rw-rw-rw-   0        0        0    27618 2024-05-19 14:42:26.000000 webscout-2.9/webscout/Local/model.py
--rw-rw-rw-   0        0        0     4372 2024-05-13 10:22:16.000000 webscout-2.9/webscout/Local/samplers.py
--rw-rw-rw-   0        0        0    26925 2024-05-19 14:44:26.000000 webscout-2.9/webscout/Local/thread.py
--rw-rw-rw-   0        0        0     6197 2024-05-26 12:41:46.000000 webscout-2.9/webscout/Local/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-26 12:43:50.612276 webscout-2.9/webscout/Provider/
--rw-rw-rw-   0        0        0     8191 2024-05-16 04:06:55.000000 webscout-2.9/webscout/Provider/BasedGPT.py
--rw-rw-rw-   0        0        0     8342 2024-05-12 04:47:12.000000 webscout-2.9/webscout/Provider/Berlin4h.py
--rw-rw-rw-   0        0        0    16743 2024-05-11 08:19:16.000000 webscout-2.9/webscout/Provider/Blackboxai.py
--rw-rw-rw-   0        0        0     8357 2024-05-12 05:14:27.000000 webscout-2.9/webscout/Provider/ChatGPTUK.py
--rw-rw-rw-   0        0        0     8489 2024-05-11 08:19:31.000000 webscout-2.9/webscout/Provider/Cohere.py
--rw-rw-rw-   0        0        0     8235 2024-05-11 08:19:44.000000 webscout-2.9/webscout/Provider/Gemini.py
--rw-rw-rw-   0        0        0    20583 2024-05-11 08:19:52.000000 webscout-2.9/webscout/Provider/Groq.py
--rw-rw-rw-   0        0        0    15405 2024-05-11 08:20:01.000000 webscout-2.9/webscout/Provider/Koboldai.py
--rw-rw-rw-   0        0        0    19519 2024-05-11 08:20:16.000000 webscout-2.9/webscout/Provider/Leo.py
--rw-rw-rw-   0        0        0    17089 2024-05-11 08:20:22.000000 webscout-2.9/webscout/Provider/Llama2.py
--rw-rw-rw-   0        0        0    18404 2024-05-11 08:20:30.000000 webscout-2.9/webscout/Provider/OpenGPT.py
--rw-rw-rw-   0        0        0    20107 2024-05-11 08:20:26.000000 webscout-2.9/webscout/Provider/Openai.py
--rw-rw-rw-   0        0        0     8597 2024-05-11 08:20:36.000000 webscout-2.9/webscout/Provider/Perplexity.py
--rw-rw-rw-   0        0        0    19390 2024-05-11 08:20:42.000000 webscout-2.9/webscout/Provider/Phind.py
--rw-rw-rw-   0        0        0     7303 2024-05-14 14:08:46.000000 webscout-2.9/webscout/Provider/Poe.py
--rw-rw-rw-   0        0        0     8692 2024-05-11 08:20:50.000000 webscout-2.9/webscout/Provider/Reka.py
--rw-rw-rw-   0        0        0    11616 2024-05-11 08:20:56.000000 webscout-2.9/webscout/Provider/ThinkAnyAI.py
--rw-rw-rw-   0        0        0     8809 2024-05-11 08:21:00.000000 webscout-2.9/webscout/Provider/Xjai.py
--rw-rw-rw-   0        0        0    19398 2024-05-11 08:21:06.000000 webscout-2.9/webscout/Provider/Yepchat.py
--rw-rw-rw-   0        0        0     7756 2024-05-21 13:54:46.000000 webscout-2.9/webscout/Provider/Youchat.py
--rw-rw-rw-   0        0        0     1372 2024-05-16 04:09:11.000000 webscout-2.9/webscout/Provider/__init__.py
--rw-rw-rw-   0        0        0     1840 2024-05-19 14:59:15.000000 webscout-2.9/webscout/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-08 15:52:48.000000 webscout-2.9/webscout/__main__.py
--rw-rw-rw-   0        0        0      684 2024-05-12 11:18:43.000000 webscout-2.9/webscout/async_providers.py
--rw-rw-rw-   0        0        0    18743 2024-05-19 12:59:44.000000 webscout-2.9/webscout/cli.py
--rw-rw-rw-   0        0        0      498 2024-05-10 14:34:10.000000 webscout-2.9/webscout/exceptions.py
--rw-rw-rw-   0        0        0    24487 2024-05-12 13:39:37.000000 webscout-2.9/webscout/g4f.py
--rw-rw-rw-   0        0        0      692 2024-05-08 15:52:48.000000 webscout-2.9/webscout/models.py
--rw-rw-rw-   0        0        0     5896 2024-05-08 15:52:48.000000 webscout-2.9/webscout/tempid.py
--rw-rw-rw-   0        0        0    20622 2024-05-08 15:52:48.000000 webscout-2.9/webscout/transcriber.py
--rw-rw-rw-   0        0        0     2603 2024-05-09 03:33:11.000000 webscout-2.9/webscout/utils.py
--rw-rw-rw-   0        0        0       23 2024-05-26 12:42:41.000000 webscout-2.9/webscout/version.py
--rw-rw-rw-   0        0        0      967 2024-05-08 15:52:48.000000 webscout-2.9/webscout/voice.py
--rw-rw-rw-   0        0        0    85324 2024-05-14 14:12:32.000000 webscout-2.9/webscout/webai.py
--rw-rw-rw-   0        0        0    42650 2024-05-19 13:03:19.000000 webscout-2.9/webscout/webscout_search.py
--rw-rw-rw-   0        0        0    14471 2024-05-19 13:04:35.000000 webscout-2.9/webscout/webscout_search_async.py
-drwxrwxrwx   0        0        0        0 2024-05-26 12:43:50.622278 webscout-2.9/webscout.egg-info/
--rw-rw-rw-   0        0        0    47775 2024-05-26 12:43:49.000000 webscout-2.9/webscout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1827 2024-05-26 12:43:49.000000 webscout-2.9/webscout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 12:43:49.000000 webscout-2.9/webscout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-05-26 12:43:49.000000 webscout-2.9/webscout.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      433 2024-05-26 12:43:49.000000 webscout-2.9/webscout.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-26 12:43:49.000000 webscout-2.9/webscout.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 06:49:41.265169 webscout-3.0b0/
+drwxrwxrwx   0        0        0        0 2024-05-30 06:49:39.148168 webscout-3.0b0/DeepWEBS/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-3.0b0/DeepWEBS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:49:39.182165 webscout-3.0b0/DeepWEBS/documents/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-3.0b0/DeepWEBS/documents/__init__.py
+-rw-rw-rw-   0        0        0     4049 2024-05-08 15:52:48.000000 webscout-3.0b0/DeepWEBS/documents/query_results_extractor.py
+-rw-rw-rw-   0        0        0     5272 2024-05-08 15:52:48.000000 webscout-3.0b0/DeepWEBS/documents/webpage_content_extractor.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:49:39.231167 webscout-3.0b0/DeepWEBS/networks/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-3.0b0/DeepWEBS/networks/__init__.py
+-rw-rw-rw-   0        0        0     3183 2024-05-08 15:52:48.000000 webscout-3.0b0/DeepWEBS/networks/filepath_converter.py
+-rw-rw-rw-   0        0        0     1966 2024-05-08 15:52:48.000000 webscout-3.0b0/DeepWEBS/networks/google_searcher.py
+-rw-rw-rw-   0        0        0      726 2024-05-08 15:52:48.000000 webscout-3.0b0/DeepWEBS/networks/network_configs.py
+-rw-rw-rw-   0        0        0     3590 2024-05-08 15:52:48.000000 webscout-3.0b0/DeepWEBS/networks/webpage_fetcher.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:49:39.283155 webscout-3.0b0/DeepWEBS/utilsdw/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-3.0b0/DeepWEBS/utilsdw/__init__.py
+-rw-rw-rw-   0        0        0     2472 2024-05-08 15:52:48.000000 webscout-3.0b0/DeepWEBS/utilsdw/enver.py
+-rw-rw-rw-   0        0        0     8174 2024-05-08 15:52:48.000000 webscout-3.0b0/DeepWEBS/utilsdw/logger.py
+-rw-rw-rw-   0        0        0     3150 2024-05-08 15:52:48.000000 webscout-3.0b0/LICENSE.md
+-rw-rw-rw-   0        0        0    47777 2024-05-30 06:49:41.259353 webscout-3.0b0/PKG-INFO
+-rw-rw-rw-   0        0        0    45203 2024-05-19 15:11:59.000000 webscout-3.0b0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-30 06:49:41.265169 webscout-3.0b0/setup.cfg
+-rw-rw-rw-   0        0        0     2821 2024-05-30 06:44:43.000000 webscout-3.0b0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:49:40.102566 webscout-3.0b0/webscout/
+-rw-rw-rw-   0        0        0    18246 2024-05-12 12:54:03.000000 webscout-3.0b0/webscout/AIauto.py
+-rw-rw-rw-   0        0        0     4710 2024-05-08 15:52:48.000000 webscout-3.0b0/webscout/AIbase.py
+-rw-rw-rw-   0        0        0    33272 2024-05-27 06:28:40.000000 webscout-3.0b0/webscout/AIutel.py
+-rw-rw-rw-   0        0        0     7332 2024-05-08 15:52:48.000000 webscout-3.0b0/webscout/DWEBS.py
+-rw-rw-rw-   0        0        0     4184 2024-05-19 17:29:05.000000 webscout-3.0b0/webscout/LLM.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:49:40.643324 webscout-3.0b0/webscout/Local/
+-rw-rw-rw-   0        0        0      217 2024-05-14 07:50:22.000000 webscout-3.0b0/webscout/Local/__init__.py
+-rw-rw-rw-   0        0        0       83 2024-05-26 12:42:35.000000 webscout-3.0b0/webscout/Local/_version.py
+-rw-rw-rw-   0        0        0    18994 2024-05-30 06:36:15.000000 webscout-3.0b0/webscout/Local/formats.py
+-rw-rw-rw-   0        0        0    30463 2024-05-30 06:26:30.000000 webscout-3.0b0/webscout/Local/model.py
+-rw-rw-rw-   0        0        0     4372 2024-05-13 10:22:16.000000 webscout-3.0b0/webscout/Local/samplers.py
+-rw-rw-rw-   0        0        0    27453 2024-05-30 06:39:51.000000 webscout-3.0b0/webscout/Local/thread.py
+-rw-rw-rw-   0        0        0     6197 2024-05-26 12:41:46.000000 webscout-3.0b0/webscout/Local/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:49:41.247290 webscout-3.0b0/webscout/Provider/
+-rw-rw-rw-   0        0        0     8191 2024-05-16 04:06:55.000000 webscout-3.0b0/webscout/Provider/BasedGPT.py
+-rw-rw-rw-   0        0        0     8342 2024-05-12 04:47:12.000000 webscout-3.0b0/webscout/Provider/Berlin4h.py
+-rw-rw-rw-   0        0        0    16743 2024-05-11 08:19:16.000000 webscout-3.0b0/webscout/Provider/Blackboxai.py
+-rw-rw-rw-   0        0        0     8357 2024-05-12 05:14:27.000000 webscout-3.0b0/webscout/Provider/ChatGPTUK.py
+-rw-rw-rw-   0        0        0     8489 2024-05-11 08:19:31.000000 webscout-3.0b0/webscout/Provider/Cohere.py
+-rw-rw-rw-   0        0        0     8235 2024-05-11 08:19:44.000000 webscout-3.0b0/webscout/Provider/Gemini.py
+-rw-rw-rw-   0        0        0    20583 2024-05-11 08:19:52.000000 webscout-3.0b0/webscout/Provider/Groq.py
+-rw-rw-rw-   0        0        0    15405 2024-05-11 08:20:01.000000 webscout-3.0b0/webscout/Provider/Koboldai.py
+-rw-rw-rw-   0        0        0    19519 2024-05-11 08:20:16.000000 webscout-3.0b0/webscout/Provider/Leo.py
+-rw-rw-rw-   0        0        0    17089 2024-05-11 08:20:22.000000 webscout-3.0b0/webscout/Provider/Llama2.py
+-rw-rw-rw-   0        0        0    18404 2024-05-11 08:20:30.000000 webscout-3.0b0/webscout/Provider/OpenGPT.py
+-rw-rw-rw-   0        0        0    20107 2024-05-11 08:20:26.000000 webscout-3.0b0/webscout/Provider/Openai.py
+-rw-rw-rw-   0        0        0     8597 2024-05-11 08:20:36.000000 webscout-3.0b0/webscout/Provider/Perplexity.py
+-rw-rw-rw-   0        0        0    19390 2024-05-11 08:20:42.000000 webscout-3.0b0/webscout/Provider/Phind.py
+-rw-rw-rw-   0        0        0     7303 2024-05-14 14:08:46.000000 webscout-3.0b0/webscout/Provider/Poe.py
+-rw-rw-rw-   0        0        0     8692 2024-05-11 08:20:50.000000 webscout-3.0b0/webscout/Provider/Reka.py
+-rw-rw-rw-   0        0        0    11616 2024-05-11 08:20:56.000000 webscout-3.0b0/webscout/Provider/ThinkAnyAI.py
+-rw-rw-rw-   0        0        0     8809 2024-05-11 08:21:00.000000 webscout-3.0b0/webscout/Provider/Xjai.py
+-rw-rw-rw-   0        0        0    19398 2024-05-11 08:21:06.000000 webscout-3.0b0/webscout/Provider/Yepchat.py
+-rw-rw-rw-   0        0        0     7756 2024-05-21 13:54:46.000000 webscout-3.0b0/webscout/Provider/Youchat.py
+-rw-rw-rw-   0        0        0     1396 2024-05-27 06:27:55.000000 webscout-3.0b0/webscout/Provider/__init__.py
+-rw-rw-rw-   0        0        0     1856 2024-05-27 06:28:13.000000 webscout-3.0b0/webscout/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-08 15:52:48.000000 webscout-3.0b0/webscout/__main__.py
+-rw-rw-rw-   0        0        0      684 2024-05-12 11:18:43.000000 webscout-3.0b0/webscout/async_providers.py
+-rw-rw-rw-   0        0        0    18743 2024-05-19 12:59:44.000000 webscout-3.0b0/webscout/cli.py
+-rw-rw-rw-   0        0        0      498 2024-05-10 14:34:10.000000 webscout-3.0b0/webscout/exceptions.py
+-rw-rw-rw-   0        0        0    24487 2024-05-12 13:39:37.000000 webscout-3.0b0/webscout/g4f.py
+-rw-rw-rw-   0        0        0      692 2024-05-08 15:52:48.000000 webscout-3.0b0/webscout/models.py
+-rw-rw-rw-   0        0        0     5896 2024-05-08 15:52:48.000000 webscout-3.0b0/webscout/tempid.py
+-rw-rw-rw-   0        0        0    20622 2024-05-08 15:52:48.000000 webscout-3.0b0/webscout/transcriber.py
+-rw-rw-rw-   0        0        0     2603 2024-05-09 03:33:11.000000 webscout-3.0b0/webscout/utils.py
+-rw-rw-rw-   0        0        0       23 2024-05-26 12:42:41.000000 webscout-3.0b0/webscout/version.py
+-rw-rw-rw-   0        0        0      967 2024-05-08 15:52:48.000000 webscout-3.0b0/webscout/voice.py
+-rw-rw-rw-   0        0        0    85324 2024-05-14 14:12:32.000000 webscout-3.0b0/webscout/webai.py
+-rw-rw-rw-   0        0        0    42650 2024-05-19 13:03:19.000000 webscout-3.0b0/webscout/webscout_search.py
+-rw-rw-rw-   0        0        0    14471 2024-05-19 13:04:35.000000 webscout-3.0b0/webscout/webscout_search_async.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:49:41.251897 webscout-3.0b0/webscout.egg-info/
+-rw-rw-rw-   0        0        0    47777 2024-05-30 06:49:37.000000 webscout-3.0b0/webscout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1827 2024-05-30 06:49:38.000000 webscout-3.0b0/webscout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 06:49:37.000000 webscout-3.0b0/webscout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-05-30 06:49:37.000000 webscout-3.0b0/webscout.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      433 2024-05-30 06:49:37.000000 webscout-3.0b0/webscout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-30 06:49:37.000000 webscout-3.0b0/webscout.egg-info/top_level.txt
```

### Comparing `webscout-2.9/DeepWEBS/documents/query_results_extractor.py` & `webscout-3.0b0/DeepWEBS/documents/query_results_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/DeepWEBS/documents/webpage_content_extractor.py` & `webscout-3.0b0/DeepWEBS/documents/webpage_content_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/DeepWEBS/networks/filepath_converter.py` & `webscout-3.0b0/DeepWEBS/networks/filepath_converter.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/DeepWEBS/networks/google_searcher.py` & `webscout-3.0b0/DeepWEBS/networks/google_searcher.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/DeepWEBS/networks/network_configs.py` & `webscout-3.0b0/DeepWEBS/networks/network_configs.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/DeepWEBS/networks/webpage_fetcher.py` & `webscout-3.0b0/DeepWEBS/networks/webpage_fetcher.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/DeepWEBS/utilsdw/enver.py` & `webscout-3.0b0/DeepWEBS/utilsdw/enver.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/DeepWEBS/utilsdw/logger.py` & `webscout-3.0b0/DeepWEBS/utilsdw/logger.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/LICENSE.md` & `webscout-3.0b0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `webscout-2.9/PKG-INFO` & `webscout-3.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 2.9
+Version: 3.0b0
 Summary: Search for anything using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, webai (terminal gpt and open interpreter) and offline LLMs
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: webscout Version: 2.9 Summary: Search for anything
-using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt
-videos, temporary email and phone number generation, has TTS support, webai
-(terminal gpt and open interpreter) and offline LLMs Author: OEvortex Author-
-email: helpingai5@gmail.com License: HelpingAI Simplified Universal License
-Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
-Project-URL: Source, https://github.com/OE-LUCIFER/Webscout Project-URL:
-Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube,
-https://youtube.com/@OEvortex Classifier: Development Status :: 5 - Production/
-Stable Classifier: Intended Audience :: Developers Classifier: License ::
-Other/Proprietary License Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search Classifier: Topic
-:: Software Development :: Libraries :: Python Modules Description-Content-
-Type: text/markdown License-File: LICENSE.md Requires-Dist:
+Metadata-Version: 2.1 Name: webscout Version: 3.0b0 Summary: Search for
+anything using Google, DuckDuckGo, phind.com, Contains AI models, can
+transcribe yt videos, temporary email and phone number generation, has TTS
+support, webai (terminal gpt and open interpreter) and offline LLMs Author:
+OEvortex Author-email: helpingai5@gmail.com License: HelpingAI Simplified
+Universal License Project-URL: Documentation, https://github.com/OE-LUCIFER/
+Webscout/wiki Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
+Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-
+URL: YouTube, https://youtube.com/@OEvortex Classifier: Development Status :: 5
+- Production/Stable Classifier: Intended Audience :: Developers Classifier:
+License :: Other/Proprietary License Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: Programming Language :: Python :: Implementation ::
+CPython Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown License-File: LICENSE.md Requires-Dist:
 docstring_inheritance Requires-Dist: click Requires-Dist: curl_cffi Requires-
 Dist: lxml Requires-Dist: nest-asyncio Requires-Dist: selenium Requires-Dist:
 tqdm Requires-Dist: webdriver-manager Requires-Dist: halo>=0.0.31 Requires-
 Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-Dist: python-dotenv Requires-
 Dist: beautifulsoup4 Requires-Dist: markdownify Requires-Dist: pydantic
 Requires-Dist: requests Requires-Dist: sse_starlette Requires-Dist: termcolor
 Requires-Dist: tiktoken Requires-Dist: tldextract Requires-Dist: orjson
```

### Comparing `webscout-2.9/README.md` & `webscout-3.0b0/README.md`

 * *Files identical despite different names*

### Comparing `webscout-2.9/setup.py` & `webscout-3.0b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="webscout",
-    version="2.9",
+    version="3.0-beta",
     description="Search for anything using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, webai (terminal gpt and open interpreter) and offline LLMs",
     long_description=README,
     long_description_content_type="text/markdown",
     author="OEvortex",
     author_email="helpingai5@gmail.com",
     packages=find_packages(),
     classifiers=[
```

### Comparing `webscout-2.9/webscout/AIauto.py` & `webscout-3.0b0/webscout/AIauto.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/AIbase.py` & `webscout-3.0b0/webscout/AIbase.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/AIutel.py` & `webscout-3.0b0/webscout/AIutel.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,14 +42,15 @@
    "you",
    "xjai",
    "thinkany",
    "berlin4h",
    "chatgptuk",
    "auto",
    "poe",
+   "basedgpt",
 ]
 gpt4free_providers = [
     provider.__name__ for provider in g4f.Provider.__providers__  # if provider.working
 ]
 
 available_providers = webai + gpt4free_providers
 def sanitize_stream(
```

### Comparing `webscout-2.9/webscout/DWEBS.py` & `webscout-3.0b0/webscout/DWEBS.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/LLM.py` & `webscout-3.0b0/webscout/LLM.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/Local/formats.py` & `webscout-3.0b0/webscout/Local/formats.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/Local/model.py` & `webscout-3.0b0/webscout/Local/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from ._version import __version__, __llama_cpp_version__
 
 """Submodule containing the Model class to work with language models"""
 
 import sys
 import numpy as np
 
@@ -11,15 +12,15 @@
     print_verbose,
     GGUFReader,
     softmax
 )
 
 from .samplers import SamplerSettings, DefaultSampling
 from llama_cpp import Llama, StoppingCriteriaList
-from typing    import Generator, Optional, Union
+from typing    import Callable, Generator, Optional, Union
 from os.path   import isdir, exists
 from heapq     import nlargest
 
 from os import cpu_count as os_cpu_count
 
 
 class ModelUnloadedException(Exception):
@@ -64,15 +65,15 @@
     def __init__(
         self,
         model_path: str,
         context_length: Optional[int] = None,
         n_gpu_layers: int = 0,
         offload_kqv: bool = True,
         flash_attn: bool = False,
-        verbose: bool = False
+        verbose: bool = False,
     ):
         """
         Given the path to a GGUF file, construct a Model instance.
 
         The model must be in GGUF format.
 
         The following parameters are optional:
@@ -101,15 +102,15 @@
         # save __init__ parameters for __repr__
         self._model_path = model_path
         self._context_length = context_length
         self._n_gpu_layers = n_gpu_layers
         self._offload_kqv = offload_kqv
         self._flash_attn = flash_attn
         self._verbose = self.verbose = verbose
-
+        self.tools = {}
         # if context_length <= 0, use n_ctx_train
         if isinstance(context_length, int) and context_length <= 0:
             context_length = None
 
         # this does not use Llama.metadata because we want to use GGUF
         # metadata to determine some parameters of the Llama instance
         # before it is created
@@ -265,15 +266,85 @@
             print_verbose(f"param: n_batch              == {n_batch}")
             print_verbose(f"param: n_threads            == {n_threads}")
             print_verbose(f"param: n_threads_batch      == {n_threads_batch}")
             print_verbose(f" gguf: n_ctx_train          == {n_ctx_train}")
             print_verbose(f"param: self.context_length  == {self.context_length}")
             print_verbose(f" gguf: rope_freq_base_train == {rope_freq_base_train}")
             print_verbose(f"param: rope_freq_base       == {rope_freq_base}")
-    
+    def register_tool(self, name: str, function: Callable):
+        """
+        Registers a tool for function calling.
+
+        Args:
+            name: The name of the tool.
+            function: The Python function to execute when the tool is called.
+        """
+        self.tools[name] = function
+
+    def _extract_tool_code(self, text: str) -> dict:
+        """
+        Extracts tool code from the model's output using the chatml-function-calling format.
+        
+        Args:
+            text: The model's generated text.
+
+        Returns:
+            A dictionary containing the tool name and arguments, or None if no tool call is found.
+        """
+        try:
+            # Assuming tool code is enclosed in ```tool_code\n...\n```tool_code```
+            start = text.find("```tool_code\n") + len("```tool_code\n")
+            end = text.find("\n```tool_code```")
+            tool_code_json = text[start:end]
+            tool_code = json.loads(tool_code_json)
+            return tool_code
+        except (ValueError, json.JSONDecodeError):
+            return None
+
+    def generate(
+        self,
+        prompt: Union[str, list[int]],
+        stops: list[Union[str, int]] = [],
+        sampler: SamplerSettings = DefaultSampling
+    ) -> str:
+        """
+        Given a prompt, return a generated string, potentially calling and executing tools.
+
+        Args:
+            prompt: The text from which to generate.
+            stops: A list of strings and/or token IDs at which to end the generation early.
+            sampler: The SamplerSettings object used to control text generation.
+
+        Returns:
+            The generated string.
+        """
+        assert_model_is_loaded(self)
+        response_text = self.llama.create_completion(
+            prompt,
+            max_tokens=sampler.max_len_tokens,
+            temperature=sampler.temp,
+            top_p=sampler.top_p,
+            min_p=sampler.min_p,
+            frequency_penalty=sampler.frequency_penalty,
+            presence_penalty=sampler.presence_penalty,
+            repeat_penalty=sampler.repeat_penalty,
+            top_k=sampler.top_k,
+            stop=stops
+        )['choices'][0]['text']
+
+        tool_code = self._extract_tool_code(response_text)
+        if tool_code:
+            # Execute the tool and get its output
+            tool_name = tool_code.get("function", {}).get("name")
+            arguments = tool_code.get("function", {}).get("arguments", "")
+            if tool_name and arguments and tool_name in self.tools:
+                tool_output = self.tools[tool_name](**json.loads(arguments))
+                # Append the tool output to the response
+                response_text += f"\n{tool_output}" 
+        return response_text
     def __repr__(self) -> str:
         return \
             f"Model({repr(self._model_path)}, " + \
             f"context_length={self._context_length}, " + \
             f"n_gpu_layers={self._n_gpu_layers}, " + \
             f"offload_kqv={self._offload_kqv}, "+ \
             f"flash_attn={self._flash_attn}, " + \
```

### Comparing `webscout-2.9/webscout/Local/samplers.py` & `webscout-3.0b0/webscout/Local/samplers.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/Local/thread.py` & `webscout-3.0b0/webscout/Local/thread.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from ._version import __version__, __llama_cpp_version__
 
 """Submodule containing the Thread class, used for interaction with a Model"""
 
 import sys
 
 from .model    import Model, assert_model_is_loaded, _SupportsWriteAndFlush
@@ -76,15 +77,17 @@
 
     def __init__(
         self,
         model: Model,
         format: Union[dict, AdvancedFormat],
         sampler: SamplerSettings = DefaultSampling,
         messages: Optional[list[Message]] = None,
+
     ):
+    
         """
         Given a Model and a format, construct a Thread instance.
 
         model: The Model to use for text generation
         format: The format specifying how messages should be structured (see m.formats)
 
         The following parameters are optional:
@@ -137,15 +140,15 @@
 
         self.model: Model = model
         self.format: Union[dict, AdvancedFormat] = format
         self.messages: list[Message] = [
             self.create_message("system", self.format['system_content'])
         ] if self._messages is None else self._messages
         self.sampler: SamplerSettings = sampler
-
+        self.tools = [] 
         if self.model.verbose:
             print_verbose("new Thread instance with the following attributes:")
             print_verbose(f"model                     == {self.model}")
             print_verbose(f"format['system_prefix']   == {truncate(repr(self.format['system_prefix']))}")
             print_verbose(f"format['system_content']  == {truncate(repr(self.format['system_content']))}")
             print_verbose(f"format['system_suffix']   == {truncate(repr(self.format['system_suffix']))}")
             print_verbose(f"format['user_prefix']     == {truncate(repr(self.format['user_prefix']))}")
@@ -158,16 +161,24 @@
             print_verbose(f"sampler.temp              == {self.sampler.temp}")
             print_verbose(f"sampler.top_p             == {self.sampler.top_p}")
             print_verbose(f"sampler.min_p             == {self.sampler.min_p}")
             print_verbose(f"sampler.frequency_penalty == {self.sampler.frequency_penalty}")
             print_verbose(f"sampler.presence_penalty  == {self.sampler.presence_penalty}")
             print_verbose(f"sampler.repeat_penalty    == {self.sampler.repeat_penalty}")
             print_verbose(f"sampler.top_k             == {self.sampler.top_k}")
-    
+    def add_tool(self, tool: dict):
+        """
+        Adds a tool to the Thread for function calling.
+        ... (Rest of your add_tool docstring)
+        """
+        self.tools.append(tool)
+        self.model.register_tool(tool['function']['name'], tool['function'].get('execute', None))
 
+        # Include tool information in the system message
+        self.messages[0]['content'] += f"\nYou have access to the following tool:\n```tool_code\n{json.dumps(tool)}\n```tool_code"
     def __repr__(self) -> str:
         return \
             f"Thread({repr(self.model)}, {repr(self.format)}, " + \
             f"{repr(self.sampler)}, {repr(self.messages)})"
     
     def __str__(self) -> str:
         return self.as_string()
```

### Comparing `webscout-2.9/webscout/Local/utils.py` & `webscout-3.0b0/webscout/Local/utils.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/Provider/BasedGPT.py` & `webscout-3.0b0/webscout/Provider/BasedGPT.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/Provider/Berlin4h.py` & `webscout-3.0b0/webscout/Provider/Berlin4h.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/Provider/Blackboxai.py` & `webscout-3.0b0/webscout/Provider/Blackboxai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/Provider/ChatGPTUK.py` & `webscout-3.0b0/webscout/Provider/ChatGPTUK.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/Provider/Cohere.py` & `webscout-3.0b0/webscout/Provider/Cohere.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/Provider/Gemini.py` & `webscout-3.0b0/webscout/Provider/Gemini.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/Provider/Groq.py` & `webscout-3.0b0/webscout/Provider/Groq.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/Provider/Koboldai.py` & `webscout-3.0b0/webscout/Provider/Koboldai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/Provider/Leo.py` & `webscout-3.0b0/webscout/Provider/Leo.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/Provider/Llama2.py` & `webscout-3.0b0/webscout/Provider/Llama2.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/Provider/OpenGPT.py` & `webscout-3.0b0/webscout/Provider/OpenGPT.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/Provider/Openai.py` & `webscout-3.0b0/webscout/Provider/Openai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/Provider/Perplexity.py` & `webscout-3.0b0/webscout/Provider/Perplexity.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/Provider/Phind.py` & `webscout-3.0b0/webscout/Provider/Phind.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/Provider/Poe.py` & `webscout-3.0b0/webscout/Provider/Poe.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/Provider/Reka.py` & `webscout-3.0b0/webscout/Provider/Reka.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/Provider/ThinkAnyAI.py` & `webscout-3.0b0/webscout/Provider/ThinkAnyAI.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/Provider/Xjai.py` & `webscout-3.0b0/webscout/Provider/Xjai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/Provider/Yepchat.py` & `webscout-3.0b0/webscout/Provider/Yepchat.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/Provider/Youchat.py` & `webscout-3.0b0/webscout/Provider/Youchat.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/Provider/__init__.py` & `webscout-3.0b0/webscout/Provider/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from .Yepchat import YEPCHAT
 from .Yepchat import AsyncYEPCHAT
 from .Youchat import YouChat
 from .Gemini import GEMINI
 from .Berlin4h import Berlin4h
 from .ChatGPTUK import ChatGPTUK
 from .Poe import POE
-from .BasedGPT import *
+from .BasedGPT import BasedGPT
 __all__ = [
     'ThinkAnyAI',
     'Xjai',
     'LLAMA2', 
     'AsyncLLAMA2',
     'Cohere',
     'REKA',
@@ -53,9 +53,10 @@
     'AsyncPhindSearch',
     'YEPCHAT',
     'AsyncYEPCHAT',
     'YouChat',
     'GEMINI',
     'Berlin4h',
     'ChatGPTUK',
-    'POE'
+    'POE',
+    'BasedGPT',
 ]
```

### Comparing `webscout-2.9/webscout/__init__.py` & `webscout-3.0b0/webscout/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,15 @@
    "you",
    "xjai",
    "thinkany",
    "berlin4h",
    "chatgptuk",
    "auto",
    "poe",
+   "basedgpt",
 ]
 
 gpt4free_providers = [
    provider.__name__ for provider in g4f.Provider.__providers__  # if provider.working
 ]
 
 available_providers = webai + gpt4free_providers
```

### Comparing `webscout-2.9/webscout/async_providers.py` & `webscout-3.0b0/webscout/async_providers.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/cli.py` & `webscout-3.0b0/webscout/cli.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/g4f.py` & `webscout-3.0b0/webscout/g4f.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/models.py` & `webscout-3.0b0/webscout/models.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/tempid.py` & `webscout-3.0b0/webscout/tempid.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/transcriber.py` & `webscout-3.0b0/webscout/transcriber.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/utils.py` & `webscout-3.0b0/webscout/utils.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/voice.py` & `webscout-3.0b0/webscout/voice.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/webai.py` & `webscout-3.0b0/webscout/webai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/webscout_search.py` & `webscout-3.0b0/webscout/webscout_search.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout/webscout_search_async.py` & `webscout-3.0b0/webscout/webscout_search_async.py`

 * *Files identical despite different names*

### Comparing `webscout-2.9/webscout.egg-info/PKG-INFO` & `webscout-3.0b0/webscout.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 2.9
+Version: 3.0b0
 Summary: Search for anything using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, webai (terminal gpt and open interpreter) and offline LLMs
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: webscout Version: 2.9 Summary: Search for anything
-using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt
-videos, temporary email and phone number generation, has TTS support, webai
-(terminal gpt and open interpreter) and offline LLMs Author: OEvortex Author-
-email: helpingai5@gmail.com License: HelpingAI Simplified Universal License
-Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
-Project-URL: Source, https://github.com/OE-LUCIFER/Webscout Project-URL:
-Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube,
-https://youtube.com/@OEvortex Classifier: Development Status :: 5 - Production/
-Stable Classifier: Intended Audience :: Developers Classifier: License ::
-Other/Proprietary License Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search Classifier: Topic
-:: Software Development :: Libraries :: Python Modules Description-Content-
-Type: text/markdown License-File: LICENSE.md Requires-Dist:
+Metadata-Version: 2.1 Name: webscout Version: 3.0b0 Summary: Search for
+anything using Google, DuckDuckGo, phind.com, Contains AI models, can
+transcribe yt videos, temporary email and phone number generation, has TTS
+support, webai (terminal gpt and open interpreter) and offline LLMs Author:
+OEvortex Author-email: helpingai5@gmail.com License: HelpingAI Simplified
+Universal License Project-URL: Documentation, https://github.com/OE-LUCIFER/
+Webscout/wiki Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
+Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-
+URL: YouTube, https://youtube.com/@OEvortex Classifier: Development Status :: 5
+- Production/Stable Classifier: Intended Audience :: Developers Classifier:
+License :: Other/Proprietary License Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: Programming Language :: Python :: Implementation ::
+CPython Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown License-File: LICENSE.md Requires-Dist:
 docstring_inheritance Requires-Dist: click Requires-Dist: curl_cffi Requires-
 Dist: lxml Requires-Dist: nest-asyncio Requires-Dist: selenium Requires-Dist:
 tqdm Requires-Dist: webdriver-manager Requires-Dist: halo>=0.0.31 Requires-
 Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-Dist: python-dotenv Requires-
 Dist: beautifulsoup4 Requires-Dist: markdownify Requires-Dist: pydantic
 Requires-Dist: requests Requires-Dist: sse_starlette Requires-Dist: termcolor
 Requires-Dist: tiktoken Requires-Dist: tldextract Requires-Dist: orjson
```

### Comparing `webscout-2.9/webscout.egg-info/SOURCES.txt` & `webscout-3.0b0/webscout.egg-info/SOURCES.txt`

 * *Files identical despite different names*

