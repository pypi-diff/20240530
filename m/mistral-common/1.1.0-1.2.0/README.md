# Comparing `tmp/mistral_common-1.1.0.tar.gz` & `tmp/mistral_common-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mistral_common-1.1.0.tar", max compression
+gzip compressed data, was "mistral_common-1.2.0.tar", max compression
```

## Comparing `mistral_common-1.1.0.tar` & `mistral_common-1.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    11339 2024-05-24 08:24:49.429905 mistral_common-1.1.0/LICENCE
--rw-r--r--   0        0        0     2971 2024-05-24 09:56:33.893366 mistral_common-1.1.0/README.md
--rw-r--r--   0        0        0     1289 2024-05-24 09:56:33.933324 mistral_common-1.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-24 08:23:05.965233 mistral_common-1.1.0/src/mistral_common/__init__.py
--rw-r--r--   0        0        0      261 2024-05-24 09:56:33.942009 mistral_common-1.1.0/src/mistral_common/base.py
--rw-r--r--   0        0        0   587404 2024-05-24 08:23:06.338148 mistral_common-1.1.0/src/mistral_common/data/mistral_instruct_tokenizer_240216.model.v2
--rw-r--r--   0        0        0   587404 2024-05-24 08:23:05.997657 mistral_common-1.1.0/src/mistral_common/data/mistral_instruct_tokenizer_240216.model.v3
--rw-r--r--   0        0        0   493443 2024-05-24 08:23:06.013826 mistral_common-1.1.0/src/mistral_common/data/tokenizer.model.v1
--rw-r--r--   0        0        0     1807 2024-05-24 08:23:04.706356 mistral_common-1.1.0/src/mistral_common/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-24 08:23:04.729841 mistral_common-1.1.0/src/mistral_common/protocol/__init__.py
--rw-r--r--   0        0        0      199 2024-05-24 08:23:04.721302 mistral_common-1.1.0/src/mistral_common/protocol/base.py
--rw-r--r--   0        0        0      400 2024-05-24 08:23:04.850885 mistral_common-1.1.0/src/mistral_common/protocol/embedding/request.py
--rw-r--r--   0        0        0      873 2024-05-24 08:23:04.833933 mistral_common-1.1.0/src/mistral_common/protocol/embedding/response.py
--rw-r--r--   0        0        0        0 2024-05-24 08:23:05.198296 mistral_common-1.1.0/src/mistral_common/protocol/instruct/__init__.py
--rw-r--r--   0        0        0     2173 2024-05-24 09:56:33.952798 mistral_common-1.1.0/src/mistral_common/protocol/instruct/messages.py
--rw-r--r--   0        0        0     7506 2024-05-24 09:56:33.959793 mistral_common-1.1.0/src/mistral_common/protocol/instruct/normalize.py
--rw-r--r--   0        0        0      986 2024-05-24 09:56:33.980403 mistral_common-1.1.0/src/mistral_common/protocol/instruct/request.py
--rw-r--r--   0        0        0     1918 2024-05-24 08:23:05.423807 mistral_common-1.1.0/src/mistral_common/protocol/instruct/response.py
--rw-r--r--   0        0        0     1043 2024-05-24 09:56:33.987559 mistral_common-1.1.0/src/mistral_common/protocol/instruct/tool_calls.py
--rw-r--r--   0        0        0    12976 2024-05-24 09:56:33.998965 mistral_common-1.1.0/src/mistral_common/protocol/instruct/validator.py
--rw-r--r--   0        0        0       73 2024-05-24 08:23:05.959141 mistral_common-1.1.0/src/mistral_common/protocol/utils.py
--rw-r--r--   0        0        0        0 2024-05-24 08:23:06.580639 mistral_common-1.1.0/src/mistral_common/py.typed
--rw-r--r--   0        0        0        0 2024-05-24 08:23:06.561184 mistral_common-1.1.0/src/mistral_common/tokens/__init__.py
--rw-r--r--   0        0        0      479 2024-05-24 09:56:34.014187 mistral_common-1.1.0/src/mistral_common/tokens/instruct/request.py
--rw-r--r--   0        0        0     2134 2024-05-24 09:56:34.021362 mistral_common-1.1.0/src/mistral_common/tokens/tokenizers/base.py
--rw-r--r--   0        0        0     5367 2024-05-24 09:56:34.029681 mistral_common-1.1.0/src/mistral_common/tokens/tokenizers/mistral.py
--rw-r--r--   0        0        0    12947 2024-05-24 09:56:34.037770 mistral_common-1.1.0/src/mistral_common/tokens/tokenizers/sentencepiece.py
--rw-r--r--   0        0        0      187 2024-05-24 08:23:06.552824 mistral_common-1.1.0/src/mistral_common/tokens/tokenizers/utils.py
--rw-r--r--   0        0        0     3572 1970-01-01 00:00:00.000000 mistral_common-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11339 2024-05-29 12:08:57.851065 mistral_common-1.2.0/LICENCE
+-rw-r--r--   0        0        0     2971 2024-05-29 12:08:55.503775 mistral_common-1.2.0/README.md
+-rw-r--r--   0        0        0     1289 2024-05-29 12:09:37.728062 mistral_common-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-29 12:07:19.826948 mistral_common-1.2.0/src/mistral_common/__init__.py
+-rw-r--r--   0        0        0      231 2024-05-29 12:07:19.823812 mistral_common-1.2.0/src/mistral_common/base.py
+-rw-r--r--   0        0        0   587404 2024-05-29 12:07:20.026312 mistral_common-1.2.0/src/mistral_common/data/mistral_instruct_tokenizer_240216.model.v2
+-rw-r--r--   0        0        0   587404 2024-05-29 12:07:20.034173 mistral_common-1.2.0/src/mistral_common/data/mistral_instruct_tokenizer_240216.model.v3
+-rw-r--r--   0        0        0   493443 2024-05-29 12:07:20.041123 mistral_common-1.2.0/src/mistral_common/data/tokenizer.model.v1
+-rw-r--r--   0        0        0     1807 2024-05-29 12:07:19.801150 mistral_common-1.2.0/src/mistral_common/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-29 12:07:19.913321 mistral_common-1.2.0/src/mistral_common/protocol/__init__.py
+-rw-r--r--   0        0        0      502 2024-05-29 12:07:19.836008 mistral_common-1.2.0/src/mistral_common/protocol/base.py
+-rw-r--r--   0        0        0      400 2024-05-29 12:07:19.934822 mistral_common-1.2.0/src/mistral_common/protocol/embedding/request.py
+-rw-r--r--   0        0        0      873 2024-05-29 12:07:19.938459 mistral_common-1.2.0/src/mistral_common/protocol/embedding/response.py
+-rw-r--r--   0        0        0        0 2024-05-29 12:07:20.012154 mistral_common-1.2.0/src/mistral_common/protocol/instruct/__init__.py
+-rw-r--r--   0        0        0     2198 2024-05-29 12:07:19.948027 mistral_common-1.2.0/src/mistral_common/protocol/instruct/messages.py
+-rw-r--r--   0        0        0     7598 2024-05-29 12:07:19.971891 mistral_common-1.2.0/src/mistral_common/protocol/instruct/normalize.py
+-rw-r--r--   0        0        0      828 2024-05-29 12:07:19.958912 mistral_common-1.2.0/src/mistral_common/protocol/instruct/request.py
+-rw-r--r--   0        0        0     1918 2024-05-29 12:07:19.962922 mistral_common-1.2.0/src/mistral_common/protocol/instruct/response.py
+-rw-r--r--   0        0        0     1044 2024-05-29 12:07:19.954151 mistral_common-1.2.0/src/mistral_common/protocol/instruct/tool_calls.py
+-rw-r--r--   0        0        0    13516 2024-05-29 12:07:19.967205 mistral_common-1.2.0/src/mistral_common/protocol/instruct/validator.py
+-rw-r--r--   0        0        0       73 2024-05-29 12:07:19.910317 mistral_common-1.2.0/src/mistral_common/protocol/utils.py
+-rw-r--r--   0        0        0        0 2024-05-29 12:07:20.118121 mistral_common-1.2.0/src/mistral_common/py.typed
+-rw-r--r--   0        0        0        0 2024-05-29 12:07:20.115214 mistral_common-1.2.0/src/mistral_common/tokens/__init__.py
+-rw-r--r--   0        0        0      644 2024-05-29 12:07:20.053936 mistral_common-1.2.0/src/mistral_common/tokens/instruct/request.py
+-rw-r--r--   0        0        0     2577 2024-05-29 12:07:20.106833 mistral_common-1.2.0/src/mistral_common/tokens/tokenizers/base.py
+-rw-r--r--   0        0        0     5338 2024-05-29 12:16:50.262388 mistral_common-1.2.0/src/mistral_common/tokens/tokenizers/mistral.py
+-rw-r--r--   0        0        0    15022 2024-05-29 12:26:20.892875 mistral_common-1.2.0/src/mistral_common/tokens/tokenizers/sentencepiece.py
+-rw-r--r--   0        0        0      187 2024-05-29 12:07:20.112220 mistral_common-1.2.0/src/mistral_common/tokens/tokenizers/utils.py
+-rw-r--r--   0        0        0     3572 1970-01-01 00:00:00.000000 mistral_common-1.2.0/PKG-INFO
```

### Comparing `mistral_common-1.1.0/LICENCE` & `mistral_common-1.2.0/LICENCE`

 * *Files identical despite different names*

### Comparing `mistral_common-1.1.0/README.md` & `mistral_common-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mistral_common-1.1.0/pyproject.toml` & `mistral_common-1.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mistral_common"
-version = "v1.1.0"
+version = "v1.2.0"
 description = ""
 authors = ["bam4d <bam4d@mistral.ai>"]
 readme = "README.md"
 packages = [{ include = "mistral_common", from = "src" }]
 
 [tool.ruff]
 lint.select = ["E", "F", "W", "Q", "I"]
```

### Comparing `mistral_common-1.1.0/src/mistral_common/data/mistral_instruct_tokenizer_240216.model.v2` & `mistral_common-1.2.0/src/mistral_common/data/mistral_instruct_tokenizer_240216.model.v2`

 * *Files identical despite different names*

### Comparing `mistral_common-1.1.0/src/mistral_common/data/mistral_instruct_tokenizer_240216.model.v3` & `mistral_common-1.2.0/src/mistral_common/data/mistral_instruct_tokenizer_240216.model.v3`

 * *Files identical despite different names*

### Comparing `mistral_common-1.1.0/src/mistral_common/data/tokenizer.model.v1` & `mistral_common-1.2.0/src/mistral_common/data/tokenizer.model.v1`

 * *Files identical despite different names*

### Comparing `mistral_common-1.1.0/src/mistral_common/exceptions.py` & `mistral_common-1.2.0/src/mistral_common/exceptions.py`

 * *Files identical despite different names*

### Comparing `mistral_common-1.1.0/src/mistral_common/protocol/embedding/response.py` & `mistral_common-1.2.0/src/mistral_common/protocol/embedding/response.py`

 * *Files identical despite different names*

### Comparing `mistral_common-1.1.0/src/mistral_common/protocol/instruct/messages.py` & `mistral_common-1.2.0/src/mistral_common/protocol/instruct/messages.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     content: Union[str, List[ContentChunk]]
 
 
 class AssistantMessage(BaseMessage):
     role: Literal[Roles.assistant] = Roles.assistant
     content: Optional[str] = None
     tool_calls: Optional[List[ToolCall]] = None
+    prefix: bool = False
 
 
 class FinetuningAssistantMessage(AssistantMessage):
     weight: Optional[float] = None
 
 
 class ToolMessage(BaseMessage):
```

### Comparing `mistral_common-1.1.0/src/mistral_common/protocol/instruct/normalize.py` & `mistral_common-1.2.0/src/mistral_common/protocol/instruct/normalize.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,26 +107,29 @@
             function=FunctionCall(name=tool_call.function.name, arguments=normalized_function_aruments),
             id=tool_call.id,
         )
 
     def _aggregate_assistant_messages(self, messages: List[UATS]) -> AssistantMessageType:
         aggregated_content: List[str] = []
         tool_calls: List[ToolCall] = []
+        prefix: bool = False
         for message in messages:
             assert isinstance(message, self._assistant_message_class), "Expected assistant message"
             if message.tool_calls is not None:
                 for tool_call in message.tool_calls:
                     normalized_tool_call = self._normalize_tool_call(tool_call)
                     tool_calls.append(normalized_tool_call)
             elif message.content:
                 aggregated_content.append(self._aggregate_content_chunks(message.content))
+            prefix |= message.prefix
 
         return self._assistant_message_class(
             content="\n\n".join(aggregated_content) if len(aggregated_content) else None,
             tool_calls=tool_calls or None,
+            prefix=prefix
         )
 
     def _aggregate_user_messages(self, messages: List[UATS]) -> UserMessageType:
         aggregated_content: List[str] = []
         for message in messages:
             assert isinstance(message, self._user_message_class), "Expected user message"
             content = self._aggregate_content_chunks(message.content)
```

### Comparing `mistral_common-1.1.0/src/mistral_common/protocol/instruct/response.py` & `mistral_common-1.2.0/src/mistral_common/protocol/instruct/response.py`

 * *Files identical despite different names*

### Comparing `mistral_common-1.1.0/src/mistral_common/protocol/instruct/tool_calls.py` & `mistral_common-1.2.0/src/mistral_common/protocol/instruct/tool_calls.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,8 +43,9 @@
 
 
 class ToolCall(MistralBase):
     id: str = "null"  # required for V3 tokenization
     type: ToolTypes = ToolTypes.function
     function: FunctionCall
 
+
 ToolType = TypeVar("ToolType", bound=Tool)
```

### Comparing `mistral_common-1.1.0/src/mistral_common/protocol/instruct/validator.py` & `mistral_common-1.2.0/src/mistral_common/protocol/instruct/validator.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     InvalidSystemPromptException,
     InvalidToolException,
     InvalidToolMessageException,
     InvalidToolSchemaException,
 )
 from mistral_common.protocol.instruct.messages import (
     UATS,
+    AssistantMessage,
     AssistantMessageType,
     FinetuningAssistantMessage,
     Roles,
     SystemMessageType,
     ToolMessageType,
     UserMessageType,
 )
@@ -153,14 +154,19 @@
             for tool_call in message.tool_calls:
                 self._validate_tool_call(tool_call, is_last_message=is_last_message)
 
         if self._mode == ValidationMode.finetuning and isinstance(message, FinetuningAssistantMessage):
             if message.weight is not None and message.weight not in [0, 1]:
                 raise InvalidAssistantMessageException("Assistant message weight must be either 0 or 1")
 
+        if message.prefix:
+            if not is_last_message:
+                raise InvalidAssistantMessageException("Assistant message with prefix True must be last message")
+            # note : we already validate that assistant messsage has content 3 lines up.
+
     def _validate_tool_calls_followed_by_tool_messages(self, messages: List[UATS]) -> None:
         """
         Checks:
         - That the number of tool calls and tool messages are the same
         - That the tool calls are followed by tool messages
         """
         prev_role = None
@@ -215,25 +221,27 @@
                     )
 
             previous_role = current_role
 
     def _validate_last_message(self, message: UATS) -> None:
         # The last message must be a user or tool message in serving mode or an assistant message in finetuning mode
         last_message_role = message.role
-        expected_roles = (
-            {Roles.user, Roles.tool}
-            if self._mode != ValidationMode.finetuning
-            else {Roles.assistant}
-        )
-
-        if last_message_role not in expected_roles:
-            expected_roles_str = ", ".join(role.value for role in expected_roles)
-            raise InvalidMessageStructureException(
-                f"Expected last role to be one of: [{expected_roles_str}] but got {last_message_role.value}"
-            )
+        if self._mode == ValidationMode.finetuning:
+            if last_message_role  != Roles.assistant:
+                raise InvalidMessageStructureException(
+                    f"Expected last role Assistant for finetuning but got {last_message_role.value}"
+                )
+        else:
+            bad_assistant = isinstance(message, AssistantMessage) and not message.prefix
+            bad_role = message.role not in {Roles.user, Roles.tool}
+            if bad_assistant and bad_role:
+                raise InvalidMessageStructureException(
+                    f"Expected last role User or Tool (or Assistant with prefix True) for serving"
+                    f" but got {last_message_role.value}"
+                )
 
     def _validate_message_list_structure(self, messages: List[UATS]) -> None:
         """
         Validates the structure of the list of messages
 
         For example the messages must be in the correct order of user/assistant/tool
         """
@@ -287,15 +295,14 @@
             raise InvalidRequestException("Tool call id has to be defined.")
 
         if not re.match(r"^[a-zA-Z0-9]{9}$", message.tool_call_id):
             raise InvalidToolMessageException(
                 f"Tool call id was {message.tool_call_id} but must be a-z, A-Z, 0-9, with a length of 9."
             )
 
-
     def _validate_tool_call(self, tool_call: ToolCall, is_last_message: bool) -> None:
         """
         Validate that the tool call has a valid ID
         """
         if tool_call.id != "null":
             if not re.match(r"^[a-zA-Z0-9]{9}$", tool_call.id):
                 raise InvalidFunctionCallException(
```

### Comparing `mistral_common-1.1.0/src/mistral_common/tokens/tokenizers/base.py` & `mistral_common-1.2.0/src/mistral_common/tokens/tokenizers/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 from abc import ABC, abstractmethod
 from enum import Enum
 from typing import Generic, List, Optional, TypeVar
 
 from mistral_common.base import MistralBase
-from mistral_common.tokens.instruct.request import InstructRequest
+from mistral_common.protocol.instruct.messages import AssistantMessageType
+from mistral_common.tokens.instruct.request import FIMRequest, InstructRequest
 
 
 class SpecialTokens(str, Enum):
     bos = "<s>"
     eos = "</s>"
     begin_inst = "[INST]"
     end_inst = "[/INST]"
     begin_tools = "[AVAILABLE_TOOLS]"
     end_tools = "[/AVAILABLE_TOOLS]"
     begin_tool_results = "[TOOL_RESULTS]"
     end_tool_results = "[/TOOL_RESULTS]"
     tool_calls = "[TOOL_CALLS]"
+    prefix = "[PREFIX]"
+    middle = "[MIDDLE]"
+    suffix = "[SUFFIX]"
 
 
 class Tokenized(MistralBase):
     """
     A tokenized InstructRequest
     """
 
     tokens: List[int]
     text: Optional[str] = None
+    prefix_ids: Optional[List[int]] = None
 
 
 class Tokenizer(ABC):
     @property
     @abstractmethod
     def n_words(self) -> int:
         """Vocabulary size"""
@@ -61,23 +66,28 @@
 
     @abstractmethod
     def to_string(self, tokens: List[int]) -> str:
         """Convert token ids to string"""
 
 
 InstructRequestType = TypeVar("InstructRequestType", bound=InstructRequest)
+FIMRequestType = TypeVar("FIMRequestType", bound=FIMRequest)
 TokenizedType = TypeVar("TokenizedType", bound=Tokenized)
 
 
-class InstructTokenizer(Generic[InstructRequestType, TokenizedType], ABC):
+class InstructTokenizer(Generic[InstructRequestType, FIMRequestType, TokenizedType, AssistantMessageType]):
     tokenizer: Tokenizer
 
-    def __init__(self, model_path: str):
-        """Init from model file"""
+    def __init__(self, tokenizer: Tokenizer) -> None:
+        """Init from tokenizer"""
 
     @abstractmethod
     def encode_instruct(self, request: InstructRequestType) -> TokenizedType:
         """Instruct request to Tokenized object"""
 
     @abstractmethod
     def decode(self, tokens: List[int]) -> str:
         """Convert token ids to string"""
+
+    @abstractmethod
+    def encode_fim(self, request: FIMRequestType) -> TokenizedType:
+        """FIM request to Tokenized object"""
```

### Comparing `mistral_common-1.1.0/src/mistral_common/tokens/tokenizers/mistral.py` & `mistral_common-1.2.0/src/mistral_common/tokens/tokenizers/mistral.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from mistral_common.protocol.instruct.normalize import InstructRequestNormalizer
 from mistral_common.protocol.instruct.request import ChatCompletionRequest
 from mistral_common.protocol.instruct.validator import (
     MistralRequestValidator,
     MistralRequestValidatorV3,
     ValidationMode,
 )
+from mistral_common.tokens.instruct.request import FIMRequest
 from mistral_common.tokens.tokenizers.base import (
     InstructRequest,
     InstructRequestType,
     InstructTokenizer,
     Tokenized,
     TokenizedType,
 )
@@ -32,21 +33,19 @@
     InstructTokenizerV2,
     InstructTokenizerV3,
     SentencePieceTokenizer,
 )
 
 
 class MistralTokenizer(
-    Generic[
-        UserMessageType, AssistantMessageType, ToolMessageType, SystemMessageType, TokenizedType
-    ]
+    Generic[UserMessageType, AssistantMessageType, ToolMessageType, SystemMessageType, TokenizedType]
 ):
     def __init__(
         self,
-        instruct_tokenizer: InstructTokenizer[InstructRequest, TokenizedType],
+        instruct_tokenizer: InstructTokenizer[InstructRequest, FIMRequest, TokenizedType, AssistantMessageType],
         validator: MistralRequestValidator[UserMessageType, AssistantMessageType, ToolMessageType, SystemMessageType],
         request_normalizer: InstructRequestNormalizer[
             UserMessageType, AssistantMessageType, ToolMessageType, SystemMessageType, InstructRequestType
         ],
     ):
         self._chat_completion_request_validator = validator
         self._instruct_request_normalizer = request_normalizer
@@ -80,30 +79,30 @@
         model_name_to_tokenizer_cls: Dict[str, Callable[[], MistralTokenizer]] = {
             "open-mistral-7b": MistralTokenizer.v1,
             "open-mixtral-8x7b": MistralTokenizer.v1,
             "mistral-embed": MistralTokenizer.v1,
             "mistral-small": MistralTokenizer.v2,
             "mistral-large": MistralTokenizer.v2,
             "open-mixtral-8x22b": MistralTokenizer.v3,
+            "codestral-22b": MistralTokenizer.v3,
         }
 
         # Prefix search the model name mapping
         for model_name, tokenizer_cls in model_name_to_tokenizer_cls.items():
             if model_name in model:
                 return tokenizer_cls()
 
         raise TokenizerException(f"Unrecognized model: {model}")
 
     @classmethod
     def from_file(cls, tokenizer_filename: str, mode: ValidationMode = ValidationMode.test) -> MistralTokenizer:
         """
         Depending on which model we are loading, tokenization and validation might be different. 💩
         """
-
-        if tokenizer_filename.endswith(".model.v1"):
+        if tokenizer_filename.endswith(".model.v1") or tokenizer_filename.endswith(".model"):
             return MistralTokenizer(
                 InstructTokenizerV1(SentencePieceTokenizer(tokenizer_filename)),
                 validator=MistralRequestValidator(mode=mode),
                 request_normalizer=InstructRequestNormalizer.normalizer(),
             )
         elif tokenizer_filename.endswith(".model.v2"):
             return MistralTokenizer(
@@ -113,23 +112,20 @@
             )
         elif tokenizer_filename.endswith(".model.v3"):
             return MistralTokenizer(
                 InstructTokenizerV3(SentencePieceTokenizer(tokenizer_filename)),
                 validator=MistralRequestValidatorV3(mode=mode),
                 request_normalizer=InstructRequestNormalizer.normalizer(),
             )
-        elif tokenizer_filename.endswith(".model"):
-            return MistralTokenizer(
-                InstructTokenizerV1(SentencePieceTokenizer(tokenizer_filename)),
-                validator=MistralRequestValidator(mode=mode),
-                request_normalizer=InstructRequestNormalizer.normalizer(),
-            )
         else:
             raise TokenizerException(f"Unrecognized tokenizer filename: {tokenizer_filename}")
 
     def encode_chat_completion(self, request: ChatCompletionRequest[UATS]) -> Tokenized:
         validated_request = self._chat_completion_request_validator.validate_request(request)
         instruct_request = self._instruct_request_normalizer.from_chat_completion_request(validated_request)
         return self.instruct_tokenizer.encode_instruct(instruct_request)
 
+    def encode_fim(self, request: FIMRequest) -> Tokenized:
+        return self.instruct_tokenizer.encode_fim(request)
+
     def decode(self, tokens: List[int]) -> str:
         return self.instruct_tokenizer.decode(tokens)
```

### Comparing `mistral_common-1.1.0/src/mistral_common/tokens/tokenizers/sentencepiece.py` & `mistral_common-1.2.0/src/mistral_common/tokens/tokenizers/sentencepiece.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import json
 import logging
 import os
 from abc import abstractmethod
 from functools import cached_property
-from typing import Any, Dict, List, Optional, Set, Tuple
+from typing import Any, Dict, Generic, List, Optional, Set, Tuple
 
 from mistral_common.exceptions import TokenizerException
 from mistral_common.protocol.instruct.messages import (
     AssistantMessage,
+    AssistantMessageType,
     ToolMessage,
     UserMessage,
 )
 from mistral_common.protocol.instruct.tool_calls import Tool, ToolCall
-from mistral_common.tokens.instruct.request import InstructRequest
+from mistral_common.tokens.instruct.request import FIMRequest, InstructRequest
 from mistral_common.tokens.tokenizers.base import (
+    FIMRequestType,
+    InstructRequestType,
     InstructTokenizer,
     SpecialTokens,
     Tokenized,
+    TokenizedType,
     Tokenizer,
 )
 from sentencepiece import SentencePieceProcessor
 
 
 class SentencePieceTokenizer(Tokenizer):
     def __init__(self, model_path: str) -> None:
@@ -90,17 +94,20 @@
 
         if curr_tokens:
             text += "".join([self.id_to_piece(tok) for tok in curr_tokens])
 
         return text
 
 
-class InstructTokenizerBase(InstructTokenizer):
+class InstructTokenizerBase(
+    InstructTokenizer, Generic[InstructRequestType, FIMRequestType, TokenizedType, AssistantMessageType]
+):
     def __init__(self, tokenizer: Tokenizer):
         self.tokenizer = tokenizer
+        super().__init__(tokenizer)
 
     def start(self) -> List[int]:
         return [self.tokenizer.bos_id]
 
     @staticmethod
     def find_first_last_user(request: InstructRequest) -> Tuple[int, int]:
         # find last user message
@@ -122,23 +129,24 @@
         is_first: bool,
         system_prompt: Optional[str] = None,
     ) -> List[int]:
         ...
 
     @abstractmethod
     def encode_tool_message(self, message: ToolMessage, is_before_last_user_message: bool) -> List[int]:
-        ...
+        raise NotImplementedError("Tool message not implemented")
 
     @abstractmethod
-    def encode_assistant_message(self, message: AssistantMessage, is_before_last_user_message: bool) -> List[int]:
-        ...
+    def encode_assistant_message(self, message: AssistantMessageType, is_before_last_user_message: bool) -> List[int]:
+        raise NotImplementedError("Assistant message not implemented")
 
-    def encode_instruct(self, request: InstructRequest) -> Tokenized:
+    def encode_instruct(self, request: InstructRequest[AssistantMessageType, Tool]) -> Tokenized:
         # init at bos
         tokens = self.start()
+        prefix_ids: Optional[List[int]] = None
         # find last user message
         first_user_idx, last_user_idx = self.find_first_last_user(request)
         for msg_idx, msg in enumerate(request.messages):
             if isinstance(msg, UserMessage):
                 new_tokens = self.encode_user_message(
                     msg,
                     request.available_tools,
@@ -146,71 +154,82 @@
                     msg_idx == first_user_idx,
                     system_prompt=request.system_prompt,
                 )
             elif isinstance(msg, ToolMessage):
                 new_tokens = self.encode_tool_message(msg, msg_idx < last_user_idx)
             elif isinstance(msg, AssistantMessage):
                 new_tokens = self.encode_assistant_message(msg, msg_idx < last_user_idx)
+                if msg_idx == len(request.messages) - 1:
+                    prefix_ids = new_tokens
 
             tokens.extend(new_tokens)
 
-        return Tokenized(tokens=tokens, text=self.tokenizer.to_string(tokens))
+        return Tokenized(tokens=tokens, text=self.tokenizer.to_string(tokens), prefix_ids=prefix_ids)
 
     def decode(self, tokens: List[int]) -> str:
         return self.tokenizer.decode(tokens)
 
 
-class InstructTokenizerV1(InstructTokenizerBase):
+class InstructTokenizerV1(
+    InstructTokenizerBase, Generic[InstructRequestType, FIMRequestType, TokenizedType, AssistantMessageType]
+):
     def encode_user_message(
         self,
         message: UserMessage,
         available_tools: Optional[List[Tool]],
         is_last: bool,
         is_first: bool,
         system_prompt: Optional[str] = None,
     ) -> List[int]:
         assert message.content is not None
-        assert isinstance(message.content, str), "Message content must be nornmalized"
+        assert isinstance(message.content, str), "Message content must be normalized"
         content = ""
         if is_first and system_prompt:
             content = system_prompt + "\n\n" + message.content
         else:
             content = message.content
 
         message_txt = f"[INST] {content} [/INST]"
         curr_tokens = self.tokenizer.encode(message_txt, bos=False, eos=False)
         return curr_tokens
 
     def encode_tool_message(self, message: ToolMessage, is_before_last_user_message: bool) -> List[int]:
         raise TokenizerException("Tools not implemented for tokenizer V1")
 
-    def encode_assistant_message(self, message: AssistantMessage, is_before_last_user_message: bool) -> List[int]:
+    def encode_assistant_message(self, message: AssistantMessageType, is_before_last_user_message: bool) -> List[int]:
         assert isinstance(message, AssistantMessage), message
         if message.tool_calls is not None and len(message.tool_calls) > 0:
             raise TokenizerException("Tools not implemented for tokenizer V1")
         elif message.content:
             curr_tokens = self.tokenizer.encode(message.content, bos=False, eos=False)
         else:
             raise TokenizerException(f"{message.content} // {message.tool_calls}")
-
-        curr_tokens.append(self.tokenizer.eos_id)
+        if not message.prefix:
+            curr_tokens.append(self.tokenizer.eos_id)
         return curr_tokens
 
+    def encode_fim(self, request: FIMRequest) -> Tokenized:
+        raise TokenizerException("FIM not available for tokenizer V1")
+
 
-class InstructTokenizerV2(InstructTokenizerBase):
+class InstructTokenizerV2(
+    InstructTokenizerV1, Generic[InstructRequestType, FIMRequestType, TokenizedType, AssistantMessageType]
+):
     def __init__(self, tokenizer: Tokenizer):
         super().__init__(tokenizer)
-
         self.BEGIN_INST = self.tokenizer.get_control_token(SpecialTokens.begin_inst.value)
         self.END_INST = self.tokenizer.get_control_token(SpecialTokens.end_inst.value)
         self.BEGIN_AVAILABLE_TOOLS = self.tokenizer.get_control_token(SpecialTokens.begin_tools.value)
         self.END_AVAILABLE_TOOLS = self.tokenizer.get_control_token(SpecialTokens.end_tools.value)
         self.BEGIN_TOOL_RESULTS = self.tokenizer.get_control_token(SpecialTokens.begin_tool_results.value)
         self.END_TOOL_RESULTS = self.tokenizer.get_control_token(SpecialTokens.end_tool_results.value)
         self.TOOL_CALLS = self.tokenizer.get_control_token(SpecialTokens.tool_calls.value)
+        self.BOS = self.tokenizer.get_control_token(SpecialTokens.bos.value)
+        self.PREFIX = self.tokenizer.get_control_token(SpecialTokens.prefix.value)
+        self.SUFFIX = self.tokenizer.get_control_token(SpecialTokens.suffix.value)
 
     def encode_user_message(
         self,
         message: UserMessage,
         available_tools: Optional[List[Tool]],
         is_last: bool,
         is_first: bool,
@@ -277,15 +296,15 @@
         Bit of a hack due to the way function calls are tokenized
         """
         return {
             "name": tool_call.function.name,
             "arguments": self._parse_json_content(tool_call.function.arguments),
         }
 
-    def encode_assistant_message(self, message: AssistantMessage, is_before_last_user_message: bool) -> List[int]:
+    def encode_assistant_message(self, message: AssistantMessageType, is_before_last_user_message: bool) -> List[int]:
         if message.tool_calls is not None and len(message.tool_calls) > 0:
             if is_before_last_user_message:
                 # don't tokenize tool call before last user message
                 return []
 
             prepared_tool_calls = []
             for tool_call in message.tool_calls:
@@ -297,23 +316,49 @@
                 *self.tokenizer.encode(tool_call_str, bos=False, eos=False),
             ]
         elif message.content:
             curr_tokens = self.tokenizer.encode(message.content, bos=False, eos=False)
         else:
             raise TokenizerException(f"Invalid assistant message: {message.content}")
 
-        curr_tokens.append(self.tokenizer.eos_id)
+        if not message.prefix:
+            curr_tokens.append(self.tokenizer.eos_id)
         return curr_tokens
 
+    def _encode_infilling(self, text: str) -> List[int]:
+        """
+        Remove prefix space in the case of SentencePieceTokenizers
+        Thanks Fabian !
+        """
+
+        return self.tokenizer.encode("☺" + text, bos=False, eos=False)[2:]
+
+    def encode_fim(self, request: FIMRequest) -> Tokenized:
+        prefix_tokens = self.tokenizer.encode(request.prompt, bos=False, eos=False)
+        suffix_tokens = self._encode_infilling(request.suffix) if request.suffix else []
+        tokens = [
+            self.BOS,
+            self.SUFFIX,
+            *suffix_tokens,
+            self.PREFIX,
+            *prefix_tokens,
+        ]
+        return Tokenized(tokens=tokens, text=self.tokenizer.to_string(tokens))
 
-class InstructTokenizerV3(InstructTokenizerV2):
+
+class InstructTokenizerV3(
+    InstructTokenizerV2, Generic[InstructRequestType, FIMRequestType, TokenizedType, AssistantMessageType]
+):
     """
     The only difference with V3 tokenizer is that it encodes the tool messages differently
     """
 
+    def __init__(self, tokenizer: Tokenizer):
+        super().__init__(tokenizer)
+
     def _prepare_function_call(self, tool_call: ToolCall) -> Dict[str, Any]:
         function_call = {
             "name": tool_call.function.name,
             "arguments": self._parse_json_content(tool_call.function.arguments),
         }
 
         if tool_call.id and tool_call.id != "null":
@@ -338,12 +383,12 @@
         curr_tokens = [
             self.BEGIN_TOOL_RESULTS,
             *self.tokenizer.encode(tool_result_str, bos=False, eos=False),
             self.END_TOOL_RESULTS,
         ]
         return curr_tokens
 
-    def encode_assistant_message(self, message: AssistantMessage, is_before_last_user_message: bool) -> List[int]:
+    def encode_assistant_message(self, message: AssistantMessageType, is_before_last_user_message: bool) -> List[int]:
         """
         Same as V2 but always encode tool history
         """
         return super().encode_assistant_message(message, False)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mistral_common-1.1.0/PKG-INFO` & `mistral_common-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistral_common
-Version: 1.1.0
+Version: 1.2.0
 Summary: 
 Author: bam4d
 Author-email: bam4d@mistral.ai
 Requires-Python: >=3.8.10,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

