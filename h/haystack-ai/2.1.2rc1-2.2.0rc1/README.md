# Comparing `tmp/haystack_ai-2.1.2rc1.tar.gz` & `tmp/haystack_ai-2.2.0rc1.tar.gz`

## Comparing `haystack_ai-2.1.2rc1.tar` & `haystack_ai-2.2.0rc1.tar`

### file list

```diff
@@ -1,188 +1,192 @@
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/VERSION.txt
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/__init__.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/errors.py
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/lazy_imports.py
--rw-r--r--   0        0        0    13429 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/logging.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/__init__.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/audio/__init__.py
--rw-r--r--   0        0        0     7423 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/audio/whisper_local.py
--rw-r--r--   0        0        0     5899 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/audio/whisper_remote.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/builders/__init__.py
--rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/builders/answer_builder.py
--rw-r--r--   0        0        0     9405 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/builders/dynamic_chat_prompt_builder.py
--rw-r--r--   0        0        0     7130 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/builders/dynamic_prompt_builder.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/builders/prompt_builder.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/caching/__init__.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/caching/cache_checker.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/classifiers/__init__.py
--rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/classifiers/document_language_classifier.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/connectors/__init__.py
--rw-r--r--   0        0        0    13841 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/connectors/openapi_service.py
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/converters/__init__.py
--rw-r--r--   0        0        0    24642 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/converters/azure.py
--rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/converters/html.py
--rw-r--r--   0        0        0     3851 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/converters/markdown.py
--rw-r--r--   0        0        0    11313 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/converters/openapi_functions.py
--rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/converters/output_adapter.py
--rw-r--r--   0        0        0     6591 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/converters/pdfminer.py
--rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/converters/pypdf.py
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/converters/tika.py
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/converters/txt.py
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/converters/utils.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/embedders/__init__.py
--rw-r--r--   0        0        0     9251 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/embedders/azure_document_embedder.py
--rw-r--r--   0        0        0     6894 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/embedders/azure_text_embedder.py
--rw-r--r--   0        0        0    10902 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/embedders/hugging_face_api_document_embedder.py
--rw-r--r--   0        0        0     8005 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/embedders/hugging_face_api_text_embedder.py
--rw-r--r--   0        0        0     8671 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/embedders/hugging_face_tei_document_embedder.py
--rw-r--r--   0        0        0     6073 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/embedders/hugging_face_tei_text_embedder.py
--rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/embedders/openai_document_embedder.py
--rw-r--r--   0        0        0     4734 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/embedders/openai_text_embedder.py
--rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/embedders/sentence_transformers_document_embedder.py
--rw-r--r--   0        0        0     5655 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/embedders/sentence_transformers_text_embedder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/embedders/backends/__init__.py
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/embedders/backends/sentence_transformers_backend.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/evaluators/__init__.py
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/evaluators/answer_exact_match.py
--rw-r--r--   0        0        0     6562 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/evaluators/context_relevance.py
--rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/evaluators/document_map.py
--rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/evaluators/document_mrr.py
--rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/evaluators/document_recall.py
--rw-r--r--   0        0        0     7561 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/evaluators/faithfulness.py
--rw-r--r--   0        0        0    12141 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/evaluators/llm_evaluator.py
--rw-r--r--   0        0        0     8078 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/evaluators/sas_evaluator.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/extractors/__init__.py
--rw-r--r--   0        0        0    16393 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/extractors/named_entity_extractor.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/fetchers/__init__.py
--rw-r--r--   0        0        0     9385 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/fetchers/link_content.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/generators/__init__.py
--rw-r--r--   0        0        0     9100 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/generators/azure.py
--rw-r--r--   0        0        0     9912 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/generators/hugging_face_api.py
--rw-r--r--   0        0        0    11239 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/generators/hugging_face_local.py
--rw-r--r--   0        0        0    13263 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/generators/hugging_face_tgi.py
--rw-r--r--   0        0        0    13449 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/generators/openai.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/generators/utils.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/generators/chat/__init__.py
--rw-r--r--   0        0        0     9813 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/generators/chat/azure.py
--rw-r--r--   0        0        0    11191 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/generators/chat/hugging_face_api.py
--rw-r--r--   0        0        0    17793 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/generators/chat/hugging_face_local.py
--rw-r--r--   0        0        0    15851 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/generators/chat/hugging_face_tgi.py
--rw-r--r--   0        0        0    16934 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/generators/chat/openai.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/joiners/__init__.py
--rw-r--r--   0        0        0     6614 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/joiners/document_joiner.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/others/__init__.py
--rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/others/multiplexer.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/preprocessors/__init__.py
--rw-r--r--   0        0        0    10218 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/preprocessors/document_cleaner.py
--rw-r--r--   0        0        0     5913 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/preprocessors/document_splitter.py
--rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/preprocessors/text_cleaner.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/rankers/__init__.py
--rw-r--r--   0        0        0     6102 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/rankers/lost_in_the_middle.py
--rw-r--r--   0        0        0    17048 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/rankers/meta_field.py
--rw-r--r--   0        0        0    10902 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/rankers/sentence_transformers_diversity.py
--rw-r--r--   0        0        0    11598 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/rankers/transformers_similarity.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/readers/__init__.py
--rw-r--r--   0        0        0    28699 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/readers/extractive.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/retrievers/__init__.py
--rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/retrievers/filter_retriever.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/retrievers/in_memory/__init__.py
--rw-r--r--   0        0        0     4928 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/retrievers/in_memory/bm25_retriever.py
--rw-r--r--   0        0        0     6106 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/retrievers/in_memory/embedding_retriever.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/routers/__init__.py
--rw-r--r--   0        0        0    10151 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/routers/conditional_router.py
--rw-r--r--   0        0        0     5841 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/routers/file_type_router.py
--rw-r--r--   0        0        0     4222 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/routers/metadata_router.py
--rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/routers/text_language_router.py
--rw-r--r--   0        0        0     9560 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/routers/zero_shot_text_router.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/samplers/__init__.py
--rw-r--r--   0        0        0     6053 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/samplers/top_p.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/validators/__init__.py
--rw-r--r--   0        0        0    10328 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/validators/json_schema.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/websearch/__init__.py
--rw-r--r--   0        0        0     6782 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/websearch/searchapi.py
--rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/websearch/serper_dev.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/writers/__init__.py
--rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/components/writers/document_writer.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/core/__init__.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/core/errors.py
--rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/core/serialization.py
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/core/type_utils.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/core/component/__init__.py
--rw-r--r--   0        0        0    18608 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/core/component/component.py
--rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/core/component/sockets.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/core/component/types.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/core/pipeline/__init__.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/core/pipeline/descriptions.py
--rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/core/pipeline/draw.py
--rw-r--r--   0        0        0    57180 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/core/pipeline/pipeline.py
--rw-r--r--   0        0        0     5518 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/core/pipeline/template.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/core/pipeline/predefined/chat_with_website.yaml.jinja2
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/core/pipeline/predefined/generative_qa.yaml.jinja2
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/core/pipeline/predefined/indexing.yaml.jinja2
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/core/pipeline/predefined/rag.yaml.jinja2
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/dataclasses/__init__.py
--rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/dataclasses/answer.py
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/dataclasses/byte_stream.py
--rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/dataclasses/chat_message.py
--rw-r--r--   0        0        0     8389 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/dataclasses/document.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/dataclasses/sparse_embedding.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/dataclasses/streaming_chunk.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/document_stores/__init__.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/document_stores/errors/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/document_stores/errors/errors.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/document_stores/in_memory/__init__.py
--rw-r--r--   0        0        0    15577 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/document_stores/in_memory/document_store.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/document_stores/types/__init__.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/document_stores/types/policy.py
--rw-r--r--   0        0        0     4777 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/document_stores/types/protocol.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/evaluation/__init__.py
--rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/evaluation/eval_run_result.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/marshal/__init__.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/marshal/protocol.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/marshal/yaml.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/telemetry/__init__.py
--rw-r--r--   0        0        0     3762 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/telemetry/_environment.py
--rw-r--r--   0        0        0     7384 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/telemetry/_telemetry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/__init__.py
--rw-r--r--   0        0        0    63152 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/document_store.py
--rw-r--r--   0        0        0     8049 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/factory.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/test_utils.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/sample_components/__init__.py
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/sample_components/accumulate.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/sample_components/add_value.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/sample_components/concatenate.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/sample_components/double.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/sample_components/fstring.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/sample_components/greet.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/sample_components/hello.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/sample_components/joiner.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/sample_components/parity.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/sample_components/remainder.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/sample_components/repeat.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/sample_components/self_loop.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/sample_components/subtract.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/sample_components/sum.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/sample_components/text_splitter.py
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/testing/sample_components/threshold.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/tracing/__init__.py
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/tracing/datadog.py
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/tracing/opentelemetry.py
--rw-r--r--   0        0        0     7683 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/tracing/tracer.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/tracing/utils.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/utils/__init__.py
--rw-r--r--   0        0        0     6599 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/utils/auth.py
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/utils/callable_serialization.py
--rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/utils/device.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/utils/expit.py
--rw-r--r--   0        0        0    11735 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/utils/filters.py
--rw-r--r--   0        0        0    15510 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/utils/hf.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/utils/jupyter.py
--rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/utils/requests_utils.py
--rw-r--r--   0        0        0     4849 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/utils/type_serialization.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/haystack/utils/url_validation.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/.gitignore
--rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/LICENSE
--rw-r--r--   0        0        0    11365 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/README.md
--rw-r--r--   0        0        0    10033 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/pyproject.toml
--rw-r--r--   0        0        0    13263 2020-02-02 00:00:00.000000 haystack_ai-2.1.2rc1/PKG-INFO
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/VERSION.txt
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/__init__.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/errors.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/lazy_imports.py
+-rw-r--r--   0        0        0    13540 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/logging.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/version.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/__init__.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/audio/__init__.py
+-rw-r--r--   0        0        0     7568 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/audio/whisper_local.py
+-rw-r--r--   0        0        0     6010 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/audio/whisper_remote.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/builders/__init__.py
+-rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/builders/answer_builder.py
+-rw-r--r--   0        0        0    11033 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/builders/chat_prompt_builder.py
+-rw-r--r--   0        0        0     9739 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/builders/dynamic_chat_prompt_builder.py
+-rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/builders/dynamic_prompt_builder.py
+-rw-r--r--   0        0        0     9940 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/builders/prompt_builder.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/caching/__init__.py
+-rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/caching/cache_checker.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/classifiers/__init__.py
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/classifiers/document_language_classifier.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/connectors/__init__.py
+-rw-r--r--   0        0        0    13952 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/connectors/openapi_service.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/converters/__init__.py
+-rw-r--r--   0        0        0    24753 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/converters/azure.py
+-rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/converters/html.py
+-rw-r--r--   0        0        0     3962 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/converters/markdown.py
+-rw-r--r--   0        0        0    11424 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/converters/openapi_functions.py
+-rw-r--r--   0        0        0     5625 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/converters/output_adapter.py
+-rw-r--r--   0        0        0     6703 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/converters/pdfminer.py
+-rw-r--r--   0        0        0     6739 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/converters/pypdf.py
+-rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/converters/tika.py
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/converters/txt.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/converters/utils.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/embedders/__init__.py
+-rw-r--r--   0        0        0     9362 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/embedders/azure_document_embedder.py
+-rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/embedders/azure_text_embedder.py
+-rw-r--r--   0        0        0    11013 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/embedders/hugging_face_api_document_embedder.py
+-rw-r--r--   0        0        0     8116 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/embedders/hugging_face_api_text_embedder.py
+-rw-r--r--   0        0        0     8782 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/embedders/hugging_face_tei_document_embedder.py
+-rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/embedders/hugging_face_tei_text_embedder.py
+-rw-r--r--   0        0        0     8587 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/embedders/openai_document_embedder.py
+-rw-r--r--   0        0        0     5889 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/embedders/openai_text_embedder.py
+-rw-r--r--   0        0        0     7107 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/embedders/sentence_transformers_document_embedder.py
+-rw-r--r--   0        0        0     5766 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/embedders/sentence_transformers_text_embedder.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/embedders/backends/__init__.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/embedders/backends/sentence_transformers_backend.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/evaluators/__init__.py
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/evaluators/answer_exact_match.py
+-rw-r--r--   0        0        0     7202 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/evaluators/context_relevance.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/evaluators/document_map.py
+-rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/evaluators/document_mrr.py
+-rw-r--r--   0        0        0     4937 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/evaluators/document_recall.py
+-rw-r--r--   0        0        0     8201 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/evaluators/faithfulness.py
+-rw-r--r--   0        0        0    14488 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/evaluators/llm_evaluator.py
+-rw-r--r--   0        0        0     8244 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/evaluators/sas_evaluator.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/extractors/__init__.py
+-rw-r--r--   0        0        0    16470 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/extractors/named_entity_extractor.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/fetchers/__init__.py
+-rw-r--r--   0        0        0     9573 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/fetchers/link_content.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/generators/__init__.py
+-rw-r--r--   0        0        0     9435 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/generators/azure.py
+-rw-r--r--   0        0        0    10023 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/generators/hugging_face_api.py
+-rw-r--r--   0        0        0    11720 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/generators/hugging_face_local.py
+-rw-r--r--   0        0        0    13515 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/generators/hugging_face_tgi.py
+-rw-r--r--   0        0        0    14480 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/generators/openai.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/generators/utils.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/generators/chat/__init__.py
+-rw-r--r--   0        0        0    10030 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/generators/chat/azure.py
+-rw-r--r--   0        0        0    11302 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/generators/chat/hugging_face_api.py
+-rw-r--r--   0        0        0    17938 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/generators/chat/hugging_face_local.py
+-rw-r--r--   0        0        0    16274 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/generators/chat/hugging_face_tgi.py
+-rw-r--r--   0        0        0    17962 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/generators/chat/openai.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/joiners/__init__.py
+-rw-r--r--   0        0        0     6566 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/joiners/branch.py
+-rw-r--r--   0        0        0     6954 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/joiners/document_joiner.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/others/__init__.py
+-rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/others/multiplexer.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/preprocessors/__init__.py
+-rw-r--r--   0        0        0    10489 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/preprocessors/document_cleaner.py
+-rw-r--r--   0        0        0     6845 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/preprocessors/document_splitter.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/preprocessors/text_cleaner.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/rankers/__init__.py
+-rw-r--r--   0        0        0     6213 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/rankers/lost_in_the_middle.py
+-rw-r--r--   0        0        0    17159 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/rankers/meta_field.py
+-rw-r--r--   0        0        0    11066 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/rankers/sentence_transformers_diversity.py
+-rw-r--r--   0        0        0    11691 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/rankers/transformers_similarity.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/readers/__init__.py
+-rw-r--r--   0        0        0    28999 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/readers/extractive.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/retrievers/__init__.py
+-rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/retrievers/filter_retriever.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/retrievers/in_memory/__init__.py
+-rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/retrievers/in_memory/bm25_retriever.py
+-rw-r--r--   0        0        0     6217 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/retrievers/in_memory/embedding_retriever.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/routers/__init__.py
+-rw-r--r--   0        0        0    10262 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/routers/conditional_router.py
+-rw-r--r--   0        0        0     5931 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/routers/file_type_router.py
+-rw-r--r--   0        0        0     4333 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/routers/metadata_router.py
+-rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/routers/text_language_router.py
+-rw-r--r--   0        0        0     9671 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/routers/zero_shot_text_router.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/samplers/__init__.py
+-rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/samplers/top_p.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/validators/__init__.py
+-rw-r--r--   0        0        0    10439 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/validators/json_schema.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/websearch/__init__.py
+-rw-r--r--   0        0        0     6893 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/websearch/searchapi.py
+-rw-r--r--   0        0        0     6861 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/websearch/serper_dev.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/writers/__init__.py
+-rw-r--r--   0        0        0     4595 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/components/writers/document_writer.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/__init__.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/errors.py
+-rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/serialization.py
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/type_utils.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/component/__init__.py
+-rw-r--r--   0        0        0    18609 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/component/component.py
+-rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/component/sockets.py
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/component/types.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/pipeline/__init__.py
+-rw-r--r--   0        0        0    36291 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/pipeline/base.py
+-rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/pipeline/descriptions.py
+-rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/pipeline/draw.py
+-rw-r--r--   0        0        0    21292 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/pipeline/pipeline.py
+-rw-r--r--   0        0        0     5629 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/pipeline/template.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/pipeline/utils.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/pipeline/predefined/chat_with_website.yaml.jinja2
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/pipeline/predefined/generative_qa.yaml.jinja2
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/pipeline/predefined/indexing.yaml.jinja2
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/core/pipeline/predefined/rag.yaml.jinja2
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/dataclasses/__init__.py
+-rw-r--r--   0        0        0     6074 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/dataclasses/answer.py
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/dataclasses/byte_stream.py
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/dataclasses/chat_message.py
+-rw-r--r--   0        0        0     8500 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/dataclasses/document.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/dataclasses/sparse_embedding.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/dataclasses/streaming_chunk.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/document_stores/__init__.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/document_stores/errors/__init__.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/document_stores/errors/errors.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/document_stores/in_memory/__init__.py
+-rw-r--r--   0        0        0    23733 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/document_stores/in_memory/document_store.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/document_stores/types/__init__.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/document_stores/types/policy.py
+-rw-r--r--   0        0        0     4888 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/document_stores/types/protocol.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/evaluation/__init__.py
+-rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/evaluation/eval_run_result.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/marshal/__init__.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/marshal/protocol.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/marshal/yaml.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/telemetry/__init__.py
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/telemetry/_environment.py
+-rw-r--r--   0        0        0     7495 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/telemetry/_telemetry.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/__init__.py
+-rw-r--r--   0        0        0    63265 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/document_store.py
+-rw-r--r--   0        0        0     8160 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/factory.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/test_utils.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/sample_components/__init__.py
+-rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/sample_components/accumulate.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/sample_components/add_value.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/sample_components/concatenate.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/sample_components/double.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/sample_components/fstring.py
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/sample_components/greet.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/sample_components/hello.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/sample_components/joiner.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/sample_components/parity.py
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/sample_components/remainder.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/sample_components/repeat.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/sample_components/self_loop.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/sample_components/subtract.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/sample_components/sum.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/sample_components/text_splitter.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/testing/sample_components/threshold.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/tracing/__init__.py
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/tracing/datadog.py
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/tracing/opentelemetry.py
+-rw-r--r--   0        0        0     7794 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/tracing/tracer.py
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/tracing/utils.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/utils/__init__.py
+-rw-r--r--   0        0        0     6710 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/utils/auth.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/utils/callable_serialization.py
+-rw-r--r--   0        0        0    15539 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/utils/device.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/utils/expit.py
+-rw-r--r--   0        0        0    11846 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/utils/filters.py
+-rw-r--r--   0        0        0    15621 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/utils/hf.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/utils/jupyter.py
+-rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/utils/requests_utils.py
+-rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/utils/type_serialization.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/haystack/utils/url_validation.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/.gitignore
+-rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/LICENSE
+-rw-r--r--   0        0        0    11365 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/README.md
+-rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/pyproject.toml
+-rw-r--r--   0        0        0    13236 2020-02-02 00:00:00.000000 haystack_ai-2.2.0rc1/PKG-INFO
```

### Comparing `haystack_ai-2.1.2rc1/haystack/__init__.py` & `haystack_ai-2.2.0rc1/haystack/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import haystack.logging
 from haystack.core.component import component
 from haystack.core.errors import ComponentError, DeserializationError
 from haystack.core.pipeline import Pipeline, PredefinedPipeline
 from haystack.core.serialization import default_from_dict, default_to_dict
 from haystack.dataclasses import Answer, Document, ExtractedAnswer, GeneratedAnswer
```

### Comparing `haystack_ai-2.1.2rc1/haystack/lazy_imports.py` & `haystack_ai-2.2.0rc1/haystack/lazy_imports.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from types import TracebackType
 from typing import Optional, Type
 
 from lazy_imports.try_import import _DeferredImportExceptionContextManager
 
 DEFAULT_IMPORT_ERROR_MSG = "Try 'pip install {}'"
```

### Comparing `haystack_ai-2.1.2rc1/haystack/logging.py` & `haystack_ai-2.2.0rc1/haystack/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import builtins
 import functools
 import logging
 import os
 import sys
 import typing
 from typing import Any, List, Optional
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/audio/whisper_local.py` & `haystack_ai-2.2.0rc1/haystack/components/audio/whisper_local.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import tempfile
 from pathlib import Path
 from typing import Any, Dict, List, Literal, Optional, Union, get_args
 
-from haystack import ComponentError, Document, component, default_from_dict, default_to_dict, logging
+from haystack import Document, component, default_from_dict, default_to_dict, logging
 from haystack.dataclasses import ByteStream
 from haystack.lazy_imports import LazyImport
 from haystack.utils import ComponentDevice
 
 with LazyImport("Run 'pip install \"openai-whisper>=20231106\"' to install whisper.") as whisper_import:
     import whisper
 
@@ -105,15 +109,17 @@
 
         :returns: A dictionary with the following keys:
             - `documents`: A list of Documents, one for each file. The content of the document is the transcription text,
                 while the document's metadata contains the values returned by the Whisper model, such as the
                 alignment data and the path to the audio file used for the transcription.
         """
         if self._model is None:
-            raise ComponentError("The component was not warmed up. Run 'warm_up()' before calling 'run()'.")
+            raise RuntimeError(
+                "The component LocalWhisperTranscriber was not warmed up. Run 'warm_up()' before calling 'run()'."
+            )
 
         if whisper_params is None:
             whisper_params = self.whisper_params
 
         documents = self.transcribe(sources, **whisper_params)
         return {"documents": documents}
 
@@ -148,15 +154,15 @@
 
         :param audio_files:
             A list of paths or binary streams to transcribe.
         :returns:
             A dictionary mapping 'file_path' to 'transcription'.
         """
         if self._model is None:
-            raise ComponentError("Model is not loaded, please run 'warm_up()' before calling 'run()'")
+            raise RuntimeError("Model is not loaded, please run 'warm_up()' before calling 'run()'")
 
         return_segments = kwargs.pop("return_segments", False)
         transcriptions: Dict[Path, Any] = {}
         for source in sources:
             if not isinstance(source, ByteStream):
                 path = Path(source)
                 source = ByteStream.from_file_path(path)
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/audio/whisper_remote.py` & `haystack_ai-2.2.0rc1/haystack/components/audio/whisper_remote.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import io
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 
 from openai import OpenAI
 
 from haystack import Document, component, default_from_dict, default_to_dict, logging
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/builders/answer_builder.py` & `haystack_ai-2.2.0rc1/haystack/components/builders/answer_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import re
 from typing import Any, Dict, List, Optional
 
 from haystack import Document, GeneratedAnswer, component, logging
 
 logger = logging.getLogger(__name__)
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/builders/dynamic_chat_prompt_builder.py` & `haystack_ai-2.2.0rc1/haystack/components/builders/dynamic_chat_prompt_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
+import warnings
 from typing import Any, Dict, List, Optional, Set
 
 from jinja2 import Template, meta
 
 from haystack import component, logging
 from haystack.dataclasses.chat_message import ChatMessage, ChatRole
 
@@ -76,14 +81,19 @@
         :param runtime_variables:
             A list of template variable names you can use in chat prompt construction. For example,
             if `runtime_variables` contains the string `documents`, the component will create an input called
             `documents` of type `Any`. These variable names are used to resolve variables and their values during
             pipeline execution. The values associated with variables from the pipeline runtime are then injected into
             template placeholders of a ChatMessage that is provided to the `run` method.
         """
+        warnings.warn(
+            "`DynamicChatPromptBuilder` is deprecated and will be removed in Haystack 2.4.0."
+            "Use `ChatPromptBuilder` instead.",
+            DeprecationWarning,
+        )
         runtime_variables = runtime_variables or []
 
         # setup inputs
         default_inputs = {"prompt_source": List[ChatMessage], "template_variables": Optional[Dict[str, Any]]}
         additional_input_slots = {var: Optional[Any] for var in runtime_variables}
         component.set_input_types(self, **default_inputs, **additional_input_slots)
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/builders/dynamic_prompt_builder.py` & `haystack_ai-2.2.0rc1/haystack/components/builders/dynamic_prompt_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
+import warnings
 from typing import Any, Dict, List, Optional, Set
 
 from jinja2 import Template, meta
 
 from haystack import component, logging
 
 logger = logging.getLogger(__name__)
@@ -76,14 +81,20 @@
         :param runtime_variables:
             A list of template variable names you can use in prompt construction. For example,
             if `runtime_variables` contains the string `documents`, the component will create an input called
             `documents` of type `Any`. These variable names are used to resolve variables and their values during
             pipeline execution. The values associated with variables from the pipeline runtime are then injected into
             template placeholders of a prompt text template that is provided to the `run` method.
         """
+        warnings.warn(
+            "`DynamicPromptBuilder` is deprecated and will be removed in Haystack 2.4.0."
+            "Use `PromptBuilder` instead.",
+            DeprecationWarning,
+        )
+
         runtime_variables = runtime_variables or []
 
         # setup inputs
         run_input_slots = {"prompt_source": str, "template_variables": Optional[Dict[str, Any]]}
         kwargs_input_slots = {var: Optional[Any] for var in runtime_variables}
         component.set_input_types(self, **run_input_slots, **kwargs_input_slots)
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/caching/cache_checker.py` & `haystack_ai-2.2.0rc1/haystack/components/caching/cache_checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import importlib
 from typing import Any, Dict, List
 
 from haystack import DeserializationError, Document, component, default_from_dict, default_to_dict, logging
 from haystack.document_stores.types import DocumentStore
 
 logger = logging.getLogger(__name__)
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/classifiers/document_language_classifier.py` & `haystack_ai-2.2.0rc1/haystack/components/classifiers/document_language_classifier.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from typing import Dict, List, Optional
 
 from haystack import Document, component, logging
 from haystack.lazy_imports import LazyImport
 
 logger = logging.getLogger(__name__)
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/connectors/openapi_service.py` & `haystack_ai-2.2.0rc1/haystack/components/connectors/openapi_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import json
 from collections import defaultdict
 from copy import copy
 from typing import Any, Dict, List, Optional, Union
 
 from haystack import component, logging
 from haystack.dataclasses import ChatMessage, ChatRole
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/converters/azure.py` & `haystack_ai-2.2.0rc1/haystack/components/converters/azure.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import copy
 import hashlib
 from collections import defaultdict
 from pathlib import Path
 from typing import Any, Dict, List, Literal, Optional, Union
 
 import networkx as nx
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/converters/html.py` & `haystack_ai-2.2.0rc1/haystack/components/converters/html.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,16 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
+import warnings
 from pathlib import Path
-from typing import Any, ClassVar, Dict, List, Literal, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
-from boilerpy3 import extractors
+from trafilatura import extract
 
 from haystack import Document, component, default_from_dict, default_to_dict, logging
 from haystack.components.converters.utils import get_bytestream_from_source, normalize_metadata
 from haystack.dataclasses import ByteStream
 
 logger = logging.getLogger(__name__)
 
@@ -23,57 +28,52 @@
     results = converter.run(sources=["path/to/sample.html"])
     documents = results["documents"]
     print(documents[0].content)
     # 'This is a text from the HTML file.'
     ```
     """
 
-    known_extractors: ClassVar[List[str]] = [
-        "DefaultExtractor",
-        "ArticleExtractor",
-        "ArticleSentencesExtractor",
-        "LargestContentExtractor",
-        "CanolaExtractor",
-        "KeepEverythingExtractor",
-        "NumWordsRulesExtractor",
-    ]
-
     def __init__(
         self,
-        extractor_type: Literal[
-            "DefaultExtractor",
-            "ArticleExtractor",
-            "ArticleSentencesExtractor",
-            "LargestContentExtractor",
-            "CanolaExtractor",
-            "KeepEverythingExtractor",
-            "NumWordsRulesExtractor",
-        ] = "DefaultExtractor",
-        try_others: bool = True,
+        extractor_type: Optional[str] = None,
+        try_others: Optional[bool] = None,
+        extraction_kwargs: Optional[Dict[str, Any]] = None,
     ):
         """
         Create an HTMLToDocument component.
 
-        :param
-            extractor_type: Name of the extractor class to use. Defaults to `DefaultExtractor`.
-            For more information on the different types of extractors,
-            see [boilerpy3 documentation](https://github.com/jmriebold/BoilerPy3?tab=readme-ov-file#extractors).
-        :param try_others: If `True`, the component will try other extractors if the user chosen extractor fails.
-        """
-        self.extractor_type = extractor_type
-        self.try_others = try_others
+        :param extractor_type: Ignored. This parameter is kept for compatibility with previous versions. It will be
+            removed in Haystack 2.4.0. To customize the extraction, use the `extraction_kwargs` parameter.
+        :param try_others: Ignored. This parameter is kept for compatibility with previous versions. It will be
+            removed in Haystack 2.4.0.
+        :param extraction_kwargs: A dictionary containing keyword arguments to customize the extraction process. These
+            are passed to the underlying Trafilatura `extract` function. For the full list of available arguments, see
+            the [Trafilatura documentation](https://trafilatura.readthedocs.io/en/latest/corefunctions.html#extract).
+        """
+        if extractor_type is not None:
+            warnings.warn(
+                "The `extractor_type` parameter is ignored and will be removed in Haystack 2.4.0. "
+                "To customize the extraction, use the `extraction_kwargs` parameter.",
+                DeprecationWarning,
+            )
+        if try_others is not None:
+            warnings.warn(
+                "The `try_others` parameter is ignored and will be removed in Haystack 2.4.0. ", DeprecationWarning
+            )
+
+        self.extraction_kwargs = extraction_kwargs or {}
 
     def to_dict(self) -> Dict[str, Any]:
         """
         Serializes the component to a dictionary.
 
         :returns:
             Dictionary with serialized data.
         """
-        return default_to_dict(self, extractor_type=self.extractor_type, try_others=self.try_others)
+        return default_to_dict(self, extraction_kwargs=self.extraction_kwargs)
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> "HTMLToDocument":
         """
         Deserializes the component from a dictionary.
 
         :param data:
@@ -84,74 +84,54 @@
         return default_from_dict(cls, data)
 
     @component.output_types(documents=List[Document])
     def run(
         self,
         sources: List[Union[str, Path, ByteStream]],
         meta: Optional[Union[Dict[str, Any], List[Dict[str, Any]]]] = None,
+        extraction_kwargs: Optional[Dict[str, Any]] = None,
     ):
         """
         Converts a list of HTML files to Documents.
 
         :param sources:
             List of HTML file paths or ByteStream objects.
         :param meta:
             Optional metadata to attach to the Documents.
             This value can be either a list of dictionaries or a single dictionary.
             If it's a single dictionary, its content is added to the metadata of all produced Documents.
             If it's a list, the length of the list must match the number of sources, because the two lists will be zipped.
             If `sources` contains ByteStream objects, their `meta` will be added to the output Documents.
+        :param extraction_kwargs:
+            Additional keyword arguments to customize the extraction process.
 
         :returns:
             A dictionary with the following keys:
             - `documents`: Created Documents
         """
 
+        merged_extraction_kwargs = {**self.extraction_kwargs, **(extraction_kwargs or {})}
+
         documents = []
         meta_list = normalize_metadata(meta=meta, sources_count=len(sources))
 
-        # Use all extractor types, ensuring user chosen extractor is first, preserve order, avoid duplicates
-        extractors_list = (
-            list(
-                dict.fromkeys(
-                    [self.extractor_type, *self.known_extractors]  # User chosen extractor is always tried first
-                )
-            )
-            if self.try_others
-            else [self.extractor_type]
-        )
-
         for source, metadata in zip(sources, meta_list):
             try:
                 bytestream = get_bytestream_from_source(source=source)
             except Exception as e:
                 logger.warning("Could not read {source}. Skipping it. Error: {error}", source=source, error=e)
                 continue
 
-            text = None
-            for extractor_name in extractors_list:
-                extractor_class = getattr(extractors, extractor_name)
-                extractor = extractor_class(raise_on_failure=False)
-                try:
-                    text = extractor.get_content(bytestream.data.decode("utf-8"))
-                    if text:
-                        break
-                except Exception as conversion_e:
-                    if self.try_others:
-                        logger.warning(
-                            "Failed to extract text using {extractor} from {source}. Trying next extractor. Error: {error}",
-                            extractor=extractor_name,
-                            source=source,
-                            error=conversion_e,
-                        )
-            if not text:
+            try:
+                text = extract(bytestream.data.decode("utf-8"), **merged_extraction_kwargs)
+            except Exception as conversion_e:
                 logger.warning(
-                    f"Failed to extract text from {source} using extractors: {extractors_list}. Skipping it.",
+                    "Failed to extract text from {source}. Skipping it. Error: {error}",
                     source=source,
-                    extractors_list=extractors_list,
+                    error=conversion_e,
                 )
                 continue
 
             document = Document(content=text, meta={**bytestream.meta, **metadata})
             documents.append(document)
 
         return {"documents": documents}
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/converters/markdown.py` & `haystack_ai-2.2.0rc1/haystack/components/converters/markdown.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 
 from tqdm import tqdm
 
 from haystack import Document, component, logging
 from haystack.components.converters.utils import get_bytestream_from_source, normalize_metadata
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/converters/openapi_functions.py` & `haystack_ai-2.2.0rc1/haystack/components/converters/openapi_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import json
 import os
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 
 import yaml
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/converters/output_adapter.py` & `haystack_ai-2.2.0rc1/haystack/components/converters/output_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from typing import Any, Callable, Dict, Optional, Set
 
 import jinja2.runtime
 from jinja2 import TemplateSyntaxError, meta
 from jinja2.nativetypes import NativeEnvironment
 from typing_extensions import TypeAlias
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/converters/pdfminer.py` & `haystack_ai-2.2.0rc1/haystack/components/converters/pdfminer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import io
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 
 from haystack import Document, component, logging
 from haystack.components.converters.utils import get_bytestream_from_source, normalize_metadata
 from haystack.dataclasses import ByteStream
@@ -108,15 +112,15 @@
             pages.append(text)
 
         # Add a page delimiter
         concat = "\f".join(pages)
 
         return Document(content=concat)
 
-    @component.output_types(document=List[Document])
+    @component.output_types(documents=List[Document])
     def run(
         self,
         sources: List[Union[str, Path, ByteStream]],
         meta: Optional[Union[Dict[str, Any], List[Dict[str, Any]]]] = None,
     ):
         """
         Converts PDF files to Documents.
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/converters/pypdf.py` & `haystack_ai-2.2.0rc1/haystack/components/converters/pypdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import io
 import warnings
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Protocol, Union
 
 from haystack import Document, component, default_from_dict, default_to_dict, logging
 from haystack.components.converters.utils import get_bytestream_from_source, normalize_metadata
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/converters/tika.py` & `haystack_ai-2.2.0rc1/haystack/components/converters/tika.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import io
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 
 from haystack import Document, component, logging
 from haystack.components.converters.utils import get_bytestream_from_source, normalize_metadata
 from haystack.dataclasses import ByteStream
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/converters/txt.py` & `haystack_ai-2.2.0rc1/haystack/components/converters/txt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 
 from haystack import Document, component, logging
 from haystack.components.converters.utils import get_bytestream_from_source, normalize_metadata
 from haystack.dataclasses import ByteStream
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/embedders/__init__.py` & `haystack_ai-2.2.0rc1/haystack/components/embedders/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from haystack.components.embedders.azure_document_embedder import AzureOpenAIDocumentEmbedder
 from haystack.components.embedders.azure_text_embedder import AzureOpenAITextEmbedder
 from haystack.components.embedders.hugging_face_api_document_embedder import HuggingFaceAPIDocumentEmbedder
 from haystack.components.embedders.hugging_face_api_text_embedder import HuggingFaceAPITextEmbedder
 from haystack.components.embedders.hugging_face_tei_document_embedder import HuggingFaceTEIDocumentEmbedder
 from haystack.components.embedders.hugging_face_tei_text_embedder import HuggingFaceTEITextEmbedder
 from haystack.components.embedders.openai_document_embedder import OpenAIDocumentEmbedder
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/embedders/azure_document_embedder.py` & `haystack_ai-2.2.0rc1/haystack/components/embedders/azure_document_embedder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import os
 from typing import Any, Dict, List, Optional, Tuple
 
 from openai.lib.azure import AzureOpenAI
 from tqdm import tqdm
 
 from haystack import Document, component, default_from_dict, default_to_dict
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/embedders/azure_text_embedder.py` & `haystack_ai-2.2.0rc1/haystack/components/embedders/azure_text_embedder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import os
 from typing import Any, Dict, List, Optional
 
 from openai.lib.azure import AzureOpenAI
 
 from haystack import Document, component, default_from_dict, default_to_dict
 from haystack.utils import Secret, deserialize_secrets_inplace
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/embedders/hugging_face_api_document_embedder.py` & `haystack_ai-2.2.0rc1/haystack/components/embedders/hugging_face_api_document_embedder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import json
 from typing import Any, Dict, List, Optional, Union
 
 from tqdm import tqdm
 
 from haystack import component, default_from_dict, default_to_dict, logging
 from haystack.dataclasses import Document
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/embedders/hugging_face_api_text_embedder.py` & `haystack_ai-2.2.0rc1/haystack/components/embedders/hugging_face_api_text_embedder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import json
 from typing import Any, Dict, List, Optional, Union
 
 from haystack import component, default_from_dict, default_to_dict, logging
 from haystack.lazy_imports import LazyImport
 from haystack.utils import Secret, deserialize_secrets_inplace
 from haystack.utils.hf import HFEmbeddingAPIType, HFModelType, check_valid_model
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/embedders/hugging_face_tei_document_embedder.py` & `haystack_ai-2.2.0rc1/haystack/components/embedders/hugging_face_tei_document_embedder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import json
 import warnings
 from typing import Any, Dict, List, Optional
 from urllib.parse import urlparse
 
 from tqdm import tqdm
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/embedders/hugging_face_tei_text_embedder.py` & `haystack_ai-2.2.0rc1/haystack/components/embedders/hugging_face_tei_text_embedder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import json
 import warnings
 from typing import Any, Dict, List, Optional
 from urllib.parse import urlparse
 
 from haystack import component, default_from_dict, default_to_dict, logging
 from haystack.lazy_imports import LazyImport
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/embedders/openai_document_embedder.py` & `haystack_ai-2.2.0rc1/haystack/components/embedders/openai_document_embedder.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
+import os
 from typing import Any, Dict, List, Optional, Tuple
 
 from openai import OpenAI
 from tqdm import tqdm
 
 from haystack import Document, component, default_from_dict, default_to_dict
 from haystack.utils import Secret, deserialize_secrets_inplace
@@ -37,18 +42,23 @@
         organization: Optional[str] = None,
         prefix: str = "",
         suffix: str = "",
         batch_size: int = 32,
         progress_bar: bool = True,
         meta_fields_to_embed: Optional[List[str]] = None,
         embedding_separator: str = "\n",
+        timeout: Optional[float] = None,
+        max_retries: Optional[int] = None,
     ):
         """
         Create a OpenAIDocumentEmbedder component.
 
+        By setting the 'OPENAI_TIMEOUT' and 'OPENAI_MAX_RETRIES' you can change the timeout and max_retries parameters in the OpenAI client.
+
+
         :param api_key:
             The OpenAI API key.
         :param model:
             The name of the model to use.
         :param dimensions:
             The number of dimensions the resulting output embeddings should have. Only supported in `text-embedding-3` and later models.
         :param api_base_url:
@@ -65,28 +75,43 @@
             Number of Documents to encode at once.
         :param progress_bar:
             If True shows a progress bar when running.
         :param meta_fields_to_embed:
             List of meta fields that will be embedded along with the Document text.
         :param embedding_separator:
             Separator used to concatenate the meta fields to the Document text.
+        :param timeout:
+            Timeout for OpenAI Client calls, if not set it is inferred from the `OPENAI_TIMEOUT` environment variable or set to 30.
+        :param max_retries:
+            Maximum retries to stablish contact with OpenAI if it returns an internal error, if not set it is inferred from the `OPENAI_MAX_RETRIES` environment variable or set to 5.
         """
         self.api_key = api_key
         self.model = model
         self.dimensions = dimensions
         self.api_base_url = api_base_url
         self.organization = organization
         self.prefix = prefix
         self.suffix = suffix
         self.batch_size = batch_size
         self.progress_bar = progress_bar
         self.meta_fields_to_embed = meta_fields_to_embed or []
         self.embedding_separator = embedding_separator
 
-        self.client = OpenAI(api_key=api_key.resolve_value(), organization=organization, base_url=api_base_url)
+        if timeout is None:
+            timeout = float(os.environ.get("OPENAI_TIMEOUT", 30.0))
+        if max_retries is None:
+            max_retries = int(os.environ.get("OPENAI_MAX_RETRIES", 5))
+
+        self.client = OpenAI(
+            api_key=api_key.resolve_value(),
+            organization=organization,
+            base_url=api_base_url,
+            timeout=timeout,
+            max_retries=max_retries,
+        )
 
     def _get_telemetry_data(self) -> Dict[str, Any]:
         """
         Data that is sent to Posthog for usage analytics.
         """
         return {"model": self.model}
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/embedders/openai_text_embedder.py` & `haystack_ai-2.2.0rc1/haystack/components/embedders/openai_text_embedder.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,22 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
+import os
 from typing import Any, Dict, List, Optional
 
 from openai import OpenAI
 
 from haystack import component, default_from_dict, default_to_dict
 from haystack.utils import Secret, deserialize_secrets_inplace
 
+OPENAI_TIMEOUT = float(os.environ.get("OPENAI_TIMEOUT", 30))
+OPENAI_MAX_RETRIES = int(os.environ.get("OPENAI_MAX_RETRIES", 5))
+
 
 @component
 class OpenAITextEmbedder:
     """
     A component for embedding strings using OpenAI models.
 
     Usage example:
@@ -32,18 +40,22 @@
         api_key: Secret = Secret.from_env_var("OPENAI_API_KEY"),
         model: str = "text-embedding-ada-002",
         dimensions: Optional[int] = None,
         api_base_url: Optional[str] = None,
         organization: Optional[str] = None,
         prefix: str = "",
         suffix: str = "",
+        timeout: Optional[float] = None,
+        max_retries: Optional[int] = None,
     ):
         """
         Create an OpenAITextEmbedder component.
 
+        By setting the 'OPENAI_TIMEOUT' and 'OPENAI_MAX_RETRIES' you can change the timeout and max_retries parameters in the OpenAI client.
+
         :param api_key:
             The OpenAI API key.
         :param model:
             The name of the model to use.
         :param dimensions:
             The number of dimensions the resulting output embeddings should have. Only supported in `text-embedding-3` and later models.
         :param api_base_url:
@@ -52,24 +64,39 @@
             The Organization ID. See OpenAI's
             [production best practices](https://platform.openai.com/docs/guides/production-best-practices/setting-up-your-organization)
             for more information.
         :param prefix:
             A string to add at the beginning of each text.
         :param suffix:
             A string to add at the end of each text.
+        :param timeout:
+            Timeout for OpenAI Client calls, if not set it is inferred from the `OPENAI_TIMEOUT` environment variable or set to 30.
+        :param max_retries:
+            Maximum retries to stablish contact with OpenAI if it returns an internal error, if not set it is inferred from the `OPENAI_MAX_RETRIES` environment variable or set to 5.
         """
         self.model = model
         self.dimensions = dimensions
         self.api_base_url = api_base_url
         self.organization = organization
         self.prefix = prefix
         self.suffix = suffix
         self.api_key = api_key
 
-        self.client = OpenAI(api_key=api_key.resolve_value(), organization=organization, base_url=api_base_url)
+        if timeout is None:
+            timeout = float(os.environ.get("OPENAI_TIMEOUT", 30.0))
+        if max_retries is None:
+            max_retries = int(os.environ.get("OPENAI_MAX_RETRIES", 5))
+
+        self.client = OpenAI(
+            api_key=api_key.resolve_value(),
+            organization=organization,
+            base_url=api_base_url,
+            timeout=timeout,
+            max_retries=max_retries,
+        )
 
     def _get_telemetry_data(self) -> Dict[str, Any]:
         """
         Data that is sent to Posthog for usage analytics.
         """
         return {"model": self.model}
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/embedders/sentence_transformers_document_embedder.py` & `haystack_ai-2.2.0rc1/haystack/components/embedders/sentence_transformers_document_embedder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from typing import Any, Dict, List, Optional
 
 from haystack import Document, component, default_from_dict, default_to_dict
 from haystack.components.embedders.backends.sentence_transformers_backend import (
     _SentenceTransformersEmbeddingBackendFactory,
 )
 from haystack.utils import ComponentDevice, Secret, deserialize_secrets_inplace
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/embedders/sentence_transformers_text_embedder.py` & `haystack_ai-2.2.0rc1/haystack/components/embedders/sentence_transformers_text_embedder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from typing import Any, Dict, List, Optional
 
 from haystack import component, default_from_dict, default_to_dict
 from haystack.components.embedders.backends.sentence_transformers_backend import (
     _SentenceTransformersEmbeddingBackendFactory,
 )
 from haystack.utils import ComponentDevice, Secret, deserialize_secrets_inplace
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/embedders/backends/sentence_transformers_backend.py` & `haystack_ai-2.2.0rc1/haystack/components/embedders/backends/sentence_transformers_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from typing import Dict, List, Optional
 
 from haystack.lazy_imports import LazyImport
 from haystack.utils.auth import Secret
 
 with LazyImport(message="Run 'pip install \"sentence-transformers>=2.2.0\"'") as sentence_transformers_import:
     from sentence_transformers import SentenceTransformer
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/evaluators/answer_exact_match.py` & `haystack_ai-2.2.0rc1/haystack/components/evaluators/answer_exact_match.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from typing import Any, Dict, List
 
 from haystack.core.component import component
 
 
 @component
 class AnswerExactMatchEvaluator:
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/evaluators/context_relevance.py` & `haystack_ai-2.2.0rc1/haystack/components/evaluators/context_relevance.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from typing import Any, Dict, List, Optional
 
 from numpy import mean as np_mean
 
 from haystack import default_from_dict
 from haystack.components.evaluators.llm_evaluator import LLMEvaluator
 from haystack.core.component import component
@@ -59,16 +63,18 @@
     # [{'statements': ['Python, created by Guido van Rossum in the late 1980s.'], 'statement_scores': [1], 'score': 1.0}]
     ```
     """
 
     def __init__(
         self,
         examples: Optional[List[Dict[str, Any]]] = None,
+        progress_bar: bool = True,
         api: str = "openai",
         api_key: Secret = Secret.from_env_var("OPENAI_API_KEY"),
+        raise_on_failure: bool = True,
     ):
         """
         Creates an instance of ContextRelevanceEvaluator.
 
         :param examples:
             Optional few-shot examples conforming to the expected input and output format of ContextRelevanceEvaluator.
             Default examples will be used if none are provided.
@@ -81,19 +87,23 @@
                     "questions": "What is the capital of Italy?", "contexts": ["Rome is the capital of Italy."],
                 },
                 "outputs": {
                     "statements": ["Rome is the capital of Italy."],
                     "statement_scores": [1],
                 },
             }]
+        :param progress_bar:
+            Whether to show a progress bar during the evaluation.
         :param api:
             The API to use for calling an LLM through a Generator.
             Supported APIs: "openai".
         :param api_key:
             The API key.
+        :param raise_on_failure:
+            Whether to raise an exception if the API call fails.
 
         """
         self.instructions = (
             "Your task is to judge how relevant the provided context is for answering a question. "
             "First, please extract statements from the provided context. "
             "Second, calculate a relevance score for each statement in the context. "
             "The score is 1 if the statement is relevant to answer the question or 0 if it is not relevant."
@@ -107,14 +117,16 @@
         super().__init__(
             instructions=self.instructions,
             inputs=self.inputs,
             outputs=self.outputs,
             examples=self.examples,
             api=self.api,
             api_key=self.api_key,
+            raise_on_failure=raise_on_failure,
+            progress_bar=progress_bar,
         )
 
     @component.output_types(individual_scores=List[int], score=float, results=List[Dict[str, Any]])
     def run(self, questions: List[str], contexts: List[List[str]]) -> Dict[str, Any]:
         """
         Run the LLM evaluator.
 
@@ -127,15 +139,18 @@
                 - `score`: Mean context relevance score over all the provided input questions.
                 - `individual_scores`: A list of context relevance scores for each input question.
                 - `results`: A list of dictionaries with `statements` and `statement_scores` for each input context.
         """
         result = super().run(questions=questions, contexts=contexts)
 
         # calculate average statement relevance score per query
-        for res in result["results"]:
+        for idx, res in enumerate(result["results"]):
+            if res is None:
+                result["results"][idx] = {"statements": [], "statement_scores": [], "score": float("nan")}
+                continue
             if not res["statements"]:
                 res["score"] = 0
             else:
                 res["score"] = np_mean(res["statement_scores"])
 
         # calculate average context relevance score over all queries
         result["score"] = np_mean([res["score"] for res in result["results"]])
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/evaluators/document_map.py` & `haystack_ai-2.2.0rc1/haystack/components/evaluators/document_mrr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,88 +1,85 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from typing import Any, Dict, List
 
 from haystack import Document, component
 
 
 @component
-class DocumentMAPEvaluator:
+class DocumentMRREvaluator:
     """
-    A Mean Average Precision (MAP) evaluator for documents.
+    Evaluator that calculates the mean reciprocal rank of the retrieved documents.
 
-    Evaluator that calculates the mean average precision of the retrieved documents, a metric
-    that measures how high retrieved documents are ranked.
+    MRR measures how high the first retrieved document is ranked.
     Each question can have multiple ground truth documents and multiple retrieved documents.
 
-    `DocumentMAPEvaluator` doesn't normalize its inputs, the `DocumentCleaner` component
+    `DocumentMRREvaluator` doesn't normalize its inputs, the `DocumentCleaner` component
     should be used to clean and normalize the documents before passing them to this evaluator.
 
     Usage example:
     ```python
     from haystack import Document
-    from haystack.components.evaluators import DocumentMAPEvaluator
+    from haystack.components.evaluators import DocumentMRREvaluator
 
-    evaluator = DocumentMAPEvaluator()
+    evaluator = DocumentMRREvaluator()
     result = evaluator.run(
         ground_truth_documents=[
             [Document(content="France")],
             [Document(content="9th century"), Document(content="9th")],
         ],
         retrieved_documents=[
             [Document(content="France")],
             [Document(content="9th century"), Document(content="10th century"), Document(content="9th")],
         ],
     )
-
     print(result["individual_scores"])
-    # [1.0, 0.8333333333333333]
+    # [1.0, 1.0]
     print(result["score"])
-    # 0.9166666666666666
+    # 1.0
     ```
     """
 
     @component.output_types(score=float, individual_scores=List[float])
     def run(
         self, ground_truth_documents: List[List[Document]], retrieved_documents: List[List[Document]]
     ) -> Dict[str, Any]:
         """
-        Run the DocumentMAPEvaluator on the given inputs.
+        Run the DocumentMRREvaluator on the given inputs.
 
-        All lists must have the same length.
+        `ground_truth_documents` and `retrieved_documents` must have the same length.
 
         :param ground_truth_documents:
             A list of expected documents for each question.
         :param retrieved_documents:
             A list of retrieved documents for each question.
         :returns:
             A dictionary with the following outputs:
             - `score` - The average of calculated scores.
-            - `individual_scores` - A list of numbers from 0.0 to 1.0 that represents how high retrieved documents are ranked.
+            - `individual_scores` - A list of numbers from 0.0 to 1.0 that represents how high the first retrieved document is ranked.
         """
         if len(ground_truth_documents) != len(retrieved_documents):
             msg = "The length of ground_truth_documents and retrieved_documents must be the same."
             raise ValueError(msg)
 
         individual_scores = []
 
         for ground_truth, retrieved in zip(ground_truth_documents, retrieved_documents):
             score = 0.0
             for ground_document in ground_truth:
                 if ground_document.content is None:
                     continue
 
-                average_precision = 0.0
-                relevant_documents = 0
-
                 for rank, retrieved_document in enumerate(retrieved):
                     if retrieved_document.content is None:
                         continue
 
                     if ground_document.content in retrieved_document.content:
-                        relevant_documents += 1
-                        average_precision += relevant_documents / (rank + 1)
-                if relevant_documents > 0:
-                    score = average_precision / relevant_documents
+                        score = 1 / (rank + 1)
+                        break
             individual_scores.append(score)
 
         score = sum(individual_scores) / len(retrieved_documents)
 
         return {"score": score, "individual_scores": individual_scores}
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/evaluators/document_mrr.py` & `haystack_ai-2.2.0rc1/haystack/components/evaluators/document_map.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,92 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from typing import Any, Dict, List
 
 from haystack import Document, component
 
 
 @component
-class DocumentMRREvaluator:
+class DocumentMAPEvaluator:
     """
-    Evaluator that calculates the mean reciprocal rank of the retrieved documents.
+    A Mean Average Precision (MAP) evaluator for documents.
 
-    MRR measures how high the first retrieved document is ranked.
+    Evaluator that calculates the mean average precision of the retrieved documents, a metric
+    that measures how high retrieved documents are ranked.
     Each question can have multiple ground truth documents and multiple retrieved documents.
 
-    `DocumentMRREvaluator` doesn't normalize its inputs, the `DocumentCleaner` component
+    `DocumentMAPEvaluator` doesn't normalize its inputs, the `DocumentCleaner` component
     should be used to clean and normalize the documents before passing them to this evaluator.
 
     Usage example:
     ```python
     from haystack import Document
-    from haystack.components.evaluators import DocumentMRREvaluator
+    from haystack.components.evaluators import DocumentMAPEvaluator
 
-    evaluator = DocumentMRREvaluator()
+    evaluator = DocumentMAPEvaluator()
     result = evaluator.run(
         ground_truth_documents=[
             [Document(content="France")],
             [Document(content="9th century"), Document(content="9th")],
         ],
         retrieved_documents=[
             [Document(content="France")],
             [Document(content="9th century"), Document(content="10th century"), Document(content="9th")],
         ],
     )
+
     print(result["individual_scores"])
-    # [1.0, 1.0]
+    # [1.0, 0.8333333333333333]
     print(result["score"])
-    # 1.0
+    # 0.9166666666666666
     ```
     """
 
     @component.output_types(score=float, individual_scores=List[float])
     def run(
         self, ground_truth_documents: List[List[Document]], retrieved_documents: List[List[Document]]
     ) -> Dict[str, Any]:
         """
-        Run the DocumentMRREvaluator on the given inputs.
+        Run the DocumentMAPEvaluator on the given inputs.
 
-        `ground_truth_documents` and `retrieved_documents` must have the same length.
+        All lists must have the same length.
 
         :param ground_truth_documents:
             A list of expected documents for each question.
         :param retrieved_documents:
             A list of retrieved documents for each question.
         :returns:
             A dictionary with the following outputs:
             - `score` - The average of calculated scores.
-            - `individual_scores` - A list of numbers from 0.0 to 1.0 that represents how high the first retrieved document is ranked.
+            - `individual_scores` - A list of numbers from 0.0 to 1.0 that represents how high retrieved documents are ranked.
         """
         if len(ground_truth_documents) != len(retrieved_documents):
             msg = "The length of ground_truth_documents and retrieved_documents must be the same."
             raise ValueError(msg)
 
         individual_scores = []
 
         for ground_truth, retrieved in zip(ground_truth_documents, retrieved_documents):
             score = 0.0
             for ground_document in ground_truth:
                 if ground_document.content is None:
                     continue
 
+                average_precision = 0.0
+                relevant_documents = 0
+
                 for rank, retrieved_document in enumerate(retrieved):
                     if retrieved_document.content is None:
                         continue
 
                     if ground_document.content in retrieved_document.content:
-                        score = 1 / (rank + 1)
-                        break
+                        relevant_documents += 1
+                        average_precision += relevant_documents / (rank + 1)
+                if relevant_documents > 0:
+                    score = average_precision / relevant_documents
             individual_scores.append(score)
 
         score = sum(individual_scores) / len(retrieved_documents)
 
         return {"score": score, "individual_scores": individual_scores}
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/evaluators/document_recall.py` & `haystack_ai-2.2.0rc1/haystack/components/evaluators/document_recall.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from enum import Enum
 from typing import Any, Dict, List, Union
 
 from haystack import component, default_to_dict
 from haystack.dataclasses import Document
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/evaluators/faithfulness.py` & `haystack_ai-2.2.0rc1/haystack/components/evaluators/faithfulness.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from typing import Any, Dict, List, Optional
 
 from numpy import mean as np_mean
 
 from haystack import default_from_dict
 from haystack.components.evaluators.llm_evaluator import LLMEvaluator
 from haystack.core.component import component
@@ -73,16 +77,18 @@
     'Python was created by George Lucas.'], 'statement_scores': [1, 0], 'score': 0.5}]
     ```
     """
 
     def __init__(
         self,
         examples: Optional[List[Dict[str, Any]]] = None,
+        progress_bar: bool = True,
         api: str = "openai",
         api_key: Secret = Secret.from_env_var("OPENAI_API_KEY"),
+        raise_on_failure: bool = True,
     ):
         """
         Creates an instance of FaithfulnessEvaluator.
 
         :param examples:
             Optional few-shot examples conforming to the expected input and output format of FaithfulnessEvaluator.
             Default examples will be used if none are provided.
@@ -96,19 +102,23 @@
                     "predicted_answers": "Rome is the capital of Italy with more than 4 million inhabitants.",
                 },
                 "outputs": {
                     "statements": ["Rome is the capital of Italy.", "Rome has more than 4 million inhabitants."],
                     "statement_scores": [1, 0],
                 },
             }]
+        :param progress_bar:
+            Whether to show a progress bar during the evaluation.
         :param api:
             The API to use for calling an LLM through a Generator.
             Supported APIs: "openai".
         :param api_key:
             The API key.
+        :param raise_on_failure:
+            Whether to raise an exception if the API call fails.
 
         """
         self.instructions = (
             "Your task is to judge the faithfulness or groundedness of statements based "
             "on context information. First, please extract statements from a provided "
             "predicted answer to a question. Second, calculate a faithfulness score for each "
             "statement made in the predicted answer. The score is 1 if the statement can be "
@@ -123,14 +133,16 @@
         super().__init__(
             instructions=self.instructions,
             inputs=self.inputs,
             outputs=self.outputs,
             examples=self.examples,
             api=self.api,
             api_key=self.api_key,
+            raise_on_failure=raise_on_failure,
+            progress_bar=progress_bar,
         )
 
     @component.output_types(individual_scores=List[int], score=float, results=List[Dict[str, Any]])
     def run(self, questions: List[str], contexts: List[List[str]], predicted_answers: List[str]) -> Dict[str, Any]:
         """
         Run the LLM evaluator.
 
@@ -145,15 +157,18 @@
                 - `score`: Mean faithfulness score over all the provided input answers.
                 - `individual_scores`: A list of faithfulness scores for each input answer.
                 - `results`: A list of dictionaries with `statements` and `statement_scores` for each input answer.
         """
         result = super().run(questions=questions, contexts=contexts, predicted_answers=predicted_answers)
 
         # calculate average statement faithfulness score per query
-        for res in result["results"]:
+        for idx, res in enumerate(result["results"]):
+            if res is None:
+                result["results"][idx] = {"statements": [], "statement_scores": [], "score": float("nan")}
+                continue
             if not res["statements"]:
                 res["score"] = 0
             else:
                 res["score"] = np_mean(res["statement_scores"])
 
         # calculate average answer faithfulness score over all queries
         result["score"] = np_mean([res["score"] for res in result["results"]])
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/evaluators/llm_evaluator.py` & `haystack_ai-2.2.0rc1/haystack/components/evaluators/llm_evaluator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,16 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import json
-from typing import Any, Dict, List, Tuple, Type
+from typing import Any, Dict, List, Optional, Tuple, Type
+from warnings import warn
+
+from tqdm import tqdm
 
 from haystack import component, default_from_dict, default_to_dict
 from haystack.components.builders import PromptBuilder
 from haystack.components.generators import OpenAIGenerator
 from haystack.utils import Secret, deserialize_secrets_inplace
 
 
@@ -42,15 +49,17 @@
 
     def __init__(
         self,
         instructions: str,
         inputs: List[Tuple[str, Type[List]]],
         outputs: List[str],
         examples: List[Dict[str, Any]],
+        progress_bar: bool = True,
         *,
+        raise_on_failure: bool = True,
         api: str = "openai",
         api_key: Secret = Secret.from_env_var("OPENAI_API_KEY"),
     ):
         """
         Creates an instance of LLMEvaluator.
 
         :param instructions:
@@ -62,44 +71,50 @@
         :param outputs:
             Output names of the evaluation results. They correspond to keys in the output dictionary.
         :param examples:
             Few-shot examples conforming to the expected input and output format as defined in the `inputs` and
              `outputs` parameters.
             Each example is a dictionary with keys "inputs" and "outputs"
             They contain the input and output as dictionaries respectively.
+        :param raise_on_failure:
+            If True, the component will raise an exception on an unsuccessful API call.
+        :param progress_bar:
+            Whether to show a progress bar during the evaluation.
         :param api:
             The API to use for calling an LLM through a Generator.
             Supported APIs: "openai".
         :param api_key:
             The API key.
 
         """
         self.validate_init_parameters(inputs, outputs, examples)
-
+        self.raise_on_failure = raise_on_failure
         self.instructions = instructions
         self.inputs = inputs
         self.outputs = outputs
         self.examples = examples
         self.api = api
         self.api_key = api_key
+        self.progress_bar = progress_bar
 
         if api == "openai":
             self.generator = OpenAIGenerator(
-                api_key=api_key, generation_kwargs={"response_format": {"type": "json_object"}}
+                api_key=api_key, generation_kwargs={"response_format": {"type": "json_object"}, "seed": 42}
             )
         else:
             raise ValueError(f"Unsupported API: {api}")
 
         template = self.prepare_template()
         self.builder = PromptBuilder(template=template)
 
         component.set_input_types(self, **dict(inputs))
 
+    @staticmethod
     def validate_init_parameters(
-        self, inputs: List[Tuple[str, Type[List]]], outputs: List[str], examples: List[Dict[str, Any]]
+        inputs: List[Tuple[str, Type[List]]], outputs: List[str], examples: List[Dict[str, Any]]
     ):
         """
         Validate the init parameters.
 
         :param inputs:
             The inputs to validate.
         :param outputs:
@@ -154,31 +169,52 @@
         Run the LLM evaluator.
 
         :param inputs:
             The input values to evaluate. The keys are the input names and the values are lists of input values.
         :returns:
             A dictionary with a single `results` entry that contains a list of results.
             Each result is a dictionary containing the keys as defined in the `outputs` parameter of the LLMEvaluator
-            and the evaluation results as the values.
+            and the evaluation results as the values. If an exception occurs for a particular input value, the result
+            will be `None` for that entry.
+        :raises ValueError:
+            Only in the case that  `raise_on_failure` is set to True and the received inputs are not lists or have
+            different lengths, or if the output is not a valid JSON or doesn't contain the expected keys.
         """
         self.validate_input_parameters(dict(self.inputs), inputs)
 
         # inputs is a dictionary with keys being input names and values being a list of input values
         # We need to iterate through the lists in parallel for all keys of the dictionary
         input_names, values = inputs.keys(), list(zip(*inputs.values()))
         list_of_input_names_to_values = [dict(zip(input_names, v)) for v in values]
 
-        results = []
-        for input_names_to_values in list_of_input_names_to_values:
+        results: List[Optional[Dict[str, Any]]] = []
+        errors = 0
+        for input_names_to_values in tqdm(list_of_input_names_to_values, disable=not self.progress_bar):
             prompt = self.builder.run(**input_names_to_values)
-            result = self.generator.run(prompt=prompt["prompt"])
-
-            self.validate_outputs(expected=self.outputs, received=result["replies"][0])
-            parsed_result = json.loads(result["replies"][0])
-            results.append(parsed_result)
+            try:
+                result = self.generator.run(prompt=prompt["prompt"])
+            except Exception as e:
+                msg = f"Error while generating response for prompt: {prompt}. Error: {e}"
+                if self.raise_on_failure:
+                    raise ValueError(msg)
+                warn(msg)
+                results.append(None)
+                errors += 1
+                continue
+
+            if self.is_valid_json_and_has_expected_keys(expected=self.outputs, received=result["replies"][0]):
+                parsed_result = json.loads(result["replies"][0])
+                results.append(parsed_result)
+            else:
+                results.append(None)
+                errors += 1
+
+        if errors > 0:
+            msg = f"LLM evaluator failed for {errors} out of {len(list_of_input_names_to_values)} inputs."
+            warn(msg)
 
         return {"results": results}
 
     def prepare_template(self) -> str:
         """
         Prepare the prompt template.
 
@@ -234,14 +270,15 @@
             self,
             instructions=self.instructions,
             inputs=self.inputs,
             outputs=self.outputs,
             examples=self.examples,
             api=self.api,
             api_key=self.api_key.to_dict(),
+            progress_bar=self.progress_bar,
         )
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> "LLMEvaluator":
         """
         Deserialize this component from a dictionary.
 
@@ -284,24 +321,41 @@
         if not all(len(_input) == length for _input in inputs):
             msg = (
                 f"LLM evaluator expects all input lists to have the same length but received {inputs} with lengths "
                 f"{[len(_input) for _input in inputs]}."
             )
             raise ValueError(msg)
 
-    @staticmethod
-    def validate_outputs(expected: List[str], received: str) -> None:
+    def is_valid_json_and_has_expected_keys(self, expected: List[str], received: str) -> bool:
         """
-        Validate the output.
+        Output must be a valid JSON with the expected keys.
 
         :param expected:
             Names of expected outputs
         :param received:
             Names of received outputs
 
         :raises ValueError:
-            If not all expected outputs are present in the received outputs
+            If the output is not a valid JSON with the expected keys:
+            - with `raise_on_failure` set to True a ValueError is raised.
+            - with `raise_on_failure` set to False a warning is issued and False is returned.
+
+        :returns:
+            True if the received output is a valid JSON with the expected keys, False otherwise.
         """
-        parsed_output = json.loads(received)
+        try:
+            parsed_output = json.loads(received)
+        except json.JSONDecodeError:
+            msg = "Response from LLM evaluator is not a valid JSON."
+            if self.raise_on_failure:
+                raise ValueError(msg)
+            warn(msg)
+            return False
+
         if not all(output in parsed_output for output in expected):
             msg = f"Expected response from LLM evaluator to be JSON with keys {expected}, got {received}."
-            raise ValueError(msg)
+            if self.raise_on_failure:
+                raise ValueError(msg)
+            warn(msg)
+            return False
+
+        return True
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/evaluators/sas_evaluator.py` & `haystack_ai-2.2.0rc1/haystack/components/evaluators/sas_evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from typing import Any, Dict, List, Optional
 
 from numpy import mean as np_mean
 
 from haystack import component, default_from_dict, default_to_dict
 from haystack.lazy_imports import LazyImport
 from haystack.utils import ComponentDevice, expit
@@ -108,14 +112,17 @@
             data["init_parameters"]["device"] = ComponentDevice.from_dict(device)
         return default_from_dict(cls, data)
 
     def warm_up(self):
         """
         Initializes the component.
         """
+        if self._similarity_model:
+            return
+
         token = self._token.resolve_value() if self._token else None
         config = AutoConfig.from_pretrained(self._model, use_auth_token=token)
         cross_encoder_used = False
         if config.architectures:
             cross_encoder_used = any(arch.endswith("ForSequenceClassification") for arch in config.architectures)
         device = ComponentDevice.resolve_device(self._device).to_torch_str()
         # Based on the Model string we can load either Bi-Encoders or Cross Encoders.
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/extractors/named_entity_extractor.py` & `haystack_ai-2.2.0rc1/haystack/components/extractors/named_entity_extractor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from abc import ABC, abstractmethod
 from contextlib import contextmanager
 from dataclasses import dataclass
-from enum import Enum, EnumMeta
+from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
 from haystack import ComponentError, DeserializationError, Document, component, default_from_dict, default_to_dict
 from haystack.lazy_imports import LazyImport
 from haystack.utils.device import ComponentDevice
 
 with LazyImport(message="Run 'pip install transformers[torch]'") as transformers_import:
@@ -13,46 +17,43 @@
     from transformers import Pipeline as HfPipeline
 
 with LazyImport(message="Run 'pip install spacy'") as spacy_import:
     import spacy
     from spacy import Language as SpacyPipeline
 
 
-class _BackendEnumMeta(EnumMeta):
-    """
-    Metaclass for fine-grained error handling of backend enums.
-    """
-
-    def __call__(cls, value, names=None, *, module=None, qualname=None, type=None, start=1):  # noqa: A002
-        if names is None:
-            try:
-                return EnumMeta.__call__(cls, value, names, module=module, qualname=qualname, type=type, start=start)
-            except ValueError:
-                supported_backends = ", ".join(sorted(v.value for v in cls))  # pylint: disable=not-an-iterable
-                raise ComponentError(
-                    f"Invalid backend `{value}` for named entity extractor. "
-                    f"Supported backends: {supported_backends}"
-                )
-        else:
-            return EnumMeta.__call__(  # pylint: disable=too-many-function-args
-                cls, value, names, module, qualname, type, start
-            )
-
-
-class NamedEntityExtractorBackend(Enum, metaclass=_BackendEnumMeta):
+class NamedEntityExtractorBackend(Enum):
     """
     NLP backend to use for Named Entity Recognition.
     """
 
     #: Uses an Hugging Face model and pipeline.
     HUGGING_FACE = "hugging_face"
 
     #: Uses a spaCy model and pipeline.
     SPACY = "spacy"
 
+    def __str__(self):
+        return self.value
+
+    @staticmethod
+    def from_str(string: str) -> "NamedEntityExtractorBackend":
+        """
+        Convert a string to a NamedEntityExtractorBackend enum.
+        """
+        enum_map = {e.value: e for e in NamedEntityExtractorBackend}
+        mode = enum_map.get(string)
+        if mode is None:
+            msg = (
+                f"Invalid backend '{string}' for named entity extractor. "
+                f"Supported backends are: {list(enum_map.keys())}"
+            )
+            raise ComponentError(msg)
+        return mode
+
 
 @dataclass
 class NamedEntityAnnotation:
     """
     Describes a single NER annotation.
 
     :param entity:
@@ -126,17 +127,18 @@
             the default device is automatically selected. If a
             device/device map is specified in `pipeline_kwargs`,
             it overrides this parameter (only applicable to the
             HuggingFace backend).
         """
 
         if isinstance(backend, str):
-            backend = NamedEntityExtractorBackend(backend)
+            backend = NamedEntityExtractorBackend.from_str(backend)
 
         self._backend: _NerBackend
+        self._warmed_up: bool = False
         device = ComponentDevice.resolve_device(device)
 
         if backend == NamedEntityExtractorBackend.HUGGING_FACE:
             self._backend = _HfBackend(model_name_or_path=model, device=device, pipeline_kwargs=pipeline_kwargs)
         elif backend == NamedEntityExtractorBackend.SPACY:
             self._backend = _SpacyBackend(model_name_or_path=model, device=device, pipeline_kwargs=pipeline_kwargs)
         else:
@@ -145,16 +147,20 @@
     def warm_up(self):
         """
         Initialize the component.
 
         :raises ComponentError:
             If the backend fails to initialize successfully.
         """
+        if self._warmed_up:
+            return
+
         try:
             self._backend.initialize()
+            self._warmed_up = True
         except Exception as e:
             raise ComponentError(
                 f"Named entity extractor with backend '{self._backend.type} failed to initialize."
             ) from e
 
     @component.output_types(documents=List[Document])
     def run(self, documents: List[Document], batch_size: int = 1) -> Dict[str, Any]:
@@ -166,14 +172,18 @@
         :param batch_size:
             Batch size used for processing the documents.
         :returns:
             Processed documents.
         :raises ComponentError:
             If the backend fails to process a document.
         """
+        if not self._warmed_up:
+            msg = "The component NamedEntityExtractor was not warmed up. Call warm_up() before running the component."
+            raise RuntimeError(msg)
+
         texts = [doc.content if doc.content is not None else "" for doc in documents]
         annotations = self._backend.annotate(texts, batch_size=batch_size)
 
         if len(annotations) != len(documents):
             raise ComponentError(
                 "NER backend did not return the correct number of annotations; "
                 f"got {len(annotations)} but expected {len(documents)}"
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/fetchers/link_content.py` & `haystack_ai-2.2.0rc1/haystack/components/fetchers/link_content.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from collections import defaultdict
 from concurrent.futures import ThreadPoolExecutor
 from typing import Callable, Dict, List, Optional, Tuple
 
 import requests
 from requests import Response
 from requests.exceptions import HTTPError
@@ -143,14 +147,15 @@
         else:
             with ThreadPoolExecutor() as executor:
                 results = executor.map(self._fetch_with_exception_suppression, urls)
 
             for stream_metadata, stream in results:  # type: ignore
                 if stream_metadata is not None and stream is not None:
                     stream.meta.update(stream_metadata)
+                    stream.mime_type = stream.meta.get("content_type", None)
                     streams.append(stream)
 
         return {"streams": streams}
 
     def _fetch(self, url: str) -> Tuple[Dict[str, str], ByteStream]:
         """
         Fetches content from a URL and returns it as a ByteStream.
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/generators/__init__.py` & `haystack_ai-2.2.0rc1/haystack/components/generators/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from haystack.components.generators.openai import (  # noqa: I001 (otherwise we end up with partial imports)
     OpenAIGenerator,
 )
 from haystack.components.generators.azure import AzureOpenAIGenerator
 from haystack.components.generators.hugging_face_local import HuggingFaceLocalGenerator
 from haystack.components.generators.hugging_face_tgi import HuggingFaceTGIGenerator
 from haystack.components.generators.hugging_face_api import HuggingFaceAPIGenerator
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/generators/azure.py` & `haystack_ai-2.2.0rc1/haystack/components/generators/azure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import os
 from typing import Any, Callable, Dict, Optional
 
 # pylint: disable=import-error
 from openai.lib.azure import AzureOpenAI
 
 from haystack import component, default_from_dict, default_to_dict, logging
@@ -54,14 +58,15 @@
         api_version: Optional[str] = "2023-05-15",
         azure_deployment: Optional[str] = "gpt-35-turbo",
         api_key: Optional[Secret] = Secret.from_env_var("AZURE_OPENAI_API_KEY", strict=False),
         azure_ad_token: Optional[Secret] = Secret.from_env_var("AZURE_OPENAI_AD_TOKEN", strict=False),
         organization: Optional[str] = None,
         streaming_callback: Optional[Callable[[StreamingChunk], None]] = None,
         system_prompt: Optional[str] = None,
+        timeout: Optional[float] = None,
         generation_kwargs: Optional[Dict[str, Any]] = None,
     ):
         """
         Initialize the Azure OpenAI Generator.
 
         :param azure_endpoint: The endpoint of the deployed model, e.g. `https://example-resource.azure.openai.com/`
         :param api_version: The version of the API to use. Defaults to 2023-05-15
@@ -69,14 +74,15 @@
         :param api_key: The API key to use for authentication.
         :param azure_ad_token: [Azure Active Directory token](https://www.microsoft.com/en-us/security/business/identity-access/microsoft-entra-id)
         :param organization: The Organization ID, defaults to `None`. See
         [production best practices](https://platform.openai.com/docs/guides/production-best-practices/setting-up-your-organization).
         :param streaming_callback: A callback function that is called when a new token is received from the stream.
             The callback function accepts StreamingChunk as an argument.
         :param system_prompt: The prompt to use for the system. If not provided, the system prompt will be
+        :param timeout: The timeout to be passed to the underlying `AzureOpenAI` client.
         :param generation_kwargs: Other parameters to use for the model. These parameters are all sent directly to
             the OpenAI endpoint. See OpenAI [documentation](https://platform.openai.com/docs/api-reference/chat) for
             more details.
             Some of the supported parameters:
             - `max_tokens`: The maximum number of tokens the output text can have.
             - `temperature`: What sampling temperature to use. Higher values mean the model will take more risks.
                 Try 0.9 for more creative applications and 0 (argmax sampling) for ones with a well-defined answer.
@@ -115,22 +121,24 @@
         self.system_prompt = system_prompt
         self.streaming_callback = streaming_callback
         self.api_version = api_version
         self.azure_endpoint = azure_endpoint
         self.azure_deployment = azure_deployment
         self.organization = organization
         self.model: str = azure_deployment or "gpt-35-turbo"
+        self.timeout = timeout
 
         self.client = AzureOpenAI(
             api_version=api_version,
             azure_endpoint=azure_endpoint,
             azure_deployment=azure_deployment,
             api_key=api_key.resolve_value() if api_key is not None else None,
             azure_ad_token=azure_ad_token.resolve_value() if azure_ad_token is not None else None,
             organization=organization,
+            timeout=timeout,
         )
 
     def to_dict(self) -> Dict[str, Any]:
         """
         Serialize this component to a dictionary.
 
         :returns:
@@ -144,14 +152,15 @@
             organization=self.organization,
             api_version=self.api_version,
             streaming_callback=callback_name,
             generation_kwargs=self.generation_kwargs,
             system_prompt=self.system_prompt,
             api_key=self.api_key.to_dict() if self.api_key is not None else None,
             azure_ad_token=self.azure_ad_token.to_dict() if self.azure_ad_token is not None else None,
+            timeout=self.timeout,
         )
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> "AzureOpenAIGenerator":
         """
         Deserialize this component from a dictionary.
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/generators/hugging_face_api.py` & `haystack_ai-2.2.0rc1/haystack/components/generators/hugging_face_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from dataclasses import asdict
 from typing import Any, Callable, Dict, Iterable, List, Optional, Union
 
 from haystack import component, default_from_dict, default_to_dict, logging
 from haystack.dataclasses import StreamingChunk
 from haystack.lazy_imports import LazyImport
 from haystack.utils import Secret, deserialize_callable, deserialize_secrets_inplace, serialize_callable
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/generators/hugging_face_local.py` & `haystack_ai-2.2.0rc1/haystack/components/generators/hugging_face_local.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from typing import Any, Callable, Dict, List, Literal, Optional
 
 from haystack import component, default_from_dict, default_to_dict, logging
 from haystack.dataclasses import StreamingChunk
 from haystack.lazy_imports import LazyImport
 from haystack.utils import (
     ComponentDevice,
@@ -132,18 +136,27 @@
         """
         Data that is sent to Posthog for usage analytics.
         """
         if isinstance(self.huggingface_pipeline_kwargs["model"], str):
             return {"model": self.huggingface_pipeline_kwargs["model"]}
         return {"model": f"[object of type {type(self.huggingface_pipeline_kwargs['model'])}]"}
 
+    @property
+    def _warmed_up(self) -> bool:
+        if self.stop_words:
+            return (self.pipeline is not None) and (self.stopping_criteria_list is not None)
+        return self.pipeline is not None
+
     def warm_up(self):
         """
         Initializes the component.
         """
+        if self._warmed_up:
+            return
+
         if self.pipeline is None:
             self.pipeline = pipeline(**self.huggingface_pipeline_kwargs)
 
         if self.stop_words:
             stop_words_criteria = StopWordsCriteria(
                 tokenizer=self.pipeline.tokenizer, stop_words=self.stop_words, device=self.pipeline.device
             )
@@ -201,39 +214,41 @@
         :param generation_kwargs:
             Additional keyword arguments for text generation.
 
         :returns:
             A dictionary containing the generated replies.
             - replies: A list of strings representing the generated replies.
         """
-        if self.pipeline is None:
-            raise RuntimeError("The generation model has not been loaded. Please call warm_up() before running.")
+        if not self._warmed_up:
+            raise RuntimeError(
+                "The component HuggingFaceLocalGenerator was not warmed up. Please call warm_up() before running."
+            )
 
         if not prompt:
             return {"replies": []}
 
         # merge generation kwargs from init method with those from run method
         updated_generation_kwargs = {**self.generation_kwargs, **(generation_kwargs or {})}
 
         if self.streaming_callback:
             num_responses = updated_generation_kwargs.get("num_return_sequences", 1)
             if num_responses > 1:
-                logger.warning(
-                    "Streaming is enabled, but the number of responses is set to %d. "
+                msg = (
+                    "Streaming is enabled, but the number of responses is set to {num_responses}. "
                     "Streaming is only supported for single response generation. "
-                    "Setting the number of responses to 1.",
-                    num_responses,
+                    "Setting the number of responses to 1."
                 )
+                logger.warning(msg, num_responses=num_responses)
                 updated_generation_kwargs["num_return_sequences"] = 1
             # streamer parameter hooks into HF streaming, HFTokenStreamingHandler is an adapter to our streaming
             updated_generation_kwargs["streamer"] = HFTokenStreamingHandler(
-                self.pipeline.tokenizer, self.streaming_callback, self.stop_words
+                self.pipeline.tokenizer, self.streaming_callback, self.stop_words  # type: ignore
             )
 
-        output = self.pipeline(prompt, stopping_criteria=self.stopping_criteria_list, **updated_generation_kwargs)
+        output = self.pipeline(prompt, stopping_criteria=self.stopping_criteria_list, **updated_generation_kwargs)  # type: ignore
         replies = [o["generated_text"] for o in output if "generated_text" in o]
 
         if self.stop_words:
             # the output of the pipeline includes the stop word
             replies = [reply.replace(stop_word, "").rstrip() for reply in replies for stop_word in self.stop_words]
 
         return {"replies": replies}
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/generators/hugging_face_tgi.py` & `haystack_ai-2.2.0rc1/haystack/components/generators/hugging_face_tgi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import warnings
 from dataclasses import asdict
 from typing import Any, Callable, Dict, Iterable, List, Optional
 from urllib.parse import urlparse
 
 from haystack import component, default_from_dict, default_to_dict, logging
 from haystack.dataclasses import StreamingChunk
@@ -132,14 +136,16 @@
         self.streaming_callback = streaming_callback
         self.tokenizer = None
 
     def warm_up(self) -> None:
         """
         Initializes the component.
         """
+        if self.tokenizer is not None:
+            return
 
         # is this user using HF free tier inference API?
         if self.model and not self.url:
             deployed_models = list_inference_deployed_models()
             # Determine if the specified model is deployed in the free tier.
             if self.model not in deployed_models:
                 raise ValueError(
@@ -197,26 +203,28 @@
             A string representing the prompt.
         :param generation_kwargs:
             Additional keyword arguments for text generation.
         :returns:
             A dictionary containing the generated replies and metadata. Both are lists of length n.
             - replies: A list of strings representing the generated replies.
         """
+        if not self.tokenizer:
+            raise RuntimeError(
+                "The component HuggingFaceTGIGenerator was not warmed up. Please call warm_up() before running LLM inference."
+            )
+
         # check generation kwargs given as parameters to override the default ones
         additional_params = ["n", "stop_words"]
         check_generation_params(generation_kwargs, additional_params)
 
         # update generation kwargs by merging with the default ones
         generation_kwargs = {**self.generation_kwargs, **(generation_kwargs or {})}
         num_responses = generation_kwargs.pop("n", 1)
         generation_kwargs.setdefault("stop_sequences", []).extend(generation_kwargs.pop("stop_words", []))
 
-        if self.tokenizer is None:
-            raise RuntimeError("Please call warm_up() before running LLM inference.")
-
         prompt_token_count = len(self.tokenizer.encode(prompt, add_special_tokens=False))
 
         if self.streaming_callback:
             if num_responses > 1:
                 raise ValueError("Cannot stream multiple responses, please set n=1.")
 
             return self._run_streaming(prompt, prompt_token_count, generation_kwargs)
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/generators/openai.py` & `haystack_ai-2.2.0rc1/haystack/components/generators/openai.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
+import os
 from typing import Any, Callable, Dict, List, Optional, Union
 
 from openai import OpenAI, Stream
 from openai.types.chat import ChatCompletion, ChatCompletionChunk
 
 from haystack import component, default_from_dict, default_to_dict, logging
 from haystack.dataclasses import ChatMessage, StreamingChunk
@@ -52,18 +57,23 @@
         api_key: Secret = Secret.from_env_var("OPENAI_API_KEY"),
         model: str = "gpt-3.5-turbo",
         streaming_callback: Optional[Callable[[StreamingChunk], None]] = None,
         api_base_url: Optional[str] = None,
         organization: Optional[str] = None,
         system_prompt: Optional[str] = None,
         generation_kwargs: Optional[Dict[str, Any]] = None,
+        timeout: Optional[float] = None,
+        max_retries: Optional[int] = None,
     ):
         """
         Creates an instance of OpenAIGenerator. Unless specified otherwise in the `model`, this is for OpenAI's GPT-3.5 model.
 
+        By setting the 'OPENAI_TIMEOUT' and 'OPENAI_MAX_RETRIES' you can change the timeout and max_retries parameters in the OpenAI client.
+
+
         :param api_key: The OpenAI API key.
         :param model: The name of the model to use.
         :param streaming_callback: A callback function that is called when a new token is received from the stream.
             The callback function accepts StreamingChunk as an argument.
         :param api_base_url: An optional base URL.
         :param organization: The Organization ID, defaults to `None`. See
         [production best practices](https://platform.openai.com/docs/guides/production-best-practices/setting-up-your-organization).
@@ -84,24 +94,41 @@
             - `stop`: One or more sequences after which the LLM should stop generating tokens.
             - `presence_penalty`: What penalty to apply if a token is already present at all. Bigger values mean
                 the model will be less likely to repeat the same token in the text.
             - `frequency_penalty`: What penalty to apply if a token has already been generated in the text.
                 Bigger values mean the model will be less likely to repeat the same token in the text.
             - `logit_bias`: Add a logit bias to specific tokens. The keys of the dictionary are tokens, and the
                 values are the bias to add to that token.
+        :param timeout:
+            Timeout for OpenAI Client calls, if not set it is inferred from the `OPENAI_TIMEOUT` environment variable or set to 30.
+        :param max_retries:
+            Maximum retries to establish contact with OpenAI if it returns an internal error, if not set it is inferred from the `OPENAI_MAX_RETRIES` environment variable or set to 5.
+
         """
         self.api_key = api_key
         self.model = model
         self.generation_kwargs = generation_kwargs or {}
         self.system_prompt = system_prompt
         self.streaming_callback = streaming_callback
 
         self.api_base_url = api_base_url
         self.organization = organization
-        self.client = OpenAI(api_key=api_key.resolve_value(), organization=organization, base_url=api_base_url)
+
+        if timeout is None:
+            timeout = float(os.environ.get("OPENAI_TIMEOUT", 30.0))
+        if max_retries is None:
+            max_retries = int(os.environ.get("OPENAI_MAX_RETRIES", 5))
+
+        self.client = OpenAI(
+            api_key=api_key.resolve_value(),
+            organization=organization,
+            base_url=api_base_url,
+            timeout=timeout,
+            max_retries=max_retries,
+        )
 
     def _get_telemetry_data(self) -> Dict[str, Any]:
         """
         Data that is sent to Posthog for usage analytics.
         """
         return {"model": self.model}
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/generators/utils.py` & `haystack_ai-2.2.0rc1/haystack/components/generators/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from typing import Callable, Optional
 
 from haystack.dataclasses import StreamingChunk
 from haystack.utils import deserialize_callable, serialize_callable
 
 
 def print_streaming_chunk(chunk: StreamingChunk) -> None:
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/generators/chat/azure.py` & `haystack_ai-2.2.0rc1/haystack/components/generators/chat/azure.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import os
 from typing import Any, Callable, Dict, Optional
 
 # pylint: disable=import-error
 from openai.lib.azure import AzureOpenAI
 
 from haystack import component, default_from_dict, default_to_dict, logging
@@ -72,14 +76,15 @@
         azure_endpoint: Optional[str] = None,
         api_version: Optional[str] = "2023-05-15",
         azure_deployment: Optional[str] = "gpt-35-turbo",
         api_key: Optional[Secret] = Secret.from_env_var("AZURE_OPENAI_API_KEY", strict=False),
         azure_ad_token: Optional[Secret] = Secret.from_env_var("AZURE_OPENAI_AD_TOKEN", strict=False),
         organization: Optional[str] = None,
         streaming_callback: Optional[Callable[[StreamingChunk], None]] = None,
+        timeout: Optional[float] = None,
         generation_kwargs: Optional[Dict[str, Any]] = None,
     ):
         """
         Initialize the Azure OpenAI Chat Generator component.
 
         :param azure_endpoint: The endpoint of the deployed model, e.g. `"https://example-resource.azure.openai.com/"`
         :param api_version: The version of the API to use. Defaults to 2023-05-15
@@ -131,14 +136,15 @@
         self.generation_kwargs = generation_kwargs or {}
         self.streaming_callback = streaming_callback
         self.api_version = api_version
         self.azure_endpoint = azure_endpoint
         self.azure_deployment = azure_deployment
         self.organization = organization
         self.model = azure_deployment or "gpt-35-turbo"
+        self.timeout = timeout
 
         self.client = AzureOpenAI(
             api_version=api_version,
             azure_endpoint=azure_endpoint,
             azure_deployment=azure_deployment,
             api_key=api_key.resolve_value() if api_key is not None else None,
             azure_ad_token=azure_ad_token.resolve_value() if azure_ad_token is not None else None,
@@ -157,14 +163,15 @@
             self,
             azure_endpoint=self.azure_endpoint,
             azure_deployment=self.azure_deployment,
             organization=self.organization,
             api_version=self.api_version,
             streaming_callback=callback_name,
             generation_kwargs=self.generation_kwargs,
+            timeout=self.timeout,
             api_key=self.api_key.to_dict() if self.api_key is not None else None,
             azure_ad_token=self.azure_ad_token.to_dict() if self.azure_ad_token is not None else None,
         )
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> "AzureOpenAIChatGenerator":
         """
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/generators/chat/hugging_face_api.py` & `haystack_ai-2.2.0rc1/haystack/components/generators/chat/hugging_face_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from typing import Any, Callable, Dict, Iterable, List, Optional, Union
 
 from haystack import component, default_from_dict, default_to_dict, logging
 from haystack.dataclasses import ChatMessage, StreamingChunk
 from haystack.lazy_imports import LazyImport
 from haystack.utils import Secret, deserialize_callable, deserialize_secrets_inplace, serialize_callable
 from haystack.utils.hf import HFGenerationAPIType, HFModelType, check_valid_model
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/generators/chat/hugging_face_local.py` & `haystack_ai-2.2.0rc1/haystack/components/generators/chat/hugging_face_local.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import sys
 from typing import Any, Callable, Dict, List, Literal, Optional, Union
 
 from haystack import component, default_from_dict, default_to_dict, logging
 from haystack.dataclasses import ChatMessage, StreamingChunk
 from haystack.lazy_imports import LazyImport
 from haystack.utils import (
@@ -257,20 +261,20 @@
         stop_words_criteria = StopWordsCriteria(tokenizer, stop_words, self.pipeline.device) if stop_words else None
         if stop_words_criteria:
             generation_kwargs["stopping_criteria"] = StoppingCriteriaList([stop_words_criteria])
 
         if self.streaming_callback:
             num_responses = generation_kwargs.get("num_return_sequences", 1)
             if num_responses > 1:
-                logger.warning(
-                    "Streaming is enabled, but the number of responses is set to %d. "
+                msg = (
+                    "Streaming is enabled, but the number of responses is set to {num_responses}. "
                     "Streaming is only supported for single response generation. "
-                    "Setting the number of responses to 1.",
-                    num_responses,
+                    "Setting the number of responses to 1."
                 )
+                logger.warning(msg, num_responses=num_responses)
                 generation_kwargs["num_return_sequences"] = 1
             # streamer parameter hooks into HF streaming, HFTokenStreamingHandler is an adapter to our streaming
             generation_kwargs["streamer"] = HFTokenStreamingHandler(tokenizer, self.streaming_callback, stop_words)
 
         # Prepare the prompt for the model
         prepared_prompt = tokenizer.apply_chat_template(
             messages, tokenize=False, chat_template=self.chat_template, add_generation_prompt=True
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/generators/chat/hugging_face_tgi.py` & `haystack_ai-2.2.0rc1/haystack/components/generators/chat/hugging_face_tgi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import warnings
 from dataclasses import asdict
 from typing import Any, Callable, Dict, Iterable, List, Optional
 from urllib.parse import urlparse
 
 from haystack import component, default_from_dict, default_to_dict, logging
 from haystack.dataclasses import ChatMessage, StreamingChunk
@@ -142,22 +146,25 @@
         self.url = url
         self.chat_template = chat_template
         self.token = token
         self.generation_kwargs = generation_kwargs
         self.client = InferenceClient(url or model, token=token.resolve_value() if token else None)
         self.streaming_callback = streaming_callback
         self.tokenizer = None
+        self._warmed_up: bool = False
 
     def warm_up(self) -> None:
         """
         Warm up the tokenizer by loading it from the model.
 
         If the url is not provided, check if the model is deployed on the free tier of the HF inference API.
         Load the tokenizer
         """
+        if self._warmed_up:
+            return
 
         # is this user using HF free tier inference API?
         if self.model and not self.url:
             deployed_models = list_inference_deployed_models()
             # Determine if the specified model is deployed in the free tier.
             if self.model not in deployed_models:
                 raise ValueError(
@@ -176,14 +183,16 @@
             logger.warning(
                 "The model '{model}' doesn't have a default chat_template, and no chat_template was supplied during "
                 "this component's initialization. It’s possible that the model doesn't support ChatML inference "
                 "format, potentially leading to unexpected behavior.",
                 model=self.model,
             )
 
+        self._warmed_up = True
+
     def to_dict(self) -> Dict[str, Any]:
         """
         Serialize this component to a dictionary.
 
         :return: A dictionary containing the serialized component.
         """
         callback_name = serialize_callable(self.streaming_callback) if self.streaming_callback else None
@@ -221,14 +230,18 @@
         """
         Invoke the text generation inference based on the provided messages and generation parameters.
 
         :param messages: A list of ChatMessage instances representing the input messages.
         :param generation_kwargs: Additional keyword arguments for text generation.
         :return: A list containing the generated responses as ChatMessage instances.
         """
+        if not self._warmed_up:
+            raise RuntimeError(
+                "The component HuggingFaceTGIChatGenerator was not warmed up. Please call warm_up() before running."
+            )
 
         # check generation kwargs given as parameters to override the default ones
         additional_params = ["n", "stop_words"]
         check_generation_params(generation_kwargs, additional_params)
 
         # update generation kwargs by merging with the default ones
         generation_kwargs = {**self.generation_kwargs, **(generation_kwargs or {})}
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/generators/chat/openai.py` & `haystack_ai-2.2.0rc1/haystack/components/generators/chat/openai.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,14 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import copy
 import json
+import os
 from typing import Any, Callable, Dict, List, Optional, Union
 
 from openai import OpenAI, Stream
 from openai.types.chat import ChatCompletion, ChatCompletionChunk, ChatCompletionMessage
 from openai.types.chat.chat_completion import Choice
 from openai.types.chat.chat_completion_chunk import Choice as ChunkChoice
 
@@ -67,21 +72,25 @@
         self,
         api_key: Secret = Secret.from_env_var("OPENAI_API_KEY"),
         model: str = "gpt-3.5-turbo",
         streaming_callback: Optional[Callable[[StreamingChunk], None]] = None,
         api_base_url: Optional[str] = None,
         organization: Optional[str] = None,
         generation_kwargs: Optional[Dict[str, Any]] = None,
+        timeout: Optional[float] = None,
+        max_retries: Optional[int] = None,
     ):
         """
         Initializes the OpenAIChatGenerator component.
 
         Creates an instance of OpenAIChatGenerator. Unless specified otherwise in the `model`, this is for OpenAI's
         GPT-3.5 model.
 
+        By setting the 'OPENAI_TIMEOUT' and 'OPENAI_MAX_RETRIES' you can change the timeout and max_retries parameters in the OpenAI client.
+
         :param api_key: The OpenAI API key.
         :param model: The name of the model to use.
         :param streaming_callback: A callback function that is called when a new token is received from the stream.
             The callback function accepts StreamingChunk as an argument.
         :param api_base_url: An optional base URL.
         :param organization: The Organization ID, defaults to `None`. See
         [production best practices](https://platform.openai.com/docs/guides/production-best-practices/setting-up-your-organization).
@@ -100,22 +109,38 @@
             - `stop`: One or more sequences after which the LLM should stop generating tokens.
             - `presence_penalty`: What penalty to apply if a token is already present at all. Bigger values mean
                 the model will be less likely to repeat the same token in the text.
             - `frequency_penalty`: What penalty to apply if a token has already been generated in the text.
                 Bigger values mean the model will be less likely to repeat the same token in the text.
             - `logit_bias`: Add a logit bias to specific tokens. The keys of the dictionary are tokens, and the
                 values are the bias to add to that token.
+        :param timeout:
+            Timeout for OpenAI Client calls, if not set it is inferred from the `OPENAI_TIMEOUT` environment variable or set to 30.
+        :param max_retries:
+            Maximum retries to stablish contact with OpenAI if it returns an internal error, if not set it is inferred from the `OPENAI_MAX_RETRIES` environment variable or set to 5.
         """
         self.api_key = api_key
         self.model = model
         self.generation_kwargs = generation_kwargs or {}
         self.streaming_callback = streaming_callback
         self.api_base_url = api_base_url
         self.organization = organization
-        self.client = OpenAI(api_key=api_key.resolve_value(), organization=organization, base_url=api_base_url)
+
+        if timeout is None:
+            timeout = float(os.environ.get("OPENAI_TIMEOUT", 30.0))
+        if max_retries is None:
+            max_retries = int(os.environ.get("OPENAI_MAX_RETRIES", 5))
+
+        self.client = OpenAI(
+            api_key=api_key.resolve_value(),
+            organization=organization,
+            base_url=api_base_url,
+            timeout=timeout,
+            max_retries=max_retries,
+        )
 
     def _get_telemetry_data(self) -> Dict[str, Any]:
         """
         Data that is sent to Posthog for usage analytics.
         """
         return {"model": self.model}
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/joiners/document_joiner.py` & `haystack_ai-2.2.0rc1/haystack/components/joiners/document_joiner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import itertools
 from collections import defaultdict
 from math import inf
 from typing import List, Optional
 
 from haystack import Document, component, logging
 from haystack.core.component.types import Variadic
@@ -66,20 +70,22 @@
             raise ValueError(f"DocumentJoiner component does not support '{join_mode}' join_mode.")
         self.join_mode = join_mode
         self.weights = [float(i) / sum(weights) for i in weights] if weights else None
         self.top_k = top_k
         self.sort_by_score = sort_by_score
 
     @component.output_types(documents=List[Document])
-    def run(self, documents: Variadic[List[Document]]):
+    def run(self, documents: Variadic[List[Document]], top_k: Optional[int] = None):
         """
         Joins multiple lists of Documents into a single list depending on the `join_mode` parameter.
 
         :param documents:
             List of list of Documents to be merged.
+        :param top_k:
+            The maximum number of Documents to return. Overrides the instance's `top_k` if provided.
 
         :returns:
             A dictionary with the following keys:
             - `documents`: Merged list of Documents
         """
         output_documents = []
         if self.join_mode == "concatenate":
@@ -95,16 +101,19 @@
             )
             if any(doc.score is None for doc in output_documents):
                 logger.info(
                     "Some of the Documents DocumentJoiner got have score=None. It was configured to sort Documents by "
                     "score, so those with score=None were sorted as if they had a score of -infinity."
                 )
 
-        if self.top_k:
+        if top_k:
+            output_documents = output_documents[:top_k]
+        elif self.top_k:
             output_documents = output_documents[: self.top_k]
+
         return {"documents": output_documents}
 
     def _concatenate(self, document_lists):
         """
         Concatenate multiple lists of Documents and return only the Document with the highest score for duplicate Documents.
         """
         output = []
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/others/multiplexer.py` & `haystack_ai-2.2.0rc1/haystack/components/others/multiplexer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,13 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import sys
+import warnings
 from typing import Any, Dict
 
 from haystack import component, default_from_dict, default_to_dict, logging
 from haystack.core.component.types import Variadic
 from haystack.utils import deserialize_type, serialize_type
 
 if sys.version_info < (3, 10):
@@ -95,14 +100,18 @@
     def __init__(self, type_: TypeAlias):
         """
         Create a `Multiplexer` component.
 
         :param type_: The type of data that the `Multiplexer` will receive from the upstream connected components and
                         distribute to the downstream connected components.
         """
+        warnings.warn(
+            "`Multiplexer` is deprecated and will be removed in Haystack 2.4.0. Use `joiners.BranchJoiner` instead.",
+            DeprecationWarning,
+        )
         self.type_ = type_
         component.set_input_types(self, value=Variadic[type_])
         component.set_output_types(self, value=type_)
 
     def to_dict(self):
         """
         Serializes the component to a dictionary.
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/preprocessors/document_cleaner.py` & `haystack_ai-2.2.0rc1/haystack/components/preprocessors/document_cleaner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import re
 from copy import deepcopy
 from functools import partial, reduce
 from itertools import chain
 from typing import Generator, List, Optional, Set
 
 from haystack import Document, component, logging
@@ -32,34 +36,37 @@
     """
 
     def __init__(
         self,
         remove_empty_lines: bool = True,
         remove_extra_whitespaces: bool = True,
         remove_repeated_substrings: bool = False,
+        keep_id: bool = False,
         remove_substrings: Optional[List[str]] = None,
         remove_regex: Optional[str] = None,
     ):
         """
         Initialize the DocumentCleaner.
 
         :param remove_empty_lines: Whether to remove empty lines.
         :param remove_extra_whitespaces: Whether to remove extra whitespaces.
         :param remove_repeated_substrings: Whether to remove repeated substrings (headers/footers) from pages.
             Pages in the text need to be separated by form feed character "\\f",
             which is supported by `TextFileToDocument` and `AzureOCRDocumentConverter`.
         :param remove_substrings: List of substrings to remove from the text.
         :param remove_regex: Regex to match and replace substrings by "".
+        :param keep_id: keep the ids of the original documents
         """
 
         self.remove_empty_lines = remove_empty_lines
         self.remove_extra_whitespaces = remove_extra_whitespaces
         self.remove_repeated_substrings = remove_repeated_substrings
         self.remove_substrings = remove_substrings
         self.remove_regex = remove_regex
+        self.keep_id = keep_id
 
     @component.output_types(documents=List[Document])
     def run(self, documents: List[Document]):
         """
         Cleans up the documents.
 
         :param documents: List of Documents to clean.
@@ -90,15 +97,15 @@
             if self.remove_substrings:
                 text = self._remove_substrings(text, self.remove_substrings)
             if self.remove_regex:
                 text = self._remove_regex(text, self.remove_regex)
             if self.remove_repeated_substrings:
                 text = self._remove_repeated_substrings(text)
 
-            cleaned_docs.append(Document(content=text, meta=deepcopy(doc.meta)))
+            cleaned_docs.append(Document(content=text, meta=deepcopy(doc.meta), id=doc.id if self.keep_id else ""))
 
         return {"documents": cleaned_docs}
 
     def _remove_empty_lines(self, text: str) -> str:
         """
         Remove empty lines and lines that contain nothing but whitespaces from text.
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/preprocessors/document_splitter.py` & `haystack_ai-2.2.0rc1/haystack/components/preprocessors/document_splitter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from copy import deepcopy
 from typing import Dict, List, Literal, Tuple
 
 from more_itertools import windowed
 
 from haystack import Document, component
 
@@ -17,33 +21,36 @@
     """
 
     def __init__(
         self,
         split_by: Literal["word", "sentence", "page", "passage"] = "word",
         split_length: int = 200,
         split_overlap: int = 0,
+        split_threshold: int = 0,
     ):
         """
         Initialize the DocumentSplitter.
 
         :param split_by: The unit by which the document should be split. Choose from "word" for splitting by " ",
             "sentence" for splitting by ".", "page" for splitting by "\\f" or "passage" for splitting by "\\n\\n".
         :param split_length: The maximum number of units in each split.
         :param split_overlap: The number of units that each split should overlap.
+        :param split_threshold: The minimum number of units that the split should have. If the split has fewer units than the threshold, it will be attached to the previous split.
         """
 
         self.split_by = split_by
         if split_by not in ["word", "sentence", "page", "passage"]:
             raise ValueError("split_by must be one of 'word', 'sentence', 'page' or 'passage'.")
         if split_length <= 0:
             raise ValueError("split_length must be greater than 0.")
         self.split_length = split_length
         if split_overlap < 0:
             raise ValueError("split_overlap must be greater than or equal to 0.")
         self.split_overlap = split_overlap
+        self.split_threshold = split_threshold
 
     @component.output_types(documents=List[Document])
     def run(self, documents: List[Document]):
         """
         Split documents into smaller parts.
 
         Splits documents by the unit expressed in `split_by`, with a length of `split_length`
@@ -66,15 +73,17 @@
         split_docs = []
         for doc in documents:
             if doc.content is None:
                 raise ValueError(
                     f"DocumentSplitter only works with text documents but document.content for document ID {doc.id} is None."
                 )
             units = self._split_into_units(doc.content, self.split_by)
-            text_splits, splits_pages = self._concatenate_units(units, self.split_length, self.split_overlap)
+            text_splits, splits_pages = self._concatenate_units(
+                units, self.split_length, self.split_overlap, self.split_threshold
+            )
             metadata = deepcopy(doc.meta)
             metadata["source_id"] = doc.id
             split_docs += self._create_docs_from_splits(
                 text_splits=text_splits, splits_pages=splits_pages, meta=metadata
             )
         return {"documents": split_docs}
 
@@ -94,35 +103,42 @@
         units = text.split(split_at)
         # Add the delimiter back to all units except the last one
         for i in range(len(units) - 1):
             units[i] += split_at
         return units
 
     def _concatenate_units(
-        self, elements: List[str], split_length: int, split_overlap: int
+        self, elements: List[str], split_length: int, split_overlap: int, split_threshold: int
     ) -> Tuple[List[str], List[int]]:
         """
         Concatenates the elements into parts of split_length units keeping track of the original page number that each element belongs.
+
+        If the length of the current units is less than the pre-defined `split_threshold`, it does not create a new split. Instead, it concatenates the current units with the last split, preventing the creation of excessively small splits.
         """
-        text_splits = []
+
+        text_splits: List[str] = []
         splits_pages = []
         cur_page = 1
         segments = windowed(elements, n=split_length, step=split_length - split_overlap)
         for seg in segments:
             current_units = [unit for unit in seg if unit is not None]
             txt = "".join(current_units)
-            if len(txt) > 0:
+            # check if length of current units is below split_threshold
+            if len(current_units) < split_threshold and len(text_splits) > 0:
+                # concatenate the last split with the current one
+                text_splits[-1] += txt
+            elif len(txt) > 0:
                 text_splits.append(txt)
                 splits_pages.append(cur_page)
-                processed_units = current_units[: split_length - split_overlap]
-                if self.split_by == "page":
-                    num_page_breaks = len(processed_units)
-                else:
-                    num_page_breaks = sum(processed_unit.count("\f") for processed_unit in processed_units)
-                cur_page += num_page_breaks
+            processed_units = current_units[: split_length - split_overlap]
+            if self.split_by == "page":
+                num_page_breaks = len(processed_units)
+            else:
+                num_page_breaks = sum(processed_unit.count("\f") for processed_unit in processed_units)
+            cur_page += num_page_breaks
         return text_splits, splits_pages
 
     @staticmethod
     def _create_docs_from_splits(text_splits: List[str], splits_pages: List[int], meta: Dict) -> List[Document]:
         """
         Creates Document objects from text splits enriching them with page number and the metadata of the original document.
         """
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/preprocessors/text_cleaner.py` & `haystack_ai-2.2.0rc1/haystack/components/preprocessors/text_cleaner.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import re
 import string
 from typing import Any, Dict, List, Optional
 
 from haystack import component
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/rankers/lost_in_the_middle.py` & `haystack_ai-2.2.0rc1/haystack/components/rankers/lost_in_the_middle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from typing import Dict, List, Optional
 
 from haystack import Document, component
 
 
 @component
 class LostInTheMiddleRanker:
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/rankers/meta_field.py` & `haystack_ai-2.2.0rc1/haystack/components/rankers/meta_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from collections import defaultdict
 from typing import Any, Callable, Dict, List, Literal, Optional
 
 from dateutil.parser import parse as date_parse
 
 from haystack import Document, component, logging
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/rankers/sentence_transformers_diversity.py` & `haystack_ai-2.2.0rc1/haystack/components/rankers/sentence_transformers_diversity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from typing import Any, Dict, List, Literal, Optional
 
-from haystack import ComponentError, Document, component, default_from_dict, default_to_dict, logging
+from haystack import Document, component, default_from_dict, default_to_dict, logging
 from haystack.lazy_imports import LazyImport
 from haystack.utils import ComponentDevice, Secret, deserialize_secrets_inplace
 
 logger = logging.getLogger(__name__)
 
 
 with LazyImport(message="Run 'pip install \"sentence-transformers>=2.2.0\"'") as torch_and_sentence_transformers_import:
@@ -223,26 +227,27 @@
         :param documents: List of Document objects to be ranker.
         :param top_k: Optional. An integer to override the top_k set during initialization.
 
         :returns: A dictionary with the following key:
             - `documents`: List of Document objects that have been selected based on the diversity ranking.
 
         :raises ValueError: If the top_k value is less than or equal to 0.
+        :raises RuntimeError: If the component has not been warmed up.
         """
+        if self.model is None:
+            error_msg = (
+                "The component SentenceTransformersDiversityRanker wasn't warmed up. "
+                "Run 'warm_up()' before calling 'run()'."
+            )
+            raise RuntimeError(error_msg)
+
         if not documents:
             return {"documents": []}
 
         if top_k is None:
             top_k = self.top_k
         elif top_k <= 0:
             raise ValueError(f"top_k must be > 0, but got {top_k}")
 
-        if self.model is None:
-            error_msg = (
-                "The component SentenceTransformersDiversityRanker wasn't warmed up. "
-                "Run 'warm_up()' before calling 'run()'."
-            )
-            raise ComponentError(error_msg)
-
         diversity_sorted = self._greedy_diversity_order(query=query, documents=documents)
 
         return {"documents": diversity_sorted[:top_k]}
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/rankers/transformers_similarity.py` & `haystack_ai-2.2.0rc1/haystack/components/rankers/transformers_similarity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 
-from haystack import ComponentError, Document, component, default_from_dict, default_to_dict, logging
+from haystack import Document, component, default_from_dict, default_to_dict, logging
 from haystack.lazy_imports import LazyImport
 from haystack.utils import ComponentDevice, DeviceMap, Secret, deserialize_secrets_inplace
 from haystack.utils.hf import deserialize_hf_model_kwargs, resolve_hf_device_map, serialize_hf_model_kwargs
 
 logger = logging.getLogger(__name__)
 
 
@@ -210,17 +214,23 @@
         :returns:
             A dictionary with the following keys:
             - `documents`: List of Documents most similar to the given query in descending order of similarity.
 
         :raises ValueError:
             If `top_k` is not > 0.
             If `scale_score` is True and `calibration_factor` is not provided.
-        :raises ComponentError:
+        :raises RuntimeError:
             If the model is not loaded because `warm_up()` was not called before.
         """
+        # If a model path is provided but the model isn't loaded
+        if self.model is None:
+            raise RuntimeError(
+                "The component TransformersSimilarityRanker wasn't warmed up. Run 'warm_up()' before calling 'run()'."
+            )
+
         if not documents:
             return {"documents": []}
 
         top_k = top_k or self.top_k
         scale_score = scale_score or self.scale_score
         calibration_factor = calibration_factor or self.calibration_factor
         score_threshold = score_threshold or self.score_threshold
@@ -229,20 +239,14 @@
             raise ValueError(f"top_k must be > 0, but got {top_k}")
 
         if scale_score and calibration_factor is None:
             raise ValueError(
                 f"scale_score is True so calibration_factor must be provided, but got {calibration_factor}"
             )
 
-        # If a model path is provided but the model isn't loaded
-        if self.model is None:
-            raise ComponentError(
-                f"The component {self.__class__.__name__} wasn't warmed up. Run 'warm_up()' before calling 'run()'."
-            )
-
         query_doc_pairs = []
         for doc in documents:
             meta_values_to_embed = [
                 str(doc.meta[key]) for key in self.meta_fields_to_embed if key in doc.meta and doc.meta[key]
             ]
             text_to_embed = self.embedding_separator.join(meta_values_to_embed + [doc.content or ""])
             query_doc_pairs.append([self.query_prefix + query, self.document_prefix + text_to_embed])
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/readers/extractive.py` & `haystack_ai-2.2.0rc1/haystack/components/readers/extractive.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import math
 import warnings
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union
 
-from haystack import ComponentError, Document, ExtractedAnswer, component, default_from_dict, default_to_dict, logging
+from haystack import Document, ExtractedAnswer, component, default_from_dict, default_to_dict, logging
 from haystack.lazy_imports import LazyImport
 from haystack.utils import ComponentDevice, DeviceMap, Secret, deserialize_secrets_inplace
 from haystack.utils.hf import deserialize_hf_model_kwargs, resolve_hf_device_map, serialize_hf_model_kwargs
 
 with LazyImport("Run 'pip install transformers[torch,sentencepiece]'") as torch_and_transformers_import:
     import accelerate  # pylint: disable=unused-import # the library is used but not directly referenced
     import torch
@@ -202,26 +206,29 @@
         self, queries: List[str], documents: List[Document], max_seq_length: int, query_ids: List[int], stride: int
     ) -> Tuple["torch.Tensor", "torch.Tensor", "torch.Tensor", List["Encoding"], List[int], List[int]]:
         """
         Splits and tokenizes Documents and preserves structures by returning mappings to query and Document IDs.
         """
         texts = []
         document_ids = []
+        document_contents = []
         for i, doc in enumerate(documents):
             if doc.content is None:
                 warnings.warn(
                     f"Document with id {doc.id} was passed to ExtractiveReader. The Document doesn't "
                     f"contain any text and it will be ignored."
                 )
                 continue
             texts.append(doc.content)
             document_ids.append(i)
+            document_contents.append(doc.content)
+
         encodings_pt = self.tokenizer(  # type: ignore
             queries,
-            [document.content for document in documents],
+            document_contents,
             padding=True,
             truncation=True,
             max_length=max_seq_length,
             return_tensors="pt",
             return_overflowing_tokens=True,
             stride=stride,
         )
@@ -560,22 +567,27 @@
             one of these answers since the second answer has a 100% (1.0) overlap with the first answer.
             However, for the answers "the river in" and "in Maine" there is only a max overlap percentage of 25% so
             both of these answers could be kept if this variable is set to 0.24 or lower.
             If None is provided then all answers are kept.
         :returns:
             List of answers sorted by (desc.) answer score.
 
-        :raises ComponentError:
+        :raises RuntimeError:
             If the component was not warmed up by calling 'warm_up()' before.
         """
-        queries = [query]  # Temporary solution until we have decided what batching should look like in v2
-        nested_documents = [documents]
         if self.model is None:
-            raise ComponentError("The component was not warmed up. Run 'warm_up()' before calling 'run()'.")
+            raise RuntimeError(
+                "The component ExtractiveReader was not warmed up. Run 'warm_up()' before calling 'run()'."
+            )
+
+        if not documents:
+            return {"answers": []}
 
+        queries = [query]  # Temporary solution until we have decided what batching should look like in v2
+        nested_documents = [documents]
         top_k = top_k or self.top_k
         score_threshold = score_threshold or self.score_threshold
         max_seq_length = max_seq_length or self.max_seq_length
         stride = stride or self.stride
         max_batch_size = max_batch_size or self.max_batch_size
         answers_per_seq = answers_per_seq or self.answers_per_seq or 20
         no_answer = no_answer if no_answer is not None else self.no_answer
@@ -594,15 +606,16 @@
 
         for i in range(num_batches):
             start_index = i * batch_size
             end_index = start_index + batch_size
             cur_input_ids = input_ids[start_index:end_index]
             cur_attention_mask = attention_mask[start_index:end_index]
 
-            output = self.model(input_ids=cur_input_ids, attention_mask=cur_attention_mask)
+            with torch.inference_mode():
+                output = self.model(input_ids=cur_input_ids, attention_mask=cur_attention_mask)
             cur_start_logits = output.start_logits
             cur_end_logits = output.end_logits
             if num_batches != 1:
                 cur_start_logits = cur_start_logits.cpu()
                 cur_end_logits = cur_end_logits.cpu()
             start_logits_list.append(cur_start_logits)
             end_logits_list.append(cur_end_logits)
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/retrievers/filter_retriever.py` & `haystack_ai-2.2.0rc1/haystack/components/retrievers/filter_retriever.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import importlib
 from typing import Any, Dict, List, Optional
 
 from haystack import DeserializationError, Document, component, default_from_dict, default_to_dict, logging
 from haystack.document_stores.types import DocumentStore
 
 logger = logging.getLogger(__name__)
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/retrievers/in_memory/bm25_retriever.py` & `haystack_ai-2.2.0rc1/haystack/components/retrievers/in_memory/bm25_retriever.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from typing import Any, Dict, List, Optional
 
 from haystack import DeserializationError, Document, component, default_from_dict, default_to_dict
 from haystack.document_stores.in_memory import InMemoryDocumentStore
 
 
 @component
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/retrievers/in_memory/embedding_retriever.py` & `haystack_ai-2.2.0rc1/haystack/components/retrievers/in_memory/embedding_retriever.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from typing import Any, Dict, List, Optional
 
 from haystack import DeserializationError, Document, component, default_from_dict, default_to_dict
 from haystack.document_stores.in_memory import InMemoryDocumentStore
 
 
 @component
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/routers/conditional_router.py` & `haystack_ai-2.2.0rc1/haystack/components/routers/conditional_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from typing import Any, Dict, List, Set
 
 from jinja2 import Environment, TemplateSyntaxError, meta
 from jinja2.nativetypes import NativeEnvironment
 
 from haystack import component, default_from_dict, default_to_dict, logging
 from haystack.utils import deserialize_type, serialize_type
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/routers/file_type_router.py` & `haystack_ai-2.2.0rc1/haystack/components/routers/file_type_router.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import mimetypes
 import re
 from collections import defaultdict
 from pathlib import Path
 from typing import Dict, List, Optional, Union
 
 from haystack import component, logging
@@ -82,15 +86,15 @@
         mime_types = defaultdict(list)
         for source in sources:
             if isinstance(source, str):
                 source = Path(source)
             if isinstance(source, Path):
                 mime_type = self._get_mime_type(source)
             elif isinstance(source, ByteStream):
-                mime_type = source.meta.get("content_type", None)
+                mime_type = source.mime_type
             else:
                 raise ValueError(f"Unsupported data source type: {type(source).__name__}")
 
             matched = False
             if mime_type:
                 for pattern in self.mime_type_patterns:
                     if pattern.fullmatch(mime_type):
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/routers/metadata_router.py` & `haystack_ai-2.2.0rc1/haystack/components/routers/metadata_router.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from typing import Dict, List
 
 from haystack import Document, component
 from haystack.utils.filters import convert, document_matches_filter
 
 
 @component
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/routers/text_language_router.py` & `haystack_ai-2.2.0rc1/haystack/components/routers/text_language_router.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from typing import Dict, List, Optional
 
 from haystack import component, logging
 from haystack.lazy_imports import LazyImport
 
 logger = logging.getLogger(__name__)
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/routers/zero_shot_text_router.py` & `haystack_ai-2.2.0rc1/haystack/components/routers/zero_shot_text_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from typing import Any, Dict, List, Optional
 
 from haystack import component, default_from_dict, default_to_dict, logging
 from haystack.lazy_imports import LazyImport
 from haystack.utils import ComponentDevice, Secret, deserialize_secrets_inplace
 
 logger = logging.getLogger(__name__)
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/samplers/top_p.py` & `haystack_ai-2.2.0rc1/haystack/components/samplers/top_p.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from typing import List, Optional
 
 from haystack import ComponentError, Document, component, logging
 from haystack.lazy_imports import LazyImport
 
 logger = logging.getLogger(__name__)
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/validators/json_schema.py` & `haystack_ai-2.2.0rc1/haystack/components/validators/json_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import json
 from typing import Any, Dict, List, Optional
 
 from haystack import component
 from haystack.dataclasses import ChatMessage
 from haystack.lazy_imports import LazyImport
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/websearch/searchapi.py` & `haystack_ai-2.2.0rc1/haystack/components/websearch/searchapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from typing import Any, Dict, List, Optional, Union
 
 import requests
 
 from haystack import ComponentError, Document, component, default_from_dict, default_to_dict, logging
 from haystack.utils import Secret, deserialize_secrets_inplace
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/websearch/serper_dev.py` & `haystack_ai-2.2.0rc1/haystack/components/websearch/serper_dev.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import json
 from typing import Any, Dict, List, Optional, Union
 
 import requests
 
 from haystack import ComponentError, Document, component, default_from_dict, default_to_dict, logging
 from haystack.utils import Secret, deserialize_secrets_inplace
@@ -116,15 +120,15 @@
             raise SerperDevError(f"An error occurred while querying {self.__class__.__name__}. Error: {e}") from e
 
         # If we reached this point, it means the request was successful and we can proceed
         json_result = response.json()
 
         # we get the snippet from the json result and put it in the content field of the document
         organic = [
-            Document(meta={k: v for k, v in d.items() if k != "snippet"}, content=d["snippet"])
+            Document(meta={k: v for k, v in d.items() if k != "snippet"}, content=d.get("snippet"))
             for d in json_result["organic"]
         ]
 
         # answer box is what search engine shows as a direct answer to the query
         answer_box = []
         if "answerBox" in json_result:
             answer_dict = json_result["answerBox"]
```

### Comparing `haystack_ai-2.1.2rc1/haystack/components/writers/document_writer.py` & `haystack_ai-2.2.0rc1/haystack/components/writers/document_writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import importlib
 from typing import Any, Dict, List, Optional
 
 from haystack import DeserializationError, Document, component, default_from_dict, default_to_dict, logging
 from haystack.document_stores.types import DocumentStore, DuplicatePolicy
 
 logger = logging.getLogger(__name__)
```

### Comparing `haystack_ai-2.1.2rc1/haystack/core/errors.py` & `haystack_ai-2.2.0rc1/haystack/core/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
+
+
 class PipelineError(Exception):
     pass
 
 
 class PipelineRuntimeError(Exception):
     pass
```

### Comparing `haystack_ai-2.1.2rc1/haystack/core/serialization.py` & `haystack_ai-2.2.0rc1/haystack/core/serialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
+
 import inspect
 from collections.abc import Callable
 from dataclasses import dataclass
 from typing import Any, Dict, Optional, Type
 
 from haystack.core.component.component import _hook_component_init
 from haystack.core.errors import DeserializationError, SerializationError
```

### Comparing `haystack_ai-2.1.2rc1/haystack/core/type_utils.py` & `haystack_ai-2.2.0rc1/haystack/core/type_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
+
 from typing import Any, Union, get_args, get_origin
 
 from haystack import logging
 
 logger = logging.getLogger(__name__)
```

### Comparing `haystack_ai-2.1.2rc1/haystack/core/component/component.py` & `haystack_ai-2.2.0rc1/haystack/core/component/component.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
+
 """
     Attributes:
 
         component: Marks a class as a component. Any class decorated with `@component` can be used by a Pipeline.
 
     All components must follow the contract below. This docstring is the source of truth for components contract.
```

### Comparing `haystack_ai-2.1.2rc1/haystack/core/component/sockets.py` & `haystack_ai-2.2.0rc1/haystack/core/component/sockets.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.2rc1/haystack/core/component/types.py` & `haystack_ai-2.2.0rc1/haystack/core/component/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from dataclasses import dataclass, field
 from typing import Any, Iterable, List, Type, TypeVar, get_args
 
 from typing_extensions import Annotated, TypeAlias  # Python 3.8 compatibility
 
 HAYSTACK_VARIADIC_ANNOTATION = "__haystack__variadic_t"
```

### Comparing `haystack_ai-2.1.2rc1/haystack/core/pipeline/descriptions.py` & `haystack_ai-2.2.0rc1/haystack/core/pipeline/descriptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
+
 from typing import Dict, List
 
 import networkx  # type:ignore
 
 from haystack import logging
 from haystack.core.component.types import InputSocket, OutputSocket
 from haystack.core.type_utils import _type_name
@@ -12,16 +13,17 @@
 logger = logging.getLogger(__name__)
 
 
 def find_pipeline_inputs(
     graph: networkx.MultiDiGraph, include_connected_sockets: bool = False
 ) -> Dict[str, List[InputSocket]]:
     """
-    Collect components that have disconnected/connected input sockets. Note that this method returns *ALL*
-    disconnected input sockets, including all such sockets with default values.
+    Collect components that have disconnected/connected input sockets.
+
+    Note that this method returns *ALL* disconnected input sockets, including all such sockets with default values.
     """
     return {
         name: [
             socket
             for socket in data.get("input_sockets", {}).values()
             if socket.is_variadic or (include_connected_sockets or not socket.senders)
         ]
```

### Comparing `haystack_ai-2.1.2rc1/haystack/core/pipeline/draw.py` & `haystack_ai-2.2.0rc1/haystack/core/pipeline/draw.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
+
 import base64
 
 import networkx  # type:ignore
 import requests
 
 from haystack import logging
 from haystack.core.errors import PipelineDrawingError
```

### Comparing `haystack_ai-2.1.2rc1/haystack/core/pipeline/template.py` & `haystack_ai-2.2.0rc1/haystack/core/pipeline/template.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from enum import Enum
 from pathlib import Path
 from typing import Any, Dict, Optional, Union
 
 from jinja2 import Environment, PackageLoader, TemplateSyntaxError, meta
 
 TEMPLATE_FILE_EXTENSION = ".yaml.jinja2"
```

### Comparing `haystack_ai-2.1.2rc1/haystack/core/pipeline/predefined/chat_with_website.yaml.jinja2` & `haystack_ai-2.2.0rc1/haystack/core/pipeline/predefined/chat_with_website.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.2rc1/haystack/core/pipeline/predefined/generative_qa.yaml.jinja2` & `haystack_ai-2.2.0rc1/haystack/core/pipeline/predefined/generative_qa.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.2rc1/haystack/core/pipeline/predefined/indexing.yaml.jinja2` & `haystack_ai-2.2.0rc1/haystack/core/pipeline/predefined/indexing.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.2rc1/haystack/core/pipeline/predefined/rag.yaml.jinja2` & `haystack_ai-2.2.0rc1/haystack/core/pipeline/predefined/rag.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.2rc1/haystack/dataclasses/answer.py` & `haystack_ai-2.2.0rc1/haystack/dataclasses/answer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import io
 from dataclasses import asdict, dataclass, field
 from typing import Any, Dict, List, Optional, Protocol, runtime_checkable
 
 from pandas import DataFrame, read_json
 
 from haystack.core.serialization import default_from_dict, default_to_dict
```

### Comparing `haystack_ai-2.1.2rc1/haystack/dataclasses/byte_stream.py` & `haystack_ai-2.2.0rc1/haystack/dataclasses/byte_stream.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Any, Dict, Optional
 
 
 @dataclass
 class ByteStream:
```

### Comparing `haystack_ai-2.1.2rc1/haystack/dataclasses/chat_message.py` & `haystack_ai-2.2.0rc1/haystack/dataclasses/chat_message.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from dataclasses import dataclass, field
 from enum import Enum
 from typing import Any, Dict, Optional
 
 
 class ChatRole(str, Enum):
     """Enumeration representing the roles within a chat."""
```

### Comparing `haystack_ai-2.1.2rc1/haystack/dataclasses/document.py` & `haystack_ai-2.2.0rc1/haystack/dataclasses/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import hashlib
 import io
 from dataclasses import asdict, dataclass, field, fields
 from typing import Any, Dict, List, Optional
 
 from numpy import ndarray
 from pandas import DataFrame, read_json
```

### Comparing `haystack_ai-2.1.2rc1/haystack/dataclasses/sparse_embedding.py` & `haystack_ai-2.2.0rc1/haystack/dataclasses/sparse_embedding.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.2rc1/haystack/document_stores/in_memory/document_store.py` & `haystack_ai-2.2.0rc1/haystack/document_stores/in_memory/document_store.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,18 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
+import math
 import re
-from typing import Any, Dict, Iterable, List, Literal, Optional
+from collections import Counter
+from dataclasses import dataclass
+from typing import Any, Dict, Iterable, List, Literal, Optional, Tuple
 
 import numpy as np
-from haystack_bm25 import rank_bm25
-from tqdm.auto import tqdm
 
 from haystack import default_from_dict, default_to_dict, logging
 from haystack.dataclasses import Document
 from haystack.document_stores.errors import DocumentStoreError, DuplicateDocumentError
 from haystack.document_stores.types import DuplicatePolicy
 from haystack.utils import expit
 from haystack.utils.filters import convert, document_matches_filter
@@ -20,14 +25,27 @@
 # Larger scaling factor decreases scaled scores. For example, an input of 10 is scaled to 0.99 with BM25_SCALING_FACTOR=2
 # but to 0.78 with BM25_SCALING_FACTOR=8 (default). The defaults were chosen empirically. Increase the default if most
 # unscaled scores are larger than expected (>30) and otherwise would incorrectly all be mapped to scores ~1.
 BM25_SCALING_FACTOR = 8
 DOT_PRODUCT_SCALING_FACTOR = 100
 
 
+@dataclass
+class BM25DocumentStats:
+    """
+    A dataclass for managing document statistics for BM25 retrieval.
+
+    :param freq_token: A Counter of token frequencies in the document.
+    :param doc_len: Number of tokens in the document.
+    """
+
+    freq_token: Dict[str, int]
+    doc_len: int
+
+
 class InMemoryDocumentStore:
     """
     Stores data in-memory. It's ephemeral and cannot be saved to disk.
     """
 
     def __init__(
         self,
@@ -46,34 +64,225 @@
                                 You can learn more about these parameters by visiting https://github.com/dorianbrown/rank_bm25.
                                 By default, no parameters are set.
         :param embedding_similarity_function: The similarity function used to compare Documents embeddings.
                                               One of "dot_product" (default) or "cosine".
                                               To choose the most appropriate function, look for information about your embedding model.
         """
         self.storage: Dict[str, Document] = {}
-        self._bm25_tokenization_regex = bm25_tokenization_regex
+        self.bm25_tokenization_regex = bm25_tokenization_regex
         self.tokenizer = re.compile(bm25_tokenization_regex).findall
-        algorithm_class = getattr(rank_bm25, bm25_algorithm)
-        if algorithm_class is None:
-            raise ValueError(f"BM25 algorithm '{bm25_algorithm}' not found.")
-        self.bm25_algorithm = algorithm_class
+
+        self.bm25_algorithm = bm25_algorithm
+        self.bm25_algorithm_inst = self._dispatch_bm25()
         self.bm25_parameters = bm25_parameters or {}
         self.embedding_similarity_function = embedding_similarity_function
 
+        # Global BM25 statistics
+        self._avg_doc_len: float = 0.0
+        self._freq_vocab_for_idf: Counter = Counter()
+
+        # Per-document statistics
+        self._bm25_attr: Dict[str, BM25DocumentStats] = {}
+
+    def _dispatch_bm25(self):
+        """
+        Select the correct BM25 algorithm based on user specification.
+
+        :returns:
+            The BM25 algorithm method.
+        """
+        table = {"BM25Okapi": self._score_bm25okapi, "BM25L": self._score_bm25l, "BM25Plus": self._score_bm25plus}
+
+        if self.bm25_algorithm not in table:
+            raise ValueError(f"BM25 algorithm '{self.bm25_algorithm}' is not supported.")
+        return table[self.bm25_algorithm]
+
+    def _tokenize_bm25(self, text: str) -> List[str]:
+        """
+        Tokenize text using the BM25 tokenization regex.
+
+        Here we explicitly create a tokenization method to encapsulate
+        all pre-processing logic used to create BM25 tokens, such as
+        lowercasing. This helps track the exact tokenization process
+        used for BM25 scoring at any given time.
+
+        :param text:
+            The text to tokenize.
+        :returns:
+            A list of tokens.
+        """
+        text = text.lower()
+        return self.tokenizer(text)
+
+    def _score_bm25l(self, query: str, documents: List[Document]) -> List[Tuple[Document, float]]:
+        """
+        Calculate BM25L scores for the given query and filtered documents.
+
+        :param query:
+            The query string.
+        :param documents:
+            The list of documents to score, should be produced by
+            the filter_documents method; may be an empty list.
+        :returns:
+            A list of tuples, each containing a Document and its BM25L score.
+        """
+        k = self.bm25_parameters.get("k1", 1.5)
+        b = self.bm25_parameters.get("b", 0.75)
+        delta = self.bm25_parameters.get("delta", 0.5)
+
+        def _compute_idf(tokens: List[str]) -> Dict[str, float]:
+            """Per-token IDF computation for all tokens."""
+            idf = {}
+            n_corpus = len(self._bm25_attr)
+            for tok in tokens:
+                n = self._freq_vocab_for_idf.get(tok, 0)
+                idf[tok] = math.log((n_corpus + 1.0) / (n + 0.5)) * int(n != 0)
+            return idf
+
+        def _compute_tf(token: str, freq: Dict[str, int], doc_len: int) -> float:
+            """Per-token BM25L computation."""
+            freq_term = freq.get(token, 0.0)
+            ctd = freq_term / (1 - b + b * doc_len / self._avg_doc_len)
+            return (1.0 + k) * (ctd + delta) / (k + ctd + delta)
+
+        idf = _compute_idf(self._tokenize_bm25(query))
+        bm25_attr = {doc.id: self._bm25_attr[doc.id] for doc in documents}
+
+        ret = []
+        for doc in documents:
+            doc_stats = bm25_attr[doc.id]
+            freq = doc_stats.freq_token
+            doc_len = doc_stats.doc_len
+
+            score = 0.0
+            for tok in idf.keys():  # pylint: disable=consider-using-dict-items
+                score += idf[tok] * _compute_tf(tok, freq, doc_len)
+            ret.append((doc, score))
+
+        return ret
+
+    def _score_bm25okapi(self, query: str, documents: List[Document]) -> List[Tuple[Document, float]]:
+        """
+        Calculate BM25Okapi scores for the given query and filtered documents.
+
+        :param query:
+            The query string.
+        :param documents:
+            The list of documents to score, should be produced by
+            the filter_documents method; may be an empty list.
+        :returns:
+            A list of tuples, each containing a Document and its BM25L score.
+        """
+        k = self.bm25_parameters.get("k1", 1.5)
+        b = self.bm25_parameters.get("b", 0.75)
+        epsilon = self.bm25_parameters.get("epsilon", 0.25)
+
+        def _compute_idf(tokens: List[str]) -> Dict[str, float]:
+            """Per-token IDF computation for all tokens."""
+            sum_idf = 0.0
+            neg_idf_tokens = []
+
+            # Although this is a global statistic, we compute it here
+            # to make the computation more self-contained. And the
+            # complexity is O(vocab_size), which is acceptable.
+            idf = {}
+            for tok, n in self._freq_vocab_for_idf.items():
+                idf[tok] = math.log((len(self._bm25_attr) - n + 0.5) / (n + 0.5))
+                sum_idf += idf[tok]
+                if idf[tok] < 0:
+                    neg_idf_tokens.append(tok)
+
+            eps = epsilon * sum_idf / len(self._freq_vocab_for_idf)
+            for tok in neg_idf_tokens:
+                idf[tok] = eps
+            return {tok: idf.get(tok, 0.0) for tok in tokens}
+
+        def _compute_tf(token: str, freq: Dict[str, int], doc_len: int) -> float:
+            """Per-token BM25L computation."""
+            freq_term = freq.get(token, 0.0)
+            freq_norm = freq_term + k * (1 - b + b * doc_len / self._avg_doc_len)
+            return freq_term * (1.0 + k) / freq_norm
+
+        idf = _compute_idf(self._tokenize_bm25(query))
+        bm25_attr = {doc.id: self._bm25_attr[doc.id] for doc in documents}
+
+        ret = []
+        for doc in documents:
+            doc_stats = bm25_attr[doc.id]
+            freq = doc_stats.freq_token
+            doc_len = doc_stats.doc_len
+
+            score = 0.0
+            for tok in idf.keys():
+                score += idf[tok] * _compute_tf(tok, freq, doc_len)
+            ret.append((doc, score))
+
+        return ret
+
+    def _score_bm25plus(self, query: str, documents: List[Document]) -> List[Tuple[Document, float]]:
+        """
+        Calculate BM25+ scores for the given query and filtered documents.
+
+        This implementation follows the document on BM25 Wikipedia page,
+        which add 1 (smoothing factor) to document frequency when computing IDF.
+
+        :param query:
+            The query string.
+        :param documents:
+            The list of documents to score, should be produced by
+            the filter_documents method; may be an empty list.
+        :returns:
+            A list of tuples, each containing a Document and its BM25+ score.
+        """
+        k = self.bm25_parameters.get("k1", 1.5)
+        b = self.bm25_parameters.get("b", 0.75)
+        delta = self.bm25_parameters.get("delta", 1.0)
+
+        def _compute_idf(tokens: List[str]) -> Dict[str, float]:
+            """Per-token IDF computation."""
+            idf = {}
+            n_corpus = len(self._bm25_attr)
+            for tok in tokens:
+                n = self._freq_vocab_for_idf.get(tok, 0)
+                idf[tok] = math.log(1 + (n_corpus - n + 0.5) / (n + 0.5)) * int(n != 0)
+            return idf
+
+        def _compute_tf(token: str, freq: Dict[str, int], doc_len: float) -> float:
+            """Per-token normalized term frequency."""
+            freq_term = freq.get(token, 0.0)
+            freq_damp = k * (1 - b + b * doc_len / self._avg_doc_len)
+            return freq_term * (1.0 + k) / (freq_term + freq_damp) + delta
+
+        idf = _compute_idf(self._tokenize_bm25(query))
+        bm25_attr = {doc.id: self._bm25_attr[doc.id] for doc in documents}
+
+        ret = []
+        for doc in documents:
+            doc_stats = bm25_attr[doc.id]
+            freq = doc_stats.freq_token
+            doc_len = doc_stats.doc_len
+
+            score = 0.0
+            for tok in idf.keys():  # pylint: disable=consider-using-dict-items
+                score += idf[tok] * _compute_tf(tok, freq, doc_len)
+            ret.append((doc, score))
+
+        return ret
+
     def to_dict(self) -> Dict[str, Any]:
         """
         Serializes the component to a dictionary.
 
         :returns:
             Dictionary with serialized data.
         """
         return default_to_dict(
             self,
-            bm25_tokenization_regex=self._bm25_tokenization_regex,
-            bm25_algorithm=self.bm25_algorithm.__name__,
+            bm25_tokenization_regex=self.bm25_tokenization_regex,
+            bm25_algorithm=self.bm25_algorithm,
             bm25_parameters=self.bm25_parameters,
             embedding_similarity_function=self.embedding_similarity_function,
         )
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> "InMemoryDocumentStore":
         """
@@ -128,28 +337,68 @@
             if policy != DuplicatePolicy.OVERWRITE and document.id in self.storage.keys():
                 if policy == DuplicatePolicy.FAIL:
                     raise DuplicateDocumentError(f"ID '{document.id}' already exists.")
                 if policy == DuplicatePolicy.SKIP:
                     logger.warning("ID '{document_id}' already exists", document_id=document.id)
                     written_documents -= 1
                     continue
+
+            # Since the statistics are updated in an incremental manner,
+            # we need to explicitly remove the existing document to revert
+            # the statistics before updating them with the new document.
+            if document.id in self.storage.keys():
+                self.delete_documents([document.id])
+
+            # This processing logic is extracted from the original bm25_retrieval method.
+            # Since we are creating index incrementally before the first retrieval,
+            # we need to determine what content to use for indexing here, not at query time.
+            if document.content is not None:
+                if document.dataframe is not None:
+                    logger.warning(
+                        "Document '{document_id}' has both text and dataframe content. "
+                        "Using text content for retrieval and skipping dataframe content.",
+                        document_id=document.id,
+                    )
+                tokens = self._tokenize_bm25(document.content)
+            elif document.dataframe is not None:
+                str_content = document.dataframe.astype(str)
+                csv_content = str_content.to_csv(index=False)
+                tokens = self._tokenize_bm25(csv_content)
+            else:
+                tokens = []
+
             self.storage[document.id] = document
+
+            self._bm25_attr[document.id] = BM25DocumentStats(Counter(tokens), len(tokens))
+            self._freq_vocab_for_idf.update(set(tokens))
+            self._avg_doc_len = (len(tokens) + self._avg_doc_len * len(self._bm25_attr)) / (len(self._bm25_attr) + 1)
         return written_documents
 
     def delete_documents(self, document_ids: List[str]) -> None:
         """
         Deletes all documents with matching document_ids from the DocumentStore.
 
         :param document_ids: The object_ids to delete.
         """
         for doc_id in document_ids:
             if doc_id not in self.storage.keys():
                 continue
             del self.storage[doc_id]
 
+            # Update statistics accordingly
+            doc_stats = self._bm25_attr.pop(doc_id)
+            freq = doc_stats.freq_token
+            doc_len = doc_stats.doc_len
+
+            self._freq_vocab_for_idf.subtract(Counter(freq.keys()))
+            try:
+                self._avg_doc_len = (self._avg_doc_len * (len(self._bm25_attr) + 1) - doc_len) / len(self._bm25_attr)
+            except ZeroDivisionError:
+                self._avg_doc_len = 0
+
     def bm25_retrieval(
         self, query: str, filters: Optional[Dict[str, Any]] = None, top_k: int = 10, scale_score: bool = False
     ) -> List[Document]:
         """
         Retrieves documents that are most relevant to the query using BM25 algorithm.
 
         :param query: The query string.
@@ -170,73 +419,41 @@
         }
         if filters:
             if "operator" not in filters:
                 filters = convert(filters)
             filters = {"operator": "AND", "conditions": [content_type_filter, filters]}
         else:
             filters = content_type_filter
-        all_documents = self.filter_documents(filters=filters)
 
-        # Lowercase all documents
-        lower_case_documents = []
-        for doc in all_documents:
-            if doc.content is None and doc.dataframe is None:
-                logger.info(
-                    "Document '{document_id}' has no text or dataframe content. Skipping it.", document_id=doc.id
-                )
-            else:
-                if doc.content is not None:
-                    lower_case_documents.append(doc.content.lower())
-                    if doc.dataframe is not None:
-                        logger.warning(
-                            "Document '{document_id}' has both text and dataframe content. "
-                            "Using text content and skipping dataframe content.",
-                            document_id=doc.id,
-                        )
-                        continue
-                if doc.dataframe is not None:
-                    str_content = doc.dataframe.astype(str)
-                    csv_content = str_content.to_csv(index=False)
-                    lower_case_documents.append(csv_content.lower())
-
-        # Tokenize the entire content of the DocumentStore
-        tokenized_corpus = [
-            self.tokenizer(doc) for doc in tqdm(lower_case_documents, unit=" docs", desc="Ranking by BM25...")
-        ]
-        if len(tokenized_corpus) == 0:
+        all_documents = self.filter_documents(filters=filters)
+        if len(all_documents) == 0:
             logger.info("No documents found for BM25 retrieval. Returning empty list.")
             return []
 
-        # initialize BM25
-        bm25_scorer = self.bm25_algorithm(tokenized_corpus, **self.bm25_parameters)
-        # tokenize query
-        tokenized_query = self.tokenizer(query.lower())
-        # get scores for the query against the corpus
-        docs_scores = bm25_scorer.get_scores(tokenized_query)
-        if scale_score:
-            docs_scores = [expit(float(score / BM25_SCALING_FACTOR)) for score in docs_scores]
-        # get the last top_k indexes and reverse them
-        top_docs_positions = np.argsort(docs_scores)[-top_k:][::-1]
+        results = sorted(self.bm25_algorithm_inst(query, all_documents), key=lambda x: x[1], reverse=True)[:top_k]
 
         # BM25Okapi can return meaningful negative values, so they should not be filtered out when scale_score is False.
         # It's the only algorithm supported by rank_bm25 at the time of writing (2024) that can return negative scores.
         # see https://github.com/deepset-ai/haystack/pull/6889 for more context.
-        negatives_are_valid = self.bm25_algorithm is rank_bm25.BM25Okapi and not scale_score
+        negatives_are_valid = self.bm25_algorithm == "BM25Okapi" and not scale_score
 
         # Create documents with the BM25 score to return them
         return_documents = []
-        for i in top_docs_positions:
-            doc = all_documents[i]
-            score = docs_scores[i]
+        for doc, score in results:
+            if scale_score:
+                score = expit(score / BM25_SCALING_FACTOR)
+
             if not negatives_are_valid and score <= 0.0:
                 continue
+
             doc_fields = doc.to_dict()
             doc_fields["score"] = score
             return_document = Document.from_dict(doc_fields)
             return_documents.append(return_document)
+
         return return_documents
 
     def embedding_retrieval(
         self,
         query_embedding: List[float],
         filters: Optional[Dict[str, Any]] = None,
         top_k: int = 10,
```

### Comparing `haystack_ai-2.1.2rc1/haystack/document_stores/types/protocol.py` & `haystack_ai-2.2.0rc1/haystack/document_stores/types/protocol.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from typing import Any, Dict, List, Optional, Protocol
 
 from haystack import logging
 from haystack.dataclasses import Document
 from haystack.document_stores.types.policy import DuplicatePolicy
 
 # Ellipsis are needed for the type checker, it's safe to disable module-wide
```

### Comparing `haystack_ai-2.1.2rc1/haystack/evaluation/eval_run_result.py` & `haystack_ai-2.2.0rc1/haystack/evaluation/eval_run_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from abc import ABC, abstractmethod
 from copy import deepcopy
 from typing import Any, Dict, List
 from warnings import warn
 
 from pandas import DataFrame
 from pandas import concat as pd_concat
```

### Comparing `haystack_ai-2.1.2rc1/haystack/telemetry/_environment.py` & `haystack_ai-2.2.0rc1/haystack/telemetry/_environment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-# pylint: disable=global-statement
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import os
 import platform
 import sys
 from typing import Any, Dict, Optional
 
 from haystack import logging
 from haystack.version import __version__
 
 logger = logging.getLogger(__name__)
 
-
 # This value cannot change during the lifetime of the process
 _IS_DOCKER_CACHE = None
 
 
 def _in_podman() -> bool:
     """
     Check if the code is running in a Podman container.
@@ -52,15 +54,15 @@
     return os.path.isfile(path) and any("/docker/containers/" in line for line in open(path))
 
 
 def _is_containerized() -> Optional[bool]:
     """
     This code is based on the popular 'is-docker' package for node.js
     """
-    global _IS_DOCKER_CACHE
+    global _IS_DOCKER_CACHE  # pylint: disable=global-statement
 
     if _IS_DOCKER_CACHE is None:
         _IS_DOCKER_CACHE = _in_podman() or _has_dockerenv() or _has_docker_cgroup_v1() or _has_docker_cgroup_v2()
 
     return _IS_DOCKER_CACHE
```

### Comparing `haystack_ai-2.1.2rc1/haystack/telemetry/_telemetry.py` & `haystack_ai-2.2.0rc1/haystack/telemetry/_telemetry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import datetime
 import logging
 import os
 import uuid
 from collections import defaultdict
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple
```

### Comparing `haystack_ai-2.1.2rc1/haystack/testing/document_store.py` & `haystack_ai-2.2.0rc1/haystack/testing/document_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-# pylint: disable=too-many-public-methods
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import random
 from datetime import datetime
 from typing import List
 
 import pandas as pd
 
 from haystack.dataclasses import Document
@@ -15,14 +18,17 @@
     import pytest
 
 
 def _random_embeddings(n):
     return [random.random() for _ in range(n)]
 
 
+# pylint: disable=too-many-public-methods
+
+
 # These are random embedding that are used to test filters.
 # We declare them here as they're used both in the `filterable_docs` fixture
 # and the body of several `filter_documents` tests.
 TEST_EMBEDDING_1 = _random_embeddings(768)
 TEST_EMBEDDING_2 = _random_embeddings(768)
```

### Comparing `haystack_ai-2.1.2rc1/haystack/testing/factory.py` & `haystack_ai-2.2.0rc1/haystack/testing/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
 from haystack.core.component import Component, component
 from haystack.core.serialization import default_from_dict, default_to_dict
 from haystack.dataclasses import Document
 from haystack.document_stores.types import DocumentStore, DuplicatePolicy
```

### Comparing `haystack_ai-2.1.2rc1/haystack/testing/sample_components/__init__.py` & `haystack_ai-2.2.0rc1/haystack/testing/sample_components/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
+
 from haystack.testing.sample_components.accumulate import Accumulate
 from haystack.testing.sample_components.add_value import AddFixedValue
 from haystack.testing.sample_components.concatenate import Concatenate
 from haystack.testing.sample_components.double import Double
 from haystack.testing.sample_components.fstring import FString
 from haystack.testing.sample_components.greet import Greet
 from haystack.testing.sample_components.hello import Hello
```

### Comparing `haystack_ai-2.1.2rc1/haystack/testing/sample_components/accumulate.py` & `haystack_ai-2.2.0rc1/haystack/testing/sample_components/accumulate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
+
 import builtins
 import sys
 from importlib import import_module
 from typing import Any, Callable, Dict, Optional
 
 from haystack.core.component import component
 from haystack.core.errors import ComponentDeserializationError
```

### Comparing `haystack_ai-2.1.2rc1/haystack/testing/sample_components/add_value.py` & `haystack_ai-2.2.0rc1/haystack/testing/sample_components/add_value.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
+
 from typing import Optional
 
 from haystack.core.component import component
 
 
 @component
 class AddFixedValue:
```

### Comparing `haystack_ai-2.1.2rc1/haystack/testing/sample_components/concatenate.py` & `haystack_ai-2.2.0rc1/haystack/testing/sample_components/concatenate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
+
 from typing import List, Union
 
 from haystack.core.component import component
 
 
 @component
 class Concatenate:
```

### Comparing `haystack_ai-2.1.2rc1/haystack/testing/sample_components/fstring.py` & `haystack_ai-2.2.0rc1/haystack/testing/sample_components/fstring.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
+
 from typing import Any, List, Optional
 
 from haystack.core.component import component
 
 
 @component
 class FString:
```

### Comparing `haystack_ai-2.1.2rc1/haystack/testing/sample_components/greet.py` & `haystack_ai-2.2.0rc1/haystack/testing/sample_components/greet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
+
 import logging
 from typing import Optional
 
 import haystack.logging as haystack_logging
 from haystack.core.component import component
 
 logger = haystack_logging.getLogger(__name__)
```

### Comparing `haystack_ai-2.1.2rc1/haystack/testing/sample_components/joiner.py` & `haystack_ai-2.2.0rc1/haystack/testing/sample_components/joiner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
+
 from typing import List
 
 from haystack.core.component import component
 from haystack.core.component.types import Variadic
 
 
 @component
```

### Comparing `haystack_ai-2.1.2rc1/haystack/testing/sample_components/parity.py` & `haystack_ai-2.2.0rc1/haystack/testing/sample_components/parity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
+
 from haystack.core.component import component
 
 
 @component
 class Parity:  # pylint: disable=too-few-public-methods
     """
     Redirects the value, unchanged, along the 'even' connection if even, or along the 'odd' one if odd.
```

### Comparing `haystack_ai-2.1.2rc1/haystack/testing/sample_components/remainder.py` & `haystack_ai-2.2.0rc1/haystack/testing/sample_components/remainder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
+
 from haystack.core.component import component
 
 
 @component
 class Remainder:
     def __init__(self, divisor=3):
         if divisor == 0:
```

### Comparing `haystack_ai-2.1.2rc1/haystack/testing/sample_components/subtract.py` & `haystack_ai-2.2.0rc1/haystack/testing/sample_components/subtract.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
+
 from haystack.core.component import component
 
 
 @component
 class Subtract:
     """
     Compute the difference between two values.
```

### Comparing `haystack_ai-2.1.2rc1/haystack/testing/sample_components/threshold.py` & `haystack_ai-2.2.0rc1/haystack/testing/sample_components/threshold.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
+
 from typing import Optional
 
 from haystack.core.component import component
 
 
 @component
 class Threshold:  # pylint: disable=too-few-public-methods
```

### Comparing `haystack_ai-2.1.2rc1/haystack/tracing/datadog.py` & `haystack_ai-2.2.0rc1/haystack/tracing/datadog.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import contextlib
 from typing import Any, Dict, Iterator, Optional
 
 from haystack.lazy_imports import LazyImport
 from haystack.tracing import Span, Tracer
 from haystack.tracing import utils as tracing_utils
```

### Comparing `haystack_ai-2.1.2rc1/haystack/tracing/opentelemetry.py` & `haystack_ai-2.2.0rc1/haystack/tracing/opentelemetry.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import contextlib
 from typing import Any, Dict, Iterator, Optional
 
 from haystack.lazy_imports import LazyImport
 from haystack.tracing import Span, Tracer
 from haystack.tracing import utils as tracing_utils
```

### Comparing `haystack_ai-2.1.2rc1/haystack/tracing/tracer.py` & `haystack_ai-2.2.0rc1/haystack/tracing/tracer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import abc
 import contextlib
 import os
 from typing import Any, Dict, Iterator, Optional
 
 from haystack import logging
```

### Comparing `haystack_ai-2.1.2rc1/haystack/tracing/utils.py` & `haystack_ai-2.2.0rc1/haystack/tracing/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import json
 from typing import Any, Union
 
 from haystack import logging
 
 logger = logging.getLogger(__name__)
```

### Comparing `haystack_ai-2.1.2rc1/haystack/utils/__init__.py` & `haystack_ai-2.2.0rc1/haystack/utils/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from .auth import Secret, deserialize_secrets_inplace
 from .callable_serialization import deserialize_callable, serialize_callable
 from .device import ComponentDevice, Device, DeviceMap, DeviceType
 from .expit import expit
 from .filters import document_matches_filter
 from .jupyter import is_in_jupyter
 from .requests_utils import request_with_retry
```

### Comparing `haystack_ai-2.1.2rc1/haystack/utils/auth.py` & `haystack_ai-2.2.0rc1/haystack/utils/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import os
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from enum import Enum
 from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
```

### Comparing `haystack_ai-2.1.2rc1/haystack/utils/callable_serialization.py` & `haystack_ai-2.2.0rc1/haystack/utils/callable_serialization.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import inspect
 import sys
 from typing import Callable, Optional
 
 from haystack import DeserializationError
```

### Comparing `haystack_ai-2.1.2rc1/haystack/utils/device.py` & `haystack_ai-2.2.0rc1/haystack/utils/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import os
 from dataclasses import dataclass, field
 from enum import Enum
 from typing import Any, Dict, Optional, Tuple, Union
 
 from haystack import logging
 from haystack.lazy_imports import LazyImport
```

### Comparing `haystack_ai-2.1.2rc1/haystack/utils/filters.py` & `haystack_ai-2.2.0rc1/haystack/utils/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from dataclasses import fields
 from datetime import datetime
 from typing import Any, Dict, List, Union
 
 import pandas as pd
 
 from haystack.dataclasses import Document
```

### Comparing `haystack_ai-2.1.2rc1/haystack/utils/hf.py` & `haystack_ai-2.2.0rc1/haystack/utils/hf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import copy
 import inspect
 from enum import Enum
 from typing import Any, Callable, Dict, List, Optional, Union
 
 import requests
```

### Comparing `haystack_ai-2.1.2rc1/haystack/utils/jupyter.py` & `haystack_ai-2.2.0rc1/haystack/utils/jupyter.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.2rc1/haystack/utils/requests_utils.py` & `haystack_ai-2.2.0rc1/haystack/utils/requests_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import logging
 from typing import List, Optional
 
 import requests
 from tenacity import after_log, before_log, retry, retry_if_exception_type, stop_after_attempt, wait_exponential
 
 logger = logging.getLogger(__file__)
```

### Comparing `haystack_ai-2.1.2rc1/haystack/utils/type_serialization.py` & `haystack_ai-2.2.0rc1/haystack/utils/type_serialization.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+
 import importlib
 import inspect
 import sys
 import typing
 from typing import Any, get_args, get_origin
 
 from haystack import DeserializationError
```

### Comparing `haystack_ai-2.1.2rc1/.gitignore` & `haystack_ai-2.2.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.2rc1/LICENSE` & `haystack_ai-2.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.2rc1/README.md` & `haystack_ai-2.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.2rc1/pyproject.toml` & `haystack_ai-2.2.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -43,38 +43,38 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dependencies = [
   "pandas",
-  "haystack-bm25",
   "tqdm",
   "tenacity",
   "lazy-imports",
   "openai>=1.1.0",
   "Jinja2",
   "posthog",  # telemetry
   "pyyaml",
   "more-itertools",  # TextDocumentSplitter
   "networkx", # Pipeline graphs
   "typing_extensions>=4.7", # typing support for Python 3.8
-  "boilerpy3", # Fulltext extraction from HTML pages
+  "trafilatura", # Fulltext extraction from HTML pages
   "requests",
   "numpy",
   "python-dateutil",
 ]
 
 [tool.hatch.envs.default]
 dependencies = [
   "pre-commit",
   # Type check
   "mypy",
   # Test
   "pytest",
+  "pytest-bdd",
   "pytest-cov",
   "pytest-custom_exit_code",  # used in the CI
   "pytest-asyncio",
   "pytest-rerunfailures",
   "responses",
   "tox",
   "coverage",
```

### Comparing `haystack_ai-2.1.2rc1/PKG-INFO` & `haystack_ai-2.2.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: haystack-ai
-Version: 2.1.2rc1
+Version: 2.2.0rc1
 Summary: LLM framework to build customizable, production-ready LLM applications. Connect components (models, vector DBs, file converters) to pipelines or agents that can interact with your data.
 Project-URL: CI: GitHub, https://github.com/deepset-ai/haystack/actions
 Project-URL: Docs: RTD, https://haystack.deepset.ai/overview/intro
 Project-URL: GitHub: issues, https://github.com/deepset-ai/haystack/issues
 Project-URL: GitHub: repo, https://github.com/deepset-ai/haystack
 Project-URL: Homepage, https://github.com/deepset-ai/haystack
 Author-email: "deepset.ai" <malte.pietsch@deepset.ai>
@@ -19,29 +19,28 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
-Requires-Dist: boilerpy3
-Requires-Dist: haystack-bm25
 Requires-Dist: jinja2
 Requires-Dist: lazy-imports
 Requires-Dist: more-itertools
 Requires-Dist: networkx
 Requires-Dist: numpy
 Requires-Dist: openai>=1.1.0
 Requires-Dist: pandas
 Requires-Dist: posthog
 Requires-Dist: python-dateutil
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Requires-Dist: tenacity
 Requires-Dist: tqdm
+Requires-Dist: trafilatura
 Requires-Dist: typing-extensions>=4.7
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://haystack.deepset.ai/"><img src="https://github.com/deepset-ai/haystack/blob/main/docs/img/banner_20.png" alt="Green logo of a stylized white 'H' with the text 'Haystack, by deepset. Haystack 2.0 is live 🎉' Abstract green and yellow diagrams in the background."></a>
 
 |         |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: haystack-ai Version: 2.1.2rc1 Summary: LLM
+Metadata-Version: 2.3 Name: haystack-ai Version: 2.2.0rc1 Summary: LLM
 framework to build customizable, production-ready LLM applications. Connect
 components (models, vector DBs, file converters) to pipelines or agents that
 can interact with your data. Project-URL: CI: GitHub, https://github.com/
 deepset-ai/haystack/actions Project-URL: Docs: RTD, https://
 haystack.deepset.ai/overview/intro Project-URL: GitHub: issues, https://
 github.com/deepset-ai/haystack/issues Project-URL: GitHub: repo, https://
 github.com/deepset-ai/haystack Project-URL: Homepage, https://github.com/
@@ -14,20 +14,20 @@
 Audience :: Science/Research Classifier: License :: Freely Distributable
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
-Requires-Dist: boilerpy3 Requires-Dist: haystack-bm25 Requires-Dist: jinja2
-Requires-Dist: lazy-imports Requires-Dist: more-itertools Requires-Dist:
-networkx Requires-Dist: numpy Requires-Dist: openai>=1.1.0 Requires-Dist:
-pandas Requires-Dist: posthog Requires-Dist: python-dateutil Requires-Dist:
-pyyaml Requires-Dist: requests Requires-Dist: tenacity Requires-Dist: tqdm
-Requires-Dist: typing-extensions>=4.7 Description-Content-Type: text/markdown
+Requires-Dist: jinja2 Requires-Dist: lazy-imports Requires-Dist: more-itertools
+Requires-Dist: networkx Requires-Dist: numpy Requires-Dist: openai>=1.1.0
+Requires-Dist: pandas Requires-Dist: posthog Requires-Dist: python-dateutil
+Requires-Dist: pyyaml Requires-Dist: requests Requires-Dist: tenacity Requires-
+Dist: tqdm Requires-Dist: trafilatura Requires-Dist: typing-extensions>=4.7
+Description-Content-Type: text/markdown
    _[_G_r_e_e_n_ _l_o_g_o_ _o_f_ _a_ _s_t_y_l_i_z_e_d_ _w_h_i_t_e_ _'_H_'_ _w_i_t_h_ _t_h_e_ _t_e_x_t_ _'_H_a_y_s_t_a_c_k_,_ _b_y_ _d_e_e_p_s_e_t_.
      _H_a_y_s_t_a_c_k_ _2_._0_ _i_s_ _l_i_v_e_ _ð____'_Â_ _A_b_s_t_r_a_c_t_ _g_r_e_e_n_ _a_n_d_ _y_e_l_l_o_w_ _d_i_a_g_r_a_m_s_ _i_n_ _t_h_e
 _b_a_c_k_g_r_o_u_n_d_._]| | | | ------- | -------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
```

