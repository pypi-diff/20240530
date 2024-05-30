# Comparing `tmp/rigging-1.1.2.tar.gz` & `tmp/rigging-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rigging-1.1.2.tar", max compression
+gzip compressed data, was "rigging-1.2.0.tar", max compression
```

## Comparing `rigging-1.1.2.tar` & `rigging-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1066 2024-05-24 04:26:38.225791 rigging-1.1.2/LICENSE
--rw-r--r--   0        0        0     1477 2024-05-24 04:26:38.225791 rigging-1.1.2/README.md
--rw-r--r--   0        0        0     3012 2024-05-24 04:26:38.229791 rigging-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      879 2024-05-24 04:26:38.229791 rigging-1.1.2/rigging/__init__.py
--rw-r--r--   0        0        0    45371 2024-05-24 04:26:38.229791 rigging-1.1.2/rigging/chat.py
--rw-r--r--   0        0        0    29155 2024-05-24 04:26:38.233791 rigging-1.1.2/rigging/completion.py
--rw-r--r--   0        0        0     3491 2024-05-24 04:26:38.233791 rigging-1.1.2/rigging/data.py
--rw-r--r--   0        0        0     1775 2024-05-24 04:26:38.233791 rigging-1.1.2/rigging/error.py
--rw-r--r--   0        0        0      762 2024-05-24 04:26:38.233791 rigging-1.1.2/rigging/generator/__init__.py
--rw-r--r--   0        0        0    15398 2024-05-24 04:26:38.233791 rigging-1.1.2/rigging/generator/base.py
--rw-r--r--   0        0        0     6417 2024-05-24 04:26:38.233791 rigging-1.1.2/rigging/generator/litellm_.py
--rw-r--r--   0        0        0     7306 2024-05-24 04:26:38.233791 rigging-1.1.2/rigging/generator/transformers_.py
--rw-r--r--   0        0        0     5808 2024-05-24 04:26:38.233791 rigging-1.1.2/rigging/generator/vllm_.py
--rw-r--r--   0        0        0     1852 2024-05-24 04:26:38.233791 rigging-1.1.2/rigging/logging.py
--rw-r--r--   0        0        0    13758 2024-05-24 04:26:38.233791 rigging-1.1.2/rigging/message.py
--rw-r--r--   0        0        0    13572 2024-05-24 04:26:38.233791 rigging-1.1.2/rigging/model.py
--rw-r--r--   0        0        0     3829 2024-05-24 04:26:38.233791 rigging-1.1.2/rigging/parsing.py
--rw-r--r--   0        0        0     1090 2024-05-24 04:26:38.233791 rigging-1.1.2/rigging/prompt.py
--rw-r--r--   0        0        0        0 2024-05-24 04:26:38.233791 rigging-1.1.2/rigging/py.typed
--rw-r--r--   0        0        0    10516 2024-05-24 04:26:38.233791 rigging-1.1.2/rigging/tool.py
--rw-r--r--   0        0        0     2731 1970-01-01 00:00:00.000000 rigging-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-30 20:41:54.263858 rigging-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1477 2024-05-30 20:41:54.263858 rigging-1.2.0/README.md
+-rw-r--r--   0        0        0     3012 2024-05-30 20:41:54.267858 rigging-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      994 2024-05-30 20:41:54.267858 rigging-1.2.0/rigging/__init__.py
+-rw-r--r--   0        0        0    47092 2024-05-30 20:41:54.267858 rigging-1.2.0/rigging/chat.py
+-rw-r--r--   0        0        0    30816 2024-05-30 20:41:54.267858 rigging-1.2.0/rigging/completion.py
+-rw-r--r--   0        0        0     3491 2024-05-30 20:41:54.267858 rigging-1.2.0/rigging/data.py
+-rw-r--r--   0        0        0     1775 2024-05-30 20:41:54.267858 rigging-1.2.0/rigging/error.py
+-rw-r--r--   0        0        0      848 2024-05-30 20:41:54.267858 rigging-1.2.0/rigging/generator/__init__.py
+-rw-r--r--   0        0        0    18001 2024-05-30 20:41:54.267858 rigging-1.2.0/rigging/generator/base.py
+-rw-r--r--   0        0        0     7537 2024-05-30 20:41:54.267858 rigging-1.2.0/rigging/generator/litellm_.py
+-rw-r--r--   0        0        0     7557 2024-05-30 20:41:54.267858 rigging-1.2.0/rigging/generator/transformers_.py
+-rw-r--r--   0        0        0     6267 2024-05-30 20:41:54.267858 rigging-1.2.0/rigging/generator/vllm_.py
+-rw-r--r--   0        0        0     1852 2024-05-30 20:41:54.267858 rigging-1.2.0/rigging/logging.py
+-rw-r--r--   0        0        0    13758 2024-05-30 20:41:54.267858 rigging-1.2.0/rigging/message.py
+-rw-r--r--   0        0        0    13572 2024-05-30 20:41:54.267858 rigging-1.2.0/rigging/model.py
+-rw-r--r--   0        0        0     3829 2024-05-30 20:41:54.267858 rigging-1.2.0/rigging/parsing.py
+-rw-r--r--   0        0        0     1090 2024-05-30 20:41:54.267858 rigging-1.2.0/rigging/prompt.py
+-rw-r--r--   0        0        0        0 2024-05-30 20:41:54.267858 rigging-1.2.0/rigging/py.typed
+-rw-r--r--   0        0        0    10516 2024-05-30 20:41:54.267858 rigging-1.2.0/rigging/tool.py
+-rw-r--r--   0        0        0     2731 1970-01-01 00:00:00.000000 rigging-1.2.0/PKG-INFO
```

### Comparing `rigging-1.1.2/LICENSE` & `rigging-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rigging-1.1.2/README.md` & `rigging-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `rigging-1.1.2/pyproject.toml` & `rigging-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rigging"
-version = "1.1.2"
+version = "1.2.0"
 description = "LLM Interaction Framework"
 authors = ["Nick Landers <monoxgas@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/dreadnode/rigging"
 readme = "README.md"
 packages = [
     {include = "rigging"}
```

### Comparing `rigging-1.1.2/rigging/__init__.py` & `rigging-1.2.0/rigging/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 from rigging.chat import Chat, PendingChat
 from rigging.completion import Completion, PendingCompletion
 from rigging.data import chats_to_df, df_to_chats
-from rigging.generator import GenerateParams, Generator, chat, complete, get_generator, register_generator
+from rigging.generator import (
+    GeneratedMessage,
+    GeneratedText,
+    GenerateParams,
+    Generator,
+    chat,
+    complete,
+    get_generator,
+    register_generator,
+)
 from rigging.message import Message, MessageDict, Messages
 from rigging.model import Model, attr, element, make_primitive, wrapped
 from rigging.tool import Tool
 
 __version__ = "1.1.1"
 
 __all__ = [
@@ -18,14 +27,16 @@
     "attr",
     "element",
     "wrapped",
     "Chat",
     "PendingChat",
     "Generator",
     "GenerateParams",
+    "GeneratedMessage",
+    "GeneratedText",
     "chat",
     "complete",
     "Completion",
     "PendingCompletion",
     "register_generator",
     "chats_to_df",
     "df_to_chats",
```

### Comparing `rigging-1.1.2/rigging/chat.py` & `rigging-1.2.0/rigging/chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from uuid import UUID, uuid4
 
 from loguru import logger
 from pydantic import BaseModel, ConfigDict, Field, ValidationError, computed_field
 
 from rigging.error import MessagesExhaustedMaxRoundsError
 from rigging.generator import GenerateParams, Generator, get_generator
+from rigging.generator.base import StopReason, Usage  # noqa: TCH001
 from rigging.message import Message, MessageDict, Messages
 from rigging.model import Model, ModelT, SystemErrorModel, ValidationErrorModel
 from rigging.prompt import system_tool_extension
 from rigging.tool import Tool, ToolCalls, ToolDescriptionList, ToolResult, ToolResults
 
 DEFAULT_MAX_ROUNDS = 5
 """Maximum number of internal callback rounds to attempt during generation before giving up."""
@@ -42,14 +43,21 @@
     messages: list[Message]
     """The list of messages prior to generation."""
     generated: list[Message] = Field(default_factory=list)
     """The list of messages resulting from the generation."""
     metadata: dict[str, t.Any] = Field(default_factory=dict)
     """Additional metadata for the chat."""
 
+    stop_reason: StopReason = Field(default="unknown")
+    """The reason the generation stopped."""
+    usage: t.Optional[Usage] = Field(None, repr=False)
+    """The usage statistics for the generation if available."""
+    extra: dict[str, t.Any] = Field(default_factory=dict, repr=False)
+    """Any additional information from the generation."""
+
     generator: t.Optional[Generator] = Field(None, exclude=True, repr=False)
     """The generator associated with the chat."""
     params: t.Optional[GenerateParams] = Field(None, exclude=True, repr=False)
     """Any additional generation params used for this chat."""
 
     failed: bool = Field(False, exclude=True, repr=False)
     """
@@ -970,34 +978,40 @@
         while pending_states:
             inbounds = self.generator.generate_messages(
                 [self.chat.all + s.messages for s in pending_states], [s.params for s in pending_states]
             )
 
             for inbound, state in zip(inbounds, pending_states):
                 try:
-                    state.messages = state.processor.send(inbound)
+                    state.messages = state.processor.send(inbound.message)
                 except StopIteration as stop:
                     state.done = True
                     state.chat = Chat(
                         self.chat.all,
                         t.cast(list[Message], stop.value),
                         generator=self.generator,
                         metadata=self.metadata,
                         params=state.params,
+                        stop_reason=inbound.stop_reason,
+                        usage=inbound.usage,
+                        extra=inbound.extra,
                     )
                 except MessagesExhaustedMaxRoundsError as exhausted:
                     if not skip_failed and not include_failed:
                         raise
                     if include_failed:
                         state.chat = Chat(
                             self.chat.all,
                             exhausted.messages,
                             generator=self.generator,
                             metadata=self.metadata,
                             params=state.params,
+                            stop_reason=inbound.stop_reason,
+                            usage=inbound.usage,
+                            extra=inbound.extra,
                             failed=True,
                         )
                     state.done = True
 
             pending_states = [s for s in pending_states if not s.done]
 
         return self._post_run([s.chat for s in states if s.chat is not None])
@@ -1021,34 +1035,40 @@
         while pending_states:
             inbounds = await self.generator.agenerate_messages(
                 [self.chat.all + s.messages for s in pending_states], [s.params for s in pending_states]
             )
 
             for inbound, state in zip(inbounds, pending_states):
                 try:
-                    state.messages = state.processor.send(inbound)
+                    state.messages = state.processor.send(inbound.message)
                 except StopIteration as stop:
                     state.done = True
                     state.chat = Chat(
                         self.chat.all,
                         t.cast(list[Message], stop.value),
                         generator=self.generator,
                         metadata=self.metadata,
                         params=state.params,
+                        stop_reason=inbound.stop_reason,
+                        usage=inbound.usage,
+                        extra=inbound.extra,
                     )
                 except MessagesExhaustedMaxRoundsError as exhausted:
                     if not skip_failed and not include_failed:
                         raise
                     if include_failed:
                         state.chat = Chat(
                             self.chat.all,
                             exhausted.messages,
                             generator=self.generator,
                             metadata=self.metadata,
                             params=state.params,
+                            stop_reason=inbound.stop_reason,
+                            usage=inbound.usage,
+                            extra=inbound.extra,
                             failed=True,
                         )
                     state.done = True
 
             pending_states = [s for s in pending_states if not s.done]
 
         return await self._apost_run([s.chat for s in states if s.chat is not None])
@@ -1110,34 +1130,40 @@
                 inbounds = self.generator.generate_messages(
                     [s.inputs + s.messages for s in chunk],
                     [s.params for s in chunk],
                 )
 
                 for inbound, state in zip(inbounds, chunk):
                     try:
-                        state.messages = state.processor.send(inbound)
+                        state.messages = state.processor.send(inbound.message)
                     except StopIteration as stop:
                         state.done = True
                         state.chat = Chat(
                             state.inputs,
                             t.cast(list[Message], stop.value),
                             generator=self.generator,
                             metadata=self.metadata,
                             params=state.params,
+                            stop_reason=inbound.stop_reason,
+                            usage=inbound.usage,
+                            extra=inbound.extra,
                         )
                     except MessagesExhaustedMaxRoundsError as exhausted:
                         if not skip_failed and not include_failed:
                             raise
                         if include_failed:
                             state.chat = Chat(
                                 state.inputs,
                                 exhausted.messages,
                                 generator=self.generator,
                                 metadata=self.metadata,
                                 params=state.params,
+                                stop_reason=inbound.stop_reason,
+                                usage=inbound.usage,
+                                extra=inbound.extra,
                                 failed=True,
                             )
                         state.done = True
 
             pending_states = [s for s in pending_states if not s.done]
 
         return self._post_run([s.chat for s in states if s.chat is not None])
@@ -1181,34 +1207,40 @@
                 inbounds = await self.generator.agenerate_messages(
                     [s.inputs + s.messages for s in chunk],
                     [s.params for s in chunk],
                 )
 
                 for inbound, state in zip(inbounds, chunk):
                     try:
-                        state.messages = state.processor.send(inbound)
+                        state.messages = state.processor.send(inbound.message)
                     except StopIteration as stop:
                         state.done = True
                         state.chat = Chat(
                             state.inputs,
                             t.cast(list[Message], stop.value),
                             generator=self.generator,
                             metadata=self.metadata,
                             params=state.params,
+                            stop_reason=inbound.stop_reason,
+                            usage=inbound.usage,
+                            extra=inbound.extra,
                         )
                     except MessagesExhaustedMaxRoundsError as exhausted:
                         if not skip_failed and not include_failed:
                             raise
                         if include_failed:
                             state.chat = Chat(
                                 state.inputs,
                                 exhausted.messages,
                                 generator=self.generator,
                                 metadata=self.metadata,
                                 params=state.params,
+                                stop_reason=inbound.stop_reason,
+                                usage=inbound.usage,
+                                extra=inbound.extra,
                                 failed=True,
                             )
                         state.done = True
 
             pending_states = [s for s in pending_states if not s.done]
 
         return await self._apost_run([s.chat for s in states if s.chat is not None])
```

### Comparing `rigging-1.1.2/rigging/completion.py` & `rigging-1.2.0/rigging/completion.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from uuid import UUID, uuid4
 
 from loguru import logger
 from pydantic import BaseModel, ConfigDict, Field, computed_field
 
 from rigging.error import CompletionExhaustedMaxRoundsError
 from rigging.generator import GenerateParams, Generator, get_generator
+from rigging.generator.base import StopReason, Usage  # noqa: TCH001
 from rigging.parsing import parse_many
 
 if t.TYPE_CHECKING:
     from rigging.model import Model, ModelT
 
 DEFAULT_MAX_ROUNDS = 5
 
@@ -43,14 +44,21 @@
     text: str
     """The original text."""
     generated: str
     """The generated text."""
     metadata: dict[str, t.Any] = Field(default_factory=dict)
     """Additional metadata for the completion."""
 
+    stop_reason: StopReason = Field(default="unknown")
+    """The reason the generation stopped."""
+    usage: t.Optional[Usage] = Field(None, repr=False)
+    """The usage statistics for the generation if available."""
+    extra: dict[str, t.Any] = Field(default_factory=dict, repr=False)
+    """Any additional information from the generation."""
+
     generator: t.Optional[Generator] = Field(None, exclude=True, repr=False)
     """The generator associated with the completion."""
     params: t.Optional[GenerateParams] = Field(None, exclude=True, repr=False)
     """Any additional generation params used for this completion."""
 
     failed: bool = Field(default=False, repr=False)
     """
@@ -592,34 +600,40 @@
         while pending_states:
             inbounds = self.generator.generate_texts(
                 [s.text for s in pending_states], [s.params for s in pending_states]
             )
 
             for inbound, state in zip(inbounds, pending_states):
                 try:
-                    state.processor.send(inbound)
+                    state.processor.send(inbound.text)
                 except StopIteration as stop:
                     state.done = True
                     state.completion = Completion(
                         self.text,
                         t.cast(str, stop.value),
                         generator=self.generator,
                         params=state.params,
                         metadata=self.metadata,
+                        stop_reason=inbound.stop_reason,
+                        usage=inbound.usage,
+                        extra=inbound.extra,
                     )
                 except CompletionExhaustedMaxRoundsError as exhausted:
                     if not skip_failed and not include_failed:
                         raise
                     if include_failed:
                         state.completion = Completion(
                             self.text,
                             exhausted.completion,
                             generator=self.generator,
                             params=state.params,
                             metadata=self.metadata,
+                            stop_reason=inbound.stop_reason,
+                            usage=inbound.usage,
+                            extra=inbound.extra,
                             failed=True,
                         )
                     state.done = True
 
             pending_states = [s for s in pending_states if not s.done]
 
         return self._post_run([s.completion for s in states if s.completion is not None])
@@ -643,34 +657,40 @@
         while pending_states:
             inbounds = await self.generator.agenerate_texts(
                 [s.text for s in pending_states], [s.params for s in pending_states]
             )
 
             for inbound, state in zip(inbounds, pending_states):
                 try:
-                    state.processor.send(inbound)
+                    state.processor.send(inbound.text)
                 except StopIteration as stop:
                     state.done = True
                     state.completion = Completion(
                         self.text,
                         t.cast(str, stop.value),
                         generator=self.generator,
                         params=state.params,
                         metadata=self.metadata,
+                        stop_reason=inbound.stop_reason,
+                        usage=inbound.usage,
+                        extra=inbound.extra,
                     )
                 except CompletionExhaustedMaxRoundsError as exhausted:
                     if not skip_failed and not include_failed:
                         raise
                     if include_failed:
                         state.completion = Completion(
                             self.text,
                             exhausted.completion,
                             generator=self.generator,
                             params=state.params,
                             metadata=self.metadata,
+                            stop_reason=inbound.stop_reason,
+                            usage=inbound.usage,
+                            extra=inbound.extra,
                             failed=True,
                         )
                     state.done = True
 
             pending_states = [s for s in pending_states if not s.done]
 
         return self._post_run([s.completion for s in states if s.completion is not None])
@@ -712,34 +732,40 @@
             inbounds = self.generator.generate_texts(
                 [self.text + s.text for s in pending_states],
                 [s.params for s in pending_states],
             )
 
             for inbound, state in zip(inbounds, pending_states):
                 try:
-                    state.processor.send(inbound)
+                    state.processor.send(inbound.text)
                 except StopIteration as stop:
                     state.done = True
                     state.completion = Completion(
                         self.text,
                         t.cast(str, stop.value),
                         generator=self.generator,
                         params=state.params,
                         metadata=self.metadata,
+                        stop_reason=inbound.stop_reason,
+                        usage=inbound.usage,
+                        extra=inbound.extra,
                     )
                 except CompletionExhaustedMaxRoundsError as exhausted:
                     if not skip_failed and not include_failed:
                         raise
                     if include_failed:
                         state.completion = Completion(
                             self.text,
                             exhausted.completion,
                             generator=self.generator,
                             params=state.params,
                             metadata=self.metadata,
+                            stop_reason=inbound.stop_reason,
+                            usage=inbound.usage,
+                            extra=inbound.extra,
                             failed=True,
                         )
                     state.done = True
 
             pending_states = [s for s in pending_states if not s.done]
 
         return self._post_run([s.completion for s in states if s.completion is not None])
@@ -765,34 +791,40 @@
             inbounds = await self.generator.agenerate_texts(
                 [self.text + s.text for s in pending_states],
                 [s.params for s in pending_states],
             )
 
             for inbound, state in zip(inbounds, pending_states):
                 try:
-                    state.processor.send(inbound)
+                    state.processor.send(inbound.text)
                 except StopIteration as stop:
                     state.done = True
                     state.completion = Completion(
                         self.text,
                         t.cast(str, stop.value),
                         generator=self.generator,
                         params=state.params,
                         metadata=self.metadata,
+                        stop_reason=inbound.stop_reason,
+                        usage=inbound.usage,
+                        extra=inbound.extra,
                     )
                 except CompletionExhaustedMaxRoundsError as exhausted:
                     if not skip_failed and not include_failed:
                         raise
                     if include_failed:
                         state.completion = Completion(
                             self.text,
                             exhausted.completion,
                             generator=self.generator,
                             params=state.params,
                             metadata=self.metadata,
+                            stop_reason=inbound.stop_reason,
+                            usage=inbound.usage,
+                            extra=inbound.extra,
                             failed=True,
                         )
                     state.done = True
 
             pending_states = [s for s in pending_states if not s.done]
 
         return self._post_run([s.completion for s in states if s.completion is not None])
```

### Comparing `rigging-1.1.2/rigging/data.py` & `rigging-1.2.0/rigging/data.py`

 * *Files identical despite different names*

### Comparing `rigging-1.1.2/rigging/error.py` & `rigging-1.2.0/rigging/error.py`

 * *Files identical despite different names*

### Comparing `rigging-1.1.2/rigging/generator/base.py` & `rigging-1.2.0/rigging/generator/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import inspect
 import typing as t
 
 from loguru import logger
-from pydantic import BaseModel, ConfigDict, Field, field_validator
+from pydantic import BaseModel, BeforeValidator, ConfigDict, Field, field_validator
 from typing_extensions import Self
 
 from rigging.error import InvalidModelSpecifiedError
 from rigging.message import Message, MessageDict
 
 if t.TYPE_CHECKING:
     from rigging.chat import PendingChat
@@ -111,14 +111,96 @@
         """
         params = self.model_dump(exclude_unset=True)
         if "extra" in params:
             params.update(params.pop("extra"))
         return params
 
 
+StopReason = t.Literal["stop", "length", "content_filter", "unknown"]
+"""Reporting reason for generation completing."""
+
+
+def convert_stop_reason(reason: t.Optional[str]) -> StopReason:
+    if reason in ["stop", "eos"]:
+        return "stop"
+    elif reason in ["model_length"]:
+        return "length"
+    elif reason in ["length"]:
+        return "length"
+    elif reason in ["content_filter"]:
+        return "content_filter"
+    return "unknown"
+
+
+class Usage(BaseModel):
+    input_tokens: int
+    """The number of input tokens."""
+    output_tokens: int
+    """The number of output tokens."""
+    total_tokens: int
+    """The total number of tokens processed."""
+
+
+GeneratedT = t.TypeVar("GeneratedT", Message, str)
+
+
+class GeneratedMessage(BaseModel):
+    """A generated message with additional generation information."""
+
+    message: Message
+    """The generated message."""
+
+    stop_reason: t.Annotated[StopReason, BeforeValidator(convert_stop_reason)] = "unknown"
+    """The reason for stopping generation."""
+
+    usage: t.Optional[Usage] = None
+    """The usage statistics for the generation if available."""
+
+    extra: dict[str, t.Any] = Field(default_factory=dict)
+    """Any additional information from the generation."""
+
+    def __str__(self) -> str:
+        return str(self.message)
+
+    @classmethod
+    def from_text(cls, text: str, stop_reason: StopReason = "unknown") -> GeneratedMessage:
+        return cls(message=Message(role="assistant", content=text), stop_reason=stop_reason)
+
+
+class GeneratedText(BaseModel):
+    """A generated text with additional generation information."""
+
+    text: str
+    """The generated text."""
+
+    stop_reason: t.Annotated[StopReason, BeforeValidator(convert_stop_reason)] = "unknown"
+    """The reason for stopping generation."""
+
+    usage: t.Optional[Usage] = None
+    """The usage statistics for the generation if available."""
+
+    extra: dict[str, t.Any] = Field(default_factory=dict)
+    """Any additional information from the generation."""
+
+    def __str__(self) -> str:
+        return self.text
+
+    @classmethod
+    def from_text(cls, text: str, stop_reason: StopReason = "unknown") -> GeneratedText:
+        return cls(text=text, stop_reason=stop_reason)
+
+    def to_generated_message(self) -> GeneratedMessage:
+        return GeneratedMessage(
+            message=Message(role="assistant", content=self.text),
+            stop_reason=self.stop_reason,
+            usage=self.usage,
+            extra=self.extra,
+        )
+
+
 class Generator(BaseModel):
     """
     Base class for all rigging generators.
 
     This class provides common functionality and methods for generating completion messages.
 
     A subclass of this can implement any of the following:
@@ -168,15 +250,15 @@
         """
         return self
 
     def generate_messages(
         self,
         messages: t.Sequence[t.Sequence[Message]],
         params: t.Sequence[GenerateParams],
-    ) -> t.Sequence[Message]:
+    ) -> t.Sequence[GeneratedMessage]:
         """
         Generate a batch of messages using the specified parameters.
 
         Note:
             The length of `params` must be the same as the length of `many`.
 
         Args:
@@ -191,23 +273,23 @@
         """
         raise NotImplementedError("`generate_messages` is not supported by this generator.")
 
     async def agenerate_messages(
         self,
         messages: t.Sequence[t.Sequence[Message]],
         params: t.Sequence[GenerateParams],
-    ) -> t.Sequence[Message]:
+    ) -> t.Sequence[GeneratedMessage]:
         """async version of [rigging.generator.Generator.generate_messages][]"""
         raise NotImplementedError("`agenerate_messages` is not supported by this generator.")
 
     def generate_texts(
         self,
         texts: t.Sequence[str],
         params: t.Sequence[GenerateParams],
-    ) -> t.Sequence[str]:
+    ) -> t.Sequence[GeneratedText]:
         """
         Generate a batch of text completions using the generator.
 
         Note:
             This method falls back to looping over the inputs and calling `generate_text` for each item.
 
         Note:
@@ -225,15 +307,15 @@
         """
         raise NotImplementedError("`generate_texts` is not supported by this generator.")
 
     async def agenerate_texts(
         self,
         texts: t.Sequence[str],
         params: t.Sequence[GenerateParams],
-    ) -> t.Sequence[str]:
+    ) -> t.Sequence[GeneratedText]:
         """async version of [rigging.generator.Generator.generate_texts][]"""
         raise NotImplementedError("`agenerate_texts` is not supported by this generator.")
 
     # Helper alternative to chat(generator) -> generator.chat(...)
     #
     # params seem odd, but mypy doesn't like the TypedDict in a list otherwise
 
@@ -469,15 +551,15 @@
         provider: The name of the provider.
         generator_cls: The generator class to register.
     """
     global g_providers
     g_providers[provider] = generator_cls
 
 
-def trace_messages(messages: t.Sequence[Message], title: str) -> None:
+def trace_messages(messages: t.Sequence[Message] | t.Sequence[GeneratedMessage], title: str) -> None:
     """
     Helper function to trace log a sequence of Message objects.
 
     Args:
         messages: A sequence of Message objects to be logged.
         title: The title to be displayed in the log.
 
@@ -485,21 +567,21 @@
         None
     """
     logger.trace(f"--- {title} ---")
     logger.trace("\n".join([str(msg) for msg in messages]))
     logger.trace("---")
 
 
-def trace_str(content: str, title: str) -> None:
+def trace_str(content: str | GeneratedText, title: str) -> None:
     """
     Helper function to trace log a string.
 
     Parameters:
         content: The string content to be logged.
         title: The title of the log entry.
 
     Returns:
         None
     """
     logger.trace(f"--- {title} ---")
-    logger.trace(content)
+    logger.trace(str(content))
     logger.trace("---")
```

### Comparing `rigging-1.1.2/rigging/generator/litellm_.py` & `rigging-1.2.0/rigging/generator/vllm_.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,164 +1,187 @@
 from __future__ import annotations
 
-import asyncio
+import gc
+import inspect
 import typing as t
 
-import litellm  # type: ignore
+import torch
+import vllm
 
-from rigging.generator.base import GenerateParams, Generator, register_generator, trace_messages, trace_str
-from rigging.message import Message
+from rigging.generator.base import (
+    GeneratedMessage,
+    GeneratedText,
+    GenerateParams,
+    Generator,
+    register_generator,
+    trace_messages,
+    trace_str,
+)
+
+if t.TYPE_CHECKING:
+    from rigging.message import Message
+
+# Any batch over this size will trigger a dedicated
+# cache warmup step
+CACHE_TRIGGER = 8
 
-# We should probably let people configure
-# this independently, but for now we'll
-# fix it to prevent confusion
-litellm.drop_params = True
 
-
-class LiteLLMGenerator(Generator):
+class VLLMGenerator(Generator):
     """
-    Generator backed by the LiteLLM library.
+    Generator backed by the vLLM library for local model loading.
+
+    Find more information about supported models and formats [in their docs.](https://docs.vllm.ai/en/latest/index.html)
 
-    Find more information about supported models and formats [in their docs.](https://docs.litellm.ai/docs/providers).
+    Warning:
+        The use of VLLM requires the `vllm` package to be installed directly or by
+        installing rigging as `rigging[all]`.
 
     Note:
-        Batching support is not performant and simply a loop over inputs.
+        The async methods currently just call synchronous variants for compatibility.
 
-    Warning:
-        While some providers support passing `n` to produce a batch
-        of completions per request, we don't currently use this in the
-        implementation due to it's brittle requirements.
-
-    Tip:
-        Consider setting [`max_requests`][rigging.generator.litellm_.LiteLLMGenerator.max_requests]
-        to a lower value if you run into API limits. You can pass this directly in the generator id:
-
-        ```py
-        get_generator("litellm!openai/gpt-4o,max_requests=5")
-        ```
-    """
+    Note:
+        The model load into memory will occur lazily when the first generation is requested.
+        If you'd want to force this to happen earlier, you can use the
+        [`.load()`][rigging.generator.Generator.load] method.
 
-    max_requests: int | None = None
-    """
-    When using async variants, how many simultaneous requests to pool at one time.
-    This is useful to set when you run into API limits at a provider.
-    Defaults to `None` for no limit.
+        To unload, call [`.unload()`][rigging.generator.Generator.unload].
     """
 
-    # TODO: Some model providers support using `n` as a batch
-    # parameter to generate multiple completions at once. Which
-    # could help us optimize run_many calls.
-    #
-    # If we wanted this, we'd need to check the model provider
-    # and see if it was supported, and all our messages/texts
-    # were equal before overriding that parameter to the call.
-    #
-    # This seems like a brittle feature at the moment, so we'll
-    # leave it out for now.
-
-    def _generate_message(self, messages: t.Sequence[Message], params: GenerateParams) -> Message:
-        result = litellm.completion(
-            self.model,
-            [message.model_dump(include={"role", "content"}) for message in messages],
-            api_key=self.api_key,
-            **self.params.merge_with(params).to_dict(),
-        )
-        response = result.choices[-1].message.content.strip()
-        return Message(role="assistant", content=response)
+    dtype: str = "auto"
+    """Tensor dtype passed to [`vllm.LLM`](https://docs.vllm.ai/en/latest/offline_inference/llm.html)"""
+    quantization: str | None = None
+    """Quantiziation passed to [`vllm.LLM`](https://docs.vllm.ai/en/latest/offline_inference/llm.html)"""
+    gpu_memory_utilization: float = 0.9
+    """Memory utilization passed to [`vllm.LLM`](https://docs.vllm.ai/en/latest/offline_inference/llm.html)"""
+    enforce_eager: bool = False
+    """Eager enforcement passed to [`vllm.LLM`](https://docs.vllm.ai/en/latest/offline_inference/llm.html)"""
+    trust_remote_code: bool = False
+    """Trust remote code passed to [`vllm.LLM`](https://docs.vllm.ai/en/latest/offline_inference/llm.html)"""
+
+    _llm: vllm.LLM | None = None
+
+    @property
+    def llm(self) -> vllm.LLM:
+        """The underlying [`vLLM model`](https://docs.vllm.ai/en/latest/offline_inference/llm.html) instance."""
+        # Lazy initialization
+        if self._llm is None:
+            self._llm = vllm.LLM(
+                self.model,
+                dtype=self.dtype,
+                quantization=self.quantization,
+                gpu_memory_utilization=self.gpu_memory_utilization,
+                enforce_eager=self.enforce_eager,
+                trust_remote_code=self.trust_remote_code,
+            )
+        return self._llm
 
-    async def _agenerate_message(self, messages: t.Sequence[Message], params: GenerateParams) -> Message:
-        result = await litellm.acompletion(
-            self.model,
-            [message.model_dump(include={"role", "content"}) for message in messages],
-            api_key=self.api_key,
-            **self.params.merge_with(params).to_dict(),
-        )
-        response = result.choices[-1].message.content.strip()
-        return Message(role="assistant", content=response)
+    @classmethod
+    def from_obj(cls, model: str, llm: vllm.LLM, *, params: GenerateParams | None = None) -> VLLMGenerator:
+        """Create a generator from an existing vLLM instance.
+
+        Args:
+            llm: The vLLM instance to create the generator from.
+
+        Returns:
+            The VLLMGenerator instance.
+        """
+        generator = cls(model=model, params=params or GenerateParams())
+        generator._llm = llm
+        return generator
+
+    def load(self) -> VLLMGenerator:
+        _ = self.llm
+        return self
+
+    def unload(self) -> VLLMGenerator:
+        del self._llm
+        gc.collect()
+        torch.cuda.empty_cache()
+        return self
 
-    def _generate_text(self, text: str, params: GenerateParams) -> str:
-        result = litellm.text_completion(
-            text, self.model, api_key=self.api_key, **self.params.merge_with(params).to_dict()
+    def _generate(
+        self,
+        texts: list[str],
+        params: t.Sequence[GenerateParams],
+    ) -> list[GeneratedText]:
+        sampling_params_args = list(inspect.signature(vllm.SamplingParams.__init__).parameters.keys())
+        sampling_params = (
+            [
+                vllm.SamplingParams(
+                    **{k: v for k, v in self.params.merge_with(p).to_dict().items() if k in sampling_params_args}
+                )
+                for p in params
+            ]
+            if params
+            else None
         )
-        return t.cast(str, result.choices[-1]["text"])
 
-    async def _agenerate_text(self, text: str, params: GenerateParams) -> str:
-        result = await litellm.atext_completion(
-            text, self.model, api_key=self.api_key, **self.params.merge_with(params).to_dict()
+        # Do a cache warmup step if we have a lot of texts
+        if len(texts) > CACHE_TRIGGER:
+            self.llm.generate(
+                prompts=min(texts, key=len),
+                use_tqdm=False,
+            )
+
+        outputs = self.llm.generate(
+            prompts=texts,
+            sampling_params=sampling_params,
+            use_tqdm=False,
         )
-        return t.cast(str, result.choices[-1]["text"])
+        return [
+            GeneratedText(
+                text=o.outputs[-1].text,
+                stop_reason=o.outputs[-1].finish_reason,
+                extra={
+                    "request_id": o.request_id,
+                    "metrics": o.metrics,
+                    "stop_token": o.outputs[-1].stop_reason,
+                },
+            )
+            for o in outputs
+        ]
 
     def generate_messages(
         self,
         messages: t.Sequence[t.Sequence[Message]],
         params: t.Sequence[GenerateParams],
-    ) -> t.Sequence[Message]:
-        generated: list[Message] = []
-        for i, (_messages, _params) in enumerate(zip(messages, params)):
-            trace_messages(_messages, f"Messages {i+1}/{len(messages)}")
-            next_message = self._generate_message(_messages, _params)
-            generated.append(next_message)
-            trace_messages([next_message], f"Response {i+1}/{len(messages)}")
+    ) -> t.Sequence[GeneratedMessage]:
+        message_dicts = [[m.model_dump(include={"role", "content"}) for m in _messages] for _messages in messages]
+        texts = self.llm.get_tokenizer().apply_chat_template(message_dicts, add_generation_prompt=True, tokenize=False)
+        generated_texts = self._generate(texts, params=params)
+        generated = [g.to_generated_message() for g in generated_texts]
+
+        for i, (in_messages, out_message) in enumerate(zip(messages, generated)):
+            trace_messages(in_messages, f"Messages {i+1}/{len(in_messages)}")
+            trace_messages([out_message], f"Response {i+1}/{len(in_messages)}")
 
         return generated
 
     async def agenerate_messages(
         self,
         messages: t.Sequence[t.Sequence[Message]],
         params: t.Sequence[GenerateParams],
-    ) -> t.Sequence[Message]:
-        generated: list[Message] = []
-        max_requests = self.max_requests or len(messages)
-        for i in range(0, len(messages), max_requests):
-            chunk_messages = messages[i : i + max_requests]
-            chunk_params = params[i : i + max_requests]
-            chunk_generated = await asyncio.gather(
-                *[
-                    self._agenerate_message(_messages, _params)
-                    for _messages, _params in zip(chunk_messages, chunk_params)
-                ]
-            )
-            generated.extend(chunk_generated)
-
-            for j, (_messages, _generated) in enumerate(zip(chunk_messages, chunk_generated)):
-                trace_messages(_messages, f"Messages {i+j+1}/{len(messages)}")
-                trace_messages([_generated], f"Response {i+j+1}/{len(messages)}")
-
-        return generated
+    ) -> t.Sequence[GeneratedMessage]:
+        return self.generate_messages(messages, params)
 
     def generate_texts(
         self,
         texts: t.Sequence[str],
         params: t.Sequence[GenerateParams],
-    ) -> t.Sequence[str]:
-        generated: list[str] = []
-        for i, (text, _params) in enumerate(zip(texts, params)):
+    ) -> t.Sequence[GeneratedText]:
+        generated = self._generate(list(texts), params=params)
+
+        for i, (text, response) in enumerate(zip(texts, generated)):
             trace_str(text, f"Text {i+1}/{len(texts)}")
-            response = self._generate_text(text, _params)
-            generated.append(response)
             trace_str(response, f"Generated {i+1}/{len(texts)}")
 
         return generated
 
     async def agenerate_texts(
         self,
         texts: t.Sequence[str],
         params: t.Sequence[GenerateParams],
-    ) -> t.Sequence[str]:
-        generated: list[str] = []
-        max_requests = self.max_requests or len(texts)
-        for i in range(0, len(texts), max_requests or len(texts)):
-            chunk_texts = texts[i : i + max_requests]
-            chunk_params = params[i : i + max_requests]
-            chunk_generated = await asyncio.gather(
-                *[self._agenerate_text(text, _params) for text, _params in zip(chunk_texts, chunk_params)]
-            )
-            generated.extend(chunk_generated)
-
-            for i, (text, response) in enumerate(zip(chunk_texts, chunk_generated)):
-                trace_str(text, f"Text {i+1}/{len(texts)}")
-                trace_str(response, f"Generated {i+1}/{len(texts)}")
-
-        return generated
+    ) -> t.Sequence[GeneratedText]:
+        return self.generate_texts(texts, params)
 
 
-register_generator("litellm", LiteLLMGenerator)
+register_generator("vllm", VLLMGenerator)
```

### Comparing `rigging-1.1.2/rigging/generator/transformers_.py` & `rigging-1.2.0/rigging/generator/transformers_.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,26 @@
 import gc
 import typing as t
 
 import torch
 import transformers  # type: ignore
 from transformers import AutoModelForCausalLM, AutoTokenizer, PreTrainedTokenizer, TextGenerationPipeline
 
-from rigging.generator.base import GenerateParams, Generator, register_generator, trace_messages, trace_str
-from rigging.message import Message
+from rigging.generator.base import (
+    GeneratedMessage,
+    GeneratedText,
+    GenerateParams,
+    Generator,
+    register_generator,
+    trace_messages,
+    trace_str,
+)
+
+if t.TYPE_CHECKING:
+    from rigging.message import Message
 
 DEFAULT_MAX_TOKENS = 1024
 """Lifting the default max tokens from transformers"""
 
 
 class TransformersGenerator(Generator):
     """
@@ -124,15 +134,15 @@
         torch.cuda.empty_cache()
         return self
 
     def _generate(
         self,
         inputs: t.Sequence[str] | t.Sequence[t.Sequence[dict[str, str]]],
         params: t.Sequence[GenerateParams],
-    ) -> list[str]:
+    ) -> list[GeneratedText]:
         param_set = {p.model_dump_json() for p in params}
         if len(param_set) != 1:
             raise ValueError("All GenerateParams must be identical for this generator")
 
         # Generation Args + Fixups
         if self.params.max_tokens is None:
             self.params.max_tokens = DEFAULT_MAX_TOKENS
@@ -140,53 +150,56 @@
         kwargs = self.params.merge_with(params[0]).to_dict()
         if "max_tokens" in kwargs:
             kwargs["max_new_tokens"] = kwargs.pop("max_tokens")
         if any(k in kwargs for k in ["temperature", "top_k", "top_p"]):
             kwargs["do_sample"] = True
 
         outputs = self.pipeline(inputs, **kwargs)
-        return [output[-1]["generated_text"].strip() for output in outputs]
+
+        # TODO: We do strip() here as it's often needed, but I think
+        # we should return and standardize this behavior.
+        return [GeneratedText(text=o["generated_text"].strip()) for o in outputs]
 
     def generate_messages(
         self,
         messages: t.Sequence[t.Sequence[Message]],
         params: t.Sequence[GenerateParams],
-    ) -> t.Sequence[Message]:
+    ) -> t.Sequence[GeneratedMessage]:
         message_dicts = [[m.model_dump(include={"role", "content"}) for m in _messages] for _messages in messages]
         outputs = self._generate(message_dicts, params)
-        generated = [Message(role="assistant", content=output) for output in outputs]
+        generated = [o.to_generated_message() for o in outputs]
 
         for i, (in_messages, out_message) in enumerate(zip(messages, generated)):
             trace_messages(in_messages, f"Messages {i+1}/{len(in_messages)}")
             trace_messages([out_message], f"Response {i+1}/{len(in_messages)}")
 
         return generated
 
     async def agenerate_messages(
         self,
         messages: t.Sequence[t.Sequence[Message]],
         params: t.Sequence[GenerateParams],
-    ) -> t.Sequence[Message]:
+    ) -> t.Sequence[GeneratedMessage]:
         return self.generate_messages(messages, params)
 
     def generate_texts(
         self,
         texts: t.Sequence[str],
         params: t.Sequence[GenerateParams],
-    ) -> t.Sequence[str]:
+    ) -> t.Sequence[GeneratedText]:
         generated = self._generate(texts, params)
 
         for i, (text, response) in enumerate(zip(texts, generated)):
             trace_str(text, f"Text {i+1}/{len(texts)}")
             trace_str(response, f"Generated {i+1}/{len(texts)}")
 
         return generated
 
     async def agenerate_texts(
         self,
         texts: t.Sequence[str],
         params: t.Sequence[GenerateParams],
-    ) -> t.Sequence[str]:
+    ) -> t.Sequence[GeneratedText]:
         return self.generate_texts(texts, params)
 
 
 register_generator("transformers", TransformersGenerator)
```

### Comparing `rigging-1.1.2/rigging/logging.py` & `rigging-1.2.0/rigging/logging.py`

 * *Files identical despite different names*

### Comparing `rigging-1.1.2/rigging/message.py` & `rigging-1.2.0/rigging/message.py`

 * *Files identical despite different names*

### Comparing `rigging-1.1.2/rigging/model.py` & `rigging-1.2.0/rigging/model.py`

 * *Files identical despite different names*

### Comparing `rigging-1.1.2/rigging/parsing.py` & `rigging-1.2.0/rigging/parsing.py`

 * *Files identical despite different names*

### Comparing `rigging-1.1.2/rigging/prompt.py` & `rigging-1.2.0/rigging/prompt.py`

 * *Files identical despite different names*

### Comparing `rigging-1.1.2/rigging/tool.py` & `rigging-1.2.0/rigging/tool.py`

 * *Files identical despite different names*

### Comparing `rigging-1.1.2/PKG-INFO` & `rigging-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rigging
-Version: 1.1.2
+Version: 1.2.0
 Summary: LLM Interaction Framework
 Home-page: https://github.com/dreadnode/rigging
 License: MIT
 Author: Nick Landers
 Author-email: monoxgas@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

