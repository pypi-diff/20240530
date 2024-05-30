# Comparing `tmp/autorag-0.2.1.tar.gz` & `tmp/autorag-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autorag-0.2.1.tar", last modified: Tue May 28 05:00:42 2024, max compression
+gzip compressed data, was "autorag-0.2.2.tar", last modified: Thu May 30 03:02:50 2024, max compression
```

## Comparing `autorag-0.2.1.tar` & `autorag-0.2.2.tar`

### file list

```diff
@@ -1,544 +1,544 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.700013 autorag-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.612012 autorag-0.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-28 05:00:31.000000 autorag-0.2.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.616012 autorag-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-28 05:00:31.000000 autorag-0.2.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-28 05:00:31.000000 autorag-0.2.1/.github/workflows/sphinx.yml
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-28 05:00:31.000000 autorag-0.2.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-28 05:00:31.000000 autorag-0.2.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.700013 autorag-0.2.1/AutoRAG.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    25129 2024-05-28 05:00:42.000000 autorag-0.2.1/AutoRAG.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21167 2024-05-28 05:00:42.000000 autorag-0.2.1/AutoRAG.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 05:00:42.000000 autorag-0.2.1/AutoRAG.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 05:00:42.000000 autorag-0.2.1/AutoRAG.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-28 05:00:42.000000 autorag-0.2.1/AutoRAG.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-28 05:00:42.000000 autorag-0.2.1/AutoRAG.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-28 05:00:31.000000 autorag-0.2.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-05-28 05:00:31.000000 autorag-0.2.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-28 05:00:31.000000 autorag-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    25129 2024-05-28 05:00:42.700013 autorag-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-05-28 05:00:31.000000 autorag-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.616012 autorag-0.2.1/autorag/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.616012 autorag-0.2.1/autorag/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.620013 autorag-0.2.1/autorag/data/corpus/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/data/corpus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/data/corpus/langchain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/data/corpus/llama_index.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.620013 autorag-0.2.1/autorag/data/qacreation/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/data/qacreation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/data/qacreation/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/data/qacreation/llama_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/data/qacreation/llama_index_default_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/data/qacreation/ragas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/data/qacreation/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.620013 autorag-0.2.1/autorag/data/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/data/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/data/utils/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     8871 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/deploy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.620013 autorag-0.2.1/autorag/evaluate/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/evaluate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/evaluate/generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.620013 autorag-0.2.1/autorag/evaluate/metric/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/evaluate/metric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.624013 autorag-0.2.1/autorag/evaluate/metric/g_eval_prompts/
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/evaluate/metric/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/evaluate/metric/retrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/evaluate/metric/retrieval_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/evaluate/metric/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/evaluate/retrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/evaluate/retrieval_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/evaluate/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    17782 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/node_line.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.624013 autorag-0.2.1/autorag/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.624013 autorag-0.2.1/autorag/nodes/generator/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/generator/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/generator/llama_index_llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/generator/openai_llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/generator/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/generator/vllm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.624013 autorag-0.2.1/autorag/nodes/passageaugmenter/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passageaugmenter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passageaugmenter/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passageaugmenter/pass_passage_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passageaugmenter/prev_next_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passageaugmenter/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.624013 autorag-0.2.1/autorag/nodes/passagecompressor/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagecompressor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagecompressor/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagecompressor/longllmlingua.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagecompressor/pass_compressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagecompressor/refine.py
--rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagecompressor/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagecompressor/tree_summarize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.628013 autorag-0.2.1/autorag/nodes/passagefilter/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagefilter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagefilter/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagefilter/pass_passage_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagefilter/percentile_cutoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagefilter/recency.py
--rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagefilter/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagefilter/similarity_percentile_cutoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagefilter/similarity_threshold_cutoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagefilter/threshold_cutoff.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.628013 autorag-0.2.1/autorag/nodes/passagereranker/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/colbert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/flag_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/flag_embedding_llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/jina.py
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/koreranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/monot5.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/pass_reranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/rankgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/sentence_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.632012 autorag-0.2.1/autorag/nodes/passagereranker/tart/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/tart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/tart/modeling_enc_t5.py
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/tart/tart.py
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/time_reranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     5799 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/upr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.632012 autorag-0.2.1/autorag/nodes/promptmaker/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/promptmaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/promptmaker/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/promptmaker/fstring.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/promptmaker/long_context_reorder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9455 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/promptmaker/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.632012 autorag-0.2.1/autorag/nodes/queryexpansion/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/queryexpansion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/queryexpansion/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/queryexpansion/hyde.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/queryexpansion/multi_query_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/queryexpansion/pass_query_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/queryexpansion/query_decompose.py
--rw-r--r--   0 runner    (1001) docker     (127)     8330 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/queryexpansion/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.632012 autorag-0.2.1/autorag/nodes/retrieval/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/retrieval/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/retrieval/bm25.py
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/retrieval/hybrid_cc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/retrieval/hybrid_dbsf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/retrieval/hybrid_rrf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/retrieval/hybrid_rsf.py
--rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/retrieval/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/retrieval/vectordb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.636013 autorag-0.2.1/autorag/schema/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/schema/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/schema/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.636013 autorag-0.2.1/autorag/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/utils/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)    15273 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/utils/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/web.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.636013 autorag-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.636013 autorag-0.2.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.640013 autorag-0.2.1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    57124 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/data_creation.png
--rw-r--r--   0 runner    (1001) docker     (127)    30770 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/data_folder.png
--rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/dcg.png
--rw-r--r--   0 runner    (1001) docker     (127)     9212 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/f1_score.png
--rw-r--r--   0 runner    (1001) docker     (127)    38900 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/map.png
--rw-r--r--   0 runner    (1001) docker     (127)    45576 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/mrr.png
--rw-r--r--   0 runner    (1001) docker     (127)    81810 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/ndcg.png
--rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/ndcg_formula.png
--rw-r--r--   0 runner    (1001) docker     (127)    31538 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/node_folder.png
--rw-r--r--   0 runner    (1001) docker     (127)    18941 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/node_line_folder.png
--rw-r--r--   0 runner    (1001) docker     (127)    42589 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/node_line_summary.png
--rw-r--r--   0 runner    (1001) docker     (127)    92939 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/node_lines.png
--rw-r--r--   0 runner    (1001) docker     (127)    95669 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/node_summary.png
--rw-r--r--   0 runner    (1001) docker     (127)    36728 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/project_folder_example.png
--rw-r--r--   0 runner    (1001) docker     (127)    19853 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/project_folders.png
--rw-r--r--   0 runner    (1001) docker     (127)    22432 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/resources_folder.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.644013 autorag-0.2.1/docs/source/_static/roadmap/
--rw-r--r--   0 runner    (1001) docker     (127)   159068 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/roadmap/RAG_paradigms.png
--rw-r--r--   0 runner    (1001) docker     (127)    38568 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/roadmap/advanced_RAG.png
--rw-r--r--   0 runner    (1001) docker     (127)    62853 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/roadmap/cycle.png
--rw-r--r--   0 runner    (1001) docker     (127)    75826 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/roadmap/merger.png
--rw-r--r--   0 runner    (1001) docker     (127)    82200 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/roadmap/node_line_modular.png
--rw-r--r--   0 runner    (1001) docker     (127)    69999 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/roadmap/policy.png
--rw-r--r--   0 runner    (1001) docker     (127)   567356 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/samsung_sundae.jpeg
--rw-r--r--   0 runner    (1001) docker     (127)    37348 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/trial_folder.png
--rw-r--r--   0 runner    (1001) docker     (127)    25499 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/trial_json.png
--rw-r--r--   0 runner    (1001) docker     (127)   177107 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/trial_summary.png
--rw-r--r--   0 runner    (1001) docker     (127)   269046 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/web_interface.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.644013 autorag-0.2.1/docs/source/api_spec/
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.data.corpus.rst
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.data.qacreation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.data.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.evaluate.metric.rst
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.evaluate.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.nodes.generator.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.nodes.passageaugmenter.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.nodes.passagecompressor.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.nodes.passagefilter.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.nodes.passagereranker.rst
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.nodes.promptmaker.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.nodes.queryexpansion.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.nodes.retrieval.rst
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.nodes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.rst
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.schema.rst
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.648012 autorag-0.2.1/docs/source/data_creation/
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/data_creation/data_format.md
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/data_creation/ragas.md
--rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/data_creation/tutorial.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.648012 autorag-0.2.1/docs/source/deploy/
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/deploy/api_endpoint.md
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/deploy/web.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.648012 autorag-0.2.1/docs/source/evaluate_metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/evaluate_metrics/generation.md
--rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/evaluate_metrics/retrieval.md
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/evaluate_metrics/retrieval_contents.md
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/install.md
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/local_model.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.648012 autorag-0.2.1/docs/source/nodes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.648012 autorag-0.2.1/docs/source/nodes/generator/
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/generator/generator.md
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/generator/llama_index_llm.md
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/generator/openai_llm.md
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/generator/vllm.md
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.648012 autorag-0.2.1/docs/source/nodes/passage_augmenter/
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_augmenter/passage_augmenter.md
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_augmenter/prev_next_augmenter.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.648012 autorag-0.2.1/docs/source/nodes/passage_compressor/
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_compressor/longllmlingua.md
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_compressor/passage_compressor.md
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_compressor/refine.md
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_compressor/tree_summarize.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.648012 autorag-0.2.1/docs/source/nodes/passage_filter/
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_filter/passage_filter.md
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_filter/percentile_cutoff.md
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_filter/recency_filter.md
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_filter/threshold_cutoff.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.652013 autorag-0.2.1/docs/source/nodes/passage_reranker/
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_reranker/cohere.md
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_reranker/colbert.md
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_reranker/flag_embedding_reranker.md
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_reranker/jina_reranker.md
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_reranker/koreranker.md
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_reranker/monot5.md
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_reranker/passage_reranker.md
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_reranker/rankgpt.md
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_reranker/tart.md
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_reranker/time_reranker.md
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_reranker/upr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.652013 autorag-0.2.1/docs/source/nodes/prompt_maker/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/prompt_maker/fstring.md
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/prompt_maker/long_context_reorder.md
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/prompt_maker/prompt_maker.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.652013 autorag-0.2.1/docs/source/nodes/query_expansion/
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/query_expansion/hyde.md
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/query_expansion/multi_query_expansion.md
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/query_expansion/query_decompose.md
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/query_expansion/query_expansion.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.656013 autorag-0.2.1/docs/source/nodes/retrieval/
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/retrieval/bm25.md
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/retrieval/hybrid_cc.md
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/retrieval/hybrid_dbsf.md
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/retrieval/hybrid_rrf.md
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/retrieval/hybrid_rsf.md
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/retrieval/retrieval.md
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/retrieval/vectordb.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.656013 autorag-0.2.1/docs/source/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/optimization/custom_config.md
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/optimization/folder_structure.md
--rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/optimization/optimization.md
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/optimization/sample_full_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/optimization/strategies.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.656013 autorag-0.2.1/docs/source/roadmap/
--rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/roadmap/modular_rag.md
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/structure.md
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/troubleshooting.md
--rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/tutorial.md
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-28 05:00:31.000000 autorag-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-28 05:00:31.000000 autorag-0.2.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.656013 autorag-0.2.1/sample_config/
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-28 05:00:31.000000 autorag-0.2.1/sample_config/compact_local.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-28 05:00:31.000000 autorag-0.2.1/sample_config/compact_openai.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-28 05:00:31.000000 autorag-0.2.1/sample_config/config_korean.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-28 05:00:31.000000 autorag-0.2.1/sample_config/extracted_sample.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-05-28 05:00:31.000000 autorag-0.2.1/sample_config/full.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-28 05:00:31.000000 autorag-0.2.1/sample_config/simple_local.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-28 05:00:31.000000 autorag-0.2.1/sample_config/simple_openai.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.656013 autorag-0.2.1/sample_dataset/
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-28 05:00:31.000000 autorag-0.2.1/sample_dataset/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.656013 autorag-0.2.1/sample_dataset/eli5/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-28 05:00:31.000000 autorag-0.2.1/sample_dataset/eli5/load_eli5_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.656013 autorag-0.2.1/sample_dataset/msmarco/
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-28 05:00:31.000000 autorag-0.2.1/sample_dataset/msmarco/load_msmarco_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.656013 autorag-0.2.1/sample_dataset/triviaqa/
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-28 05:00:31.000000 autorag-0.2.1/sample_dataset/triviaqa/load_triviaqa_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 05:00:42.700013 autorag-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.656013 autorag-0.2.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.660013 autorag-0.2.1/tests/autorag/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.604013 autorag-0.2.1/tests/autorag/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.660013 autorag-0.2.1/tests/autorag/data/corpus/
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/data/corpus/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/data/corpus/test_langchain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/data/corpus/test_llama_index_corpus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.660013 autorag-0.2.1/tests/autorag/data/qacreation/
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/data/qacreation/test_base_qacreation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/data/qacreation/test_llama_index_qacreation.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/data/qacreation/test_ragas_qa_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/data/qacreation/test_simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.660013 autorag-0.2.1/tests/autorag/evaluate/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.660013 autorag-0.2.1/tests/autorag/evaluate/metric/
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/evaluate/metric/test_generation_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/evaluate/metric/test_retrieval_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/evaluate/test_evaluate_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/evaluate/test_generation_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/evaluate/test_retrieval_contents_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/evaluate/test_retrieval_evaluate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.608013 autorag-0.2.1/tests/autorag/nodes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.660013 autorag-0.2.1/tests/autorag/nodes/generator/
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/generator/test_generator_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/generator/test_llama_index_llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/generator/test_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/generator/test_run_generator_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/generator/test_vllm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.664013 autorag-0.2.1/tests/autorag/nodes/passageaugmenter/
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passageaugmenter/test_base_passage_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passageaugmenter/test_pass_passage_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passageaugmenter/test_prev_next_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passageaugmenter/test_run_passage_augmenter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.664013 autorag-0.2.1/tests/autorag/nodes/passagecompressor/
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagecompressor/test_longllmlingua.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagecompressor/test_pass_compressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagecompressor/test_refine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagecompressor/test_tree_summarize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.664013 autorag-0.2.1/tests/autorag/nodes/passagefilter/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagefilter/test_passage_filter_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagefilter/test_passage_filter_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagefilter/test_percentile_cutoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagefilter/test_recency_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagefilter/test_similarity_percentile_cutoff.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagefilter/test_similarity_threshold_cutoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagefilter/test_threshold_cutoff.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.668013 autorag-0.2.1/tests/autorag/nodes/passagereranker/
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagereranker/test_cohere_reranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagereranker/test_colbert_reranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagereranker/test_flag_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagereranker/test_jina_reranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagereranker/test_koreranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagereranker/test_monot5.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagereranker/test_pass_reranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagereranker/test_rankgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagereranker/test_sentence_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagereranker/test_tart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagereranker/test_time_reranker.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagereranker/test_upr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.668013 autorag-0.2.1/tests/autorag/nodes/promptmaker/
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/promptmaker/test_fstring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/promptmaker/test_long_context_reorder.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.668013 autorag-0.2.1/tests/autorag/nodes/queryexpansion/
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/queryexpansion/test_hyde.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/queryexpansion/test_multi_query_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/queryexpansion/test_query_decompose.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.668013 autorag-0.2.1/tests/autorag/nodes/retrieval/
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/retrieval/test_bm25.py
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/retrieval/test_hybrid_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/retrieval/test_hybrid_cc.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/retrieval/test_hybrid_rrf.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/retrieval/test_hybrid_rsf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/retrieval/test_retrieval_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11272 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/retrieval/test_run_retrieval_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/retrieval/test_vectordb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.672013 autorag-0.2.1/tests/autorag/schema/
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/schema/test_module_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/schema/test_node_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/test_deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)    15166 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/test_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/test_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/test_support.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/test_web.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.672013 autorag-0.2.1/tests/autorag/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/utils/test_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)    13545 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/utils/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/delete_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.672013 autorag-0.2.1/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   111931 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/corpus_data_sample.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.608013 autorag-0.2.1/tests/resources/data_creation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.672013 autorag-0.2.1/tests/resources/data_creation/raw_dir/
--rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/data_creation/raw_dir/sample1.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/data_creation/raw_dir/sample2.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/data_creation/raw_dir/sample3.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/full.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/qa_data_sample.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.672013 autorag-0.2.1/tests/resources/qa_gen_prompts/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/qa_gen_prompts/prompt1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/qa_gen_prompts/prompt2.txt
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/qa_gen_prompts/prompt3.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/qa_test_data_sample.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.672013 autorag-0.2.1/tests/resources/result_project/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.672013 autorag-0.2.1/tests/resources/result_project/0/
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.672013 autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.676013 autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/generator/
--rw-r--r--   0 runner    (1001) docker     (127)    23516 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    26448 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    33716 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    14618 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    14683 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    13278 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    54234 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.676013 autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/
--rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     8443 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    41557 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.676013 autorag-0.2.1/tests/resources/result_project/0/pre_retrieve_node_line/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.676013 autorag-0.2.1/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    28924 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/summary.csv
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/pre_retrieve_node_line/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.676013 autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.676013 autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/passage_compressor/
--rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    31124 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/passage_compressor/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.680013 autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/passage_reranker/
--rw-r--r--   0 runner    (1001) docker     (127)    67610 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    67719 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    84239 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/passage_reranker/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.680013 autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/retrieval/
--rw-r--r--   0 runner    (1001) docker     (127)   103655 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    86579 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)   117633 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/retrieval/summary.csv
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/summary.csv
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.680013 autorag-0.2.1/tests/resources/result_project/1/
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/1/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.680013 autorag-0.2.1/tests/resources/result_project/1/pre_retrieve_node_line/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.680013 autorag-0.2.1/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    28924 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/summary.csv
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/1/pre_retrieve_node_line/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.608013 autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.680013 autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/passage_filter/
--rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/passage_filter/0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.680013 autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/passage_reranker/
--rw-r--r--   0 runner    (1001) docker     (127)    67610 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    67719 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    84239 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/passage_reranker/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.684013 autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/retrieval/
--rw-r--r--   0 runner    (1001) docker     (127)   103655 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    86579 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)   117633 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/retrieval/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.684013 autorag-0.2.1/tests/resources/result_project/2/
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.612012 autorag-0.2.1/tests/resources/result_project/2/post_retrieve_node_line/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.684013 autorag-0.2.1/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/
--rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.684013 autorag-0.2.1/tests/resources/result_project/2/pre_retrieve_node_line/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.684013 autorag-0.2.1/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    28924 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/summary.csv
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/pre_retrieve_node_line/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.684013 autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.684013 autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/passage_compressor/
--rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    31124 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/passage_compressor/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.684013 autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/passage_reranker/
--rw-r--r--   0 runner    (1001) docker     (127)    67610 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    67719 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    84239 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/passage_reranker/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.688013 autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/retrieval/
--rw-r--r--   0 runner    (1001) docker     (127)   103655 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    86579 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)   117633 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/retrieval/summary.csv
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.688013 autorag-0.2.1/tests/resources/result_project/3/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/3/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/best.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.688013 autorag-0.2.1/tests/resources/result_project/data/
--rw-r--r--   0 runner    (1001) docker     (127)   111931 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/data/corpus.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/data/qa.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.688013 autorag-0.2.1/tests/resources/result_project/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    91651 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/resources/bm25_porter_stemmer.pkl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.688013 autorag-0.2.1/tests/resources/result_project/resources/chroma/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.696013 autorag-0.2.1/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/
--rw-r--r--   0 runner    (1001) docker     (127)  6284000 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/header.bin
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/link_lists.bin
--rw-r--r--   0 runner    (1001) docker     (127)   352256 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/resources/chroma/chroma.sqlite3
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/trial.json
--rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/sample_contents_nqa.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.612012 autorag-0.2.1/tests/resources/sample_project/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.696013 autorag-0.2.1/tests/resources/sample_project/data/
--rw-r--r--   0 runner    (1001) docker     (127)   115302 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/sample_project/data/corpus.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/sample_project/data/qa.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.700013 autorag-0.2.1/tests/resources/sample_project/resources/
--rw-r--r--   0 runner    (1001) docker     (127)   109478 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/sample_project/resources/bm25_gpt2.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    91651 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/sample_project/resources/bm25_porter_stemmer.pkl
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/simple.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    26773 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/test_bm25_retrieval.pkl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.350749 autorag-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.250749 autorag-0.2.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-30 03:02:36.000000 autorag-0.2.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.250749 autorag-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-30 03:02:36.000000 autorag-0.2.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-30 03:02:36.000000 autorag-0.2.2/.github/workflows/sphinx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-30 03:02:36.000000 autorag-0.2.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-30 03:02:36.000000 autorag-0.2.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.350749 autorag-0.2.2/AutoRAG.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    25129 2024-05-30 03:02:50.000000 autorag-0.2.2/AutoRAG.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21167 2024-05-30 03:02:50.000000 autorag-0.2.2/AutoRAG.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 03:02:50.000000 autorag-0.2.2/AutoRAG.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-30 03:02:50.000000 autorag-0.2.2/AutoRAG.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-30 03:02:50.000000 autorag-0.2.2/AutoRAG.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-30 03:02:50.000000 autorag-0.2.2/AutoRAG.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-30 03:02:36.000000 autorag-0.2.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-05-30 03:02:36.000000 autorag-0.2.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-30 03:02:36.000000 autorag-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    25129 2024-05-30 03:02:50.350749 autorag-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-05-30 03:02:36.000000 autorag-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.254749 autorag-0.2.2/autorag/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.254749 autorag-0.2.2/autorag/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.254749 autorag-0.2.2/autorag/data/corpus/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/data/corpus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/data/corpus/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/data/corpus/llama_index.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.258749 autorag-0.2.2/autorag/data/qacreation/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/data/qacreation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/data/qacreation/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/data/qacreation/llama_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/data/qacreation/llama_index_default_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/data/qacreation/ragas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/data/qacreation/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.258749 autorag-0.2.2/autorag/data/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/data/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/data/utils/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8871 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/deploy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.258749 autorag-0.2.2/autorag/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/evaluate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/evaluate/generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.258749 autorag-0.2.2/autorag/evaluate/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/evaluate/metric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.258749 autorag-0.2.2/autorag/evaluate/metric/g_eval_prompts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/evaluate/metric/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/evaluate/metric/retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/evaluate/metric/retrieval_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/evaluate/metric/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/evaluate/retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/evaluate/retrieval_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/evaluate/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17782 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/node_line.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.258749 autorag-0.2.2/autorag/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.262749 autorag-0.2.2/autorag/nodes/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/generator/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/generator/llama_index_llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/generator/openai_llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/generator/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/generator/vllm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.262749 autorag-0.2.2/autorag/nodes/passageaugmenter/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passageaugmenter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passageaugmenter/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passageaugmenter/pass_passage_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passageaugmenter/prev_next_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passageaugmenter/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.262749 autorag-0.2.2/autorag/nodes/passagecompressor/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passagecompressor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passagecompressor/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passagecompressor/longllmlingua.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passagecompressor/pass_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passagecompressor/refine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passagecompressor/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passagecompressor/tree_summarize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.266749 autorag-0.2.2/autorag/nodes/passagefilter/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passagefilter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passagefilter/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passagefilter/pass_passage_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passagefilter/percentile_cutoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passagefilter/recency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passagefilter/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passagefilter/similarity_percentile_cutoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passagefilter/similarity_threshold_cutoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passagefilter/threshold_cutoff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.266749 autorag-0.2.2/autorag/nodes/passagereranker/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passagereranker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passagereranker/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passagereranker/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passagereranker/colbert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passagereranker/flag_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passagereranker/flag_embedding_llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passagereranker/jina.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passagereranker/koreranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passagereranker/monot5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passagereranker/pass_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passagereranker/rankgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passagereranker/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passagereranker/sentence_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.270749 autorag-0.2.2/autorag/nodes/passagereranker/tart/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passagereranker/tart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passagereranker/tart/modeling_enc_t5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passagereranker/tart/tart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passagereranker/time_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5799 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/passagereranker/upr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.270749 autorag-0.2.2/autorag/nodes/promptmaker/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/promptmaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/promptmaker/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/promptmaker/fstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/promptmaker/long_context_reorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9455 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/promptmaker/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.270749 autorag-0.2.2/autorag/nodes/queryexpansion/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/queryexpansion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/queryexpansion/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/queryexpansion/hyde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/queryexpansion/multi_query_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/queryexpansion/pass_query_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/queryexpansion/query_decompose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8330 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/queryexpansion/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.274749 autorag-0.2.2/autorag/nodes/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/retrieval/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/retrieval/bm25.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/retrieval/hybrid_cc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/retrieval/hybrid_dbsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/retrieval/hybrid_rrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/retrieval/hybrid_rsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/retrieval/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/nodes/retrieval/vectordb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.274749 autorag-0.2.2/autorag/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/schema/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/schema/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.274749 autorag-0.2.2/autorag/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/utils/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15360 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/utils/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-30 03:02:36.000000 autorag-0.2.2/autorag/web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.274749 autorag-0.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.274749 autorag-0.2.2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.282749 autorag-0.2.2/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    57124 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/_static/data_creation.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30770 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/_static/data_folder.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/_static/dcg.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9212 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/_static/f1_score.png
+-rw-r--r--   0 runner    (1001) docker     (127)    38900 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/_static/map.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45576 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/_static/mrr.png
+-rw-r--r--   0 runner    (1001) docker     (127)    81810 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/_static/ndcg.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/_static/ndcg_formula.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31538 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/_static/node_folder.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18941 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/_static/node_line_folder.png
+-rw-r--r--   0 runner    (1001) docker     (127)    42589 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/_static/node_line_summary.png
+-rw-r--r--   0 runner    (1001) docker     (127)    92939 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/_static/node_lines.png
+-rw-r--r--   0 runner    (1001) docker     (127)    95669 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/_static/node_summary.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36728 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/_static/project_folder_example.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19853 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/_static/project_folders.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22432 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/_static/resources_folder.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.286749 autorag-0.2.2/docs/source/_static/roadmap/
+-rw-r--r--   0 runner    (1001) docker     (127)   159068 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/_static/roadmap/RAG_paradigms.png
+-rw-r--r--   0 runner    (1001) docker     (127)    38568 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/_static/roadmap/advanced_RAG.png
+-rw-r--r--   0 runner    (1001) docker     (127)    62853 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/_static/roadmap/cycle.png
+-rw-r--r--   0 runner    (1001) docker     (127)    75826 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/_static/roadmap/merger.png
+-rw-r--r--   0 runner    (1001) docker     (127)    82200 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/_static/roadmap/node_line_modular.png
+-rw-r--r--   0 runner    (1001) docker     (127)    69999 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/_static/roadmap/policy.png
+-rw-r--r--   0 runner    (1001) docker     (127)   567356 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/_static/samsung_sundae.jpeg
+-rw-r--r--   0 runner    (1001) docker     (127)    37348 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/_static/trial_folder.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25499 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/_static/trial_json.png
+-rw-r--r--   0 runner    (1001) docker     (127)   177107 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/_static/trial_summary.png
+-rw-r--r--   0 runner    (1001) docker     (127)   269046 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/_static/web_interface.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.290749 autorag-0.2.2/docs/source/api_spec/
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/api_spec/autorag.data.corpus.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/api_spec/autorag.data.qacreation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/api_spec/autorag.data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/api_spec/autorag.data.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/api_spec/autorag.evaluate.metric.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/api_spec/autorag.evaluate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/api_spec/autorag.nodes.generator.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/api_spec/autorag.nodes.passageaugmenter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/api_spec/autorag.nodes.passagecompressor.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/api_spec/autorag.nodes.passagefilter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/api_spec/autorag.nodes.passagereranker.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/api_spec/autorag.nodes.promptmaker.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/api_spec/autorag.nodes.queryexpansion.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/api_spec/autorag.nodes.retrieval.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/api_spec/autorag.nodes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/api_spec/autorag.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/api_spec/autorag.schema.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/api_spec/autorag.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/api_spec/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.290749 autorag-0.2.2/docs/source/data_creation/
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/data_creation/data_format.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/data_creation/ragas.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/data_creation/tutorial.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.290749 autorag-0.2.2/docs/source/deploy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/deploy/api_endpoint.md
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/deploy/web.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.290749 autorag-0.2.2/docs/source/evaluate_metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/evaluate_metrics/generation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/evaluate_metrics/retrieval.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/evaluate_metrics/retrieval_contents.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/install.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/local_model.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.290749 autorag-0.2.2/docs/source/nodes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.290749 autorag-0.2.2/docs/source/nodes/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/generator/generator.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/generator/llama_index_llm.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/generator/openai_llm.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/generator/vllm.md
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.290749 autorag-0.2.2/docs/source/nodes/passage_augmenter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/passage_augmenter/passage_augmenter.md
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/passage_augmenter/prev_next_augmenter.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.290749 autorag-0.2.2/docs/source/nodes/passage_compressor/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/passage_compressor/longllmlingua.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/passage_compressor/passage_compressor.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/passage_compressor/refine.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/passage_compressor/tree_summarize.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.294749 autorag-0.2.2/docs/source/nodes/passage_filter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/passage_filter/passage_filter.md
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/passage_filter/percentile_cutoff.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/passage_filter/recency_filter.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/passage_filter/threshold_cutoff.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.294749 autorag-0.2.2/docs/source/nodes/passage_reranker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/passage_reranker/cohere.md
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/passage_reranker/colbert.md
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/passage_reranker/flag_embedding_reranker.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/passage_reranker/jina_reranker.md
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/passage_reranker/koreranker.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/passage_reranker/monot5.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/passage_reranker/passage_reranker.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/passage_reranker/rankgpt.md
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/passage_reranker/tart.md
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/passage_reranker/time_reranker.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/passage_reranker/upr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.294749 autorag-0.2.2/docs/source/nodes/prompt_maker/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/prompt_maker/fstring.md
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/prompt_maker/long_context_reorder.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/prompt_maker/prompt_maker.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.294749 autorag-0.2.2/docs/source/nodes/query_expansion/
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/query_expansion/hyde.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/query_expansion/multi_query_expansion.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/query_expansion/query_decompose.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/query_expansion/query_expansion.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.298749 autorag-0.2.2/docs/source/nodes/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/retrieval/bm25.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/retrieval/hybrid_cc.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/retrieval/hybrid_dbsf.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/retrieval/hybrid_rrf.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/retrieval/hybrid_rsf.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/retrieval/retrieval.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/nodes/retrieval/vectordb.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.298749 autorag-0.2.2/docs/source/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/optimization/custom_config.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/optimization/folder_structure.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/optimization/optimization.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/optimization/sample_full_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/optimization/strategies.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.298749 autorag-0.2.2/docs/source/roadmap/
+-rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/roadmap/modular_rag.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/structure.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/troubleshooting.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-05-30 03:02:36.000000 autorag-0.2.2/docs/source/tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-30 03:02:36.000000 autorag-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-30 03:02:36.000000 autorag-0.2.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.298749 autorag-0.2.2/sample_config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-30 03:02:36.000000 autorag-0.2.2/sample_config/compact_local.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-30 03:02:36.000000 autorag-0.2.2/sample_config/compact_openai.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-30 03:02:36.000000 autorag-0.2.2/sample_config/config_korean.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-30 03:02:36.000000 autorag-0.2.2/sample_config/extracted_sample.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-05-30 03:02:36.000000 autorag-0.2.2/sample_config/full.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-30 03:02:36.000000 autorag-0.2.2/sample_config/simple_local.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-30 03:02:36.000000 autorag-0.2.2/sample_config/simple_openai.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.298749 autorag-0.2.2/sample_dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-30 03:02:36.000000 autorag-0.2.2/sample_dataset/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.298749 autorag-0.2.2/sample_dataset/eli5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-30 03:02:36.000000 autorag-0.2.2/sample_dataset/eli5/load_eli5_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.298749 autorag-0.2.2/sample_dataset/msmarco/
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-30 03:02:36.000000 autorag-0.2.2/sample_dataset/msmarco/load_msmarco_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.302749 autorag-0.2.2/sample_dataset/triviaqa/
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-30 03:02:36.000000 autorag-0.2.2/sample_dataset/triviaqa/load_triviaqa_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 03:02:50.350749 autorag-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.302749 autorag-0.2.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.302749 autorag-0.2.2/tests/autorag/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.242749 autorag-0.2.2/tests/autorag/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.302749 autorag-0.2.2/tests/autorag/data/corpus/
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/data/corpus/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/data/corpus/test_langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/data/corpus/test_llama_index_corpus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.302749 autorag-0.2.2/tests/autorag/data/qacreation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/data/qacreation/test_base_qacreation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/data/qacreation/test_llama_index_qacreation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/data/qacreation/test_ragas_qa_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/data/qacreation/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.302749 autorag-0.2.2/tests/autorag/evaluate/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.306749 autorag-0.2.2/tests/autorag/evaluate/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/evaluate/metric/test_generation_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/evaluate/metric/test_retrieval_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/evaluate/test_evaluate_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/evaluate/test_generation_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/evaluate/test_retrieval_contents_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/evaluate/test_retrieval_evaluate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.242749 autorag-0.2.2/tests/autorag/nodes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.306749 autorag-0.2.2/tests/autorag/nodes/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/nodes/generator/test_generator_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/nodes/generator/test_llama_index_llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/nodes/generator/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/nodes/generator/test_run_generator_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/nodes/generator/test_vllm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.306749 autorag-0.2.2/tests/autorag/nodes/passageaugmenter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/nodes/passageaugmenter/test_base_passage_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/nodes/passageaugmenter/test_pass_passage_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/nodes/passageaugmenter/test_prev_next_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/nodes/passageaugmenter/test_run_passage_augmenter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.306749 autorag-0.2.2/tests/autorag/nodes/passagecompressor/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/nodes/passagecompressor/test_longllmlingua.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/nodes/passagecompressor/test_pass_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/nodes/passagecompressor/test_refine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/nodes/passagecompressor/test_tree_summarize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.310749 autorag-0.2.2/tests/autorag/nodes/passagefilter/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/nodes/passagefilter/test_passage_filter_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/nodes/passagefilter/test_passage_filter_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/nodes/passagefilter/test_percentile_cutoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/nodes/passagefilter/test_recency_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/nodes/passagefilter/test_similarity_percentile_cutoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/nodes/passagefilter/test_similarity_threshold_cutoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/nodes/passagefilter/test_threshold_cutoff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.310749 autorag-0.2.2/tests/autorag/nodes/passagereranker/
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/nodes/passagereranker/test_cohere_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/nodes/passagereranker/test_colbert_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-30 03:02:36.000000 autorag-0.2.2/tests/autorag/nodes/passagereranker/test_flag_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/nodes/passagereranker/test_jina_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/nodes/passagereranker/test_koreranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/nodes/passagereranker/test_monot5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/nodes/passagereranker/test_pass_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/nodes/passagereranker/test_rankgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/nodes/passagereranker/test_sentence_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/nodes/passagereranker/test_tart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/nodes/passagereranker/test_time_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/nodes/passagereranker/test_upr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.314749 autorag-0.2.2/tests/autorag/nodes/promptmaker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/nodes/promptmaker/test_fstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/nodes/promptmaker/test_long_context_reorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.314749 autorag-0.2.2/tests/autorag/nodes/queryexpansion/
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/nodes/queryexpansion/test_hyde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/nodes/queryexpansion/test_multi_query_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/nodes/queryexpansion/test_query_decompose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.314749 autorag-0.2.2/tests/autorag/nodes/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/nodes/retrieval/test_bm25.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/nodes/retrieval/test_hybrid_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/nodes/retrieval/test_hybrid_cc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/nodes/retrieval/test_hybrid_rrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/nodes/retrieval/test_hybrid_rsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/nodes/retrieval/test_retrieval_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11272 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/nodes/retrieval/test_run_retrieval_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/nodes/retrieval/test_vectordb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.314749 autorag-0.2.2/tests/autorag/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/schema/test_module_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/schema/test_node_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/test_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15166 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/test_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/test_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/test_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.318749 autorag-0.2.2/tests/autorag/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/utils/test_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13545 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/autorag/utils/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/delete_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.318749 autorag-0.2.2/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   111931 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/corpus_data_sample.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.242749 autorag-0.2.2/tests/resources/data_creation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.318749 autorag-0.2.2/tests/resources/data_creation/raw_dir/
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/data_creation/raw_dir/sample1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/data_creation/raw_dir/sample2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/data_creation/raw_dir/sample3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/full.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/qa_data_sample.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.318749 autorag-0.2.2/tests/resources/qa_gen_prompts/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/qa_gen_prompts/prompt1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/qa_gen_prompts/prompt2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/qa_gen_prompts/prompt3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/qa_test_data_sample.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.318749 autorag-0.2.2/tests/resources/result_project/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.318749 autorag-0.2.2/tests/resources/result_project/0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/0/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.322749 autorag-0.2.2/tests/resources/result_project/0/post_retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.322749 autorag-0.2.2/tests/resources/result_project/0/post_retrieve_node_line/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)    23516 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    26448 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    33716 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    14618 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    14683 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    13278 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    54234 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.322749 autorag-0.2.2/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/
+-rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     8443 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    41557 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/0/post_retrieve_node_line/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.322749 autorag-0.2.2/tests/resources/result_project/0/pre_retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.326749 autorag-0.2.2/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    28924 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/0/pre_retrieve_node_line/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.326749 autorag-0.2.2/tests/resources/result_project/0/retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.326749 autorag-0.2.2/tests/resources/result_project/0/retrieve_node_line/passage_compressor/
+-rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    31124 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/0/retrieve_node_line/passage_compressor/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.326749 autorag-0.2.2/tests/resources/result_project/0/retrieve_node_line/passage_reranker/
+-rw-r--r--   0 runner    (1001) docker     (127)    67610 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    67719 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    84239 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/0/retrieve_node_line/passage_reranker/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.326749 autorag-0.2.2/tests/resources/result_project/0/retrieve_node_line/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)   103655 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    86579 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)   117633 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/0/retrieve_node_line/retrieval/summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/0/retrieve_node_line/summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/0/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.326749 autorag-0.2.2/tests/resources/result_project/1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/1/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.326749 autorag-0.2.2/tests/resources/result_project/1/pre_retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.330749 autorag-0.2.2/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    28924 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/1/pre_retrieve_node_line/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.246749 autorag-0.2.2/tests/resources/result_project/1/retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.330749 autorag-0.2.2/tests/resources/result_project/1/retrieve_node_line/passage_filter/
+-rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/1/retrieve_node_line/passage_filter/0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.330749 autorag-0.2.2/tests/resources/result_project/1/retrieve_node_line/passage_reranker/
+-rw-r--r--   0 runner    (1001) docker     (127)    67610 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    67719 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    84239 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/1/retrieve_node_line/passage_reranker/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.330749 autorag-0.2.2/tests/resources/result_project/1/retrieve_node_line/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)   103655 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    86579 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)   117633 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/1/retrieve_node_line/retrieval/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.330749 autorag-0.2.2/tests/resources/result_project/2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/2/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.246749 autorag-0.2.2/tests/resources/result_project/2/post_retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.330749 autorag-0.2.2/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/
+-rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.330749 autorag-0.2.2/tests/resources/result_project/2/pre_retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.334749 autorag-0.2.2/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    28924 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/2/pre_retrieve_node_line/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.334749 autorag-0.2.2/tests/resources/result_project/2/retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.334749 autorag-0.2.2/tests/resources/result_project/2/retrieve_node_line/passage_compressor/
+-rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    31124 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/2/retrieve_node_line/passage_compressor/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.334749 autorag-0.2.2/tests/resources/result_project/2/retrieve_node_line/passage_reranker/
+-rw-r--r--   0 runner    (1001) docker     (127)    67610 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    67719 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    84239 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/2/retrieve_node_line/passage_reranker/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.338749 autorag-0.2.2/tests/resources/result_project/2/retrieve_node_line/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)   103655 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    86579 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)   117633 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/2/retrieve_node_line/retrieval/summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/2/retrieve_node_line/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.338749 autorag-0.2.2/tests/resources/result_project/3/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/3/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/best.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.338749 autorag-0.2.2/tests/resources/result_project/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   111931 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/data/corpus.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/data/qa.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.338749 autorag-0.2.2/tests/resources/result_project/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    91651 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/resources/bm25_porter_stemmer.pkl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.338749 autorag-0.2.2/tests/resources/result_project/resources/chroma/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.350749 autorag-0.2.2/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/
+-rw-r--r--   0 runner    (1001) docker     (127)  6284000 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/header.bin
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/link_lists.bin
+-rw-r--r--   0 runner    (1001) docker     (127)   352256 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/resources/chroma/chroma.sqlite3
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/result_project/trial.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/sample_contents_nqa.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.250749 autorag-0.2.2/tests/resources/sample_project/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.350749 autorag-0.2.2/tests/resources/sample_project/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   115302 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/sample_project/data/corpus.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/sample_project/data/qa.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:02:50.350749 autorag-0.2.2/tests/resources/sample_project/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)   109478 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/sample_project/resources/bm25_gpt2.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    91651 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/sample_project/resources/bm25_porter_stemmer.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/simple.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    26773 2024-05-30 03:02:37.000000 autorag-0.2.2/tests/resources/test_bm25_retrieval.pkl
```

### Comparing `autorag-0.2.1/.github/workflows/publish.yml` & `autorag-0.2.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/.github/workflows/sphinx.yml` & `autorag-0.2.2/.github/workflows/sphinx.yml`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/.github/workflows/test.yml` & `autorag-0.2.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/.gitignore` & `autorag-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/AutoRAG.egg-info/PKG-INFO` & `autorag-0.2.2/AutoRAG.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoRAG
-Version: 0.2.1
+Version: 0.2.2
 Summary: Automatically Evaluate RAG pipelines with your own data. Find optimal structure for new RAG product.
 Author-email: Marker-Inc <vkehfdl1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `autorag-0.2.1/AutoRAG.egg-info/SOURCES.txt` & `autorag-0.2.2/AutoRAG.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/AutoRAG.egg-info/requires.txt` & `autorag-0.2.2/AutoRAG.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/CODE_OF_CONDUCT.md` & `autorag-0.2.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/CONTRIBUTING.md` & `autorag-0.2.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/LICENSE` & `autorag-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/PKG-INFO` & `autorag-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoRAG
-Version: 0.2.1
+Version: 0.2.2
 Summary: Automatically Evaluate RAG pipelines with your own data. Find optimal structure for new RAG product.
 Author-email: Marker-Inc <vkehfdl1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `autorag-0.2.1/README.md` & `autorag-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/__init__.py` & `autorag-0.2.2/autorag/__init__.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/cli.py` & `autorag-0.2.2/autorag/cli.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/dashboard.py` & `autorag-0.2.2/autorag/dashboard.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/data/corpus/langchain.py` & `autorag-0.2.2/autorag/data/corpus/langchain.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/data/corpus/llama_index.py` & `autorag-0.2.2/autorag/data/corpus/llama_index.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/data/qacreation/base.py` & `autorag-0.2.2/autorag/data/qacreation/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/data/qacreation/llama_index.py` & `autorag-0.2.2/autorag/data/qacreation/llama_index.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/data/qacreation/llama_index_default_prompt.txt` & `autorag-0.2.2/autorag/data/qacreation/llama_index_default_prompt.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/data/qacreation/ragas.py` & `autorag-0.2.2/autorag/data/qacreation/ragas.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/data/qacreation/simple.py` & `autorag-0.2.2/autorag/data/qacreation/simple.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/data/utils/util.py` & `autorag-0.2.2/autorag/data/utils/util.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/deploy.py` & `autorag-0.2.2/autorag/deploy.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/evaluate/generation.py` & `autorag-0.2.2/autorag/evaluate/generation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt` & `autorag-0.2.2/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt` & `autorag-0.2.2/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt` & `autorag-0.2.2/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt` & `autorag-0.2.2/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/evaluate/metric/generation.py` & `autorag-0.2.2/autorag/evaluate/metric/generation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/evaluate/metric/retrieval.py` & `autorag-0.2.2/autorag/evaluate/metric/retrieval.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/evaluate/metric/retrieval_contents.py` & `autorag-0.2.2/autorag/evaluate/metric/retrieval_contents.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/evaluate/retrieval.py` & `autorag-0.2.2/autorag/evaluate/retrieval.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/evaluate/retrieval_contents.py` & `autorag-0.2.2/autorag/evaluate/retrieval_contents.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/evaluate/util.py` & `autorag-0.2.2/autorag/evaluate/util.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/evaluator.py` & `autorag-0.2.2/autorag/evaluator.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/node_line.py` & `autorag-0.2.2/autorag/node_line.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/generator/base.py` & `autorag-0.2.2/autorag/nodes/generator/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/generator/llama_index_llm.py` & `autorag-0.2.2/autorag/nodes/generator/llama_index_llm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/generator/openai_llm.py` & `autorag-0.2.2/autorag/nodes/generator/openai_llm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/generator/run.py` & `autorag-0.2.2/autorag/nodes/generator/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/generator/vllm.py` & `autorag-0.2.2/autorag/nodes/generator/vllm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/passageaugmenter/base.py` & `autorag-0.2.2/autorag/nodes/passageaugmenter/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/passageaugmenter/prev_next_augmenter.py` & `autorag-0.2.2/autorag/nodes/passageaugmenter/prev_next_augmenter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/passageaugmenter/run.py` & `autorag-0.2.2/autorag/nodes/passageaugmenter/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/passagecompressor/base.py` & `autorag-0.2.2/autorag/nodes/passagecompressor/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/passagecompressor/longllmlingua.py` & `autorag-0.2.2/autorag/nodes/passagecompressor/longllmlingua.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/passagecompressor/refine.py` & `autorag-0.2.2/autorag/nodes/passagecompressor/refine.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/passagecompressor/run.py` & `autorag-0.2.2/autorag/nodes/passagecompressor/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/passagecompressor/tree_summarize.py` & `autorag-0.2.2/autorag/nodes/passagecompressor/tree_summarize.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/passagefilter/base.py` & `autorag-0.2.2/autorag/nodes/passagefilter/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/passagefilter/percentile_cutoff.py` & `autorag-0.2.2/autorag/nodes/passagefilter/percentile_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/passagefilter/recency.py` & `autorag-0.2.2/autorag/nodes/passagefilter/recency.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/passagefilter/run.py` & `autorag-0.2.2/autorag/nodes/passagefilter/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/passagefilter/similarity_percentile_cutoff.py` & `autorag-0.2.2/autorag/nodes/passagefilter/similarity_percentile_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/passagefilter/similarity_threshold_cutoff.py` & `autorag-0.2.2/autorag/nodes/passagefilter/similarity_threshold_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/passagefilter/threshold_cutoff.py` & `autorag-0.2.2/autorag/nodes/passagefilter/threshold_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/passagereranker/base.py` & `autorag-0.2.2/autorag/nodes/passagereranker/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/passagereranker/cohere.py` & `autorag-0.2.2/autorag/nodes/passagereranker/cohere.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/passagereranker/colbert.py` & `autorag-0.2.2/autorag/nodes/passagereranker/colbert.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/passagereranker/flag_embedding.py` & `autorag-0.2.2/autorag/nodes/passagereranker/flag_embedding.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/passagereranker/flag_embedding_llm.py` & `autorag-0.2.2/autorag/nodes/passagereranker/flag_embedding_llm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/passagereranker/jina.py` & `autorag-0.2.2/autorag/nodes/passagereranker/jina.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/passagereranker/koreranker.py` & `autorag-0.2.2/autorag/nodes/passagereranker/koreranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/passagereranker/monot5.py` & `autorag-0.2.2/autorag/nodes/passagereranker/monot5.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/passagereranker/pass_reranker.py` & `autorag-0.2.2/autorag/nodes/passagereranker/pass_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/passagereranker/rankgpt.py` & `autorag-0.2.2/autorag/nodes/passagereranker/rankgpt.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/passagereranker/run.py` & `autorag-0.2.2/autorag/nodes/passagereranker/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/passagereranker/sentence_transformer.py` & `autorag-0.2.2/autorag/nodes/passagereranker/sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/passagereranker/tart/modeling_enc_t5.py` & `autorag-0.2.2/autorag/nodes/passagereranker/tart/modeling_enc_t5.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/passagereranker/tart/tart.py` & `autorag-0.2.2/autorag/nodes/passagereranker/tart/tart.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py` & `autorag-0.2.2/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/passagereranker/time_reranker.py` & `autorag-0.2.2/autorag/nodes/passagereranker/time_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/passagereranker/upr.py` & `autorag-0.2.2/autorag/nodes/passagereranker/upr.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/promptmaker/base.py` & `autorag-0.2.2/autorag/nodes/promptmaker/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/promptmaker/fstring.py` & `autorag-0.2.2/autorag/nodes/promptmaker/fstring.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/promptmaker/long_context_reorder.py` & `autorag-0.2.2/autorag/nodes/promptmaker/long_context_reorder.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/promptmaker/run.py` & `autorag-0.2.2/autorag/nodes/promptmaker/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/queryexpansion/base.py` & `autorag-0.2.2/autorag/nodes/queryexpansion/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/queryexpansion/hyde.py` & `autorag-0.2.2/autorag/nodes/queryexpansion/hyde.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/queryexpansion/multi_query_expansion.py` & `autorag-0.2.2/autorag/nodes/queryexpansion/multi_query_expansion.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/queryexpansion/query_decompose.py` & `autorag-0.2.2/autorag/nodes/queryexpansion/query_decompose.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/queryexpansion/run.py` & `autorag-0.2.2/autorag/nodes/queryexpansion/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/retrieval/base.py` & `autorag-0.2.2/autorag/nodes/retrieval/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/retrieval/bm25.py` & `autorag-0.2.2/autorag/nodes/retrieval/bm25.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/retrieval/hybrid_cc.py` & `autorag-0.2.2/autorag/nodes/retrieval/hybrid_cc.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/retrieval/hybrid_dbsf.py` & `autorag-0.2.2/autorag/nodes/retrieval/hybrid_dbsf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/retrieval/hybrid_rrf.py` & `autorag-0.2.2/autorag/nodes/retrieval/hybrid_rrf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/retrieval/hybrid_rsf.py` & `autorag-0.2.2/autorag/nodes/retrieval/hybrid_rsf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/retrieval/run.py` & `autorag-0.2.2/autorag/nodes/retrieval/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/nodes/retrieval/vectordb.py` & `autorag-0.2.2/autorag/nodes/retrieval/vectordb.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/schema/module.py` & `autorag-0.2.2/autorag/schema/module.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/schema/node.py` & `autorag-0.2.2/autorag/schema/node.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/strategy.py` & `autorag-0.2.2/autorag/strategy.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/support.py` & `autorag-0.2.2/autorag/support.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/utils/preprocess.py` & `autorag-0.2.2/autorag/utils/preprocess.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/autorag/utils/util.py` & `autorag-0.2.2/autorag/utils/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -357,15 +357,17 @@
         else:
             raise KeyError(f"Key '{key}' not found in dictionary.")
     return result
 
 
 def split_dataframe(df, chunk_size):
     num_chunks = len(df) // chunk_size + 1 if len(df) % chunk_size != 0 else len(df) // chunk_size
-    return list(map(lambda x: df[x * chunk_size:(x + 1) * chunk_size], range(num_chunks)))
+    result = list(map(lambda x: df[x * chunk_size:(x + 1) * chunk_size], range(num_chunks)))
+    result = list(map(lambda x: x.reset_index(drop=True), result))
+    return result
 
 
 def find_trial_dir(project_dir: str) -> List[str]:
     # Pattern to match directories named with numbers
     pattern = os.path.join(project_dir, '[0-9]*')
     all_entries = glob.glob(pattern)
```

### Comparing `autorag-0.2.1/autorag/web.py` & `autorag-0.2.2/autorag/web.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/Makefile` & `autorag-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/make.bat` & `autorag-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/_static/data_creation.png` & `autorag-0.2.2/docs/source/_static/data_creation.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/_static/data_folder.png` & `autorag-0.2.2/docs/source/_static/data_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/_static/dcg.png` & `autorag-0.2.2/docs/source/_static/dcg.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/_static/f1_score.png` & `autorag-0.2.2/docs/source/_static/f1_score.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/_static/map.png` & `autorag-0.2.2/docs/source/_static/map.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/_static/mrr.png` & `autorag-0.2.2/docs/source/_static/mrr.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/_static/ndcg.png` & `autorag-0.2.2/docs/source/_static/ndcg.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/_static/ndcg_formula.png` & `autorag-0.2.2/docs/source/_static/ndcg_formula.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/_static/node_folder.png` & `autorag-0.2.2/docs/source/_static/node_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/_static/node_line_folder.png` & `autorag-0.2.2/docs/source/_static/node_line_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/_static/node_line_summary.png` & `autorag-0.2.2/docs/source/_static/node_line_summary.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/_static/node_lines.png` & `autorag-0.2.2/docs/source/_static/node_lines.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/_static/node_summary.png` & `autorag-0.2.2/docs/source/_static/node_summary.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/_static/project_folder_example.png` & `autorag-0.2.2/docs/source/_static/project_folder_example.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/_static/project_folders.png` & `autorag-0.2.2/docs/source/_static/project_folders.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/_static/resources_folder.png` & `autorag-0.2.2/docs/source/_static/resources_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/_static/roadmap/RAG_paradigms.png` & `autorag-0.2.2/docs/source/_static/roadmap/RAG_paradigms.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/_static/roadmap/advanced_RAG.png` & `autorag-0.2.2/docs/source/_static/roadmap/advanced_RAG.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/_static/roadmap/cycle.png` & `autorag-0.2.2/docs/source/_static/roadmap/cycle.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/_static/roadmap/merger.png` & `autorag-0.2.2/docs/source/_static/roadmap/merger.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/_static/roadmap/node_line_modular.png` & `autorag-0.2.2/docs/source/_static/roadmap/node_line_modular.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/_static/roadmap/policy.png` & `autorag-0.2.2/docs/source/_static/roadmap/policy.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/_static/samsung_sundae.jpeg` & `autorag-0.2.2/docs/source/_static/samsung_sundae.jpeg`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/_static/trial_folder.png` & `autorag-0.2.2/docs/source/_static/trial_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/_static/trial_json.png` & `autorag-0.2.2/docs/source/_static/trial_json.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/_static/trial_summary.png` & `autorag-0.2.2/docs/source/_static/trial_summary.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/_static/web_interface.png` & `autorag-0.2.2/docs/source/_static/web_interface.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/api_spec/autorag.data.corpus.rst` & `autorag-0.2.2/docs/source/api_spec/autorag.data.corpus.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/api_spec/autorag.data.qacreation.rst` & `autorag-0.2.2/docs/source/api_spec/autorag.data.qacreation.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/api_spec/autorag.evaluate.metric.rst` & `autorag-0.2.2/docs/source/api_spec/autorag.evaluate.metric.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/api_spec/autorag.evaluate.rst` & `autorag-0.2.2/docs/source/api_spec/autorag.evaluate.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/api_spec/autorag.nodes.generator.rst` & `autorag-0.2.2/docs/source/api_spec/autorag.nodes.generator.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/api_spec/autorag.nodes.passageaugmenter.rst` & `autorag-0.2.2/docs/source/api_spec/autorag.nodes.passageaugmenter.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/api_spec/autorag.nodes.passagecompressor.rst` & `autorag-0.2.2/docs/source/api_spec/autorag.nodes.passagecompressor.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/api_spec/autorag.nodes.passagefilter.rst` & `autorag-0.2.2/docs/source/api_spec/autorag.nodes.passagefilter.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/api_spec/autorag.nodes.passagereranker.rst` & `autorag-0.2.2/docs/source/api_spec/autorag.nodes.passagereranker.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst` & `autorag-0.2.2/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/api_spec/autorag.nodes.promptmaker.rst` & `autorag-0.2.2/docs/source/api_spec/autorag.nodes.promptmaker.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/api_spec/autorag.nodes.queryexpansion.rst` & `autorag-0.2.2/docs/source/api_spec/autorag.nodes.queryexpansion.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/api_spec/autorag.nodes.retrieval.rst` & `autorag-0.2.2/docs/source/api_spec/autorag.nodes.retrieval.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/api_spec/autorag.rst` & `autorag-0.2.2/docs/source/api_spec/autorag.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/conf.py` & `autorag-0.2.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/data_creation/data_format.md` & `autorag-0.2.2/docs/source/data_creation/data_format.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/data_creation/ragas.md` & `autorag-0.2.2/docs/source/data_creation/ragas.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/data_creation/tutorial.md` & `autorag-0.2.2/docs/source/data_creation/tutorial.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/deploy/api_endpoint.md` & `autorag-0.2.2/docs/source/deploy/api_endpoint.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/deploy/web.md` & `autorag-0.2.2/docs/source/deploy/web.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/evaluate_metrics/generation.md` & `autorag-0.2.2/docs/source/evaluate_metrics/generation.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/evaluate_metrics/retrieval.md` & `autorag-0.2.2/docs/source/evaluate_metrics/retrieval.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/evaluate_metrics/retrieval_contents.md` & `autorag-0.2.2/docs/source/evaluate_metrics/retrieval_contents.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/index.rst` & `autorag-0.2.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/install.md` & `autorag-0.2.2/docs/source/install.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/local_model.md` & `autorag-0.2.2/docs/source/local_model.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/generator/generator.md` & `autorag-0.2.2/docs/source/nodes/generator/generator.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/generator/llama_index_llm.md` & `autorag-0.2.2/docs/source/nodes/generator/llama_index_llm.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/generator/openai_llm.md` & `autorag-0.2.2/docs/source/nodes/generator/openai_llm.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/generator/vllm.md` & `autorag-0.2.2/docs/source/nodes/generator/vllm.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/passage_augmenter/passage_augmenter.md` & `autorag-0.2.2/docs/source/nodes/passage_augmenter/passage_augmenter.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/passage_augmenter/prev_next_augmenter.md` & `autorag-0.2.2/docs/source/nodes/passage_augmenter/prev_next_augmenter.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/passage_compressor/longllmlingua.md` & `autorag-0.2.2/docs/source/nodes/passage_compressor/longllmlingua.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/passage_compressor/passage_compressor.md` & `autorag-0.2.2/docs/source/nodes/passage_compressor/passage_compressor.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/passage_compressor/refine.md` & `autorag-0.2.2/docs/source/nodes/passage_compressor/refine.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/passage_compressor/tree_summarize.md` & `autorag-0.2.2/docs/source/nodes/passage_compressor/tree_summarize.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/passage_filter/passage_filter.md` & `autorag-0.2.2/docs/source/nodes/passage_filter/passage_filter.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/passage_filter/percentile_cutoff.md` & `autorag-0.2.2/docs/source/nodes/passage_filter/percentile_cutoff.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/passage_filter/recency_filter.md` & `autorag-0.2.2/docs/source/nodes/passage_filter/recency_filter.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md` & `autorag-0.2.2/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md` & `autorag-0.2.2/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/passage_filter/threshold_cutoff.md` & `autorag-0.2.2/docs/source/nodes/passage_filter/threshold_cutoff.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/passage_reranker/cohere.md` & `autorag-0.2.2/docs/source/nodes/passage_reranker/cohere.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/passage_reranker/colbert.md` & `autorag-0.2.2/docs/source/nodes/passage_reranker/colbert.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md` & `autorag-0.2.2/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/passage_reranker/flag_embedding_reranker.md` & `autorag-0.2.2/docs/source/nodes/passage_reranker/flag_embedding_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/passage_reranker/jina_reranker.md` & `autorag-0.2.2/docs/source/nodes/passage_reranker/jina_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/passage_reranker/monot5.md` & `autorag-0.2.2/docs/source/nodes/passage_reranker/monot5.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/passage_reranker/passage_reranker.md` & `autorag-0.2.2/docs/source/nodes/passage_reranker/passage_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/passage_reranker/rankgpt.md` & `autorag-0.2.2/docs/source/nodes/passage_reranker/rankgpt.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md` & `autorag-0.2.2/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/passage_reranker/tart.md` & `autorag-0.2.2/docs/source/nodes/passage_reranker/tart.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/passage_reranker/time_reranker.md` & `autorag-0.2.2/docs/source/nodes/passage_reranker/time_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/passage_reranker/upr.md` & `autorag-0.2.2/docs/source/nodes/passage_reranker/upr.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/prompt_maker/fstring.md` & `autorag-0.2.2/docs/source/nodes/prompt_maker/fstring.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/prompt_maker/long_context_reorder.md` & `autorag-0.2.2/docs/source/nodes/prompt_maker/long_context_reorder.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/prompt_maker/prompt_maker.md` & `autorag-0.2.2/docs/source/nodes/prompt_maker/prompt_maker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/query_expansion/hyde.md` & `autorag-0.2.2/docs/source/nodes/query_expansion/hyde.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/query_expansion/multi_query_expansion.md` & `autorag-0.2.2/docs/source/nodes/query_expansion/multi_query_expansion.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/query_expansion/query_decompose.md` & `autorag-0.2.2/docs/source/nodes/query_expansion/query_decompose.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/query_expansion/query_expansion.md` & `autorag-0.2.2/docs/source/nodes/query_expansion/query_expansion.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/retrieval/bm25.md` & `autorag-0.2.2/docs/source/nodes/retrieval/bm25.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/retrieval/hybrid_cc.md` & `autorag-0.2.2/docs/source/nodes/retrieval/hybrid_cc.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/retrieval/hybrid_dbsf.md` & `autorag-0.2.2/docs/source/nodes/retrieval/hybrid_dbsf.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/retrieval/hybrid_rrf.md` & `autorag-0.2.2/docs/source/nodes/retrieval/hybrid_rrf.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/retrieval/hybrid_rsf.md` & `autorag-0.2.2/docs/source/nodes/retrieval/hybrid_rsf.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/retrieval/retrieval.md` & `autorag-0.2.2/docs/source/nodes/retrieval/retrieval.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/nodes/retrieval/vectordb.md` & `autorag-0.2.2/docs/source/nodes/retrieval/vectordb.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/optimization/custom_config.md` & `autorag-0.2.2/docs/source/optimization/custom_config.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/optimization/folder_structure.md` & `autorag-0.2.2/docs/source/optimization/folder_structure.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/optimization/optimization.md` & `autorag-0.2.2/docs/source/optimization/optimization.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/optimization/sample_full_config.yaml` & `autorag-0.2.2/docs/source/optimization/sample_full_config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/optimization/strategies.md` & `autorag-0.2.2/docs/source/optimization/strategies.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/roadmap/modular_rag.md` & `autorag-0.2.2/docs/source/roadmap/modular_rag.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/structure.md` & `autorag-0.2.2/docs/source/structure.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/troubleshooting.md` & `autorag-0.2.2/docs/source/troubleshooting.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/docs/source/tutorial.md` & `autorag-0.2.2/docs/source/tutorial.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/pyproject.toml` & `autorag-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/requirements.txt` & `autorag-0.2.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/sample_config/compact_local.yaml` & `autorag-0.2.2/sample_config/compact_local.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/sample_config/compact_openai.yaml` & `autorag-0.2.2/sample_config/compact_openai.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/sample_config/config_korean.yaml` & `autorag-0.2.2/sample_config/config_korean.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/sample_config/extracted_sample.yaml` & `autorag-0.2.2/sample_config/extracted_sample.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/sample_config/full.yaml` & `autorag-0.2.2/sample_config/full.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/sample_config/simple_local.yaml` & `autorag-0.2.2/sample_config/simple_local.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/sample_config/simple_openai.yaml` & `autorag-0.2.2/sample_config/simple_openai.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/sample_dataset/README.md` & `autorag-0.2.2/sample_dataset/README.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/sample_dataset/eli5/load_eli5_dataset.py` & `autorag-0.2.2/sample_dataset/eli5/load_eli5_dataset.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/sample_dataset/msmarco/load_msmarco_dataset.py` & `autorag-0.2.2/sample_dataset/msmarco/load_msmarco_dataset.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/sample_dataset/triviaqa/load_triviaqa_dataset.py` & `autorag-0.2.2/sample_dataset/triviaqa/load_triviaqa_dataset.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/data/corpus/test_base.py` & `autorag-0.2.2/tests/autorag/data/corpus/test_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/data/corpus/test_langchain.py` & `autorag-0.2.2/tests/autorag/data/corpus/test_langchain.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/data/corpus/test_llama_index_corpus.py` & `autorag-0.2.2/tests/autorag/data/corpus/test_llama_index_corpus.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/data/qacreation/test_base_qacreation.py` & `autorag-0.2.2/tests/autorag/data/qacreation/test_base_qacreation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/data/qacreation/test_llama_index_qacreation.py` & `autorag-0.2.2/tests/autorag/data/qacreation/test_llama_index_qacreation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/data/qacreation/test_ragas_qa_creation.py` & `autorag-0.2.2/tests/autorag/data/qacreation/test_ragas_qa_creation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/data/qacreation/test_simple.py` & `autorag-0.2.2/tests/autorag/data/qacreation/test_simple.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/evaluate/metric/test_generation_metric.py` & `autorag-0.2.2/tests/autorag/evaluate/metric/test_generation_metric.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py` & `autorag-0.2.2/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/evaluate/metric/test_retrieval_metric.py` & `autorag-0.2.2/tests/autorag/evaluate/metric/test_retrieval_metric.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/evaluate/test_evaluate_util.py` & `autorag-0.2.2/tests/autorag/evaluate/test_evaluate_util.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/evaluate/test_generation_evaluate.py` & `autorag-0.2.2/tests/autorag/evaluate/test_generation_evaluate.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/evaluate/test_retrieval_contents_evaluate.py` & `autorag-0.2.2/tests/autorag/evaluate/test_retrieval_contents_evaluate.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/evaluate/test_retrieval_evaluate.py` & `autorag-0.2.2/tests/autorag/evaluate/test_retrieval_evaluate.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/generator/test_generator_base.py` & `autorag-0.2.2/tests/autorag/nodes/generator/test_generator_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/generator/test_llama_index_llm.py` & `autorag-0.2.2/tests/autorag/nodes/generator/test_llama_index_llm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/generator/test_openai.py` & `autorag-0.2.2/tests/autorag/nodes/generator/test_openai.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/generator/test_run_generator_node.py` & `autorag-0.2.2/tests/autorag/nodes/generator/test_run_generator_node.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/generator/test_vllm.py` & `autorag-0.2.2/tests/autorag/nodes/generator/test_vllm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/passageaugmenter/test_base_passage_augmenter.py` & `autorag-0.2.2/tests/autorag/nodes/passageaugmenter/test_base_passage_augmenter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/passageaugmenter/test_pass_passage_augmenter.py` & `autorag-0.2.2/tests/autorag/nodes/passageaugmenter/test_pass_passage_augmenter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/passageaugmenter/test_prev_next_augmenter.py` & `autorag-0.2.2/tests/autorag/nodes/passageaugmenter/test_prev_next_augmenter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/passageaugmenter/test_run_passage_augmenter.py` & `autorag-0.2.2/tests/autorag/nodes/passageaugmenter/test_run_passage_augmenter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py` & `autorag-0.2.2/tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/passagecompressor/test_longllmlingua.py` & `autorag-0.2.2/tests/autorag/nodes/passagecompressor/test_longllmlingua.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/passagecompressor/test_pass_compressor.py` & `autorag-0.2.2/tests/autorag/nodes/passagecompressor/test_pass_compressor.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/passagecompressor/test_refine.py` & `autorag-0.2.2/tests/autorag/nodes/passagecompressor/test_refine.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py` & `autorag-0.2.2/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/passagecompressor/test_tree_summarize.py` & `autorag-0.2.2/tests/autorag/nodes/passagecompressor/test_tree_summarize.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py` & `autorag-0.2.2/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/passagefilter/test_passage_filter_base.py` & `autorag-0.2.2/tests/autorag/nodes/passagefilter/test_passage_filter_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/passagefilter/test_passage_filter_run.py` & `autorag-0.2.2/tests/autorag/nodes/passagefilter/test_passage_filter_run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/passagefilter/test_percentile_cutoff.py` & `autorag-0.2.2/tests/autorag/nodes/passagefilter/test_percentile_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/passagefilter/test_recency_filter.py` & `autorag-0.2.2/tests/autorag/nodes/passagefilter/test_recency_filter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/passagefilter/test_similarity_percentile_cutoff.py` & `autorag-0.2.2/tests/autorag/nodes/passagefilter/test_similarity_percentile_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/passagefilter/test_similarity_threshold_cutoff.py` & `autorag-0.2.2/tests/autorag/nodes/passagefilter/test_similarity_threshold_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/passagefilter/test_threshold_cutoff.py` & `autorag-0.2.2/tests/autorag/nodes/passagefilter/test_threshold_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/passagereranker/test_cohere_reranker.py` & `autorag-0.2.2/tests/autorag/nodes/passagereranker/test_cohere_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/passagereranker/test_colbert_reranker.py` & `autorag-0.2.2/tests/autorag/nodes/passagereranker/test_colbert_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/passagereranker/test_flag_embedding.py` & `autorag-0.2.2/tests/autorag/nodes/passagereranker/test_flag_embedding.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py` & `autorag-0.2.2/tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/passagereranker/test_jina_reranker.py` & `autorag-0.2.2/tests/autorag/nodes/passagereranker/test_jina_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/passagereranker/test_koreranker.py` & `autorag-0.2.2/tests/autorag/nodes/passagereranker/test_koreranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/passagereranker/test_monot5.py` & `autorag-0.2.2/tests/autorag/nodes/passagereranker/test_monot5.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/passagereranker/test_pass_reranker.py` & `autorag-0.2.2/tests/autorag/nodes/passagereranker/test_pass_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py` & `autorag-0.2.2/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py` & `autorag-0.2.2/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/passagereranker/test_rankgpt.py` & `autorag-0.2.2/tests/autorag/nodes/passagereranker/test_rankgpt.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/passagereranker/test_sentence_transformer.py` & `autorag-0.2.2/tests/autorag/nodes/passagereranker/test_sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/passagereranker/test_tart.py` & `autorag-0.2.2/tests/autorag/nodes/passagereranker/test_tart.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/passagereranker/test_time_reranker.py` & `autorag-0.2.2/tests/autorag/nodes/passagereranker/test_time_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/passagereranker/test_upr.py` & `autorag-0.2.2/tests/autorag/nodes/passagereranker/test_upr.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/promptmaker/test_fstring.py` & `autorag-0.2.2/tests/autorag/nodes/promptmaker/test_fstring.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/promptmaker/test_long_context_reorder.py` & `autorag-0.2.2/tests/autorag/nodes/promptmaker/test_long_context_reorder.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py` & `autorag-0.2.2/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py` & `autorag-0.2.2/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/queryexpansion/test_hyde.py` & `autorag-0.2.2/tests/autorag/nodes/queryexpansion/test_hyde.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/queryexpansion/test_multi_query_expansion.py` & `autorag-0.2.2/tests/autorag/nodes/queryexpansion/test_multi_query_expansion.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py` & `autorag-0.2.2/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/queryexpansion/test_query_decompose.py` & `autorag-0.2.2/tests/autorag/nodes/queryexpansion/test_query_decompose.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py` & `autorag-0.2.2/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py` & `autorag-0.2.2/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/retrieval/test_bm25.py` & `autorag-0.2.2/tests/autorag/nodes/retrieval/test_bm25.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/retrieval/test_hybrid_base.py` & `autorag-0.2.2/tests/autorag/nodes/retrieval/test_hybrid_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/retrieval/test_hybrid_cc.py` & `autorag-0.2.2/tests/autorag/nodes/retrieval/test_hybrid_cc.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py` & `autorag-0.2.2/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/retrieval/test_hybrid_rrf.py` & `autorag-0.2.2/tests/autorag/nodes/retrieval/test_hybrid_rrf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/retrieval/test_hybrid_rsf.py` & `autorag-0.2.2/tests/autorag/nodes/retrieval/test_hybrid_rsf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/retrieval/test_retrieval_base.py` & `autorag-0.2.2/tests/autorag/nodes/retrieval/test_retrieval_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/retrieval/test_run_retrieval_node.py` & `autorag-0.2.2/tests/autorag/nodes/retrieval/test_run_retrieval_node.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/nodes/retrieval/test_vectordb.py` & `autorag-0.2.2/tests/autorag/nodes/retrieval/test_vectordb.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/schema/test_module_schema.py` & `autorag-0.2.2/tests/autorag/schema/test_module_schema.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/schema/test_node_schema.py` & `autorag-0.2.2/tests/autorag/schema/test_node_schema.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/test_cli.py` & `autorag-0.2.2/tests/autorag/test_cli.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/test_dashboard.py` & `autorag-0.2.2/tests/autorag/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/test_deploy.py` & `autorag-0.2.2/tests/autorag/test_deploy.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/test_evaluator.py` & `autorag-0.2.2/tests/autorag/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/test_strategy.py` & `autorag-0.2.2/tests/autorag/test_strategy.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/test_web.py` & `autorag-0.2.2/tests/autorag/test_web.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/utils/test_preprocess.py` & `autorag-0.2.2/tests/autorag/utils/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/autorag/utils/test_util.py` & `autorag-0.2.2/tests/autorag/utils/test_util.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/delete_tests.py` & `autorag-0.2.2/tests/delete_tests.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/mock.py` & `autorag-0.2.2/tests/mock.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/README.md` & `autorag-0.2.2/tests/resources/README.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/corpus_data_sample.parquet` & `autorag-0.2.2/tests/resources/corpus_data_sample.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/data_creation/raw_dir/sample1.txt` & `autorag-0.2.2/tests/resources/data_creation/raw_dir/sample1.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/data_creation/raw_dir/sample2.txt` & `autorag-0.2.2/tests/resources/data_creation/raw_dir/sample2.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/data_creation/raw_dir/sample3.txt` & `autorag-0.2.2/tests/resources/data_creation/raw_dir/sample3.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/full.yaml` & `autorag-0.2.2/tests/resources/full.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/qa_data_sample.parquet` & `autorag-0.2.2/tests/resources/qa_data_sample.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/qa_test_data_sample.parquet` & `autorag-0.2.2/tests/resources/qa_test_data_sample.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/0/config.yaml` & `autorag-0.2.2/tests/resources/result_project/0/config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet` & `autorag-0.2.2/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet` & `autorag-0.2.2/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet` & `autorag-0.2.2/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet` & `autorag-0.2.2/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet` & `autorag-0.2.2/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet` & `autorag-0.2.2/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet` & `autorag-0.2.2/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv` & `autorag-0.2.2/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet` & `autorag-0.2.2/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet` & `autorag-0.2.2/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet` & `autorag-0.2.2/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv` & `autorag-0.2.2/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet` & `autorag-0.2.2/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet` & `autorag-0.2.2/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet` & `autorag-0.2.2/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet` & `autorag-0.2.2/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet` & `autorag-0.2.2/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet` & `autorag-0.2.2/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet` & `autorag-0.2.2/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet` & `autorag-0.2.2/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet` & `autorag-0.2.2/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet` & `autorag-0.2.2/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet` & `autorag-0.2.2/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet` & `autorag-0.2.2/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/0/summary.csv` & `autorag-0.2.2/tests/resources/result_project/0/summary.csv`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/1/config.yaml` & `autorag-0.2.2/tests/resources/result_project/1/config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet` & `autorag-0.2.2/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet` & `autorag-0.2.2/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet` & `autorag-0.2.2/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet` & `autorag-0.2.2/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/passage_filter/0.parquet` & `autorag-0.2.2/tests/resources/result_project/1/retrieve_node_line/passage_filter/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet` & `autorag-0.2.2/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet` & `autorag-0.2.2/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet` & `autorag-0.2.2/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet` & `autorag-0.2.2/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet` & `autorag-0.2.2/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet` & `autorag-0.2.2/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/2/config.yaml` & `autorag-0.2.2/tests/resources/result_project/2/config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet` & `autorag-0.2.2/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet` & `autorag-0.2.2/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet` & `autorag-0.2.2/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet` & `autorag-0.2.2/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet` & `autorag-0.2.2/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet` & `autorag-0.2.2/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet` & `autorag-0.2.2/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet` & `autorag-0.2.2/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet` & `autorag-0.2.2/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet` & `autorag-0.2.2/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet` & `autorag-0.2.2/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet` & `autorag-0.2.2/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet` & `autorag-0.2.2/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/3/config.yaml` & `autorag-0.2.2/tests/resources/result_project/3/config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/best.yaml` & `autorag-0.2.2/tests/resources/result_project/best.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/data/corpus.parquet` & `autorag-0.2.2/tests/resources/result_project/data/corpus.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/data/qa.parquet` & `autorag-0.2.2/tests/resources/result_project/data/qa.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/resources/bm25_porter_stemmer.pkl` & `autorag-0.2.2/tests/resources/result_project/resources/bm25_porter_stemmer.pkl`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin` & `autorag-0.2.2/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin` & `autorag-0.2.2/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/result_project/resources/chroma/chroma.sqlite3` & `autorag-0.2.2/tests/resources/result_project/resources/chroma/chroma.sqlite3`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/sample_contents_nqa.csv` & `autorag-0.2.2/tests/resources/sample_contents_nqa.csv`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/sample_project/data/corpus.parquet` & `autorag-0.2.2/tests/resources/sample_project/data/corpus.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/sample_project/data/qa.parquet` & `autorag-0.2.2/tests/resources/sample_project/data/qa.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/sample_project/resources/bm25_gpt2.pkl` & `autorag-0.2.2/tests/resources/sample_project/resources/bm25_gpt2.pkl`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/sample_project/resources/bm25_porter_stemmer.pkl` & `autorag-0.2.2/tests/resources/sample_project/resources/bm25_porter_stemmer.pkl`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/simple.yaml` & `autorag-0.2.2/tests/resources/simple.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.2.1/tests/resources/test_bm25_retrieval.pkl` & `autorag-0.2.2/tests/resources/test_bm25_retrieval.pkl`

 * *Files identical despite different names*

