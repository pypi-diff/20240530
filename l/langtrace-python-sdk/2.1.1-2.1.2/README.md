# Comparing `tmp/langtrace_python_sdk-2.1.1.tar.gz` & `tmp/langtrace_python_sdk-2.1.2.tar.gz`

## Comparing `langtrace_python_sdk-2.1.1.tar` & `langtrace_python_sdk-2.1.2.tar`

### file list

```diff
@@ -1,146 +1,146 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/__init__.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/run_example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/anthropic_example/__init__.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/anthropic_example/completion.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/chroma_example/__init__.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/chroma_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/cohere_example/__init__.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/cohere_example/chat.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/cohere_example/chat_stream.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/cohere_example/embed.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/cohere_example/rerank.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/cohere_example/tools.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/fastapi_example/basic_route.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/hiveagent_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/langchain_example/__init__.py
--rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/langchain_example/basic.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/langchain_example/groq_example.py
--rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/langchain_example/langgraph_example.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/langchain_example/tool.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/llamaindex_example/__init__.py
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/llamaindex_example/agent.py
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/llamaindex_example/basic.py
--rw-r--r--   0        0        0    32667 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/llamaindex_example/data/abramov.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/openai_example/__init__.py
--rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/openai_example/async_tool_calling_nonstreaming.py
--rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/openai_example/async_tool_calling_streaming.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/openai_example/chat_completion.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/openai_example/embeddings_create.py
--rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/openai_example/function_calling.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/openai_example/images_generate.py
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/openai_example/tool_calling.py
--rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/openai_example/tool_calling_nonstreaming.py
--rw-r--r--   0        0        0     7015 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/openai_example/tool_calling_streaming.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/perplexity_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/pinecone_example/__init__.py
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/pinecone_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/qdrant_example/__init__.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/qdrant_example/basic.py
--rw-r--r--   0        0        0    64533 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/examples/weaviate_example/query_text.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/__init__.py
--rw-r--r--   0        0        0     6993 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/langtrace.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/constants/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/constants/exporter/langtrace_exporter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/constants/instrumentation/__init__.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/constants/instrumentation/anthropic.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/constants/instrumentation/chroma.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/constants/instrumentation/cohere.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/constants/instrumentation/common.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/constants/instrumentation/groq.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/constants/instrumentation/openai.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/constants/instrumentation/pinecone.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/constants/instrumentation/qdrant.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/constants/instrumentation/weaviate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/extensions/__init__.py
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/extensions/langtrace_exporter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/anthropic/__init__.py
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py
--rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/anthropic/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/chroma/__init__.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py
--rw-r--r--   0        0        0     8750 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/chroma/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/cohere/__init__.py
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py
--rw-r--r--   0        0        0    26563 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/cohere/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/groq/__init__.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py
--rw-r--r--   0        0        0    26068 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/groq/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/langchain/__init__.py
--rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py
--rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/langchain/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/langchain_community/__init__.py
--rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py
--rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/langchain_core/__init__.py
--rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py
--rw-r--r--   0        0        0     8458 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/langgraph/__init__.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py
--rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/langgraph/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/llamaindex/__init__.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py
--rw-r--r--   0        0        0     4189 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py
--rw-r--r--   0        0        0    37288 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/openai/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/pinecone/__init__.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py
--rw-r--r--   0        0        0     4889 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/pinecone/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/qdrant/__init__.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py
--rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/qdrant/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/weaviate/__init__.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/weaviate/instrumentation.py
--rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/weaviate/patch.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/types/__init__.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/utils/__init__.py
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/utils/llm.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/utils/misc.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/utils/prompt_registry.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/utils/silently_fail.py
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/utils/types.py
--rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/utils/with_root_span.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/tests/__init__.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/tests/conftest.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/tests/utils.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/tests/anthropic/conftest.py
--rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/tests/anthropic/test_anthropic.py
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/tests/anthropic/cassettes/test_anthropic.yaml
--rw-r--r--   0        0        0    11675 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml
--rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/tests/chroma/conftest.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/tests/chroma/test_chroma.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/tests/cohere/conftest.py
--rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/tests/cohere/test_cohere_chat.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/tests/cohere/test_cohere_embed.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/tests/cohere/test_cohere_rerank.py
--rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/tests/cohere/cassettes/test_cohere_chat.yaml
--rw-r--r--   0        0        0     8174 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/tests/cohere/cassettes/test_cohere_chat_streaming.yaml
--rw-r--r--   0        0        0    27320 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/tests/cohere/cassettes/test_cohere_embed.yaml
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/tests/cohere/cassettes/test_cohere_rerank.yaml
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/tests/langchain/test_langchain.py
--rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/tests/langchain/test_langchain_community.py
--rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/tests/langchain/test_langchain_core.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/tests/openai/conftest.py
--rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/tests/openai/test_chat_completion.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/tests/openai/test_embeddings.py
--rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/tests/openai/test_image_generation.py
--rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/tests/openai/cassettes/test_async_image_generation.yaml
--rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/tests/openai/cassettes/test_chat_completion.yaml
--rw-r--r--   0        0        0  2592394 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/tests/openai/cassettes/test_chat_completion_streaming.yaml
--rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/tests/openai/cassettes/test_image_generation.yaml
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/tests/pinecone/conftest.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/tests/pinecone/test_pinecone.py
--rw-r--r--   0        0        0   103821 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/tests/pinecone/cassettes/test_query.yaml
--rw-r--r--   0        0        0    38607 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/tests/pinecone/cassettes/test_upsert.yaml
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/tests/qdrant/conftest.py
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/src/tests/qdrant/test_qdrant.py
--rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/.gitignore
--rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/LICENSE
--rw-r--r--   0        0        0    10255 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/README.md
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/pyproject.toml
--rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/__init__.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/run_example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/anthropic_example/__init__.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/anthropic_example/completion.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/chroma_example/__init__.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/chroma_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/cohere_example/__init__.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/cohere_example/chat.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/cohere_example/chat_stream.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/cohere_example/embed.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/cohere_example/rerank.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/cohere_example/tools.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/fastapi_example/basic_route.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/hiveagent_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/langchain_example/__init__.py
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/langchain_example/basic.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/langchain_example/groq_example.py
+-rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/langchain_example/langgraph_example.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/langchain_example/tool.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/llamaindex_example/__init__.py
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/llamaindex_example/agent.py
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/llamaindex_example/basic.py
+-rw-r--r--   0        0        0    32667 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/llamaindex_example/data/abramov.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/openai_example/__init__.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/openai_example/async_tool_calling_nonstreaming.py
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/openai_example/async_tool_calling_streaming.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/openai_example/chat_completion.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/openai_example/embeddings_create.py
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/openai_example/function_calling.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/openai_example/images_generate.py
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/openai_example/tool_calling.py
+-rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/openai_example/tool_calling_nonstreaming.py
+-rw-r--r--   0        0        0     7015 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/openai_example/tool_calling_streaming.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/perplexity_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/pinecone_example/__init__.py
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/pinecone_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/qdrant_example/__init__.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/qdrant_example/basic.py
+-rw-r--r--   0        0        0    64533 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/weaviate_example/query_text.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/__init__.py
+-rw-r--r--   0        0        0     6993 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/langtrace.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/constants/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/constants/exporter/langtrace_exporter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/constants/instrumentation/__init__.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/constants/instrumentation/anthropic.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/constants/instrumentation/chroma.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/constants/instrumentation/cohere.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/constants/instrumentation/common.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/constants/instrumentation/groq.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/constants/instrumentation/openai.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/constants/instrumentation/pinecone.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/constants/instrumentation/qdrant.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/constants/instrumentation/weaviate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/extensions/__init__.py
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/extensions/langtrace_exporter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/anthropic/__init__.py
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py
+-rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/anthropic/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/chroma/__init__.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py
+-rw-r--r--   0        0        0     8750 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/chroma/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/cohere/__init__.py
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py
+-rw-r--r--   0        0        0    26563 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/cohere/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/groq/__init__.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py
+-rw-r--r--   0        0        0    26068 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/groq/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langchain/__init__.py
+-rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langchain/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langchain_community/__init__.py
+-rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py
+-rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langchain_core/__init__.py
+-rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py
+-rw-r--r--   0        0        0     8458 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langgraph/__init__.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py
+-rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langgraph/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/llamaindex/__init__.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py
+-rw-r--r--   0        0        0     4189 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py
+-rw-r--r--   0        0        0    37288 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/openai/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/pinecone/__init__.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py
+-rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/pinecone/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/qdrant/__init__.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py
+-rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/qdrant/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/weaviate/__init__.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/weaviate/instrumentation.py
+-rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/weaviate/patch.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/types/__init__.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/utils/__init__.py
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/utils/llm.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/utils/misc.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/utils/prompt_registry.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/utils/silently_fail.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/utils/types.py
+-rw-r--r--   0        0        0     6103 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/utils/with_root_span.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/__init__.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/conftest.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/utils.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/anthropic/conftest.py
+-rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/anthropic/test_anthropic.py
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/anthropic/cassettes/test_anthropic.yaml
+-rw-r--r--   0        0        0    11675 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml
+-rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/chroma/conftest.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/chroma/test_chroma.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/cohere/conftest.py
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/cohere/test_cohere_chat.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/cohere/test_cohere_embed.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/cohere/test_cohere_rerank.py
+-rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/cohere/cassettes/test_cohere_chat.yaml
+-rw-r--r--   0        0        0     8174 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/cohere/cassettes/test_cohere_chat_streaming.yaml
+-rw-r--r--   0        0        0    27320 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/cohere/cassettes/test_cohere_embed.yaml
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/cohere/cassettes/test_cohere_rerank.yaml
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/langchain/test_langchain.py
+-rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/langchain/test_langchain_community.py
+-rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/langchain/test_langchain_core.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/openai/conftest.py
+-rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/openai/test_chat_completion.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/openai/test_embeddings.py
+-rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/openai/test_image_generation.py
+-rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/openai/cassettes/test_async_image_generation.yaml
+-rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/openai/cassettes/test_chat_completion.yaml
+-rw-r--r--   0        0        0  2592394 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/openai/cassettes/test_chat_completion_streaming.yaml
+-rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/openai/cassettes/test_image_generation.yaml
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/pinecone/conftest.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/pinecone/test_pinecone.py
+-rw-r--r--   0        0        0   103821 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/pinecone/cassettes/test_query.yaml
+-rw-r--r--   0        0        0    38607 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/pinecone/cassettes/test_upsert.yaml
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/qdrant/conftest.py
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/qdrant/test_qdrant.py
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/.gitignore
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/LICENSE
+-rw-r--r--   0        0        0    10255 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/README.md
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0    11738 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/PKG-INFO
```

### Comparing `langtrace_python_sdk-2.1.1/src/run_example.py` & `langtrace_python_sdk-2.1.2/src/run_example.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/examples/anthropic_example/completion.py` & `langtrace_python_sdk-2.1.2/src/examples/anthropic_example/completion.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/examples/chroma_example/basic.py` & `langtrace_python_sdk-2.1.2/src/examples/chroma_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/examples/cohere_example/chat.py` & `langtrace_python_sdk-2.1.2/src/examples/cohere_example/chat.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/examples/cohere_example/chat_stream.py` & `langtrace_python_sdk-2.1.2/src/examples/cohere_example/chat_stream.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/examples/cohere_example/embed.py` & `langtrace_python_sdk-2.1.2/src/examples/cohere_example/embed.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/examples/cohere_example/rerank.py` & `langtrace_python_sdk-2.1.2/src/examples/cohere_example/rerank.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/examples/cohere_example/tools.py` & `langtrace_python_sdk-2.1.2/src/examples/cohere_example/tools.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/examples/fastapi_example/basic_route.py` & `langtrace_python_sdk-2.1.2/src/examples/fastapi_example/basic_route.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/examples/langchain_example/basic.py` & `langtrace_python_sdk-2.1.2/src/examples/langchain_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/examples/langchain_example/groq_example.py` & `langtrace_python_sdk-2.1.2/src/examples/langchain_example/groq_example.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/examples/langchain_example/langgraph_example.py` & `langtrace_python_sdk-2.1.2/src/examples/langchain_example/langgraph_example.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/examples/langchain_example/tool.py` & `langtrace_python_sdk-2.1.2/src/examples/langchain_example/tool.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/examples/llamaindex_example/agent.py` & `langtrace_python_sdk-2.1.2/src/examples/llamaindex_example/agent.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/examples/llamaindex_example/basic.py` & `langtrace_python_sdk-2.1.2/src/examples/llamaindex_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/examples/llamaindex_example/data/abramov.txt` & `langtrace_python_sdk-2.1.2/src/examples/llamaindex_example/data/abramov.txt`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/examples/openai_example/async_tool_calling_nonstreaming.py` & `langtrace_python_sdk-2.1.2/src/examples/openai_example/async_tool_calling_nonstreaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/examples/openai_example/async_tool_calling_streaming.py` & `langtrace_python_sdk-2.1.2/src/examples/openai_example/async_tool_calling_streaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/examples/openai_example/chat_completion.py` & `langtrace_python_sdk-2.1.2/src/examples/openai_example/chat_completion.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/examples/openai_example/function_calling.py` & `langtrace_python_sdk-2.1.2/src/examples/openai_example/function_calling.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/examples/openai_example/tool_calling.py` & `langtrace_python_sdk-2.1.2/src/examples/openai_example/tool_calling.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/examples/openai_example/tool_calling_nonstreaming.py` & `langtrace_python_sdk-2.1.2/src/examples/openai_example/tool_calling_nonstreaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/examples/openai_example/tool_calling_streaming.py` & `langtrace_python_sdk-2.1.2/src/examples/openai_example/tool_calling_streaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/examples/perplexity_example/basic.py` & `langtrace_python_sdk-2.1.2/src/examples/perplexity_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/examples/pinecone_example/basic.py` & `langtrace_python_sdk-2.1.2/src/examples/pinecone_example/basic.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 """
 This example demonstrates how to use Pinecone with Langtrace.
 """
 
-from langtrace_python_sdk import langtrace
 from dotenv import find_dotenv, load_dotenv
 from openai import OpenAI
-from pinecone import Pinecone
+from pinecone import Pinecone, ServerlessSpec
 
-
-from langtrace_python_sdk import with_langtrace_root_span, send_user_feedback
+from langtrace_python_sdk import langtrace, with_langtrace_root_span
+from langtrace_python_sdk.utils.with_root_span import send_user_feedback
 
 _ = load_dotenv(find_dotenv())
 
 langtrace.init()
 
 client = OpenAI()
 pinecone = Pinecone()
 
+PINECONE_INDEX_NAME = "test-index"
+
+
+def create_index():
+    pinecone.create_index(
+        name=PINECONE_INDEX_NAME,
+        dimension=1536,
+        metric="cosine",
+        spec=ServerlessSpec(cloud="aws", region="us-east-1"),
+    )
+
 
 @with_langtrace_root_span()
 def basic(span_id, trace_id):
 
     result = client.embeddings.create(
         model="text-embedding-ada-002",
         input="Some random text string goes here",
@@ -28,18 +38,22 @@
     )
 
     embedding = result.data[0].embedding
 
     unique_id = "unique_random_id"
     data_to_upsert = {"id": unique_id, "values": embedding}
 
-    index = pinecone.Index("test-index")
+    index = pinecone.Index(PINECONE_INDEX_NAME)
     res = index.upsert(vectors=[data_to_upsert], namespace="test-namespace")
     print("res", res)
 
     resp = index.query(
         vector=embedding, top_k=1, include_values=False, namespace="test-namespace"
     )
     send_user_feedback(
         {"spanId": span_id, "traceId": trace_id, "userScore": 1, "userId": "123"}
     )
     print(resp)
+
+
+# create_index()
+basic("span_id", "trace_id")
```

### Comparing `langtrace_python_sdk-2.1.1/src/examples/qdrant_example/basic.py` & `langtrace_python_sdk-2.1.2/src/examples/qdrant_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/examples/weaviate_example/query_text.py` & `langtrace_python_sdk-2.1.2/src/examples/weaviate_example/query_text.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/__init__.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/langtrace.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/langtrace.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/constants/instrumentation/chroma.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/constants/instrumentation/chroma.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/constants/instrumentation/cohere.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/constants/instrumentation/cohere.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/constants/instrumentation/common.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/constants/instrumentation/common.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/constants/instrumentation/openai.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/constants/instrumentation/openai.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/constants/instrumentation/qdrant.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/constants/instrumentation/qdrant.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/constants/instrumentation/weaviate.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/constants/instrumentation/weaviate.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/extensions/langtrace_exporter.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/extensions/langtrace_exporter.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/anthropic/patch.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/anthropic/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/chroma/patch.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/chroma/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/cohere/patch.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/cohere/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/groq/patch.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/groq/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/langchain/patch.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langchain/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/langgraph/patch.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langgraph/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/openai/patch.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/openai/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,50 +14,42 @@
 limitations under the License.
 """
 
 import importlib.metadata
 import logging
 from typing import Collection
 
-import pinecone
-from langtrace.trace_attributes import PineconeMethods
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.trace import get_tracer
 from wrapt import wrap_function_wrapper
 
-from langtrace_python_sdk.constants.instrumentation.pinecone import APIS
-from langtrace_python_sdk.instrumentation.pinecone.patch import generic_patch
+from langtrace_python_sdk.constants.instrumentation.qdrant import APIS
+from langtrace_python_sdk.instrumentation.qdrant.patch import collection_patch
 
 logging.basicConfig(level=logging.FATAL)
 
 
-class PineconeInstrumentation(BaseInstrumentor):
+class QdrantInstrumentation(BaseInstrumentor):
+    """
+    The QdrantInstrumentation class represents the Qdrant DB instrumentation
     """
-    The PineconeInstrumentation class represents the Pinecone instrumentation"""
 
     def instrumentation_dependencies(self) -> Collection[str]:
-        return ["pinecone-client >= 3.1.0"]
+        return ["qdrant-client >= 1.9.0"]
 
     def _instrument(self, **kwargs):
         tracer_provider = kwargs.get("tracer_provider")
         tracer = get_tracer(__name__, "", tracer_provider)
-        version = importlib.metadata.version("pinecone-client")
-        for operation_name, details in APIS.items():
-            method_ref = details["METHOD"]
-            method = None
-            if method_ref is PineconeMethods.UPSERT.value:
-                method = pinecone.Index.upsert
-            elif method_ref is PineconeMethods.QUERY.value:
-                method = pinecone.Index.query
-            elif method_ref is PineconeMethods.DELETE.value:
-                method = pinecone.Index.delete
-            operation = details["OPERATION"]
+        version = importlib.metadata.version("qdrant-client")
 
-            # Dynamically creating the patching call
+        for operation, _ in APIS.items():
             wrap_function_wrapper(
-                "pinecone.data.index",
-                f"Index.{operation}",
-                generic_patch(method, operation_name, version, tracer),
+                "qdrant_client.qdrant_client",
+                f"QdrantClient.{operation.lower()}",
+                collection_patch(operation, version, tracer),
             )
 
+    def _instrument_module(self, module_name):
+        pass
+
     def _uninstrument(self, **kwargs):
         pass
```

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/pinecone/patch.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/pinecone/patch.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,35 +10,36 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
+import json
+
 from langtrace.trace_attributes import DatabaseSpanAttributes
-from langtrace_python_sdk.utils import set_span_attribute
-from langtrace_python_sdk.utils.silently_fail import silently_fail
 from opentelemetry import baggage
 from opentelemetry.trace import SpanKind
 from opentelemetry.trace.status import Status, StatusCode
 
 from langtrace_python_sdk.constants.instrumentation.common import (
     LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY,
     SERVICE_PROVIDERS,
 )
 from langtrace_python_sdk.constants.instrumentation.pinecone import APIS
-import json
+from langtrace_python_sdk.utils import set_span_attribute
+from langtrace_python_sdk.utils.silently_fail import silently_fail
 
 
-def generic_patch(original_method, method, version, tracer):
+def generic_patch(operation_name, version, tracer):
     """
     A generic patch method that wraps a function with a span"""
 
     def traced_method(wrapped, instance, args, kwargs):
-        api = APIS[method]
+        api = APIS[operation_name]
         service_provider = SERVICE_PROVIDERS["PINECONE"]
         extra_attributes = baggage.get_baggage(LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY)
 
         span_attributes = {
             "langtrace.sdk.name": "langtrace-python-sdk",
             "langtrace.service.name": service_provider,
             "langtrace.service.type": "vectordb",
@@ -52,23 +53,23 @@
 
         attributes = DatabaseSpanAttributes(**span_attributes)
 
         with tracer.start_as_current_span(api["METHOD"], kind=SpanKind.CLIENT) as span:
 
             if span.is_recording():
                 set_span_attribute(span, "server.address", instance._config.host)
-                if method == "QUERY":
+                if operation_name == "QUERY":
                     set_query_input_attributes(span, kwargs)
 
             for field, value in attributes.model_dump(by_alias=True).items():
                 if value is not None:
                     span.set_attribute(field, value)
             try:
                 # Attempt to call the original method
-                result = original_method(instance, *args, **kwargs)
+                result = wrapped(*args, **kwargs)
                 if result:
                     if span.is_recording():
                         set_query_response_attributes(span, result)
                 span.set_status(StatusCode.OK)
                 return result
             except Exception as err:
                 # Record the exception in the span
```

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/weaviate/instrumentation.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,38 +18,49 @@
 import logging
 from typing import Collection
 
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.trace import get_tracer
 from wrapt import wrap_function_wrapper
 
-from langtrace_python_sdk.constants.instrumentation.qdrant import APIS
-from langtrace_python_sdk.instrumentation.qdrant.patch import collection_patch
+from langtrace_python_sdk.instrumentation.weaviate.patch import (
+    generic_collection_patch,
+    generic_query_patch,
+)
+from langtrace_python_sdk.constants.instrumentation.weaviate import APIS
 
 logging.basicConfig(level=logging.FATAL)
 
 
-class QdrantInstrumentation(BaseInstrumentor):
+class WeaviateInstrumentation(BaseInstrumentor):
     """
-    The QdrantInstrumentation class represents the Qdrant DB instrumentation
+    The WeaviateInstrumentation class represents the instrumentation for the Weaviate SDK.
     """
 
     def instrumentation_dependencies(self) -> Collection[str]:
-        return ["qdrant-client >= 1.9.0"]
+        return ["weaviate-client >= 4.6.1", "trace-attributes >= 4.0.2"]
 
     def _instrument(self, **kwargs):
         tracer_provider = kwargs.get("tracer_provider")
         tracer = get_tracer(__name__, "", tracer_provider)
-        version = importlib.metadata.version("qdrant-client")
+        version = importlib.metadata.version("weaviate-client")
 
-        for operation, _ in APIS.items():
-            wrap_function_wrapper(
-                "qdrant_client.qdrant_client",
-                f"QdrantClient.{operation.lower()}",
-                collection_patch(operation, version, tracer),
-            )
+        for api_name, api_config in APIS.items():
+            module_path, function_name = api_name.rsplit(".", 1)
+            if api_config.get("OPERATION") == "query":
+                wrap_function_wrapper(
+                    api_config["MODULE"],
+                    api_config["METHOD"],
+                    generic_query_patch(api_name, version, tracer),
+                )
+            elif api_config.get("OPERATION") == "create":
+                wrap_function_wrapper(
+                    api_config["MODULE"],
+                    api_config["METHOD"],
+                    generic_collection_patch(api_name, version, tracer),
+                )
 
     def _instrument_module(self, module_name):
         pass
 
     def _uninstrument(self, **kwargs):
         pass
```

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/qdrant/patch.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/qdrant/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/weaviate/instrumentation.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,53 +14,40 @@
 limitations under the License.
 """
 
 import importlib.metadata
 import logging
 from typing import Collection
 
+from langtrace.trace_attributes import PineconeMethods
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.trace import get_tracer
 from wrapt import wrap_function_wrapper
 
-from langtrace_python_sdk.instrumentation.weaviate.patch import (
-    generic_collection_patch,
-    generic_query_patch,
-)
-from langtrace_python_sdk.constants.instrumentation.weaviate import APIS
+from langtrace_python_sdk.constants.instrumentation.pinecone import APIS
+from langtrace_python_sdk.instrumentation.pinecone.patch import generic_patch
 
 logging.basicConfig(level=logging.FATAL)
 
 
-class WeaviateInstrumentation(BaseInstrumentor):
-    """
-    The WeaviateInstrumentation class represents the instrumentation for the Weaviate SDK.
+class PineconeInstrumentation(BaseInstrumentor):
     """
+    The PineconeInstrumentation class represents the Pinecone instrumentation"""
 
     def instrumentation_dependencies(self) -> Collection[str]:
-        return ["weaviate-client >= 4.6.1", "trace-attributes >= 4.0.2"]
+        return ["pinecone-client >= 3.1.0"]
 
     def _instrument(self, **kwargs):
         tracer_provider = kwargs.get("tracer_provider")
         tracer = get_tracer(__name__, "", tracer_provider)
-        version = importlib.metadata.version("weaviate-client")
-
-        for api_name, api_config in APIS.items():
-            module_path, function_name = api_name.rsplit(".", 1)
-            if api_config.get("OPERATION") == "query":
-                wrap_function_wrapper(
-                    api_config["MODULE"],
-                    api_config["METHOD"],
-                    generic_query_patch(api_name, version, tracer),
-                )
-            elif api_config.get("OPERATION") == "create":
-                wrap_function_wrapper(
-                    api_config["MODULE"],
-                    api_config["METHOD"],
-                    generic_collection_patch(api_name, version, tracer),
-                )
-
-    def _instrument_module(self, module_name):
-        pass
+        version = importlib.metadata.version("pinecone-client")
+        for operation_name, details in APIS.items():
+            operation = details["OPERATION"]
+            # Dynamically creating the patching call
+            wrap_function_wrapper(
+                "pinecone.data.index",
+                f"Index.{operation}",
+                generic_patch(operation_name, version, tracer),
+            )
 
     def _uninstrument(self, **kwargs):
         pass
```

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/instrumentation/weaviate/patch.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/weaviate/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/types/__init__.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/types/__init__.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/utils/llm.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/utils/llm.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/utils/misc.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/utils/misc.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/utils/prompt_registry.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/utils/prompt_registry.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/langtrace_python_sdk/utils/with_root_span.py` & `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/utils/with_root_span.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,33 +11,33 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import asyncio
+import os
 from functools import wraps
 from typing import Optional
 
+import requests
+from opentelemetry import baggage, context, trace
+from opentelemetry.trace import SpanKind
+
 from langtrace_python_sdk.constants.exporter.langtrace_exporter import (
     LANGTRACE_REMOTE_URL,
 )
+from langtrace_python_sdk.constants.instrumentation.common import (
+    LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY,
+)
 from langtrace_python_sdk.utils.types import (
     EvaluationAPIData,
     LangTraceApiError,
     LangTraceEvaluation,
 )
-from opentelemetry import baggage, context, trace
-from opentelemetry.trace import SpanKind
-
-from langtrace_python_sdk.constants.instrumentation.common import (
-    LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY,
-)
-import os
-import requests
 
 
 def with_langtrace_root_span(
     name="LangtraceRootSpan",
     kind=SpanKind.INTERNAL,
 ):
 
@@ -157,15 +157,15 @@
     try:
         response = requests.get(
             f"{LANGTRACE_REMOTE_URL}/api/evaluation",
             params={"spanId": span_id},
             headers={"x-api-key": os.environ["LANGTRACE_API_KEY"]},
             timeout=None,
         )
-        evaluations = response.json()["evaluations"]
+        evaluations = response.json().get("evaluations", [])
         response.raise_for_status()
         return None if not evaluations else evaluations[0]
 
     except requests.RequestException as err:
         if err.response is not None:
             message = (
                 err.response.json().get("message", "")
```

### Comparing `langtrace_python_sdk-2.1.1/src/tests/conftest.py` & `langtrace_python_sdk-2.1.2/src/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/tests/utils.py` & `langtrace_python_sdk-2.1.2/src/tests/utils.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/tests/anthropic/conftest.py` & `langtrace_python_sdk-2.1.2/src/tests/anthropic/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/tests/anthropic/test_anthropic.py` & `langtrace_python_sdk-2.1.2/src/tests/anthropic/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/tests/anthropic/cassettes/test_anthropic.yaml` & `langtrace_python_sdk-2.1.2/src/tests/anthropic/cassettes/test_anthropic.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml` & `langtrace_python_sdk-2.1.2/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml` & `langtrace_python_sdk-2.1.2/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/tests/chroma/test_chroma.py` & `langtrace_python_sdk-2.1.2/src/tests/chroma/test_chroma.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/tests/cohere/conftest.py` & `langtrace_python_sdk-2.1.2/src/tests/cohere/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/tests/cohere/test_cohere_chat.py` & `langtrace_python_sdk-2.1.2/src/tests/cohere/test_cohere_chat.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/tests/cohere/test_cohere_embed.py` & `langtrace_python_sdk-2.1.2/src/tests/cohere/test_cohere_embed.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/tests/cohere/test_cohere_rerank.py` & `langtrace_python_sdk-2.1.2/src/tests/cohere/test_cohere_rerank.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/tests/cohere/cassettes/test_cohere_chat.yaml` & `langtrace_python_sdk-2.1.2/src/tests/cohere/cassettes/test_cohere_chat.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/tests/cohere/cassettes/test_cohere_chat_streaming.yaml` & `langtrace_python_sdk-2.1.2/src/tests/cohere/cassettes/test_cohere_chat_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/tests/cohere/cassettes/test_cohere_embed.yaml` & `langtrace_python_sdk-2.1.2/src/tests/cohere/cassettes/test_cohere_embed.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/tests/cohere/cassettes/test_cohere_rerank.yaml` & `langtrace_python_sdk-2.1.2/src/tests/cohere/cassettes/test_cohere_rerank.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/tests/langchain/test_langchain.py` & `langtrace_python_sdk-2.1.2/src/tests/langchain/test_langchain.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/tests/langchain/test_langchain_community.py` & `langtrace_python_sdk-2.1.2/src/tests/langchain/test_langchain_community.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/tests/langchain/test_langchain_core.py` & `langtrace_python_sdk-2.1.2/src/tests/langchain/test_langchain_core.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/tests/openai/conftest.py` & `langtrace_python_sdk-2.1.2/src/tests/openai/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/tests/openai/test_chat_completion.py` & `langtrace_python_sdk-2.1.2/src/tests/openai/test_chat_completion.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/tests/openai/test_image_generation.py` & `langtrace_python_sdk-2.1.2/src/tests/openai/test_image_generation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml` & `langtrace_python_sdk-2.1.2/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/tests/openai/cassettes/test_async_image_generation.yaml` & `langtrace_python_sdk-2.1.2/src/tests/openai/cassettes/test_async_image_generation.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/tests/openai/cassettes/test_chat_completion.yaml` & `langtrace_python_sdk-2.1.2/src/tests/openai/cassettes/test_chat_completion.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/tests/openai/cassettes/test_chat_completion_streaming.yaml` & `langtrace_python_sdk-2.1.2/src/tests/openai/cassettes/test_chat_completion_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/tests/openai/cassettes/test_image_generation.yaml` & `langtrace_python_sdk-2.1.2/src/tests/openai/cassettes/test_image_generation.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/tests/pinecone/conftest.py` & `langtrace_python_sdk-2.1.2/src/tests/pinecone/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/tests/pinecone/test_pinecone.py` & `langtrace_python_sdk-2.1.2/src/tests/pinecone/test_pinecone.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/tests/pinecone/cassettes/test_query.yaml` & `langtrace_python_sdk-2.1.2/src/tests/pinecone/cassettes/test_query.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/tests/pinecone/cassettes/test_upsert.yaml` & `langtrace_python_sdk-2.1.2/src/tests/pinecone/cassettes/test_upsert.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/src/tests/qdrant/test_qdrant.py` & `langtrace_python_sdk-2.1.2/src/tests/qdrant/test_qdrant.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/.gitignore` & `langtrace_python_sdk-2.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/LICENSE` & `langtrace_python_sdk-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/README.md` & `langtrace_python_sdk-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.1/pyproject.toml` & `langtrace_python_sdk-2.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -14,34 +14,33 @@
 license = "Apache-2.0"
 classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  'trace-attributes>=4.0.2',
-  'opentelemetry-api',
-  'opentelemetry-sdk',
-  'opentelemetry-instrumentation',
-  'pinecone-client',
-  'tiktoken',
+  'trace-attributes>=4.0.4',
+  'opentelemetry-api>=1.24.0',
+  'opentelemetry-sdk>=1.24.0',
+  'opentelemetry-instrumentation>=0.45b0',
+  'tiktoken>=0.1.1',
   'opentelemetry-exporter-otlp-proto-http>=1.24.0',
   'opentelemetry-exporter-otlp-proto-grpc>=1.24.0',
-  'weaviate-client',
 ]
 
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = [
     "openai",
     "anthropic",
     "chromadb",
     'qdrant-client',
     "python-dotenv",
+    'pinecone-client',
     "langchain",
     'langchain-community',
     "langchain-openai",
     "langchain-openai",
     "chromadb",
     "cohere",
     "qdrant_client",
```

### Comparing `langtrace_python_sdk-2.1.1/PKG-INFO` & `langtrace_python_sdk-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 Metadata-Version: 2.3
 Name: langtrace-python-sdk
-Version: 2.1.1
+Version: 2.1.2
 Summary: Python SDK for LangTrace
 Project-URL: Homepage, https://github.com/Scale3-Labs/langtrace-python-sdk
 Author-email: Scale3 Labs <engineering@scale3labs.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
-Requires-Dist: opentelemetry-api
+Requires-Dist: opentelemetry-api>=1.24.0
 Requires-Dist: opentelemetry-exporter-otlp-proto-grpc>=1.24.0
 Requires-Dist: opentelemetry-exporter-otlp-proto-http>=1.24.0
-Requires-Dist: opentelemetry-instrumentation
-Requires-Dist: opentelemetry-sdk
-Requires-Dist: pinecone-client
-Requires-Dist: tiktoken
-Requires-Dist: trace-attributes>=4.0.2
-Requires-Dist: weaviate-client
+Requires-Dist: opentelemetry-instrumentation>=0.45b0
+Requires-Dist: opentelemetry-sdk>=1.24.0
+Requires-Dist: tiktoken>=0.1.1
+Requires-Dist: trace-attributes>=4.0.4
 Provides-Extra: dev
 Requires-Dist: anthropic; extra == 'dev'
 Requires-Dist: chromadb; extra == 'dev'
 Requires-Dist: cohere; extra == 'dev'
 Requires-Dist: langchain; extra == 'dev'
 Requires-Dist: langchain-community; extra == 'dev'
 Requires-Dist: langchain-openai; extra == 'dev'
 Requires-Dist: openai; extra == 'dev'
+Requires-Dist: pinecone-client; extra == 'dev'
 Requires-Dist: python-dotenv; extra == 'dev'
 Requires-Dist: qdrant-client; extra == 'dev'
 Requires-Dist: weaviate-client; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-asyncio; extra == 'test'
 Requires-Dist: pytest-vcr; extra == 'test'
```

