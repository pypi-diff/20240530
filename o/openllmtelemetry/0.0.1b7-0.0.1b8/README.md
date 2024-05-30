# Comparing `tmp/openllmtelemetry-0.0.1b7.tar.gz` & `tmp/openllmtelemetry-0.0.1b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openllmtelemetry-0.0.1b7.tar", max compression
+gzip compressed data, was "openllmtelemetry-0.0.1b8.tar", max compression
```

## Comparing `openllmtelemetry-0.0.1b7.tar` & `openllmtelemetry-0.0.1b8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    11357 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b7/LICENSE
--rw-r--r--   0        0        0     4317 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b7/README.md
--rw-r--r--   0        0        0       99 2024-05-23 21:28:06.887620 openllmtelemetry-0.0.1b7/openllmtelemetry/__init__.py
--rw-r--r--   0        0        0     8650 2024-05-24 16:00:12.713852 openllmtelemetry-0.0.1b7/openllmtelemetry/config.py
--rw-r--r--   0        0        0       61 2024-05-24 16:00:12.713852 openllmtelemetry-0.0.1b7/openllmtelemetry/guardrails/__init__.py
--rw-r--r--   0        0        0     4541 2024-05-24 16:00:12.713852 openllmtelemetry-0.0.1b7/openllmtelemetry/guardrails/client.py
--rw-r--r--   0        0        0     7180 2024-05-24 16:00:12.713852 openllmtelemetry-0.0.1b7/openllmtelemetry/guardrails/handlers.py
--rw-r--r--   0        0        0     2667 2024-05-24 16:00:12.713852 openllmtelemetry-0.0.1b7/openllmtelemetry/instrument.py
--rw-r--r--   0        0        0    11339 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/LICENSE
--rw-r--r--   0        0        0        0 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/__init__.py
--rw-r--r--   0        0        0    14054 2024-05-28 16:10:07.443574 openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/bedrock/__init__.py
--rw-r--r--   0        0        0     2344 2024-05-14 21:55:10.222851 openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/bedrock/reusable_streaming_body.py
--rw-r--r--   0        0        0     1719 2024-05-24 16:00:12.713852 openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0     4769 2024-05-24 16:00:12.713852 openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/openai/shared/__init__.py
--rw-r--r--   0        0        0     9995 2024-05-24 16:00:12.713852 openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/openai/shared/chat_wrappers.py
--rw-r--r--   0        0        0     6306 2024-05-24 16:00:12.713852 openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/openai/shared/completion_wrappers.py
--rw-r--r--   0        0        0     3509 2024-05-24 16:00:12.713852 openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/openai/shared/embeddings_wrappers.py
--rw-r--r--   0        0        0     1231 2024-05-14 21:55:10.222851 openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/openai/utils.py
--rw-r--r--   0        0        0     2401 2024-05-24 16:00:12.713852 openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/openai/v0/__init__.py
--rw-r--r--   0        0        0     2908 2024-05-24 16:00:12.713852 openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/openai/v1/__init__.py
--rw-r--r--   0        0        0       28 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/openai/version.py
--rw-r--r--   0        0        0     1407 2024-05-24 16:00:12.713852 openllmtelemetry-0.0.1b7/openllmtelemetry/intrument_openai.py
--rw-r--r--   0        0        0     2493 2024-05-24 16:00:12.713852 openllmtelemetry-0.0.1b7/openllmtelemetry/semantic_conventions/gen_ai/__init__.py
--rw-r--r--   0        0        0      809 2024-04-25 18:42:42.775178 openllmtelemetry-0.0.1b7/openllmtelemetry/span_exporter.py
--rw-r--r--   0        0        0      477 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b7/openllmtelemetry/version.py
--rw-r--r--   0        0        0     1653 2024-05-24 16:00:12.713852 openllmtelemetry-0.0.1b7/pyproject.toml
--rw-r--r--   0        0        0     5320 1970-01-01 00:00:00.000000 openllmtelemetry-0.0.1b7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-11-22 23:27:14.459880 openllmtelemetry-0.0.1b8/LICENSE
+-rw-r--r--   0        0        0     4317 2024-04-24 17:37:18.405975 openllmtelemetry-0.0.1b8/README.md
+-rw-r--r--   0        0        0       99 2024-05-24 17:45:47.459524 openllmtelemetry-0.0.1b8/openllmtelemetry/__init__.py
+-rw-r--r--   0        0        0     8650 2024-05-24 17:45:47.460020 openllmtelemetry-0.0.1b8/openllmtelemetry/config.py
+-rw-r--r--   0        0        0       61 2024-05-24 17:45:47.460264 openllmtelemetry-0.0.1b8/openllmtelemetry/guardrails/__init__.py
+-rw-r--r--   0        0        0     4541 2024-05-24 17:45:47.460515 openllmtelemetry-0.0.1b8/openllmtelemetry/guardrails/client.py
+-rw-r--r--   0        0        0     7227 2024-05-29 22:38:28.252547 openllmtelemetry-0.0.1b8/openllmtelemetry/guardrails/handlers.py
+-rw-r--r--   0        0        0     2667 2024-05-24 17:45:47.461134 openllmtelemetry-0.0.1b8/openllmtelemetry/instrument.py
+-rw-r--r--   0        0        0    11339 2024-04-24 17:37:18.407381 openllmtelemetry-0.0.1b8/openllmtelemetry/instrumentation/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-24 17:37:18.407435 openllmtelemetry-0.0.1b8/openllmtelemetry/instrumentation/__init__.py
+-rw-r--r--   0        0        0    14054 2024-05-24 17:45:47.461419 openllmtelemetry-0.0.1b8/openllmtelemetry/instrumentation/bedrock/__init__.py
+-rw-r--r--   0        0        0     2344 2024-05-24 17:45:47.461701 openllmtelemetry-0.0.1b8/openllmtelemetry/instrumentation/bedrock/reusable_streaming_body.py
+-rw-r--r--   0        0        0     1719 2024-05-24 17:45:47.462072 openllmtelemetry-0.0.1b8/openllmtelemetry/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0     4903 2024-05-29 23:43:58.526847 openllmtelemetry-0.0.1b8/openllmtelemetry/instrumentation/openai/shared/__init__.py
+-rw-r--r--   0        0        0    10656 2024-05-29 23:36:32.251784 openllmtelemetry-0.0.1b8/openllmtelemetry/instrumentation/openai/shared/chat_wrappers.py
+-rw-r--r--   0        0        0     6090 2024-05-29 22:45:06.220020 openllmtelemetry-0.0.1b8/openllmtelemetry/instrumentation/openai/shared/completion_wrappers.py
+-rw-r--r--   0        0        0     3509 2024-05-24 17:45:47.463370 openllmtelemetry-0.0.1b8/openllmtelemetry/instrumentation/openai/shared/embeddings_wrappers.py
+-rw-r--r--   0        0        0     1231 2024-05-24 17:45:47.463645 openllmtelemetry-0.0.1b8/openllmtelemetry/instrumentation/openai/utils.py
+-rw-r--r--   0        0        0     2401 2024-05-24 17:45:47.463857 openllmtelemetry-0.0.1b8/openllmtelemetry/instrumentation/openai/v0/__init__.py
+-rw-r--r--   0        0        0     2908 2024-05-24 17:45:47.464149 openllmtelemetry-0.0.1b8/openllmtelemetry/instrumentation/openai/v1/__init__.py
+-rw-r--r--   0        0        0       28 2024-04-24 17:37:18.409700 openllmtelemetry-0.0.1b8/openllmtelemetry/instrumentation/openai/version.py
+-rw-r--r--   0        0        0     1407 2024-05-24 17:45:47.464398 openllmtelemetry-0.0.1b8/openllmtelemetry/intrument_openai.py
+-rw-r--r--   0        0        0     2519 2024-05-29 22:14:04.247624 openllmtelemetry-0.0.1b8/openllmtelemetry/semantic_conventions/gen_ai/__init__.py
+-rw-r--r--   0        0        0      809 2024-05-24 17:15:42.172550 openllmtelemetry-0.0.1b8/openllmtelemetry/span_exporter.py
+-rw-r--r--   0        0        0      477 2024-04-24 17:37:18.410285 openllmtelemetry-0.0.1b8/openllmtelemetry/version.py
+-rw-r--r--   0        0        0     1653 2024-05-30 20:24:37.751873 openllmtelemetry-0.0.1b8/pyproject.toml
+-rw-r--r--   0        0        0     5320 1970-01-01 00:00:00.000000 openllmtelemetry-0.0.1b8/PKG-INFO
```

### Comparing `openllmtelemetry-0.0.1b7/LICENSE` & `openllmtelemetry-0.0.1b8/LICENSE`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b7/README.md` & `openllmtelemetry-0.0.1b8/README.md`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b7/openllmtelemetry/config.py` & `openllmtelemetry-0.0.1b8/openllmtelemetry/config.py`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b7/openllmtelemetry/guardrails/client.py` & `openllmtelemetry-0.0.1b8/openllmtelemetry/guardrails/client.py`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b7/openllmtelemetry/guardrails/handlers.py` & `openllmtelemetry-0.0.1b8/openllmtelemetry/guardrails/handlers.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     prompt_provider,
     llm_caller,
     response_extractor,
     prompt_attributes_setter,
     request_type: LLMRequestTypeValues,
     streaming_response_handler=None,
     blocked_message_factory=None,
+    completion_span_name=SPAN_NAME,
 ):
     """
     Wrapper for synchronous calls to an LLM API.
     :param blocked_message_factory:
     :param streaming_response_handler:
     :param request_type:
     :param tracer: the trace provider
@@ -44,15 +45,15 @@
         prompt = prompt_provider()
         prompt_eval = _evaluate_prompt(tracer, guardrails_client, prompt)
 
         if prompt_eval and prompt_eval.action and prompt_eval.action.action_type == "block":
             return blocked_message_factory(prompt_eval, True)
 
         with tracer.start_span(
-            SPAN_NAME,
+            completion_span_name,
             kind=SpanKind.CLIENT,
             attributes={SpanAttributes.LLM_REQUEST_TYPE: request_type.value, SPAN_TYPE: "completion"},
         ) as span:
             prompt_attributes_setter(span)
             response, is_streaming = llm_caller(span)
             if is_streaming:
                 if streaming_response_handler:
```

### Comparing `openllmtelemetry-0.0.1b7/openllmtelemetry/instrument.py` & `openllmtelemetry-0.0.1b8/openllmtelemetry/instrument.py`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/LICENSE` & `openllmtelemetry-0.0.1b8/openllmtelemetry/instrumentation/LICENSE`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/bedrock/__init__.py` & `openllmtelemetry-0.0.1b8/openllmtelemetry/instrumentation/bedrock/__init__.py`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/bedrock/reusable_streaming_body.py` & `openllmtelemetry-0.0.1b8/openllmtelemetry/instrumentation/bedrock/reusable_streaming_body.py`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/openai/__init__.py` & `openllmtelemetry-0.0.1b8/openllmtelemetry/instrumentation/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/openai/shared/__init__.py` & `openllmtelemetry-0.0.1b8/openllmtelemetry/instrumentation/openai/shared/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,24 +42,25 @@
 def _set_span_attribute(span, name, value):
     if value is not None:
         if value != "":
             span.set_attribute(name, value)
     return
 
 
-def _set_api_attributes(span):
+def _set_api_attributes(span, instance=None):
     if not span.is_recording():
         return
 
     try:
-        base_url = openai.base_url if hasattr(openai, "base_url") else openai.api_base
+        base_url = getattr(getattr(instance, "_client", None), "base_url", None)
 
-        _set_span_attribute(span, OPENAI_API_BASE, base_url)
+        _set_span_attribute(span, "llm.base_url", str(base_url))
         _set_span_attribute(span, OPENAI_API_TYPE, openai.api_type)
         _set_span_attribute(span, OPENAI_API_VERSION, openai.api_version)
+        _set_span_attribute(span, "openapi.client.version", openai.__version__)
     except Exception as ex:  # pylint: disable=broad-except
         logger.warning("Failed to set api attributes for openai span, error: %s", str(ex))
 
     return
 
 
 def _set_functions_attributes(span, functions):
@@ -69,21 +70,21 @@
     for i, function in enumerate(functions):
         prefix = f"{SpanAttributes.LLM_REQUEST_FUNCTIONS}.{i}"
         _set_span_attribute(span, f"{prefix}.name", function.get("name"))
         _set_span_attribute(span, f"{prefix}.description", function.get("description"))
         _set_span_attribute(span, f"{prefix}.parameters", json.dumps(function.get("parameters")))
 
 
-def _set_request_attributes(span, kwargs):
+def _set_request_attributes(span, kwargs, vendor="unknown", instance=None):
     if not span.is_recording():
         return
 
     try:
-        _set_api_attributes(span)
-        _set_span_attribute(span, SpanAttributes.LLM_VENDOR, "OpenAI")
+        _set_api_attributes(span, instance)
+        _set_span_attribute(span, SpanAttributes.LLM_VENDOR, vendor)
         _set_span_attribute(span, SpanAttributes.LLM_REQUEST_MODEL, kwargs.get("model"))
         _set_span_attribute(span, SpanAttributes.LLM_REQUEST_MAX_TOKENS, kwargs.get("max_tokens"))
         _set_span_attribute(span, SpanAttributes.LLM_TEMPERATURE, kwargs.get("temperature"))
         _set_span_attribute(span, SpanAttributes.LLM_TOP_P, kwargs.get("top_p"))
         _set_span_attribute(span, SpanAttributes.LLM_FREQUENCY_PENALTY, kwargs.get("frequency_penalty"))
         _set_span_attribute(span, SpanAttributes.LLM_PRESENCE_PENALTY, kwargs.get("presence_penalty"))
         _set_span_attribute(span, SpanAttributes.LLM_USER, kwargs.get("user"))
```

### Comparing `openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/openai/shared/chat_wrappers.py` & `openllmtelemetry-0.0.1b8/openllmtelemetry/instrumentation/openai/shared/chat_wrappers.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,18 @@
 
 Changes made: customization for WhyLabs
 
 Original source: openllmetry: https://github.com/traceloop/openllmetry
 """
 import json
 import logging
+import time
 from typing import Optional
 
+# Get current datetime in epoch seconds and convert to int
 from opentelemetry import context as context_api
 
 # noinspection PyProtectedMember
 from opentelemetry.instrumentation.utils import _SUPPRESS_INSTRUMENTATION_KEY
 from opentelemetry.trace.status import Status, StatusCode
 from whylogs_container_client.models import EvaluationResult
 
@@ -71,20 +73,31 @@
 
 @_with_tracer_wrapper
 def chat_wrapper(tracer, guardrails_api: GuardrailsApi, wrapped, instance, args, kwargs):
     if context_api.get_value(_SUPPRESS_INSTRUMENTATION_KEY):
         return wrapped(*args, **kwargs)
 
     prompt_provider = create_prompt_provider(kwargs)
+    host = getattr(getattr(getattr(instance, "_client", None), "base_url", None), "host", None)
+    vendor = "GenericOpenAI"
+    span_name = "llm.chat"
+    if host and host.endswith(".openai.com"):
+        vendor = "OpenAI"
+        span_name = "openai.chat"
+    elif host.endswith(".azure.com"):
+        vendor = "AzureOpenAI"
+        span_name = "azureopenai.chat"
+    elif host.endswith(".nvidia.com"):
+        vendor = "Nvidia"
+        span_name = "nvidia.nim.chat"
 
     def call_llm(span):
         r = wrapped(*args, **kwargs)
         is_streaming = kwargs.get("stream")
         if not is_streaming:
-            _handle_response(r)
             if is_openai_v1():
                 response_dict = model_as_dict(r)
             else:
                 response_dict = r
 
             _set_response_attributes(response_dict, span)
         return r, is_streaming
@@ -93,48 +106,50 @@
         if open_api_v1:
             from openai.types.chat.chat_completion import ChatCompletion, Choice
             from openai.types.chat.chat_completion_chunk import ChatCompletionChunk
             from openai.types.chat.chat_completion_message import ChatCompletionMessage
             from openai.types.completion_usage import CompletionUsage
 
             if is_prompt:
-                content = "The prompt violates the policy set in WhyLabs Secure and cannot be processed."
+                content = f"Prompt blocked by WhyLabs: {eval_result.action.block_message}"
             else:
-                content = "The response violates the policy set in WhyLabs Secure and cannot be processed."
+                content = f"Response blocked by WhyLabs: {eval_result.action.block_message}"
             choice = Choice(
                 index=0,
                 finish_reason="stop",
                 message=ChatCompletionMessage(
                     content=content,  #
                     role="assistant",
                 ),
             )
+            current_epoch_time = int(time.time())
+
             if not is_streaming:
                 return ChatCompletion(
                     id="whylabs-guardrails-blocked",
                     choices=[
                         choice,
                     ],
-                    created=1715902825,
+                    created=current_epoch_time,
                     model="whylabs-guardrails",
                     object="chat.completion",
                     system_fingerprint=None,
                     usage=CompletionUsage(completion_tokens=0, prompt_tokens=0, total_tokens=0),
                 )
             else:
                 return ChatCompletionChunk(
-                    id="xyz",
-                    created=1715902825,
+                    id="whylabs-guardrails-blocked",
+                    created=current_epoch_time,
                     choices=[choice],
                     model="whylabs-guardrails",
                     object="chat.completion.chunk",
                 )
 
     def prompt_attributes_setter(span):
-        _set_request_attributes(span, kwargs)
+        _set_request_attributes(span, kwargs, vendor=vendor, instance=instance)
 
     def response_extractor(r):
         if is_openai_v1():
             response_dict = model_as_dict(r)
         else:
             response_dict = r
         return response_dict["choices"][0]["message"]["content"]
@@ -144,14 +159,15 @@
         guardrails_api,
         prompt_provider,
         call_llm,
         response_extractor,
         prompt_attributes_setter,
         LLMRequestTypeValues.CHAT,
         blocked_message_factory=blocked_message_factory,
+        completion_span_name=span_name,
     )
 
 
 @_with_tracer_wrapper
 async def achat_wrapper(tracer, guardrails_api: GuardrailsApi, wrapped, instance, args, kwargs):
     if context_api.get_value(_SUPPRESS_INSTRUMENTATION_KEY):
         return wrapped(*args, **kwargs)
@@ -173,15 +189,15 @@
 
         else:
             # TODO: handle streaming response. Where does guard response live?
             res = _abuild_from_streaming_response(span, r)
             return False, res
 
     def prompt_attributes_setter(span):
-        _set_request_attributes(span, kwargs)
+        _set_request_attributes(span, kwargs, instance=instance)
 
     def response_extractor(r):
         if is_openai_v1():
             response_dict = model_as_dict(r)
         else:
             response_dict = r
         return response_dict["choices"][0]["message"]["content"]
```

### Comparing `openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/openai/shared/completion_wrappers.py` & `openllmtelemetry-0.0.1b8/openllmtelemetry/instrumentation/openai/shared/completion_wrappers.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 from opentelemetry import context as context_api
 from opentelemetry.instrumentation.utils import _SUPPRESS_INSTRUMENTATION_KEY
 from opentelemetry.trace.status import Status, StatusCode
 
 from openllmtelemetry.guardrails import GuardrailsApi
 from openllmtelemetry.guardrails.handlers import async_wrapper, sync_wrapper
 from openllmtelemetry.instrumentation.openai.shared import (
-    _set_functions_attributes,
     _set_request_attributes,
     _set_response_attributes,
     _set_span_attribute,
     is_streaming_response,
     model_as_dict,
     should_send_prompts,
 )
@@ -70,15 +69,15 @@
             else:
                 response_dict = r
 
             _set_response_attributes(response_dict, span)
         return r
 
     def prompt_attributes_setter(span):
-        _set_request_attributes(span, kwargs)
+        _set_request_attributes(span, kwargs, instance=instance)
 
     def response_extractor(r):
         if is_openai_v1():
             response_dict = model_as_dict(r)
         else:
             response_dict = r
         return response_dict["choices"][0]["text"]
@@ -98,15 +97,15 @@
     async def call_llm(span):
         r = await wrapped(*args, **kwargs)
         if not kwargs.get("stream"):
             _handle_response(r, span)
         return r
 
     def prompt_attributes_setter(span):
-        _set_request_attributes(span, kwargs)
+        _set_request_attributes(span, kwargs, instance=instance)
 
     def response_extractor(r):
         if is_openai_v1():
             response_dict = model_as_dict(r)
         else:
             response_dict = r
         return response_dict["choices"][0]["text"]
@@ -121,21 +120,14 @@
         prompt_attributes_setter,
         _build_from_streaming_response,
         is_streaming_response,
         LLMRequestTypeValues.COMPLETION,
     )
 
 
-def _handle_request(span, kwargs):
-    _set_request_attributes(span, kwargs)
-    if should_send_prompts():
-        _set_prompts(span, kwargs.get("prompt"))
-        _set_functions_attributes(span, kwargs.get("functions"))
-
-
 def _handle_response(response, span):
     if is_openai_v1():
         response_dict = model_as_dict(response)
     else:
         response_dict = response
 
     _set_response_attributes(response_dict, span)
```

### Comparing `openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/openai/shared/embeddings_wrappers.py` & `openllmtelemetry-0.0.1b8/openllmtelemetry/instrumentation/openai/shared/embeddings_wrappers.py`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/openai/utils.py` & `openllmtelemetry-0.0.1b8/openllmtelemetry/instrumentation/openai/utils.py`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/openai/v0/__init__.py` & `openllmtelemetry-0.0.1b8/openllmtelemetry/instrumentation/openai/v0/__init__.py`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/openai/v1/__init__.py` & `openllmtelemetry-0.0.1b8/openllmtelemetry/instrumentation/openai/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b7/openllmtelemetry/intrument_openai.py` & `openllmtelemetry-0.0.1b8/openllmtelemetry/intrument_openai.py`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b7/openllmtelemetry/semantic_conventions/gen_ai/__init__.py` & `openllmtelemetry-0.0.1b8/openllmtelemetry/semantic_conventions/gen_ai/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     LLM_PRESENCE_PENALTY = "llm.presence_penalty"
     LLM_PROMPTS = "llm.prompts"
     LLM_COMPLETIONS = "llm.completions"
     LLM_CHAT_STOP_SEQUENCES = "llm.chat.stop_sequences"
     LLM_REQUEST_FUNCTIONS = "llm.request.functions"
     LLM_STREAMING = "llm.streaming"
 
+    LLM_HOST = "llm.host"
     # Vector DB
     VECTOR_DB_VENDOR = "vector_db.vendor"
     VECTOR_DB_QUERY_TOP_K = "vector_db.query.top_k"
 
 
 class Events(Enum):
     VECTOR_DB_QUERY_EMBEDDINGS = "vector_db.query.embeddings"
```

### Comparing `openllmtelemetry-0.0.1b7/openllmtelemetry/span_exporter.py` & `openllmtelemetry-0.0.1b8/openllmtelemetry/span_exporter.py`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b7/pyproject.toml` & `openllmtelemetry-0.0.1b8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "OpenLLMTelemetry"
-version = "0.0.1.b7"
+version = "0.0.1.b8"
 description = "End-to-end observability with built-in security guardrails."
 authors = ["WhyLabs.ai <support@whylabs.ai>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
```

### Comparing `openllmtelemetry-0.0.1b7/PKG-INFO` & `openllmtelemetry-0.0.1b8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: OpenLLMTelemetry
-Version: 0.0.1b7
+Name: openllmtelemetry
+Version: 0.0.1b8
 Summary: End-to-end observability with built-in security guardrails.
 License: Apache-2.0
 Author: WhyLabs.ai
 Author-email: support@whylabs.ai
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

