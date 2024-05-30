# Comparing `tmp/langfun-0.0.2.dev20240528.tar.gz` & `tmp/langfun-0.0.2.dev20240529.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langfun-0.0.2.dev20240528.tar", last modified: Tue May 28 08:04:07 2024, max compression
+gzip compressed data, was "langfun-0.0.2.dev20240529.tar", last modified: Wed May 29 08:04:27 2024, max compression
```

## Comparing `langfun-0.0.2.dev20240528.tar` & `langfun-0.0.2.dev20240529.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:04:07.176238 langfun-0.0.2.dev20240528/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-28 08:04:07.172238 langfun-0.0.2.dev20240528/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:04:07.156238 langfun-0.0.2.dev20240528/langfun/
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:04:07.160238 langfun-0.0.2.dev20240528/langfun/core/
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:04:07.160238 langfun-0.0.2.dev20240528/langfun/core/coding/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/coding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:04:07.164238 langfun-0.0.2.dev20240528/langfun/core/coding/python/
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/coding/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/coding/python/correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/coding/python/correction_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/coding/python/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/coding/python/errors_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/coding/python/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/coding/python/execution_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/coding/python/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/coding/python/generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/coding/python/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/coding/python/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/coding/python/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/coding/python/permissions_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/component_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/concurrent_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/console_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:04:07.164238 langfun-0.0.2.dev20240528/langfun/core/eval/
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    74268 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/eval/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    26743 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/eval/base_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/eval/matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/eval/matching_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/eval/patching.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/eval/patching_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/eval/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/eval/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11060 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/langfunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/langfunc_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    20760 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/language_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    20122 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/language_model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:04:07.168238 langfun-0.0.2.dev20240528/langfun/core/llms/
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/llms/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/llms/anthropic_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:04:07.168238 langfun-0.0.2.dev20240528/langfun/core/llms/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/llms/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/llms/cache/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/llms/cache/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/llms/cache/in_memory_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/llms/fake.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/llms/fake_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/llms/google_genai.py
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/llms/google_genai_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/llms/groq.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/llms/groq_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/llms/llama_cpp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/llms/llama_cpp_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13657 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/llms/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    14854 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/llms/openai_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9921 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/llms/vertexai.py
--rw-r--r--   0 runner    (1001) docker     (127)     7641 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/llms/vertexai_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:04:07.168238 langfun-0.0.2.dev20240528/langfun/core/memories/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/memories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/memories/conversation_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/memories/conversation_history_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/message_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:04:07.168238 langfun-0.0.2.dev20240528/langfun/core/modalities/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/modalities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/modalities/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/modalities/image_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/modalities/mime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/modalities/mime_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/modalities/pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/modalities/pdf_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/modalities/video.py
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/modalities/video_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/modality.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/modality_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/natural_language.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/natural_language_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/sampling_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:04:07.172238 langfun-0.0.2.dev20240528/langfun/core/structured/
--rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/structured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/structured/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)    19273 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/structured/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/structured/description.py
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/structured/description_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/structured/function_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/structured/function_generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/structured/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/structured/mapping_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/structured/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    20895 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/structured/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/structured/prompting.py
--rw-r--r--   0 runner    (1001) docker     (127)    21700 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/structured/prompting_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    25967 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/structured/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/structured/schema_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/structured/schema_generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    23318 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/structured/schema_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/structured/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/structured/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/subscription_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22284 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    15464 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/template_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:04:07.172238 langfun-0.0.2.dev20240528/langfun/core/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/templates/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/templates/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/templates/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/templates/conversation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/templates/demonstration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/templates/demonstration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/templates/selfplay.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/templates/selfplay_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/text_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/langfun/core/text_formatting_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:04:07.172238 langfun-0.0.2.dev20240528/langfun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-28 08:04:07.000000 langfun-0.0.2.dev20240528/langfun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-28 08:04:07.000000 langfun-0.0.2.dev20240528/langfun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 08:04:07.000000 langfun-0.0.2.dev20240528/langfun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-28 08:04:07.000000 langfun-0.0.2.dev20240528/langfun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-28 08:04:07.000000 langfun-0.0.2.dev20240528/langfun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 08:04:07.176238 langfun-0.0.2.dev20240528/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-28 08:03:32.000000 langfun-0.0.2.dev20240528/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:04:27.852230 langfun-0.0.2.dev20240529/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-29 08:04:27.852230 langfun-0.0.2.dev20240529/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:04:27.832230 langfun-0.0.2.dev20240529/langfun/
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:04:27.836230 langfun-0.0.2.dev20240529/langfun/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:04:27.836230 langfun-0.0.2.dev20240529/langfun/core/coding/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/coding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:04:27.840230 langfun-0.0.2.dev20240529/langfun/core/coding/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/coding/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/coding/python/correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/coding/python/correction_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/coding/python/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/coding/python/errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/coding/python/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/coding/python/execution_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/coding/python/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/coding/python/generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/coding/python/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/coding/python/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/coding/python/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/coding/python/permissions_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/component_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/concurrent_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/console_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:04:27.840230 langfun-0.0.2.dev20240529/langfun/core/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74268 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/eval/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26743 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/eval/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/eval/matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/eval/matching_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/eval/patching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/eval/patching_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/eval/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/eval/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11060 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/langfunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/langfunc_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20760 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/language_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20137 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/language_model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:04:27.844230 langfun-0.0.2.dev20240529/langfun/core/llms/
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/llms/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/llms/anthropic_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:04:27.844230 langfun-0.0.2.dev20240529/langfun/core/llms/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/llms/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/llms/cache/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/llms/cache/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/llms/cache/in_memory_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/llms/fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/llms/fake_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/llms/google_genai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7529 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/llms/google_genai_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/llms/groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/llms/groq_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/llms/llama_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/llms/llama_cpp_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13657 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/llms/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14858 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/llms/openai_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9921 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/llms/vertexai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/llms/vertexai_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:04:27.844230 langfun-0.0.2.dev20240529/langfun/core/memories/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/memories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/memories/conversation_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/memories/conversation_history_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15738 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9574 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/message_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:04:27.848230 langfun-0.0.2.dev20240529/langfun/core/modalities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/modalities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/modalities/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/modalities/image_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/modalities/mime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/modalities/mime_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/modalities/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/modalities/pdf_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/modalities/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/modalities/video_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/modality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/modality_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/natural_language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/natural_language_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/sampling_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:04:27.852230 langfun-0.0.2.dev20240529/langfun/core/structured/
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/structured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/structured/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19281 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/structured/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/structured/description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/structured/description_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/structured/function_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/structured/function_generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/structured/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/structured/mapping_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/structured/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20895 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/structured/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/structured/prompting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21756 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/structured/prompting_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25967 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/structured/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/structured/schema_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/structured/schema_generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23318 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/structured/schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/structured/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/structured/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/subscription_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22284 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15468 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/template_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:04:27.852230 langfun-0.0.2.dev20240529/langfun/core/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/templates/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/templates/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/templates/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/templates/conversation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/templates/demonstration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/templates/demonstration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/templates/selfplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/templates/selfplay_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/text_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/langfun/core/text_formatting_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:04:27.852230 langfun-0.0.2.dev20240529/langfun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-29 08:04:27.000000 langfun-0.0.2.dev20240529/langfun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-29 08:04:27.000000 langfun-0.0.2.dev20240529/langfun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 08:04:27.000000 langfun-0.0.2.dev20240529/langfun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-29 08:04:27.000000 langfun-0.0.2.dev20240529/langfun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-29 08:04:27.000000 langfun-0.0.2.dev20240529/langfun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 08:04:27.852230 langfun-0.0.2.dev20240529/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-29 08:03:58.000000 langfun-0.0.2.dev20240529/setup.py
```

### Comparing `langfun-0.0.2.dev20240528/LICENSE` & `langfun-0.0.2.dev20240529/LICENSE`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/PKG-INFO` & `langfun-0.0.2.dev20240529/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240528
+Version: 0.0.2.dev20240529
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langfun-0.0.2.dev20240528/README.md` & `langfun-0.0.2.dev20240529/README.md`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/__init__.py` & `langfun-0.0.2.dev20240529/langfun/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/__init__.py` & `langfun-0.0.2.dev20240529/langfun/core/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/coding/__init__.py` & `langfun-0.0.2.dev20240529/langfun/core/coding/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/coding/python/__init__.py` & `langfun-0.0.2.dev20240529/langfun/core/coding/python/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/coding/python/correction.py` & `langfun-0.0.2.dev20240529/langfun/core/coding/python/correction.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/coding/python/correction_test.py` & `langfun-0.0.2.dev20240529/langfun/core/coding/python/correction_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/coding/python/errors.py` & `langfun-0.0.2.dev20240529/langfun/core/coding/python/errors.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/coding/python/errors_test.py` & `langfun-0.0.2.dev20240529/langfun/core/coding/python/errors_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/coding/python/execution.py` & `langfun-0.0.2.dev20240529/langfun/core/coding/python/execution.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/coding/python/execution_test.py` & `langfun-0.0.2.dev20240529/langfun/core/coding/python/execution_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/coding/python/generation.py` & `langfun-0.0.2.dev20240529/langfun/core/coding/python/generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/coding/python/generation_test.py` & `langfun-0.0.2.dev20240529/langfun/core/coding/python/generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/coding/python/parsing.py` & `langfun-0.0.2.dev20240529/langfun/core/coding/python/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/coding/python/parsing_test.py` & `langfun-0.0.2.dev20240529/langfun/core/coding/python/parsing_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/coding/python/permissions.py` & `langfun-0.0.2.dev20240529/langfun/core/coding/python/permissions.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/coding/python/permissions_test.py` & `langfun-0.0.2.dev20240529/langfun/core/coding/python/permissions_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/component.py` & `langfun-0.0.2.dev20240529/langfun/core/component.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/component_test.py` & `langfun-0.0.2.dev20240529/langfun/core/component_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/concurrent.py` & `langfun-0.0.2.dev20240529/langfun/core/concurrent.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/concurrent_test.py` & `langfun-0.0.2.dev20240529/langfun/core/concurrent_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/console.py` & `langfun-0.0.2.dev20240529/langfun/core/console.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/console_test.py` & `langfun-0.0.2.dev20240529/langfun/core/console_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/eval/__init__.py` & `langfun-0.0.2.dev20240529/langfun/core/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/eval/base.py` & `langfun-0.0.2.dev20240529/langfun/core/eval/base.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/eval/base_test.py` & `langfun-0.0.2.dev20240529/langfun/core/eval/base_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/eval/matching.py` & `langfun-0.0.2.dev20240529/langfun/core/eval/matching.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/eval/matching_test.py` & `langfun-0.0.2.dev20240529/langfun/core/eval/matching_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/eval/patching.py` & `langfun-0.0.2.dev20240529/langfun/core/eval/patching.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/eval/patching_test.py` & `langfun-0.0.2.dev20240529/langfun/core/eval/patching_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/eval/scoring.py` & `langfun-0.0.2.dev20240529/langfun/core/eval/scoring.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/eval/scoring_test.py` & `langfun-0.0.2.dev20240529/langfun/core/eval/scoring_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/langfunc.py` & `langfun-0.0.2.dev20240529/langfun/core/langfunc.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/langfunc_test.py` & `langfun-0.0.2.dev20240529/langfun/core/langfunc_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/language_model.py` & `langfun-0.0.2.dev20240529/langfun/core/language_model.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/language_model_test.py` & `langfun-0.0.2.dev20240529/langfun/core/language_model_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -414,16 +414,17 @@
         return b'fake_image'
 
     string_io = io.StringIO()
     lm = MockModel(sampling_options=lm_lib.LMSamplingOptions(top_k=1))
     with contextlib.redirect_stdout(string_io):
       self.assertEqual(
           lm(message_lib.UserMessage(
-              'hi {{image}}', image=Image()), debug=True),
-          'hi {{image}}')
+              'hi <<[[image]]>>', image=Image()), debug=True),
+          'hi <<[[image]]>>'
+      )
 
     debug_info = string_io.getvalue()
     self.assertIn('[0] LM INFO', debug_info)
     self.assertIn('[0] PROMPT SENT TO LM', debug_info)
     self.assertIn('[0] MODALITY OBJECTS SENT TO LM', debug_info)
     self.assertIn('[0] LM RESPONSE', debug_info)
```

### Comparing `langfun-0.0.2.dev20240528/langfun/core/llms/__init__.py` & `langfun-0.0.2.dev20240529/langfun/core/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/llms/anthropic.py` & `langfun-0.0.2.dev20240529/langfun/core/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/llms/anthropic_test.py` & `langfun-0.0.2.dev20240529/langfun/core/llms/anthropic_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/llms/cache/__init__.py` & `langfun-0.0.2.dev20240529/langfun/core/llms/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/llms/cache/base.py` & `langfun-0.0.2.dev20240529/langfun/core/llms/cache/base.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/llms/cache/in_memory.py` & `langfun-0.0.2.dev20240529/langfun/core/llms/cache/in_memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/llms/cache/in_memory_test.py` & `langfun-0.0.2.dev20240529/langfun/core/llms/cache/in_memory_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/llms/fake.py` & `langfun-0.0.2.dev20240529/langfun/core/llms/fake.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/llms/fake_test.py` & `langfun-0.0.2.dev20240529/langfun/core/llms/fake_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/llms/google_genai.py` & `langfun-0.0.2.dev20240529/langfun/core/llms/google_genai.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/llms/google_genai_test.py` & `langfun-0.0.2.dev20240529/langfun/core/llms/google_genai_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     text = 'This is a beautiful day'
     model = google_genai.GeminiPro()
     chunks = model._content_from_message(lf.UserMessage(text))
     self.assertEqual(chunks, [text])
 
   def test_content_from_message_mm(self):
     message = lf.UserMessage(
-        'This is an {{image}}, what is it?',
+        'This is an <<[[image]]>>, what is it?',
         image=lf_modalities.Image.from_bytes(example_image),
     )
 
     # Non-multimodal model.
     with self.assertRaisesRegex(ValueError, 'Unsupported modality'):
       google_genai.GeminiPro()._content_from_message(message)
```

### Comparing `langfun-0.0.2.dev20240528/langfun/core/llms/groq.py` & `langfun-0.0.2.dev20240529/langfun/core/llms/groq.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/llms/groq_test.py` & `langfun-0.0.2.dev20240529/langfun/core/llms/groq_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/llms/llama_cpp.py` & `langfun-0.0.2.dev20240529/langfun/core/llms/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/llms/llama_cpp_test.py` & `langfun-0.0.2.dev20240529/langfun/core/llms/llama_cpp_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/llms/openai.py` & `langfun-0.0.2.dev20240529/langfun/core/llms/openai.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/llms/openai_test.py` & `langfun-0.0.2.dev20240529/langfun/core/llms/openai_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
       mock_chat_completion.side_effect = mock_chat_completion_query_vision
       lm_1 = openai.Gpt4Turbo(api_key='test_key')
       lm_2 = openai.Gpt4VisionPreview(api_key='test_key')
       for lm in (lm_1, lm_2):
         self.assertEqual(
             lm(
                 lf.UserMessage(
-                    'hello {{image}}',
+                    'hello <<[[image]]>>',
                     image=lf_modalities.Image.from_uri('https://fake/image')
                 ),
                 sampling_options=lf.LMSamplingOptions(n=2)
             ),
             'Sample 0 for message: https://fake/image',
         )
```

### Comparing `langfun-0.0.2.dev20240528/langfun/core/llms/vertexai.py` & `langfun-0.0.2.dev20240529/langfun/core/llms/vertexai.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/llms/vertexai_test.py` & `langfun-0.0.2.dev20240529/langfun/core/llms/vertexai_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     text = 'This is a beautiful day'
     model = vertexai.VertexAIGeminiPro1()
     chunks = model._content_from_message(lf.UserMessage(text))
     self.assertEqual(chunks, [text])
 
   def test_content_from_message_mm(self):
     message = lf.UserMessage(
-        'This is an {{image}}, what is it?',
+        'This is an <<[[image]]>>, what is it?',
         image=lf_modalities.Image.from_bytes(example_image),
     )
 
     # Non-multimodal model.
     with self.assertRaisesRegex(ValueError, 'Unsupported modality'):
       vertexai.VertexAIGeminiPro1()._content_from_message(message)
```

### Comparing `langfun-0.0.2.dev20240528/langfun/core/memories/__init__.py` & `langfun-0.0.2.dev20240529/langfun/core/memories/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/memories/conversation_history.py` & `langfun-0.0.2.dev20240529/langfun/core/memories/conversation_history.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/memories/conversation_history_test.py` & `langfun-0.0.2.dev20240529/langfun/core/memories/conversation_history_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/memory.py` & `langfun-0.0.2.dev20240529/langfun/core/memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/message.py` & `langfun-0.0.2.dev20240529/langfun/core/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
     )
     self._source = source
 
   @classmethod
   def from_value(cls, value: Union[str, 'Message']) -> 'Message':
     """Creates a message from a value or return value itself if a Message."""
     if isinstance(value, modality.Modality):
-      return cls('{{object}}', object=value)
+      return cls('<<[[object]]>>', object=value)
     if isinstance(value, Message):
       return value
     return cls(value)
 
   #
   # Unified interface for accessing text, result and metadata.
   #
```

### Comparing `langfun-0.0.2.dev20240528/langfun/core/message_test.py` & `langfun-0.0.2.dev20240529/langfun/core/message_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
   def test_from_value(self):
     self.assertTrue(
         pg.eq(message.UserMessage.from_value('hi'), message.UserMessage('hi'))
     )
     self.assertTrue(
         pg.eq(
             message.UserMessage.from_value(CustomModality('foo')),
-            message.UserMessage('{{object}}', object=CustomModality('foo')),
+            message.UserMessage('<<[[object]]>>', object=CustomModality('foo')),
         )
     )
     m = message.UserMessage('hi')
     self.assertIs(message.UserMessage.from_value(m), m)
 
   def test_source_tracking(self):
     m1 = message.UserMessage('hi')
@@ -254,64 +254,67 @@
     )
     self.assertIs(m3.get_modality('x.img2'), m1.x.img2)
     self.assertIs(m3.get_modality('output_image'), m3.output_image)
     self.assertIsNone(m3.get_modality('video'))
 
   def test_referred_modalities(self):
     m1 = message.UserMessage(
-        'hi, this is a {{img1}} and {{x.img2}}',
+        'hi, this is a <<[[img1]]>> and <<[[x.img2]]>>',
         img1=CustomModality('foo'),
         x=dict(img2=CustomModality('bar')),
     )
     m2 = message.SystemMessage('class Question:\n  image={{img1}}', source=m1)
     m3 = message.AIMessage(
-        'This is the {{output_image}} based on {{x.img2}}, {{unknown_var}}',
+        (
+            'This is the <<[[output_image]]>> based on <<[[x.img2]]>>, '
+            '{{unknown_var}}'
+        ),
         output_image=CustomModality('bar'),
         source=m2,
     )
     self.assertEqual(
         m3.referred_modalities(),
         {
             'output_image': m3.output_image,
             'x.img2': m1.x.img2,
         },
     )
 
   def test_chunking(self):
     m = message.UserMessage(
         inspect.cleandoc("""
-            Hi, this is {{a}} and this is {{b}}.
-            {{x.c}} {{something else
+            Hi, this is <<[[a]]>> and this is {{b}}.
+            <<[[x.c]]>> {{something else
             """),
         a=CustomModality('foo'),
         x=dict(c=CustomModality('bar')),
     )
     chunks = m.chunk()
     self.assertTrue(
         pg.eq(
             chunks,
             [
                 'Hi, this is',
                 CustomModality('foo'),
                 'and this is {{b}}.',
                 CustomModality('bar'),
-                ' {{something else',
+                '{{something else',
             ],
         )
     )
     self.assertTrue(
         pg.eq(
             message.AIMessage.from_chunks(chunks),
             message.AIMessage(
                 inspect.cleandoc("""
                     Hi, this is
-                    {{obj0}}
+                    <<[[obj0]]>>
                     and this is {{b}}.
-                    {{obj1}}
-                     {{something else
+                    <<[[obj1]]>>
+                    {{something else
                     """),
                 obj0=pg.Ref(m.a),
                 obj1=pg.Ref(m.x.c),
             ),
         )
     )
```

### Comparing `langfun-0.0.2.dev20240528/langfun/core/modalities/__init__.py` & `langfun-0.0.2.dev20240529/langfun/core/modalities/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/modalities/image.py` & `langfun-0.0.2.dev20240529/langfun/core/modalities/image.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/modalities/image_test.py` & `langfun-0.0.2.dev20240529/langfun/core/modalities/image_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/modalities/mime.py` & `langfun-0.0.2.dev20240529/langfun/core/modalities/mime.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/modalities/mime_test.py` & `langfun-0.0.2.dev20240529/langfun/core/modalities/mime_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/modalities/pdf.py` & `langfun-0.0.2.dev20240529/langfun/core/modalities/pdf.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/modalities/pdf_test.py` & `langfun-0.0.2.dev20240529/langfun/core/modalities/pdf_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/modalities/video.py` & `langfun-0.0.2.dev20240529/langfun/core/modalities/video.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/modalities/video_test.py` & `langfun-0.0.2.dev20240529/langfun/core/modalities/video_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/modality.py` & `langfun-0.0.2.dev20240529/langfun/core/modality.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,16 @@
       _TLS_MODALITY_AS_REF, enabled, False
   )
 
 
 class Modality(component.Component):
   """Base class for multimodal object."""
 
-  REF_START = '{{'
-  REF_END = '}}'
+  REF_START = '<<[['
+  REF_END = ']]>>'
 
   def format(self, *args, **kwargs) -> str:
     if self.referred_name is None or not pg.object_utils.thread_local_get(
         _TLS_MODALITY_AS_REF, False
     ):
       return super().format(*args, **kwargs)
     return Modality.text_marker(self.referred_name)
```

### Comparing `langfun-0.0.2.dev20240528/langfun/core/modality_test.py` & `langfun-0.0.2.dev20240529/langfun/core/modality_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     self.assertIsNone(v.referred_name)
     self.assertEqual(str(v), "CustomModality(\n  content = 'a'\n)")
 
     _ = pg.Dict(metadata=pg.Dict(x=pg.Dict(metadata=pg.Dict(y=v))))
     self.assertEqual(v.referred_name, 'x.metadata.y')
     self.assertEqual(str(v), "CustomModality(\n  content = 'a'\n)")
     with modality.format_modality_as_ref():
-      self.assertEqual(str(v), '{{x.metadata.y}}')
+      self.assertEqual(str(v), '<<[[x.metadata.y]]>>')
 
 
 class ModalityRefTest(unittest.TestCase):
 
   def test_placehold(self):
     class A(pg.Object):
       x: Any
```

### Comparing `langfun-0.0.2.dev20240528/langfun/core/natural_language.py` & `langfun-0.0.2.dev20240529/langfun/core/natural_language.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/natural_language_test.py` & `langfun-0.0.2.dev20240529/langfun/core/natural_language_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/sampling.py` & `langfun-0.0.2.dev20240529/langfun/core/sampling.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/sampling_test.py` & `langfun-0.0.2.dev20240529/langfun/core/sampling_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/structured/__init__.py` & `langfun-0.0.2.dev20240529/langfun/core/structured/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/structured/completion.py` & `langfun-0.0.2.dev20240529/langfun/core/structured/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/structured/completion_test.py` & `langfun-0.0.2.dev20240529/langfun/core/structured/completion_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -460,15 +460,15 @@
                 ),
                 name=MISSING(str)
               )
               ```
 
             MODALITY_REFERENCES:
               {
-                'examples[0].input.image': {{examples[0].input.image}}
+                'examples[0].input.image': <<[[examples[0].input.image]]>>
               }
 
             OUTPUT_OBJECT:
               ```python
               Animal(
                 image=ModalityRef(
                   name='examples[0].output.image'
@@ -486,15 +486,15 @@
                 ),
                 name=MISSING(str)
               )
               ```
 
             MODALITY_REFERENCES:
               {
-                'input.image': {{input.image}}
+                'input.image': <<[[input.image]]>>
               }
 
             OUTPUT_OBJECT:
             """),
     )
     self.assertTrue(
         pg.eq(
```

### Comparing `langfun-0.0.2.dev20240528/langfun/core/structured/description.py` & `langfun-0.0.2.dev20240529/langfun/core/structured/description.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/structured/description_test.py` & `langfun-0.0.2.dev20240529/langfun/core/structured/description_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/structured/function_generation.py` & `langfun-0.0.2.dev20240529/langfun/core/structured/function_generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/structured/function_generation_test.py` & `langfun-0.0.2.dev20240529/langfun/core/structured/function_generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/structured/mapping.py` & `langfun-0.0.2.dev20240529/langfun/core/structured/mapping.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/structured/mapping_test.py` & `langfun-0.0.2.dev20240529/langfun/core/structured/mapping_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/structured/parsing.py` & `langfun-0.0.2.dev20240529/langfun/core/structured/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/structured/parsing_test.py` & `langfun-0.0.2.dev20240529/langfun/core/structured/parsing_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/structured/prompting.py` & `langfun-0.0.2.dev20240529/langfun/core/structured/prompting.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/structured/prompting_test.py` & `langfun-0.0.2.dev20240529/langfun/core/structured/prompting_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,52 +204,54 @@
 
   def test_root_modality_to_structure_render(self):
     lm = fake.StaticResponse('1')
     self.assert_render(
         modalities.Image.from_bytes(b'mock_image'),
         int,
         lm=lm,
-        expected_snippet='\n\nINPUT_OBJECT:\n  {{input}}\n\n',
+        expected_snippet='\n\nINPUT_OBJECT:\n  <<[[input]]>>\n\n',
         expected_modalities=1,
     )
 
   def test_root_modality_to_str_render(self):
     lm = fake.StaticResponse('1')
     self.assert_render(
         modalities.Image.from_bytes(b'mock_image'),
         None,
         lm=lm,
-        expected_snippet='{{input}}',
+        expected_snippet='<<[[input]]>>',
         exact_match=True,
         expected_modalities=1,
     )
 
   def test_str_with_modality_to_str_render(self):
     lm = fake.StaticResponse('A cat and a mouse.')
     self.assert_render(
         'What are these? {{this_image}} and {{that_image}}',
         None,
         this_image=modalities.Image.from_bytes(b'cat_image'),
         that_image=modalities.Image.from_bytes(b'mouse_image'),
         lm=lm,
-        expected_snippet='What are these? {{this_image}} and {{that_image}}',
+        expected_snippet=(
+            'What are these? <<[[this_image]]>> and <<[[that_image]]>>'
+        ),
         exact_match=True,
         expected_modalities=2,
     )
 
   def test_structure_with_modality_to_str_render(self):
     lm = fake.StaticResponse('A cat and a mouse.')
     self.assert_render(
         [
             modalities.Image.from_bytes(b'cat_image'),
             modalities.Image.from_bytes(b'mouse_image'),
         ],
         None,
         lm=lm,
-        expected_snippet='`[{{input[0]}}, {{input[1]}}]`',
+        expected_snippet='`[<<[[input[0]]]>>, <<[[input[1]]]>>]`',
         exact_match=True,
         expected_modalities=2,
     )
 
   def test_structure_with_modality_to_structure_render(self):
     lm = fake.StaticResponse('["cat", "mouse"]')
     self.assert_render(
@@ -270,16 +272,16 @@
                   name='input[1]'
                 )
               ]
               ```
 
             MODALITY_REFERENCES:
               {
-                'input[0]': {{input[0]}},
-                'input[1]': {{input[1]}}
+                'input[0]': <<[[input[0]]]>>,
+                'input[1]': <<[[input[1]]]>>
               }
             """),
         expected_modalities=2,
     )
 
   def test_bad_protocol(self):
     with self.assertRaisesRegex(ValueError, 'Unknown protocol'):
```

### Comparing `langfun-0.0.2.dev20240528/langfun/core/structured/schema.py` & `langfun-0.0.2.dev20240529/langfun/core/structured/schema.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/structured/schema_generation.py` & `langfun-0.0.2.dev20240529/langfun/core/structured/schema_generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/structured/schema_generation_test.py` & `langfun-0.0.2.dev20240529/langfun/core/structured/schema_generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/structured/schema_test.py` & `langfun-0.0.2.dev20240529/langfun/core/structured/schema_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/structured/scoring.py` & `langfun-0.0.2.dev20240529/langfun/core/structured/scoring.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/structured/scoring_test.py` & `langfun-0.0.2.dev20240529/langfun/core/structured/scoring_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/subscription.py` & `langfun-0.0.2.dev20240529/langfun/core/subscription.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/subscription_test.py` & `langfun-0.0.2.dev20240529/langfun/core/subscription_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/template.py` & `langfun-0.0.2.dev20240529/langfun/core/template.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/template_test.py` & `langfun-0.0.2.dev20240529/langfun/core/template_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,15 +305,15 @@
       def to_bytes(self):
         return self.content.encode()
 
     self.assertEqual(
         Template(
             'This is {{ x }} and {{ a }}', x=1, a=CustomModality('foo')
         ).render(),
-        'This is 1 and {{a}}',
+        'This is 1 and <<[[a]]>>',
     )
 
   def test_render_with_default(self):
 
     class Foo(Template):
       """Foo.
```

### Comparing `langfun-0.0.2.dev20240528/langfun/core/templates/__init__.py` & `langfun-0.0.2.dev20240529/langfun/core/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/templates/completion.py` & `langfun-0.0.2.dev20240529/langfun/core/templates/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/templates/completion_test.py` & `langfun-0.0.2.dev20240529/langfun/core/templates/completion_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/templates/conversation.py` & `langfun-0.0.2.dev20240529/langfun/core/templates/conversation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/templates/conversation_test.py` & `langfun-0.0.2.dev20240529/langfun/core/templates/conversation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/templates/demonstration.py` & `langfun-0.0.2.dev20240529/langfun/core/templates/demonstration.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/templates/demonstration_test.py` & `langfun-0.0.2.dev20240529/langfun/core/templates/demonstration_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/templates/selfplay.py` & `langfun-0.0.2.dev20240529/langfun/core/templates/selfplay.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/templates/selfplay_test.py` & `langfun-0.0.2.dev20240529/langfun/core/templates/selfplay_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/text_formatting.py` & `langfun-0.0.2.dev20240529/langfun/core/text_formatting.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun/core/text_formatting_test.py` & `langfun-0.0.2.dev20240529/langfun/core/text_formatting_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/langfun.egg-info/PKG-INFO` & `langfun-0.0.2.dev20240529/langfun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240528
+Version: 0.0.2.dev20240529
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langfun-0.0.2.dev20240528/langfun.egg-info/SOURCES.txt` & `langfun-0.0.2.dev20240529/langfun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240528/setup.py` & `langfun-0.0.2.dev20240529/setup.py`

 * *Files identical despite different names*

