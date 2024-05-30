# Comparing `tmp/gpt-researcher-0.6.0.tar.gz` & `tmp/gpt-researcher-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-researcher-0.6.0.tar", last modified: Mon May 27 07:04:25 2024, max compression
+gzip compressed data, was "gpt-researcher-0.6.1.tar", last modified: Thu May 30 14:29:34 2024, max compression
```

## Comparing `gpt-researcher-0.6.0.tar` & `gpt-researcher-0.6.1.tar`

### file list

```diff
@@ -1,121 +1,122 @@
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.057073 gpt-researcher-0.6.0/
--rw-r--r--   0 assafel    (501) staff       (20)     1069 2024-04-22 11:21:41.000000 gpt-researcher-0.6.0/LICENSE
--rw-r--r--   0 assafel    (501) staff       (20)    13395 2024-05-27 07:04:25.056505 gpt-researcher-0.6.0/PKG-INFO
--rw-r--r--   0 assafel    (501) staff       (20)    12672 2024-05-26 12:12:16.000000 gpt-researcher-0.6.0/README.md
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:24.996781 gpt-researcher-0.6.0/backend/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.6.0/backend/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:24.997722 gpt-researcher-0.6.0/backend/report_type/
--rw-r--r--   0 assafel    (501) staff       (20)      165 2024-04-22 11:21:41.000000 gpt-researcher-0.6.0/backend/report_type/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:24.999100 gpt-researcher-0.6.0/backend/report_type/basic_report/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.6.0/backend/report_type/basic_report/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      859 2024-05-20 06:53:38.000000 gpt-researcher-0.6.0/backend/report_type/basic_report/basic_report.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.000600 gpt-researcher-0.6.0/backend/report_type/detailed_report/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.6.0/backend/report_type/detailed_report/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     6151 2024-05-20 06:53:38.000000 gpt-researcher-0.6.0/backend/report_type/detailed_report/detailed_report.py
--rw-r--r--   0 assafel    (501) staff       (20)     2405 2024-05-20 06:53:38.000000 gpt-researcher-0.6.0/backend/server.py
--rw-r--r--   0 assafel    (501) staff       (20)     2720 2024-05-20 05:44:03.000000 gpt-researcher-0.6.0/backend/utils.py
--rw-r--r--   0 assafel    (501) staff       (20)     2986 2024-05-20 06:53:38.000000 gpt-researcher-0.6.0/backend/websocket_manager.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.001717 gpt-researcher-0.6.0/gpt_researcher/
--rw-r--r--   0 assafel    (501) staff       (20)      100 2023-11-13 18:29:19.000000 gpt-researcher-0.6.0/gpt_researcher/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.006260 gpt-researcher-0.6.0/gpt_researcher/config/
--rw-r--r--   0 assafel    (501) staff       (20)       48 2023-11-13 18:29:19.000000 gpt-researcher-0.6.0/gpt_researcher/config/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2454 2024-05-27 05:45:21.000000 gpt-researcher-0.6.0/gpt_researcher/config/config.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.008963 gpt-researcher-0.6.0/gpt_researcher/context/
--rw-r--r--   0 assafel    (501) staff       (20)      140 2023-11-19 07:01:11.000000 gpt-researcher-0.6.0/gpt_researcher/context/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1796 2024-05-09 12:40:13.000000 gpt-researcher-0.6.0/gpt_researcher/context/compression.py
--rw-r--r--   0 assafel    (501) staff       (20)      801 2023-11-19 07:01:11.000000 gpt-researcher-0.6.0/gpt_researcher/context/retriever.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.010868 gpt-researcher-0.6.0/gpt_researcher/document/
--rw-r--r--   0 assafel    (501) staff       (20)       67 2024-05-20 06:53:38.000000 gpt-researcher-0.6.0/gpt_researcher/document/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2229 2024-05-20 06:53:38.000000 gpt-researcher-0.6.0/gpt_researcher/document/document.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.011739 gpt-researcher-0.6.0/gpt_researcher/llm_provider/
--rw-r--r--   0 assafel    (501) staff       (20)      644 2024-05-27 06:43:44.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.012729 gpt-researcher-0.6.0/gpt_researcher/llm_provider/anthropic/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-05-27 06:15:55.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/anthropic/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2116 2024-05-27 06:42:16.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/anthropic/anthropic.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.013967 gpt-researcher-0.6.0/gpt_researcher/llm_provider/azureopenai/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/azureopenai/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     3068 2024-04-22 11:21:41.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/azureopenai/azureopenai.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.016825 gpt-researcher-0.6.0/gpt_researcher/llm_provider/google/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/google/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     3670 2024-04-22 11:21:41.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/google/google.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.018732 gpt-researcher-0.6.0/gpt_researcher/llm_provider/groq/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-05-26 12:12:16.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/groq/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2074 2024-05-26 12:12:16.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/groq/groq.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.020780 gpt-researcher-0.6.0/gpt_researcher/llm_provider/huggingface/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-05-27 06:16:19.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/huggingface/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2130 2024-05-27 06:41:57.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/huggingface/huggingface.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.021988 gpt-researcher-0.6.0/gpt_researcher/llm_provider/mistral/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-05-27 06:16:34.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/mistral/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2108 2024-05-27 06:42:02.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/mistral/mistral.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.023201 gpt-researcher-0.6.0/gpt_researcher/llm_provider/ollama/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-05-27 05:45:21.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/ollama/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2037 2024-05-27 05:45:21.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/ollama/ollama.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.024969 gpt-researcher-0.6.0/gpt_researcher/llm_provider/openai/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/openai/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2457 2024-05-21 05:23:12.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/openai/openai.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.026484 gpt-researcher-0.6.0/gpt_researcher/llm_provider/together/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-05-27 06:36:44.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/together/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2106 2024-05-27 06:42:09.000000 gpt-researcher-0.6.0/gpt_researcher/llm_provider/together/together.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.030226 gpt-researcher-0.6.0/gpt_researcher/master/
--rw-r--r--   0 assafel    (501) staff       (20)       61 2023-11-13 18:29:19.000000 gpt-researcher-0.6.0/gpt_researcher/master/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)    10219 2024-05-21 05:18:28.000000 gpt-researcher-0.6.0/gpt_researcher/master/agent.py
--rw-r--r--   0 assafel    (501) staff       (20)    12330 2024-05-26 12:12:16.000000 gpt-researcher-0.6.0/gpt_researcher/master/functions.py
--rw-r--r--   0 assafel    (501) staff       (20)    14933 2024-05-25 06:42:57.000000 gpt-researcher-0.6.0/gpt_researcher/master/prompts.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.032146 gpt-researcher-0.6.0/gpt_researcher/memory/
--rw-r--r--   0 assafel    (501) staff       (20)       31 2023-11-19 07:01:11.000000 gpt-researcher-0.6.0/gpt_researcher/memory/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1721 2024-05-27 05:45:21.000000 gpt-researcher-0.6.0/gpt_researcher/memory/embeddings.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.033049 gpt-researcher-0.6.0/gpt_researcher/retrievers/
--rw-r--r--   0 assafel    (501) staff       (20)      445 2024-05-26 12:12:16.000000 gpt-researcher-0.6.0/gpt_researcher/retrievers/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.034685 gpt-researcher-0.6.0/gpt_researcher/retrievers/bing/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-08 11:24:31.000000 gpt-researcher-0.6.0/gpt_researcher/retrievers/bing/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2240 2023-12-08 11:24:31.000000 gpt-researcher-0.6.0/gpt_researcher/retrievers/bing/bing.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.036144 gpt-researcher-0.6.0/gpt_researcher/retrievers/duckduckgo/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.6.0/gpt_researcher/retrievers/duckduckgo/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      479 2024-05-06 05:46:56.000000 gpt-researcher-0.6.0/gpt_researcher/retrievers/duckduckgo/duckduckgo.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.037971 gpt-researcher-0.6.0/gpt_researcher/retrievers/google/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.6.0/gpt_researcher/retrievers/google/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2535 2023-11-19 07:01:11.000000 gpt-researcher-0.6.0/gpt_researcher/retrievers/google/google.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.039402 gpt-researcher-0.6.0/gpt_researcher/retrievers/searx/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.6.0/gpt_researcher/retrievers/searx/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1294 2024-04-22 11:21:41.000000 gpt-researcher-0.6.0/gpt_researcher/retrievers/searx/searx.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.040865 gpt-researcher-0.6.0/gpt_researcher/retrievers/serpapi/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.6.0/gpt_researcher/retrievers/serpapi/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2418 2024-05-16 08:47:07.000000 gpt-researcher-0.6.0/gpt_researcher/retrievers/serpapi/serpapi.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.042340 gpt-researcher-0.6.0/gpt_researcher/retrievers/serper/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.6.0/gpt_researcher/retrievers/serper/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2149 2024-05-16 08:47:07.000000 gpt-researcher-0.6.0/gpt_researcher/retrievers/serper/serper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.043728 gpt-researcher-0.6.0/gpt_researcher/retrievers/tavily_search/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.6.0/gpt_researcher/retrievers/tavily_search/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1926 2024-05-26 12:12:16.000000 gpt-researcher-0.6.0/gpt_researcher/retrievers/tavily_search/tavily_search.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.045598 gpt-researcher-0.6.0/gpt_researcher/scraper/
--rw-r--r--   0 assafel    (501) staff       (20)      398 2024-03-17 08:29:46.000000 gpt-researcher-0.6.0/gpt_researcher/scraper/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.046879 gpt-researcher-0.6.0/gpt_researcher/scraper/arxiv/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.6.0/gpt_researcher/scraper/arxiv/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      762 2024-03-12 13:09:58.000000 gpt-researcher-0.6.0/gpt_researcher/scraper/arxiv/arxiv.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.048402 gpt-researcher-0.6.0/gpt_researcher/scraper/beautiful_soup/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.6.0/gpt_researcher/scraper/beautiful_soup/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1992 2024-03-12 13:09:58.000000 gpt-researcher-0.6.0/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.049886 gpt-researcher-0.6.0/gpt_researcher/scraper/newspaper/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.6.0/gpt_researcher/scraper/newspaper/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1312 2024-03-12 13:09:58.000000 gpt-researcher-0.6.0/gpt_researcher/scraper/newspaper/newspaper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.051121 gpt-researcher-0.6.0/gpt_researcher/scraper/pymupdf/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.6.0/gpt_researcher/scraper/pymupdf/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      640 2024-03-12 13:09:58.000000 gpt-researcher-0.6.0/gpt_researcher/scraper/pymupdf/pymupdf.py
--rw-r--r--   0 assafel    (501) staff       (20)     3111 2024-03-17 08:29:46.000000 gpt-researcher-0.6.0/gpt_researcher/scraper/scraper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.052432 gpt-researcher-0.6.0/gpt_researcher/scraper/web_base_loader/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.6.0/gpt_researcher/scraper/web_base_loader/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1074 2024-03-12 13:09:58.000000 gpt-researcher-0.6.0/gpt_researcher/scraper/web_base_loader/web_base_loader.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.055461 gpt-researcher-0.6.0/gpt_researcher/utils/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.6.0/gpt_researcher/utils/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      341 2024-05-20 06:53:38.000000 gpt-researcher-0.6.0/gpt_researcher/utils/enum.py
--rw-r--r--   0 assafel    (501) staff       (20)     6062 2024-05-27 06:45:30.000000 gpt-researcher-0.6.0/gpt_researcher/utils/llm.py
--rw-r--r--   0 assafel    (501) staff       (20)      216 2024-04-22 11:21:41.000000 gpt-researcher-0.6.0/gpt_researcher/utils/validators.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-27 07:04:25.004843 gpt-researcher-0.6.0/gpt_researcher.egg-info/
--rw-r--r--   0 assafel    (501) staff       (20)    13395 2024-05-27 07:04:24.000000 gpt-researcher-0.6.0/gpt_researcher.egg-info/PKG-INFO
--rw-r--r--   0 assafel    (501) staff       (20)     3275 2024-05-27 07:04:24.000000 gpt-researcher-0.6.0/gpt_researcher.egg-info/SOURCES.txt
--rw-r--r--   0 assafel    (501) staff       (20)        1 2024-05-27 07:04:24.000000 gpt-researcher-0.6.0/gpt_researcher.egg-info/dependency_links.txt
--rw-r--r--   0 assafel    (501) staff       (20)      458 2024-05-27 07:04:24.000000 gpt-researcher-0.6.0/gpt_researcher.egg-info/requires.txt
--rw-r--r--   0 assafel    (501) staff       (20)       23 2024-05-27 07:04:24.000000 gpt-researcher-0.6.0/gpt_researcher.egg-info/top_level.txt
--rw-r--r--   0 assafel    (501) staff       (20)     1182 2024-05-20 06:53:38.000000 gpt-researcher-0.6.0/pyproject.toml
--rw-r--r--   0 assafel    (501) staff       (20)       38 2024-05-27 07:04:25.057226 gpt-researcher-0.6.0/setup.cfg
--rw-r--r--   0 assafel    (501) staff       (20)     1176 2024-05-27 07:04:02.000000 gpt-researcher-0.6.0/setup.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.103357 gpt-researcher-0.6.1/
+-rw-r--r--   0 assafel    (501) staff       (20)     1069 2024-04-22 11:21:41.000000 gpt-researcher-0.6.1/LICENSE
+-rw-r--r--   0 assafel    (501) staff       (20)    13395 2024-05-30 14:29:34.102629 gpt-researcher-0.6.1/PKG-INFO
+-rw-r--r--   0 assafel    (501) staff       (20)    12672 2024-05-30 06:43:18.000000 gpt-researcher-0.6.1/README.md
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.020636 gpt-researcher-0.6.1/backend/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.6.1/backend/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.021610 gpt-researcher-0.6.1/backend/report_type/
+-rw-r--r--   0 assafel    (501) staff       (20)      165 2024-04-22 11:21:41.000000 gpt-researcher-0.6.1/backend/report_type/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.023219 gpt-researcher-0.6.1/backend/report_type/basic_report/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.6.1/backend/report_type/basic_report/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      859 2024-05-20 06:53:38.000000 gpt-researcher-0.6.1/backend/report_type/basic_report/basic_report.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.024574 gpt-researcher-0.6.1/backend/report_type/detailed_report/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.6.1/backend/report_type/detailed_report/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     6149 2024-05-30 14:29:23.000000 gpt-researcher-0.6.1/backend/report_type/detailed_report/detailed_report.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2405 2024-05-20 06:53:38.000000 gpt-researcher-0.6.1/backend/server.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2720 2024-05-20 05:44:03.000000 gpt-researcher-0.6.1/backend/utils.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2986 2024-05-20 06:53:38.000000 gpt-researcher-0.6.1/backend/websocket_manager.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.025202 gpt-researcher-0.6.1/gpt_researcher/
+-rw-r--r--   0 assafel    (501) staff       (20)      100 2023-11-13 18:29:19.000000 gpt-researcher-0.6.1/gpt_researcher/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.030943 gpt-researcher-0.6.1/gpt_researcher/config/
+-rw-r--r--   0 assafel    (501) staff       (20)       48 2023-11-13 18:29:19.000000 gpt-researcher-0.6.1/gpt_researcher/config/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2454 2024-05-27 05:45:21.000000 gpt-researcher-0.6.1/gpt_researcher/config/config.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.033532 gpt-researcher-0.6.1/gpt_researcher/context/
+-rw-r--r--   0 assafel    (501) staff       (20)      140 2023-11-19 07:01:11.000000 gpt-researcher-0.6.1/gpt_researcher/context/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2111 2024-05-30 14:29:23.000000 gpt-researcher-0.6.1/gpt_researcher/context/compression.py
+-rw-r--r--   0 assafel    (501) staff       (20)      801 2023-11-19 07:01:11.000000 gpt-researcher-0.6.1/gpt_researcher/context/retriever.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.036483 gpt-researcher-0.6.1/gpt_researcher/document/
+-rw-r--r--   0 assafel    (501) staff       (20)       67 2024-05-20 06:53:38.000000 gpt-researcher-0.6.1/gpt_researcher/document/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2229 2024-05-20 06:53:38.000000 gpt-researcher-0.6.1/gpt_researcher/document/document.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.037967 gpt-researcher-0.6.1/gpt_researcher/llm_provider/
+-rw-r--r--   0 assafel    (501) staff       (20)      644 2024-05-27 06:43:44.000000 gpt-researcher-0.6.1/gpt_researcher/llm_provider/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.040035 gpt-researcher-0.6.1/gpt_researcher/llm_provider/anthropic/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-05-27 06:15:55.000000 gpt-researcher-0.6.1/gpt_researcher/llm_provider/anthropic/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2116 2024-05-27 06:42:16.000000 gpt-researcher-0.6.1/gpt_researcher/llm_provider/anthropic/anthropic.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.042171 gpt-researcher-0.6.1/gpt_researcher/llm_provider/azureopenai/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.6.1/gpt_researcher/llm_provider/azureopenai/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3068 2024-04-22 11:21:41.000000 gpt-researcher-0.6.1/gpt_researcher/llm_provider/azureopenai/azureopenai.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.046230 gpt-researcher-0.6.1/gpt_researcher/llm_provider/google/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.6.1/gpt_researcher/llm_provider/google/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3670 2024-04-22 11:21:41.000000 gpt-researcher-0.6.1/gpt_researcher/llm_provider/google/google.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.048033 gpt-researcher-0.6.1/gpt_researcher/llm_provider/groq/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-05-26 12:12:16.000000 gpt-researcher-0.6.1/gpt_researcher/llm_provider/groq/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2074 2024-05-26 12:12:16.000000 gpt-researcher-0.6.1/gpt_researcher/llm_provider/groq/groq.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.049691 gpt-researcher-0.6.1/gpt_researcher/llm_provider/huggingface/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-05-27 06:16:19.000000 gpt-researcher-0.6.1/gpt_researcher/llm_provider/huggingface/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2130 2024-05-27 06:41:57.000000 gpt-researcher-0.6.1/gpt_researcher/llm_provider/huggingface/huggingface.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.052231 gpt-researcher-0.6.1/gpt_researcher/llm_provider/mistral/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-05-27 06:16:34.000000 gpt-researcher-0.6.1/gpt_researcher/llm_provider/mistral/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2108 2024-05-27 06:42:02.000000 gpt-researcher-0.6.1/gpt_researcher/llm_provider/mistral/mistral.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.053931 gpt-researcher-0.6.1/gpt_researcher/llm_provider/ollama/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-05-27 05:45:21.000000 gpt-researcher-0.6.1/gpt_researcher/llm_provider/ollama/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2037 2024-05-27 05:45:21.000000 gpt-researcher-0.6.1/gpt_researcher/llm_provider/ollama/ollama.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.055574 gpt-researcher-0.6.1/gpt_researcher/llm_provider/openai/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.6.1/gpt_researcher/llm_provider/openai/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2457 2024-05-21 05:23:12.000000 gpt-researcher-0.6.1/gpt_researcher/llm_provider/openai/openai.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.057452 gpt-researcher-0.6.1/gpt_researcher/llm_provider/together/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-05-27 06:36:44.000000 gpt-researcher-0.6.1/gpt_researcher/llm_provider/together/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2106 2024-05-27 06:42:09.000000 gpt-researcher-0.6.1/gpt_researcher/llm_provider/together/together.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.062255 gpt-researcher-0.6.1/gpt_researcher/master/
+-rw-r--r--   0 assafel    (501) staff       (20)       61 2023-11-13 18:29:19.000000 gpt-researcher-0.6.1/gpt_researcher/master/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)    13108 2024-05-30 14:29:23.000000 gpt-researcher-0.6.1/gpt_researcher/master/actions.py
+-rw-r--r--   0 assafel    (501) staff       (20)    11974 2024-05-30 14:29:23.000000 gpt-researcher-0.6.1/gpt_researcher/master/agent.py
+-rw-r--r--   0 assafel    (501) staff       (20)    14933 2024-05-25 06:42:57.000000 gpt-researcher-0.6.1/gpt_researcher/master/prompts.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.064681 gpt-researcher-0.6.1/gpt_researcher/memory/
+-rw-r--r--   0 assafel    (501) staff       (20)       31 2023-11-19 07:01:11.000000 gpt-researcher-0.6.1/gpt_researcher/memory/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1768 2024-05-30 14:29:23.000000 gpt-researcher-0.6.1/gpt_researcher/memory/embeddings.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.065567 gpt-researcher-0.6.1/gpt_researcher/retrievers/
+-rw-r--r--   0 assafel    (501) staff       (20)      445 2024-05-26 12:12:16.000000 gpt-researcher-0.6.1/gpt_researcher/retrievers/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.067483 gpt-researcher-0.6.1/gpt_researcher/retrievers/bing/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-08 11:24:31.000000 gpt-researcher-0.6.1/gpt_researcher/retrievers/bing/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2240 2023-12-08 11:24:31.000000 gpt-researcher-0.6.1/gpt_researcher/retrievers/bing/bing.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.069603 gpt-researcher-0.6.1/gpt_researcher/retrievers/duckduckgo/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.6.1/gpt_researcher/retrievers/duckduckgo/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      479 2024-05-06 05:46:56.000000 gpt-researcher-0.6.1/gpt_researcher/retrievers/duckduckgo/duckduckgo.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.071570 gpt-researcher-0.6.1/gpt_researcher/retrievers/google/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.6.1/gpt_researcher/retrievers/google/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2535 2023-11-19 07:01:11.000000 gpt-researcher-0.6.1/gpt_researcher/retrievers/google/google.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.077921 gpt-researcher-0.6.1/gpt_researcher/retrievers/searx/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.6.1/gpt_researcher/retrievers/searx/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1294 2024-04-22 11:21:41.000000 gpt-researcher-0.6.1/gpt_researcher/retrievers/searx/searx.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.080724 gpt-researcher-0.6.1/gpt_researcher/retrievers/serpapi/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.6.1/gpt_researcher/retrievers/serpapi/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2418 2024-05-16 08:47:07.000000 gpt-researcher-0.6.1/gpt_researcher/retrievers/serpapi/serpapi.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.083029 gpt-researcher-0.6.1/gpt_researcher/retrievers/serper/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.6.1/gpt_researcher/retrievers/serper/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2149 2024-05-16 08:47:07.000000 gpt-researcher-0.6.1/gpt_researcher/retrievers/serper/serper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.084868 gpt-researcher-0.6.1/gpt_researcher/retrievers/tavily_search/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.6.1/gpt_researcher/retrievers/tavily_search/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1926 2024-05-26 12:12:16.000000 gpt-researcher-0.6.1/gpt_researcher/retrievers/tavily_search/tavily_search.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.087570 gpt-researcher-0.6.1/gpt_researcher/scraper/
+-rw-r--r--   0 assafel    (501) staff       (20)      398 2024-03-17 08:29:46.000000 gpt-researcher-0.6.1/gpt_researcher/scraper/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.089172 gpt-researcher-0.6.1/gpt_researcher/scraper/arxiv/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.6.1/gpt_researcher/scraper/arxiv/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      762 2024-03-12 13:09:58.000000 gpt-researcher-0.6.1/gpt_researcher/scraper/arxiv/arxiv.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.091060 gpt-researcher-0.6.1/gpt_researcher/scraper/beautiful_soup/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.6.1/gpt_researcher/scraper/beautiful_soup/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1992 2024-03-12 13:09:58.000000 gpt-researcher-0.6.1/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.092832 gpt-researcher-0.6.1/gpt_researcher/scraper/newspaper/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.6.1/gpt_researcher/scraper/newspaper/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1312 2024-03-12 13:09:58.000000 gpt-researcher-0.6.1/gpt_researcher/scraper/newspaper/newspaper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.094398 gpt-researcher-0.6.1/gpt_researcher/scraper/pymupdf/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.6.1/gpt_researcher/scraper/pymupdf/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      640 2024-03-12 13:09:58.000000 gpt-researcher-0.6.1/gpt_researcher/scraper/pymupdf/pymupdf.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3111 2024-03-17 08:29:46.000000 gpt-researcher-0.6.1/gpt_researcher/scraper/scraper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.096304 gpt-researcher-0.6.1/gpt_researcher/scraper/web_base_loader/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.6.1/gpt_researcher/scraper/web_base_loader/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1074 2024-03-12 13:09:58.000000 gpt-researcher-0.6.1/gpt_researcher/scraper/web_base_loader/web_base_loader.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.101251 gpt-researcher-0.6.1/gpt_researcher/utils/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.6.1/gpt_researcher/utils/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      937 2024-05-30 14:29:23.000000 gpt-researcher-0.6.1/gpt_researcher/utils/costs.py
+-rw-r--r--   0 assafel    (501) staff       (20)      341 2024-05-20 06:53:38.000000 gpt-researcher-0.6.1/gpt_researcher/utils/enum.py
+-rw-r--r--   0 assafel    (501) staff       (20)     5147 2024-05-30 14:29:23.000000 gpt-researcher-0.6.1/gpt_researcher/utils/llm.py
+-rw-r--r--   0 assafel    (501) staff       (20)      216 2024-04-22 11:21:41.000000 gpt-researcher-0.6.1/gpt_researcher/utils/validators.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-30 14:29:34.029465 gpt-researcher-0.6.1/gpt_researcher.egg-info/
+-rw-r--r--   0 assafel    (501) staff       (20)    13395 2024-05-30 14:29:33.000000 gpt-researcher-0.6.1/gpt_researcher.egg-info/PKG-INFO
+-rw-r--r--   0 assafel    (501) staff       (20)     3303 2024-05-30 14:29:33.000000 gpt-researcher-0.6.1/gpt_researcher.egg-info/SOURCES.txt
+-rw-r--r--   0 assafel    (501) staff       (20)        1 2024-05-30 14:29:33.000000 gpt-researcher-0.6.1/gpt_researcher.egg-info/dependency_links.txt
+-rw-r--r--   0 assafel    (501) staff       (20)      555 2024-05-30 14:29:33.000000 gpt-researcher-0.6.1/gpt_researcher.egg-info/requires.txt
+-rw-r--r--   0 assafel    (501) staff       (20)       23 2024-05-30 14:29:33.000000 gpt-researcher-0.6.1/gpt_researcher.egg-info/top_level.txt
+-rw-r--r--   0 assafel    (501) staff       (20)     1202 2024-05-30 14:29:23.000000 gpt-researcher-0.6.1/pyproject.toml
+-rw-r--r--   0 assafel    (501) staff       (20)       38 2024-05-30 14:29:34.103507 gpt-researcher-0.6.1/setup.cfg
+-rw-r--r--   0 assafel    (501) staff       (20)     1176 2024-05-30 14:29:23.000000 gpt-researcher-0.6.1/setup.py
```

### Comparing `gpt-researcher-0.6.0/LICENSE` & `gpt-researcher-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.6.0/PKG-INFO` & `gpt-researcher-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-researcher
-Version: 0.6.0
+Version: 0.6.1
 Summary: GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.
 Home-page: https://github.com/assafelovic/gpt-researcher
 Author: Assaf Elovic
 Author-email: assaf.elovic@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -19,15 +19,15 @@
 <h1 style="display: flex; align-items: center; gap: 10px;">
   <img src="https://github.com/assafelovic/gpt-researcher/assets/13554167/a45bac7c-092c-42e5-8eb6-69acbf20dde5" alt="Logo" width="25">
   GPT Researcher
 </h1>
 
 [![Official Website](https://img.shields.io/badge/Official%20Website-gptr.dev-teal?style=for-the-badge&logo=world&logoColor=white)](https://gptr.dev)
 [![Official Website](https://img.shields.io/badge/Documentation-GPTR-pink?logo=googledocs&logoColor=white&style=for-the-badge)](https://docs.gptr.dev)
-[![Discord Follow](https://dcbadge.vercel.app/api/server/SK3KKuSD?style=for-the-badge)](https://discord.gg/SK3KKuSD)
+[![Discord Follow](https://dcbadge.vercel.app/api/server/cPhHPZ6Z?style=for-the-badge)](https://discord.gg/cPhHPZ6Z)
 
 [![GitHub Repo stars](https://img.shields.io/github/stars/assafelovic/gpt-researcher?style=social)](https://github.com/assafelovic/gpt-researcher)
 [![Twitter Follow](https://img.shields.io/twitter/follow/assaf_elovic?style=social)](https://twitter.com/assaf_elovic)
 [![PyPI version](https://badge.fury.io/py/gpt-researcher.svg)](https://badge.fury.io/py/gpt-researcher)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/assafelovic/gpt-researcher/blob/master/examples/pip-run.ipynb)
 
 <!-- MARKDOWN LINKS & IMAGES -->
```

### Comparing `gpt-researcher-0.6.0/README.md` & `gpt-researcher-0.6.1/gpt_researcher.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,33 @@
+Metadata-Version: 2.1
+Name: gpt-researcher
+Version: 0.6.1
+Summary: GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.
+Home-page: https://github.com/assafelovic/gpt-researcher
+Author: Assaf Elovic
+Author-email: assaf.elovic@gmail.com
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <h1 style="display: flex; align-items: center; gap: 10px;">
   <img src="https://github.com/assafelovic/gpt-researcher/assets/13554167/a45bac7c-092c-42e5-8eb6-69acbf20dde5" alt="Logo" width="25">
   GPT Researcher
 </h1>
 
 [![Official Website](https://img.shields.io/badge/Official%20Website-gptr.dev-teal?style=for-the-badge&logo=world&logoColor=white)](https://gptr.dev)
 [![Official Website](https://img.shields.io/badge/Documentation-GPTR-pink?logo=googledocs&logoColor=white&style=for-the-badge)](https://docs.gptr.dev)
-[![Discord Follow](https://dcbadge.vercel.app/api/server/SK3KKuSD?style=for-the-badge)](https://discord.gg/SK3KKuSD)
+[![Discord Follow](https://dcbadge.vercel.app/api/server/cPhHPZ6Z?style=for-the-badge)](https://discord.gg/cPhHPZ6Z)
 
 [![GitHub Repo stars](https://img.shields.io/github/stars/assafelovic/gpt-researcher?style=social)](https://github.com/assafelovic/gpt-researcher)
 [![Twitter Follow](https://img.shields.io/twitter/follow/assaf_elovic?style=social)](https://twitter.com/assaf_elovic)
 [![PyPI version](https://badge.fury.io/py/gpt-researcher.svg)](https://badge.fury.io/py/gpt-researcher)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/assafelovic/gpt-researcher/blob/master/examples/pip-run.ipynb)
 
 <!-- MARKDOWN LINKS & IMAGES -->
```

### Comparing `gpt-researcher-0.6.0/backend/report_type/basic_report/basic_report.py` & `gpt-researcher-0.6.1/backend/report_type/basic_report/basic_report.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.6.0/backend/report_type/detailed_report/detailed_report.py` & `gpt-researcher-0.6.1/backend/report_type/detailed_report/detailed_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 
 from fastapi import WebSocket
 
 from gpt_researcher.master.agent import GPTResearcher
-from gpt_researcher.master.functions import (add_source_urls, extract_headers,
+from gpt_researcher.master.actions import (add_source_urls, extract_headers,
                                              table_of_contents)
 
 
 class DetailedReport():
     def __init__(self, query: str, report_type: str, report_source: str, source_urls, config_path: str, websocket: WebSocket, subtopics=[]):
         self.query = query
         self.report_type = report_type
```

### Comparing `gpt-researcher-0.6.0/backend/server.py` & `gpt-researcher-0.6.1/backend/server.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.6.0/backend/utils.py` & `gpt-researcher-0.6.1/backend/utils.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.6.0/backend/websocket_manager.py` & `gpt-researcher-0.6.1/backend/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.6.0/gpt_researcher/config/config.py` & `gpt-researcher-0.6.1/gpt_researcher/config/config.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.6.0/gpt_researcher/context/compression.py` & `gpt-researcher-0.6.1/gpt_researcher/context/compression.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,42 +3,47 @@
     ContextualCompressionRetriever,
 )
 from langchain.retrievers.document_compressors import (
     DocumentCompressorPipeline,
     EmbeddingsFilter,
 )
 from langchain.text_splitter import RecursiveCharacterTextSplitter
+from gpt_researcher.utils.costs import estimate_embedding_cost
+from gpt_researcher.memory.embeddings import OPENAI_EMBEDDING_MODEL
 
 
 class ContextCompressor:
     def __init__(self, documents, embeddings, max_results=5, **kwargs):
         self.max_results = max_results
         self.documents = documents
         self.kwargs = kwargs
         self.embeddings = embeddings
         self.similarity_threshold = 0.38
 
-    def _get_contextual_retriever(self):
+    def __get_contextual_retriever(self):
         splitter = RecursiveCharacterTextSplitter(chunk_size=1000, chunk_overlap=100)
         relevance_filter = EmbeddingsFilter(embeddings=self.embeddings,
                                             similarity_threshold=self.similarity_threshold)
         pipeline_compressor = DocumentCompressorPipeline(
             transformers=[splitter, relevance_filter]
         )
         base_retriever = SearchAPIRetriever(
             pages=self.documents
         )
         contextual_retriever = ContextualCompressionRetriever(
             base_compressor=pipeline_compressor, base_retriever=base_retriever
         )
         return contextual_retriever
 
-    def _pretty_print_docs(self, docs, top_n):
+    def __pretty_print_docs(self, docs, top_n):
         return f"\n".join(f"Source: {d.metadata.get('source')}\n"
                           f"Title: {d.metadata.get('title')}\n"
                           f"Content: {d.page_content}\n"
                           for i, d in enumerate(docs) if i < top_n)
 
-    def get_context(self, query, max_results=5):
-        compressed_docs = self._get_contextual_retriever()
+    def get_context(self, query, max_results=5, cost_callback=None):
+        compressed_docs = self.__get_contextual_retriever()
+        print(compressed_docs)
+        if cost_callback:
+            cost_callback(estimate_embedding_cost(model=OPENAI_EMBEDDING_MODEL, docs=self.documents))
         relevant_docs = compressed_docs.invoke(query)
-        return self._pretty_print_docs(relevant_docs, max_results)
+        return self.__pretty_print_docs(relevant_docs, max_results)
```

### Comparing `gpt-researcher-0.6.0/gpt_researcher/context/retriever.py` & `gpt-researcher-0.6.1/gpt_researcher/context/retriever.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.6.0/gpt_researcher/document/document.py` & `gpt-researcher-0.6.1/gpt_researcher/document/document.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.6.0/gpt_researcher/llm_provider/__init__.py` & `gpt-researcher-0.6.1/gpt_researcher/llm_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.6.0/gpt_researcher/llm_provider/anthropic/anthropic.py` & `gpt-researcher-0.6.1/gpt_researcher/llm_provider/anthropic/anthropic.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.6.0/gpt_researcher/llm_provider/azureopenai/azureopenai.py` & `gpt-researcher-0.6.1/gpt_researcher/llm_provider/azureopenai/azureopenai.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.6.0/gpt_researcher/llm_provider/google/google.py` & `gpt-researcher-0.6.1/gpt_researcher/llm_provider/google/google.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.6.0/gpt_researcher/llm_provider/groq/groq.py` & `gpt-researcher-0.6.1/gpt_researcher/llm_provider/groq/groq.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.6.0/gpt_researcher/llm_provider/huggingface/huggingface.py` & `gpt-researcher-0.6.1/gpt_researcher/llm_provider/huggingface/huggingface.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.6.0/gpt_researcher/llm_provider/mistral/mistral.py` & `gpt-researcher-0.6.1/gpt_researcher/llm_provider/mistral/mistral.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.6.0/gpt_researcher/llm_provider/ollama/ollama.py` & `gpt-researcher-0.6.1/gpt_researcher/llm_provider/ollama/ollama.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.6.0/gpt_researcher/llm_provider/openai/openai.py` & `gpt-researcher-0.6.1/gpt_researcher/llm_provider/openai/openai.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.6.0/gpt_researcher/llm_provider/together/together.py` & `gpt-researcher-0.6.1/gpt_researcher/llm_provider/together/together.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.6.0/gpt_researcher/master/agent.py` & `gpt-researcher-0.6.1/gpt_researcher/master/agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 import time
 
 from gpt_researcher.config import Config
 from gpt_researcher.context.compression import ContextCompressor
 from gpt_researcher.document import DocumentLoader
-from gpt_researcher.master.functions import *
+from gpt_researcher.master.actions import *
 from gpt_researcher.memory import Memory
 from gpt_researcher.utils.enum import ReportSource, ReportType
 
 
 class GPTResearcher:
     """
     GPT Researcher
@@ -40,28 +40,29 @@
             websocket
             agent
             role
             parent_query: str
             subtopics: list
             visited_urls: set
         """
-        self.query = query
-        self.agent = agent
-        self.role = role
-        self.report_type = report_type
-        self.report_prompt = get_prompt_by_report_type(self.report_type)  # this validates the report type
-        self.report_source = report_source
-        self.websocket = websocket
+        self.query: str = query
+        self.agent: str = agent
+        self.role: str = role
+        self.report_type: str = report_type
+        self.report_prompt: str = get_prompt_by_report_type(self.report_type)  # this validates the report type
+        self.report_source: str = report_source
+        self.research_costs: float = 0.0
         self.cfg = Config(config_path)
         self.retriever = get_retriever(self.cfg.retriever)
         self.context = context
         self.source_urls = source_urls
         self.memory = Memory(self.cfg.embedding_provider)
-        self.visited_urls = visited_urls
-        self.verbose = verbose
+        self.visited_urls: set[str] = visited_urls
+        self.verbose: bool = verbose
+        self.websocket = websocket
 
         # Only relevant for DETAILED REPORTS
         # --------------------------------------
 
         # Stores the main query of the detailed report
         self.parent_query = parent_query
 
@@ -73,135 +74,152 @@
         Runs the GPT Researcher to conduct research
         """
         if self.verbose:
             await stream_output("logs", f"🔎 Starting the research task for '{self.query}'...", self.websocket)
         
         # Generate Agent
         if not (self.agent and self.role):
-            self.agent, self.role = await choose_agent(self.query, self.cfg, self.parent_query)
+            self.agent, self.role = await choose_agent(query=self.query, cfg=self.cfg,
+                                                       parent_query=self.parent_query, cost_callback=self.add_costs)
 
         if self.verbose:
             await stream_output("logs", self.agent, self.websocket)
 
         # If specified, the researcher will use the given urls as the context for the research.
         if self.source_urls:
-            context = await self.get_context_by_urls(self.source_urls)
+            context = await self.__get_context_by_urls(self.source_urls)
             
         elif self.report_source == ReportSource.Local.value:
             document_data = await DocumentLoader(self.cfg.doc_path).load()
-            context = await self.get_context_by_search(self.query, document_data)
+            context = await self.__get_context_by_search(self.query, document_data)
         
         else:
-            context = await self.get_context_by_search(self.query)
+            context = await self.__get_context_by_search(self.query)
 
         # Extending the global context (This is useful instead of setting the context directly above to avoid over-writing input context)
         self.context.extend(context)
         
         time.sleep(2)
+        if self.verbose:
+            await stream_output("logs", f"Finalized research step.\n💸 Total Research Costs: ${self.get_costs()}", self.websocket)
 
         return self.context
 
     async def write_report(self, existing_headers: list = []):
         """
         Writes the report based on research conducted
 
         Returns:
             str: The report
         """
+        report = ""
 
         if self.verbose:
             await stream_output("logs", f"✍️ Writing summary for research task: {self.query}...", self.websocket)
-
+            
         if self.report_type == "custom_report":
             self.role = self.cfg.agent_role if self.cfg.agent_role else self.role
+            report = await generate_report(
+                query=self.query,
+                context=self.context,
+                agent_role_prompt=self.role,
+                report_type=self.report_type,
+                report_source=self.report_source,
+                websocket=self.websocket,
+                cfg=self.cfg
+            )
         elif self.report_type == "subtopic_report":
             report = await generate_report(
                 query=self.query,
                 context=self.context,
                 agent_role_prompt=self.role,
                 report_type=self.report_type,
                 report_source=self.report_source,
                 websocket=self.websocket,
                 cfg=self.cfg,
                 main_topic=self.parent_query,
-                existing_headers=existing_headers
+                existing_headers=existing_headers,
+                cost_callback=self.add_costs
             )
         else:
             report = await generate_report(
                 query=self.query,
                 context=self.context,
                 agent_role_prompt=self.role,
                 report_type=self.report_type,
                 report_source=self.report_source,
                 websocket=self.websocket,
-                cfg=self.cfg
+                cfg=self.cfg,
+                cost_callback=self.add_costs
             )
 
         return report
 
-    async def get_context_by_urls(self, urls):
+    async def __get_context_by_urls(self, urls):
         """
             Scrapes and compresses the context from the given urls
         """
-        new_search_urls = await self.get_new_urls(urls)
+        new_search_urls = await self.__get_new_urls(urls)
         if self.verbose:
             await stream_output("logs",
                             f"🧠 I will conduct my research based on the following urls: {new_search_urls}...",
                             self.websocket)
         scraped_sites = scrape_urls(new_search_urls, self.cfg)
-        return await self.get_similar_content_by_query(self.query, scraped_sites)
+        return await self.__get_similar_content_by_query(self.query, scraped_sites)
 
-    async def get_context_by_search(self, query, scraped_data: list = []):
+    async def __get_context_by_search(self, query, scraped_data: list = []):
         """
            Generates the context for the research task by searching the query and scraping the results
         Returns:
             context: List of context
         """
         context = []
         # Generate Sub-Queries including original query
-        sub_queries = await get_sub_queries(query, self.role, self.cfg, self.parent_query, self.report_type)
+        sub_queries = await get_sub_queries(query=query, agent_role_prompt=self.role,
+                                            cfg=self.cfg, parent_query=self.parent_query,
+                                            report_type=self.report_type, cost_callback=self.add_costs)
 
         # If this is not part of a sub researcher, add original query to research for better results
         if self.report_type != "subtopic_report":
             sub_queries.append(query)
 
         if self.verbose:
             await stream_output("logs",
                                 f"🧠 I will conduct my research based on the following queries: {sub_queries}...",
                                 self.websocket)
 
         # Using asyncio.gather to process the sub_queries asynchronously
-        context = await asyncio.gather(*[self.process_sub_query(sub_query, scraped_data) for sub_query in sub_queries])
+        context = await asyncio.gather(*[self.__process_sub_query(sub_query, scraped_data) for sub_query in sub_queries])
         return context
 
-    async def process_sub_query(self, sub_query: str, scraped_data: list = []):
+    async def __process_sub_query(self, sub_query: str, scraped_data: list = []):
         """Takes in a sub query and scrapes urls based on it and gathers context.
 
         Args:
             sub_query (str): The sub-query generated from the original query
             scraped_data (list): Scraped data passed in
 
         Returns:
             str: The context gathered from search
         """
         if self.verbose:
             await stream_output("logs", f"\n🔎 Running research for '{sub_query}'...", self.websocket)
 
         if not scraped_data:
-            scraped_data = await self.scrape_data_by_query(sub_query)
+            scraped_data = await self.__scrape_data_by_query(sub_query)
 
-        content = await self.get_similar_content_by_query(sub_query, scraped_data)
+        content = await self.__get_similar_content_by_query(sub_query, scraped_data)
 
         if content and self.verbose:
             await stream_output("logs", f"📃 {content}", self.websocket)
         elif self.verbose:
             await stream_output("logs", f"🤷 No content found for '{sub_query}'...", self.websocket)
         return content
 
-    async def get_new_urls(self, url_set_input):
+    async def __get_new_urls(self, url_set_input):
         """ Gets the new urls from the given url set.
         Args: url_set_input (set[str]): The url set to get the new urls from
         Returns: list[str]: The new urls from the given url set
         """
 
         new_urls = []
         for url in url_set_input:
@@ -209,56 +227,79 @@
                 self.visited_urls.add(url)
                 new_urls.append(url)
                 if self.verbose:
                     await stream_output("logs", f"✅ Added source url to research: {url}\n", self.websocket)
 
         return new_urls
 
-    async def scrape_data_by_query(self, sub_query):
+    async def __scrape_data_by_query(self, sub_query):
         """
         Runs a sub-query
         Args:
             sub_query:
 
         Returns:
             Summary
         """
         # Get Urls
         retriever = self.retriever(sub_query)
         search_results = retriever.search(
             max_results=self.cfg.max_search_results_per_query)
-        new_search_urls = await self.get_new_urls([url.get("href") for url in search_results])
+        new_search_urls = await self.__get_new_urls([url.get("href") for url in search_results])
 
         # Scrape Urls
         if self.verbose:
             await stream_output("logs", f"🤔 Researching for relevant information...\n", self.websocket)
 
         # Scrape Urls
         scraped_content_results = scrape_urls(new_search_urls, self.cfg)
         return scraped_content_results
 
-    async def get_similar_content_by_query(self, query, pages):
+    async def __get_similar_content_by_query(self, query, pages):
         if self.verbose:
             await stream_output("logs", f"📝 Getting relevant content based on query: {query}...", self.websocket)
 
         # Summarize Raw Data
         context_compressor = ContextCompressor(
             documents=pages,
             embeddings=self.memory.get_embeddings()
         )
         # Run Tasks
-        return context_compressor.get_context(query, max_results=8)
+        return context_compressor.get_context(query=query, max_results=8, cost_callback=self.add_costs)
+
+    ########################################################################################
+
+    # GETTERS & SETTERS
+    def get_source_urls(self) -> list:
+        return list(self.visited_urls)
+
+    def get_research_context(self) -> list:
+        return self.context
+
+    def get_costs(self) -> float:
+        return self.research_costs
+
+    def set_verbose(self, verbose: bool):
+        self.verbose = verbose
+
+    def add_costs(self, cost: int) -> None:
+        if not isinstance(cost, float) and not isinstance(cost, int):
+            raise ValueError("Cost must be an integer or float")
+        self.research_costs += cost
+
+
 
     ########################################################################################
 
     # DETAILED REPORT
 
     async def write_introduction(self):
         # Construct Report Introduction from main topic research
-        introduction = await get_report_introduction(self.query, self.context, self.role, self.cfg, self.websocket)
+        introduction = await get_report_introduction(self.query, self.context, self.role,
+                                                     self.cfg, self.websocket, self.add_costs)
 
         return introduction
 
     async def get_subtopics(self):
         """
         This async function generates subtopics based on user input and other parameters.
```

### Comparing `gpt-researcher-0.6.0/gpt_researcher/master/functions.py` & `gpt-researcher-0.6.1/gpt_researcher/master/actions.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,63 +43,71 @@
 
         case _:
             raise Exception("Retriever not found.")
 
     return retriever
 
 
-async def choose_agent(query, cfg, parent_query=None):
+async def choose_agent(query, cfg, parent_query=None, cost_callback: callable = None):
     """
     Chooses the agent automatically
     Args:
         parent_query: In some cases the research is conducted on a subtopic from the main query.
         Tge parent query allows the agent to know the main context for better reasoning.
         query: original query
         cfg: Config
+        cost_callback: callback for calculating llm costs
 
     Returns:
         agent: Agent name
         agent_role_prompt: Agent role prompt
     """
     query = f"{parent_query} - {query}" if parent_query else f"{query}"
     try:
         response = await create_chat_completion(
             model=cfg.smart_llm_model,
             messages=[
                 {"role": "system", "content": f"{auto_agent_instructions()}"},
                 {"role": "user", "content": f"task: {query}"}],
             temperature=0,
-            llm_provider=cfg.llm_provider
+            llm_provider=cfg.llm_provider,
+            cost_callback=cost_callback
         )
         agent_dict = json.loads(response)
         return agent_dict["server"], agent_dict["agent_role_prompt"]
     except Exception as e:
+        print(f"Error choosing agent: {e}")
         return "Default Agent", "You are an AI critical thinker research assistant. Your sole purpose is to write well written, critically acclaimed, objective and structured reports on given text."
 
 
-async def get_sub_queries(query: str, agent_role_prompt: str, cfg, parent_query: str, report_type: str):
+async def get_sub_queries(query: str, agent_role_prompt: str, cfg, parent_query: str,
+                          report_type: str, cost_callback: callable = None):
     """
     Gets the sub queries
     Args:
         query: original query
         agent_role_prompt: agent role prompt
         cfg: Config
+        parent_query:
+        report_type:
+        cost_callback:
 
     Returns:
         sub_queries: List of sub queries
 
     """
     max_research_iterations = cfg.max_iterations if cfg.max_iterations else 1
     response = await create_chat_completion(
         model=cfg.smart_llm_model,
         messages=[
             {"role": "system", "content": f"{agent_role_prompt}"},
             {"role": "user", "content": generate_search_queries_prompt(query, parent_query, report_type, max_iterations=max_research_iterations)}],
         temperature=0,
-        llm_provider=cfg.llm_provider
+        llm_provider=cfg.llm_provider,
+        cost_callback=cost_callback
     )
 
     print("response : ", response)
 
     sub_queries = json.loads(response)
     return sub_queries
 
@@ -119,16 +127,17 @@
     user_agent = cfg.user_agent if cfg else "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/119.0.0.0 Safari/537.36 Edg/119.0.0.0"
     try:
         content = Scraper(urls, user_agent, cfg.scraper).run()
     except Exception as e:
         print(f"{Fore.RED}Error in scrape_urls: {e}{Style.RESET_ALL}")
     return content
 
-
-async def summarize(query, content, agent_role_prompt, cfg, websocket=None):
+# Deprecated: Instead of summaries using ContextualRetriever embedding.
+# This exists in case we decide to modify in the future
+async def summarize(query, content, agent_role_prompt, cfg, websocket=None, cost_callback: callable = None):
     """
     Asynchronously summarizes a list of URLs.
 
     Args:
         query (str): The search query.
         content (list): List of dictionaries with 'url' and 'raw_content'.
         agent_role_prompt (str): The role prompt for the agent.
@@ -136,15 +145,15 @@
 
     Returns:
         list: A list of dictionaries with 'url' and 'summary'.
     """
 
     # Function to handle each summarization task for a chunk
     async def handle_task(url, chunk):
-        summary = await summarize_url(query, chunk, agent_role_prompt, cfg)
+        summary = await summarize_url(query, chunk, agent_role_prompt, cfg, cost_callback)
         if summary:
             await stream_output("logs", f"🌐 Summarizing url: {url}", websocket)
             await stream_output("logs", f"📃 {summary}", websocket)
         return url, summary
 
     # Function to split raw content into chunks of 10,000 words
     def chunk_content(raw_content, chunk_size=10000):
@@ -170,36 +179,38 @@
         concatenated_summary = ' '.join(summaries)
         concatenated_summaries.append(
             {'url': url, 'summary': concatenated_summary})
 
     return concatenated_summaries
 
 
-async def summarize_url(query, raw_data, agent_role_prompt, cfg):
+async def summarize_url(query, raw_data, agent_role_prompt, cfg, cost_callback: callable = None):
     """
     Summarizes the text
     Args:
         query:
         raw_data:
         agent_role_prompt:
         cfg:
+        cost_callback
 
     Returns:
         summary: str
 
     """
     summary = ""
     try:
         summary = await create_chat_completion(
             model=cfg.fast_llm_model,
             messages=[
                 {"role": "system", "content": f"{agent_role_prompt}"},
                 {"role": "user", "content": f"{generate_summary_prompt(query, raw_data)}"}],
             temperature=0,
-            llm_provider=cfg.llm_provider
+            llm_provider=cfg.llm_provider,
+            cost_callback=cost_callback
         )
     except Exception as e:
         print(f"{Fore.RED}Error in summarize: {e}{Style.RESET_ALL}")
     return summary
 
 
 async def generate_report(
@@ -207,27 +218,29 @@
     context,
     agent_role_prompt: str,
     report_type: str,
     report_source: str,
     websocket,
     cfg,
     main_topic: str = "",
-    existing_headers: list = []
+    existing_headers: list = [],
+    cost_callback: callable = None
 ):
     """
     generates the final report
     Args:
         query:
         context:
         agent_role_prompt:
         report_type:
         websocket:
         cfg:
         main_topic:
         existing_headers:
+        cost_callback:
 
     Returns:
         report:
 
     """
     generate_prompt = get_prompt_by_report_type(report_type)
     report = ""
@@ -243,15 +256,16 @@
             messages=[
                 {"role": "system", "content": f"{agent_role_prompt}"},
                 {"role": "user", "content": content}],
             temperature=0,
             llm_provider=cfg.llm_provider,
             stream=True,
             websocket=websocket,
-            max_tokens=cfg.smart_token_limit
+            max_tokens=cfg.smart_token_limit,
+            cost_callback=cost_callback
         )
     except Exception as e:
         print(f"{Fore.RED}Error in generate_report: {e}{Style.RESET_ALL}")
 
     return report
 
 
@@ -268,26 +282,27 @@
     if not websocket or logging:
         print(output)
 
     if websocket:
         await websocket.send_json({"type": type, "output": output})
 
 
-async def get_report_introduction(query, context, role, config, websocket=None):
+async def get_report_introduction(query, context, role, config, websocket=None, cost_callback: callable = None):
     try:
         introduction = await create_chat_completion(
             model=config.smart_llm_model,
             messages=[
                 {"role": "system", "content": f"{role}"},
                 {"role": "user", "content": generate_report_introduction(query, context)}],
             temperature=0,
             llm_provider=config.llm_provider,
             stream=True,
             websocket=websocket,
-            max_tokens=config.smart_token_limit
+            max_tokens=config.smart_token_limit,
+            cost_callback=cost_callback
         )
 
         return introduction
     except Exception as e:
         print(
             f"{Fore.RED}Error in generating report introduction: {e}{Style.RESET_ALL}")
```

### Comparing `gpt-researcher-0.6.0/gpt_researcher/master/prompts.py` & `gpt-researcher-0.6.1/gpt_researcher/master/prompts.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.6.0/gpt_researcher/memory/embeddings.py` & `gpt-researcher-0.6.1/gpt_researcher/memory/embeddings.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from langchain_community.vectorstores import FAISS
 import os
-
+OPENAI_EMBEDDING_MODEL = "text-embedding-3-small"
 
 class Memory:
     def __init__(self, embedding_provider, **kwargs):
 
         _embeddings = None
         match embedding_provider:
             case "ollama":
@@ -14,15 +14,15 @@
                 from langchain_openai import OpenAIEmbeddings
                 _embeddings = OpenAIEmbeddings(model=os.environ.get("OPENAI_EMBEDDING_MODEL", "custom"),
                                                    openai_api_key=os.environ.get("OPENAI_API_KEY", "custom"), 
                                                    openai_api_base=os.environ.get("OPENAI_BASE_URL", "http://localhost:1234/v1"), #default for lmstudio
                                                    check_embedding_ctx_length=False) #quick fix for lmstudio
             case "openai":
                 from langchain_openai import OpenAIEmbeddings
-                _embeddings = OpenAIEmbeddings(model="text-embedding-3-small")
+                _embeddings = OpenAIEmbeddings(model=OPENAI_EMBEDDING_MODEL)
             case "azureopenai":
                 from langchain_openai import AzureOpenAIEmbeddings
                 _embeddings = AzureOpenAIEmbeddings(deployment=os.environ["AZURE_EMBEDDING_MODEL"], chunk_size=16)
             case "huggingface":
                 from langchain.embeddings import HuggingFaceEmbeddings
                 _embeddings = HuggingFaceEmbeddings()
```

### Comparing `gpt-researcher-0.6.0/gpt_researcher/retrievers/bing/bing.py` & `gpt-researcher-0.6.1/gpt_researcher/retrievers/bing/bing.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.6.0/gpt_researcher/retrievers/google/google.py` & `gpt-researcher-0.6.1/gpt_researcher/retrievers/google/google.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.6.0/gpt_researcher/retrievers/searx/searx.py` & `gpt-researcher-0.6.1/gpt_researcher/retrievers/searx/searx.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.6.0/gpt_researcher/retrievers/serpapi/serpapi.py` & `gpt-researcher-0.6.1/gpt_researcher/retrievers/serpapi/serpapi.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.6.0/gpt_researcher/retrievers/serper/serper.py` & `gpt-researcher-0.6.1/gpt_researcher/retrievers/serper/serper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.6.0/gpt_researcher/retrievers/tavily_search/tavily_search.py` & `gpt-researcher-0.6.1/gpt_researcher/retrievers/tavily_search/tavily_search.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.6.0/gpt_researcher/scraper/arxiv/arxiv.py` & `gpt-researcher-0.6.1/gpt_researcher/scraper/arxiv/arxiv.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.6.0/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py` & `gpt-researcher-0.6.1/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.6.0/gpt_researcher/scraper/newspaper/newspaper.py` & `gpt-researcher-0.6.1/gpt_researcher/scraper/newspaper/newspaper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.6.0/gpt_researcher/scraper/pymupdf/pymupdf.py` & `gpt-researcher-0.6.1/gpt_researcher/scraper/pymupdf/pymupdf.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.6.0/gpt_researcher/scraper/scraper.py` & `gpt-researcher-0.6.1/gpt_researcher/scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.6.0/gpt_researcher/scraper/web_base_loader/web_base_loader.py` & `gpt-researcher-0.6.1/gpt_researcher/scraper/web_base_loader/web_base_loader.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.6.0/gpt_researcher/utils/llm.py` & `gpt-researcher-0.6.1/gpt_researcher/utils/llm.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from colorama import Fore, Style
 from fastapi import WebSocket
 from langchain.output_parsers import PydanticOutputParser
 from langchain.prompts import PromptTemplate
 
 from gpt_researcher.master.prompts import auto_agent_instructions, generate_subtopics_prompt
-
+from .costs import estimate_llm_cost
 from .validators import Subtopics
 
 
 def get_provider(llm_provider):
     match llm_provider:
         case "openai":
             from ..llm_provider import OpenAIProvider
@@ -56,24 +56,26 @@
         messages: list,  # type: ignore
         model: Optional[str] = None,
         temperature: float = 1.0,
         max_tokens: Optional[int] = None,
         llm_provider: Optional[str] = None,
         stream: Optional[bool] = False,
         websocket: WebSocket | None = None,
+        cost_callback: callable = None
 ) -> str:
     """Create a chat completion using the OpenAI API
     Args:
         messages (list[dict[str, str]]): The messages to send to the chat completion
         model (str, optional): The model to use. Defaults to None.
         temperature (float, optional): The temperature to use. Defaults to 0.9.
         max_tokens (int, optional): The max tokens to use. Defaults to None.
         stream (bool, optional): Whether to stream the response. Defaults to False.
         llm_provider (str, optional): The LLM Provider to use.
-        webocket (WebSocket): The websocket used in the currect request
+        webocket (WebSocket): The websocket used in the currect request,
+        cost_callback: Callback function for updating cost
     Returns:
         str: The response from the chat completion
     """
 
     # validate input
     if model is None:
         raise ValueError("Model cannot be None")
@@ -85,51 +87,29 @@
     ProviderClass = get_provider(llm_provider)
     provider = ProviderClass(
         model,
         temperature,
         max_tokens
     )
 
+    response = ""
     # create response
     for _ in range(10):  # maximum of 10 attempts
         response = await provider.get_chat_response(
             messages, stream, websocket
         )
-        return response
 
-    logging.error("Failed to get response from OpenAI API")
-    raise RuntimeError("Failed to get response from OpenAI API")
+        if cost_callback:
+            llm_costs = estimate_llm_cost(str(messages), response)
+            cost_callback(llm_costs)
 
+        return response
 
-def choose_agent(smart_llm_model: str, llm_provider: str, task: str) -> dict:
-    """Determines what server should be used
-    Args:
-        task (str): The research question the user asked
-        smart_llm_model (str): the llm model to be used
-        llm_provider (str): the llm provider used
-    Returns:
-        server - The server that will be used
-        agent_role_prompt (str): The prompt for the server
-    """
-    try:
-        response = create_chat_completion(
-            model=smart_llm_model,
-            messages=[
-                {"role": "system", "content": f"{auto_agent_instructions()}"},
-                {"role": "user", "content": f"task: {task}"}],
-            temperature=0,
-            llm_provider=llm_provider
-        )
-        agent_dict = json.loads(response)
-        print(f"Agent: {agent_dict.get('server')}")
-        return agent_dict
-    except Exception as e:
-        print(f"{Fore.RED}Error in choose_agent: {e}{Style.RESET_ALL}")
-        return {"server": "Default Agent",
-                "agent_role_prompt": "You are an AI critical thinker research assistant. Your sole purpose is to write well written, critically acclaimed, objective and structured reports on given text."}
+    logging.error(f"Failed to get response from {llm_provider} API")
+    raise RuntimeError(f"Failed to get response from {llm_provider} API")
 
 
 async def construct_subtopics(task: str, data: str, config, subtopics: list = []) -> list:
     try:
         parser = PydanticOutputParser(pydantic_object=Subtopics)
 
         prompt = PromptTemplate(
```

### Comparing `gpt-researcher-0.6.0/gpt_researcher.egg-info/PKG-INFO` & `gpt-researcher-0.6.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,15 @@
-Metadata-Version: 2.1
-Name: gpt-researcher
-Version: 0.6.0
-Summary: GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.
-Home-page: https://github.com/assafelovic/gpt-researcher
-Author: Assaf Elovic
-Author-email: assaf.elovic@gmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <h1 style="display: flex; align-items: center; gap: 10px;">
   <img src="https://github.com/assafelovic/gpt-researcher/assets/13554167/a45bac7c-092c-42e5-8eb6-69acbf20dde5" alt="Logo" width="25">
   GPT Researcher
 </h1>
 
 [![Official Website](https://img.shields.io/badge/Official%20Website-gptr.dev-teal?style=for-the-badge&logo=world&logoColor=white)](https://gptr.dev)
 [![Official Website](https://img.shields.io/badge/Documentation-GPTR-pink?logo=googledocs&logoColor=white&style=for-the-badge)](https://docs.gptr.dev)
-[![Discord Follow](https://dcbadge.vercel.app/api/server/SK3KKuSD?style=for-the-badge)](https://discord.gg/SK3KKuSD)
+[![Discord Follow](https://dcbadge.vercel.app/api/server/cPhHPZ6Z?style=for-the-badge)](https://discord.gg/cPhHPZ6Z)
 
 [![GitHub Repo stars](https://img.shields.io/github/stars/assafelovic/gpt-researcher?style=social)](https://github.com/assafelovic/gpt-researcher)
 [![Twitter Follow](https://img.shields.io/twitter/follow/assaf_elovic?style=social)](https://twitter.com/assaf_elovic)
 [![PyPI version](https://badge.fury.io/py/gpt-researcher.svg)](https://badge.fury.io/py/gpt-researcher)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/assafelovic/gpt-researcher/blob/master/examples/pip-run.ipynb)
 
 <!-- MARKDOWN LINKS & IMAGES -->
```

### Comparing `gpt-researcher-0.6.0/gpt_researcher.egg-info/SOURCES.txt` & `gpt-researcher-0.6.1/gpt_researcher.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 gpt_researcher/llm_provider/ollama/__init__.py
 gpt_researcher/llm_provider/ollama/ollama.py
 gpt_researcher/llm_provider/openai/__init__.py
 gpt_researcher/llm_provider/openai/openai.py
 gpt_researcher/llm_provider/together/__init__.py
 gpt_researcher/llm_provider/together/together.py
 gpt_researcher/master/__init__.py
+gpt_researcher/master/actions.py
 gpt_researcher/master/agent.py
-gpt_researcher/master/functions.py
 gpt_researcher/master/prompts.py
 gpt_researcher/memory/__init__.py
 gpt_researcher/memory/embeddings.py
 gpt_researcher/retrievers/__init__.py
 gpt_researcher/retrievers/bing/__init__.py
 gpt_researcher/retrievers/bing/bing.py
 gpt_researcher/retrievers/duckduckgo/__init__.py
@@ -73,10 +73,11 @@
 gpt_researcher/scraper/newspaper/__init__.py
 gpt_researcher/scraper/newspaper/newspaper.py
 gpt_researcher/scraper/pymupdf/__init__.py
 gpt_researcher/scraper/pymupdf/pymupdf.py
 gpt_researcher/scraper/web_base_loader/__init__.py
 gpt_researcher/scraper/web_base_loader/web_base_loader.py
 gpt_researcher/utils/__init__.py
+gpt_researcher/utils/costs.py
 gpt_researcher/utils/enum.py
 gpt_researcher/utils/llm.py
 gpt_researcher/utils/validators.py
```

### Comparing `gpt-researcher-0.6.0/pyproject.toml` & `gpt-researcher-0.6.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "gpt-researcher"
-version = "0.0.5"
+version = "0.6.1"
 description = "GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks."
-authors = ["Tavily <support@tavily.com>"]
+authors = ["Assaf Elovic <assaf.elovic@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 beautifulsoup4 = ">=4.12.2"
 colorama = ">=0.4.6"
@@ -17,30 +17,31 @@
 python-dotenv = ">=1.0.0"
 pyyaml = ">=6.0.1"
 uvicorn = ">=0.24.0.post1"
 pydantic = ">=2.5.1"
 fastapi = ">=0.104.1"
 python-multipart = ">=0.0.6"
 markdown = ">=3.5.1"
-langchain = ">=0.0.350"
-langgraph = ">=0.0.29"
+langchain = "^0.2"
+langgraph = ">=0.0.29,<0.1"
+langchain_community = "^0.2"
+langchain-openai = "^0.1"
+langchain-google-genai = "^1"
 tavily-python = ">=0.2.8"
 permchain = ">=0.0.6"
 arxiv = ">=2.0.0"
 PyMuPDF = ">=1.23.6"
 requests = ">=2.31.0"
 jinja2 = ">=3.1.2"
 aiofiles = ">=23.2.1"
 newspaper3k = ">=0.2.8"
-langchain_community = ">=0.0.28"
 SQLAlchemy = ">=2.0.28"
 mistune = "^3.0.2"
 htmldocx = "^0.0.6"
 python-docx = "^1.1.0"
-langchain-openai = "^0.1.1"
-langchain-google-genai = "^0.0.11"
 lxml = { version = ">=4.9.2", extras = ["html_clean"] }
 unstructured = "^0.13.0"
+tiktoken = ">=0.7.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `gpt-researcher-0.6.0/setup.py` & `gpt-researcher-0.6.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt", "r") as f:
     reqs = [line.strip() for line in f if ('selenium' not in line and 'webdriver' not in line)]
 
 setup(
     name="gpt-researcher",
-    version="0.6.0",
+    version="0.6.1",
     description="GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.",
     package_dir={'gpt_researcher': 'gpt_researcher'},
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/assafelovic/gpt-researcher",
     author="Assaf Elovic",
```

