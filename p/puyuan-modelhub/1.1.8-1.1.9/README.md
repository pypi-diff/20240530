# Comparing `tmp/puyuan_modelhub-1.1.8.tar.gz` & `tmp/puyuan_modelhub-1.1.9.tar.gz`

## Comparing `puyuan_modelhub-1.1.8.tar` & `puyuan_modelhub-1.1.9.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/modelhub/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/modelhub/_version.py
--rw-r--r--   0        0        0    13294 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/modelhub/client.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/modelhub/constants.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/modelhub/errors.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/modelhub/utils.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/modelhub/types/__init__.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/modelhub/types/audio.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/modelhub/types/base.py
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/modelhub/types/chat.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/modelhub/types/encoder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/modelhub/types/errors.py
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/modelhub/types/generation.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/modelhub/types/message.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/LICENSE.txt
--rw-r--r--   0        0        0    30849 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/README.md
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/pyproject.toml
--rw-r--r--   0        0        0    31593 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.9/modelhub/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.9/modelhub/_version.py
+-rw-r--r--   0        0        0    16403 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.9/modelhub/client.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.9/modelhub/constants.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.9/modelhub/errors.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.9/modelhub/utils.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.9/modelhub/types/__init__.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.9/modelhub/types/audio.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.9/modelhub/types/base.py
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.9/modelhub/types/chat.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.9/modelhub/types/encoder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.9/modelhub/types/errors.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.9/modelhub/types/generation.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.9/modelhub/types/message.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.9/modelhub/types/retrieve.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.9/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.9/LICENSE.txt
+-rw-r--r--   0        0        0    30849 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.9/README.md
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0    31593 2020-02-02 00:00:00.000000 puyuan_modelhub-1.1.9/PKG-INFO
```

### Comparing `puyuan_modelhub-1.1.8/modelhub/client.py` & `puyuan_modelhub-1.1.9/modelhub/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-from modelhub.utils import BaseModel
+from modelhub.utils import BaseModel, retrieve_top_k
 import json
 import os
+import numpy as np
+from functools import partial
 from io import TextIOWrapper
 from typing import Any, Dict, Generator, List, Literal, Optional, Union, AsyncGenerator
 
 import httpx
 import retrying
 from httpx import Response
 
@@ -18,15 +20,15 @@
     ModelInfo,
     ModelInfoOutput,
     NTokensOutput,
     TextGenerationOutput,
     TextGenerationStreamOutput,
     Transcription,
 )
-
+from modelhub.types.retrieve import RerankOutput, RetrieveOutput
 from .errors import (
     APIConnectionError,
     APIRateLimitError,
     AuthenticationError,
     InternalServerError,
 )
 
@@ -277,14 +279,112 @@
             ) as r:
                 async for line in r.aiter_lines():
                     if line.startswith("data:"):
                         out = TextGenerationStreamOutput(**json.loads(line[5:]))
                         self.raise_for_status(r, out.code, out.msg)
                         yield out
 
+    def retrieve(
+        self,
+        querys: list[str] | str,
+        passages: list[str],
+        model: str | None = None,
+        embedding_params: Dict[str, Any] = {},
+        top_k: int = 5,
+        threshold: float = 0.0,
+    ):
+        model = model or self.model
+        if isinstance(querys, str):
+            querys = [querys]
+        embedding = partial(
+            self.get_embeddings, model=model, parameters=embedding_params
+        )
+        query_embeddings = np.array(embedding(querys).embeddings)
+        passage_embeddings = np.array(embedding(passages).embeddings)
+        return RetrieveOutput(
+            **retrieve_top_k(
+                passages,
+                query_embeddings,
+                passage_embeddings,
+                top_k,
+                threshold,
+            )
+        )
+
+    async def aretrieve(
+        self,
+        querys: list[str] | str,
+        passages: list[str],
+        model: str | None = None,
+        embedding_params: Dict[str, Any] = {},
+        top_k: int = 5,
+        threshold: float = 0.0,
+    ):
+        model = model or self.model
+        if isinstance(querys, str):
+            querys = [querys]
+        embedding = partial(
+            self.aget_embeddings, model=model, parameters=embedding_params
+        )
+        query_embeddings = np.array((await embedding(querys)).embeddings)
+        passage_embeddings = np.array((await embedding(passages)).embeddings)
+        return RetrieveOutput(
+            **retrieve_top_k(
+                passages,
+                query_embeddings,
+                passage_embeddings,
+                top_k,
+                threshold,
+            )
+        )
+
+    def rerank(
+        self,
+        query: str,
+        docs: list[str],
+        model: str | None = None,
+        parameters: Dict[str, Any] = {},
+        top_k: int = 5,
+        threshold: float = 0.0,
+    ):
+        pairs = [[query, doc] for doc in docs]
+        scores = np.array(
+            self.cross_embedding(pairs, model=model, parameters=parameters).scores
+        )
+        idxs = np.argsort(scores)[::-1][:top_k]
+        idxs = idxs[scores[idxs] > threshold]
+        return RerankOutput(
+            passages=[docs[i] for i in idxs],
+            idxs=idxs.tolist(),
+            scores=scores[idxs].tolist(),
+        )
+
+    async def arerank(
+        self,
+        query: str,
+        docs: list[str],
+        model: str | None = None,
+        parameters: Dict[str, Any] = {},
+        top_k: int = 5,
+        threshold: float = 0.0,
+    ):
+        pairs = [[query, doc] for doc in docs]
+        scores = np.array(
+            (
+                await self.across_embedding(pairs, model=model, parameters=parameters)
+            ).scores
+        )
+        idxs = np.argsort(scores)[::-1][:top_k]
+        idxs = idxs[scores[idxs] > threshold]
+        return RerankOutput(
+            passages=[docs[i] for i in idxs],
+            idxs=idxs.tolist(),
+            scores=scores[idxs].tolist(),
+        )
+
     def get_embeddings(
         self, prompt: str, model: str = "", parameters: Dict[str, Any] = {}
     ) -> EmbeddingOutput:
         model = model or self.model
         response = self._post(
             self.host + "/embedding",
             json={
```

### Comparing `puyuan_modelhub-1.1.8/modelhub/errors.py` & `puyuan_modelhub-1.1.9/modelhub/errors.py`

 * *Files identical despite different names*

### Comparing `puyuan_modelhub-1.1.8/modelhub/types/__init__.py` & `puyuan_modelhub-1.1.9/modelhub/types/__init__.py`

 * *Files identical despite different names*

### Comparing `puyuan_modelhub-1.1.8/modelhub/types/chat.py` & `puyuan_modelhub-1.1.9/modelhub/types/chat.py`

 * *Files identical despite different names*

### Comparing `puyuan_modelhub-1.1.8/modelhub/types/encoder.py` & `puyuan_modelhub-1.1.9/modelhub/types/encoder.py`

 * *Files identical despite different names*

### Comparing `puyuan_modelhub-1.1.8/modelhub/types/generation.py` & `puyuan_modelhub-1.1.9/modelhub/types/generation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from typing import Any, Dict, List, Literal, Optional
 
-from fastapi.responses import JSONResponse
-
-from .base import BaseModel
+from .base import BaseModel, BaseOutput
 from .message import BaseMessage
 
 
 class GenerationParams(BaseModel):
     inputs: str
     parameters: Dict[str, Any] = {}
 
@@ -23,26 +21,14 @@
     request_time: Optional[float] = None
     prompt_tokens: Optional[int] = None
     generated_tokens: Optional[int] = None
     seed: Optional[int] = None
     tokens: Optional[List[TextGenerationStreamToken]] = None
 
 
-class BaseOutput(BaseModel):
-    success: bool = True
-    code: int = 200
-    msg: str = "success"
-
-    def to_response(self):
-        return JSONResponse(self.dict(), status_code=self.code)
-
-    class Config:
-        extra = "allow"
-
-
 class TextGenerationStreamOutput(BaseOutput):
     token: TextGenerationStreamToken
     generated_text: Optional[str] = None
     history: List[Dict[str, Any]] = []
     details: Optional[TextGenerationDetails] = None
```

### Comparing `puyuan_modelhub-1.1.8/modelhub/types/message.py` & `puyuan_modelhub-1.1.9/modelhub/types/message.py`

 * *Files identical despite different names*

### Comparing `puyuan_modelhub-1.1.8/LICENSE.txt` & `puyuan_modelhub-1.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `puyuan_modelhub-1.1.8/README.md` & `puyuan_modelhub-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `puyuan_modelhub-1.1.8/pyproject.toml` & `puyuan_modelhub-1.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `puyuan_modelhub-1.1.8/PKG-INFO` & `puyuan_modelhub-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: puyuan-modelhub
-Version: 1.1.8
+Version: 1.1.9
 Summary: A library for managing LLM models
 Project-URL: Homepage, https://github.com/puyuantech/modelhub
 Author-email: HSPK <whxway@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

