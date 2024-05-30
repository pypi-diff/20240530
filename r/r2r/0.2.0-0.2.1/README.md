# Comparing `tmp/r2r-0.2.0.tar.gz` & `tmp/r2r-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r2r-0.2.0.tar", max compression
+gzip compressed data, was "r2r-0.2.1.tar", max compression
```

## Comparing `r2r-0.2.0.tar` & `r2r-0.2.1.tar`

### file list

```diff
@@ -1,96 +1,96 @@
--rw-r--r--   0        0        0     1082 2024-05-23 09:52:58.844723 r2r-0.2.0/LICENSE.md
--rw-r--r--   0        0        0    12944 2024-05-23 09:52:58.844723 r2r-0.2.0/README.md
--rw-r--r--   0        0        0     1181 2024-05-23 09:52:58.844723 r2r-0.2.0/config.json
--rw-r--r--   0        0        0     1980 2024-05-23 09:52:58.864723 r2r-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2047 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/__init__.py
--rw-r--r--   0        0        0     3083 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/__init__.py
--rw-r--r--   0        0        0     1371 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/abstractions/document.py
--rw-r--r--   0        0        0      186 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/abstractions/llm.py
--rw-r--r--   0        0        0     1083 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/abstractions/prompt.py
--rw-r--r--   0        0        0      813 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/abstractions/search.py
--rw-r--r--   0        0        0     1934 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/abstractions/vector.py
--rw-r--r--   0        0        0      538 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/parsers/__init__.py
--rw-r--r--   0        0        0      334 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/parsers/base_parser.py
--rw-r--r--   0        0        0    14096 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/parsers/parser_impls.py
--rw-r--r--   0        0        0     9066 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/pipeline/base_pipeline.py
--rw-r--r--   0        0        0     3803 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/pipes/base_pipe.py
--rw-r--r--   0        0        0     2215 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/pipes/loggable_pipe.py
--rw-r--r--   0        0        0    16417 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/pipes/pipe_logging.py
--rw-r--r--   0        0        0     1306 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/providers/base_provider.py
--rw-r--r--   0        0        0     2267 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/providers/embedding_provider.py
--rw-r--r--   0        0        0     1306 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/providers/eval_provider.py
--rw-r--r--   0        0        0     2345 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/providers/llm_provider.py
--rw-r--r--   0        0        0     1456 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/providers/prompt_provider.py
--rw-r--r--   0        0        0     2550 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/providers/vector_db_provider.py
--rw-r--r--   0        0        0      363 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/utils/__init__.py
--rw-r--r--   0        0        0      922 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/utils/base_utils.py
--rw-r--r--   0        0        0       95 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/utils/splitter/__init__.py
--rw-r--r--   0        0        0    66643 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/core/utils/splitter/text.py
--rw-r--r--   0        0        0      332 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/embeddings/__init__.py
--rw-r--r--   0        0        0     2363 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/embeddings/dummy/provider.py
--rw-r--r--   0        0        0     6309 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/embeddings/openai/openai_base.py
--rw-r--r--   0        0        0     6238 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/embeddings/setence_transformer/sentence_transformer_base.py
--rw-r--r--   0        0        0       78 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/eval/__init__.py
--rw-r--r--   0        0        0     2867 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/eval/llm/base_llm_eval.py
--rw-r--r--   0        0        0        0 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/examples/__init__.py
--rw-r--r--   0        0        0     3067 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/examples/custom_rag.py
--rw-r--r--   0        0        0    73353 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/examples/data/aristotle.txt
--rw-r--r--   0        0        0       49 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/examples/data/example_postgres_logger_config.json
--rw-r--r--   0        0        0       91 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/examples/data/example_qdrant_config.json
--rw-r--r--   0        0        0      455 2024-05-23 09:52:58.864723 r2r-0.2.0/r2r/examples/data/example_rerank_config.json
--rw-r--r--   0        0        0  1440303 2024-05-23 09:52:58.872723 r2r-0.2.0/r2r/examples/data/lyft_2021.pdf
--rw-r--r--   0        0        0   131542 2024-05-23 09:52:58.872723 r2r-0.2.0/r2r/examples/data/pg_essay_1.html
--rw-r--r--   0        0        0   125150 2024-05-23 09:52:58.872723 r2r-0.2.0/r2r/examples/data/pg_essay_2.html
--rw-r--r--   0        0        0   124948 2024-05-23 09:52:58.872723 r2r-0.2.0/r2r/examples/data/pg_essay_3.html
--rw-r--r--   0        0        0   118147 2024-05-23 09:52:58.872723 r2r-0.2.0/r2r/examples/data/pg_essay_4.html
--rw-r--r--   0        0        0   123820 2024-05-23 09:52:58.872723 r2r-0.2.0/r2r/examples/data/pg_essay_5.html
--rw-r--r--   0        0        0   791764 2024-05-23 09:52:58.876723 r2r-0.2.0/r2r/examples/data/screen_shot.png
--rw-r--r--   0        0        0       19 2024-05-23 09:52:58.876723 r2r-0.2.0/r2r/examples/data/test.txt
--rw-r--r--   0        0        0  1880483 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/examples/data/uber_2021.pdf
--rw-r--r--   0        0        0    11969 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/examples/demo.py
--rw-r--r--   0        0        0        0 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/examples/servers/__init__.py
--rw-r--r--   0        0        0     1569 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/examples/servers/configurable_pipeline.py
--rw-r--r--   0        0        0      147 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/integrations/__init__.py
--rw-r--r--   0        0        0     1839 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/integrations/exa.py
--rw-r--r--   0        0        0     1535 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/integrations/ionic.py
--rw-r--r--   0        0        0     3940 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/integrations/serper.py
--rw-r--r--   0        0        0      232 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/llms/__init__.py
--rw-r--r--   0        0        0     3315 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/llms/litellm/base_litellm.py
--rw-r--r--   0        0        0     3919 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/llms/llama_cpp/base_llama_cpp.py
--rw-r--r--   0        0        0        0 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/llms/llama_cpp/model/__init__.py
--rw-r--r--   0        0        0     3462 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/llms/openai/base_openai.py
--rw-r--r--   0        0        0      410 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/main/__init__.py
--rw-r--r--   0        0        0     1102 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/main/r2r_abstractions.py
--rw-r--r--   0        0        0    23069 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/main/r2r_app.py
--rw-r--r--   0        0        0     5529 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/main/r2r_client.py
--rw-r--r--   0        0        0     4632 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/main/r2r_config.py
--rw-r--r--   0        0        0    11331 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/main/r2r_factory.py
--rw-r--r--   0        0        0      593 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/pipes/__init__.py
--rw-r--r--   0        0        0     1266 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/pipes/abstractions/generator_pipe.py
--rw-r--r--   0        0        0     1588 2024-05-23 09:52:58.884723 r2r-0.2.0/r2r/pipes/abstractions/search_pipe.py
--rw-r--r--   0        0        0     7244 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/pipes/embedding_pipe.py
--rw-r--r--   0        0        0     1407 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/pipes/eval_pipe.py
--rw-r--r--   0        0        0     7590 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/pipes/parsing_pipe.py
--rw-r--r--   0        0        0     3050 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/pipes/query_transform_pipe.py
--rw-r--r--   0        0        0     2738 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/pipes/rag_pipe.py
--rw-r--r--   0        0        0     3317 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/pipes/streaming_rag_pipe.py
--rw-r--r--   0        0        0     2798 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/pipes/vector_search_pipe.py
--rw-r--r--   0        0        0     3073 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/pipes/vector_storage_pipe.py
--rw-r--r--   0        0        0       90 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/prompts/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/prompts/local/__init__.py
--rw-r--r--   0        0        0     4390 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/prompts/local/defaults.jsonl
--rw-r--r--   0        0        0     1900 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/prompts/local/r2r_prompt_provider.py
--rw-r--r--   0        0        0      539 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/vecs/__init__.py
--rw-r--r--   0        0        0      363 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/vecs/adapter/__init__.py
--rw-r--r--   0        0        0     3263 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/vecs/adapter/base.py
--rw-r--r--   0        0        0     3170 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/vecs/adapter/markdown.py
--rw-r--r--   0        0        0     1668 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/vecs/adapter/noop.py
--rw-r--r--   0        0        0     5317 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/vecs/adapter/text.py
--rw-r--r--   0        0        0     9350 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/vecs/client.py
--rw-r--r--   0        0        0    36863 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/vecs/collection.py
--rw-r--r--   0        0        0     1687 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/vecs/exc.py
--rw-r--r--   0        0        0      213 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/vector_dbs/__init__.py
--rw-r--r--   0        0        0     6379 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/vector_dbs/local/r2r_local_vector_db.py
--rw-r--r--   0        0        0     6268 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/vector_dbs/pgvector/pgvector_db.py
--rw-r--r--   0        0        0     7412 2024-05-23 09:52:58.888723 r2r-0.2.0/r2r/vector_dbs/qdrant/qdrant_db.py
--rw-r--r--   0        0        0    14924 1970-01-01 00:00:00.000000 r2r-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-05-30 00:51:23.130715 r2r-0.2.1/LICENSE.md
+-rw-r--r--   0        0        0    12944 2024-05-30 00:51:23.130715 r2r-0.2.1/README.md
+-rw-r--r--   0        0        0     1151 2024-05-30 00:51:23.134715 r2r-0.2.1/config.json
+-rw-r--r--   0        0        0     1980 2024-05-30 00:51:23.150715 r2r-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2047 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/__init__.py
+-rw-r--r--   0        0        0     3083 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/__init__.py
+-rw-r--r--   0        0        0     1371 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/abstractions/document.py
+-rw-r--r--   0        0        0      186 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/abstractions/llm.py
+-rw-r--r--   0        0        0     1083 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/abstractions/prompt.py
+-rw-r--r--   0        0        0      813 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/abstractions/search.py
+-rw-r--r--   0        0        0     1934 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/abstractions/vector.py
+-rw-r--r--   0        0        0      538 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/parsers/__init__.py
+-rw-r--r--   0        0        0      334 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/parsers/base_parser.py
+-rw-r--r--   0        0        0    14096 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/parsers/parser_impls.py
+-rw-r--r--   0        0        0     9358 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/pipeline/base_pipeline.py
+-rw-r--r--   0        0        0     3949 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/pipes/base_pipe.py
+-rw-r--r--   0        0        0     2409 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/pipes/loggable_pipe.py
+-rw-r--r--   0        0        0    16417 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/pipes/pipe_logging.py
+-rw-r--r--   0        0        0     1306 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/providers/base_provider.py
+-rw-r--r--   0        0        0     2267 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/providers/embedding_provider.py
+-rw-r--r--   0        0        0     1029 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/providers/eval_provider.py
+-rw-r--r--   0        0        0     2328 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/providers/llm_provider.py
+-rw-r--r--   0        0        0     1456 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/providers/prompt_provider.py
+-rw-r--r--   0        0        0     2550 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/providers/vector_db_provider.py
+-rw-r--r--   0        0        0      363 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/utils/__init__.py
+-rw-r--r--   0        0        0      922 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/utils/base_utils.py
+-rw-r--r--   0        0        0       95 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/utils/splitter/__init__.py
+-rw-r--r--   0        0        0    66643 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/core/utils/splitter/text.py
+-rw-r--r--   0        0        0      332 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/embeddings/__init__.py
+-rw-r--r--   0        0        0     2363 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/embeddings/dummy/provider.py
+-rw-r--r--   0        0        0     6309 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/embeddings/openai/openai_base.py
+-rw-r--r--   0        0        0     6238 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/embeddings/setence_transformer/sentence_transformer_base.py
+-rw-r--r--   0        0        0       78 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/eval/__init__.py
+-rw-r--r--   0        0        0     2867 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/eval/llm/base_llm_eval.py
+-rw-r--r--   0        0        0        0 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/examples/__init__.py
+-rw-r--r--   0        0        0     3091 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/examples/custom_rag.py
+-rw-r--r--   0        0        0    73353 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/examples/data/aristotle.txt
+-rw-r--r--   0        0        0       49 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/examples/data/example_postgres_logger_config.json
+-rw-r--r--   0        0        0       91 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/examples/data/example_qdrant_config.json
+-rw-r--r--   0        0        0      455 2024-05-30 00:51:23.150715 r2r-0.2.1/r2r/examples/data/example_rerank_config.json
+-rw-r--r--   0        0        0  1440303 2024-05-30 00:51:23.158715 r2r-0.2.1/r2r/examples/data/lyft_2021.pdf
+-rw-r--r--   0        0        0   131542 2024-05-30 00:51:23.158715 r2r-0.2.1/r2r/examples/data/pg_essay_1.html
+-rw-r--r--   0        0        0   125150 2024-05-30 00:51:23.158715 r2r-0.2.1/r2r/examples/data/pg_essay_2.html
+-rw-r--r--   0        0        0   124948 2024-05-30 00:51:23.158715 r2r-0.2.1/r2r/examples/data/pg_essay_3.html
+-rw-r--r--   0        0        0   118147 2024-05-30 00:51:23.158715 r2r-0.2.1/r2r/examples/data/pg_essay_4.html
+-rw-r--r--   0        0        0   123820 2024-05-30 00:51:23.158715 r2r-0.2.1/r2r/examples/data/pg_essay_5.html
+-rw-r--r--   0        0        0   791764 2024-05-30 00:51:23.162715 r2r-0.2.1/r2r/examples/data/screen_shot.png
+-rw-r--r--   0        0        0       19 2024-05-30 00:51:23.162715 r2r-0.2.1/r2r/examples/data/test.txt
+-rw-r--r--   0        0        0  1880483 2024-05-30 00:51:23.170715 r2r-0.2.1/r2r/examples/data/uber_2021.pdf
+-rw-r--r--   0        0        0    12004 2024-05-30 00:51:23.170715 r2r-0.2.1/r2r/examples/demo.py
+-rw-r--r--   0        0        0        0 2024-05-30 00:51:23.170715 r2r-0.2.1/r2r/examples/servers/__init__.py
+-rw-r--r--   0        0        0     1569 2024-05-30 00:51:23.170715 r2r-0.2.1/r2r/examples/servers/configurable_pipeline.py
+-rw-r--r--   0        0        0      147 2024-05-30 00:51:23.170715 r2r-0.2.1/r2r/integrations/__init__.py
+-rw-r--r--   0        0        0     1839 2024-05-30 00:51:23.170715 r2r-0.2.1/r2r/integrations/exa.py
+-rw-r--r--   0        0        0     1535 2024-05-30 00:51:23.170715 r2r-0.2.1/r2r/integrations/ionic.py
+-rw-r--r--   0        0        0     3940 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/integrations/serper.py
+-rw-r--r--   0        0        0      232 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/llms/__init__.py
+-rw-r--r--   0        0        0     3315 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/llms/litellm/base_litellm.py
+-rw-r--r--   0        0        0     3919 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/llms/llama_cpp/base_llama_cpp.py
+-rw-r--r--   0        0        0        0 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/llms/llama_cpp/model/__init__.py
+-rw-r--r--   0        0        0     3462 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/llms/openai/base_openai.py
+-rw-r--r--   0        0        0      410 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/main/__init__.py
+-rw-r--r--   0        0        0     1102 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/main/r2r_abstractions.py
+-rw-r--r--   0        0        0    24571 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/main/r2r_app.py
+-rw-r--r--   0        0        0     5529 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/main/r2r_client.py
+-rw-r--r--   0        0        0     4599 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/main/r2r_config.py
+-rw-r--r--   0        0        0    11331 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/main/r2r_factory.py
+-rw-r--r--   0        0        0      593 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/pipes/__init__.py
+-rw-r--r--   0        0        0     1266 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/pipes/abstractions/generator_pipe.py
+-rw-r--r--   0        0        0     1552 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/pipes/abstractions/search_pipe.py
+-rw-r--r--   0        0        0     7244 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/pipes/embedding_pipe.py
+-rw-r--r--   0        0        0     1272 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/pipes/eval_pipe.py
+-rw-r--r--   0        0        0     7590 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/pipes/parsing_pipe.py
+-rw-r--r--   0        0        0     3050 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/pipes/query_transform_pipe.py
+-rw-r--r--   0        0        0     2738 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/pipes/rag_pipe.py
+-rw-r--r--   0        0        0     3307 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/pipes/streaming_rag_pipe.py
+-rw-r--r--   0        0        0     2808 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/pipes/vector_search_pipe.py
+-rw-r--r--   0        0        0     3166 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/pipes/vector_storage_pipe.py
+-rw-r--r--   0        0        0       90 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/prompts/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/prompts/local/__init__.py
+-rw-r--r--   0        0        0     4390 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/prompts/local/defaults.jsonl
+-rw-r--r--   0        0        0     1900 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/prompts/local/r2r_prompt_provider.py
+-rw-r--r--   0        0        0      539 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/vecs/__init__.py
+-rw-r--r--   0        0        0      363 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/vecs/adapter/__init__.py
+-rw-r--r--   0        0        0     3263 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/vecs/adapter/base.py
+-rw-r--r--   0        0        0     3170 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/vecs/adapter/markdown.py
+-rw-r--r--   0        0        0     1668 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/vecs/adapter/noop.py
+-rw-r--r--   0        0        0     5317 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/vecs/adapter/text.py
+-rw-r--r--   0        0        0     9350 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/vecs/client.py
+-rw-r--r--   0        0        0    36863 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/vecs/collection.py
+-rw-r--r--   0        0        0     1687 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/vecs/exc.py
+-rw-r--r--   0        0        0      213 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/vector_dbs/__init__.py
+-rw-r--r--   0        0        0     6379 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/vector_dbs/local/r2r_local_vector_db.py
+-rw-r--r--   0        0        0     6268 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/vector_dbs/pgvector/pgvector_db.py
+-rw-r--r--   0        0        0     7412 2024-05-30 00:51:23.174715 r2r-0.2.1/r2r/vector_dbs/qdrant/qdrant_db.py
+-rw-r--r--   0        0        0    14924 1970-01-01 00:00:00.000000 r2r-0.2.1/PKG-INFO
```

### Comparing `r2r-0.2.0/LICENSE.md` & `r2r-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/README.md` & `r2r-0.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
 ```
 
 ### Streaming Response
 
 For streaming results from a RAG query, use the following command:
 
 ```bash
-python -m r2r.examples.demo rag --query="What was Lyft's profit in 2020?" --streaming=True
+python -m r2r.examples.demo rag --query="What was Lyft's profit in 2020?" --streaming=true
 ```
 
 **Demo Output:**
 
 ```plaintext
 r2r.main.r2r_config - INFO - Loading configuration from <YOUR_WORKDIR>/config.json - 2024-05-20 22:27:31,890
 ...
@@ -256,15 +256,15 @@
    ```bash
    python -m r2r.examples.demo rag --query="What was Uber's profit in 2020?" --base_url=http://localhost:8000
    ```
    This command sends the RAG query to the server and retrieves the generated response.
 
 4. **Run a RAG Stream**:
    ```bash
-   python -m r2r.examples.demo rag --query="What was Lyft's profit in 2020?" --streaming=True --base_url=http://localhost:8000
+   python -m r2r.examples.demo rag --query="What was Lyft's profit in 2020?" --streaming=true --base_url=http://localhost:8000
    ```
    This command streams the RAG query results from the server.
 
 ### Server-Client Summary
 
 By using the server-client model, you can extend the basic R2R demo to support more scalable and modular deployments. The server handles requests and performs heavy computations, while clients can communicate with the server to perform ingestion, search, RAG, and other operations, as shown in the examples above. For detailed setup and basic functionality, refer back to the [R2R Demo](#r2r-demo).
```

#### html2text {}

```diff
@@ -76,15 +76,15 @@
 ( content="Uber's profit in 2020 was a net loss of $6,768 million [10].",
 role='assistant', function_call=None, tool_calls=None ) ) ],
 created=1716268695, model='gpt-3.5-turbo-0125', object='chat.completion',
 system_fingerprint=None, usage=CompletionUsage( completion_tokens=20,
 prompt_tokens=1470, total_tokens=1490 ) ) ] } ``` ### Streaming Response For
 streaming results from a RAG query, use the following command: ```bash python -
 m r2r.examples.demo rag --query="What was Lyft's profit in 2020?" --
-streaming=True ``` **Demo Output:** ```plaintext r2r.main.r2r_config - INFO -
+streaming=true ``` **Demo Output:** ```plaintext r2r.main.r2r_config - INFO -
 Loading configuration from /config.json - 2024-05-20 22:27:31,890 ... ["
 {\"id\":\"808c47c5-ebef-504a-a230-aa9ddcfbd87 .... Lyft reported a net loss of
 $1,752,857,000 in 2020 according to [2]. Therefore, Lyft did not make a profit
 in 2020. Time taken to stream RAG response: 2.79 seconds ``` ## Document
 Management Demo ### Document Deletion To delete a document by its ID, or any
 other metadata field, use the delete command. For example, to delete all chunks
 corresponding to the uploaded file `aristotle.txt`, we can call delete on the
@@ -107,15 +107,15 @@
 ```bash python -m r2r.examples.demo search --query="Who was Aristotle?" --
 base_url=http://localhost:8000 ``` This command sends the search query to the
 server and retrieves the results. 3. **Run a RAG Completion**: ```bash python -
 m r2r.examples.demo rag --query="What was Uber's profit in 2020?" --
 base_url=http://localhost:8000 ``` This command sends the RAG query to the
 server and retrieves the generated response. 4. **Run a RAG Stream**: ```bash
 python -m r2r.examples.demo rag --query="What was Lyft's profit in 2020?" --
-streaming=True --base_url=http://localhost:8000 ``` This command streams the
+streaming=true --base_url=http://localhost:8000 ``` This command streams the
 RAG query results from the server. ### Server-Client Summary By using the
 server-client model, you can extend the basic R2R demo to support more scalable
 and modular deployments. The server handles requests and performs heavy
 computations, while clients can communicate with the server to perform
 ingestion, search, RAG, and other operations, as shown in the examples above.
 For detailed setup and basic functionality, refer back to the [R2R Demo](#r2r-
 demo). # Core Abstractions The framework revolves around three core
```

### Comparing `r2r-0.2.0/config.json` & `r2r-0.2.1/config.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'eval'": "{delete: ['sampling_fraction']}"}*

```diff
@@ -19,16 +19,15 @@
         }
     },
     "eval": {
         "llm": {
             "model": "gpt-4o",
             "provider": "openai"
         },
-        "provider": "local",
-        "sampling_fraction": 1.0
+        "provider": "local"
     },
     "ingestion": {
         "selected_parsers": {
             "csv": "default",
             "docx": "default",
             "gif": "default",
             "html": "default",
```

### Comparing `r2r-0.2.0/pyproject.toml` & `r2r-0.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "setuptools", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "r2r"
-version = "0.2.00"
+version = "0.2.01"
 description = "SciPhi R2R"
 authors = ["Owen Colegrove <owen@sciphi.ai>"]
 license = "MIT"
 readme = "README.md"
 include = ["config.json"]
 
 [tool.poetry.dependencies]
```

### Comparing `r2r-0.2.0/r2r/__init__.py` & `r2r-0.2.1/r2r/__init__.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/core/__init__.py` & `r2r-0.2.1/r2r/core/__init__.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/core/abstractions/document.py` & `r2r-0.2.1/r2r/core/abstractions/document.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/core/abstractions/prompt.py` & `r2r-0.2.1/r2r/core/abstractions/prompt.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/core/abstractions/search.py` & `r2r-0.2.1/r2r/core/abstractions/search.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/core/abstractions/vector.py` & `r2r-0.2.1/r2r/core/abstractions/vector.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/core/parsers/__init__.py` & `r2r-0.2.1/r2r/core/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/core/parsers/parser_impls.py` & `r2r-0.2.1/r2r/core/parsers/parser_impls.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/core/pipeline/base_pipeline.py` & `r2r-0.2.1/r2r/core/pipeline/base_pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Base pipeline class for running a sequence of pipes."""
-
 import asyncio
+from contextlib import asynccontextmanager
 import logging
 import uuid
 from enum import Enum
 from typing import Any, AsyncGenerator, Optional
 
 from ..pipes.base_pipe import AsyncPipe, AsyncState
 from ..pipes.pipe_logging import PipeLoggingConnectionSingleton
@@ -17,28 +17,37 @@
     EVAL = "eval"
     INGESTION = "ingestion"
     SEARCH = "search"
     RAG = "rag"
     OTHER = "other"
 
 
+@asynccontextmanager
+async def manage_run_id(pipeline: "Pipeline"):
+    try:
+        pipeline.run_id = generate_run_id()
+        yield
+    finally:
+        pipeline.run_id = None
+
+
 class Pipeline:
     """Pipeline class for running a sequence of pipes."""
 
     pipeline_type: str = "other"
 
     def __init__(
         self, pipe_logger: Optional[PipeLoggingConnectionSingleton] = None
     ):
         self.pipes: list[AsyncPipe] = []
         self.upstream_outputs: list[list[dict[str, str]]] = []
         self.pipe_logger = pipe_logger or PipeLoggingConnectionSingleton()
         self.futures = {}
         self.level = 0
-        self.run_id = None
+        # self.run_id = None
 
     def add_pipe(
         self,
         pipe: AsyncPipe,
         add_upstream_outputs: Optional[list[dict[str, str]]] = None,
         *args,
         **kwargs,
@@ -63,47 +72,45 @@
         except ValueError:
             raise ValueError(
                 f"Invalid pipeline type: {self.pipeline_type}, must be one of {PipelineTypes.__members__.keys()}"
             )
 
         self.state = state or AsyncState()
         current_input = input
-        self.run_id = generate_run_id()
-        await self.pipe_logger.log(
-            pipe_run_id=self.run_id,
-            key="pipeline_type",
-            value=self.pipeline_type,
-            is_pipeline_info=True,
-        )
-        try:
-            for pipe_num in range(len(self.pipes)):
-                config_name = self.pipes[pipe_num].config.name
-                self.futures[config_name] = asyncio.Future()
-
-                current_input = self._run_pipe(
-                    pipe_num, current_input, *args, **kwargs
-                )
-                self.futures[config_name].set_result(current_input)
+        async with manage_run_id(self):
+            await self.pipe_logger.log(
+                pipe_run_id=self.run_id,
+                key="pipeline_type",
+                value=self.pipeline_type,
+                is_pipeline_info=True,
+            )
+            try:
+                for pipe_num in range(len(self.pipes)):
+                    config_name = self.pipes[pipe_num].config.name
+                    self.futures[config_name] = asyncio.Future()
+
+                    current_input = self._run_pipe(
+                        pipe_num,
+                        self.run_id,
+                        current_input,
+                        *args,
+                        **kwargs,  # pass run_id to retain value throughout execution.
+                    )
+                    self.futures[config_name].set_result(current_input)
 
-            if not streaming:
-                final_result = await self._consume_all(current_input)
-                return final_result
-            else:
-                return current_input
-        except Exception as error:
-            logger.error(f"Pipeline failed with error: {error}")
-            # await self.pipe_logger.log(
-            #     pipe_run_id=run_id,
-            #     key="error",
-            #     value=error,
-            #     is_pipeline_info=False,
-            # )
-            raise error
-        finally:
-            self.run_id = None
+                if not streaming:
+                    final_result = await self._consume_all(current_input)
+                    return final_result
+                else:
+                    return current_input
+            except Exception as error:
+                logger.error(f"Pipeline failed with error: {error}")
+                raise error
+            finally:
+                pass
 
     async def _consume_all(self, gen: AsyncGenerator) -> list[Any]:
         result = []
         async for item in gen:
             if hasattr(
                 item, "__aiter__"
             ):  # Check if the item is an async generator
@@ -112,14 +119,15 @@
             else:
                 result.append(item)
         return result
 
     async def _run_pipe(
         self,
         pipe_num: int,
+        run_id: uuid.UUID,
         input: Any,
         *args: Any,
         **kwargs: Any,
     ):
         # Collect inputs, waiting for the necessary futures
         pipe = self.pipes[pipe_num]
         add_upstream_outputs = self.sort_upstream_outputs(
@@ -168,15 +176,15 @@
                     prev_output_field
                 ]
 
         # Handle the pipe generator
         async for ele in await pipe.run(
             pipe.Input(**input_dict),
             self.state,
-            run_id=self.run_id,
+            run_id=run_id,
             *args,
             **kwargs,
         ):
             yield ele
 
     def sort_upstream_outputs(
         self, add_upstream_outputs: list[dict[str, str]]
```

### Comparing `r2r-0.2.0/r2r/core/pipes/base_pipe.py` & `r2r-0.2.1/r2r/core/pipes/base_pipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from contextlib import asynccontextmanager
 import asyncio
 import logging
 import uuid
 from abc import ABC, abstractmethod
 from enum import Enum
 from typing import Any, AsyncGenerator, Optional
 
@@ -64,14 +65,26 @@
                 if inner_key not in self.data[outer_key]:
                     raise ValueError(
                         f"Key {inner_key} does not exist in the state."
                     )
                 del self.data[outer_key][inner_key]
 
 
+@asynccontextmanager
+async def manage_run_info(
+    pipe: "AsyncPipe", run_id: Optional[uuid.UUID] = None
+):
+    try:
+        run_id = run_id or generate_run_id()
+        pipe._run_info = PipeRunInfo(run_id=run_id)
+        yield
+    finally:
+        pipe.run_id = None
+
+
 class AsyncPipe(ABC):
     """An asynchronous pipe for processing data."""
 
     class PipeConfig(BaseModel):
         """Configuration for a pipe."""
 
         name: str = "default_pipe"
@@ -93,14 +106,15 @@
         self,
         type: PipeType = PipeType.OTHER,
         config: Optional[PipeConfig] = None,
     ):
         self._config = config or self.PipeConfig()
         self._run_info = None
         self._type = type
+
         logger.info(f"Initialized pipe {self.config.name} of type {self.type}")
 
     @property
     def config(self) -> PipeConfig:
         return self._config
 
     @property
@@ -115,21 +129,16 @@
         self,
         input: Input,
         state: AsyncState,
         run_id: Optional[uuid.UUID] = None,
         *args: Any,
         **kwargs: Any,
     ) -> AsyncGenerator[Any, None]:
-        await self._initiate_run(run_id)
-        result = self._run_logic(input, state)
-        return result
+        async with manage_run_info(self, run_id):
+            result = self._run_logic(input, state)
+            return result
 
     @abstractmethod
     async def _run_logic(
         self, input: Input, state: AsyncState, *args: Any, **kwargs: Any
     ) -> AsyncGenerator[Any, None]:
         pass
-
-    async def _initiate_run(self, run_id: Optional[uuid.UUID] = None):
-        if not run_id:
-            run_id = generate_run_id()
-        self._run_info = PipeRunInfo(run_id=run_id)
```

### Comparing `r2r-0.2.0/r2r/core/pipes/loggable_pipe.py` & `r2r-0.2.1/r2r/core/pipes/loggable_pipe.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 import uuid
 from typing import Any, AsyncGenerator, Optional
 
-from .base_pipe import AsyncPipe, AsyncState, PipeType
+from .base_pipe import AsyncPipe, AsyncState, PipeType, manage_run_info
 from .pipe_logging import PipeLoggingConnectionSingleton
 
 
 class LoggableAsyncPipe(AsyncPipe):
     """An asynchronous pipe for processing data with logging capabilities."""
 
     class PipeConfig(AsyncPipe.PipeConfig):
@@ -17,15 +17,15 @@
 
     def __init__(
         self,
         pipe_logger: Optional[PipeLoggingConnectionSingleton] = None,
         type: PipeType = PipeType.OTHER,
         config: Optional[AsyncPipe.PipeConfig] = None,
         *args,
-        **kwargs
+        **kwargs,
     ):
         if not pipe_logger:
             pipe_logger = PipeLoggingConnectionSingleton()
         self.pipe_logger = pipe_logger
         self.log_queue = asyncio.Queue()
         self.log_worker_task = None
 
@@ -44,24 +44,27 @@
 
     async def run(
         self,
         input: AsyncPipe.Input,
         state: AsyncState,
         run_id: Optional[uuid.UUID] = None,
         *args: Any,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> AsyncGenerator[Any, None]:
         """Run the pipe with logging capabilities."""
 
         async def wrapped_run() -> AsyncGenerator[Any, None]:
-            await self._initiate_run(run_id)
-            self.log_worker_task = asyncio.create_task(self.log_worker())
-            try:
-                async for result in self._run_logic(
-                    input, state, *args, **kwargs
-                ):
-                    yield result
-            finally:
-                await self.log_queue.join()
-                self.log_worker_task.cancel()
+            async with manage_run_info(self, run_id):
+                self.log_worker_task = asyncio.create_task(
+                    self.log_worker(), name=f"log-worker-{self.config.name}"
+                )
+                try:
+                    async for result in self._run_logic(
+                        input, state, *args, **kwargs
+                    ):
+                        yield result
+                finally:
+                    await self.log_queue.join()
+                    self.log_worker_task.cancel()
+                    self.log_queue = asyncio.Queue()
 
         return wrapped_run()
```

### Comparing `r2r-0.2.0/r2r/core/pipes/pipe_logging.py` & `r2r-0.2.1/r2r/core/pipes/pipe_logging.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/core/providers/base_provider.py` & `r2r-0.2.1/r2r/core/providers/base_provider.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/core/providers/embedding_provider.py` & `r2r-0.2.1/r2r/core/providers/embedding_provider.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/core/providers/eval_provider.py` & `r2r-0.2.1/r2r/core/providers/eval_provider.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-import random
 from abc import abstractmethod
-from typing import Optional, Union
+from typing import Union
 
 from .base_provider import Provider, ProviderConfig
 from .llm_provider import LLMConfig
 
 
 class EvalConfig(ProviderConfig):
     """A base eval config class"""
 
-    sampling_fraction: float = 0.0
     llm: LLMConfig
 
     def validate(self) -> None:
         if self.provider not in self.supported_providers:
             raise ValueError(f"Provider {self.provider} not supported.")
 
     @property
@@ -28,19 +26,11 @@
         if not isinstance(config, EvalConfig):
             raise ValueError(
                 "EvalProvider must be initialized with a `EvalConfig`."
             )
 
         super().__init__(config)
 
-    @abstractmethod
-    def _evaluate(
-        self, query: str, context: str, completion: str
-    ) -> dict[str, dict[str, Union[str, float]]]:
-        pass
-
     def evaluate(
         self, query: str, context: str, completion: str
-    ) -> Optional[dict]:
-        if random.random() < self.config.sampling_fraction:
-            return self._evaluate(query, context, completion)
-        return None
+    ) -> dict[str, dict[str, Union[str, float]]]:
+        return self._evaluate(query, context, completion)
```

### Comparing `r2r-0.2.0/r2r/core/providers/llm_provider.py` & `r2r-0.2.1/r2r/core/providers/llm_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 class GenerationConfig(BaseModel):
     temperature: float = 0.1
     top_p: float = 1.0
     top_k: int = 100
     max_tokens_to_sample: int = 1_024
-    model: Optional[str] = None
+    model: str
     stream: bool = False
     functions: Optional[list[dict]] = None
     skip_special_tokens: bool = False
     stop_token: Optional[str] = None
     num_beams: int = 1
     do_sample: bool = True
     # Additional args to pass to the generation config
```

### Comparing `r2r-0.2.0/r2r/core/providers/prompt_provider.py` & `r2r-0.2.1/r2r/core/providers/prompt_provider.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/core/providers/vector_db_provider.py` & `r2r-0.2.1/r2r/core/providers/vector_db_provider.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/core/utils/base_utils.py` & `r2r-0.2.1/r2r/core/utils/base_utils.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/core/utils/splitter/text.py` & `r2r-0.2.1/r2r/core/utils/splitter/text.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/embeddings/dummy/provider.py` & `r2r-0.2.1/r2r/embeddings/dummy/provider.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/embeddings/openai/openai_base.py` & `r2r-0.2.1/r2r/embeddings/openai/openai_base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/embeddings/setence_transformer/sentence_transformer_base.py` & `r2r-0.2.1/r2r/embeddings/setence_transformer/sentence_transformer_base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/eval/llm/base_llm_eval.py` & `r2r-0.2.1/r2r/eval/llm/base_llm_eval.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/examples/custom_rag.py` & `r2r-0.2.1/r2r/examples/custom_rag.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from r2r import (
     GenerationConfig,
     PipeLoggingConnectionSingleton,
     R2RConfig,
     R2RPipeFactory,
     R2RProviderFactory,
+    R2RPipelineFactory,
     R2RQueryTransformPipe,
     RAGPipeline,
     run_pipeline,
 )
 
 if __name__ == "__main__":
     # Load the default configuration
```

### Comparing `r2r-0.2.0/r2r/examples/data/aristotle.txt` & `r2r-0.2.1/r2r/examples/data/aristotle.txt`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/examples/data/lyft_2021.pdf` & `r2r-0.2.1/r2r/examples/data/lyft_2021.pdf`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/examples/data/pg_essay_1.html` & `r2r-0.2.1/r2r/examples/data/pg_essay_1.html`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/examples/data/pg_essay_2.html` & `r2r-0.2.1/r2r/examples/data/pg_essay_2.html`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/examples/data/pg_essay_3.html` & `r2r-0.2.1/r2r/examples/data/pg_essay_3.html`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/examples/data/pg_essay_4.html` & `r2r-0.2.1/r2r/examples/data/pg_essay_4.html`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/examples/data/pg_essay_5.html` & `r2r-0.2.1/r2r/examples/data/pg_essay_5.html`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/examples/data/screen_shot.png` & `r2r-0.2.1/r2r/examples/data/screen_shot.png`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/examples/data/uber_2021.pdf` & `r2r-0.2.1/r2r/examples/data/uber_2021.pdf`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/examples/demo.py` & `r2r-0.2.1/r2r/examples/demo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """A complete demo class for the R2R library."""
 
 import asyncio
 import json
+import glob
 import logging
 import os
 import time
 from typing import Optional
 
 import fire
 from fastapi.datastructures import UploadFile
@@ -86,17 +87,18 @@
             t0 = time.time()
             response = self.client.ingest_documents(documents_dicts)
             t1 = time.time()
             print(f"Time taken to ingest files: {t1-t0:.2f} seconds")
             print(response)
         else:
             t0 = time.time()
-            self.r2r.ingest_documents(documents)
+            response = self.r2r.ingest_documents(documents)
             t1 = time.time()
             print(f"Time taken to ingest files: {t1-t0:.2f} seconds")
+            print(response)
 
     def ingest_as_files(self, file_paths: Optional[list[str]] = None):
         file_paths = file_paths or self.default_files
         files = [
             UploadFile(
                 filename=file_path.split(os.path.sep)[-1],
                 file=open(file_path, "rb"),
@@ -124,17 +126,17 @@
                 metadatas=metadatas, files=file_paths
             )
             t1 = time.time()
             print(f"Time taken to ingest files: {t1-t0:.2f} seconds")
             print(response)
         else:
             t0 = time.time()
-            self.r2r.ingest_files(files=files, metadatas=metadatas)
+            response = self.r2r.ingest_files(files=files, metadatas=metadatas)
             t1 = time.time()
-            print(f"Time taken to ingest files: {t1-t0:.2f} seconds")
+            print("response = ", response)
 
     def search(self, query: str):
         if hasattr(self, "client"):
             t0 = time.time()
             results = self.client.search(
                 query, search_filters={"user_id": self.user_id}
             )
```

### Comparing `r2r-0.2.0/r2r/examples/servers/configurable_pipeline.py` & `r2r-0.2.1/r2r/examples/servers/configurable_pipeline.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/integrations/exa.py` & `r2r-0.2.1/r2r/integrations/exa.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/integrations/ionic.py` & `r2r-0.2.1/r2r/integrations/ionic.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/integrations/serper.py` & `r2r-0.2.1/r2r/integrations/serper.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/llms/litellm/base_litellm.py` & `r2r-0.2.1/r2r/llms/litellm/base_litellm.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/llms/llama_cpp/base_llama_cpp.py` & `r2r-0.2.1/r2r/llms/llama_cpp/base_llama_cpp.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/llms/openai/base_openai.py` & `r2r-0.2.1/r2r/llms/openai/base_openai.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/main/r2r_abstractions.py` & `r2r-0.2.1/r2r/main/r2r_abstractions.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/main/r2r_app.py` & `r2r-0.2.1/r2r/main/r2r_app.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,42 +32,72 @@
 def syncable(func):
     """Decorator to mark methods for synchronous wrapper creation."""
     func._syncable = True
     return func
 
 
 class AsyncSyncMeta(type):
-    """Metaclass to create synchronous wrappers for async methods."""
+    _event_loop = None  # Class-level shared event loop
+
+    @classmethod
+    def get_event_loop(cls):
+        if cls._event_loop is None or cls._event_loop.is_closed():
+            cls._event_loop = asyncio.new_event_loop()
+            asyncio.set_event_loop(cls._event_loop)
+        return cls._event_loop
 
     def __new__(cls, name, bases, dct):
         new_cls = super().__new__(cls, name, bases, dct)
         for attr_name, attr_value in dct.items():
             if asyncio.iscoroutinefunction(attr_value) and getattr(
                 attr_value, "_syncable", False
             ):
                 sync_method_name = attr_name[
                     1:
                 ]  # Remove leading 'a' for sync method
                 async_method = attr_value
 
                 def make_sync_method(async_method):
                     def sync_wrapper(self, *args, **kwargs):
-                        try:
-                            import nest_asyncio
-
-                            nest_asyncio.apply()
-                            result = asyncio.run(
-                                async_method(self, *args, **kwargs)
-                            )
+                        loop = cls.get_event_loop()
+                        if not loop.is_running():
+                            # Setup to run the loop in a background thread if necessary
+                            # to prevent blocking the main thread in a synchronous call environment
+                            from threading import Thread
+
+                            result = None
+                            exception = None
+
+                            def run():
+                                nonlocal result, exception
+                                try:
+                                    asyncio.set_event_loop(loop)
+                                    result = loop.run_until_complete(
+                                        async_method(self, *args, **kwargs)
+                                    )
+                                except Exception as e:
+                                    exception = e
+                                finally:
+                                    loop.run_until_complete(
+                                        loop.shutdown_asyncgens()
+                                    )
+                                    loop.close()
+
+                            thread = Thread(target=run)
+                            thread.start()
+                            thread.join()
+                            if exception:
+                                raise exception
                             return result
-                        except Exception as e:
-                            logger.error(
-                                f"Error in sync method {sync_method_name}: {str(e)}"
+                        else:
+                            # If there's already a running loop, schedule and execute the coroutine
+                            future = asyncio.run_coroutine_threadsafe(
+                                async_method(self, *args, **kwargs), loop
                             )
-                            raise
+                            return future.result()
 
                     return sync_wrapper
 
                 setattr(
                     new_cls, sync_method_name, make_sync_method(async_method)
                 )
         return new_cls
@@ -426,15 +456,15 @@
             raise HTTPException(status_code=500, detail=str(e))
 
     class RAGRequest(BaseModel):
         message: str
         search_filters: Optional[str] = None
         search_limit: int = 10
         rag_generation_config: Optional[str] = None
-        streaming: bool = False
+        streaming: Optional[bool] = None
 
     async def rag_app(self, request: RAGRequest):
         try:
             search_filters = (
                 None
                 if request.search_filters is None
                 or request.search_filters == "null"
```

### Comparing `r2r-0.2.0/r2r/main/r2r_client.py` & `r2r-0.2.1/r2r/main/r2r_client.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/main/r2r_config.py` & `r2r-0.2.1/r2r/main/r2r_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
             "search_model",
             "search_dimension",
             "batch_size",
             "text_splitter",
         ],
         "eval": [
             "llm",
-            "sampling_fraction",
         ],
         "ingestion": ["selected_parsers"],
         "completions": ["provider"],
         "logging": ["provider", "log_table"],
         "prompt": ["provider"],
         "vector_database": ["provider", "collection_name"],
     }
```

### Comparing `r2r-0.2.0/r2r/main/r2r_factory.py` & `r2r-0.2.1/r2r/main/r2r_factory.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/pipes/__init__.py` & `r2r-0.2.1/r2r/pipes/__init__.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/pipes/abstractions/generator_pipe.py` & `r2r-0.2.1/r2r/pipes/abstractions/generator_pipe.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/pipes/abstractions/search_pipe.py` & `r2r-0.2.1/r2r/pipes/abstractions/search_pipe.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import logging
 from abc import abstractmethod
 from typing import Any, AsyncGenerator, Optional, Union
 
 from r2r.core import (
     AsyncPipe,
     AsyncState,
+    LoggableAsyncPipe,
     PipeLoggingConnectionSingleton,
     PipeType,
     SearchResult,
     VectorDBProvider,
 )
 
-from ...core.pipes.loggable_pipe import LoggableAsyncPipe
-
 logger = logging.getLogger(__name__)
 
 
 class SearchPipe(LoggableAsyncPipe):
     class SearchConfig(LoggableAsyncPipe.PipeConfig):
         name: str = "default_vector_search"
         search_filters: dict = {}
```

### Comparing `r2r-0.2.0/r2r/pipes/embedding_pipe.py` & `r2r-0.2.1/r2r/pipes/embedding_pipe.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/pipes/eval_pipe.py` & `r2r-0.2.1/r2r/pipes/eval_pipe.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,13 +41,10 @@
             **kwargs,
         )
 
     async def _run_logic(
         self, input: Input, state: AsyncState, *args: Any, **kwargs: Any
     ) -> AsyncGenerator[LLMChatCompletion, None]:
         async for item in input.message:
-            if random.random() < self.eval_provider.config.sampling_fraction:
-                yield self.eval_provider.evaluate(
-                    item.query, item.context, item.completion
-                )
-            else:
-                yield None
+            yield self.eval_provider.evaluate(
+                item.query, item.context, item.completion
+            )
```

### Comparing `r2r-0.2.0/r2r/pipes/parsing_pipe.py` & `r2r-0.2.1/r2r/pipes/parsing_pipe.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/pipes/query_transform_pipe.py` & `r2r-0.2.1/r2r/pipes/query_transform_pipe.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/pipes/rag_pipe.py` & `r2r-0.2.1/r2r/pipes/rag_pipe.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/pipes/streaming_rag_pipe.py` & `r2r-0.2.1/r2r/pipes/streaming_rag_pipe.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,30 +51,30 @@
         **kwargs: Any,
     ) -> AsyncGenerator[str, None]:
         iteration = 0
         context = ""
         # dump the search results and construct the context
         yield f"<{self.SEARCH_STREAM_MARKER}>"
         for result in input.raw_search_results:
-            yield f'"{json.dumps(result.json())}"'
             if iteration >= 1:
                 yield ","
+            yield json.dumps(result.json())
             context += f"Result {iteration+1}:\n{result.metadata['text']}\n\n"
             iteration += 1
         yield f"</{self.SEARCH_STREAM_MARKER}>"
 
         messages = self._get_message_payload(str(input.query), context)
         yield f"<{self.COMPLETION_STREAM_MARKER}>"
         response = ""
         for chunk in self.llm_provider.get_completion_stream(
             messages=messages, generation_config=rag_generation_config
         ):
             chunk = R2RStreamingRAGPipe._process_chunk(chunk)
             response += chunk
-            yield response
+            yield chunk
 
         yield f"</{self.COMPLETION_STREAM_MARKER}>"
 
         await self.enqueue_log(
             pipe_run_id=self.run_info.run_id,
             key="llm_response",
             value=response,
```

### Comparing `r2r-0.2.0/r2r/pipes/vector_search_pipe.py` & `r2r-0.2.1/r2r/pipes/vector_search_pipe.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         for result in self.vector_db_provider.search(
             query_vector=self.embedding_provider.get_embedding(
                 message,
             ),
             filters=search_filters_override or self.config.search_filters,
             limit=search_limit_override or self.config.search_limit,
         ):
-            result.metadata["query"] = message
+            result.metadata["associatedQuery"] = message
             results.append(result)
             yield result
 
         await self.enqueue_log(
             pipe_run_id=self.run_info.run_id,
             key="search_results",
             value=json.dumps([ele.json() for ele in results]),
```

### Comparing `r2r-0.2.0/r2r/pipes/vector_storage_pipe.py` & `r2r-0.2.1/r2r/pipes/vector_storage_pipe.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import asyncio
 import logging
 from typing import Any, AsyncGenerator, Optional
 
 from r2r.core import (
     AsyncState,
+    LoggableAsyncPipe,
     PipeLoggingConnectionSingleton,
     PipeType,
     VectorDBProvider,
     VectorEntry,
 )
 
-from ..core.pipes.loggable_pipe import LoggableAsyncPipe
-
 logger = logging.getLogger(__name__)
 
 
 class R2RVectorStoragePipe(LoggableAsyncPipe):
     class Input(LoggableAsyncPipe.Input):
         message: AsyncGenerator[VectorEntry, None]
         do_upsert: bool = True
@@ -82,22 +81,24 @@
 
         async for vector_entry in input.message:
             vector_batch.append(vector_entry)
             if len(vector_batch) >= self.storage_batch_size:
                 # Schedule the storage task
                 batch_tasks.append(
                     asyncio.create_task(
-                        self.store(vector_batch.copy(), input.do_upsert)
+                        self.store(vector_batch.copy(), input.do_upsert),
+                        name=f"vector-store-{self.config.name}",
                     )
                 )
                 vector_batch.clear()
 
         if vector_batch:  # Process any remaining vectors
             batch_tasks.append(
                 asyncio.create_task(
-                    self.store(vector_batch.copy(), input.do_upsert)
+                    self.store(vector_batch.copy(), input.do_upsert),
+                    name=f"vector-store-{self.config.name}",
                 )
             )
 
         # Wait for all storage tasks to complete
         await asyncio.gather(*batch_tasks)
         yield None
```

### Comparing `r2r-0.2.0/r2r/prompts/local/defaults.jsonl` & `r2r-0.2.1/r2r/prompts/local/defaults.jsonl`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/prompts/local/r2r_prompt_provider.py` & `r2r-0.2.1/r2r/prompts/local/r2r_prompt_provider.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/vecs/__init__.py` & `r2r-0.2.1/r2r/vecs/__init__.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/vecs/adapter/base.py` & `r2r-0.2.1/r2r/vecs/adapter/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/vecs/adapter/markdown.py` & `r2r-0.2.1/r2r/vecs/adapter/markdown.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/vecs/adapter/noop.py` & `r2r-0.2.1/r2r/vecs/adapter/noop.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/vecs/adapter/text.py` & `r2r-0.2.1/r2r/vecs/adapter/text.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/vecs/client.py` & `r2r-0.2.1/r2r/vecs/client.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/vecs/collection.py` & `r2r-0.2.1/r2r/vecs/collection.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/vecs/exc.py` & `r2r-0.2.1/r2r/vecs/exc.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/vector_dbs/local/r2r_local_vector_db.py` & `r2r-0.2.1/r2r/vector_dbs/local/r2r_local_vector_db.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/vector_dbs/pgvector/pgvector_db.py` & `r2r-0.2.1/r2r/vector_dbs/pgvector/pgvector_db.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/r2r/vector_dbs/qdrant/qdrant_db.py` & `r2r-0.2.1/r2r/vector_dbs/qdrant/qdrant_db.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.0/PKG-INFO` & `r2r-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r2r
-Version: 0.2.0
+Version: 0.2.1
 Summary: SciPhi R2R
 License: MIT
 Author: Owen Colegrove
 Author-email: owen@sciphi.ai
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -236,15 +236,15 @@
 ```
 
 ### Streaming Response
 
 For streaming results from a RAG query, use the following command:
 
 ```bash
-python -m r2r.examples.demo rag --query="What was Lyft's profit in 2020?" --streaming=True
+python -m r2r.examples.demo rag --query="What was Lyft's profit in 2020?" --streaming=true
 ```
 
 **Demo Output:**
 
 ```plaintext
 r2r.main.r2r_config - INFO - Loading configuration from <YOUR_WORKDIR>/config.json - 2024-05-20 22:27:31,890
 ...
@@ -304,15 +304,15 @@
    ```bash
    python -m r2r.examples.demo rag --query="What was Uber's profit in 2020?" --base_url=http://localhost:8000
    ```
    This command sends the RAG query to the server and retrieves the generated response.
 
 4. **Run a RAG Stream**:
    ```bash
-   python -m r2r.examples.demo rag --query="What was Lyft's profit in 2020?" --streaming=True --base_url=http://localhost:8000
+   python -m r2r.examples.demo rag --query="What was Lyft's profit in 2020?" --streaming=true --base_url=http://localhost:8000
    ```
    This command streams the RAG query results from the server.
 
 ### Server-Client Summary
 
 By using the server-client model, you can extend the basic R2R demo to support more scalable and modular deployments. The server handles requests and performs heavy computations, while clients can communicate with the server to perform ingestion, search, RAG, and other operations, as shown in the examples above. For detailed setup and basic functionality, refer back to the [R2R Demo](#r2r-demo).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: r2r Version: 0.2.0 Summary: SciPhi R2R License: MIT
+Metadata-Version: 2.1 Name: r2r Version: 0.2.1 Summary: SciPhi R2R License: MIT
 Author: Owen Colegrove Author-email: owen@sciphi.ai Requires-Python:
 >=3.9,<3.13 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Provides-Extra: all Provides-Extra: exa Provides-Extra: ionic
 Provides-Extra: local-llm Provides-Extra: sentence-transformers-only Requires-
@@ -103,15 +103,15 @@
 ( content="Uber's profit in 2020 was a net loss of $6,768 million [10].",
 role='assistant', function_call=None, tool_calls=None ) ) ],
 created=1716268695, model='gpt-3.5-turbo-0125', object='chat.completion',
 system_fingerprint=None, usage=CompletionUsage( completion_tokens=20,
 prompt_tokens=1470, total_tokens=1490 ) ) ] } ``` ### Streaming Response For
 streaming results from a RAG query, use the following command: ```bash python -
 m r2r.examples.demo rag --query="What was Lyft's profit in 2020?" --
-streaming=True ``` **Demo Output:** ```plaintext r2r.main.r2r_config - INFO -
+streaming=true ``` **Demo Output:** ```plaintext r2r.main.r2r_config - INFO -
 Loading configuration from /config.json - 2024-05-20 22:27:31,890 ... ["
 {\"id\":\"808c47c5-ebef-504a-a230-aa9ddcfbd87 .... Lyft reported a net loss of
 $1,752,857,000 in 2020 according to [2]. Therefore, Lyft did not make a profit
 in 2020. Time taken to stream RAG response: 2.79 seconds ``` ## Document
 Management Demo ### Document Deletion To delete a document by its ID, or any
 other metadata field, use the delete command. For example, to delete all chunks
 corresponding to the uploaded file `aristotle.txt`, we can call delete on the
@@ -134,15 +134,15 @@
 ```bash python -m r2r.examples.demo search --query="Who was Aristotle?" --
 base_url=http://localhost:8000 ``` This command sends the search query to the
 server and retrieves the results. 3. **Run a RAG Completion**: ```bash python -
 m r2r.examples.demo rag --query="What was Uber's profit in 2020?" --
 base_url=http://localhost:8000 ``` This command sends the RAG query to the
 server and retrieves the generated response. 4. **Run a RAG Stream**: ```bash
 python -m r2r.examples.demo rag --query="What was Lyft's profit in 2020?" --
-streaming=True --base_url=http://localhost:8000 ``` This command streams the
+streaming=true --base_url=http://localhost:8000 ``` This command streams the
 RAG query results from the server. ### Server-Client Summary By using the
 server-client model, you can extend the basic R2R demo to support more scalable
 and modular deployments. The server handles requests and performs heavy
 computations, while clients can communicate with the server to perform
 ingestion, search, RAG, and other operations, as shown in the examples above.
 For detailed setup and basic functionality, refer back to the [R2R Demo](#r2r-
 demo). # Core Abstractions The framework revolves around three core
```

