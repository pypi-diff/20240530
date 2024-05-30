# Comparing `tmp/cuminai-0.0.1.dev285.tar.gz` & `tmp/cuminai-0.0.1.dev295.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuminai-0.0.1.dev285.tar", max compression
+gzip compressed data, was "cuminai-0.0.1.dev295.tar", max compression
```

## Comparing `cuminai-0.0.1.dev285.tar` & `cuminai-0.0.1.dev295.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0       75 2024-05-12 07:46:46.527637 cuminai-0.0.1.dev285/cuminai/__init__.py
--rw-r--r--   0        0        0      670 2024-05-28 11:51:04.207306 cuminai-0.0.1.dev285/cuminai/chunker.py
--rw-r--r--   0        0        0      380 2024-05-28 06:29:15.756996 cuminai-0.0.1.dev285/cuminai/config.py
--rw-r--r--   0        0        0      900 2024-05-28 12:39:08.543774 cuminai-0.0.1.dev285/cuminai/constants.py
--rw-r--r--   0        0        0     2576 2024-05-27 20:06:10.643890 cuminai-0.0.1.dev285/cuminai/contextstores.py
--rw-r--r--   0        0        0     9861 2024-05-28 12:45:11.612930 cuminai-0.0.1.dev285/cuminai/creator.py
--rw-r--r--   0        0        0     1237 2024-05-28 11:44:20.752198 cuminai-0.0.1.dev285/cuminai/document_loader.py
--rw-r--r--   0        0        0     1572 2024-05-28 12:30:42.700909 cuminai-0.0.1.dev285/cuminai/tagger.py
--rw-r--r--   0        0        0      653 2024-05-28 10:32:15.075085 cuminai-0.0.1.dev285/cuminai/utils.py
--rw-r--r--   0        0        0     5982 2024-05-28 12:28:57.373661 cuminai-0.0.1.dev285/cuminai/validator.py
--rw-r--r--   0        0        0    11558 2024-05-11 18:16:30.219425 cuminai-0.0.1.dev285/LICENSE
--rw-r--r--   0        0        0      579 2024-05-28 10:43:33.325871 cuminai-0.0.1.dev285/pyproject.toml
--rw-r--r--   0        0        0     4324 2024-05-28 13:35:25.516807 cuminai-0.0.1.dev285/README.md
--rw-r--r--   0        0        0     4943 1970-01-01 00:00:00.000000 cuminai-0.0.1.dev285/PKG-INFO
+-rw-r--r--   0        0        0       75 2024-05-12 07:46:46.527637 cuminai-0.0.1.dev295/cuminai/__init__.py
+-rw-r--r--   0        0        0     1239 2024-05-29 13:37:29.554766 cuminai-0.0.1.dev295/cuminai/chunker.py
+-rw-r--r--   0        0        0      380 2024-05-28 06:29:15.756996 cuminai-0.0.1.dev295/cuminai/config.py
+-rw-r--r--   0        0        0      900 2024-05-28 12:39:08.543774 cuminai-0.0.1.dev295/cuminai/constants.py
+-rw-r--r--   0        0        0     2576 2024-05-27 20:06:10.643890 cuminai-0.0.1.dev295/cuminai/contextstores.py
+-rw-r--r--   0        0        0     9580 2024-05-29 16:04:19.581946 cuminai-0.0.1.dev295/cuminai/creator.py
+-rw-r--r--   0        0        0     1420 2024-05-29 16:04:09.797293 cuminai-0.0.1.dev295/cuminai/document_loader.py
+-rw-r--r--   0        0        0     1237 2024-05-29 16:03:24.886639 cuminai-0.0.1.dev295/cuminai/embedding.py
+-rw-r--r--   0        0        0     1682 2024-05-29 13:53:38.500528 cuminai-0.0.1.dev295/cuminai/tagger.py
+-rw-r--r--   0        0        0      645 2024-05-29 13:19:47.377866 cuminai-0.0.1.dev295/cuminai/utils.py
+-rw-r--r--   0        0        0     5982 2024-05-28 12:28:57.373661 cuminai-0.0.1.dev295/cuminai/validator.py
+-rw-r--r--   0        0        0    11558 2024-05-11 18:16:30.219425 cuminai-0.0.1.dev295/LICENSE
+-rw-r--r--   0        0        0      598 2024-05-29 16:01:03.160223 cuminai-0.0.1.dev295/pyproject.toml
+-rw-r--r--   0        0        0     4324 2024-05-28 13:35:25.516807 cuminai-0.0.1.dev295/README.md
+-rw-r--r--   0        0        0     4974 1970-01-01 00:00:00.000000 cuminai-0.0.1.dev295/PKG-INFO
```

### Comparing `cuminai-0.0.1.dev285/cuminai/constants.py` & `cuminai-0.0.1.dev295/cuminai/constants.py`

 * *Files identical despite different names*

### Comparing `cuminai-0.0.1.dev285/cuminai/contextstores.py` & `cuminai-0.0.1.dev295/cuminai/contextstores.py`

 * *Files identical despite different names*

### Comparing `cuminai-0.0.1.dev285/cuminai/creator.py` & `cuminai-0.0.1.dev295/cuminai/creator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 import click
-import time
 from pathlib import Path
 import http.client
 import yaml
 from cuminai.constants import (
     _CUMINAI_CONFIG_DIR,
     _CUMINAI_CONFIG_FILE,
     _CUMINAI_CREATOR_HOST,
@@ -20,22 +19,25 @@
     _GLOBAL_TAGGING,
     _LOCAL_TAGGING,
     _CUMINAI_DUMMY_COLLECTION_NAME,
 )
 
 from cuminai.validator import Validator, UsernameValidator, OllamaEmbeddingFetcher
 
-from langchain_community.embeddings import OllamaEmbeddings
+#from langchain_community.embeddings import OllamaEmbeddings
 import qdrant_client
 from langchain_qdrant import Qdrant
-from cuminai.config import Cuminfile, ChunkStrategy, Tag, KnowledgeSource
+from cuminai.config import Cuminfile
 import cuminai.utils as utils
 from cuminai.chunker import Chunker
 from cuminai.document_loader import Loader
 from cuminai.tagger import Tagger
+from cuminai.embedding import CuminAIEmbeddings
+import logging
+logging.getLogger().setLevel(logging.ERROR)
 
 @click.group()
 def executor():
     pass
 
 @executor.command(help='Log in to a Cumin AI managed knowledge store')
 @click.option('-u', '--username',  help='username', required=True)
@@ -148,18 +150,15 @@
             click.echo("creator not logged in. Run command: 'cuminai login' with username and apikey")
             return
         creds['username'] = data['username']
         creds['apikey'] = data['apikey']
     
     click.echo("creator logged in. got credentials")
 
-    click.echo("Preparing knowledge...")
-    sources = [source_details.source for source_details in cuminfile.knowledge]
-
-    doc_loader = Loader(sources=sources)
+    doc_loader = Loader(knowledge=cuminfile.knowledge)
     
     if cuminfile.kind == _LINK_KIND:
         docs = doc_loader.get_link_docs()
     elif cuminfile.kind == _TEXT_KIND:
         docs = doc_loader.get_text_docs()
 
     parser = None
@@ -167,43 +166,36 @@
         parser = Chunker(docs=docs, 
                         chunk_size=cuminfile.chunkstrategy.size, 
                         chunk_overlap=cuminfile.chunkstrategy.overlap)
     else:
         parser = Chunker(docs=docs)
     
     doc_splits = parser.get_chunks()
-    click.echo("knowledge prepared")
-
-    click.echo("Enriching knowledge metadata...")
 
-    tags = dict()
-    for source in cuminfile.knowledge:
-        tags[source.source] = source.metadata['tags']
+    if cuminfile.kind == _TEXT_KIND:
+        for chunk in doc_splits:
+            chunk.metadata['source'] = utils.get_file_name(chunk.metadata['source'])
 
-    tagger = Tagger(chunks=doc_splits, source_kind=cuminfile.kind, tags=tags)
+    tagger = Tagger(chunks=doc_splits, knowledge=cuminfile.knowledge)
 
     if cuminfile.tag.type == _GLOBAL_TAGGING:
         tagger.add_global_tags()
     elif cuminfile.tag.type == _LOCAL_TAGGING:
         tagger.add_local_tags(cuminfile.tag.minoccurances)
 
     doc_splits = tagger.get_tagged_chunks()
 
-    click.echo("knowledge metadata enriched")
-
     match = OllamaEmbeddingFetcher.match(cuminfile.embedding)
     ollama_embedding_name = match.groups(1)[0]
-    embedding_function = OllamaEmbeddings(model=ollama_embedding_name)
+    embedding_function = CuminAIEmbeddings(model=ollama_embedding_name)
 
     is_public_header = "false"
     if cuminfile.type == _PUBLIC_VISIBILITY:
         is_public_header = "true"
 
-    click.echo("Deploying knowledge to Cumin AI...")
-
     client = qdrant_client.QdrantClient(
         url=_CUMINAI_CREATOR_HOST, 
         port=443,
         https=True,
         metadata={
             _CUMINAI_API_KEY_HEADER: creds['apikey'],
             _CUMINAI_KB_NAME_HEADER: cuminfile.name,
@@ -215,25 +207,23 @@
         store = Qdrant(
             client=client,
             collection_name=_CUMINAI_DUMMY_COLLECTION_NAME,
             embeddings=embedding_function,
         )
 
         store.add_documents(documents=doc_splits)
-        click.echo(f"knowledge deployed and is available at @{creds['username']}/{cuminfile.name}")
+        click.echo(f"Deployment successful... knowledge is available at @{creds['username']}/{cuminfile.name}")
         return
     except qdrant_client.http.exceptions.UnexpectedResponse as e:
         if e.status_code != 404:
             click.echo("Oops... something went wrong. Failed to deploy to Cumin AI")
-            click.echo(e)
             return
         click.echo(f"knowledge source {cuminfile.name} doesn't exist.")
     except ValueError as e:
         click.echo("Oops... something went wrong. Failed to deploy to Cumin AI")
-        click.echo(e)
         return
     
     try:
         click.echo(f"creating knowledge source {cuminfile.name} and uploading knowledge...")
         _ = Qdrant.from_documents(
             documents=doc_splits,
             collection_name=_CUMINAI_DUMMY_COLLECTION_NAME,
@@ -243,22 +233,20 @@
             https=True,
             metadata={
                 _CUMINAI_API_KEY_HEADER: creds['apikey'],
                 _CUMINAI_KB_NAME_HEADER: cuminfile.name,
                 _CUMINAI_IS_PUBLIC_HEADER: is_public_header,
             }
         )
-        click.echo(f"knowledge deployed and is available at @{creds['username']}/{cuminfile.name}")
+        click.echo(f"Deployment successful... knowledge is available at @{creds['username']}/{cuminfile.name}")
     except qdrant_client.http.exceptions.UnexpectedResponse as e:
         click.echo("Oops... something went wrong. Failed to deploy to Cumin AI")
-        click.echo(e)
         return
     except ValueError as e:
         click.echo("Oops... something went wrong. Failed to deploy to Cumin AI")
-        click.echo(e)
         return
 
 def _validate(projectdir, get_parsed=False):
     cuminfile = None
     with open(os.path.join(projectdir, _CUMIN_FILE_NAME), 'r') as f:
         try:
             data = yaml.safe_load(f)
```

### Comparing `cuminai-0.0.1.dev285/cuminai/document_loader.py` & `cuminai-0.0.1.dev295/cuminai/embedding.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,34 @@
+from tqdm.asyncio import tqdm_asyncio
+from typing import List
+from langchain_community.embeddings import OllamaEmbeddings
 import asyncio
 
-from langchain_community.document_loaders import WebBaseLoader, TextLoader
-
 def background(f):
     def wrapped(*args, **kwargs):
         return asyncio.get_event_loop().run_in_executor(None, f, *args, **kwargs)
     return wrapped
 
-class Loader:
-    def __init__(self, **kwargs):
-        self._sources = kwargs.get('sources', [])
+class CuminAIEmbeddings(OllamaEmbeddings):
+    def _embed(self, input: List[str]) -> List[List[float]]:
+        return asyncio.run(self._embed_prompts(input))
 
-    def get_link_docs(self):
-        return asyncio.run(self._aload_link_docs())
-    
-    def get_text_docs(self):
-        return asyncio.run(self._aload_text_docs())
-    
-    async def _aload_link_docs(self):
-        docs = [self._aload_link_doc(url) for url in self._sources]
-        docs_list = [item for sublist in await asyncio.gather(*docs) for item in sublist]
-        return docs_list
-    
-    async def _aload_text_docs(self):
-        docs = [self._aload_text_doc(file) for file in self._sources]
-        docs_list = [item for sublist in await asyncio.gather(*docs) for item in sublist]
-        return docs_list
-    
-    @background
-    def _aload_link_doc(self, url):
-        return WebBaseLoader(url).load()
+    def embed_documents(self, texts: List[str]) -> List[List[float]]:
+        """Embed documents using an Ollama deployed embedding model.
+
+        Args:
+            texts: The list of texts to embed.
+
+        Returns:
+            List of embeddings, one for each text.
+        """
+        instruction_pairs = [f"{self.embed_instruction}{text}" for text in texts]
+        embeddings = self._embed(instruction_pairs)
+        return embeddings
     
+    async def _embed_prompts(self, prompts):
+        embeddings = [self._aembed_prompt(prompt) for prompt in prompts]
+        return await tqdm_asyncio.gather(*embeddings, desc="Embedding Knowledge")
+
     @background
-    def _aload_text_doc(self, filename):
-        return TextLoader(f"./{filename}", autodetect_encoding=True).load()
+    def _aembed_prompt(self, prompt):
+        return self._process_emb_response(prompt)
```

### Comparing `cuminai-0.0.1.dev285/cuminai/tagger.py` & `cuminai-0.0.1.dev295/cuminai/tagger.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,47 @@
-from cuminai.constants import (
-    _LINK_KIND,
-    _TEXT_KIND
-)
+import asyncio
+from tqdm.asyncio import tqdm_asyncio
 
 import cuminai.utils as utils
 
+def background(f):
+    def wrapped(*args, **kwargs):
+        return asyncio.get_event_loop().run_in_executor(None, f, *args, **kwargs)
+    return wrapped
+
 class Tagger:
-    def __init__(self, chunks, source_kind, tags, **kwargs):
+    def __init__(self, chunks, knowledge, **kwargs):
         self._chunks = chunks
-        self._sourcekind = source_kind
+        
+        tags = dict()
+        for source in knowledge:
+            tags[source.source] = [tag.lower() for tag in source.metadata['tags']]
+        
         self._tags = tags
 
     def add_global_tags(self):
-        if self._sourcekind == _LINK_KIND:
-            for chunk in self._chunks:
-                for tag in self._tags[chunk.metadata['source']]:
-                    chunk.metadata[f'tag-{utils.get_processed_tag(tag)}'] = True
-        elif self._sourcekind == _TEXT_KIND:
-            for chunk in self._chunks:
-                for tag in self._tags[utils.get_file_name(chunk.metadata['source'])]:
-                    chunk.metadata[f'tag-{utils.get_processed_tag(tag)}'] = True
+        asyncio.run(self._tag_chunks_global())
 
     def add_local_tags(self, tag_threshold):
-        if self._sourcekind == _LINK_KIND:
-            for chunk in self._chunks:
-                for tag in self._tags[chunk.metadata['source']]:
-                    if utils.num_found(chunk.page_content, tag) >= tag_threshold:
-                        chunk.metadata[f'tag-{utils.get_processed_tag(tag)}'] = True
-        elif self._sourcekind == _TEXT_KIND:
-            for chunk in self._chunks:
-                for tag in self._tags[utils.get_file_name(chunk.metadata['source'])]:
-                    if utils.num_found(chunk.page_content, tag) >= tag_threshold:
-                        chunk.metadata[f'tag-{utils.get_processed_tag(tag)}'] = True
+        asyncio.run(self._tag_chunks_local(tag_threshold))
 
     def get_tagged_chunks(self):
-        return self._chunks
+        return self._chunks
+    
+    async def _tag_chunks_global(self):
+        tasks = [self._tag_chunk_global(chunk) for chunk in self._chunks]
+        await tqdm_asyncio.gather(*tasks, desc="Tagging Knowledge")
+
+    @background
+    def _tag_chunk_global(self, chunk):
+        for tag in self._tags[chunk.metadata['source']]:
+            chunk.metadata[f'tag-{utils.get_processed_tag(tag)}'] = True
+    
+    async def _tag_chunks_local(self, tag_threshold):
+        tasks = [self._tag_chunk_local(chunk, tag_threshold) for chunk in self._chunks]
+        await tqdm_asyncio.gather(*tasks, desc="Tagging Knowledge")
+    
+    @background
+    def _tag_chunk_local(self, chunk, tag_threshold):
+        for tag in self._tags[chunk.metadata['source']]:
+            if utils.num_found(chunk.page_content, tag) >= tag_threshold:
+                chunk.metadata[f'tag-{utils.get_processed_tag(tag)}'] = True
```

### Comparing `cuminai-0.0.1.dev285/cuminai/utils.py` & `cuminai-0.0.1.dev295/cuminai/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,11 +15,11 @@
     
     return False
 
 def get_processed_tag(tag):
     return tag.lower().replace("-","_").replace(" ", "_")
 
 def num_found(page_content, tag):
-    return page_content.lower().count(tag.lower())
+    return page_content.lower().count(tag)
 
 def get_file_name(path):
     return Path(path).name
```

### Comparing `cuminai-0.0.1.dev285/cuminai/validator.py` & `cuminai-0.0.1.dev295/cuminai/validator.py`

 * *Files identical despite different names*

### Comparing `cuminai-0.0.1.dev285/LICENSE` & `cuminai-0.0.1.dev295/LICENSE`

 * *Files identical despite different names*

### Comparing `cuminai-0.0.1.dev285/pyproject.toml` & `cuminai-0.0.1.dev295/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "cuminai"
-version = "0.0.1dev285"
+version = "0.0.1dev295"
 description = ""
 authors = ["Harshal Priyadarshi <harshal@cuminai.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 langchain_qdrant = ">=0.1.0"
 qdrant-client = ">=1.0.0"
 langchain-community = ">=0.0.10"
 langchain_text_splitters = ">=0.0.1"
 beautifulsoup4 = ">=4.10.0"
 tiktoken = ">=0.4.0"
 click = ">=8.1.0"
 chardet = ">=5.2.0"
+tqdm = ">=4.66.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 cuminai = "cuminai.creator:executor"
```

### Comparing `cuminai-0.0.1.dev285/README.md` & `cuminai-0.0.1.dev295/README.md`

 * *Files identical despite different names*

### Comparing `cuminai-0.0.1.dev285/PKG-INFO` & `cuminai-0.0.1.dev295/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuminai
-Version: 0.0.1.dev285
+Version: 0.0.1.dev295
 Summary: 
 Author: Harshal Priyadarshi
 Author-email: harshal@cuminai.com
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -14,14 +14,15 @@
 Requires-Dist: chardet (>=5.2.0)
 Requires-Dist: click (>=8.1.0)
 Requires-Dist: langchain-community (>=0.0.10)
 Requires-Dist: langchain_qdrant (>=0.1.0)
 Requires-Dist: langchain_text_splitters (>=0.0.1)
 Requires-Dist: qdrant-client (>=1.0.0)
 Requires-Dist: tiktoken (>=0.4.0)
+Requires-Dist: tqdm (>=4.66.0)
 Description-Content-Type: text/markdown
 
 # cuminai
 
 This package contains the Cumin AI Python SDK. Cumin AI is a Managed LLM Context Service. This package provides integration with Langchain.
 
 ## Installation
```

