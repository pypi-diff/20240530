# Comparing `tmp/langtrace_python_sdk-2.1.2.tar.gz` & `tmp/langtrace_python_sdk-2.1.4.tar.gz`

## Comparing `langtrace_python_sdk-2.1.2.tar` & `langtrace_python_sdk-2.1.4.tar`

### file list

```diff
@@ -1,146 +1,146 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/__init__.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/run_example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/anthropic_example/__init__.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/anthropic_example/completion.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/chroma_example/__init__.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/chroma_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/cohere_example/__init__.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/cohere_example/chat.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/cohere_example/chat_stream.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/cohere_example/embed.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/cohere_example/rerank.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/cohere_example/tools.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/fastapi_example/basic_route.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/hiveagent_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/langchain_example/__init__.py
--rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/langchain_example/basic.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/langchain_example/groq_example.py
--rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/langchain_example/langgraph_example.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/langchain_example/tool.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/llamaindex_example/__init__.py
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/llamaindex_example/agent.py
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/llamaindex_example/basic.py
--rw-r--r--   0        0        0    32667 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/llamaindex_example/data/abramov.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/openai_example/__init__.py
--rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/openai_example/async_tool_calling_nonstreaming.py
--rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/openai_example/async_tool_calling_streaming.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/openai_example/chat_completion.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/openai_example/embeddings_create.py
--rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/openai_example/function_calling.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/openai_example/images_generate.py
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/openai_example/tool_calling.py
--rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/openai_example/tool_calling_nonstreaming.py
--rw-r--r--   0        0        0     7015 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/openai_example/tool_calling_streaming.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/perplexity_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/pinecone_example/__init__.py
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/pinecone_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/qdrant_example/__init__.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/qdrant_example/basic.py
--rw-r--r--   0        0        0    64533 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/examples/weaviate_example/query_text.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/__init__.py
--rw-r--r--   0        0        0     6993 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/langtrace.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/constants/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/constants/exporter/langtrace_exporter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/constants/instrumentation/__init__.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/constants/instrumentation/anthropic.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/constants/instrumentation/chroma.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/constants/instrumentation/cohere.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/constants/instrumentation/common.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/constants/instrumentation/groq.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/constants/instrumentation/openai.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/constants/instrumentation/pinecone.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/constants/instrumentation/qdrant.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/constants/instrumentation/weaviate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/extensions/__init__.py
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/extensions/langtrace_exporter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/anthropic/__init__.py
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py
--rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/anthropic/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/chroma/__init__.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py
--rw-r--r--   0        0        0     8750 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/chroma/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/cohere/__init__.py
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py
--rw-r--r--   0        0        0    26563 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/cohere/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/groq/__init__.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py
--rw-r--r--   0        0        0    26068 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/groq/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langchain/__init__.py
--rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py
--rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langchain/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langchain_community/__init__.py
--rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py
--rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langchain_core/__init__.py
--rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py
--rw-r--r--   0        0        0     8458 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langgraph/__init__.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py
--rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langgraph/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/llamaindex/__init__.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py
--rw-r--r--   0        0        0     4189 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py
--rw-r--r--   0        0        0    37288 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/openai/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/pinecone/__init__.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py
--rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/pinecone/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/qdrant/__init__.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py
--rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/qdrant/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/weaviate/__init__.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/weaviate/instrumentation.py
--rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/weaviate/patch.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/types/__init__.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/utils/__init__.py
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/utils/llm.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/utils/misc.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/utils/prompt_registry.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/utils/silently_fail.py
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/utils/types.py
--rw-r--r--   0        0        0     6103 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/utils/with_root_span.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/__init__.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/conftest.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/utils.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/anthropic/conftest.py
--rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/anthropic/test_anthropic.py
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/anthropic/cassettes/test_anthropic.yaml
--rw-r--r--   0        0        0    11675 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml
--rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/chroma/conftest.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/chroma/test_chroma.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/cohere/conftest.py
--rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/cohere/test_cohere_chat.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/cohere/test_cohere_embed.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/cohere/test_cohere_rerank.py
--rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/cohere/cassettes/test_cohere_chat.yaml
--rw-r--r--   0        0        0     8174 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/cohere/cassettes/test_cohere_chat_streaming.yaml
--rw-r--r--   0        0        0    27320 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/cohere/cassettes/test_cohere_embed.yaml
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/cohere/cassettes/test_cohere_rerank.yaml
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/langchain/test_langchain.py
--rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/langchain/test_langchain_community.py
--rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/langchain/test_langchain_core.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/openai/conftest.py
--rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/openai/test_chat_completion.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/openai/test_embeddings.py
--rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/openai/test_image_generation.py
--rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/openai/cassettes/test_async_image_generation.yaml
--rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/openai/cassettes/test_chat_completion.yaml
--rw-r--r--   0        0        0  2592394 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/openai/cassettes/test_chat_completion_streaming.yaml
--rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/openai/cassettes/test_image_generation.yaml
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/pinecone/conftest.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/pinecone/test_pinecone.py
--rw-r--r--   0        0        0   103821 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/pinecone/cassettes/test_query.yaml
--rw-r--r--   0        0        0    38607 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/pinecone/cassettes/test_upsert.yaml
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/qdrant/conftest.py
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/src/tests/qdrant/test_qdrant.py
--rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/.gitignore
--rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/LICENSE
--rw-r--r--   0        0        0    10255 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/README.md
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/pyproject.toml
--rw-r--r--   0        0        0    11738 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/__init__.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/run_example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/anthropic_example/__init__.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/anthropic_example/completion.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/chroma_example/__init__.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/chroma_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/cohere_example/__init__.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/cohere_example/chat.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/cohere_example/chat_stream.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/cohere_example/embed.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/cohere_example/rerank.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/cohere_example/tools.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/fastapi_example/basic_route.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/hiveagent_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/langchain_example/__init__.py
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/langchain_example/basic.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/langchain_example/groq_example.py
+-rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/langchain_example/langgraph_example.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/langchain_example/tool.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/llamaindex_example/__init__.py
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/llamaindex_example/agent.py
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/llamaindex_example/basic.py
+-rw-r--r--   0        0        0    32667 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/llamaindex_example/data/abramov.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/openai_example/__init__.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/openai_example/async_tool_calling_nonstreaming.py
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/openai_example/async_tool_calling_streaming.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/openai_example/chat_completion.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/openai_example/embeddings_create.py
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/openai_example/function_calling.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/openai_example/images_generate.py
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/openai_example/tool_calling.py
+-rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/openai_example/tool_calling_nonstreaming.py
+-rw-r--r--   0        0        0     7015 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/openai_example/tool_calling_streaming.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/perplexity_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/pinecone_example/__init__.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/pinecone_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/qdrant_example/__init__.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/qdrant_example/basic.py
+-rw-r--r--   0        0        0    64533 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/examples/weaviate_example/query_text.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/__init__.py
+-rw-r--r--   0        0        0     7409 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/langtrace.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/constants/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/constants/exporter/langtrace_exporter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/constants/instrumentation/__init__.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/constants/instrumentation/anthropic.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/constants/instrumentation/chroma.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/constants/instrumentation/cohere.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/constants/instrumentation/common.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/constants/instrumentation/groq.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/constants/instrumentation/openai.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/constants/instrumentation/pinecone.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/constants/instrumentation/qdrant.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/constants/instrumentation/weaviate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/extensions/__init__.py
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/extensions/langtrace_exporter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/anthropic/__init__.py
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py
+-rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/anthropic/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/chroma/__init__.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py
+-rw-r--r--   0        0        0     8750 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/chroma/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/cohere/__init__.py
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py
+-rw-r--r--   0        0        0    26563 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/cohere/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/groq/__init__.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py
+-rw-r--r--   0        0        0    26068 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/groq/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langchain/__init__.py
+-rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langchain/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langchain_community/__init__.py
+-rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py
+-rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langchain_core/__init__.py
+-rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py
+-rw-r--r--   0        0        0     8458 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langgraph/__init__.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py
+-rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langgraph/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/llamaindex/__init__.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py
+-rw-r--r--   0        0        0     4189 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py
+-rw-r--r--   0        0        0    37288 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/openai/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/pinecone/__init__.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py
+-rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/pinecone/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/qdrant/__init__.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py
+-rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/qdrant/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/weaviate/__init__.py
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/weaviate/instrumentation.py
+-rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/weaviate/patch.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/types/__init__.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/utils/__init__.py
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/utils/llm.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/utils/misc.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/utils/prompt_registry.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/utils/silently_fail.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/utils/types.py
+-rw-r--r--   0        0        0     5957 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/utils/with_root_span.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/__init__.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/conftest.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/utils.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/anthropic/conftest.py
+-rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/anthropic/test_anthropic.py
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/anthropic/cassettes/test_anthropic.yaml
+-rw-r--r--   0        0        0    11675 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml
+-rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/chroma/conftest.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/chroma/test_chroma.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/cohere/conftest.py
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/cohere/test_cohere_chat.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/cohere/test_cohere_embed.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/cohere/test_cohere_rerank.py
+-rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/cohere/cassettes/test_cohere_chat.yaml
+-rw-r--r--   0        0        0     8174 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/cohere/cassettes/test_cohere_chat_streaming.yaml
+-rw-r--r--   0        0        0    27320 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/cohere/cassettes/test_cohere_embed.yaml
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/cohere/cassettes/test_cohere_rerank.yaml
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/langchain/conftest.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/langchain/test_langchain.py
+-rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/langchain/cassettes/test_langchain.yaml
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/openai/conftest.py
+-rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/openai/test_chat_completion.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/openai/test_embeddings.py
+-rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/openai/test_image_generation.py
+-rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/openai/cassettes/test_async_image_generation.yaml
+-rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/openai/cassettes/test_chat_completion.yaml
+-rw-r--r--   0        0        0  2592394 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/openai/cassettes/test_chat_completion_streaming.yaml
+-rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/openai/cassettes/test_image_generation.yaml
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/pinecone/conftest.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/pinecone/test_pinecone.py
+-rw-r--r--   0        0        0   103821 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/pinecone/cassettes/test_query.yaml
+-rw-r--r--   0        0        0    38607 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/pinecone/cassettes/test_upsert.yaml
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/qdrant/conftest.py
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/src/tests/qdrant/test_qdrant.py
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/.gitignore
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/LICENSE
+-rw-r--r--   0        0        0    10255 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/README.md
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/pyproject.toml
+-rw-r--r--   0        0        0    11769 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.4/PKG-INFO
```

### Comparing `langtrace_python_sdk-2.1.2/src/run_example.py` & `langtrace_python_sdk-2.1.4/src/run_example.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/examples/anthropic_example/completion.py` & `langtrace_python_sdk-2.1.4/src/examples/anthropic_example/completion.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/examples/chroma_example/basic.py` & `langtrace_python_sdk-2.1.4/src/examples/chroma_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/examples/cohere_example/chat.py` & `langtrace_python_sdk-2.1.4/src/examples/cohere_example/chat.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/examples/cohere_example/chat_stream.py` & `langtrace_python_sdk-2.1.4/src/examples/cohere_example/chat_stream.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/examples/cohere_example/embed.py` & `langtrace_python_sdk-2.1.4/src/examples/cohere_example/embed.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/examples/cohere_example/rerank.py` & `langtrace_python_sdk-2.1.4/src/examples/cohere_example/rerank.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/examples/cohere_example/tools.py` & `langtrace_python_sdk-2.1.4/src/examples/cohere_example/tools.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/examples/fastapi_example/basic_route.py` & `langtrace_python_sdk-2.1.4/src/examples/fastapi_example/basic_route.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/examples/langchain_example/basic.py` & `langtrace_python_sdk-2.1.4/src/examples/langchain_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/examples/langchain_example/groq_example.py` & `langtrace_python_sdk-2.1.4/src/examples/langchain_example/groq_example.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/examples/langchain_example/langgraph_example.py` & `langtrace_python_sdk-2.1.4/src/examples/langchain_example/langgraph_example.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/examples/langchain_example/tool.py` & `langtrace_python_sdk-2.1.4/src/examples/langchain_example/tool.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/examples/llamaindex_example/agent.py` & `langtrace_python_sdk-2.1.4/src/examples/llamaindex_example/agent.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/examples/llamaindex_example/basic.py` & `langtrace_python_sdk-2.1.4/src/examples/llamaindex_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/examples/llamaindex_example/data/abramov.txt` & `langtrace_python_sdk-2.1.4/src/examples/llamaindex_example/data/abramov.txt`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/examples/openai_example/async_tool_calling_nonstreaming.py` & `langtrace_python_sdk-2.1.4/src/examples/openai_example/async_tool_calling_nonstreaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/examples/openai_example/async_tool_calling_streaming.py` & `langtrace_python_sdk-2.1.4/src/examples/openai_example/async_tool_calling_streaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/examples/openai_example/chat_completion.py` & `langtrace_python_sdk-2.1.4/src/examples/openai_example/chat_completion.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/examples/openai_example/function_calling.py` & `langtrace_python_sdk-2.1.4/src/examples/openai_example/function_calling.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/examples/openai_example/tool_calling.py` & `langtrace_python_sdk-2.1.4/src/examples/openai_example/tool_calling.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/examples/openai_example/tool_calling_nonstreaming.py` & `langtrace_python_sdk-2.1.4/src/examples/openai_example/tool_calling_nonstreaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/examples/openai_example/tool_calling_streaming.py` & `langtrace_python_sdk-2.1.4/src/examples/openai_example/tool_calling_streaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/examples/perplexity_example/basic.py` & `langtrace_python_sdk-2.1.4/src/examples/perplexity_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/examples/pinecone_example/basic.py` & `langtrace_python_sdk-2.1.4/src/examples/pinecone_example/basic.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,35 +25,33 @@
         dimension=1536,
         metric="cosine",
         spec=ServerlessSpec(cloud="aws", region="us-east-1"),
     )
 
 
 @with_langtrace_root_span()
-def basic(span_id, trace_id):
+def basic(span_id=None, trace_id=None):
 
     result = client.embeddings.create(
         model="text-embedding-ada-002",
         input="Some random text string goes here",
         encoding_format="float",
     )
 
     embedding = result.data[0].embedding
 
     unique_id = "unique_random_id"
     data_to_upsert = {"id": unique_id, "values": embedding}
 
     index = pinecone.Index(PINECONE_INDEX_NAME)
     res = index.upsert(vectors=[data_to_upsert], namespace="test-namespace")
-    print("res", res)
 
     resp = index.query(
         vector=embedding, top_k=1, include_values=False, namespace="test-namespace"
     )
     send_user_feedback(
         {"spanId": span_id, "traceId": trace_id, "userScore": 1, "userId": "123"}
     )
-    print(resp)
+    return [res, resp]
 
 
 # create_index()
-basic("span_id", "trace_id")
```

### Comparing `langtrace_python_sdk-2.1.2/src/examples/qdrant_example/basic.py` & `langtrace_python_sdk-2.1.4/src/examples/qdrant_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/examples/weaviate_example/query_text.py` & `langtrace_python_sdk-2.1.4/src/examples/weaviate_example/query_text.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/__init__.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/langtrace.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/langtrace.py`

 * *Files 9% similar despite different names*

```diff
@@ -64,50 +64,57 @@
 from langtrace_python_sdk.instrumentation.qdrant.instrumentation import (
     QdrantInstrumentation,
 )
 from langtrace_python_sdk.instrumentation.weaviate.instrumentation import (
     WeaviateInstrumentation,
 )
 
+from colorama import Fore
+
 
 def init(
     api_key: str = None,
     batch: bool = True,
     write_spans_to_console: bool = False,
     custom_remote_exporter=None,
     api_host: Optional[str] = None,
     disable_instrumentations: Optional[DisableInstrumentations] = None,
 ):
+    print(Fore.GREEN + "Initializing Langtrace SDK.." + Fore.RESET)
     provider = TracerProvider(resource=Resource.create({"service.name": sys.argv[0]}))
 
     remote_write_exporter = (
         LangTraceExporter(api_key=api_key, api_host=api_host)
         if custom_remote_exporter is None
         else custom_remote_exporter
     )
     console_exporter = ConsoleSpanExporter()
     batch_processor_remote = BatchSpanProcessor(remote_write_exporter)
     simple_processor_remote = SimpleSpanProcessor(remote_write_exporter)
     simple_processor_console = SimpleSpanProcessor(console_exporter)
 
     if write_spans_to_console:
+        print(Fore.BLUE + "Writing spans to console" + Fore.RESET)
         provider.add_span_processor(simple_processor_console)
 
     elif custom_remote_exporter is not None:
+        print(Fore.BLUE + f"Exporting spans to custom remote exporter.." + Fore.RESET)
         if batch:
             provider.add_span_processor(batch_processor_remote)
         else:
             provider.add_span_processor(simple_processor_remote)
 
     elif api_host is not None:
+        print(Fore.BLUE + f"Exporting spans to custom host: {api_host}.." + Fore.RESET)
         if batch:
             provider.add_span_processor(batch_processor_remote)
         else:
             provider.add_span_processor(simple_processor_remote)
     else:
+        print(Fore.BLUE + "Exporting spans to Langtrace cloud.." + Fore.RESET)
         provider.add_span_processor(batch_processor_remote)
 
     # Initialize tracer
     trace.set_tracer_provider(provider)
 
     all_instrumentations = {
         "openai": OpenAIInstrumentation(),
```

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/constants/instrumentation/chroma.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/constants/instrumentation/chroma.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/constants/instrumentation/cohere.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/constants/instrumentation/cohere.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/constants/instrumentation/common.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/constants/instrumentation/common.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/constants/instrumentation/openai.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/constants/instrumentation/openai.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/constants/instrumentation/qdrant.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/constants/instrumentation/qdrant.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/constants/instrumentation/weaviate.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/constants/instrumentation/weaviate.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/extensions/langtrace_exporter.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/extensions/langtrace_exporter.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import requests
 from opentelemetry.sdk.trace.export import ReadableSpan, SpanExporter, SpanExportResult
 from opentelemetry.trace.span import format_trace_id
 
 from langtrace_python_sdk.constants.exporter.langtrace_exporter import (
     LANGTRACE_REMOTE_URL,
 )
+from colorama import Fore
+from requests.exceptions import RequestException
 
 
 class LangTraceExporter(SpanExporter):
     """
     **LangTraceExporter Class**
 
     This class exports telemetry data in the LangTrace format to a remote URL. It inherits from the `SpanExporter` class in OpenTelemetry.
@@ -51,47 +53,60 @@
         self,
         api_key: str = None,
         api_host: typing.Optional[str] = None,
     ) -> None:
         self.api_key = api_key or os.environ.get("LANGTRACE_API_KEY")
         self.api_host: str = api_host or LANGTRACE_REMOTE_URL
 
-        if not self.api_key:
-            raise ValueError("No API key provided")
-
     def export(self, spans: typing.Sequence[ReadableSpan]) -> SpanExportResult:
         """
         Exports a batch of telemetry data.
 
         Args:
             spans: The list of `opentelemetry.trace.Span` objects to be exported
 
         Returns:
             The result of the export SUCCESS or FAILURE
         """
+        if not self.api_key:
+            print(Fore.RED)
+            print(
+                "Missing Langtrace API key, proceed to https://langtrace.ai to create one"
+            )
+            print("Set the API key as an environment variable LANGTRACE_API_KEY")
+            print(Fore.RESET)
+            return
         data = [
             {
                 "traceId": format_trace_id(span.get_span_context().trace_id),
-                "instrumentationLibrary": span.instrumentation_info.__repr__(),
                 "droppedEventsCount": span.dropped_events,
                 "droppedAttributesCount": span.dropped_attributes,
                 "droppedLinksCount": span.dropped_links,
                 "ended": span.status.is_ok,
                 **json.loads(span.to_json()),
             }
             for span in spans
         ]
 
         # Send data to remote URL
         try:
-            requests.post(
+            response = requests.post(
                 url=f"{self.api_host}/api/trace",
                 data=json.dumps(data),
                 headers={"Content-Type": "application/json", "x-api-key": self.api_key},
+                timeout=20,
+            )
+
+            if not response.ok:
+                raise RequestException(response.text)
+
+            print(
+                Fore.GREEN + f"Exported {len(spans)} spans successfully." + Fore.RESET
             )
-            print(f"sent to {self.api_host}/api/trace with {len(data)} spans")
             return SpanExportResult.SUCCESS
-        except Exception as e:
+        except RequestException as err:
+            print(Fore.RED + "Failed to export spans.")
+            print(Fore.RED + f"Error: {err}" + Fore.RESET)
             return SpanExportResult.FAILURE
 
     def shutdown(self) -> None:
         pass
```

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/anthropic/patch.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/anthropic/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/chroma/patch.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/chroma/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/cohere/patch.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/cohere/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/groq/patch.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/groq/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langchain/patch.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langchain/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/langgraph/patch.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/langgraph/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/openai/patch.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/openai/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/pinecone/patch.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/pinecone/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/qdrant/patch.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/qdrant/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/weaviate/instrumentation.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/weaviate/instrumentation.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import importlib.metadata
 import logging
 from typing import Collection
-
+from opentelemetry.instrumentation.utils import unwrap
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.trace import get_tracer
 from wrapt import wrap_function_wrapper
 
 from langtrace_python_sdk.instrumentation.weaviate.patch import (
     generic_collection_patch,
     generic_query_patch,
 )
 from langtrace_python_sdk.constants.instrumentation.weaviate import APIS
 
-logging.basicConfig(level=logging.FATAL)
+logging.basicConfig(level=logging.DEBUG)  # Set to DEBUG for detailed logging
 
 
 class WeaviateInstrumentation(BaseInstrumentor):
     """
     The WeaviateInstrumentation class represents the instrumentation for the Weaviate SDK.
     """
 
@@ -43,24 +43,26 @@
         tracer_provider = kwargs.get("tracer_provider")
         tracer = get_tracer(__name__, "", tracer_provider)
         version = importlib.metadata.version("weaviate-client")
 
         for api_name, api_config in APIS.items():
             module_path, function_name = api_name.rsplit(".", 1)
             if api_config.get("OPERATION") == "query":
-                wrap_function_wrapper(
-                    api_config["MODULE"],
-                    api_config["METHOD"],
-                    generic_query_patch(api_name, version, tracer),
-                )
+                if getattr(api_config["MODULE"], api_config["METHOD"], None):
+                    wrap_function_wrapper(
+                        api_config["MODULE"],
+                        api_config["METHOD"],
+                        generic_query_patch(api_name, version, tracer),
+                    )
             elif api_config.get("OPERATION") == "create":
-                wrap_function_wrapper(
-                    api_config["MODULE"],
-                    api_config["METHOD"],
-                    generic_collection_patch(api_name, version, tracer),
-                )
+                if getattr(api_config["MODULE"], api_config["METHOD"], None):
+                    wrap_function_wrapper(
+                        api_config["MODULE"],
+                        api_config["METHOD"],
+                        generic_collection_patch(api_name, version, tracer),
+                    )
 
     def _instrument_module(self, module_name):
         pass
 
     def _uninstrument(self, **kwargs):
         pass
```

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/instrumentation/weaviate/patch.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/instrumentation/weaviate/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/types/__init__.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/types/__init__.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/utils/llm.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/utils/llm.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/utils/misc.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/utils/misc.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/utils/prompt_registry.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/utils/prompt_registry.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/langtrace_python_sdk/utils/with_root_span.py` & `langtrace_python_sdk-2.1.4/src/langtrace_python_sdk/utils/with_root_span.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,26 +122,24 @@
                 f"{LANGTRACE_REMOTE_URL}/api/evaluation",
                 json=data,
                 params={"spanId": data["spanId"]},
                 headers=headers,
                 timeout=None,
             )
             response.raise_for_status()
-            print("SENDING FEEDBACK PUT", response.status_code, response.text)
 
         else:
             # Make a POST request to create a new evaluation
             response = requests.post(
                 f"{LANGTRACE_REMOTE_URL}/api/evaluation",
                 json=data,
                 params={"spanId": data["spanId"]},
                 headers=headers,
                 timeout=None,
             )
-            print("Response", response.status_code, response.text)
             response.raise_for_status()
 
     except requests.RequestException as err:
         # Handle specific HTTP errors or general request exceptions
         error_msg = str(err)
         if err.response:
             try:
```

### Comparing `langtrace_python_sdk-2.1.2/src/tests/conftest.py` & `langtrace_python_sdk-2.1.4/src/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/tests/utils.py` & `langtrace_python_sdk-2.1.4/src/tests/utils.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/tests/anthropic/conftest.py` & `langtrace_python_sdk-2.1.4/src/tests/anthropic/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/tests/anthropic/test_anthropic.py` & `langtrace_python_sdk-2.1.4/src/tests/anthropic/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/tests/anthropic/cassettes/test_anthropic.yaml` & `langtrace_python_sdk-2.1.4/src/tests/anthropic/cassettes/test_anthropic.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml` & `langtrace_python_sdk-2.1.4/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml` & `langtrace_python_sdk-2.1.4/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/tests/chroma/test_chroma.py` & `langtrace_python_sdk-2.1.4/src/tests/chroma/test_chroma.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/tests/cohere/conftest.py` & `langtrace_python_sdk-2.1.4/src/tests/cohere/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/tests/cohere/test_cohere_chat.py` & `langtrace_python_sdk-2.1.4/src/tests/cohere/test_cohere_chat.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/tests/cohere/test_cohere_embed.py` & `langtrace_python_sdk-2.1.4/src/tests/cohere/test_cohere_embed.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/tests/cohere/test_cohere_rerank.py` & `langtrace_python_sdk-2.1.4/src/tests/cohere/test_cohere_rerank.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/tests/cohere/cassettes/test_cohere_chat.yaml` & `langtrace_python_sdk-2.1.4/src/tests/cohere/cassettes/test_cohere_chat.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/tests/cohere/cassettes/test_cohere_chat_streaming.yaml` & `langtrace_python_sdk-2.1.4/src/tests/cohere/cassettes/test_cohere_chat_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/tests/cohere/cassettes/test_cohere_embed.yaml` & `langtrace_python_sdk-2.1.4/src/tests/cohere/cassettes/test_cohere_embed.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/tests/cohere/cassettes/test_cohere_rerank.yaml` & `langtrace_python_sdk-2.1.4/src/tests/cohere/cassettes/test_cohere_rerank.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/tests/openai/conftest.py` & `langtrace_python_sdk-2.1.4/src/tests/openai/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/tests/openai/test_chat_completion.py` & `langtrace_python_sdk-2.1.4/src/tests/openai/test_chat_completion.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/tests/openai/test_image_generation.py` & `langtrace_python_sdk-2.1.4/src/tests/openai/test_image_generation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml` & `langtrace_python_sdk-2.1.4/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/tests/openai/cassettes/test_async_image_generation.yaml` & `langtrace_python_sdk-2.1.4/src/tests/openai/cassettes/test_async_image_generation.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/tests/openai/cassettes/test_chat_completion.yaml` & `langtrace_python_sdk-2.1.4/src/tests/openai/cassettes/test_chat_completion.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/tests/openai/cassettes/test_chat_completion_streaming.yaml` & `langtrace_python_sdk-2.1.4/src/tests/openai/cassettes/test_chat_completion_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/tests/openai/cassettes/test_image_generation.yaml` & `langtrace_python_sdk-2.1.4/src/tests/openai/cassettes/test_image_generation.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/tests/pinecone/conftest.py` & `langtrace_python_sdk-2.1.4/src/tests/pinecone/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/tests/pinecone/test_pinecone.py` & `langtrace_python_sdk-2.1.4/src/tests/pinecone/test_pinecone.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/tests/pinecone/cassettes/test_query.yaml` & `langtrace_python_sdk-2.1.4/src/tests/pinecone/cassettes/test_query.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/tests/pinecone/cassettes/test_upsert.yaml` & `langtrace_python_sdk-2.1.4/src/tests/pinecone/cassettes/test_upsert.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/src/tests/qdrant/test_qdrant.py` & `langtrace_python_sdk-2.1.4/src/tests/qdrant/test_qdrant.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/.gitignore` & `langtrace_python_sdk-2.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/LICENSE` & `langtrace_python_sdk-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/README.md` & `langtrace_python_sdk-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.1.2/pyproject.toml` & `langtrace_python_sdk-2.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
   'trace-attributes>=4.0.4',
   'opentelemetry-api>=1.24.0',
   'opentelemetry-sdk>=1.24.0',
   'opentelemetry-instrumentation>=0.45b0',
   'tiktoken>=0.1.1',
   'opentelemetry-exporter-otlp-proto-http>=1.24.0',
   'opentelemetry-exporter-otlp-proto-grpc>=1.24.0',
+  'colorama>=0.4.6'
 ]
 
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = [
     "openai",
```

### Comparing `langtrace_python_sdk-2.1.2/PKG-INFO` & `langtrace_python_sdk-2.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.3
 Name: langtrace-python-sdk
-Version: 2.1.2
+Version: 2.1.4
 Summary: Python SDK for LangTrace
 Project-URL: Homepage, https://github.com/Scale3-Labs/langtrace-python-sdk
 Author-email: Scale3 Labs <engineering@scale3labs.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
+Requires-Dist: colorama>=0.4.6
 Requires-Dist: opentelemetry-api>=1.24.0
 Requires-Dist: opentelemetry-exporter-otlp-proto-grpc>=1.24.0
 Requires-Dist: opentelemetry-exporter-otlp-proto-http>=1.24.0
 Requires-Dist: opentelemetry-instrumentation>=0.45b0
 Requires-Dist: opentelemetry-sdk>=1.24.0
 Requires-Dist: tiktoken>=0.1.1
 Requires-Dist: trace-attributes>=4.0.4
```

