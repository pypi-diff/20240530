# Comparing `tmp/langchain_nvidia_ai_endpoints-0.0.8.tar.gz` & `tmp/langchain_nvidia_ai_endpoints-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_nvidia_ai_endpoints-0.0.8.tar", max compression
+gzip compressed data, was "langchain_nvidia_ai_endpoints-0.0.9.tar", max compression
```

## Comparing `langchain_nvidia_ai_endpoints-0.0.8.tar` & `langchain_nvidia_ai_endpoints-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1072 2024-04-18 19:13:25.981102 langchain_nvidia_ai_endpoints-0.0.8/LICENSE
--rw-r--r--   0        0        0    10720 2024-04-18 19:13:25.981102 langchain_nvidia_ai_endpoints-0.0.8/README.md
--rw-r--r--   0        0        0     2070 2024-04-18 19:13:25.985102 langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/__init__.py
--rw-r--r--   0        0        0    29740 2024-04-18 19:13:25.985102 langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/_common.py
--rw-r--r--   0        0        0     7056 2024-04-18 19:13:25.985102 langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/_statics.py
--rw-r--r--   0        0        0    10149 2024-04-18 19:13:25.985102 langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/callbacks.py
--rw-r--r--   0        0        0    16465 2024-04-18 19:13:25.985102 langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/chat_models.py
--rw-r--r--   0        0        0     5442 2024-04-18 19:13:25.985102 langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/embeddings.py
--rw-r--r--   0        0        0     5735 2024-04-18 19:13:25.985102 langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/image_gen.py
--rw-r--r--   0        0        0     7597 2024-04-18 19:13:25.985102 langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/llm.py
--rw-r--r--   0        0        0        0 2024-04-18 19:13:25.985102 langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/py.typed
--rw-r--r--   0        0        0    10047 2024-04-18 19:13:25.985102 langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/tools.py
--rw-r--r--   0        0        0     2894 2024-04-18 19:13:25.989102 langchain_nvidia_ai_endpoints-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    11619 1970-01-01 00:00:00.000000 langchain_nvidia_ai_endpoints-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-23 20:25:41.432902 langchain_nvidia_ai_endpoints-0.0.9/LICENSE
+-rw-r--r--   0        0        0     9661 2024-04-23 20:25:41.432902 langchain_nvidia_ai_endpoints-0.0.9/README.md
+-rw-r--r--   0        0        0     2140 2024-04-23 20:25:41.440902 langchain_nvidia_ai_endpoints-0.0.9/langchain_nvidia_ai_endpoints/__init__.py
+-rw-r--r--   0        0        0    29908 2024-04-23 20:25:41.440902 langchain_nvidia_ai_endpoints-0.0.9/langchain_nvidia_ai_endpoints/_common.py
+-rw-r--r--   0        0        0     7292 2024-04-23 20:25:41.440902 langchain_nvidia_ai_endpoints-0.0.9/langchain_nvidia_ai_endpoints/_statics.py
+-rw-r--r--   0        0        0    10149 2024-04-23 20:25:41.440902 langchain_nvidia_ai_endpoints-0.0.9/langchain_nvidia_ai_endpoints/callbacks.py
+-rw-r--r--   0        0        0    16465 2024-04-23 20:25:41.440902 langchain_nvidia_ai_endpoints-0.0.9/langchain_nvidia_ai_endpoints/chat_models.py
+-rw-r--r--   0        0        0     6644 2024-04-23 20:25:41.440902 langchain_nvidia_ai_endpoints-0.0.9/langchain_nvidia_ai_endpoints/embeddings.py
+-rw-r--r--   0        0        0     5735 2024-04-23 20:25:41.440902 langchain_nvidia_ai_endpoints-0.0.9/langchain_nvidia_ai_endpoints/image_gen.py
+-rw-r--r--   0        0        0     7597 2024-04-23 20:25:41.440902 langchain_nvidia_ai_endpoints-0.0.9/langchain_nvidia_ai_endpoints/llm.py
+-rw-r--r--   0        0        0        0 2024-04-23 20:25:41.440902 langchain_nvidia_ai_endpoints-0.0.9/langchain_nvidia_ai_endpoints/py.typed
+-rw-r--r--   0        0        0     6525 2024-04-23 20:25:41.440902 langchain_nvidia_ai_endpoints-0.0.9/langchain_nvidia_ai_endpoints/reranking.py
+-rw-r--r--   0        0        0    10047 2024-04-23 20:25:41.440902 langchain_nvidia_ai_endpoints-0.0.9/langchain_nvidia_ai_endpoints/tools.py
+-rw-r--r--   0        0        0     2913 2024-04-23 20:25:41.440902 langchain_nvidia_ai_endpoints-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    10561 1970-01-01 00:00:00.000000 langchain_nvidia_ai_endpoints-0.0.9/PKG-INFO
```

### Comparing `langchain_nvidia_ai_endpoints-0.0.8/LICENSE` & `langchain_nvidia_ai_endpoints-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.8/README.md` & `langchain_nvidia_ai_endpoints-0.0.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -4,153 +4,139 @@
 
 > [NVIDIA AI Foundation Endpoints](https://www.nvidia.com/en-us/ai-data-science/foundation-models/) give users easy access to hosted endpoints for generative AI models like Llama-2, SteerLM, Mistral, etc. Using the API, you can query live endpoints available on the [NVIDIA GPU Cloud (NGC)](https://catalog.ngc.nvidia.com/ai-foundation-models) to get quick results from a DGX-hosted cloud compute environment. All models are source-accessible and can be deployed on your own compute cluster.
 
 Below is an example on how to use some common functionality surrounding text-generative and embedding models
 
 ## Installation
 
-
 ```python
 %pip install -U --quiet langchain-nvidia-ai-endpoints
 ```
 
 ## Setup
 
 **To get started:**
 1. Create a free account with the [NVIDIA GPU Cloud](https://catalog.ngc.nvidia.com/) service, which hosts AI solution catalogs, containers, models, etc.
 2. Navigate to `Catalog > AI Foundation Models > (Model with API endpoint)`.
 3. Select the `API` option and click `Generate Key`.
 4. Save the generated key as `NVIDIA_API_KEY`. From there, you should have access to the endpoints.
 
-
 ```python
 import getpass
 import os
 
 if not os.environ.get("NVIDIA_API_KEY", "").startswith("nvapi-"):
     nvidia_api_key = getpass.getpass("Enter your NVIDIA AIPLAY API key: ")
     assert nvidia_api_key.startswith("nvapi-"), f"{nvidia_api_key[:5]}... is not a valid key"
     os.environ["NVIDIA_API_KEY"] = nvidia_api_key
 ```
 
-
 ```python
 ## Core LC Chat Interface
 from langchain_nvidia_ai_endpoints import ChatNVIDIA
 
-llm = ChatNVIDIA(model="mixtral_8x7b")
+llm = ChatNVIDIA(model="ai-llama3-70b", max_tokens=419)
 result = llm.invoke("Write a ballad about LangChain.")
 print(result.content)
 ```
 
-
 ## Stream, Batch, and Async
 
 These models natively support streaming, and as is the case with all LangChain LLMs they expose a batch method to handle concurrent requests, as well as async methods for invoke, stream, and batch. Below are a few examples.
 
-
 ```python
 print(llm.batch(["What's 2*3?", "What's 2*6?"]))
 # Or via the async API
 # await llm.abatch(["What's 2*3?", "What's 2*6?"])
 ```
 
-
 ```python
 for chunk in llm.stream("How far can a seagull fly in one day?"):
     # Show the token separations
     print(chunk.content, end="|")
 ```
 
-
 ```python
 async for chunk in llm.astream("How long does it take for monarch butterflies to migrate?"):
     print(chunk.content, end="|")
 ```
 
 ## Supported models
 
 Querying `available_models` will still give you all of the other models offered by your API credentials.
 
-The `playground_` prefix is optional.
-
-
 ```python
-list(llm.available_models)
-
+[model.id for model in llm.available_models if model.model_type]
 
-# ['playground_llama2_13b',
-# 'playground_llama2_code_13b',
-# 'playground_clip',
-# 'playground_fuyu_8b',
-# 'playground_mistral_7b',
-# 'playground_nvolveqa_40k',
-# 'playground_yi_34b',
-# 'playground_nemotron_steerlm_8b',
-# 'playground_nv_llama2_rlhf_70b',
-# 'playground_llama2_code_34b',
-# 'playground_mixtral_8x7b',
-# 'playground_neva_22b',
-# 'playground_steerlm_llama_70b',
-# 'playground_nemotron_qa_8b',
-# 'playground_sdxl']
+#['ai-codegemma-7b',
+# 'ai-codellama-70b',
+# 'ai-fuyu-8b',
+# 'ai-gemma-2b',
+# 'ai-gemma-7b',
+# 'ai-google-deplot',
+# 'ai-llama2-70b',
+# 'ai-llama3-70b',
+# 'ai-llama3-8b',
+# 'ai-microsoft-kosmos-2',
+# 'ai-mistral-7b-instruct-v2',
+# 'ai-mistral-large',
+# 'ai-mixtral-8x22b-instruct',
+# 'ai-mixtral-8x7b-instruct',
+# 'ai-neva-22b',
+# 'ai-recurrentgemma-2b',
+# ]
 ```
 
-
 ## Model types
 
-All of these models above are supported and can be accessed via `ChatNVIDIA`. 
+All of these models above are supported and can be accessed via `ChatNVIDIA`.
 
 Some model types support unique prompting techniques and chat messages. We will review a few important ones below.
 
-
-**To find out more about a specific model, please navigate to the API section of an AI Foundation Model [as linked here](https://catalog.ngc.nvidia.com/orgs/nvidia/teams/ai-foundation/models/codellama-13b/api).**
+**To find out more about a specific model, please navigate to the NVIDIA NIM section of ai.nvidia.com [as linked here](https://docs.api.nvidia.com/nim/).**
 
 ### General Chat
 
-Models such as `llama2_13b` and `mixtral_8x7b` are good all-around models that you can use for with any LangChain chat messages. Example below.
-
+Models such as `ai-llama3-70b` and `ai-mixtral-8x22b-instruct` are good all-around models that you can use for with any LangChain chat messages. Example below.
 
 ```python
 from langchain_nvidia_ai_endpoints import ChatNVIDIA
 from langchain_core.prompts import ChatPromptTemplate
 from langchain_core.output_parsers import StrOutputParser
 
 prompt = ChatPromptTemplate.from_messages(
     [
         ("system", "You are a helpful AI assistant named Fred."),
         ("user", "{input}")
     ]
 )
 chain = (
     prompt
-    | ChatNVIDIA(model="llama2_13b")
+    | ChatNVIDIA(model="ai-llama3-70b")
     | StrOutputParser()
 )
 
 for txt in chain.stream({"input": "What's your name?"}):
     print(txt, end="")
 ```
 
-
 ### Code Generation
 
-These models accept the same arguments and input structure as regular chat models, but they tend to perform better on code-genreation and structured code tasks. An example of this is `llama2_code_13b`.
-
+These models accept the same arguments and input structure as regular chat models, but they tend to perform better on code-genreation and structured code tasks. An example of this is `ai-codellama-70b` and `ai-codegemma-7b`.
 
 ```python
 prompt = ChatPromptTemplate.from_messages(
     [
         ("system", "You are an expert coding AI. Respond only in valid python; no narration whatsoever."),
         ("user", "{input}")
     ]
 )
 chain = (
     prompt
-    | ChatNVIDIA(model="llama2_code_13b")
+    | ChatNVIDIA(model="ai-codellama-70b", max_tokens=419)
     | StrOutputParser()
 )
 
 for txt in chain.stream({"input": "How do I solve this fizz buzz problem?"}):
     print(txt, end="")
 ```
 
@@ -158,15 +144,14 @@
 
 > [SteerLM-optimized models](https://developer.nvidia.com/blog/announcing-steerlm-a-simple-and-practical-technique-to-customize-llms-during-inference/) supports "dynamic steering" of model outputs at inference time.
 
 This lets you "control" the complexity, verbosity, and creativity of the model via integer labels on a scale from 0 to 9. Under the hood, these are passed as a special type of assistant message to the model.
 
 The "steer" models support this type of input, such as `steerlm_llama_70b`
 
-
 ```python
 from langchain_nvidia_ai_endpoints import ChatNVIDIA
 
 llm = ChatNVIDIA(model="steerlm_llama_70b")
 # Try making it uncreative and not verbose
 complex_result = llm.invoke(
     "What's a PB&J?",
@@ -180,20 +165,18 @@
 creative_result = llm.invoke(
     "What's a PB&J?",
     labels={"creativity": 9, "complexity": 3, "verbosity": 9}
 )
 print(creative_result.content)
 ```
 
-
 #### Use within LCEL
 
 The labels are passed as invocation params. You can `bind` these to the LLM using the `bind` method on the LLM to include it within a declarative, functional chain. Below is an example.
 
-
 ```python
 from langchain_nvidia_ai_endpoints import ChatNVIDIA
 from langchain_core.prompts import ChatPromptTemplate
 from langchain_core.output_parsers import StrOutputParser
 
 prompt = ChatPromptTemplate.from_messages(
     [
@@ -211,78 +194,49 @@
     print(txt, end="")
 ```
 
 ## Multimodal
 
 NVIDIA also supports multimodal inputs, meaning you can provide both images and text for the model to reason over.
 
-These models also accept `labels`, similar to the Steering LLMs above. In addition to `creativity`, `complexity`, and `verbosity`, these models support a `quality` toggle.
-
-An example model supporting multimodal inputs is `playground_neva_22b`.
+An example model supporting multimodal inputs is `ai-neva-22b`.
 
 These models accept LangChain's standard image formats. Below are examples.
 
-
 ```python
 import requests
 
 image_url = "https://picsum.photos/seed/kitten/300/200"
 image_content = requests.get(image_url).content
 ```
 
 Initialize the model like so:
 
 ```python
 from langchain_nvidia_ai_endpoints import ChatNVIDIA
 
-llm = ChatNVIDIA(model="playground_neva_22b")
+llm = ChatNVIDIA(model="ai-neva-22b")
 ```
 
 #### Passing an image as a URL
 
-
 ```python
 from langchain_core.messages import HumanMessage
 
 llm.invoke(
     [
         HumanMessage(content=[
             {"type": "text", "text": "Describe this image:"},
             {"type": "image_url", "image_url": {"url": image_url}},
         ])
     ])
 ```
 
-
-```python
-### You can specify the labels for steering here as well.  You can try setting a low verbosity, for instance
-
-from langchain_core.messages import HumanMessage
-
-llm.invoke(
-    [
-        HumanMessage(content=[
-            {"type": "text", "text": "Describe this image:"},
-            {"type": "image_url", "image_url": {"url": image_url}},
-        ])
-    ],
-    labels={
-        "creativity": 0,
-        "quality": 9,
-        "complexity": 0,
-        "verbosity": 0
-    }
-)
-```
-
-
-
 #### Passing an image as a base64 encoded string
 
-
 ```python
 import base64
 b64_string = base64.b64encode(image_content).decode('utf-8')
 llm.invoke(
     [
         HumanMessage(content=[
             {"type": "text", "text": "Describe this image:"},
@@ -291,33 +245,29 @@
     ])
 ```
 
 #### Directly within the string
 
 The NVIDIA API uniquely accepts images as base64 images inlined within <img> HTML tags. While this isn't interoperable with other LLMs, you can directly prompt the model accordingly.
 
-
 ```python
 base64_with_mime_type = f"data:image/png;base64,{b64_string}"
 llm.invoke(
     f'What\'s in this image?\n<img src="{base64_with_mime_type}" />'
 )
 ```
 
-
-
 ## RAG: Context models
 
 NVIDIA also has Q&A models that support a special "context" chat message containing retrieved context (such as documents within a RAG chain). This is useful to avoid prompt-injecting the model.
 
 **Note:** Only "user" (human) and "context" chat messages are supported for these models, not system or AI messages useful in conversational flows.
 
 The `_qa_` models like `nemotron_qa_8b` support this.
 
-
 ```python
 from langchain_nvidia_ai_endpoints import ChatNVIDIA
 from langchain_core.prompts import ChatPromptTemplate
 from langchain_core.output_parsers import StrOutputParser
 from langchain_core.messages import ChatMessage
 prompt = ChatPromptTemplate.from_messages(
     [
@@ -334,25 +284,17 @@
 chain.invoke({"input": "What was signed?"})
 ```
 
 ## Embeddings
 
 You can also connect to embeddings models through this package. Below is an example:
 
-```
+```python
 from langchain_nvidia_ai_endpoints import NVIDIAEmbeddings
 
-embedder = NVIDIAEmbeddings(model="nvolveqa_40k")
+embedder = NVIDIAEmbeddings(model="ai-embed-qa-4")
 embedder.embed_query("What's the temperature today?")
 embedder.embed_documents([
     "The temperature is 42 degrees.",
     "Class is dismissed at 9 PM."
 ])
 ```
-
-By default the embedding model will use the "passage" type for documents and "query" type for queries, but you can fix this on the instance.
-
-```python
-query_embedder = NVIDIAEmbeddings(model="nvolveqa_40k", model_type="query")
-doc_embeddder = NVIDIAEmbeddings(model="nvolveqa_40k", model_type="passage")
-```
-
```

### Comparing `langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/__init__.py` & `langchain_nvidia_ai_endpoints-0.0.9/langchain_nvidia_ai_endpoints/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,12 +37,10 @@
 embed_model = NVIDIAEmbeddings(model="nvolveqa_40k")
 embedding_output = embed_model.embed_query("Exploring AI capabilities.")
 ```
 """  # noqa: E501
 
 from langchain_nvidia_ai_endpoints.chat_models import ChatNVIDIA
 from langchain_nvidia_ai_endpoints.embeddings import NVIDIAEmbeddings
+from langchain_nvidia_ai_endpoints.reranking import NVIDIARerank
 
-__all__ = [
-    "ChatNVIDIA",
-    "NVIDIAEmbeddings",
-]
+__all__ = ["ChatNVIDIA", "NVIDIAEmbeddings", "NVIDIARerank"]
```

### Comparing `langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/_common.py` & `langchain_nvidia_ai_endpoints-0.0.9/langchain_nvidia_ai_endpoints/_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,14 +35,18 @@
 from langchain_nvidia_ai_endpoints._statics import MODEL_SPECS, Model
 
 logger = logging.getLogger(__name__)
 
 _MODE_TYPE = Literal["catalog", "nvidia", "nim", "open", "openai"]
 
 
+def default_payload_fn(payload: dict) -> dict:
+    return payload
+
+
 class NVEModel(BaseModel):
 
     """
     Underlying Client for interacting with the AI Foundation Model Function API.
     Leveraged by the NVIDIABaseModel to provide a simple requests-oriented interface.
     Direct abstraction over NGC-recommended streaming/non-streaming Python solutions.
 
@@ -76,15 +80,17 @@
     ## Generation arguments
     timeout: float = Field(60, ge=0, description="Timeout for waiting on response (s)")
     interval: float = Field(0.02, ge=0, description="Interval for pulling response")
     last_inputs: dict = Field({}, description="Last inputs sent over to the server")
     last_response: Response = Field(
         None, description="Last response sent from the server"
     )
-    payload_fn: Callable = Field(lambda d: d, description="Function to process payload")
+    payload_fn: Callable = Field(
+        default_payload_fn, description="Function to process payload"
+    )
     headers_tmpl: dict = Field(
         ...,
         description="Headers template for API calls."
         " Should contain `call` and `stream` keys.",
     )
     _available_functions: Optional[List[dict]] = PrivateAttr(default=None)
     _available_models: Optional[dict] = PrivateAttr(default=None)
@@ -527,15 +533,15 @@
     Higher-Level AI Foundation Model Function API Client with argument defaults.
     Is subclassed by ChatNVIDIA to provide a simple LangChain interface.
     """
 
     client: NVEModel = Field(NVEModel)
 
     _default_model: str = ""
-    model: Optional[str] = Field(description="Name of the model to invoke")
+    model: str = Field(description="Name of the model to invoke")
     infer_endpoint: str = Field("{base_url}/chat/completions")
     curr_mode: _MODE_TYPE = Field("nvidia")
 
     ####################################################################################
 
     @root_validator(pre=True)
     def validate_client(cls, values: Any) -> Any:
@@ -609,28 +615,31 @@
 
     @classmethod
     def get_available_models(
         cls,
         mode: Optional[_MODE_TYPE] = None,
         client: Optional[_NVIDIAClient] = None,
         list_all: bool = False,
+        filter: Optional[str] = None,
         **kwargs: Any,
     ) -> List[Model]:
         """Map the available models that can be invoked. Callable from class"""
         nveclient = (client or cls(**kwargs)).mode(mode, **kwargs).client
         nveclient.reset_method_cache()
         out = sorted(
             [
                 Model(id=k.replace("playground_", ""), path=v, **MODEL_SPECS.get(k, {}))
                 for k, v in nveclient.available_models.items()
             ],
             key=lambda x: f"{x.client or 'Z'}{x.id}{cls}",
         )
+        if not filter:
+            filter = cls.__name__
         if not list_all:
-            out = [m for m in out if m.client == cls.__name__ or m.model_type is None]
+            out = [m for m in out if m.client == filter or m.model_type is None]
         return out
 
     def get_model_details(self, model: Optional[str] = None) -> dict:
         """Get more meta-details about a model retrieved by a given name"""
         if model is None:
             model = self.model
         model_key = self.client._get_invoke_url(model).split("/")[-1]
```

### Comparing `langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/_statics.py` & `langchain_nvidia_ai_endpoints-0.0.9/langchain_nvidia_ai_endpoints/_statics.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,18 @@
             "model_name": "mistralai/mistral-7b-instruct-v0.2",
         },
         "ai-mixtral-8x7b-instruct": {
             "model_type": "chat",
             "model_name": "mistralai/mixtral-8x7b-instruct-v0.1",
         },
         "ai-neva-22b": {"model_type": "image_in"},
-        # 'ai-reranking-4b': {'model_type': 'chat'},
+        "ai-rerank-qa-mistral-4b": {
+            "model_type": "ranking",
+            "model_name": "nv-rerank-qa-mistral-4b:1",  # nvidia/rerank-qa-mistral-4b
+        },
         # 'ai-sdxl-turbo': {'model_type': 'image_out'},
         # 'ai-stable-diffusion-xl-base': {'model_type': 'iamge_out'},
         "ai-codegemma-7b": {"model_type": "chat", "model_name": "google/codegemma-7b"},
         "ai-recurrentgemma-2b": {
             "model_type": "chat",
             "model_name": "google/recurrentgemma-2b",
         },
@@ -131,14 +134,15 @@
             "model_name": "mistralai/mixtral-8x22b-instruct-v0.1",
         },
         "ai-llama3-8b": {"model_type": "chat", "model_name": "meta/llama3-8b"},
         "ai-llama3-70b": {
             "model_type": "chat",
             "model_name": "meta/llama3-70b",
         },
+        "ai-phi-3-mini": {"model_type": "chat", "model_name": "microsoft/phi-3-mini"},
     }
 )
 
 
 MODEL_SPECS.update(
     {
         "babbage-002": {"model_type": "completion"},
@@ -180,12 +184,13 @@
     "embedding": "NVIDIAEmbeddings",
     "image_in": "ChatNVIDIA",
     "image_out": "ImageGenNVIDIA",
     "qa": "ChatNVIDIA",
     "similarity": "None",
     "translation": "None",
     "tts": "None",
+    "ranking": "NVIDIARerank",
 }
 
 MODEL_SPECS = {
     k: {**v, "client": client_map[v["model_type"]]} for k, v in MODEL_SPECS.items()
 }
```

### Comparing `langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/callbacks.py` & `langchain_nvidia_ai_endpoints-0.0.9/langchain_nvidia_ai_endpoints/callbacks.py`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/chat_models.py` & `langchain_nvidia_ai_endpoints-0.0.9/langchain_nvidia_ai_endpoints/chat_models.py`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/embeddings.py` & `langchain_nvidia_ai_endpoints-0.0.9/langchain_nvidia_ai_endpoints/embeddings.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,26 +10,54 @@
 from langchain_nvidia_ai_endpoints._common import _NVIDIAClient
 from langchain_nvidia_ai_endpoints.callbacks import usage_callback_var
 
 from ._statics import MODEL_SPECS
 
 
 class NVIDIAEmbeddings(_NVIDIAClient, Embeddings):
-    """NVIDIA's AI Foundation Retriever Question-Answering Asymmetric Model."""
+    """
+    Client to NVIDIA embeddings models.
+
+    Fields:
+    - model: str, the name of the model to use
+    - truncate: "NONE", "START", "END", truncate input text if it exceeds the model's
+        maximum token length. Default is "NONE", which raises an error if an input is
+        too long.
+    """
 
     _default_model: str = "ai-embed-qa-4"
     _default_max_batch_size: int = 50
     infer_endpoint: str = Field("{base_url}/embeddings")
     model: str = Field(_default_model, description="Name of the model to invoke")
+    truncate: Literal["NONE", "START", "END"] = Field(
+        default="NONE",
+        description=(
+            "Truncate input text if it exceeds the model's maximum token length. "
+            "Default is 'NONE', which raises an error if an input is too long."
+        ),
+    )
     max_length: int = Field(2048, ge=1, le=2048)
     max_batch_size: int = Field(default=_default_max_batch_size)
     model_type: Optional[Literal["passage", "query"]] = Field(
         None, description="The type of text to be embedded."
     )
 
+    # indicate to user that max_length is deprecated when passed as an argument to
+    # NVIDIAEmbeddings' constructor, e.g. NVIDIAEmbeddings(max_length=...). this
+    # does not warning on assignment, e.g. embedder.max_length = ...
+    # todo: fix _NVIDIAClient.validate_client and enable Config.validate_assignment
+    @validator("max_length")
+    def deprecated_max_length(cls, value: int) -> int:
+        """Deprecate the max_length field."""
+        warnings.warn(
+            "The max_length field is deprecated. Use the 'truncate' instead.",
+            DeprecationWarning,
+        )
+        return value
+
     # todo: fix _NVIDIAClient.validate_client and enable Config.validate_assignment
     @validator("model")
     def deprecated_nvolveqa_40k(cls, value: str) -> str:
         """Deprecate the nvolveqa_40k model."""
         if value == "nvolveqa_40k" or value == "playground_nvolveqa_40k":
             warnings.warn(
                 "nvolveqa_40k is deprecated. Use ai-embed-qa-4 instead.",
@@ -67,14 +95,16 @@
         else:  # default to the API Catalog API
             payload = {
                 "input": texts,
                 "model": self.get_binding_model() or self.model,
                 "encoding_format": "float",
                 "input_type": model_type,
             }
+            if self.truncate:
+                payload["truncate"] = self.truncate
 
         response = self.client.get_req(
             model_name=self.model,
             payload=payload,
             endpoint="infer",
         )
         response.raise_for_status()
```

### Comparing `langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/image_gen.py` & `langchain_nvidia_ai_endpoints-0.0.9/langchain_nvidia_ai_endpoints/image_gen.py`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/llm.py` & `langchain_nvidia_ai_endpoints-0.0.9/langchain_nvidia_ai_endpoints/llm.py`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/tools.py` & `langchain_nvidia_ai_endpoints-0.0.9/langchain_nvidia_ai_endpoints/tools.py`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.8/pyproject.toml` & `langchain_nvidia_ai_endpoints-0.0.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "langchain-nvidia-ai-endpoints"
-version = "0.0.8"
+version = "0.0.9"
 description = "An integration package connecting NVIDIA AI Endpoints and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/nvidia-ai-endpoints"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = "^0.1.5"
+langchain-core = "^0.1.27"
 aiohttp = "^3.9.1"
 pillow = ">=10.0.0,<11.0.0"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
@@ -24,14 +24,15 @@
 freezegun = "^1.2.2"
 pytest-mock = "^3.10.0"
 syrupy = "^4.0.2"
 pytest-watcher = "^0.3.4"
 pytest-asyncio = "^0.21.1"
 langchain-core = {git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core"}
 requests-mock = "^1.11.0"
+faker = "^24.4.0"
 
 [tool.poetry.group.codespell]
 optional = true
 
 [tool.poetry.group.codespell.dependencies]
 codespell = "^2.2.0"
```

### Comparing `langchain_nvidia_ai_endpoints-0.0.8/PKG-INFO` & `langchain_nvidia_ai_endpoints-0.0.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: langchain-nvidia-ai-endpoints
-Version: 0.0.8
+Version: 0.0.9
 Summary: An integration package connecting NVIDIA AI Endpoints and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.1,<4.0.0)
-Requires-Dist: langchain-core (>=0.1.5,<0.2.0)
+Requires-Dist: langchain-core (>=0.1.27,<0.2.0)
 Requires-Dist: pillow (>=10.0.0,<11.0.0)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/nvidia-ai-endpoints
 Description-Content-Type: text/markdown
 
 # langchain-nvidia-ai-endpoints
 
@@ -24,153 +24,139 @@
 
 > [NVIDIA AI Foundation Endpoints](https://www.nvidia.com/en-us/ai-data-science/foundation-models/) give users easy access to hosted endpoints for generative AI models like Llama-2, SteerLM, Mistral, etc. Using the API, you can query live endpoints available on the [NVIDIA GPU Cloud (NGC)](https://catalog.ngc.nvidia.com/ai-foundation-models) to get quick results from a DGX-hosted cloud compute environment. All models are source-accessible and can be deployed on your own compute cluster.
 
 Below is an example on how to use some common functionality surrounding text-generative and embedding models
 
 ## Installation
 
-
 ```python
 %pip install -U --quiet langchain-nvidia-ai-endpoints
 ```
 
 ## Setup
 
 **To get started:**
 1. Create a free account with the [NVIDIA GPU Cloud](https://catalog.ngc.nvidia.com/) service, which hosts AI solution catalogs, containers, models, etc.
 2. Navigate to `Catalog > AI Foundation Models > (Model with API endpoint)`.
 3. Select the `API` option and click `Generate Key`.
 4. Save the generated key as `NVIDIA_API_KEY`. From there, you should have access to the endpoints.
 
-
 ```python
 import getpass
 import os
 
 if not os.environ.get("NVIDIA_API_KEY", "").startswith("nvapi-"):
     nvidia_api_key = getpass.getpass("Enter your NVIDIA AIPLAY API key: ")
     assert nvidia_api_key.startswith("nvapi-"), f"{nvidia_api_key[:5]}... is not a valid key"
     os.environ["NVIDIA_API_KEY"] = nvidia_api_key
 ```
 
-
 ```python
 ## Core LC Chat Interface
 from langchain_nvidia_ai_endpoints import ChatNVIDIA
 
-llm = ChatNVIDIA(model="mixtral_8x7b")
+llm = ChatNVIDIA(model="ai-llama3-70b", max_tokens=419)
 result = llm.invoke("Write a ballad about LangChain.")
 print(result.content)
 ```
 
-
 ## Stream, Batch, and Async
 
 These models natively support streaming, and as is the case with all LangChain LLMs they expose a batch method to handle concurrent requests, as well as async methods for invoke, stream, and batch. Below are a few examples.
 
-
 ```python
 print(llm.batch(["What's 2*3?", "What's 2*6?"]))
 # Or via the async API
 # await llm.abatch(["What's 2*3?", "What's 2*6?"])
 ```
 
-
 ```python
 for chunk in llm.stream("How far can a seagull fly in one day?"):
     # Show the token separations
     print(chunk.content, end="|")
 ```
 
-
 ```python
 async for chunk in llm.astream("How long does it take for monarch butterflies to migrate?"):
     print(chunk.content, end="|")
 ```
 
 ## Supported models
 
 Querying `available_models` will still give you all of the other models offered by your API credentials.
 
-The `playground_` prefix is optional.
-
-
 ```python
-list(llm.available_models)
-
+[model.id for model in llm.available_models if model.model_type]
 
-# ['playground_llama2_13b',
-# 'playground_llama2_code_13b',
-# 'playground_clip',
-# 'playground_fuyu_8b',
-# 'playground_mistral_7b',
-# 'playground_nvolveqa_40k',
-# 'playground_yi_34b',
-# 'playground_nemotron_steerlm_8b',
-# 'playground_nv_llama2_rlhf_70b',
-# 'playground_llama2_code_34b',
-# 'playground_mixtral_8x7b',
-# 'playground_neva_22b',
-# 'playground_steerlm_llama_70b',
-# 'playground_nemotron_qa_8b',
-# 'playground_sdxl']
+#['ai-codegemma-7b',
+# 'ai-codellama-70b',
+# 'ai-fuyu-8b',
+# 'ai-gemma-2b',
+# 'ai-gemma-7b',
+# 'ai-google-deplot',
+# 'ai-llama2-70b',
+# 'ai-llama3-70b',
+# 'ai-llama3-8b',
+# 'ai-microsoft-kosmos-2',
+# 'ai-mistral-7b-instruct-v2',
+# 'ai-mistral-large',
+# 'ai-mixtral-8x22b-instruct',
+# 'ai-mixtral-8x7b-instruct',
+# 'ai-neva-22b',
+# 'ai-recurrentgemma-2b',
+# ]
 ```
 
-
 ## Model types
 
-All of these models above are supported and can be accessed via `ChatNVIDIA`. 
+All of these models above are supported and can be accessed via `ChatNVIDIA`.
 
 Some model types support unique prompting techniques and chat messages. We will review a few important ones below.
 
-
-**To find out more about a specific model, please navigate to the API section of an AI Foundation Model [as linked here](https://catalog.ngc.nvidia.com/orgs/nvidia/teams/ai-foundation/models/codellama-13b/api).**
+**To find out more about a specific model, please navigate to the NVIDIA NIM section of ai.nvidia.com [as linked here](https://docs.api.nvidia.com/nim/).**
 
 ### General Chat
 
-Models such as `llama2_13b` and `mixtral_8x7b` are good all-around models that you can use for with any LangChain chat messages. Example below.
-
+Models such as `ai-llama3-70b` and `ai-mixtral-8x22b-instruct` are good all-around models that you can use for with any LangChain chat messages. Example below.
 
 ```python
 from langchain_nvidia_ai_endpoints import ChatNVIDIA
 from langchain_core.prompts import ChatPromptTemplate
 from langchain_core.output_parsers import StrOutputParser
 
 prompt = ChatPromptTemplate.from_messages(
     [
         ("system", "You are a helpful AI assistant named Fred."),
         ("user", "{input}")
     ]
 )
 chain = (
     prompt
-    | ChatNVIDIA(model="llama2_13b")
+    | ChatNVIDIA(model="ai-llama3-70b")
     | StrOutputParser()
 )
 
 for txt in chain.stream({"input": "What's your name?"}):
     print(txt, end="")
 ```
 
-
 ### Code Generation
 
-These models accept the same arguments and input structure as regular chat models, but they tend to perform better on code-genreation and structured code tasks. An example of this is `llama2_code_13b`.
-
+These models accept the same arguments and input structure as regular chat models, but they tend to perform better on code-genreation and structured code tasks. An example of this is `ai-codellama-70b` and `ai-codegemma-7b`.
 
 ```python
 prompt = ChatPromptTemplate.from_messages(
     [
         ("system", "You are an expert coding AI. Respond only in valid python; no narration whatsoever."),
         ("user", "{input}")
     ]
 )
 chain = (
     prompt
-    | ChatNVIDIA(model="llama2_code_13b")
+    | ChatNVIDIA(model="ai-codellama-70b", max_tokens=419)
     | StrOutputParser()
 )
 
 for txt in chain.stream({"input": "How do I solve this fizz buzz problem?"}):
     print(txt, end="")
 ```
 
@@ -178,15 +164,14 @@
 
 > [SteerLM-optimized models](https://developer.nvidia.com/blog/announcing-steerlm-a-simple-and-practical-technique-to-customize-llms-during-inference/) supports "dynamic steering" of model outputs at inference time.
 
 This lets you "control" the complexity, verbosity, and creativity of the model via integer labels on a scale from 0 to 9. Under the hood, these are passed as a special type of assistant message to the model.
 
 The "steer" models support this type of input, such as `steerlm_llama_70b`
 
-
 ```python
 from langchain_nvidia_ai_endpoints import ChatNVIDIA
 
 llm = ChatNVIDIA(model="steerlm_llama_70b")
 # Try making it uncreative and not verbose
 complex_result = llm.invoke(
     "What's a PB&J?",
@@ -200,20 +185,18 @@
 creative_result = llm.invoke(
     "What's a PB&J?",
     labels={"creativity": 9, "complexity": 3, "verbosity": 9}
 )
 print(creative_result.content)
 ```
 
-
 #### Use within LCEL
 
 The labels are passed as invocation params. You can `bind` these to the LLM using the `bind` method on the LLM to include it within a declarative, functional chain. Below is an example.
 
-
 ```python
 from langchain_nvidia_ai_endpoints import ChatNVIDIA
 from langchain_core.prompts import ChatPromptTemplate
 from langchain_core.output_parsers import StrOutputParser
 
 prompt = ChatPromptTemplate.from_messages(
     [
@@ -231,78 +214,49 @@
     print(txt, end="")
 ```
 
 ## Multimodal
 
 NVIDIA also supports multimodal inputs, meaning you can provide both images and text for the model to reason over.
 
-These models also accept `labels`, similar to the Steering LLMs above. In addition to `creativity`, `complexity`, and `verbosity`, these models support a `quality` toggle.
-
-An example model supporting multimodal inputs is `playground_neva_22b`.
+An example model supporting multimodal inputs is `ai-neva-22b`.
 
 These models accept LangChain's standard image formats. Below are examples.
 
-
 ```python
 import requests
 
 image_url = "https://picsum.photos/seed/kitten/300/200"
 image_content = requests.get(image_url).content
 ```
 
 Initialize the model like so:
 
 ```python
 from langchain_nvidia_ai_endpoints import ChatNVIDIA
 
-llm = ChatNVIDIA(model="playground_neva_22b")
+llm = ChatNVIDIA(model="ai-neva-22b")
 ```
 
 #### Passing an image as a URL
 
-
 ```python
 from langchain_core.messages import HumanMessage
 
 llm.invoke(
     [
         HumanMessage(content=[
             {"type": "text", "text": "Describe this image:"},
             {"type": "image_url", "image_url": {"url": image_url}},
         ])
     ])
 ```
 
-
-```python
-### You can specify the labels for steering here as well.  You can try setting a low verbosity, for instance
-
-from langchain_core.messages import HumanMessage
-
-llm.invoke(
-    [
-        HumanMessage(content=[
-            {"type": "text", "text": "Describe this image:"},
-            {"type": "image_url", "image_url": {"url": image_url}},
-        ])
-    ],
-    labels={
-        "creativity": 0,
-        "quality": 9,
-        "complexity": 0,
-        "verbosity": 0
-    }
-)
-```
-
-
-
 #### Passing an image as a base64 encoded string
 
-
 ```python
 import base64
 b64_string = base64.b64encode(image_content).decode('utf-8')
 llm.invoke(
     [
         HumanMessage(content=[
             {"type": "text", "text": "Describe this image:"},
@@ -311,33 +265,29 @@
     ])
 ```
 
 #### Directly within the string
 
 The NVIDIA API uniquely accepts images as base64 images inlined within <img> HTML tags. While this isn't interoperable with other LLMs, you can directly prompt the model accordingly.
 
-
 ```python
 base64_with_mime_type = f"data:image/png;base64,{b64_string}"
 llm.invoke(
     f'What\'s in this image?\n<img src="{base64_with_mime_type}" />'
 )
 ```
 
-
-
 ## RAG: Context models
 
 NVIDIA also has Q&A models that support a special "context" chat message containing retrieved context (such as documents within a RAG chain). This is useful to avoid prompt-injecting the model.
 
 **Note:** Only "user" (human) and "context" chat messages are supported for these models, not system or AI messages useful in conversational flows.
 
 The `_qa_` models like `nemotron_qa_8b` support this.
 
-
 ```python
 from langchain_nvidia_ai_endpoints import ChatNVIDIA
 from langchain_core.prompts import ChatPromptTemplate
 from langchain_core.output_parsers import StrOutputParser
 from langchain_core.messages import ChatMessage
 prompt = ChatPromptTemplate.from_messages(
     [
@@ -354,26 +304,18 @@
 chain.invoke({"input": "What was signed?"})
 ```
 
 ## Embeddings
 
 You can also connect to embeddings models through this package. Below is an example:
 
-```
+```python
 from langchain_nvidia_ai_endpoints import NVIDIAEmbeddings
 
-embedder = NVIDIAEmbeddings(model="nvolveqa_40k")
+embedder = NVIDIAEmbeddings(model="ai-embed-qa-4")
 embedder.embed_query("What's the temperature today?")
 embedder.embed_documents([
     "The temperature is 42 degrees.",
     "Class is dismissed at 9 PM."
 ])
 ```
 
-By default the embedding model will use the "passage" type for documents and "query" type for queries, but you can fix this on the instance.
-
-```python
-query_embedder = NVIDIAEmbeddings(model="nvolveqa_40k", model_type="query")
-doc_embeddder = NVIDIAEmbeddings(model="nvolveqa_40k", model_type="passage")
-```
-
-
```

