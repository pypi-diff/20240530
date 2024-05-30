# Comparing `tmp/r2r-0.2.1.tar.gz` & `tmp/r2r-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r2r-0.2.1.tar", max compression
+gzip compressed data, was "r2r-0.2.2.tar", max compression
```

## Comparing `r2r-0.2.1.tar` & `r2r-0.2.2.tar`

### file list

```diff
@@ -1,96 +1,97 @@
--rw-r--r--   0        0        0     1082 2024-05-30 00:51:23.130715 r2r-0.2.1/LICENSE.md
--rw-r--r--   0        0        0    12944 2024-05-30 00:51:23.130715 r2r-0.2.1/README.md
--rw-r--r--   0        0        0     1151 2024-05-30 00:51:23.134715 r2r-0.2.1/config.json
--rw-r--r--   0        0        0     1980 2024-05-30 00:51:23.150715 r2r-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2047 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/__init__.py
--rw-r--r--   0        0        0     3083 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/__init__.py
--rw-r--r--   0        0        0     1371 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/abstractions/document.py
--rw-r--r--   0        0        0      186 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/abstractions/llm.py
--rw-r--r--   0        0        0     1083 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/abstractions/prompt.py
--rw-r--r--   0        0        0      813 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/abstractions/search.py
--rw-r--r--   0        0        0     1934 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/abstractions/vector.py
--rw-r--r--   0        0        0      538 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/parsers/__init__.py
--rw-r--r--   0        0        0      334 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/parsers/base_parser.py
--rw-r--r--   0        0        0    14096 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/parsers/parser_impls.py
--rw-r--r--   0        0        0     9358 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/pipeline/base_pipeline.py
--rw-r--r--   0        0        0     3949 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/pipes/base_pipe.py
--rw-r--r--   0        0        0     2409 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/pipes/loggable_pipe.py
--rw-r--r--   0        0        0    16417 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/pipes/pipe_logging.py
--rw-r--r--   0        0        0     1306 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/providers/base_provider.py
--rw-r--r--   0        0        0     2267 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/providers/embedding_provider.py
--rw-r--r--   0        0        0     1029 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/providers/eval_provider.py
--rw-r--r--   0        0        0     2328 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/providers/llm_provider.py
--rw-r--r--   0        0        0     1456 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/providers/prompt_provider.py
--rw-r--r--   0        0        0     2550 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/providers/vector_db_provider.py
--rw-r--r--   0        0        0      363 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/utils/__init__.py
--rw-r--r--   0        0        0      922 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/utils/base_utils.py
--rw-r--r--   0        0        0       95 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/utils/splitter/__init__.py
--rw-r--r--   0        0        0    66643 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/utils/splitter/text.py
--rw-r--r--   0        0        0      332 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/embeddings/__init__.py
--rw-r--r--   0        0        0     2363 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/embeddings/dummy/provider.py
--rw-r--r--   0        0        0     6309 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/embeddings/openai/openai_base.py
--rw-r--r--   0        0        0     6238 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/embeddings/setence_transformer/sentence_transformer_base.py
--rw-r--r--   0        0        0       78 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/eval/__init__.py
--rw-r--r--   0        0        0     2867 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/eval/llm/base_llm_eval.py
--rw-r--r--   0        0        0        0 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/examples/__init__.py
--rw-r--r--   0        0        0     3091 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/examples/custom_rag.py
--rw-r--r--   0        0        0    73353 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/examples/data/aristotle.txt
--rw-r--r--   0        0        0       49 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/examples/data/example_postgres_logger_config.json
--rw-r--r--   0        0        0       91 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/examples/data/example_qdrant_config.json
--rw-r--r--   0        0        0      455 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/examples/data/example_rerank_config.json
--rw-r--r--   0        0        0  1440303 2024-05-30 00:51:23.158715 r2r-0.2.1/r2r/examples/data/lyft_2021.pdf
--rw-r--r--   0        0        0   131542 2024-05-30 00:51:23.158715 r2r-0.2.1/r2r/examples/data/pg_essay_1.html
--rw-r--r--   0        0        0   125150 2024-05-30 00:51:23.158715 r2r-0.2.1/r2r/examples/data/pg_essay_2.html
--rw-r--r--   0        0        0   124948 2024-05-30 00:51:23.158715 r2r-0.2.1/r2r/examples/data/pg_essay_3.html
--rw-r--r--   0        0        0   118147 2024-05-30 00:51:23.158715 r2r-0.2.1/r2r/examples/data/pg_essay_4.html
--rw-r--r--   0        0        0   123820 2024-05-30 00:51:23.158715 r2r-0.2.1/r2r/examples/data/pg_essay_5.html
--rw-r--r--   0        0        0   791764 2024-05-30 00:51:23.162715 r2r-0.2.1/r2r/examples/data/screen_shot.png
--rw-r--r--   0        0        0       19 2024-05-30 00:51:23.162715 r2r-0.2.1/r2r/examples/data/test.txt
--rw-r--r--   0        0        0  1880483 2024-05-30 00:51:23.170715 r2r-0.2.1/r2r/examples/data/uber_2021.pdf
--rw-r--r--   0        0        0    12004 2024-05-30 00:51:23.170715 r2r-0.2.1/r2r/examples/demo.py
--rw-r--r--   0        0        0        0 2024-05-30 00:51:23.170715 r2r-0.2.1/r2r/examples/servers/__init__.py
--rw-r--r--   0        0        0     1569 2024-05-30 00:51:23.170715 r2r-0.2.1/r2r/examples/servers/configurable_pipeline.py
--rw-r--r--   0        0        0      147 2024-05-30 00:51:23.170715 r2r-0.2.1/r2r/integrations/__init__.py
--rw-r--r--   0        0        0     1839 2024-05-30 00:51:23.170715 r2r-0.2.1/r2r/integrations/exa.py
--rw-r--r--   0        0        0     1535 2024-05-30 00:51:23.170715 r2r-0.2.1/r2r/integrations/ionic.py
--rw-r--r--   0        0        0     3940 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/integrations/serper.py
--rw-r--r--   0        0        0      232 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/llms/__init__.py
--rw-r--r--   0        0        0     3315 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/llms/litellm/base_litellm.py
--rw-r--r--   0        0        0     3919 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/llms/llama_cpp/base_llama_cpp.py
--rw-r--r--   0        0        0        0 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/llms/llama_cpp/model/__init__.py
--rw-r--r--   0        0        0     3462 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/llms/openai/base_openai.py
--rw-r--r--   0        0        0      410 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/main/__init__.py
--rw-r--r--   0        0        0     1102 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/main/r2r_abstractions.py
--rw-r--r--   0        0        0    24571 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/main/r2r_app.py
--rw-r--r--   0        0        0     5529 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/main/r2r_client.py
--rw-r--r--   0        0        0     4599 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/main/r2r_config.py
--rw-r--r--   0        0        0    11331 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/main/r2r_factory.py
--rw-r--r--   0        0        0      593 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/pipes/__init__.py
--rw-r--r--   0        0        0     1266 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/pipes/abstractions/generator_pipe.py
--rw-r--r--   0        0        0     1552 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/pipes/abstractions/search_pipe.py
--rw-r--r--   0        0        0     7244 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/pipes/embedding_pipe.py
--rw-r--r--   0        0        0     1272 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/pipes/eval_pipe.py
--rw-r--r--   0        0        0     7590 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/pipes/parsing_pipe.py
--rw-r--r--   0        0        0     3050 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/pipes/query_transform_pipe.py
--rw-r--r--   0        0        0     2738 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/pipes/rag_pipe.py
--rw-r--r--   0        0        0     3307 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/pipes/streaming_rag_pipe.py
--rw-r--r--   0        0        0     2808 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/pipes/vector_search_pipe.py
--rw-r--r--   0        0        0     3166 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/pipes/vector_storage_pipe.py
--rw-r--r--   0        0        0       90 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/prompts/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/prompts/local/__init__.py
--rw-r--r--   0        0        0     4390 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/prompts/local/defaults.jsonl
--rw-r--r--   0        0        0     1900 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/prompts/local/r2r_prompt_provider.py
--rw-r--r--   0        0        0      539 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/vecs/__init__.py
--rw-r--r--   0        0        0      363 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/vecs/adapter/__init__.py
--rw-r--r--   0        0        0     3263 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/vecs/adapter/base.py
--rw-r--r--   0        0        0     3170 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/vecs/adapter/markdown.py
--rw-r--r--   0        0        0     1668 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/vecs/adapter/noop.py
--rw-r--r--   0        0        0     5317 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/vecs/adapter/text.py
--rw-r--r--   0        0        0     9350 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/vecs/client.py
--rw-r--r--   0        0        0    36863 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/vecs/collection.py
--rw-r--r--   0        0        0     1687 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/vecs/exc.py
--rw-r--r--   0        0        0      213 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/vector_dbs/__init__.py
--rw-r--r--   0        0        0     6379 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/vector_dbs/local/r2r_local_vector_db.py
--rw-r--r--   0        0        0     6268 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/vector_dbs/pgvector/pgvector_db.py
--rw-r--r--   0        0        0     7412 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/vector_dbs/qdrant/qdrant_db.py
--rw-r--r--   0        0        0    14924 1970-01-01 00:00:00.000000 r2r-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-05-30 01:08:40.275281 r2r-0.2.2/LICENSE.md
+-rw-r--r--   0        0        0    12944 2024-05-30 01:08:40.275281 r2r-0.2.2/README.md
+-rw-r--r--   0        0        0     1151 2024-05-30 01:08:40.275281 r2r-0.2.2/config.json
+-rw-r--r--   0        0        0     1980 2024-05-30 01:08:40.291281 r2r-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2047 2024-05-30 01:08:40.291281 r2r-0.2.2/r2r/__init__.py
+-rw-r--r--   0        0        0     3083 2024-05-30 01:08:40.291281 r2r-0.2.2/r2r/core/__init__.py
+-rw-r--r--   0        0        0     1371 2024-05-30 01:08:40.291281 r2r-0.2.2/r2r/core/abstractions/document.py
+-rw-r--r--   0        0        0      186 2024-05-30 01:08:40.291281 r2r-0.2.2/r2r/core/abstractions/llm.py
+-rw-r--r--   0        0        0     1083 2024-05-30 01:08:40.291281 r2r-0.2.2/r2r/core/abstractions/prompt.py
+-rw-r--r--   0        0        0      813 2024-05-30 01:08:40.291281 r2r-0.2.2/r2r/core/abstractions/search.py
+-rw-r--r--   0        0        0     1934 2024-05-30 01:08:40.291281 r2r-0.2.2/r2r/core/abstractions/vector.py
+-rw-r--r--   0        0        0      538 2024-05-30 01:08:40.291281 r2r-0.2.2/r2r/core/parsers/__init__.py
+-rw-r--r--   0        0        0      334 2024-05-30 01:08:40.291281 r2r-0.2.2/r2r/core/parsers/base_parser.py
+-rw-r--r--   0        0        0    14096 2024-05-30 01:08:40.295281 r2r-0.2.2/r2r/core/parsers/parser_impls.py
+-rw-r--r--   0        0        0     9358 2024-05-30 01:08:40.295281 r2r-0.2.2/r2r/core/pipeline/base_pipeline.py
+-rw-r--r--   0        0        0     3949 2024-05-30 01:08:40.295281 r2r-0.2.2/r2r/core/pipes/base_pipe.py
+-rw-r--r--   0        0        0     2409 2024-05-30 01:08:40.295281 r2r-0.2.2/r2r/core/pipes/loggable_pipe.py
+-rw-r--r--   0        0        0    16417 2024-05-30 01:08:40.295281 r2r-0.2.2/r2r/core/pipes/pipe_logging.py
+-rw-r--r--   0        0        0     1306 2024-05-30 01:08:40.295281 r2r-0.2.2/r2r/core/providers/base_provider.py
+-rw-r--r--   0        0        0     2267 2024-05-30 01:08:40.295281 r2r-0.2.2/r2r/core/providers/embedding_provider.py
+-rw-r--r--   0        0        0     1029 2024-05-30 01:08:40.295281 r2r-0.2.2/r2r/core/providers/eval_provider.py
+-rw-r--r--   0        0        0     2328 2024-05-30 01:08:40.295281 r2r-0.2.2/r2r/core/providers/llm_provider.py
+-rw-r--r--   0        0        0     1456 2024-05-30 01:08:40.295281 r2r-0.2.2/r2r/core/providers/prompt_provider.py
+-rw-r--r--   0        0        0     2550 2024-05-30 01:08:40.295281 r2r-0.2.2/r2r/core/providers/vector_db_provider.py
+-rw-r--r--   0        0        0      363 2024-05-30 01:08:40.295281 r2r-0.2.2/r2r/core/utils/__init__.py
+-rw-r--r--   0        0        0      922 2024-05-30 01:08:40.295281 r2r-0.2.2/r2r/core/utils/base_utils.py
+-rw-r--r--   0        0        0       95 2024-05-30 01:08:40.295281 r2r-0.2.2/r2r/core/utils/splitter/__init__.py
+-rw-r--r--   0        0        0    66643 2024-05-30 01:08:40.295281 r2r-0.2.2/r2r/core/utils/splitter/text.py
+-rw-r--r--   0        0        0      332 2024-05-30 01:08:40.295281 r2r-0.2.2/r2r/embeddings/__init__.py
+-rw-r--r--   0        0        0     2363 2024-05-30 01:08:40.295281 r2r-0.2.2/r2r/embeddings/dummy/provider.py
+-rw-r--r--   0        0        0     6309 2024-05-30 01:08:40.295281 r2r-0.2.2/r2r/embeddings/openai/openai_base.py
+-rw-r--r--   0        0        0     6238 2024-05-30 01:08:40.295281 r2r-0.2.2/r2r/embeddings/setence_transformer/sentence_transformer_base.py
+-rw-r--r--   0        0        0       78 2024-05-30 01:08:40.295281 r2r-0.2.2/r2r/eval/__init__.py
+-rw-r--r--   0        0        0     2867 2024-05-30 01:08:40.295281 r2r-0.2.2/r2r/eval/llm/base_llm_eval.py
+-rw-r--r--   0        0        0        0 2024-05-30 01:08:40.295281 r2r-0.2.2/r2r/examples/__init__.py
+-rw-r--r--   0        0        0      385 2024-05-30 01:08:40.295281 r2r-0.2.2/r2r/examples/base_app.py
+-rw-r--r--   0        0        0     3091 2024-05-30 01:08:40.295281 r2r-0.2.2/r2r/examples/custom_rag.py
+-rw-r--r--   0        0        0    73353 2024-05-30 01:08:40.295281 r2r-0.2.2/r2r/examples/data/aristotle.txt
+-rw-r--r--   0        0        0       49 2024-05-30 01:08:40.295281 r2r-0.2.2/r2r/examples/data/example_postgres_logger_config.json
+-rw-r--r--   0        0        0       91 2024-05-30 01:08:40.295281 r2r-0.2.2/r2r/examples/data/example_qdrant_config.json
+-rw-r--r--   0        0        0      455 2024-05-30 01:08:40.295281 r2r-0.2.2/r2r/examples/data/example_rerank_config.json
+-rw-r--r--   0        0        0  1440303 2024-05-30 01:08:40.303281 r2r-0.2.2/r2r/examples/data/lyft_2021.pdf
+-rw-r--r--   0        0        0   131542 2024-05-30 01:08:40.303281 r2r-0.2.2/r2r/examples/data/pg_essay_1.html
+-rw-r--r--   0        0        0   125150 2024-05-30 01:08:40.303281 r2r-0.2.2/r2r/examples/data/pg_essay_2.html
+-rw-r--r--   0        0        0   124948 2024-05-30 01:08:40.303281 r2r-0.2.2/r2r/examples/data/pg_essay_3.html
+-rw-r--r--   0        0        0   118147 2024-05-30 01:08:40.303281 r2r-0.2.2/r2r/examples/data/pg_essay_4.html
+-rw-r--r--   0        0        0   123820 2024-05-30 01:08:40.303281 r2r-0.2.2/r2r/examples/data/pg_essay_5.html
+-rw-r--r--   0        0        0   791764 2024-05-30 01:08:40.307281 r2r-0.2.2/r2r/examples/data/screen_shot.png
+-rw-r--r--   0        0        0       19 2024-05-30 01:08:40.307281 r2r-0.2.2/r2r/examples/data/test.txt
+-rw-r--r--   0        0        0  1880483 2024-05-30 01:08:40.315281 r2r-0.2.2/r2r/examples/data/uber_2021.pdf
+-rw-r--r--   0        0        0    11992 2024-05-30 01:08:40.315281 r2r-0.2.2/r2r/examples/demo.py
+-rw-r--r--   0        0        0        0 2024-05-30 01:08:40.315281 r2r-0.2.2/r2r/examples/servers/__init__.py
+-rw-r--r--   0        0        0     1569 2024-05-30 01:08:40.315281 r2r-0.2.2/r2r/examples/servers/configurable_pipeline.py
+-rw-r--r--   0        0        0      147 2024-05-30 01:08:40.315281 r2r-0.2.2/r2r/integrations/__init__.py
+-rw-r--r--   0        0        0     1839 2024-05-30 01:08:40.315281 r2r-0.2.2/r2r/integrations/exa.py
+-rw-r--r--   0        0        0     1535 2024-05-30 01:08:40.315281 r2r-0.2.2/r2r/integrations/ionic.py
+-rw-r--r--   0        0        0     3940 2024-05-30 01:08:40.315281 r2r-0.2.2/r2r/integrations/serper.py
+-rw-r--r--   0        0        0      232 2024-05-30 01:08:40.315281 r2r-0.2.2/r2r/llms/__init__.py
+-rw-r--r--   0        0        0     3315 2024-05-30 01:08:40.315281 r2r-0.2.2/r2r/llms/litellm/base_litellm.py
+-rw-r--r--   0        0        0     3919 2024-05-30 01:08:40.315281 r2r-0.2.2/r2r/llms/llama_cpp/base_llama_cpp.py
+-rw-r--r--   0        0        0        0 2024-05-30 01:08:40.315281 r2r-0.2.2/r2r/llms/llama_cpp/model/__init__.py
+-rw-r--r--   0        0        0     3462 2024-05-30 01:08:40.315281 r2r-0.2.2/r2r/llms/openai/base_openai.py
+-rw-r--r--   0        0        0      410 2024-05-30 01:08:40.315281 r2r-0.2.2/r2r/main/__init__.py
+-rw-r--r--   0        0        0     1102 2024-05-30 01:08:40.315281 r2r-0.2.2/r2r/main/r2r_abstractions.py
+-rw-r--r--   0        0        0    24571 2024-05-30 01:08:40.315281 r2r-0.2.2/r2r/main/r2r_app.py
+-rw-r--r--   0        0        0     5529 2024-05-30 01:08:40.315281 r2r-0.2.2/r2r/main/r2r_client.py
+-rw-r--r--   0        0        0     4599 2024-05-30 01:08:40.315281 r2r-0.2.2/r2r/main/r2r_config.py
+-rw-r--r--   0        0        0    11331 2024-05-30 01:08:40.315281 r2r-0.2.2/r2r/main/r2r_factory.py
+-rw-r--r--   0        0        0      593 2024-05-30 01:08:40.315281 r2r-0.2.2/r2r/pipes/__init__.py
+-rw-r--r--   0        0        0     1266 2024-05-30 01:08:40.315281 r2r-0.2.2/r2r/pipes/abstractions/generator_pipe.py
+-rw-r--r--   0        0        0     1552 2024-05-30 01:08:40.315281 r2r-0.2.2/r2r/pipes/abstractions/search_pipe.py
+-rw-r--r--   0        0        0     7244 2024-05-30 01:08:40.315281 r2r-0.2.2/r2r/pipes/embedding_pipe.py
+-rw-r--r--   0        0        0     1272 2024-05-30 01:08:40.315281 r2r-0.2.2/r2r/pipes/eval_pipe.py
+-rw-r--r--   0        0        0     7590 2024-05-30 01:08:40.315281 r2r-0.2.2/r2r/pipes/parsing_pipe.py
+-rw-r--r--   0        0        0     3050 2024-05-30 01:08:40.315281 r2r-0.2.2/r2r/pipes/query_transform_pipe.py
+-rw-r--r--   0        0        0     2738 2024-05-30 01:08:40.315281 r2r-0.2.2/r2r/pipes/rag_pipe.py
+-rw-r--r--   0        0        0     3307 2024-05-30 01:08:40.315281 r2r-0.2.2/r2r/pipes/streaming_rag_pipe.py
+-rw-r--r--   0        0        0     2808 2024-05-30 01:08:40.315281 r2r-0.2.2/r2r/pipes/vector_search_pipe.py
+-rw-r--r--   0        0        0     3166 2024-05-30 01:08:40.315281 r2r-0.2.2/r2r/pipes/vector_storage_pipe.py
+-rw-r--r--   0        0        0       90 2024-05-30 01:08:40.315281 r2r-0.2.2/r2r/prompts/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 01:08:40.315281 r2r-0.2.2/r2r/prompts/local/__init__.py
+-rw-r--r--   0        0        0     4390 2024-05-30 01:08:40.315281 r2r-0.2.2/r2r/prompts/local/defaults.jsonl
+-rw-r--r--   0        0        0     1900 2024-05-30 01:08:40.315281 r2r-0.2.2/r2r/prompts/local/r2r_prompt_provider.py
+-rw-r--r--   0        0        0      539 2024-05-30 01:08:40.315281 r2r-0.2.2/r2r/vecs/__init__.py
+-rw-r--r--   0        0        0      363 2024-05-30 01:08:40.319281 r2r-0.2.2/r2r/vecs/adapter/__init__.py
+-rw-r--r--   0        0        0     3263 2024-05-30 01:08:40.319281 r2r-0.2.2/r2r/vecs/adapter/base.py
+-rw-r--r--   0        0        0     3170 2024-05-30 01:08:40.319281 r2r-0.2.2/r2r/vecs/adapter/markdown.py
+-rw-r--r--   0        0        0     1668 2024-05-30 01:08:40.319281 r2r-0.2.2/r2r/vecs/adapter/noop.py
+-rw-r--r--   0        0        0     5317 2024-05-30 01:08:40.319281 r2r-0.2.2/r2r/vecs/adapter/text.py
+-rw-r--r--   0        0        0     9350 2024-05-30 01:08:40.319281 r2r-0.2.2/r2r/vecs/client.py
+-rw-r--r--   0        0        0    36863 2024-05-30 01:08:40.319281 r2r-0.2.2/r2r/vecs/collection.py
+-rw-r--r--   0        0        0     1687 2024-05-30 01:08:40.319281 r2r-0.2.2/r2r/vecs/exc.py
+-rw-r--r--   0        0        0      213 2024-05-30 01:08:40.319281 r2r-0.2.2/r2r/vector_dbs/__init__.py
+-rw-r--r--   0        0        0     6379 2024-05-30 01:08:40.319281 r2r-0.2.2/r2r/vector_dbs/local/r2r_local_vector_db.py
+-rw-r--r--   0        0        0     6268 2024-05-30 01:08:40.319281 r2r-0.2.2/r2r/vector_dbs/pgvector/pgvector_db.py
+-rw-r--r--   0        0        0     7412 2024-05-30 01:08:40.319281 r2r-0.2.2/r2r/vector_dbs/qdrant/qdrant_db.py
+-rw-r--r--   0        0        0    14924 1970-01-01 00:00:00.000000 r2r-0.2.2/PKG-INFO
```

### Comparing `r2r-0.2.1/LICENSE.md` & `r2r-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/README.md` & `r2r-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/config.json` & `r2r-0.2.2/config.json`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/pyproject.toml` & `r2r-0.2.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "setuptools", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "r2r"
-version = "0.2.01"
+version = "0.2.02"
 description = "SciPhi R2R"
 authors = ["Owen Colegrove <owen@sciphi.ai>"]
 license = "MIT"
 readme = "README.md"
 include = ["config.json"]
 
 [tool.poetry.dependencies]
```

### Comparing `r2r-0.2.1/r2r/__init__.py` & `r2r-0.2.2/r2r/__init__.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/core/__init__.py` & `r2r-0.2.2/r2r/core/__init__.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/core/abstractions/document.py` & `r2r-0.2.2/r2r/core/abstractions/document.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/core/abstractions/prompt.py` & `r2r-0.2.2/r2r/core/abstractions/prompt.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/core/abstractions/search.py` & `r2r-0.2.2/r2r/core/abstractions/search.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/core/abstractions/vector.py` & `r2r-0.2.2/r2r/core/abstractions/vector.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/core/parsers/__init__.py` & `r2r-0.2.2/r2r/core/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/core/parsers/parser_impls.py` & `r2r-0.2.2/r2r/core/parsers/parser_impls.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/core/pipeline/base_pipeline.py` & `r2r-0.2.2/r2r/core/pipeline/base_pipeline.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/core/pipes/base_pipe.py` & `r2r-0.2.2/r2r/core/pipes/base_pipe.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/core/pipes/loggable_pipe.py` & `r2r-0.2.2/r2r/core/pipes/loggable_pipe.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/core/pipes/pipe_logging.py` & `r2r-0.2.2/r2r/core/pipes/pipe_logging.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/core/providers/base_provider.py` & `r2r-0.2.2/r2r/core/providers/base_provider.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/core/providers/embedding_provider.py` & `r2r-0.2.2/r2r/core/providers/embedding_provider.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/core/providers/eval_provider.py` & `r2r-0.2.2/r2r/core/providers/eval_provider.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/core/providers/llm_provider.py` & `r2r-0.2.2/r2r/core/providers/llm_provider.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/core/providers/prompt_provider.py` & `r2r-0.2.2/r2r/core/providers/prompt_provider.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/core/providers/vector_db_provider.py` & `r2r-0.2.2/r2r/core/providers/vector_db_provider.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/core/utils/base_utils.py` & `r2r-0.2.2/r2r/core/utils/base_utils.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/core/utils/splitter/text.py` & `r2r-0.2.2/r2r/core/utils/splitter/text.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/embeddings/dummy/provider.py` & `r2r-0.2.2/r2r/embeddings/dummy/provider.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/embeddings/openai/openai_base.py` & `r2r-0.2.2/r2r/embeddings/openai/openai_base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/embeddings/setence_transformer/sentence_transformer_base.py` & `r2r-0.2.2/r2r/embeddings/setence_transformer/sentence_transformer_base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/eval/llm/base_llm_eval.py` & `r2r-0.2.2/r2r/eval/llm/base_llm_eval.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/examples/custom_rag.py` & `r2r-0.2.2/r2r/examples/custom_rag.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/examples/data/aristotle.txt` & `r2r-0.2.2/r2r/examples/data/aristotle.txt`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/examples/data/lyft_2021.pdf` & `r2r-0.2.2/r2r/examples/data/lyft_2021.pdf`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/examples/data/pg_essay_1.html` & `r2r-0.2.2/r2r/examples/data/pg_essay_1.html`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/examples/data/pg_essay_2.html` & `r2r-0.2.2/r2r/examples/data/pg_essay_2.html`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/examples/data/pg_essay_3.html` & `r2r-0.2.2/r2r/examples/data/pg_essay_3.html`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/examples/data/pg_essay_4.html` & `r2r-0.2.2/r2r/examples/data/pg_essay_4.html`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/examples/data/pg_essay_5.html` & `r2r-0.2.2/r2r/examples/data/pg_essay_5.html`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/examples/data/screen_shot.png` & `r2r-0.2.2/r2r/examples/data/screen_shot.png`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/examples/data/uber_2021.pdf` & `r2r-0.2.2/r2r/examples/data/uber_2021.pdf`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/examples/demo.py` & `r2r-0.2.2/r2r/examples/demo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """A complete demo class for the R2R library."""
 
 import asyncio
 import json
-import glob
 import logging
 import os
 import time
 from typing import Optional
 
 import fire
 from fastapi.datastructures import UploadFile
```

### Comparing `r2r-0.2.1/r2r/examples/servers/configurable_pipeline.py` & `r2r-0.2.2/r2r/examples/servers/configurable_pipeline.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/integrations/exa.py` & `r2r-0.2.2/r2r/integrations/exa.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/integrations/ionic.py` & `r2r-0.2.2/r2r/integrations/ionic.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/integrations/serper.py` & `r2r-0.2.2/r2r/integrations/serper.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/llms/litellm/base_litellm.py` & `r2r-0.2.2/r2r/llms/litellm/base_litellm.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/llms/llama_cpp/base_llama_cpp.py` & `r2r-0.2.2/r2r/llms/llama_cpp/base_llama_cpp.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/llms/openai/base_openai.py` & `r2r-0.2.2/r2r/llms/openai/base_openai.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/main/r2r_abstractions.py` & `r2r-0.2.2/r2r/main/r2r_abstractions.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/main/r2r_app.py` & `r2r-0.2.2/r2r/main/r2r_app.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/main/r2r_client.py` & `r2r-0.2.2/r2r/main/r2r_client.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/main/r2r_config.py` & `r2r-0.2.2/r2r/main/r2r_config.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/main/r2r_factory.py` & `r2r-0.2.2/r2r/main/r2r_factory.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/pipes/__init__.py` & `r2r-0.2.2/r2r/pipes/__init__.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/pipes/abstractions/generator_pipe.py` & `r2r-0.2.2/r2r/pipes/abstractions/generator_pipe.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/pipes/abstractions/search_pipe.py` & `r2r-0.2.2/r2r/pipes/abstractions/search_pipe.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/pipes/embedding_pipe.py` & `r2r-0.2.2/r2r/pipes/embedding_pipe.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/pipes/eval_pipe.py` & `r2r-0.2.2/r2r/pipes/eval_pipe.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/pipes/parsing_pipe.py` & `r2r-0.2.2/r2r/pipes/parsing_pipe.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/pipes/query_transform_pipe.py` & `r2r-0.2.2/r2r/pipes/query_transform_pipe.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/pipes/rag_pipe.py` & `r2r-0.2.2/r2r/pipes/rag_pipe.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/pipes/streaming_rag_pipe.py` & `r2r-0.2.2/r2r/pipes/streaming_rag_pipe.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/pipes/vector_search_pipe.py` & `r2r-0.2.2/r2r/pipes/vector_search_pipe.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/pipes/vector_storage_pipe.py` & `r2r-0.2.2/r2r/pipes/vector_storage_pipe.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/prompts/local/defaults.jsonl` & `r2r-0.2.2/r2r/prompts/local/defaults.jsonl`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/prompts/local/r2r_prompt_provider.py` & `r2r-0.2.2/r2r/prompts/local/r2r_prompt_provider.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/vecs/__init__.py` & `r2r-0.2.2/r2r/vecs/__init__.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/vecs/adapter/base.py` & `r2r-0.2.2/r2r/vecs/adapter/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/vecs/adapter/markdown.py` & `r2r-0.2.2/r2r/vecs/adapter/markdown.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/vecs/adapter/noop.py` & `r2r-0.2.2/r2r/vecs/adapter/noop.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/vecs/adapter/text.py` & `r2r-0.2.2/r2r/vecs/adapter/text.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/vecs/client.py` & `r2r-0.2.2/r2r/vecs/client.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/vecs/collection.py` & `r2r-0.2.2/r2r/vecs/collection.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/vecs/exc.py` & `r2r-0.2.2/r2r/vecs/exc.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/vector_dbs/local/r2r_local_vector_db.py` & `r2r-0.2.2/r2r/vector_dbs/local/r2r_local_vector_db.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/vector_dbs/pgvector/pgvector_db.py` & `r2r-0.2.2/r2r/vector_dbs/pgvector/pgvector_db.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/r2r/vector_dbs/qdrant/qdrant_db.py` & `r2r-0.2.2/r2r/vector_dbs/qdrant/qdrant_db.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.1/PKG-INFO` & `r2r-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r2r
-Version: 0.2.1
+Version: 0.2.2
 Summary: SciPhi R2R
 License: MIT
 Author: Owen Colegrove
 Author-email: owen@sciphi.ai
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: r2r Version: 0.2.1 Summary: SciPhi R2R License: MIT
+Metadata-Version: 2.1 Name: r2r Version: 0.2.2 Summary: SciPhi R2R License: MIT
 Author: Owen Colegrove Author-email: owen@sciphi.ai Requires-Python:
 >=3.9,<3.13 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Provides-Extra: all Provides-Extra: exa Provides-Extra: ionic
 Provides-Extra: local-llm Provides-Extra: sentence-transformers-only Requires-
```

