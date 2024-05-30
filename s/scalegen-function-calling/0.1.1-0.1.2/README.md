# Comparing `tmp/scalegen-function-calling-0.1.1.tar.gz` & `tmp/scalegen-function-calling-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalegen-function-calling-0.1.1.tar", last modified: Sun May 19 17:12:40 2024, max compression
+gzip compressed data, was "scalegen-function-calling-0.1.2.tar", last modified: Wed May 29 20:23:29 2024, max compression
```

## Comparing `scalegen-function-calling-0.1.1.tar` & `scalegen-function-calling-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 tejeshbhalla   (501) staff       (20)        0 2024-05-19 17:12:40.150380 scalegen-function-calling-0.1.1/
--rw-r--r--   0 tejeshbhalla   (501) staff       (20)     1067 2024-05-11 11:20:13.000000 scalegen-function-calling-0.1.1/LICENSE
--rw-r--r--   0 tejeshbhalla   (501) staff       (20)     2272 2024-05-19 17:12:40.150265 scalegen-function-calling-0.1.1/PKG-INFO
--rw-r--r--   0 tejeshbhalla   (501) staff       (20)     1720 2024-05-19 17:12:24.000000 scalegen-function-calling-0.1.1/README.md
-drwxr-xr-x   0 tejeshbhalla   (501) staff       (20)        0 2024-05-19 17:12:40.149166 scalegen-function-calling-0.1.1/scalegen_function_calling/
--rw-r--r--   0 tejeshbhalla   (501) staff       (20)       38 2024-05-19 16:46:41.000000 scalegen-function-calling-0.1.1/scalegen_function_calling/__init__.py
--rw-r--r--   0 tejeshbhalla   (501) staff       (20)    20128 2024-05-19 16:46:01.000000 scalegen-function-calling-0.1.1/scalegen_function_calling/client.py
-drwxr-xr-x   0 tejeshbhalla   (501) staff       (20)        0 2024-05-19 17:12:40.150085 scalegen-function-calling-0.1.1/scalegen_function_calling.egg-info/
--rw-r--r--   0 tejeshbhalla   (501) staff       (20)     2272 2024-05-19 17:12:40.000000 scalegen-function-calling-0.1.1/scalegen_function_calling.egg-info/PKG-INFO
--rw-r--r--   0 tejeshbhalla   (501) staff       (20)      344 2024-05-19 17:12:40.000000 scalegen-function-calling-0.1.1/scalegen_function_calling.egg-info/SOURCES.txt
--rw-r--r--   0 tejeshbhalla   (501) staff       (20)        1 2024-05-19 17:12:40.000000 scalegen-function-calling-0.1.1/scalegen_function_calling.egg-info/dependency_links.txt
--rw-r--r--   0 tejeshbhalla   (501) staff       (20)        7 2024-05-19 17:12:40.000000 scalegen-function-calling-0.1.1/scalegen_function_calling.egg-info/requires.txt
--rw-r--r--   0 tejeshbhalla   (501) staff       (20)       26 2024-05-19 17:12:40.000000 scalegen-function-calling-0.1.1/scalegen_function_calling.egg-info/top_level.txt
--rw-r--r--   0 tejeshbhalla   (501) staff       (20)       38 2024-05-19 17:12:40.150423 scalegen-function-calling-0.1.1/setup.cfg
--rw-r--r--   0 tejeshbhalla   (501) staff       (20)      833 2024-05-19 17:12:32.000000 scalegen-function-calling-0.1.1/setup.py
+drwxr-xr-x   0 tejeshbhalla   (501) staff       (20)        0 2024-05-29 20:23:29.540848 scalegen-function-calling-0.1.2/
+-rw-r--r--   0 tejeshbhalla   (501) staff       (20)     1067 2024-05-29 20:09:23.000000 scalegen-function-calling-0.1.2/LICENSE
+-rw-r--r--   0 tejeshbhalla   (501) staff       (20)     2913 2024-05-29 20:23:29.540729 scalegen-function-calling-0.1.2/PKG-INFO
+-rw-r--r--   0 tejeshbhalla   (501) staff       (20)     2341 2024-05-29 20:09:23.000000 scalegen-function-calling-0.1.2/README.md
+drwxr-xr-x   0 tejeshbhalla   (501) staff       (20)        0 2024-05-29 20:23:29.539230 scalegen-function-calling-0.1.2/scalegen_function_calling/
+-rw-r--r--   0 tejeshbhalla   (501) staff       (20)       38 2024-05-29 20:09:23.000000 scalegen-function-calling-0.1.2/scalegen_function_calling/__init__.py
+-rw-r--r--   0 tejeshbhalla   (501) staff       (20)    21199 2024-05-29 20:19:35.000000 scalegen-function-calling-0.1.2/scalegen_function_calling/client.py
+drwxr-xr-x   0 tejeshbhalla   (501) staff       (20)        0 2024-05-29 20:23:29.540536 scalegen-function-calling-0.1.2/scalegen_function_calling.egg-info/
+-rw-r--r--   0 tejeshbhalla   (501) staff       (20)     2913 2024-05-29 20:23:29.000000 scalegen-function-calling-0.1.2/scalegen_function_calling.egg-info/PKG-INFO
+-rw-r--r--   0 tejeshbhalla   (501) staff       (20)      344 2024-05-29 20:23:29.000000 scalegen-function-calling-0.1.2/scalegen_function_calling.egg-info/SOURCES.txt
+-rw-r--r--   0 tejeshbhalla   (501) staff       (20)        1 2024-05-29 20:23:29.000000 scalegen-function-calling-0.1.2/scalegen_function_calling.egg-info/dependency_links.txt
+-rw-r--r--   0 tejeshbhalla   (501) staff       (20)        7 2024-05-29 20:23:29.000000 scalegen-function-calling-0.1.2/scalegen_function_calling.egg-info/requires.txt
+-rw-r--r--   0 tejeshbhalla   (501) staff       (20)       26 2024-05-29 20:23:29.000000 scalegen-function-calling-0.1.2/scalegen_function_calling.egg-info/top_level.txt
+-rw-r--r--   0 tejeshbhalla   (501) staff       (20)       38 2024-05-29 20:23:29.540907 scalegen-function-calling-0.1.2/setup.cfg
+-rw-r--r--   0 tejeshbhalla   (501) staff       (20)      834 2024-05-29 20:21:47.000000 scalegen-function-calling-0.1.2/setup.py
```

### Comparing `scalegen-function-calling-0.1.1/LICENSE` & `scalegen-function-calling-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scalegen-function-calling-0.1.1/scalegen_function_calling/client.py` & `scalegen-function-calling-0.1.2/scalegen_function_calling/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 import json
-from openai.types.chat import ChatCompletionMessage, ChatCompletionMessageToolCall,ChatCompletion
+from openai.types.chat import (
+    ChatCompletionMessage,
+    ChatCompletionMessageToolCall,
+    ChatCompletion,
+)
 from openai.types.chat.chat_completion_message_tool_call import Function
 from openai.types.chat.chat_completion_chunk import (
     ChatCompletionChunk,
     ChoiceDeltaToolCall,
     ChoiceDelta,
-    ChoiceDelta,
     ChoiceDeltaToolCallFunction,
     Choice as Choice_Chunk,
 )
 from openai.types.completion_usage import CompletionUsage
 from openai.types.chat.chat_completion import Choice
 from openai import OpenAI, AsyncOpenAI
 import uuid
 from typing import List, Dict, Any, Union, Tuple
 import re
 import time
+
+
 TOOL_SYSTEM_PROMPT = (
     "You have access to the following tools:\n{tool_text}"
     "Use the following format if using a tool:\n"
     "```\n"
     "Action: tool name (one of [{tool_names}]).\n"
     "Action Input: the input to the tool, in a JSON format representing the kwargs (e.g. ```{example_input}```)\n"
     "```\n"
 )
 
-def generate_json_format_example(tool_parameters: Dict[str, Any], examples: List[Dict[str, Any]]) -> str:
+
+def generate_json_format_example(
+    tool_parameters: Dict[str, Any], examples: List[Dict[str, Any]]
+) -> str:
     example_input = '{"input": "hello world", "num_beams": 5}'  # Default example input
     if examples:
         # Use the first example as the example input
         example_input = json.dumps(examples[0])
     else:
         example_kwargs = {}
         for name, param in tool_parameters.items():
@@ -38,25 +46,34 @@
                 example_value = 1
             elif param.get("type") == "boolean":
                 example_value = True
             example_kwargs[name] = example_value
         example_input = json.dumps(example_kwargs)
     return example_input
 
+
 def default_tool_formatter(tools: List[Dict[str, Any]]) -> str:
     tool_text = ""
     tool_names = []
     example_inputs = []
     for tool in tools:
         param_text = ""
         parameters = tool["function"]["parameters"]
         for name, param in parameters.get("properties", {}).items():
             required = ", required" if name in parameters.get("required", []) else ""
-            enum = ", should be one of [{}]".format(", ".join(param["enum"])) if param.get("enum", None) else ""
-            items = ", where each item should be {}".format(param["items"].get("type", "")) if param.get("items") else ""
+            enum = (
+                ", should be one of [{}]".format(", ".join(param["enum"]))
+                if param.get("enum", None)
+                else ""
+            )
+            items = (
+                ", where each item should be {}".format(param["items"].get("type", ""))
+                if param.get("items")
+                else ""
+            )
             param_text += "  - {name} ({type}{required}): {desc}{enum}{items}\n".format(
                 name=name,
                 type=param.get("type", ""),
                 required=required,
                 desc=param.get("description", ""),
                 enum=enum,
                 items=items,
@@ -64,15 +81,17 @@
 
         tool_text += "> Tool Name: {name}\nTool Description: {desc}\nTool Args:\n{args}\n".format(
             name=tool["function"]["name"],
             desc=tool["function"].get("description", ""),
             args=param_text,
         )
         tool_names.append(tool["function"]["name"])
-        example_inputs.append(generate_json_format_example(parameters.get("properties", {}), []))
+        example_inputs.append(
+            generate_json_format_example(parameters.get("properties", {}), [])
+        )
 
     if not tool_text:
         return "No tools available."
     example_input_text = " or ".join(example_inputs)
 
     return TOOL_SYSTEM_PROMPT.format(
         tool_text=tool_text,
@@ -104,19 +123,19 @@
 
         if isinstance(client, OpenAI):
             self.chat.completions.create = self.chat_completion
 
         if isinstance(client, AsyncOpenAI):
             self.chat.completions.create = self.chat_completion_async
 
-
-    async def format_async_chunks(self, response,model):
+    async def format_async_chunks(self, response, model: str):
         is_tool = False
-        function_name = ""
+        function_name: str = ""
         is_tool_arg = False
+        
         async for chunk in response:
             content = chunk.choices[0].delta.content
             if content == None:
                 continue
             if content == "Action":
                 is_tool = True
                 continue
@@ -195,15 +214,15 @@
                     system_fingerprint=None,
                     usage=None,
                 )
 
             if content and "}" in content:
                 is_tool_arg = False
 
-    def format_chunks(self, response,model):
+    def format_chunks(self, response, model):
         is_tool = False
         function_name = ""
         is_tool_arg = False
         for chunk in response:
             content = chunk.choices[0].delta.content
             if content == None:
                 continue
@@ -286,21 +305,19 @@
                     system_fingerprint=None,
                     usage=None,
                 )
 
             if content and "}" in content:
                 is_tool_arg = False
 
-
-
     async def chat_completion_async(
         self,
         model: str,
         messages: List[Dict[str, Any]],
-        tools: List[Dict[str, Any]]=[],
+        tools: List[Dict[str, Any]] = [],
         tool_choice: Union[str, Dict[str, Any]] = "auto",
         *args,
         **kwargs,
     ):
 
         system_message = next(
             (msg for msg in messages if msg.get("role") == "system"), None
@@ -312,220 +329,229 @@
             else "You are a helpful assistant. You have access to the following tools:\n"
         )
 
         system_prompt += default_tool_formatter(tools)
 
         messages = [{"role": "system", "content": system_prompt}] + messages
 
-
         if tool_choice != "auto" and tool_choice["type"] == "function":
             function = tool_choice["function"]
             if messages[-1]["role"] == "user":
-                messages[-1][
-                    "content"
-                ] += f",  utilize the tool {function['name']} \n"
-
+                messages[-1]["content"] += f",  utilize the tool {function['name']} \n"
 
         transformed_messages = []
         for msg in messages:
             if msg.get("role") == "tool":
-                
-                msg['content']=str({"response": msg["content"]})
+
+                msg["content"] = str({"response": msg["content"]})
                 transformed_messages.append(msg)
             elif msg.get("role") == "assistant" and isinstance(
                 msg.get("content"), Function
             ):
                 function_content = msg["content"]
                 transformed_messages.append(
                     {
                         "role": "assistant",
                         "content": f"Action: {function_content.name}\nAction Input: {function_content.arguments}",
                     }
                 )
+
+            elif msg.get("role") == "assistant" and not msg.get("content"):
+                tool = msg['tool_calls'][0]
+                function_content = tool['function']
+                transformed_messages.append(
+                    {
+                        "role": "assistant",
+                        "content": f"Action: {function_content['name']}\nAction Input: {function_content['arguments']}",
+                    }
+                )
+
             elif msg.get("role") == "assistant" and isinstance(
                 msg.get("content"), ChatCompletionMessage
             ):
-               content= msg.get("content")
-               if not content.content:
-                tool=content.tool_calls[0]
-                function_content=tool.function
-                transformed_messages.append(
-                      {
-                          "role": "assistant",
-                          "content": f"Action: {function_content.name}\nAction Input: {function_content.arguments}",
-                      }
-                  )
-               else:
-                transformed_messages.append(
-                      {
-                          "role": "assistant",
-                          "content": content.content,
-                      }
-                  )
+                content = msg.get("content")
+                if not content.content:
+                    tool = content.tool_calls[0]
+                    function_content = tool.function
+                    transformed_messages.append(
+                        {
+                            "role": "assistant",
+                            "content": f"Action: {function_content.name}\nAction Input: {function_content.arguments}",
+                        }
+                    )
+                else:
+                    transformed_messages.append(
+                        {
+                            "role": "assistant",
+                            "content": content.content,
+                        }
+                    )
             else:
                 transformed_messages.append(msg)
 
         response = await self.client.chat.completions.create(
             model=model, messages=transformed_messages, *args, **kwargs
         )
 
         if kwargs.get("stream") and kwargs["stream"] is True:
-            return self.format_async_chunks(response,model)
+            return self.format_async_chunks(response, model)
 
         if response.choices:
             choice = response.choices[0].message
             extracted_info = default_tool_extractor(choice.content)
             if isinstance(extracted_info, tuple):
                 tool_name, tool_args = extracted_info
                 tool_call = ChatCompletionMessageToolCall(
                     id=str(uuid.uuid4()),
                     function=Function(name=tool_name, arguments=tool_args),
                     type="function",
                 )
 
-                message= ChatCompletionMessage(
+                message = ChatCompletionMessage(
                     content=None, role="assistant", tool_calls=[tool_call]
                 )
                 return ChatCompletion(
                     id=str(uuid.uuid4()),
                     choices=[
                         Choice(
-                            finish_reason='tool_calls',
+                            finish_reason="tool_calls",
                             index=0,
                             logprobs=None,
-                            message=message
+                            message=message,
                         )
                     ],
                     created=int(time.time()),
                     model=model,
-                    object='chat.completion',
+                    object="chat.completion",
                     system_fingerprint=None,
                     usage=CompletionUsage(
                         completion_tokens=0,  # Assuming no tokens used for simplicity
                         prompt_tokens=0,  # Assuming no tokens used for simplicity
-                        total_tokens=0  # Assuming no tokens used for simplicity
-                    )
+                        total_tokens=0,  # Assuming no tokens used for simplicity
+                    ),
                 )
             return response
         return response
 
     def chat_completion(
         self,
         model: str,
         messages: List[Dict[str, Any]],
-        tools: List[Dict[str, Any]]=[],
+        tools: List[Dict[str, Any]] = [],
         tool_choice: Union[str, Dict[str, Any]] = "auto",
         *args,
         **kwargs,
     ):
 
-        
-
-
         system_message = next(
             (msg for msg in messages if msg.get("role") == "system"), None
         )
 
         system_prompt = (
             system_message["content"]
             if system_message
             else "You are a helpful assistant. You have access to the following tools:\n"
         )
 
         system_prompt += default_tool_formatter(tools)
 
         messages = [{"role": "system", "content": system_prompt}] + messages
 
-
         if tool_choice != "auto" and tool_choice["type"] == "function":
             function = tool_choice["function"]
             if messages[-1]["role"] == "user":
-                messages[-1][
-                    "content"
-                ] += f",  utilize the tool {function['name']} \n"
-
+                messages[-1]["content"] += f",  utilize the tool {function['name']} \n"
 
         transformed_messages = []
         for msg in messages:
             if msg.get("role") == "tool":
-                
-                msg['content']=str({"response": msg["content"]})
+
+                msg["content"] = str({"response": msg["content"]})
                 transformed_messages.append(msg)
             elif msg.get("role") == "assistant" and isinstance(
                 msg.get("content"), Function
             ):
                 function_content = msg["content"]
                 transformed_messages.append(
                     {
                         "role": "assistant",
                         "content": f"Action: {function_content.name}\nAction Input: {function_content.arguments}",
                     }
                 )
+            elif msg.get("role") == "assistant" and not msg.get("content"):
+                tool = msg['tool_calls'][0]
+                function_content = tool['function']
+                transformed_messages.append(
+                    {
+                        "role": "assistant",
+                        "content": f"Action: {function_content['name']}\nAction Input: {function_content['arguments']}",
+                    }
+                )
+                
             elif msg.get("role") == "assistant" and isinstance(
                 msg.get("content"), ChatCompletionMessage
             ):
-               content= msg.get("content")
-               if not content.content:
-                tool=content.tool_calls[0]
-                function_content=tool.function
-                transformed_messages.append(
-                      {
-                          "role": "assistant",
-                          "content": f"Action: {function_content.name}\nAction Input: {function_content.arguments}",
-                      }
-                  )
-               else:
-                transformed_messages.append(
-                      {
-                          "role": "assistant",
-                          "content": content.content,
-                      }
-                  )
+                content = msg.get("content")
+                if not content.content:
+                    tool = content.tool_calls[0]
+                    function_content = tool.function
+                    transformed_messages.append(
+                        {
+                            "role": "assistant",
+                            "content": f"Action: {function_content.name}\nAction Input: {function_content.arguments}",
+                        }
+                    )
+                else:
+                    transformed_messages.append(
+                        {
+                            "role": "assistant",
+                            "content": content.content,
+                        }
+                    )
             else:
                 transformed_messages.append(msg)
 
-
         response = self.client.chat.completions.create(
             model=model, messages=transformed_messages, *args, **kwargs
         )
 
         if kwargs.get("stream") and kwargs["stream"] is True:
-            return self.format_chunks(response,model)
+            return self.format_chunks(response, model)
 
         if response.choices:
 
             choice = response.choices[0].message
             extracted_info = default_tool_extractor(choice.content)
             if isinstance(extracted_info, tuple):
                 tool_name, tool_args = extracted_info
                 tool_call = ChatCompletionMessageToolCall(
                     id=str(uuid.uuid4()),
                     function=Function(name=tool_name, arguments=tool_args),
                     type="function",
                 )
 
-                message= ChatCompletionMessage(
+                message = ChatCompletionMessage(
                     content=None, role="assistant", tool_calls=[tool_call]
                 )
                 return ChatCompletion(
                     id=str(uuid.uuid4()),
                     choices=[
                         Choice(
-                            finish_reason='tool_calls',
+                            finish_reason="tool_calls",
                             index=0,
                             logprobs=None,
-                            message=message
+                            message=message,
                         )
                     ],
                     created=int(time.time()),
                     model=model,
-                    object='chat.completion',
+                    object="chat.completion",
                     system_fingerprint=None,
                     usage=CompletionUsage(
                         completion_tokens=0,  # Assuming no tokens used for simplicity
                         prompt_tokens=0,  # Assuming no tokens used for simplicity
-                        total_tokens=0  # Assuming no tokens used for simplicity
-                    )
+                        total_tokens=0,  # Assuming no tokens used for simplicity
+                    ),
                 )
 
             else:
-                return response
+                return response
```

### Comparing `scalegen-function-calling-0.1.1/setup.py` & `scalegen-function-calling-0.1.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name="scalegen-function-calling",
-    version="0.1.1",
+    version="0.1.2",
     packages=find_packages(),
     install_requires=[
         "openai",
         # Add other dependencies here
     ],
     include_package_data=True,
     license="MIT",
-    description="A package for generating function calls using OpenAI's API for scalegen function calling model's .",
+    description="A package for generating function calls using OpenAI's API for ScaleGenAI's function calling models",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author="Tejesh Bhalla",
     author_email="tejeshbhalla1@gmail.com",
     url="https://github.com/ScaleGenAI/function-calling-openai-sdk",
     classifiers=[
         "Programming Language :: Python :: 3",
```

