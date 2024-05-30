# Comparing `tmp/eidolon_ai_sdk-0.1.59.tar.gz` & `tmp/eidolon_ai_sdk-0.1.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eidolon_ai_sdk-0.1.59.tar", max compression
+gzip compressed data, was "eidolon_ai_sdk-0.1.60.tar", max compression
```

## Comparing `eidolon_ai_sdk-0.1.59.tar` & `eidolon_ai_sdk-0.1.60.tar`

### file list

```diff
@@ -1,145 +1,145 @@
--rw-r--r--   0        0        0      701 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/README.md
--rw-r--r--   0        0        0        0 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/__init__.py
--rw-r--r--   0        0        0     2424 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/agent.py
--rw-r--r--   0        0        0     1311 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/audio_agent.py
--rw-r--r--   0        0        0        0 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/__init__.py
--rw-r--r--   0        0        0     3850 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/document_manager.py
--rw-r--r--   0        0        0     2865 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/document_processor.py
--rw-r--r--   0        0        0        0 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/loaders/__init__.py
--rw-r--r--   0        0        0     1059 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py
--rw-r--r--   0        0        0     3405 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py
--rw-r--r--   0        0        0     4642 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py
--rw-r--r--   0        0        0        0 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/parsers/__init__.py
--rw-r--r--   0        0        0     2817 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py
--rw-r--r--   0        0        0     4519 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py
--rw-r--r--   0        0        0        0 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/__init__.py
--rw-r--r--   0        0        0      448 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/base_ast_generator.py
--rw-r--r--   0        0        0     3699 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py
--rw-r--r--   0        0        0     2053 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py
--rw-r--r--   0        0        0     3212 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py
--rw-r--r--   0        0        0     1647 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py
--rw-r--r--   0        0        0     1328 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py
--rw-r--r--   0        0        0     3356 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py
--rw-r--r--   0        0        0     1400 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py
--rw-r--r--   0        0        0        0 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/transformer/__init__.py
--rw-r--r--   0        0        0     1398 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py
--rw-r--r--   0        0        0     4786 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py
--rw-r--r--   0        0        0    43465 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py
--rw-r--r--   0        0        0     4825 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/generic_agent.py
--rw-r--r--   0        0        0        0 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/retriever_agent/__init__.py
--rw-r--r--   0        0        0     2078 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py
--rw-r--r--   0        0        0     1428 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py
--rw-r--r--   0        0        0     2323 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py
--rw-r--r--   0        0        0      559 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py
--rw-r--r--   0        0        0     2864 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/retriever_agent/retriever.py
--rw-r--r--   0        0        0     4142 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py
--rw-r--r--   0        0        0    13376 2024-05-28 17:58:20.123137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/simple_agent.py
--rw-r--r--   0        0        0        0 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/tot_agent/__init__.py
--rw-r--r--   0        0        0     1809 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/tot_agent/checker.py
--rw-r--r--   0        0        0     2468 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/tot_agent/controller.py
--rw-r--r--   0        0        0     1503 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/tot_agent/memory.py
--rw-r--r--   0        0        0     1423 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/tot_agent/prompts.py
--rw-r--r--   0        0        0      364 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/tot_agent/thought.py
--rw-r--r--   0        0        0     4951 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/tot_agent/thought_generators.py
--rw-r--r--   0        0        0     7614 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/tot_agent/tot_agent.py
--rw-r--r--   0        0        0     4572 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent_os.py
--rw-r--r--   0        0        0    12735 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent_os_interfaces.py
--rw-r--r--   0        0        0        0 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/bin/__init__.py
--rwxr-xr-x   0        0        0     9545 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/bin/agent_creator.py
--rw-r--r--   0        0        0     8381 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/bin/agent_http_server.py
--rwxr-xr-x   0        0        0     3789 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/bin/replay.py
--rw-r--r--   0        0        0        0 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/builtins/__init__.py
--rw-r--r--   0        0        0     9194 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/builtins/code_builtins.py
--rw-r--r--   0        0        0        0 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/builtins/components/__init__.py
--rw-r--r--   0        0        0     2223 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/builtins/components/opentelemetry.py
--rw-r--r--   0        0        0     4256 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/builtins/components/usage.py
--rw-r--r--   0        0        0        0 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/builtins/logic_units/__init__.py
--rw-r--r--   0        0        0     1822 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/builtins/logic_units/playwrite_browser.py
--rw-r--r--   0        0        0     6517 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/builtins/logic_units/web_search.py
--rw-r--r--   0        0        0      550 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml
--rw-r--r--   0        0        0      601 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/builtins/resources/claude_opus.yaml
--rw-r--r--   0        0        0      614 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml
--rw-r--r--   0        0        0      181 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/builtins/resources/machine.yaml
--rw-r--r--   0        0        0      597 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/builtins/resources/mistral_large.yaml
--rw-r--r--   0        0        0      547 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml
--rw-r--r--   0        0        0      540 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/builtins/resources/mistral_small.yaml
--rw-r--r--   0        0        0      595 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/builtins/resources/openai_35.yaml
--rw-r--r--   0        0        0      586 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/builtins/resources/openai_4.yaml
--rw-r--r--   0        0        0        0 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/__init__.py
--rw-r--r--   0        0        0     1843 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/agent_call_history.py
--rw-r--r--   0        0        0     3008 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/agent_io.py
--rw-r--r--   0        0        0     9128 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/agents_logic_unit.py
--rw-r--r--   0        0        0     6039 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/apu.py
--rw-r--r--   0        0        0     3790 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/audio_unit.py
--rw-r--r--   0        0        0      292 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/call_context.py
--rw-r--r--   0        0        0     2833 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/conversation_memory_unit.py
--rw-r--r--   0        0        0    14187 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/conversational_apu.py
--rw-r--r--   0        0        0     4841 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/image_unit.py
--rw-r--r--   0        0        0        0 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/llm/__init__.py
--rw-r--r--   0        0        0     9936 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py
--rw-r--r--   0        0        0    11967 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py
--rw-r--r--   0        0        0     4518 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py
--rw-r--r--   0        0        0     5753 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py
--rw-r--r--   0        0        0     9490 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py
--rw-r--r--   0        0        0     3597 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/llm/open_ai_speech.py
--rw-r--r--   0        0        0     3962 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/llm_message.py
--rw-r--r--   0        0        0     3099 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/llm_unit.py
--rw-r--r--   0        0        0     4491 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/logic_unit.py
--rw-r--r--   0        0        0     3541 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/memory_unit.py
--rw-r--r--   0        0        0      825 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/processing_unit.py
--rw-r--r--   0        0        0     5205 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/tool_call_unit.py
--rw-r--r--   0        0        0        0 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/io/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/memory/__init__.py
--rw-r--r--   0        0        0     1193 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/memory/agent_memory.py
--rw-r--r--   0        0        0     5309 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/memory/chroma_vector_store.py
--rw-r--r--   0        0        0      641 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/memory/document.py
--rw-r--r--   0        0        0     2766 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/memory/embeddings.py
--rw-r--r--   0        0        0      907 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/memory/file_memory.py
--rw-r--r--   0        0        0     4203 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/memory/file_system_vector_store.py
--rw-r--r--   0        0        0     3974 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/memory/in_memory_file_memory.py
--rw-r--r--   0        0        0     5788 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/memory/local_file_memory.py
--rw-r--r--   0        0        0     4845 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/memory/local_symbolic_memory.py
--rw-r--r--   0        0        0     3793 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/memory/mongo_symbolic_memory.py
--rw-r--r--   0        0        0      996 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/memory/noop_memory.py
--rw-r--r--   0        0        0     1984 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/memory/s3_file_memory.py
--rw-r--r--   0        0        0      974 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/memory/semantic_memory.py
--rw-r--r--   0        0        0     2809 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/memory/similarity_memory.py
--rw-r--r--   0        0        0     1516 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/memory/vector_store.py
--rw-r--r--   0        0        0        0 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/security/__init__.py
--rw-r--r--   0        0        0      771 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/security/authentication_processor.py
--rw-r--r--   0        0        0     2159 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/security/azure_authorizer.py
--rw-r--r--   0        0        0     1277 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/security/functional_authorizer.py
--rw-r--r--   0        0        0     2001 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/security/google_auth.py
--rw-r--r--   0        0        0     1867 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/security/jwt_processor.py
--rw-r--r--   0        0        0      484 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/security/okta_authorizor.py
--rw-r--r--   0        0        0     1017 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/security/permissions.py
--rw-r--r--   0        0        0     2508 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/security/process_authorizer.py
--rw-r--r--   0        0        0     2977 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/security/security_manager.py
--rw-r--r--   0        0        0     1035 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/security/security_middleware.py
--rw-r--r--   0        0        0      428 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/security/user.py
--rw-r--r--   0        0        0        0 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/system/__init__.py
--rw-r--r--   0        0        0     1473 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/system/agent_contract.py
--rw-r--r--   0        0        0    23004 2024-05-28 17:58:20.127137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/system/agent_controller.py
--rw-r--r--   0        0        0    14196 2024-05-28 17:58:20.131137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/system/agent_machine.py
--rw-r--r--   0        0        0     1149 2024-05-28 17:58:20.131137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/system/dynamic_middleware.py
--rw-r--r--   0        0        0     3432 2024-05-28 17:58:20.131137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/system/fn_handler.py
--rw-r--r--   0        0        0     4911 2024-05-28 17:58:20.131137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/system/process_file_system.py
--rw-r--r--   0        0        0     4275 2024-05-28 17:58:20.131137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/system/processes.py
--rw-r--r--   0        0        0     7664 2024-05-28 17:58:20.131137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/system/reference_model.py
--rw-r--r--   0        0        0        0 2024-05-28 17:58:20.131137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/system/resources/__init__.py
--rw-r--r--   0        0        0      314 2024-05-28 17:58:20.131137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/system/resources/agent_resource.py
--rw-r--r--   0        0        0      414 2024-05-28 17:58:20.131137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/system/resources/machine_resource.py
--rw-r--r--   0        0        0      684 2024-05-28 17:58:20.131137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/system/resources/reference_resource.py
--rw-r--r--   0        0        0     1663 2024-05-28 17:58:20.131137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/system/resources/resources_base.py
--rw-r--r--   0        0        0        0 2024-05-28 17:58:20.131137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/util/__init__.py
--rw-r--r--   0        0        0      509 2024-05-28 17:58:20.131137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/util/async_wrapper.py
--rw-r--r--   0        0        0     2806 2024-05-28 17:58:20.131137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/util/class_utils.py
--rw-r--r--   0        0        0     1604 2024-05-28 17:58:20.131137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/util/image_utils.py
--rw-r--r--   0        0        0     3808 2024-05-28 17:58:20.131137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/util/replay.py
--rw-r--r--   0        0        0     6917 2024-05-28 17:58:20.131137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/util/schema_to_model.py
--rw-r--r--   0        0        0      898 2024-05-28 17:58:20.131137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/util/str_utils.py
--rw-r--r--   0        0        0     3445 2024-05-28 17:58:20.131137 eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/util/stream_collector.py
--rw-r--r--   0        0        0      565 2024-05-28 17:58:20.131137 eidolon_ai_sdk-0.1.59/logging.conf
--rw-r--r--   0        0        0     2214 2024-05-28 17:58:20.131137 eidolon_ai_sdk-0.1.59/pyproject.toml
--rw-r--r--   0        0        0     2977 1970-01-01 00:00:00.000000 eidolon_ai_sdk-0.1.59/PKG-INFO
+-rw-r--r--   0        0        0      701 2024-05-29 20:01:15.598897 eidolon_ai_sdk-0.1.60/README.md
+-rw-r--r--   0        0        0        0 2024-05-29 20:01:15.598897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:01:15.598897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/__init__.py
+-rw-r--r--   0        0        0     2424 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/agent.py
+-rw-r--r--   0        0        0     1311 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/audio_agent.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/__init__.py
+-rw-r--r--   0        0        0     3850 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/document_manager.py
+-rw-r--r--   0        0        0     2865 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/document_processor.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/loaders/__init__.py
+-rw-r--r--   0        0        0     1059 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py
+-rw-r--r--   0        0        0     3405 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py
+-rw-r--r--   0        0        0     4642 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/parsers/__init__.py
+-rw-r--r--   0        0        0     2817 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py
+-rw-r--r--   0        0        0     4519 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/__init__.py
+-rw-r--r--   0        0        0      448 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/base_ast_generator.py
+-rw-r--r--   0        0        0     3699 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py
+-rw-r--r--   0        0        0     2053 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py
+-rw-r--r--   0        0        0     3212 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py
+-rw-r--r--   0        0        0     1647 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py
+-rw-r--r--   0        0        0     1328 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py
+-rw-r--r--   0        0        0     3356 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py
+-rw-r--r--   0        0        0     1399 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/transformer/__init__.py
+-rw-r--r--   0        0        0     1398 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py
+-rw-r--r--   0        0        0     4786 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py
+-rw-r--r--   0        0        0    43465 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py
+-rw-r--r--   0        0        0     4825 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/generic_agent.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/retriever_agent/__init__.py
+-rw-r--r--   0        0        0     2078 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py
+-rw-r--r--   0        0        0     1428 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py
+-rw-r--r--   0        0        0     2323 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py
+-rw-r--r--   0        0        0      559 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py
+-rw-r--r--   0        0        0     2864 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/retriever_agent/retriever.py
+-rw-r--r--   0        0        0     4142 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py
+-rw-r--r--   0        0        0    13376 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/simple_agent.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/tot_agent/__init__.py
+-rw-r--r--   0        0        0     1809 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/tot_agent/checker.py
+-rw-r--r--   0        0        0     2468 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/tot_agent/controller.py
+-rw-r--r--   0        0        0     1503 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/tot_agent/memory.py
+-rw-r--r--   0        0        0     1423 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/tot_agent/prompts.py
+-rw-r--r--   0        0        0      364 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/tot_agent/thought.py
+-rw-r--r--   0        0        0     4951 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/tot_agent/thought_generators.py
+-rw-r--r--   0        0        0     7614 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/tot_agent/tot_agent.py
+-rw-r--r--   0        0        0     4572 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent_os.py
+-rw-r--r--   0        0        0    12735 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent_os_interfaces.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/bin/__init__.py
+-rwxr-xr-x   0        0        0     9545 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/bin/agent_creator.py
+-rw-r--r--   0        0        0     8381 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/bin/agent_http_server.py
+-rwxr-xr-x   0        0        0     3789 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/bin/replay.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/builtins/__init__.py
+-rw-r--r--   0        0        0     9194 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/builtins/code_builtins.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/builtins/components/__init__.py
+-rw-r--r--   0        0        0     2223 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/builtins/components/opentelemetry.py
+-rw-r--r--   0        0        0     4256 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/builtins/components/usage.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/builtins/logic_units/__init__.py
+-rw-r--r--   0        0        0     1822 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/builtins/logic_units/playwrite_browser.py
+-rw-r--r--   0        0        0     6517 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/builtins/logic_units/web_search.py
+-rw-r--r--   0        0        0      550 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml
+-rw-r--r--   0        0        0      601 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/builtins/resources/claude_opus.yaml
+-rw-r--r--   0        0        0      614 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml
+-rw-r--r--   0        0        0      181 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/builtins/resources/machine.yaml
+-rw-r--r--   0        0        0      597 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/builtins/resources/mistral_large.yaml
+-rw-r--r--   0        0        0      547 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml
+-rw-r--r--   0        0        0      540 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/builtins/resources/mistral_small.yaml
+-rw-r--r--   0        0        0      595 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/builtins/resources/openai_35.yaml
+-rw-r--r--   0        0        0      586 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/builtins/resources/openai_4.yaml
+-rw-r--r--   0        0        0        0 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/__init__.py
+-rw-r--r--   0        0        0     1843 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/agent_call_history.py
+-rw-r--r--   0        0        0     3008 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/agent_io.py
+-rw-r--r--   0        0        0     9128 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/agents_logic_unit.py
+-rw-r--r--   0        0        0     6039 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/apu.py
+-rw-r--r--   0        0        0     3790 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/audio_unit.py
+-rw-r--r--   0        0        0      292 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/call_context.py
+-rw-r--r--   0        0        0     2833 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/conversation_memory_unit.py
+-rw-r--r--   0        0        0    14187 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/conversational_apu.py
+-rw-r--r--   0        0        0     4841 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/image_unit.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/llm/__init__.py
+-rw-r--r--   0        0        0     9936 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py
+-rw-r--r--   0        0        0    11967 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py
+-rw-r--r--   0        0        0     4518 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py
+-rw-r--r--   0        0        0     5753 2024-05-29 20:01:15.602897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py
+-rw-r--r--   0        0        0     9490 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py
+-rw-r--r--   0        0        0     3597 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/llm/open_ai_speech.py
+-rw-r--r--   0        0        0     3962 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/llm_message.py
+-rw-r--r--   0        0        0     3099 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/llm_unit.py
+-rw-r--r--   0        0        0     4491 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/logic_unit.py
+-rw-r--r--   0        0        0     3541 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/memory_unit.py
+-rw-r--r--   0        0        0      825 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/processing_unit.py
+-rw-r--r--   0        0        0     5205 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/tool_call_unit.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/io/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/memory/__init__.py
+-rw-r--r--   0        0        0     1193 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/memory/agent_memory.py
+-rw-r--r--   0        0        0     5309 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/memory/chroma_vector_store.py
+-rw-r--r--   0        0        0      641 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/memory/document.py
+-rw-r--r--   0        0        0     2766 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/memory/embeddings.py
+-rw-r--r--   0        0        0      907 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/memory/file_memory.py
+-rw-r--r--   0        0        0     4203 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/memory/file_system_vector_store.py
+-rw-r--r--   0        0        0     3974 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/memory/in_memory_file_memory.py
+-rw-r--r--   0        0        0     5788 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/memory/local_file_memory.py
+-rw-r--r--   0        0        0     4845 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/memory/local_symbolic_memory.py
+-rw-r--r--   0        0        0     3793 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/memory/mongo_symbolic_memory.py
+-rw-r--r--   0        0        0      996 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/memory/noop_memory.py
+-rw-r--r--   0        0        0     1984 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/memory/s3_file_memory.py
+-rw-r--r--   0        0        0      974 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/memory/semantic_memory.py
+-rw-r--r--   0        0        0     2809 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/memory/similarity_memory.py
+-rw-r--r--   0        0        0     1516 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/memory/vector_store.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/security/__init__.py
+-rw-r--r--   0        0        0      771 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/security/authentication_processor.py
+-rw-r--r--   0        0        0     2159 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/security/azure_authorizer.py
+-rw-r--r--   0        0        0     1277 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/security/functional_authorizer.py
+-rw-r--r--   0        0        0     2001 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/security/google_auth.py
+-rw-r--r--   0        0        0     1867 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/security/jwt_processor.py
+-rw-r--r--   0        0        0      484 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/security/okta_authorizor.py
+-rw-r--r--   0        0        0     1017 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/security/permissions.py
+-rw-r--r--   0        0        0     2508 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/security/process_authorizer.py
+-rw-r--r--   0        0        0     2977 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/security/security_manager.py
+-rw-r--r--   0        0        0     1035 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/security/security_middleware.py
+-rw-r--r--   0        0        0      428 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/security/user.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/system/__init__.py
+-rw-r--r--   0        0        0     1473 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/system/agent_contract.py
+-rw-r--r--   0        0        0    23004 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/system/agent_controller.py
+-rw-r--r--   0        0        0    14196 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/system/agent_machine.py
+-rw-r--r--   0        0        0     1149 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/system/dynamic_middleware.py
+-rw-r--r--   0        0        0     3432 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/system/fn_handler.py
+-rw-r--r--   0        0        0     4911 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/system/process_file_system.py
+-rw-r--r--   0        0        0     4275 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/system/processes.py
+-rw-r--r--   0        0        0     7664 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/system/reference_model.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/system/resources/__init__.py
+-rw-r--r--   0        0        0      314 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/system/resources/agent_resource.py
+-rw-r--r--   0        0        0      414 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/system/resources/machine_resource.py
+-rw-r--r--   0        0        0      684 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/system/resources/reference_resource.py
+-rw-r--r--   0        0        0     1663 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/system/resources/resources_base.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/util/__init__.py
+-rw-r--r--   0        0        0      509 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/util/async_wrapper.py
+-rw-r--r--   0        0        0     2806 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/util/class_utils.py
+-rw-r--r--   0        0        0     1604 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/util/image_utils.py
+-rw-r--r--   0        0        0     3808 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/util/replay.py
+-rw-r--r--   0        0        0     6917 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/util/schema_to_model.py
+-rw-r--r--   0        0        0      898 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/util/str_utils.py
+-rw-r--r--   0        0        0     3445 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/util/stream_collector.py
+-rw-r--r--   0        0        0      565 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/logging.conf
+-rw-r--r--   0        0        0     2214 2024-05-29 20:01:15.606897 eidolon_ai_sdk-0.1.60/pyproject.toml
+-rw-r--r--   0        0        0     2977 1970-01-01 00:00:00.000000 eidolon_ai_sdk-0.1.60/PKG-INFO
```

### Comparing `eidolon_ai_sdk-0.1.59/README.md` & `eidolon_ai_sdk-0.1.60/README.md`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/agent.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/audio_agent.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/audio_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/document_manager.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/document_manager.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/document_processor.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/document_processor.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 class BS4HTMLParserSpec(DocumentParserSpec):
     features: str = "lxml"
     text_separator: str = ""
 
 
 class BS4HTMLParser(DocumentParser, Specable[BS4HTMLParserSpec]):
-    """Pparse HTML files using `Beautiful Soup`."""
+    """Parse HTML files using `Beautiful Soup`."""
 
     def __init__(self, spec: BS4HTMLParserSpec):
         super().__init__(spec)
         self.bs_kwargs = {"features": spec.features}
         self.text_separator = spec.text_separator
 
     def parse(self, blob: DataBlob) -> Iterable[Document]:
```

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/generic_agent.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/generic_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/retriever_agent/retriever.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/retriever_agent/retriever.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/simple_agent.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/simple_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/tot_agent/checker.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/tot_agent/checker.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/tot_agent/controller.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/tot_agent/controller.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/tot_agent/memory.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/tot_agent/memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/tot_agent/prompts.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/tot_agent/prompts.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/tot_agent/thought_generators.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/tot_agent/thought_generators.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent/tot_agent/tot_agent.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent/tot_agent/tot_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent_os.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent_os.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/agent_os_interfaces.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/agent_os_interfaces.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/bin/agent_creator.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/bin/agent_creator.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/bin/agent_http_server.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/bin/agent_http_server.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/bin/replay.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/bin/replay.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/builtins/code_builtins.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/builtins/code_builtins.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/builtins/components/opentelemetry.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/builtins/components/opentelemetry.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/builtins/components/usage.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/builtins/components/usage.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/builtins/logic_units/playwrite_browser.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/builtins/logic_units/playwrite_browser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/builtins/logic_units/web_search.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/builtins/logic_units/web_search.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/builtins/resources/claude_opus.yaml` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/builtins/resources/claude_opus.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/builtins/resources/mistral_large.yaml` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/builtins/resources/mistral_large.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/builtins/resources/mistral_small.yaml` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/builtins/resources/mistral_small.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/builtins/resources/openai_35.yaml` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/builtins/resources/openai_35.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/builtins/resources/openai_4.yaml` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/builtins/resources/openai_4.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/agent_call_history.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/agent_call_history.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/agent_io.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/agent_io.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/agents_logic_unit.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/agents_logic_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/apu.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/apu.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/audio_unit.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/audio_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/conversation_memory_unit.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/conversation_memory_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/conversational_apu.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/conversational_apu.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/image_unit.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/image_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/llm/open_ai_speech.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/llm/open_ai_speech.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/llm_message.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/llm_message.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/llm_unit.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/logic_unit.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/logic_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/memory_unit.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/memory_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/processing_unit.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/processing_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/cpu/tool_call_unit.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/cpu/tool_call_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/memory/agent_memory.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/memory/agent_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/memory/chroma_vector_store.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/memory/chroma_vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/memory/document.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/memory/document.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/memory/embeddings.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/memory/embeddings.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/memory/file_memory.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/memory/file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/memory/file_system_vector_store.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/memory/file_system_vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/memory/in_memory_file_memory.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/memory/in_memory_file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/memory/local_file_memory.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/memory/local_file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/memory/local_symbolic_memory.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/memory/local_symbolic_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/memory/mongo_symbolic_memory.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/memory/mongo_symbolic_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/memory/noop_memory.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/memory/noop_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/memory/s3_file_memory.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/memory/s3_file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/memory/semantic_memory.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/memory/semantic_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/memory/similarity_memory.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/memory/similarity_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/memory/vector_store.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/memory/vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/security/authentication_processor.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/security/authentication_processor.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/security/azure_authorizer.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/security/azure_authorizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/security/functional_authorizer.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/security/functional_authorizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/security/google_auth.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/security/google_auth.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/security/jwt_processor.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/security/jwt_processor.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/security/permissions.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/security/permissions.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/security/process_authorizer.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/security/process_authorizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/security/security_manager.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/security/security_manager.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/security/security_middleware.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/security/security_middleware.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/system/agent_contract.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/system/agent_contract.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/system/agent_controller.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/system/agent_controller.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/system/agent_machine.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/system/agent_machine.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/system/dynamic_middleware.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/system/dynamic_middleware.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/system/fn_handler.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/system/fn_handler.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/system/process_file_system.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/system/process_file_system.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/system/processes.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/system/processes.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/system/reference_model.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/system/reference_model.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/system/resources/reference_resource.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/system/resources/reference_resource.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/system/resources/resources_base.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/system/resources/resources_base.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/util/class_utils.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/util/class_utils.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/util/image_utils.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/util/image_utils.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/util/replay.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/util/replay.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/util/schema_to_model.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/util/schema_to_model.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/util/str_utils.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/util/str_utils.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/eidolon_ai_sdk/util/stream_collector.py` & `eidolon_ai_sdk-0.1.60/eidolon_ai_sdk/util/stream_collector.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/logging.conf` & `eidolon_ai_sdk-0.1.60/logging.conf`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.59/pyproject.toml` & `eidolon_ai_sdk-0.1.60/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "eidolon-ai-sdk"
-version = "0.1.59"
+version = "0.1.60"
 description = "An open source sgent service SDK"
 authors = [ "Luke Lalor <lukehlalor@gmail.com>",]
 readme = "README.md"
 include = [ "logging.conf",]
 
 [tool.ruff]
 line-length = 121
 
 [tool.eidolon]
 update-tag = "sdk"
-last-update-hash = "3a1c2f12d1963d237011599bdaf89872a20143e2"
+last-update-hash = "797c4a27b335a5ace652ab83116c5750e7893c4b"
 
 [tool.poetry.urls]
 Github = "https://github.com/eidolon-ai/eidolon"
 Website = "https://www.eidolonai.com/"
 
 [tool.poetry.scripts]
 eidolon-server = "eidolon_ai_sdk.bin.agent_http_server:main"
```

### Comparing `eidolon_ai_sdk-0.1.59/PKG-INFO` & `eidolon_ai_sdk-0.1.60/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eidolon-ai-sdk
-Version: 0.1.59
+Version: 0.1.60
 Summary: An open source sgent service SDK
 Author: Luke Lalor
 Author-email: lukehlalor@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: anthropic (>=0.21.3,<0.22.0)
```

