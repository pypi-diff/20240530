# Comparing `tmp/hal9-2.1.5.tar.gz` & `tmp/hal9-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hal9-2.1.5.tar", max compression
+gzip compressed data, was "hal9-2.1.6.tar", max compression
```

## Comparing `hal9-2.1.5.tar` & `hal9-2.1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     2948 2024-05-28 20:23:05.052425 hal9-2.1.5/README.md
--rw-r--r--   0        0        0       86 2024-05-28 20:23:04.592424 hal9-2.1.5/hal9/__init__.py
--rw-r--r--   0        0        0     1220 2024-05-28 20:23:04.592424 hal9-2.1.5/hal9/cli.py
--rw-r--r--   0        0        0      634 2024-05-28 20:23:04.592424 hal9-2.1.5/hal9/create.py
--rw-r--r--   0        0        0      574 2024-05-28 20:23:04.592424 hal9-2.1.5/hal9/deploy.py
--rw-r--r--   0        0        0      531 2024-05-28 20:23:04.592424 hal9-2.1.5/hal9/run.py
--rw-r--r--   0        0        0      352 2024-05-28 20:23:04.592424 hal9-2.1.5/hal9/targets/docker.py
--rw-r--r--   0        0        0     2021 2024-05-28 20:23:04.592424 hal9-2.1.5/hal9/targets/hal9.py
--rw-r--r--   0        0        0       42 2024-05-28 20:23:04.592424 hal9-2.1.5/hal9/templates/docker/Dockerfile
--rw-r--r--   0        0        0       38 2024-05-28 20:23:04.592424 hal9-2.1.5/hal9/templates/openai/app.py
--rw-r--r--   0        0        0      434 2024-05-28 20:23:04.592424 hal9-2.1.5/pyproject.toml
--rw-r--r--   0        0        0     3586 1970-01-01 00:00:00.000000 hal9-2.1.5/PKG-INFO
+-rw-r--r--   0        0        0     3698 2024-05-30 15:37:06.740765 hal9-2.1.6/README.md
+-rw-r--r--   0        0        0       86 2024-05-30 15:37:06.644766 hal9-2.1.6/hal9/__init__.py
+-rw-r--r--   0        0        0     1220 2024-05-30 15:37:06.644766 hal9-2.1.6/hal9/cli.py
+-rw-r--r--   0        0        0      634 2024-05-30 15:37:06.644766 hal9-2.1.6/hal9/create.py
+-rw-r--r--   0        0        0      574 2024-05-30 15:37:06.644766 hal9-2.1.6/hal9/deploy.py
+-rw-r--r--   0        0        0      531 2024-05-30 15:37:06.644766 hal9-2.1.6/hal9/run.py
+-rw-r--r--   0        0        0      352 2024-05-30 15:37:06.644766 hal9-2.1.6/hal9/targets/docker.py
+-rw-r--r--   0        0        0     2021 2024-05-30 15:37:06.644766 hal9-2.1.6/hal9/targets/hal9.py
+-rw-r--r--   0        0        0       42 2024-05-30 15:37:06.644766 hal9-2.1.6/hal9/templates/docker/Dockerfile
+-rw-r--r--   0        0        0       38 2024-05-30 15:37:06.644766 hal9-2.1.6/hal9/templates/openai/app.py
+-rw-r--r--   0        0        0      434 2024-05-30 15:37:06.644766 hal9-2.1.6/pyproject.toml
+-rw-r--r--   0        0        0     4336 1970-01-01 00:00:00.000000 hal9-2.1.6/PKG-INFO
```

### Comparing `hal9-2.1.5/hal9/cli.py` & `hal9-2.1.6/hal9/cli.py`

 * *Files identical despite different names*

### Comparing `hal9-2.1.5/hal9/create.py` & `hal9-2.1.6/hal9/create.py`

 * *Files identical despite different names*

### Comparing `hal9-2.1.5/hal9/deploy.py` & `hal9-2.1.6/hal9/deploy.py`

 * *Files identical despite different names*

### Comparing `hal9-2.1.5/hal9/run.py` & `hal9-2.1.6/hal9/run.py`

 * *Files identical despite different names*

### Comparing `hal9-2.1.5/hal9/targets/hal9.py` & `hal9-2.1.6/hal9/targets/hal9.py`

 * *Files identical despite different names*

### Comparing `hal9-2.1.5/PKG-INFO` & `hal9-2.1.6/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,17 @@
-Metadata-Version: 2.1
-Name: hal9
-Version: 2.1.5
-Summary: 
-Author: Javier Luraschi
-Author-email: javier@hal9.ai
-Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: click (>=8.1.7,<9.0.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
-Description-Content-Type: text/markdown
-
 # Hal9: Create and Share Generative Apps
 
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Hal9 PyPi Downloads](https://img.shields.io/pypi/dm/hal9?label=PyPI)](https://pypi.org/project/hal9/)
+[![GitHub star chart](https://img.shields.io/github/stars/hal9ai/hal9?style=flat-square)](https://star-history.com/#hal9ai/hal9)
 
-Create and deploy generative (LLMs and [difussers](https://github.com/huggingface/diffusers)) applications (chatbots and APIs) in seconds.
-- **Open:** Use any model (OpenAI, Llama, Groq, Midjourney) and any library like (LangChainl, DSPy).
-- **Intuitive:** No need to learn app frameworks (flask), simply use stdin and stdout, or write file to disk.
-- **Scalable:** Engineers can integrate your app with scalable technilogies (Docker, Kubernetes, etc)
+Create and deploy generative ([LLMs](https://github.com/Hannibal046/Awesome-LLM) and [diffusers](https://github.com/huggingface/diffusers)) applications (chatbots and APIs) in seconds.
+- **Open:** Use any model ([OpenAI](https://platform.openai.com/docs/api-reference/introduction), [Llama](https://ai.meta.com/blog/5-steps-to-getting-started-with-llama-2/), [Groq](https://docs.api.groq.com/md/tutorials/python.groqapi.html), [MidJourney](https://docs.imagineapi.dev/en)) and any library like ([LangChainl](https://python.langchain.com/v0.1/docs/get_started/quickstart/), [DSPy](https://dspy-docs.vercel.app/docs/quick-start/installation)).
+- **Intuitive:** No need to learn app frameworks ([Flask](https://flask.palletsprojects.com/en/3.0.x/quickstart/)), simply use stdin and stdout, or write file to disk.
+- **Scalable:** Engineers can integrate your app with scalable technilogies ([Docker](https://www.docker.com/), [Kubernetes](https://kubernetes.io/), etc)
 - **Powerful:** Using an OS process (stdin, stdout, files) as our app contract, enables long-running agents, multiple programming languages, and complex system dependencies.
 
 Focus on AI (RAG, fine-tuning, aligment, training) and skip engineering tasks (frontend development, backend integration, deployment, operations).
 
 ## Getting started
 
 Create and share a chatbot in seconds by running the following commands:
@@ -99,8 +84,7 @@
 
 For personal use, `--target hal9` supports a free tier at `hal9.com`; enterprise support is also available to deploy with `--target hal9 --url hal9.yourcompany.com`
 
 ## Contributing
 
 Pull Requests are welcomed to consider additional application templates or deployment targets. See [CONTIBUTE.md](CONTIBUTE.md).
 
-
```

