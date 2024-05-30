# Comparing `tmp/comfy_catapult-2.0.0.tar.gz` & `tmp/comfy_catapult-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comfy_catapult-2.0.0.tar", last modified: Tue Apr  2 19:24:00 2024, max compression
+gzip compressed data, was "comfy_catapult-2.2.0.tar", last modified: Thu May 30 06:15:13 2024, max compression
```

## Comparing `comfy_catapult-2.0.0.tar` & `comfy_catapult-2.2.0.tar`

### file list

```diff
@@ -1,34 +1,31 @@
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-04-02 19:24:00.272452 comfy_catapult-2.0.0/
--rwxrwxrwx   0 realz     (1000) realz     (1000)     1102 2024-01-11 16:26:42.000000 comfy_catapult-2.0.0/LICENSE.md
--rwxrwxrwx   0 realz     (1000) realz     (1000)    24255 2024-04-02 19:24:00.263341 comfy_catapult-2.0.0/PKG-INFO
--rwxrwxrwx   0 realz     (1000) realz     (1000)    17215 2024-04-02 19:19:54.000000 comfy_catapult-2.0.0/README.md
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-04-02 19:24:00.123517 comfy_catapult-2.0.0/comfy_catapult/
--rwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-01-11 16:26:42.000000 comfy_catapult-2.0.0/comfy_catapult/__init__.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)    13665 2024-04-02 19:19:54.000000 comfy_catapult-2.0.0/comfy_catapult/api_client.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)     6464 2024-02-19 01:20:59.000000 comfy_catapult-2.0.0/comfy_catapult/api_client_base.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)    30008 2024-04-02 19:19:54.000000 comfy_catapult-2.0.0/comfy_catapult/catapult.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)     3291 2024-04-02 19:19:54.000000 comfy_catapult-2.0.0/comfy_catapult/catapult_base.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)    16582 2024-04-02 19:19:54.000000 comfy_catapult-2.0.0/comfy_catapult/comfy_schema.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)     4859 2024-04-02 19:19:54.000000 comfy_catapult-2.0.0/comfy_catapult/comfy_schema_test.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)    15682 2024-04-02 19:19:54.000000 comfy_catapult-2.0.0/comfy_catapult/comfy_utils.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)     2237 2024-04-02 19:19:54.000000 comfy_catapult-2.0.0/comfy_catapult/errors.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)     5983 2024-01-06 03:17:37.000000 comfy_catapult-2.0.0/comfy_catapult/eta_estimator.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)     2325 2024-04-02 19:19:54.000000 comfy_catapult-2.0.0/comfy_catapult/remote_file_api_base.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)    11630 2024-04-02 19:19:54.000000 comfy_catapult-2.0.0/comfy_catapult/remote_file_api_comfy.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)     8441 2024-04-02 19:19:54.000000 comfy_catapult-2.0.0/comfy_catapult/remote_file_api_comfy_test.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)     5634 2024-04-02 19:19:54.000000 comfy_catapult-2.0.0/comfy_catapult/remote_file_api_generic.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)     5772 2024-04-02 19:19:54.000000 comfy_catapult-2.0.0/comfy_catapult/remote_file_api_local.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)     4188 2024-04-02 19:19:54.000000 comfy_catapult-2.0.0/comfy_catapult/url_utils.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)      377 2024-04-02 19:19:54.000000 comfy_catapult-2.0.0/comfy_catapult/url_utils_test.py
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-04-02 19:24:00.245200 comfy_catapult-2.0.0/comfy_catapult.egg-info/
--rwxrwxrwx   0 realz     (1000) realz     (1000)    24255 2024-04-02 19:23:59.000000 comfy_catapult-2.0.0/comfy_catapult.egg-info/PKG-INFO
--rwxrwxrwx   0 realz     (1000) realz     (1000)      868 2024-04-02 19:23:59.000000 comfy_catapult-2.0.0/comfy_catapult.egg-info/SOURCES.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)        1 2024-04-02 19:23:59.000000 comfy_catapult-2.0.0/comfy_catapult.egg-info/dependency_links.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)     1929 2024-04-02 19:23:59.000000 comfy_catapult-2.0.0/comfy_catapult.egg-info/requires.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)       15 2024-04-02 19:23:59.000000 comfy_catapult-2.0.0/comfy_catapult.egg-info/top_level.txt
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-04-02 19:23:59.860027 comfy_catapult-2.0.0/examples/
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-04-02 19:24:00.225127 comfy_catapult-2.0.0/examples/utilities/
--rwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-01-11 16:26:42.000000 comfy_catapult-2.0.0/examples/utilities/__init__.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)     6227 2024-02-01 21:10:02.000000 comfy_catapult-2.0.0/examples/utilities/sdxlturbo_parse_args.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)     4122 2024-04-02 19:19:54.000000 comfy_catapult-2.0.0/pyproject.toml
--rwxrwxrwx   0 realz     (1000) realz     (1000)       38 2024-04-02 19:24:00.273961 comfy_catapult-2.0.0/setup.cfg
+drwxr-xr-x   0 realz     (1000) realz     (1000)        0 2024-05-30 06:15:13.238168 comfy_catapult-2.2.0/
+-rw-r--r--   0 realz     (1000) realz     (1000)     1102 2024-05-30 06:13:40.000000 comfy_catapult-2.2.0/LICENSE.md
+-rw-r--r--   0 realz     (1000) realz     (1000)     9761 2024-05-30 06:15:13.238168 comfy_catapult-2.2.0/PKG-INFO
+-rw-r--r--   0 realz     (1000) realz     (1000)    21324 2024-05-30 06:13:40.000000 comfy_catapult-2.2.0/README.md
+drwxr-xr-x   0 realz     (1000) realz     (1000)        0 2024-05-30 06:15:13.218167 comfy_catapult-2.2.0/comfy_catapult/
+-rw-r--r--   0 realz     (1000) realz     (1000)      398 2024-05-30 06:13:40.000000 comfy_catapult-2.2.0/comfy_catapult/__init__.py
+-rw-r--r--   0 realz     (1000) realz     (1000)    13636 2024-05-30 06:13:40.000000 comfy_catapult-2.2.0/comfy_catapult/api_client.py
+-rw-r--r--   0 realz     (1000) realz     (1000)     6825 2024-05-30 06:13:40.000000 comfy_catapult-2.2.0/comfy_catapult/api_client_base.py
+-rw-r--r--   0 realz     (1000) realz     (1000)    31627 2024-05-30 06:13:40.000000 comfy_catapult-2.2.0/comfy_catapult/catapult.py
+-rw-r--r--   0 realz     (1000) realz     (1000)     3851 2024-05-30 06:13:40.000000 comfy_catapult-2.2.0/comfy_catapult/catapult_base.py
+-rw-r--r--   0 realz     (1000) realz     (1000)     8417 2024-05-30 06:13:40.000000 comfy_catapult-2.2.0/comfy_catapult/cli.py
+-rw-r--r--   0 realz     (1000) realz     (1000)    16893 2024-05-30 06:13:40.000000 comfy_catapult-2.2.0/comfy_catapult/comfy_schema.py
+-rw-r--r--   0 realz     (1000) realz     (1000)     4788 2024-05-30 06:13:40.000000 comfy_catapult-2.2.0/comfy_catapult/comfy_schema_test.py
+-rw-r--r--   0 realz     (1000) realz     (1000)    15721 2024-05-30 06:13:40.000000 comfy_catapult-2.2.0/comfy_catapult/comfy_utils.py
+-rw-r--r--   0 realz     (1000) realz     (1000)     2387 2024-05-30 06:13:40.000000 comfy_catapult-2.2.0/comfy_catapult/errors.py
+-rw-r--r--   0 realz     (1000) realz     (1000)        0 2024-05-30 06:13:40.000000 comfy_catapult-2.2.0/comfy_catapult/py.typed
+-rw-r--r--   0 realz     (1000) realz     (1000)     2313 2024-05-30 06:13:40.000000 comfy_catapult-2.2.0/comfy_catapult/remote_file_api_base.py
+-rw-r--r--   0 realz     (1000) realz     (1000)    11640 2024-05-30 06:13:40.000000 comfy_catapult-2.2.0/comfy_catapult/remote_file_api_comfy.py
+-rw-r--r--   0 realz     (1000) realz     (1000)     8357 2024-05-30 06:13:40.000000 comfy_catapult-2.2.0/comfy_catapult/remote_file_api_comfy_test.py
+-rw-r--r--   0 realz     (1000) realz     (1000)     5627 2024-05-30 06:13:40.000000 comfy_catapult-2.2.0/comfy_catapult/remote_file_api_generic.py
+-rw-r--r--   0 realz     (1000) realz     (1000)     5715 2024-05-30 06:13:40.000000 comfy_catapult-2.2.0/comfy_catapult/remote_file_api_local.py
+-rw-r--r--   0 realz     (1000) realz     (1000)     4125 2024-05-30 06:13:40.000000 comfy_catapult-2.2.0/comfy_catapult/url_utils.py
+-rw-r--r--   0 realz     (1000) realz     (1000)      377 2024-05-30 06:13:40.000000 comfy_catapult-2.2.0/comfy_catapult/url_utils_test.py
+drwxr-xr-x   0 realz     (1000) realz     (1000)        0 2024-05-30 06:15:13.228167 comfy_catapult-2.2.0/comfy_catapult.egg-info/
+-rw-r--r--   0 realz     (1000) realz     (1000)     9761 2024-05-30 06:15:13.000000 comfy_catapult-2.2.0/comfy_catapult.egg-info/PKG-INFO
+-rw-r--r--   0 realz     (1000) realz     (1000)      808 2024-05-30 06:15:13.000000 comfy_catapult-2.2.0/comfy_catapult.egg-info/SOURCES.txt
+-rw-r--r--   0 realz     (1000) realz     (1000)        1 2024-05-30 06:15:13.000000 comfy_catapult-2.2.0/comfy_catapult.egg-info/dependency_links.txt
+-rw-r--r--   0 realz     (1000) realz     (1000)     3037 2024-05-30 06:15:13.000000 comfy_catapult-2.2.0/comfy_catapult.egg-info/requires.txt
+-rw-r--r--   0 realz     (1000) realz     (1000)       15 2024-05-30 06:15:13.000000 comfy_catapult-2.2.0/comfy_catapult.egg-info/top_level.txt
+-rw-r--r--   0 realz     (1000) realz     (1000)     5571 2024-05-30 06:13:40.000000 comfy_catapult-2.2.0/pyproject.toml
+-rw-r--r--   0 realz     (1000) realz     (1000)       38 2024-05-30 06:15:13.238168 comfy_catapult-2.2.0/setup.cfg
```

### Comparing `comfy_catapult-2.0.0/LICENSE.md` & `comfy_catapult-2.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `comfy_catapult-2.0.0/README.md` & `comfy_catapult-2.2.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -4,28 +4,74 @@
 SOURCE: `README.md.jinja2`.
 
 -->
 <!-- Note: This file is a jinja2 template of a Markdown file.                -->
 <!--
 
 
+
+
+
+
+
 -->
 
-# README
+# <div align="center">![Comfy Catapult][24]</div>
 
-**Warning:** Very raw and unmaintained code. Use at your own risk. Mainly
-intended as a starting point.
+<div align="center">
+<!-- Icons from https://lucide.dev/icons/users -->
+<!-- Icons from https://lucide.dev/icons/laptop-minimal -->
+
+![**Audience:** Developers][25] ![**Platform:** Linux][26]
+
+</div>
+
+<p align="center">
+  <strong>
+    <a href="https://github.com/realazthat/comfy-catapult">🏠Home</a>
+    &nbsp;&bull;&nbsp;
+    <a href="#-features">🎇Features</a>
+    &nbsp;&bull;&nbsp;
+    <a href="#-installation">🔨Installation</a>
+    &nbsp;&bull;&nbsp;
+    <a href="#-usage">🚜Usage</a>
+    &nbsp;&bull;&nbsp;
+    <a href="#-documentation">📘Documentation</a>
+    &nbsp;&bull;&nbsp;
+    <a href="#-api">🤖API</a>
+  </strong>
+</p>
+<p align="center">
+  <strong>
+    <a href="#-requirements">✅Requirements</a>
+    &nbsp;&bull;&nbsp;
+    <a href="#-limitations">🚸Limitations</a>
+  </strong>
+</p>
+
+<div align="center">
 
 ![Top language][19] ![GitHub License][11] [![PyPI - Version][12]][13]
 [![Python Version][18]][13]
 
-| Branch  | Build Status              |                                              |
-| ------- | ------------------------- | -------------------------------------------- |
-| Master  | [![Build and Test][1]][2] | [![since tagged][14]][20] ![last commit][16] |
-| Develop | [![Build and Test][3]][4] | [![since tagged][15]][21] ![last commit][17] |
+**Python library to programmatically schedule ComfyUI workflows via the ComfyUI
+API**
+
+</div>
+
+---
+
+<div align="center">
+
+| Branch        | Build Status              | Commits Since             | Last Commit        |
+| ------------- | ------------------------- | ------------------------- | ------------------ |
+| [Master][27]  | [![Build and Test][1]][2] | [![since tagged][14]][20] | ![last commit][16] |
+| [Develop][28] | [![Build and Test][3]][4] | [![since tagged][15]][21] | ![last commit][17] |
+
+</div>
 
 ```
 ComfyUI API Endpoint <| <=  Comfy Catapult <=> HTTP Server <| <=  Public users
                      <|                                    <|
                      <|         Your python program        <| Your Webui/JS frontend
                      <|                                    <|
                      <|           Your workflows           <|
@@ -37,27 +83,73 @@
 Comfy Catapult is a library for scheduling and running ComfyUI workflows from a
 Python program, via the existing API endpoint. ComfyUI typically works by
 hosting this API endpoint for its user interface.
 
 This makes it easier for you to make workflows via the UI, and then use it from
 a program.
 
-### Scheduling a job
+## 🎇 Features
+
+- ComfyUI API client
+  ([interface](./comfy_catapult/api_client_base.py),
+  [implementation](./comfy_catapult/api_client.py)).
+- ComfyUI Workflow scheduler
+  ([interface](./comfy_catapult/catapult_base.py),
+  [implementation](./comfy_catapult/catapult.py)).
+- ComfyUI API Pydantic Schema
+  ([./comfy_catapult/comfy_schema.py](./comfy_catapult/comfy_schema.py)).
+- Helpers to handle uploading and downloading files to/from ComfyUI.
+- Simple CLI to execute workflows.
+
+## 🔨 Installation
+
+```bash
+# Inside your environment:
+
+# From pypi:
+pip install comfy_catapult
+
+# From git:
+pip install git+https://github.com/realazthat/comfy-catapult.git@v2.2.0
+```
+
+## 🚜 Usage
+
+## Related Projects
+
+| Project                          | ComfyUI API Wrapper | Outsource Backend | Distribute Execution | Wrap Workflow | Studio |
+| -------------------------------- | ------------------- | ----------------- | -------------------- | ------------- | ------ |
+| [CushyStudio][31]                | ?                   | ?                 | ?                    | ?             | Yes    |
+| [ComfyUI-Serving-Toolkit][30]    | X                   | ?                 | ?                    | Yes           | ?      |
+| [ComfyUI_NetDist][29]            | X                   | ?                 | Yes                  | ?             | ?      |
+| [ComfyUI script_examples][32]    | Yes                 | No                | No                   | No            | No     |
+| [comfyui-python-api][5]          | ?                   | ?                 | ?                    | Yes           | ?      |
+| [comfyui-deploy][6]              | ?                   | ?                 | ?                    | Yes           | ?      |
+| [ComfyUI-to-Python-Extension][7] | ?                   | ?                 | ?                    | Yes           | ?      |
+| [ComfyScript][8]                 | ?                   | ?                 | ?                    | Yes           | ?      |
+| [hordelib][9]                    | ?                   | Yes               | ?                    | ?             | ?      |
+| [comfyui-cloud][10]              | ?                   | Yes               | ?                    | ?             | ?      |
+| [comfy_runner][22]               | ?                   | ?                 | ?                    | ?             | ?      |
+| [ComfyUI-ComfyRun][23]           | ?                   | ?                 | ?                    | ?             | ?      |
+
+## 📘 Documentation
+
+### Scheduling a Job
 
 From
 [`comfy_catapult/catapult_base.py`](comfy_catapult/catapult_base.py):
 
 ````py
   async def Catapult(
       self,
       *,
       job_id: str,
       prepared_workflow: dict,
       important: Sequence[APINodeID],
-      job_debug_path: Path | None = None,
+      job_debug_path: Optional[Path] = None,
   ) -> dict:
     """Schedule a ComfyUI workflow job.
 
     Args:
         job_id (str): A unique identifier for the job. Note: This string must
           be unique, and must be slugified! Use python-slugify to slugify the
           string.
@@ -71,14 +163,16 @@
         WorkflowSubmissionError: Failed to submit workflow.
 
     Returns:
         dict: The history of the job returned from the ComfyUI API.
     """
 ````
 
+### Example usage:
+
 From
 [`examples/sdxlturbo_example_catapulter.py`](examples/sdxlturbo_example_catapulter.py):
 
 ````py
 class ExampleWorkflowInfo:
   # Direct wrapper around the ComfyUI API.
   client: ComfyAPIClientBase
@@ -125,42 +219,23 @@
       job_id=job_id, prepared_workflow=workflow_dict, important=important)
 
   # Now that the job is done, you have to write something that will go and get
   # the results you care about, if necessary.
   await DownloadResults(job_info=job_info)
 ````
 
-## Related Projects
-
-| Project                          | ComfyUI API Wrapper | Outsource Backend | Distribute Execution | Wrap Workflow | Studio |
-| -------------------------------- | ------------------- | ----------------- | -------------------- | ------------- | ------ |
-| [CushyStudio][2]                 | ?                   | ?                 | ?                    | ?             | Yes    |
-| [ComfyUI-Serving-Toolkit][3]     | X                   | ?                 | ?                    | Yes           | ?      |
-| [ComfyUI_NetDist][4]             | X                   | ?                 | Yes                  | ?             | ?      |
-| [ComfyUI script_examples][1]     | Yes                 | No                | No                   | No            | No     |
-| [comfyui-python-api][5]          | ?                   | ?                 | ?                    | Yes           | ?      |
-| [comfyui-deploy][6]              | ?                   | ?                 | ?                    | Yes           | ?      |
-| [ComfyUI-to-Python-Extension][7] | ?                   | ?                 | ?                    | Yes           | ?      |
-| [ComfyScript][8]                 | ?                   | ?                 | ?                    | Yes           | ?      |
-| [hordelib][9]                    | ?                   | Yes               | ?                    | ?             | ?      |
-| [comfyui-cloud][10]              | ?                   | Yes               | ?                    | ?             | ?      |
-
-**Outsource compute:**
-
-## Getting Started
-
 ### Exporting workflows in the API json format
 
 In ComfyUI web interface:
 
 1. Open settings (gear box in the corner).
 2. Enable the ability to export in the API format, `Enable Dev mode Options`.
 3. Click new menu item `Save (API format)`.
 
-![ComfyUI API format export instructions](assets/comfy-export-instructions.png)
+![ComfyUI API format export instructions](.github/comfy-export-instructions.png)
 
 ### Example workflow: Prepare ComfyUI
 
 **If you don't want to try the example workflow, you can skip this section.**
 
 You need to get `sd_xl_turbo_1.0_fp16.safetensors` into the ComfyUI model
 directory.
@@ -184,20 +259,17 @@
 # to automated this right now.
 #
 # 2, Save to `./sdxlturbo_example_api.json`.
 #
 # Or just use `test_data/sdxlturbo_example_api.json`.
 ```
 
-### Install as a library and run the examples
+### Run the examples
 
 ```bash
-# Inside your environment:
-pip install comfy-catapult
-
 
 
 # If you set this environment variable, you don't have to specify it as an
 # argument.
 export COMFY_API_URL=http://127.0.0.1:8188
 # Note, in WSL2 you may have to use the IP of the host to connect to ComfyUI.
 
@@ -214,74 +286,48 @@
 
 # Done! Now $PWD/.deleteme/output.png should contain the output image.
 
 # Some other examples:
 python -m comfy_catapult.examples.add_a_node
 python -m comfy_catapult.examples.using_pydantic
 
-
-
 ```
 
-- Examine
-  [`examples/sdxlturbo_example_catapulter.py`](examples/sdxlturbo_example_catapulter.py)
-  to see how to use the main `ComfyCatapult` library.
-- Examine
-  [`test_data/sdxlturbo_example_api.json`](test_data/sdxlturbo_example_api.json)
-  to see the API format. This will be necessary in order to programmatically set
-  the proper inputs for the workflow.
-  - (Optional) See [`examples/using_pydantic.py`](examples/using_pydantic.py)
-    for how to parse the API format into the Pydantic models schema for easier
+### 🤖 API
+
+- Examine [./examples/sdxlturbo_example_catapulter.py](./examples/sdxlturbo_example_catapulter.py) to
+  see how to use the main `ComfyCatapult` library.
+- Examine [./test_data/sdxlturbo_example_api.json](./test_data/sdxlturbo_example_api.json) to see
+  the API format. This will be necessary in order to programmatically set the
+  proper inputs for the workflow.
+  - (Optional) See [./examples/using_pydantic.py](./examples/using_pydantic.py) for how
+    to parse the API format into the Pydantic models schema for easier
     navigation.
-  - (Optional) See [`examples/add_a_node.py`](examples/add_a_node.py) for how to
+  - (Optional) See [./examples/add_a_node.py](./examples/add_a_node.py) for how to
     add a new node to a workflow. This is useful when you need to add nodes at
     runtime (such as adding a bunch of LoadImage nodes).
-- See [`comfy_catapult/catapult_base.py`](comfy_catapult/catapult_base.py) for
-  the main library interface.
-- (Optional) See [`comfy_catapult/catapult.py`](comfy_catapult/catapult_base.py)
-  for the main library implementation.
-- (Optional) See
-  [`comfy_catapult/api_client_base.py`](comfy_catapult/api_client_base.py) for
+- See [./comfy_catapult/catapult_base.py](./comfy_catapult/catapult_base.py) for the main
+  library interface.
+- (Optional) See [./comfy_catapult/catapult.py](./comfy_catapult/catapult.py) for the
+  main library implementation.
+- (Optional) See [./comfy_catapult/api_client_base.py](./comfy_catapult/api_client_base.py) for
   the direct ComfyUI API endpoint client library interface; you don't need to
   use this usually.
 - (Optional) For those who want to do use the raw API themselves and learn how
-  it works: Examine
-  [`comfy_catapult/api_client.py`](comfy_catapult/api_client.py) to see the API
-  client implementation if you want to directly interface with ComfyUI endpoints
-  yourself.
+  it works: Examine [./comfy_catapult/api_client.py](./comfy_catapult/api_client.py) to see
+  the API client implementation if you want to directly interface with ComfyUI
+  endpoints yourself.
   - (Optional) Also see
     [ComfyUI/server.py](https://github.com/comfyanonymous/ComfyUI/blob/977eda19a6471fbff253dc92c3c2f1a4a67b1793/server.py#L99)
     (pinned to a specific commit) for the server `@routes` endpoint
     implementations.
 
-### Development; install dependencies and run the examples
-
-This is if you are intending on contributing or altering the library itself.
-
-```bash
-
-git clone https://github.com/realazthat/comfy-catapult.git
-cd comfy-catapult
-pip install -r requirements.txt
-
-
-# Run the example workflow:
-PYTHONPATH=$PYTHONPATH:$PWD python examples/sdxlturbo_example_catapulter.py \
-  --api_workflow_json_path "$PWD/sdxlturbo_example_api.json"
-  --tmp_path "$PWD/.deleteme/tmp/" \
-  --output_path "$PWD/.deleteme/output.png" \
-  --positive_prompt "amazing cloudscape, towering clouds, thunderstorm, awe" \
-  --negative_prompt "dull, blurry, nsfw"
-
-
-```
-
 ### Parsing the API format into the Pydantic models schema for easier navigation
 
-From [`examples/using_pydantic.py`](examples/using_pydantic.py):
+From [./examples/using_pydantic.py](./examples/using_pydantic.py):
 
 ````py
 
 from comfy_catapult.comfy_schema import APIWorkflow
 
 api_workflow_json_str: str = """
 {
@@ -322,15 +368,15 @@
 
 print(api_workflow_json)
 # 
 ````
 
 ### Adding a new node to a workflow
 
-From [`examples/add_a_node.py`](examples/add_a_node.py):
+From [examples/add_a_node.py](examples/add_a_node.py):
 
 ````py
 
 from pathlib import Path
 
 from comfy_catapult.comfy_schema import (APIWorkflow, APIWorkflowNodeInfo,
                                          APIWorkflowNodeMeta)
@@ -379,111 +425,160 @@
     class_type='LoadImage',
     _meta=APIWorkflowNodeMeta(title='My Loader Title'))
 
 print(api_workflow.model_dump_json())
 
 ````
 
-## Requirements
+### CLI
+
+<!---->
+<img src="README.help.generated.svg" alt="Output of `python -m comfy_catapult.cli --help`" />
+<!---->
+
+## ✅ Requirements
 
 - Python 3.10+
 - ComfyUI server with API endpoint enabled.
 
 ### Known to work on
 
-- **Python 3.10.0**, WSL2/Windows11, Ubuntu 22.04.2 LTS
-- **Python 3.10.0**, Ubuntu 22.04
+- WSL2/Windows11, Ubuntu 22.04.2 LTS: **Python
+  3.10.0**.
+- Ubuntu 20.04, Python `3.10.0`, tested in GitHub Actions
+  workflow ([./.github/workflows/build-and-test.yml](./.github/workflows/build-and-test.yml)).
 
-## Limitations
+## 🚸 Limitations
 
-- ETA estimator isn't working
+- Interrupting a job will interrupt any job, not the specific job interrupted.
+  See [#5](https://github.com/realazthat/comfy-catapult/issues/5).
 
 ## TODO
 
 - [ ] Helpers should support remote/cloud storage for ComfyUI input/output/model
       directories (Currently only supports local paths).
 - [ ] ETA Estimator.
 - [ ] Make sure the schema can parse the formats even if the format adds new
       fields.
 
 ## Contributions
 
 ### Development environment: Linux-like
 
 - For running `pre.sh` (Linux-like environment).
+
+  - From [./.github/dependencies.yml](./.github/dependencies.yml), which is used for
+    the GH Action to do a fresh install of everything:
+
+    ```yaml
+    bash: scripts.
+    findutils: scripts.
+    grep: tests.
+    xxd: tests.
+    git: scripts, tests.
+    xxhash: scripts (changeguard).
+    rsync: out-of-directory test.
+    jq: dependency for [yq](https://github.com/kislyuk/yq), which is used to generate
+      the README; the README generator needs to use `tomlq` (which is a part of `yq`)
+      to query `pyproject.toml`.
+    
+    ```
+
   - Requires `pyenv`, or an exact matching version of python as in
-    [`.python-version`](./.python-version).
+    [./.python-version](./.python-version).
   - `jq`, ([installation](https://jqlang.github.io/jq/)) required for
     [yq](https://github.com/kislyuk/yq), which is itself required for our
-    `README.md` generation, which uses `tomlq` (from the
+    `./README.md` generation, which uses `tomlq` (from the
     [yq](https://github.com/kislyuk/yq) package) to include version strings from
-    `pyproject.toml`.
-  - `bash`, `grep`, `awk`, `sed` `xxd`, `git`, `xxhash` (for tests/workflows).
-  - Requires nodejs (for act).
-  - Requires Go (to run act).
-  - docker (for act).
+    [./pyproject.toml](./pyproject.toml).
+  - act (to run the GH Action locally):
+    - Requires nodejs.
+    - Requires Go.
+    - docker.
+  - Generate animation:
+    - docker
 
 ### Commit Process
 
 1. (Optionally) Fork the `develop` branch.
 2. Stage your files: `git add path/to/file.py`.
 3. `bash scripts/pre.sh`, this will format, lint, and test the code.
-4. `git status` check if anything changed (generated `README.md` for
-   example), if so, `git add` the changes, and go back to the previous step.
+4. `git status` check if anything changed (generated `./README.md`
+   for example), if so, `git add` the changes, and go back to the previous step.
 5. `git commit -m "..."`.
 6. Make a PR to `develop` (or push to develop if you have the rights).
 
 ## Release Process
 
 These instructions are for maintainers of the project.
 
-1. `develop` branch: Run `bash scripts/pre.sh` to ensure everything
-   is in order.
-2. `develop` branch: Bump the version in `pyproject.toml`, following
-   semantic versioning principles. Also modify the `last_unstable_release` and
-   `last_stable_release` in the `[tool.comfy-catapult-project-metadata]` table
-   as appropriate.
+1. `develop` branch: Run `bash ./scripts/pre.sh` to ensure
+   everything is in order.
+2. `develop` branch: Bump the version in
+   [./pyproject.toml](./pyproject.toml), following semantic versioning
+   principles. Also modify the `last_release` and `last_stable_release` in the
+   `[tool.comfy_catapult-project-metadata]` table as appropriate.
 3. `develop` branch: Commit these changes with a message like "Prepare release
    X.Y.Z". (See the contributions section [above](#commit-process)).
 4. `master` branch: Merge the `develop` branch into the `master` branch:
    `git checkout master && git merge develop --no-ff`.
 5. `master` branch: Tag the release: Create a git tag for the release with
    `git tag -a vX.Y.Z -m "Version X.Y.Z"`.
 6. Publish to PyPI: Publish the release to PyPI with
-   `bash scripts/deploy-to-pypi.sh`.
+   `bash ./scripts/deploy-to-pypi.sh`.
 7. Push to GitHub: Push the commit and tags to GitHub with `git push` and
    `git push --tags`.
 8. `git checkout develop && git merge master` The `--no-ff` option adds a commit
    to the master branch for the merge, so refork the develop branch from the
    master branch.
+9. `git push origin develop` Push the develop branch to GitHub.
 
 [1]:
-  https://github.com/realazthat/comfy-catapult/actions/workflows/build-and-test.yml/badge.svg?branch=master
+  https://img.shields.io/github/actions/workflow/status/realazthat/comfy-catapult/build-and-test.yml?branch=master&style=plastic
 [2]:
   https://github.com/realazthat/comfy-catapult/actions/workflows/build-and-test.yml
 [3]:
-  https://github.com/realazthat/comfy-catapult/actions/workflows/build-and-test.yml/badge.svg?branch=develop
+  https://img.shields.io/github/actions/workflow/status/realazthat/comfy-catapult/build-and-test.yml?branch=develop&style=plastic
 [4]:
   https://github.com/realazthat/comfy-catapult/actions/workflows/build-and-test.yml
 [5]: https://github.com/andreyryabtsev/comfyui-python-api
 [6]: https://github.com/BennyKok/comfyui-deploy
 [7]: https://github.com/pydn/ComfyUI-to-Python-Extension
 [8]: https://github.com/Chaoses-Ib/ComfyScript
 [9]: https://pypi.org/project/hordelib/
 [10]: https://github.com/nathannlu/comfyui-cloud
-[11]: https://img.shields.io/github/license/realazthat/comfy-catapult
-[12]: https://img.shields.io/pypi/v/comfy-catapult
-[13]: https://pypi.org/project/comfy-catapult/
+[11]:
+  https://img.shields.io/github/license/realazthat/comfy-catapult?style=plastic&color=0A1E1E
+[12]:
+  https://img.shields.io/pypi/v/comfy_catapult?style=plastic&color=0A1E1E
+[13]: https://pypi.org/project/comfy_catapult/
 [14]:
-  https://img.shields.io/github/commits-since/realazthat/comfy-catapult/v2.0.0/master
+  https://img.shields.io/github/commits-since/realazthat/comfy-catapult/v2.2.0/master?style=plastic&color=0A1E1E
 [15]:
-  https://img.shields.io/github/commits-since/realazthat/comfy-catapult/v2.0.0/develop
-[16]: https://img.shields.io/github/last-commit/realazthat/comfy-catapult/master
+  https://img.shields.io/github/commits-since/realazthat/comfy-catapult/v2.2.0/develop?style=plastic&color=0A1E1E
+[16]:
+  https://img.shields.io/github/last-commit/realazthat/comfy-catapult/master?style=plastic&color=0A1E1E
 [17]:
-  https://img.shields.io/github/last-commit/realazthat/comfy-catapult/develop
-[18]: https://img.shields.io/pypi/pyversions/comfy-catapult
+  https://img.shields.io/github/last-commit/realazthat/comfy-catapult/develop?style=plastic&color=0A1E1E
+[18]:
+  https://img.shields.io/pypi/pyversions/comfy_catapult?style=plastic&color=0A1E1E
 [19]:
-  https://img.shields.io/github/languages/top/realazthat/comfy-catapult.svg?&cacheSeconds=28800
+  https://img.shields.io/github/languages/top/realazthat/comfy-catapult.svg?style=plastic&color=0A1E1E&cacheSeconds=28800
 [20]:
-  https://github.com/realazthat/comfy-catapult/compare/v2.0.0...master
+  https://github.com/realazthat/comfy-catapult/compare/v2.2.0...master
 [21]:
-  https://github.com/realazthat/comfy-catapult/compare/v2.0.0...develop
+  https://github.com/realazthat/comfy-catapult/compare/v2.2.0...develop
+[22]: https://github.com/piyushK52/comfy_runner
+[23]: https://github.com/thecooltechguy/ComfyUI-ComfyRun
+[24]: .github/logo-exported.svg
+[25]:
+  https://img.shields.io/badge/Audience-Developers-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
+[26]:
+  https://img.shields.io/badge/Platform-Linux-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLWxhcHRvcC1taW5pbWFsIj48cmVjdCB3aWR0aD0iMTgiIGhlaWdodD0iMTIiIHg9IjMiIHk9IjQiIHJ4PSIyIiByeT0iMiIvPjxsaW5lIHgxPSIyIiB4Mj0iMjIiIHkxPSIyMCIgeTI9IjIwIi8+PC9zdmc+
+[27]: https://github.com/realazthat/comfy-catapult/tree/master
+[28]: https://github.com/realazthat/comfy-catapult/tree/develop
+[29]: https://github.com/city96/ComfyUI_NetDist
+[30]: https://github.com/matan1905/ComfyUI-Serving-Toolkit
+[31]: https://github.com/rvion/CushyStudio
+[32]:
+  https://github.com/comfyanonymous/ComfyUI/tree/89d0e9abeb31e44cccef46537cd10d8812130ef3/script_examples
+  "Permalink"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `comfy_catapult-2.0.0/comfy_catapult/api_client.py` & `comfy_catapult-2.2.0/comfy_catapult/api_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,45 +5,45 @@
 # under the MIT license or a compatible open source license. See LICENSE.md for
 # the license text.
 
 import base64
 import json
 import logging
 import textwrap
-from typing import Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, List, Optional, Type, TypeVar, Union
 from urllib.parse import urlencode, urlparse
 
 import aiohttp
 from anyio import Path
 from pydantic import BaseModel
 
-from comfy_catapult.api_client_base import ComfyAPIClientBase
-from comfy_catapult.comfy_schema import (APIHistory, APIObjectInfo,
-                                         APIQueueInfo, APISystemStats,
-                                         APIUploadImageResp, APIWorkflowTicket,
-                                         ClientID, PromptID)
-from comfy_catapult.comfy_utils import TryParseAsModel, WatchVar, YamlDump
-from comfy_catapult.url_utils import JoinToBaseURL
+from .api_client_base import ComfyAPIClientBase
+from .comfy_schema import (APIHistory, APIObjectInfo, APIQueueInfo,
+                           APISystemStats, APIUploadImageResp,
+                           APIWorkflowTicket, ClientID, PromptID)
+from .comfy_utils import TryParseAsModel, WatchVar, YamlDump
+from .url_utils import JoinToBaseURL
 
 logger = logging.getLogger(__name__)
 
 T = TypeVar('T')
 
 
-async def _TryGetContent(*, resp: aiohttp.ClientResponse) -> str | Exception:
+async def _TryGetContent(*,
+                         resp: aiohttp.ClientResponse) -> Union[str, Exception]:
   try:
     return await resp.text(errors='replace')
   except Exception as e:
     logger.exception('Error getting content', exc_info=e, stack_info=True)
     return e
 
 
 async def _RaiseForStatus(*,
                           resp: aiohttp.ClientResponse,
-                          extra: Any | None = None):
+                          extra: Optional[Any] = None):
   """Same as raise_for_status(), but also dumps any content in the response into the exception"""
   try:
     resp.raise_for_status()
   except aiohttp.ClientResponseError as e:
     content_or_exc = await _TryGetContent(resp=resp)
 
     message = e.message
@@ -74,15 +74,15 @@
     ) from e
 
 
 async def _TryParseRespAsJson(*, resp: aiohttp.ClientResponse,
                               json_type: Type[T]) -> T:
   content_bytes = b''
   content_str: str = ''
-  content: T | None = None
+  content: Optional[T] = None
   try:
     content_bytes = await resp.content.read()
     content_str = content_bytes.decode('utf-8')
     if resp.content_type != 'application/json':
       raise Exception(
           f'Error: {resp.status} {resp.reason}'
           f'\n\nExpected content-type: application/json, got {resp.content_type}'
@@ -103,27 +103,27 @@
 
 
 _BaseModelT = TypeVar('_BaseModelT', bound=BaseModel)
 
 
 async def _TryParseRespAsModel(
     *, resp: aiohttp.ClientResponse, model_type: Type[_BaseModelT],
-    errors_dump_directory: Path | None) -> _BaseModelT:
+    errors_dump_directory: Optional[Path]) -> _BaseModelT:
   content: Any = await _TryParseRespAsJson(resp=resp, json_type=dict)
   return await TryParseAsModel(content=content,
                                model_type=model_type,
                                errors_dump_directory=errors_dump_directory)
 
 
 class ComfyAPIClient(ComfyAPIClientBase):
 
   def __init__(self,
                comfy_api_url: str,
                *,
-               errors_dump_directory: Path | None = None):
+               errors_dump_directory: Optional[Path] = None):
     self._comfy_api_url = comfy_api_url
     self._session = aiohttp.ClientSession()
     self._errors_dump_directory = errors_dump_directory
 
   async def __aenter__(self):
     await self._session.__aenter__()
     return self
@@ -173,18 +173,18 @@
     with WatchVar(url=url.geturl()):
       async with self._session.get(url.geturl()) as resp:
         return await _TryParseRespAsJson(resp=resp, json_type=dict)
 
   async def PostPromptRaw(self,
                           *,
                           prompt_workflow: dict,
-                          number: int | None = None,
-                          client_id: ClientID | None = None,
-                          prompt_id: PromptID | None = None,
-                          extra_data: dict | None = None) -> dict:
+                          number: Optional[int] = None,
+                          client_id: Optional[ClientID] = None,
+                          prompt_id: Optional[PromptID] = None,
+                          extra_data: Optional[dict] = None) -> dict:
     body: Dict[str, Any] = {'prompt': prompt_workflow}
 
     if number is not None:
       body['number'] = number
     if client_id is not None:
       body['client_id'] = client_id
     if prompt_id is not None:
@@ -197,46 +197,46 @@
     with WatchVar(url=url.geturl()):
       async with self._session.post(url.geturl(), data=data) as resp:
         return await _TryParseRespAsJson(resp=resp, json_type=dict)
 
   async def PostPrompt(self,
                        *,
                        prompt_workflow: dict,
-                       number: int | None = None,
-                       client_id: ClientID | None = None,
-                       prompt_id: PromptID | None = None,
-                       extra_data: dict | None = None) -> APIWorkflowTicket:
+                       number: Optional[int] = None,
+                       client_id: Optional[ClientID] = None,
+                       prompt_id: Optional[PromptID] = None,
+                       extra_data: Optional[dict] = None) -> APIWorkflowTicket:
     ticket = await self.PostPromptRaw(prompt_workflow=prompt_workflow,
                                       number=number,
                                       client_id=client_id,
                                       prompt_id=prompt_id,
                                       extra_data=extra_data)
     return await TryParseAsModel(
         content=ticket,
         model_type=APIWorkflowTicket,
         errors_dump_directory=self._errors_dump_directory)
 
   async def GetHistoryRaw(self,
                           *,
-                          prompt_id: PromptID | None = None,
-                          max_items: int | None = None) -> dict:
+                          prompt_id: Optional[PromptID] = None,
+                          max_items: Optional[int] = None) -> dict:
     url = urlparse(JoinToBaseURL(self._comfy_api_url, 'history'))
     if max_items is not None:
       url = url._replace(query=f'max_items={max_items}')
     if prompt_id is not None:
       url = url._replace(path=f'{url.path}/{prompt_id}')
 
     with WatchVar(url=url.geturl()):
       async with self._session.get(url.geturl()) as resp:
         return await _TryParseRespAsJson(resp=resp, json_type=dict)
 
   async def GetHistory(self,
                        *,
-                       prompt_id: PromptID | None = None,
-                       max_items: int | None = None) -> APIHistory:
+                       prompt_id: Optional[PromptID] = None,
+                       max_items: Optional[int] = None) -> APIHistory:
     history = await self.GetHistoryRaw(prompt_id=prompt_id, max_items=max_items)
     return await TryParseAsModel(
         content=history,
         model_type=APIHistory,
         errors_dump_directory=self._errors_dump_directory)
 
   async def GetQueueRaw(self) -> dict:
```

### Comparing `comfy_catapult-2.0.0/comfy_catapult/api_client_base.py` & `comfy_catapult-2.2.0/comfy_catapult/api_client_base.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 # SPDX-License-Identifier: MIT
 #
 # The Comfy Catapult project requires contributions made to this file be licensed
 # under the MIT license or a compatible open source license. See LICENSE.md for
 # the license text.
 
 from abc import ABC, abstractmethod
-from typing import List
+from typing import List, Optional
 
-from comfy_catapult.comfy_schema import (APIHistory, APIObjectInfo,
-                                         APIQueueInfo, APISystemStats,
-                                         APIUploadImageResp, APIWorkflowTicket,
-                                         ClientID, PromptID)
+from .comfy_schema import (APIHistory, APIObjectInfo, APIQueueInfo,
+                           APISystemStats, APIUploadImageResp,
+                           APIWorkflowTicket, ClientID, PromptID)
 
 
 class ComfyAPIClientBase(ABC):
 
   @abstractmethod
   async def __aenter__(self):
     raise NotImplementedError()
@@ -72,82 +71,90 @@
   async def GetPromptRaw(self) -> dict:
     raise NotImplementedError()
 
   @abstractmethod
   async def PostPromptRaw(self,
                           *,
                           prompt_workflow: dict,
-                          number: int | None = None,
-                          client_id: ClientID | None = None,
-                          prompt_id: PromptID | None = None,
-                          extra_data: dict | None = None) -> dict:
+                          number: Optional[int] = None,
+                          client_id: Optional[ClientID] = None,
+                          prompt_id: Optional[PromptID] = None,
+                          extra_data: Optional[dict] = None) -> dict:
     """See `ComfyUI/server.py` `@routes.post("/prompt")`.
 
     Args:
         prompt_workflow (dict): The API workflow, you can generate this with
           the ComfyUI web interface, as explained in `README.md`:
           1. Open settings (gear box in the corner).
-          2. Enable the ability to export in the API format, `Enable Dev mode Options`.
+          2. Enable the ability to export in the API format,
+            `Enable Dev mode Options`.
           3. Click new menu item `Save (API format)`.
-        prompt_id (PromptID | None): If you want to set the prompt id. If you
-          leave this empty, the server will generate a prompt id for you.
         number (int, optional): Where to insert into the queue. -1 means to
           insert to the front of the queue. Default is None, which uses the
           default on the server, which is also equivalent to -1.
-        client_id (ClientID | None, optional): _description_. Defaults to None.
+        client_id (ClientID | None): If you want to set the client id. ComfyUI
+          will use this to resume connections, and filter out websockets events
+          and similar etc. If you leave this empty, the server will generate a
+          client id for you.
+        prompt_id (PromptID | None): If you want to set the prompt id. If you
+          leave this empty, the server will generate a prompt id for you.
         extra_data (dict | None, optional): Extra data associated with the
           prompt/job. Defaults to None.
 
     Returns:
         dict: The json response.
     """
     raise NotImplementedError()
 
   @abstractmethod
   async def PostPrompt(self,
                        *,
                        prompt_workflow: dict,
-                       number: int | None = None,
-                       client_id: ClientID | None = None,
-                       prompt_id: PromptID | None = None,
-                       extra_data: dict | None = None) -> APIWorkflowTicket:
+                       number: Optional[int] = None,
+                       client_id: Optional[ClientID] = None,
+                       prompt_id: Optional[PromptID] = None,
+                       extra_data: Optional[dict] = None) -> APIWorkflowTicket:
     """See `ComfyUI/server.py` `@routes.post("/prompt")`.
 
     Args:
         prompt_workflow (dict): The API workflow, you can generate this with
           the ComfyUI web interface, as explained in `README.md`:
           1. Open settings (gear box in the corner).
-          2. Enable the ability to export in the API format, `Enable Dev mode Options`.
+          2. Enable the ability to export in the API format,
+            `Enable Dev mode Options`.
           3. Click new menu item `Save (API format)`.
-        prompt_id (PromptID | None): If you want to set the prompt id. If you
-          leave this empty, the server will generate a prompt id for you.
         number (int, optional): Where to insert into the queue. -1 means to
           insert to the front of the queue. Default is None, which uses the
           default on the server, which is also equivalent to -1.
-        client_id (ClientID | None, optional): _description_. Defaults to None.
+        client_id (ClientID | None): If you want to set the client id. ComfyUI
+          will use this to resume connections, and filter out websockets events
+          and similar etc. If you leave this empty, the server will generate a
+          client id for you.
+        prompt_id (PromptID | None): If you want to set the prompt id. If you
+          leave this empty, the server will generate a prompt id for you.
         extra_data (dict | None, optional): Extra data associated with the
           prompt/job. Defaults to None.
 
     Returns:
         APIWorkflowTicket: The response parsed into a pydantic model.
     """
     raise NotImplementedError()
 
   @abstractmethod
   async def GetHistoryRaw(self,
                           *,
-                          prompt_id: PromptID | None = None,
-                          max_items: int | None = None) -> dict:
+                          prompt_id: Optional[PromptID] = None,
+                          max_items: Optional[int] = None) -> dict:
     raise NotImplementedError()
 
   @abstractmethod
   async def GetHistory(self,
                        *,
-                       prompt_id: PromptID | None = None,
-                       max_items: int | None = None) -> APIHistory:
+                       prompt_id: Optional[PromptID] = None,
+                       max_items: Optional[int] = None) -> APIHistory:
     raise NotImplementedError()
 
   @abstractmethod
   async def GetQueueRaw(self) -> dict:
     raise NotImplementedError()
 
   @abstractmethod
```

### Comparing `comfy_catapult-2.0.0/comfy_catapult/catapult.py` & `comfy_catapult-2.2.0/comfy_catapult/catapult.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,69 +13,69 @@
 import textwrap
 import threading
 import traceback as tb
 import uuid
 from copy import deepcopy
 from dataclasses import dataclass
 from pprint import pformat
-from typing import Any, Dict, Generic, List, Sequence, Tuple, TypeVar
+from typing import Any, Dict, Generic, List, Optional, Sequence, Tuple, TypeVar
 from urllib.parse import ParseResult, urlparse
 
 import aiofiles
 from anyio import Path
 from slugify import slugify
 from websockets import WebSocketClientProtocol, connect
 
-from comfy_catapult.api_client import ComfyAPIClientBase, YamlDump
-from comfy_catapult.catapult_base import ComfyCatapultBase, JobStatus, Progress
-from comfy_catapult.comfy_schema import (APIHistory, APIHistoryEntry,
-                                         APIHistoryEntryStatusNote, APINodeID,
-                                         APIQueueInfo, APISystemStats,
-                                         APIWorkflowTicket, WSMessage)
-from comfy_catapult.comfy_utils import TryParseAsModel
-from comfy_catapult.errors import NodesNotExecuted, WorkflowSubmissionError
+from .api_client import ComfyAPIClientBase
+from .catapult_base import (ComfyCatapultBase, ExceptionInfo, JobStatus,
+                            Progress)
+from .comfy_schema import (APIHistory, APIHistoryEntry,
+                           APIHistoryEntryStatusNote, APINodeID, APIQueueInfo,
+                           APISystemStats, APIWorkflowTicket, WSMessage)
+from .comfy_utils import TryParseAsModel, YamlDump
+from .errors import JobFailed, NodesNotExecuted, WorkflowSubmissionError
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class _Job:
 
   class RemoteStatus(enum.Enum):
     NONE = enum.auto()
     PENDING_OR_RUNNING = enum.auto()
 
   job_id: str
   prepared_workflow: dict
   important_nodes: Tuple[APINodeID, ...]
-  ticket: APIWorkflowTicket | None
+  ticket: Optional[APIWorkflowTicket]
   status: JobStatus
   # Exceptions that should be in status but aren't because they're not pickable
   # or deepcopyable.
   errors: List[Exception]
-  future: asyncio.Future[dict]
+  future: 'asyncio.Future[dict]'
   remote_job_status: RemoteStatus
-  job_debug_path: Path | None
+  job_debug_path: Optional[Path]
 
 
 T = TypeVar('T')
 
 
 @dataclass
 class _Guess(Generic[T]):
-  value: T | None
+  value: Optional[T]
   updated: datetime.datetime
 
 
 class ComfyCatapult(ComfyCatapultBase):
 
   def __init__(self,
                comfy_client: ComfyAPIClientBase,
                *,
-               debug_path: Path | None,
+               debug_path: Optional[Path],
                debug_save_all: bool = False):
     """_summary_
 
     Args:
         comfy_client (ComfyAPIClientBase): _description_
         debug_path (Path | None): For logging of certain debug information, in
           case of errors.
@@ -142,15 +142,15 @@
 
   async def Catapult(
       self,
       *,
       job_id: str,
       prepared_workflow: dict,
       important: Sequence[APINodeID],
-      job_debug_path: Path | None = None,
+      job_debug_path: Optional[Path] = None,
   ) -> dict:
     async with self._lock:
       if job_id in self._jobs:
         raise KeyError(f'User job id {repr(job_id)} already exists')
       if not slugify(job_id) == job_id:
         raise ValueError(
             f'User job id {repr(job_id)} is not slugified (e.g {repr(slugify(job_id))})'
@@ -158,28 +158,29 @@
       if job_debug_path is None and self._debug_path is not None:
         dt = datetime.datetime.now(datetime.timezone.utc).isoformat()
         job_debug_path = self._debug_path / f'{slugify(dt)}-{slugify(job_id)}'
 
     if job_debug_path is not None:
       await job_debug_path.mkdir(parents=True, exist_ok=True)
 
+    future: asyncio.Future[dict] = asyncio.Future()
     async with self._lock:
-      future = asyncio.Future()
       self._jobs[job_id] = _Job(
           job_id=job_id,
           prepared_workflow=prepared_workflow,
           important_nodes=tuple(important),
           ticket=None,
           future=future,
           status=JobStatus(scheduled=self._Now(),
                            running=None,
                            pending=None,
                            success=None,
                            errored=None,
-                           cancelled=None),
+                           cancelled=None,
+                           errors=[]),
           errors=[],
           remote_job_status=_Job.RemoteStatus.PENDING_OR_RUNNING,
           job_debug_path=job_debug_path)
 
     async with _JobContext(job_id=job_id, comfy=self):
       ticket: APIWorkflowTicket = await self._comfy_client.PostPrompt(
           prompt_workflow=prepared_workflow)
@@ -207,15 +208,15 @@
 
       if ticket.prompt_id is None:
         raise AssertionError(
             'ticket.prompt_id is None, should be impossible here')
       return await future
 
   async def GetStatus(self, *,
-                      job_id: str) -> Tuple[JobStatus, asyncio.Future[dict]]:
+                      job_id: str) -> 'Tuple[JobStatus, asyncio.Future[dict]]':
     async with self._lock:
       if job_id not in self._jobs:
         raise KeyError(f'Job id {repr(job_id)} not found')
       job = self._jobs[job_id]
       return deepcopy(job.status), job.future
 
   async def GetExceptions(self, *, job_id: str) -> List[Exception]:
@@ -224,16 +225,16 @@
         raise KeyError(f'Job id {repr(job_id)} not found')
       job = self._jobs[job_id]
       return list(job.errors)
 
   async def CancelJob(self, *, job_id: str):
     async with _JobContext(job_id=job_id, comfy=self):
       async with self._lock:
-        ticket: APIWorkflowTicket | None = self._jobs[job_id].ticket
-        prompt_id: str | None = None
+        ticket: Optional[APIWorkflowTicket] = self._jobs[job_id].ticket
+        prompt_id: Optional[str] = None
         if ticket is not None:
           prompt_id = ticket.prompt_id
         remote_job_status = self._jobs[job_id].remote_job_status
 
       if remote_job_status == _Job.RemoteStatus.PENDING_OR_RUNNING \
           and prompt_id is not None:
         # TODO(realazthat/comfy-catapult#5): We don't know for sure that the
@@ -255,32 +256,34 @@
   async def _ReceivedJobHistory(self, *, job_id: str, history: APIHistory,
                                 job_context: '_JobContext'):
     if not isinstance(history, APIHistory):
       raise AssertionError(f'history must be APIHistory, not {type(history)}')
 
     async with self._lock:
       prepared_workflow: dict = deepcopy(self._jobs[job_id].prepared_workflow)
-      ticket: APIWorkflowTicket | None = deepcopy(self._jobs[job_id].ticket)
-      prompt_id: str | None = None
+      ticket: Optional[APIWorkflowTicket] = deepcopy(self._jobs[job_id].ticket)
+      prompt_id: Optional[str] = None
       if ticket is not None:
         prompt_id = ticket.prompt_id
       important_nodes = deepcopy(self._jobs[job_id].important_nodes)
 
     if len(history.root) == 0:
       return
     if prompt_id not in history.root:
       raise AssertionError(f'prompt_id {repr(prompt_id)} not in history.root')
+    if not isinstance(prompt_id, str):
+      raise AssertionError(f'prompt_id must be str, not {type(prompt_id)}')
     job_history: APIHistoryEntry = history.root[prompt_id]
     async with self._lock:
       self._jobs[job_id].status = self._jobs[job_id].status._replace(
-          job_history=job_history)
+          job_history=job_history.model_dump())
 
     ##########################################################################
     # Get outputs_to_execute, outputs_with_data, extra_data
-    extra_data: dict | None = None
+    extra_data: Optional[dict] = None
     outputs_to_execute: List[APINodeID] = []
     outputs_with_data: List[APINodeID] = []
     if job_history.outputs is not None:
       outputs_with_data = list(job_history.outputs.keys())
     if job_history.prompt is not None:
       if job_history.prompt.extra_data is not None:
         extra_data = job_history.prompt.extra_data
@@ -294,15 +297,15 @@
         if job_history.status.messages is not None:
           note: APIHistoryEntryStatusNote
           for note in job_history.status.messages:
             notes.append(textwrap.indent(pformat(note._asdict()), prefix='  '))
         # TODO: Turn all Exception into a subclass of Exception.
         # TODO: Make all exceptions going forward contain the metadata that
         # NodesNotExecuted does.
-        raise Exception('Job has failed'
+        raise JobFailed('Job has failed'
                         f'\n  status: {repr(job_history.status)}'
                         f'\n  notes:' + '\n'.join(notes))
 
     ##########################################################################
     logger.debug('job_history.prompt.extra_data.model_dump(): %s',
                  YamlDump(extra_data))
     logger.debug('job_history.prompt.outputs_to_execute.model_dump(): %s',
@@ -312,20 +315,20 @@
     logger.debug('outputs_that_executed: %s', YamlDump(outputs_with_data))
 
     bad_dataless_outputs = [
         node_id for node_id in outputs_to_execute
         if node_id not in outputs_with_data
     ]
 
-    def _GetTitles(node_ids: List[APINodeID]) -> List[str | None]:
+    def _GetTitles(node_ids: List[APINodeID]) -> List[Optional[str]]:
       titles = []
       for node_id in node_ids:
         node_info: dict = prepared_workflow.get(node_id, {})
         meta: dict = node_info.get('_meta', {})
-        title: str | None = meta.get('title', None)
+        title: Optional[str] = meta.get('title', None)
         titles.append(title)
       return titles
 
     if len(bad_dataless_outputs) > 0:
       logger.error('bad_dataless_outputs: %s', YamlDump(bad_dataless_outputs))
       logger.error('_GetTitles(bad_dataless_outputs): %s',
                    YamlDump(_GetTitles(bad_dataless_outputs)))
@@ -353,35 +356,69 @@
   async def _GetJobIDs(self) -> List[str]:
     async with self._lock:
       return list(self._jobs.keys())
 
   async def _Poll(self):
     ############################################################################
     await self._CheckError()
+    await self._PollFutures()
+    ############################################################################
+    await self._PollSystemStats()
+    ############################################################################
+    prompt_id_2_status: Dict[str, str] = {}
+    await self._PollQueue(prompt_id_2_status)
+
+    ############################################################################
+    prompt_info: dict = await self._comfy_client.GetPromptRaw()
+
+    exec_info = prompt_info['exec_info']
+    queue_remaining = exec_info['queue_remaining']
+    if not isinstance(queue_remaining, int):
+      raise AssertionError(
+          f'queue_remaining must be int, not {type(queue_remaining)}')
+    logger.info('queue_remaining: %s', queue_remaining)
+    ############################################################################
+    # Check the /history endpoint to see if there are any updates on our jobs.
+    await self._PollHistory(prompt_id_2_status=prompt_id_2_status)
+
+  async def _PollFutures(self):
     ############################################################################
     # Make sure any hanging future that is done matches the job status.
     done_futures_jobs: List[str] = []
     async with self._lock:
+      job_id: str
+      job: _Job
       for job_id, job in self._jobs.items():
         if job.future.done() and not job.status.IsDone():
           done_futures_jobs.append(job_id)
     for job_id in done_futures_jobs:
       async with _JobContext(job_id=job_id, comfy=self):
         async with self._lock:
           job = self._jobs[job_id]
           # See if an error occurred.
           job.future.result()
           job.status = job.status._replace(success=self._Now())
-    ############################################################################
+
+  async def _PollSystemStats(self):
     system_stats: APISystemStats = await self._comfy_client.GetSystemStats()
     logger.info('system_stats: %s', YamlDump(system_stats.model_dump()))
-    ############################################################################
+    for job_id in await self._GetJobIDs():
+      async with _JobContext(job_id=job_id, comfy=self):
+        async with self._lock:
+          job = self._jobs[job_id]
+          if job.status.IsDone():
+            continue
+          if job.status.system_stats_check is None:
+            job.status = job.status._replace(system_stats_check=self._Now())
+
+  async def _PollQueue(self, prompt_id_2_status: Dict[str, str]):
+    """Check /queue endpoint and update job status.
+    """
     queue_info: APIQueueInfo = await self._comfy_client.GetQueue()
 
-    prompt_id_2_status: Dict[str, str] = {}
     for pending in queue_info.queue_running:
       prompt_id_2_status[pending.prompt_id] = 'running'
     for running in queue_info.queue_pending:
       prompt_id_2_status[running.prompt_id] = 'pending'
     pending_count = sum(
         [1 for status in prompt_id_2_status.values() if status == 'pending'],
         start=0)
@@ -390,116 +427,112 @@
         start=0)
 
     logger.info('pending_count: %s', pending_count)
     logger.info('running_count: %s', running_count)
 
     for prompt_id, status in prompt_id_2_status.items():
       async with self._lock:
-        job_id = self._prompt_id_index.get(prompt_id, None)
-        if job_id is None:
+        if prompt_id not in self._prompt_id_index:
           continue
-        job: _Job = self._jobs[job_id]
+        job_id = self._prompt_id_index[prompt_id]
+        async with _JobContext(job_id=job_id, comfy=self):
+          job: _Job = self._jobs[job_id]
 
-        if status == 'pending' and job.status.pending is None:
-          job.status = job.status._replace(pending=self._Now())
+          if status == 'pending' and job.status.pending is None:
+            job.status = job.status._replace(pending=self._Now())
 
-        if status == 'running' and job.status.running is None:
-          job.status = job.status._replace(running=self._Now())
-          self._guess_currently_running_job_id = _Guess(value=job_id,
-                                                        updated=self._Now())
-          self._guess_currently_running_node_id = _Guess(value=None,
-                                                         updated=self._Now())
-          self._guess_currently_running_node_progress = _Guess(
-              value=None, updated=self._Now())
+          if status == 'running' and job.status.running is None:
+            job.status = job.status._replace(running=self._Now())
+            self._guess_currently_running_job_id = _Guess(value=job_id,
+                                                          updated=self._Now())
+            self._guess_currently_running_node_id = _Guess(value=None,
+                                                           updated=self._Now())
+            self._guess_currently_running_node_progress = _Guess(
+                value=None, updated=self._Now())
+          job.status = job.status._replace(queue_check=self._Now())
 
     # TODO: Reenable this or remove it.
     # print('self._jobs:', file=sys.stderr)
     # pprint(self._jobs, indent=2, stream=sys.stderr)
 
-    ############################################################################
-    prompt_info: dict = await self._comfy_client.GetPromptRaw()
-
-    exec_info = prompt_info['exec_info']
-    queue_remaining = exec_info['queue_remaining']
-    if not isinstance(queue_remaining, int):
-      raise AssertionError(
-          f'queue_remaining must be int, not {type(queue_remaining)}')
-    logger.info('queue_remaining: %s', queue_remaining)
-    ############################################################################
-    # Check the /history endpoint to see if there are any updates on our jobs.
-
+  async def _PollHistory(self, prompt_id_2_status: Dict[str, str]):
     # Update job.remote_job_status.
     for job_id in await self._GetJobIDs():
-      async with self._lock:
-        new_remote_job_status = (_Job.RemoteStatus.NONE
-                                 if job_id not in prompt_id_2_status else
-                                 _Job.RemoteStatus.PENDING_OR_RUNNING)
-        self._jobs[job_id].remote_job_status = new_remote_job_status
+      async with _JobContext(job_id=job_id, comfy=self) as job_context:
+        async with self._lock:
+          new_remote_job_status = (_Job.RemoteStatus.NONE
+                                   if job_id not in prompt_id_2_status else
+                                   _Job.RemoteStatus.PENDING_OR_RUNNING)
+          self._jobs[job_id].remote_job_status = new_remote_job_status
 
     # Update job.job_history.
     for job_id in await self._GetJobIDs():
-      async with self._lock:
-        if job_id in prompt_id_2_status:
-          # In this case, it's pending or running, not going to be in the
-          # `/history` endpoint.
-          continue
-
-        if self._jobs[job_id].status.job_history is not None:
-          # We already have the job history.
-          continue
-
-        ticket: APIWorkflowTicket | None = self._jobs[job_id].ticket
-        prompt_id: str | None = None
-        if ticket is not None:
-          prompt_id = ticket.prompt_id
-
-        if prompt_id is None:
-          # This should never happen, but :shrug:.
-          continue
-        job_debug_path = self._jobs[job_id].job_debug_path
-        errors_dump_directory: Path | None = None
-        if job_debug_path is not None:
-          errors_dump_directory = job_debug_path / 'errors'
-
-      ##########################################################################
       async with _JobContext(job_id=job_id, comfy=self) as job_context:
+        async with self._lock:
+          if job_id in prompt_id_2_status:
+            # In this case, it's pending or running, not going to be in the
+            # `/history` endpoint.
+            continue
+
+          if self._jobs[job_id].status.job_history is not None:
+            # We already have the job history.
+            continue
+
+          ticket: Optional[APIWorkflowTicket] = self._jobs[job_id].ticket
+          prompt_id: Optional[str] = None
+          if ticket is not None:
+            prompt_id = ticket.prompt_id
+
+          if prompt_id is None:
+            # This should never happen, but :shrug:.
+            continue
+          job_debug_path = self._jobs[job_id].job_debug_path
+          errors_dump_directory: Optional[Path] = None
+          if job_debug_path is not None:
+            errors_dump_directory = job_debug_path / 'errors'
+
+        ########################################################################
         history_raw: dict = await self._comfy_client.GetHistoryRaw(
             prompt_id=prompt_id)
         await job_context.WatchVar(history_raw=history_raw)
         history: APIHistory = await TryParseAsModel(
             content=history_raw,
             model_type=APIHistory,
             errors_dump_directory=errors_dump_directory)
         await self._ReceivedJobHistory(job_id=job_id,
                                        history=history,
                                        job_context=job_context)
-      ##########################################################################
+        ########################################################################
 
   def _Now(self) -> datetime.datetime:
     return datetime.datetime.now(datetime.timezone.utc)
 
   async def _Record(self):
     async with self._lock:
       guess_currently_running_job_id = self._guess_currently_running_job_id
       # guess_currently_running_node_id = self._guess_currently_running_node_id
       # guess_currently_running_node_progress = self._guess_currently_running_node_progress
 
     if guess_currently_running_job_id.value is not None:
       pass
 
   async def _LoopWS(self, *, ws: WebSocketClientProtocol):
+    prompt_id: Optional[str]
+    node_id: Optional[str]
+    node_type: Optional[str]
+
     while True:
       try:
         logger.debug('websocket recv')
         out = await ws.recv()
         if not isinstance(out, str):
           logger.debug('websocket type(out): %s', type(out))
           continue
         logger.debug('websocket raw: %s', YamlDump(out))
-        errors_dump_directory: Path | None = None
+        errors_dump_directory: Optional[Path] = None
         async with self._lock:
           if self._debug_path is not None:
             errors_dump_directory = self._debug_path / 'errors'
 
         message = await TryParseAsModel(
             content=json.loads(out),
             model_type=WSMessage,
@@ -511,15 +544,15 @@
 
           async with self._lock:
             self._guess_currently_running_node_id = _Guess(value=last_node_id,
                                                            updated=self._Now())
           await self._Record()
         elif message.type == 'executing' and 'node' in message.data and 'prompt_id' in message.data:
           prompt_id = message.data.get('prompt_id', None)
-          node_id: str | None = message.data.get('node', None)
+          node_id = message.data.get('node', None)
           async with self._lock:
             job_id = self._prompt_id_index.get(
                 prompt_id, None) if prompt_id is not None else None
             if job_id is not None:
               job = self._jobs[job_id]
               if job.status.running is None:
                 job.status = job.status._replace(running=self._Now())
@@ -545,16 +578,16 @@
                                                            updated=self._Now())
             self._guess_currently_running_node_progress = _Guess(
                 value=None, updated=self._Now())
           await self._Record()
 
         elif message.type == 'executed' and 'node' in message.data and 'output_ui' in message.data and 'prompt_id' in message.data:
           # Finished a single node?
-          prompt_id: str | None = message.data.get('prompt_id', None)
-          node_id: str | None = message.data.get('node', None)
+          prompt_id = message.data.get('prompt_id', None)
+          node_id = message.data.get('node', None)
           # output_ui = message.data['output_ui']
           async with self._lock:
             job_id = self._prompt_id_index.get(
                 prompt_id, None) if prompt_id is not None else None
             if job_id is not None:
               job = self._jobs[job_id]
               if job.status.running is None:
@@ -566,31 +599,35 @@
                                                           updated=self._Now())
             self._guess_currently_running_node_id = _Guess(value=node_id,
                                                            updated=self._Now())
             self._guess_currently_running_node_progress = _Guess(
                 value=None, updated=self._Now())
           await self._Record()
         elif message.type in ['execution_interrupted', 'execution_error']:
-          prompt_id: str | None = message.data.get('prompt_id', None)
-          node_id: str | None = message.data.get('node_id', None)
-          node_type: str | None = message.data.get('node_type', None)
-          # executed: list | None = message.data.get('executed', None)
+          prompt_id = message.data.get('prompt_id', None)
+          node_id = message.data.get('node_id', None)
+          node_type = message.data.get('node_type', None)
+          # executed: Optional[list] = message.data.get('executed', None)
           async with self._lock:
             job_id = self._prompt_id_index.get(
                 prompt_id, None) if prompt_id is not None else None
             if job_id is not None:
               job = self._jobs[job_id]
               if not job.status.IsDone():
                 now = self._Now()
+
                 job.status = job.status._replace(
                     errored=now,
                     errors=job.status.errors + [
-                        Exception(
-                            f'Node {repr(node_id)} of type {repr(node_type)} errored: {repr(message.data)}'
-                        )
+                        ExceptionInfo(
+                            type=str(node_type),
+                            message=
+                            f'Node {repr(node_id)} of type {repr(node_type)} errored:\n{YamlDump(message.data)}',
+                            traceback='',
+                            attributes={})
                     ])
             self._guess_currently_running_job_id = _Guess(value=None,
                                                           updated=self._Now())
             self._guess_currently_running_node_id = _Guess(value=None,
                                                            updated=self._Now())
             self._guess_currently_running_node_progress = _Guess(
                 value=None, updated=self._Now())
@@ -690,15 +727,15 @@
     self._watch_vars: Dict[str, Any] = {}
 
   async def WatchVar(self, **kwargs):
     for name, value in kwargs.items():
       self._watch_vars[name] = value
     async with self._comfy._lock:
       job = self._comfy._jobs[self._job_id]
-      job_debug_path: Path | None = job.job_debug_path
+      job_debug_path: Optional[Path] = job.job_debug_path
     if job_debug_path is None:
       return
     if self._comfy._debug_save_all:
       dt = datetime.datetime.now(datetime.timezone.utc).isoformat()
       for name, value in kwargs.items():
         dump_path = job_debug_path / 'watch' / f'{slugify(dt)}-{slugify(name)}.yaml'
         await dump_path.parent.mkdir(parents=True, exist_ok=True)
@@ -714,27 +751,27 @@
         if self._job_id not in self._comfy._jobs:
           return
         job = self._comfy._jobs[self._job_id]
         if job.future is not None and not job.future.done():
           job.future.set_exception(exc_value)
         if not job.status.IsDone():
           job.errors += [exc_value]
-          exc_info = JobStatus.ExceptionInfo(
-              type=exc_type.__name__,
-              message=str(exc_value),
-              traceback=''.join(
-                  tb.format_exception(exc_type, exc_value, traceback)),
-              attributes={
-                  k: str(v)
-                  for k, v in exc_value.__dict__.items()
-              })
+          exc_info = ExceptionInfo(type=exc_type.__name__,
+                                   message=str(exc_value),
+                                   traceback=''.join(
+                                       tb.format_exception(
+                                           exc_type, exc_value, traceback)),
+                                   attributes={
+                                       k: str(v)
+                                       for k, v in exc_value.__dict__.items()
+                                   })
           job.status = job.status._replace(errored=self._comfy._Now(),
                                            errors=job.status.errors +
                                            [exc_info])
-        job_debug_path: Path | None = job.job_debug_path
+        job_debug_path: Optional[Path] = job.job_debug_path
         status = deepcopy(job.status)
         workflow = deepcopy(job.prepared_workflow)
         ticket = deepcopy(job.ticket)
         remote_job_status = deepcopy(job.remote_job_status)
 
       dt = datetime.datetime.now(datetime.timezone.utc).isoformat()
       if job_debug_path is not None:
```

### Comparing `comfy_catapult-2.0.0/comfy_catapult/catapult_base.py` & `comfy_catapult-2.2.0/comfy_catapult/catapult_base.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,47 +4,60 @@
 # The Comfy Catapult project requires contributions made to this file be licensed
 # under the MIT license or a compatible open source license. See LICENSE.md for
 # the license text.
 
 import asyncio
 import datetime
 from abc import ABC, abstractmethod
-from typing import Dict, List, NamedTuple, Sequence, Tuple
+from typing import Dict, List, NamedTuple, Optional, Sequence, Tuple
 
 from anyio import Path
+from pydantic import BaseModel, ConfigDict
 
-from comfy_catapult.comfy_schema import APINodeID
+from .comfy_schema import APINodeID
 
 
 class Progress(NamedTuple):
   value: int
   max_value: int
 
 
-class JobStatus(NamedTuple):
+class ExceptionInfo(NamedTuple):
+  type: str
+  message: str
+  traceback: str
+  attributes: Dict[str, str]
+
+
+class JobStatus(BaseModel):
+  model_config = ConfigDict(frozen=True)
+
+  scheduled: Optional[datetime.datetime]
+  pending: Optional[datetime.datetime]
+  running: Optional[datetime.datetime]
+  success: Optional[datetime.datetime]
+  errored: Optional[datetime.datetime]
+  cancelled: Optional[datetime.datetime]
+  errors: List[ExceptionInfo]
+
+  system_stats_check: Optional[datetime.datetime] = None
+  """Last time system stats were successfully checked (while this job is not done)."""
+  queue_check: Optional[datetime.datetime] = None
+  """Last time /queue/job_id was successfully checked for (while this job is not done)."""
 
-  class ExceptionInfo(NamedTuple):
-    type: str
-    message: str
-    traceback: str
-    attributes: Dict[str, str]
-
-  scheduled: datetime.datetime | None
-  pending: datetime.datetime | None
-  running: datetime.datetime | None
-  success: datetime.datetime | None
-  errored: datetime.datetime | None
-  cancelled: datetime.datetime | None
-  errors: List[ExceptionInfo] = []
-  job_history: dict | None = None
+  job_history: Optional[dict] = None
+  """The history of the job. This is only set when the job is done and the history is successfully retrieved."""
 
   def IsDone(self) -> bool:
     return (self.success is not None or self.errored is not None
             or self.cancelled is not None)
 
+  def _replace(self, **kwargs):
+    return self.copy(update=kwargs)
+
 
 class ComfyCatapultBase(ABC):
 
   @abstractmethod
   def __init__(self):
     pass
 
@@ -63,15 +76,15 @@
   @abstractmethod
   async def Catapult(
       self,
       *,
       job_id: str,
       prepared_workflow: dict,
       important: Sequence[APINodeID],
-      job_debug_path: Path | None = None,
+      job_debug_path: Optional[Path] = None,
   ) -> dict:
     """Schedule a ComfyUI workflow job.
 
     Args:
         job_id (str): A unique identifier for the job. Note: This string must
           be unique, and must be slugified! Use python-slugify to slugify the
           string.
@@ -87,15 +100,15 @@
     Returns:
         dict: The history of the job returned from the ComfyUI API.
     """
     raise NotImplementedError()
 
   @abstractmethod
   async def GetStatus(self, *,
-                      job_id: str) -> Tuple[JobStatus, asyncio.Future[dict]]:
+                      job_id: str) -> 'Tuple[JobStatus, asyncio.Future[dict]]':
     """Get the status of a job.
 
     Args:
         job_id (str): The job id.
 
     Returns:
         Tuple[JobStatus, asyncio.Future[dict]]: The status of the job, and a
```

### Comparing `comfy_catapult-2.0.0/comfy_catapult/comfy_schema.py` & `comfy_catapult-2.2.0/comfy_catapult/comfy_schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
 # SPDX-License-Identifier: MIT
 #
 # The Comfy Catapult project requires contributions made to this file be licensed
 # under the MIT license or a compatible open source license. See LICENSE.md for
 # the license text.
 
-from typing import Any, Dict, List, Literal, NamedTuple
+from typing import Any, Dict, List, Literal, NamedTuple, Optional, Union
 from urllib.parse import urljoin
 
 from pydantic import BaseModel, ConfigDict, Field, RootModel, field_validator
 from typing_extensions import Annotated
 
-EXTRA = 'allow'
+EXTRA: Union[Literal['allow', 'ignore', 'forbid'], None] = 'allow'
 
 APINodeID = Annotated[
     str,
     Field(alias='node_id', description='The ID of a node in a workflow.')]
 PromptID = Annotated[
     str,
     Field(
@@ -70,31 +70,31 @@
   """
   model_config = ConfigDict(extra=EXTRA)
   """This is a pydantic thing, to configure the model, it is not an accessible field.
 
   extra: This is just to future proof the schema so it won't break if extra
   fields are added. They'll be stored dynamically.
   """
-  title: str | None = None
+  title: Optional[str] = None
 
 
 class APIWorkflowNodeInfo(BaseModel):
   model_config = ConfigDict(populate_by_name=True, extra=EXTRA)
   """This is a pydantic thing, to configure the model, it is not an accessible field.
 
   populate_by_name: This is to allow `meta` field to be populated by `_meta` or
   `meta`.
 
   extra: This is just to future proof the schema so it won't break if extra
   fields are added. They'll be stored dynamically.
   """
 
-  inputs: Dict[str, str | int | float | bool | APIWorkflowInConnection | dict]
+  inputs: Dict[str, Union[str, int, float, bool, APIWorkflowInConnection, dict]]
   class_type: str
-  meta: APIWorkflowNodeMeta | None = Field(None, alias='_meta')
+  meta: Optional[APIWorkflowNodeMeta] = Field(None, alias='_meta')
 
 
 class APIWorkflow(RootModel[Dict[APINodeID, APIWorkflowNodeInfo]]):
   """This is the API format, you get it from `Save (API Format)` in the UI.
 
 
   See test_data/sdxlturbo_example_api.json for an example of this format in json.
@@ -107,45 +107,45 @@
   model_config = ConfigDict(extra=EXTRA)
   """This is a pydantic thing, to configure the model, it is not an accessible field.
 
   extra: This is just to future proof the schema so it won't break if extra
   fields are added. They'll be stored dynamically.
   """
 
-  os: str | None = None
-  python_version: str | None = None
-  embedded_python: bool | None = None
+  os: Optional[str] = None
+  python_version: Optional[str] = None
+  embedded_python: Optional[bool] = None
 
 
 class APISystemStatsDevice(BaseModel):
   model_config = ConfigDict(extra=EXTRA)
   """This is a pydantic thing, to configure the model, it is not an accessible field.
 
   extra: This is just to future proof the schema so it won't break if extra
   fields are added. They'll be stored dynamically.
   """
-  name: str | None = None
-  type: str | None = None
-  index: int | None = None
-  vram_total: int | None = None
-  vram_free: int | None = None
-  torch_vram_total: int | None = None
-  torch_vram_free: int | None = None
+  name: Optional[str] = None
+  type: Optional[str] = None
+  index: Optional[int] = None
+  vram_total: Optional[int] = None
+  vram_free: Optional[int] = None
+  torch_vram_total: Optional[int] = None
+  torch_vram_free: Optional[int] = None
 
 
 class APISystemStats(BaseModel):
   """Returned from /system_stats endpoint."""
   model_config = ConfigDict(extra=EXTRA)
   """This is a pydantic thing, to configure the model, it is not an accessible field.
 
   extra: This is just to future proof the schema so it won't break if extra
   fields are added. They'll be stored dynamically.
   """
-  system: APISystemStatsSystem | None = None
-  devices: List[APISystemStatsDevice] | None = None
+  system: Optional[APISystemStatsSystem] = None
+  devices: Optional[List[APISystemStatsDevice]] = None
 
 
 ################################################################################
 class APIQueueInfoEntry(NamedTuple):
   number: int
   prompt_id: PromptID
   prompt: APIWorkflow
@@ -196,18 +196,18 @@
   """Return from post /prompt endpoint."""
   model_config = ConfigDict(extra=EXTRA)
   """This is a pydantic thing, to configure the model, it is not an accessible field.
 
   extra: This is just to future proof the schema so it won't break if extra
   fields are added. They'll be stored dynamically.
   """
-  node_errors: Dict[APINodeID, NodeErrors] | None = None
-  number: int | None = None
-  prompt_id: PromptID | None = None
-  error: str | None = None
+  node_errors: Optional[Dict[APINodeID, NodeErrors]] = None
+  number: Optional[int] = None
+  prompt_id: Optional[PromptID] = None
+  error: Union[NodeErrorInfo, str, None] = None
 
 
 ################################################################################
 
 
 class APIOutputUI(RootModel[Dict[OutputName, List[Any]]]):
   root: Dict[OutputName, List[Any]]
@@ -239,29 +239,29 @@
   """
   model_config = ConfigDict(extra=EXTRA)
   """This is a pydantic thing, to configure the model, it is not an accessible field.
 
   extra: This is just to future proof the schema so it won't break if extra
   fields are added. They'll be stored dynamically.
   """
-  status_str: str | None = None
-  completed: bool | None = None
-  messages: List[APIHistoryEntryStatusNote] | None = None
+  status_str: Optional[str] = None
+  completed: Optional[bool] = None
+  messages: Optional[List[APIHistoryEntryStatusNote]] = None
 
 
 class APIHistoryEntry(BaseModel):
   model_config = ConfigDict(extra=EXTRA)
   """This is a pydantic thing, to configure the model, it is not an accessible field.
 
   extra: This is just to future proof the schema so it won't break if extra
   fields are added. They'll be stored dynamically.
   """
-  outputs: Dict[APINodeID, APIOutputUI] | None = None
-  prompt: APIQueueInfoEntry | None = None
-  status: APIHistoryEntryStatus | None = None
+  outputs: Optional[Dict[APINodeID, APIOutputUI]] = None
+  prompt: Optional[APIQueueInfoEntry] = None
+  status: Optional[APIHistoryEntryStatus] = None
 
 
 class APIHistory(RootModel[Dict[PromptID, APIHistoryEntry]]):
   """Returned if you call /history and /history/{prompt_id} endpoints.
 
   TODO: Show an example.
   """
@@ -301,19 +301,19 @@
 
   extra: This is just to future proof the schema so it won't break if extra
   fields are added. They'll be stored dynamically.
 
   I allow extra here because I don't know what the keys are, and they seem to
   vary quite a bit.
   """
-  default: Any | None = None
-  min: Any | None = None
-  max: Any | None = None
-  step: Any | None = None
-  round: Any | None = None
+  default: Optional[Any] = None
+  min: Optional[Any] = None
+  max: Optional[Any] = None
+  step: Optional[Any] = None
+  round: Optional[Any] = None
   # Note: Everything else is going to be in the extra dict. Access it with the
   # `extra` attribute.
 
 
 class APIObjectInputTuple(NamedTuple):
   """
   Example:
@@ -322,17 +322,17 @@
   - INT
   - default: 0
     min: 0
     max: 18446744073709551615
 
     First item in the list/tuple is the type, second is the optional info.
   """
-  type: NamedInputType | ComboInputType
+  type: Union[NamedInputType, ComboInputType]
   # For some reason, when type=='*', this is an empty string.
-  info: APIObjectInputInfo | str | None = None
+  info: Union[APIObjectInputInfo, str, None] = None
 
 
 class APIObjectInput(BaseModel):
   """
   input:
       required:
         model:
@@ -347,22 +347,24 @@
   model_config = ConfigDict(extra=EXTRA)
   """This is a pydantic thing, to configure the model, it is not an accessible field.
 
   extra: This is just to future proof the schema so it won't break if extra
   fields are added. They'll be stored dynamically.
   """
 
-  required: Dict[str, APIObjectInputTuple | NamedInputType] | None = None
+  required: Optional[Dict[str, Union[APIObjectInputTuple,
+                                     NamedInputType]]] = None
   """
   For some reason, when type=='*', it just shows the type without a
   `[type, {... limits}] tuple, so I allowed NamedInputType.
   """
 
-  optional: Dict[str, APIObjectInputTuple | NamedInputType] | None = None
-  hidden: Dict[str, APIObjectInputTuple | NamedInputType] | None = None
+  optional: Optional[Dict[str, Union[APIObjectInputTuple,
+                                     NamedInputType]]] = None
+  hidden: Optional[Dict[str, Union[APIObjectInputTuple, NamedInputType]]] = None
 
 
 class APIObjectInfoEntry(BaseModel):
   """
 
   Example yaml version of this:
 
@@ -391,17 +393,17 @@
   model_config = ConfigDict(extra=EXTRA)
   """This is a pydantic thing, to configure the model, it is not an accessible field.
 
   extra: This is just to future proof the schema so it won't break if extra
   fields are added. They'll be stored dynamically.
   """
   input: APIObjectInput
-  output: OutputType | List[OutputType | List[OutputType]]
+  output: Union[OutputType, List[Union[OutputType, List[OutputType]]]]
   output_is_list: List[bool]
-  output_name: OutputName | List[OutputName]
+  output_name: Union[OutputName, List[OutputName]]
   name: str
   display_name: str
   description: str
   category: str
   output_node: bool
 
 
@@ -513,16 +515,16 @@
   """
   model_config = ConfigDict(extra=EXTRA)
   """This is a pydantic thing, to configure the model, it is not an accessible field.
 
   extra: This is just to future proof the schema so it won't break if extra
   fields are added. They'll be stored dynamically.
   """
-  node: str | None = None
-  prompt_id: PromptID | None = None
+  node: Optional[str] = None
+  prompt_id: Optional[PromptID] = None
 
 
 class WSMessage(BaseModel):
   """Messages from the websocket, if it is non-binary."""
   model_config = ConfigDict(extra=EXTRA)
   """This is a pydantic thing, to configure the model, it is not an accessible field.
```

### Comparing `comfy_catapult-2.0.0/comfy_catapult/comfy_schema_test.py` & `comfy_catapult-2.2.0/comfy_catapult/comfy_schema_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,16 @@
 from typing import List, Tuple, Type
 from unittest import IsolatedAsyncioTestCase
 
 import aiofiles
 import pydantic
 import yaml
 
-from comfy_catapult.comfy_schema import (VALID_FOLDER_TYPES, APIObjectInfo,
-                                         ComfyUIPathTriplet)
-from comfy_catapult.comfy_utils import TryParseAsModel
+from .comfy_schema import VALID_FOLDER_TYPES, APIObjectInfo, ComfyUIPathTriplet
+from .comfy_utils import TryParseAsModel
 
 INVALID_SUBFOLDER_EDGES: List[Tuple[str, Type[Exception]]] = [
     ('/', pydantic.ValidationError),
     ('/subfolder', pydantic.ValidationError),
     ('/subfolder/', pydantic.ValidationError),
     ('/subfolder/subsubfolder', pydantic.ValidationError),
     ('/subfolder/subsubfolder/', pydantic.ValidationError),
```

### Comparing `comfy_catapult-2.0.0/comfy_catapult/comfy_utils.py` & `comfy_catapult-2.2.0/comfy_catapult/comfy_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,33 +6,32 @@
 # the license text.
 
 import dataclasses
 import datetime
 import logging
 import textwrap
 from dataclasses import is_dataclass
-from typing import (Any, Generator, Hashable, List, Literal, NamedTuple, Type,
-                    TypeVar, cast)
+from typing import (Any, Generator, Hashable, List, Literal, NamedTuple,
+                    Optional, Type, TypeVar, Union, cast)
 
 import aiofiles
 import pydantic_core
 import pydash
 import yaml
 from anyio import Path
 from pydantic import BaseModel
 from pydash import slugify
 
-from comfy_catapult.comfy_schema import (APIHistoryEntry, APINodeID,
-                                         APIOutputUI, APIWorkflow,
-                                         APIWorkflowNodeInfo,
-                                         ComfyUIPathTriplet)
-from comfy_catapult.errors import MultipleNodesFound, NodeNotFound
-from comfy_catapult.remote_file_api_base import RemoteFileAPIBase
+from .comfy_schema import (APIHistoryEntry, APINodeID, APIOutputUI,
+                           APIWorkflow, APIWorkflowNodeInfo,
+                           ComfyUIPathTriplet)
+from .errors import MultipleNodesFound, NodeNotFound
+from .remote_file_api_base import RemoteFileAPIBase
 
-MAX_DUMP_LINES: int | None = 200
+MAX_DUMP_LINES: Optional[int] = 200
 logger = logging.getLogger(__name__)
 
 
 class NodeIDAndNode(NamedTuple):
   node_id: APINodeID
   node_info: APIWorkflowNodeInfo
 
@@ -43,15 +42,15 @@
   node_info: APIWorkflowNodeInfo
   for node_id, node_info in workflow.root.items():
     if node_info.meta is not None and node_info.meta.title == title:
       yield NodeIDAndNode(node_id=node_id, node_info=node_info)
 
 
 def FindNodeByTitle(*, workflow: APIWorkflow,
-                    title: str) -> NodeIDAndNode | None:
+                    title: str) -> Optional[NodeIDAndNode]:
   for (node_id, node_info) in FindNodesByTitle(workflow=workflow, title=title):
     return NodeIDAndNode(node_id=node_id, node_info=node_info)
   return None
 
 
 def GetNodeByTitle(*, workflow: APIWorkflow, title: str) -> NodeIDAndNode:
   nodes: List[NodeIDAndNode] = list(
@@ -67,20 +66,20 @@
                              found_nodes=[node_id for node_id, _ in nodes])
   node_id, node_info = nodes[0]
 
   return NodeIDAndNode(node_id=node_id, node_info=node_info)
 
 
 def FindNode(*, workflow: APIWorkflow,
-             id_or_title: int | str) -> NodeIDAndNode | None:
-  id_node_id: APINodeID | None = None
-  # id_node_error: Exception | None = None
+             id_or_title: Union[int, str]) -> Optional[NodeIDAndNode]:
+  id_node_id: Optional[APINodeID] = None
+  # id_node_error: Optional[Exception] = None
 
-  title_node_id: APINodeID | None = None
-  # title_node_error: Exception | None = None
+  title_node_id: Optional[APINodeID] = None
+  # title_node_error: Optional[Exception] = None
 
   try:
     if isinstance(id_or_title, str):
       title_node_id, _ = GetNodeByTitle(workflow=workflow, title=id_or_title)
 
   except NodeNotFound:
     # id_node_error = e
@@ -109,15 +108,16 @@
     if id_node_id is None:
       raise AssertionError('id_node_id is None')
 
     return NodeIDAndNode(node_id=id_node_id,
                          node_info=workflow.root[id_node_id])
 
 
-def GetNode(*, workflow: APIWorkflow, id_or_title: str | int) -> NodeIDAndNode:
+def GetNode(*, workflow: APIWorkflow, id_or_title: Union[str,
+                                                         int]) -> NodeIDAndNode:
   node = FindNode(workflow=workflow, id_or_title=id_or_title)
   if node is None:
     raise NodeNotFound(title=id_or_title, node_id=id_or_title)
   return node
 
 
 def GenerateNewNodeID(*, workflow: APIWorkflow) -> APINodeID:
@@ -132,15 +132,15 @@
       continue
 
   return cast(APINodeID, str(max_integer + 1))
 
 
 async def DownloadPreviewImage(*, node_id: APINodeID,
                                job_history: APIHistoryEntry,
-                               field_path: Hashable | List[Hashable],
+                               field_path: Union[Hashable, List[Hashable]],
                                comfy_api_url: str, remote: RemoteFileAPIBase,
                                local_dst_path: Path):
   """Downloads something that looks like an Preview Image node's outputs.
 
   * field_path=='gifs[0]' works for Video Combine
   * field_path=='images[0]' works for Preview Image
 
@@ -241,27 +241,28 @@
   while await path.exists():
     path = parent_path / f'{name}_{index}'
     index += 1
   await path.mkdir(parents=True, exist_ok=True)
   return path
 
 
-async def BigYamlDump(data: Any, *, max_lines: int | None, path: Path) -> str:
+async def BigYamlDump(data: Any, *, max_lines: Optional[int],
+                      path: Path) -> str:
   yaml_str = YamlDump(data)
   line_count = len(yaml_str.splitlines())
   if max_lines is None or line_count <= max_lines:
     return yaml_str
 
   await path.parent.mkdir(parents=True, exist_ok=True)
   async with aiofiles.open(path, 'w') as f:
     await f.write(yaml_str)
   return f'Too large, see {repr(str(path))}'
 
 
-async def BigErrorStrDump(exception: Exception, max_lines: int | None,
+async def BigErrorStrDump(exception: Exception, max_lines: Optional[int],
                           path: Path) -> str:
   if max_lines is None:
     return str(exception)
   error_str = str(exception)
   error_lines = error_str.splitlines()
   error_line = error_lines[0]
 
@@ -321,19 +322,19 @@
     pass
 
 
 async def TryParseAsModel(
     *,
     content: Any,
     model_type: Type[_BaseModelT],
-    errors_dump_directory: Path | None,
+    errors_dump_directory: Optional[Path],
     strict: Literal['yes', 'no', 'warn'] = 'warn') -> _BaseModelT:
 
-  async def _Internal(errors_dump_directory: Path | None):
-    error_dump_path: Path | None = None
+  async def _Internal(errors_dump_directory: Optional[Path]):
+    error_dump_path: Optional[Path] = None
 
     try:
       try:
         return model_type.model_validate(content,
                                          strict=strict in ['yes', 'warn'])
       except pydantic_core.ValidationError as e:
         if strict == 'yes':
```

### Comparing `comfy_catapult-2.0.0/comfy_catapult/errors.py` & `comfy_catapult-2.2.0/comfy_catapult/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,70 +2,78 @@
 # SPDX-License-Identifier: MIT
 #
 # The Comfy Catapult project requires contributions made to this file be licensed
 # under the MIT license or a compatible open source license. See LICENSE.md for
 # the license text.
 
 from copy import deepcopy
-from typing import Sequence
+from typing import Optional, Sequence, Union
 
-from comfy_catapult.comfy_schema import APINodeID, APIWorkflowTicket
+from .comfy_schema import APINodeID, APIWorkflowTicket
 
 
-class NodeNotFound(RuntimeError):
+class CatapultRuntimeError(RuntimeError):
+  pass
+
+
+class NodeNotFound(CatapultRuntimeError):
 
-  def __init__(self, *, node_id: APINodeID | int | None,
-               title: str | int | None):
+  def __init__(self, *, node_id: Union[APINodeID, int, None],
+               title: Union[str, int, None]):
     super().__init__(
         f'Node with title=={repr(title)}, node_id=={repr(node_id)} not found')
     self.node_id = node_id
     self.title = title
 
 
-class MultipleNodesFound(RuntimeError):
+class MultipleNodesFound(CatapultRuntimeError):
 
   def __init__(self, *, search_titles: Sequence[str],
                search_nodes: Sequence[APINodeID], found_titles: Sequence[str],
                found_nodes: Sequence[APINodeID]):
     super().__init__(
         f'Found multiple nodes with titles=={repr(found_titles)}, node_ids=={list(found_nodes)}'
         f' when searching for titles=={repr(search_titles)}, node_ids=={list(search_nodes)}'
     )
     self.search_titles = list(search_titles)
     self.search_node_ids = list(search_nodes)
     self.found_titles = list(found_titles)
     self.found_node_ids = list(found_nodes)
 
 
-class NodesNotExecuted(RuntimeError):
+class NodesNotExecuted(CatapultRuntimeError):
 
   def __init__(self, *, nodes: Sequence[APINodeID],
-               titles: Sequence[str | None] | None):
+               titles: Optional[Sequence[Optional[str]]]):
     if titles is None:
       titles = [None] * len(nodes)
     if len(nodes) != len(titles):
       raise ValueError(
           f'len(nodes) != len(titles): {len(nodes)} != {len(titles)}')
 
     super().__init__(
         f'Nodes {",".join(map(repr, nodes))} with titles {",".join(map(repr,titles))} not executed'
     )
     self.nodes = list(nodes)
     self.titles = list(titles)
 
 
-class WorkflowSubmissionError(RuntimeError):
+class WorkflowSubmissionError(CatapultRuntimeError):
 
   def __init__(self, msg, *, prepared_workflow: dict,
                ticket: APIWorkflowTicket):
     super().__init__(msg)
     self.prepared_workflow: dict = deepcopy(prepared_workflow)
     self.ticket: APIWorkflowTicket = deepcopy(ticket)
 
 
+class JobFailed(CatapultRuntimeError):
+  pass
+
+
 class URLValidationError(ValueError):
   pass
 
 
 class BasedURLValidationError(ValueError):
   pass
```

### Comparing `comfy_catapult-2.0.0/comfy_catapult/remote_file_api_base.py` & `comfy_catapult-2.2.0/comfy_catapult/remote_file_api_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # the license text.
 
 from abc import ABC, abstractmethod
 from typing import Tuple
 
 from anyio import Path
 
-from comfy_catapult.comfy_schema import ComfyUIPathTriplet
+from .comfy_schema import ComfyUIPathTriplet
 
 
 class RemoteFileAPIBase(ABC):
 
   @abstractmethod
   async def UploadFile(self, *, src_path: Path, untrusted_dst_url: str) -> str:
     """Upload a file.
@@ -63,10 +63,10 @@
 
   @abstractmethod
   def URLToTriplet(self, *, url: str) -> Tuple[str, ComfyUIPathTriplet]:
     """Convert a URL that this API can handle to a triplet, that this API can handle."""
     raise NotImplementedError()
 
   @abstractmethod
-  def GetBases(self) -> list[str]:
+  def GetBases(self) -> 'list[str]':
     """Return a list of base URLs that this API can handle."""
     raise NotImplementedError()
```

### Comparing `comfy_catapult-2.0.0/comfy_catapult/remote_file_api_comfy.py` & `comfy_catapult-2.2.0/comfy_catapult/remote_file_api_comfy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 # -*- coding: utf-8 -*-
 # SPDX-License-Identifier: MIT
 #
 # The Comfy Catapult project requires contributions made to this file be licensed
 # under the MIT license or a compatible open source license. See LICENSE.md for
 # the license text.
 
-from typing import List, Tuple
+from typing import List, Optional, Tuple, cast
 from urllib.parse import ParseResult
 
 from anyio import Path
+from typing_extensions import Literal
 
-from comfy_catapult.api_client import ComfyAPIClient
-from comfy_catapult.comfy_schema import (VALID_FOLDER_TYPES,
-                                         APIUploadImageResp,
-                                         ComfyUIPathTriplet)
-from comfy_catapult.remote_file_api_base import RemoteFileAPIBase
-from comfy_catapult.url_utils import (VALID_COMFY_API_SCHEMES, SmartURLJoin,
-                                      ToParseResult, ValidateIsBasedURL,
-                                      ValidateIsComfyAPITargetURL)
+from .api_client import ComfyAPIClient
+from .comfy_schema import (VALID_FOLDER_TYPES, APIUploadImageResp,
+                           ComfyUIPathTriplet)
+from .remote_file_api_base import RemoteFileAPIBase
+from .url_utils import (VALID_COMFY_API_SCHEMES, SmartURLJoin, ToParseResult,
+                        ValidateIsBasedURL, ValidateIsComfyAPITargetURL)
 
 VALID_COMFY_SCHEME_SCHEMES = ['comfy+http', 'comfy+https']
 
 
 def _ValidateComfyAPITargetURL(url: str, *,
-                               any_api_targets: List[str] | None) -> str:
+                               any_api_targets: Optional[List[str]]) -> str:
   url_pr = ToParseResult(url=url)
   if url_pr.scheme not in VALID_COMFY_API_SCHEMES:
     raise ValueError(
         f'URL {repr(url)} scheme does not start with one of {VALID_COMFY_API_SCHEMES}'
     )
 
   if any_api_targets is not None:
     if url not in any_api_targets:
       raise ValueError(f'URL {repr(url)} is not one of {any_api_targets}')
 
   return url
 
 
-def _ValidateComfySchemeURL(url: str, *, any_bases: List[str] | None) -> str:
+def _ValidateComfySchemeURL(url: str, *, any_bases: Optional[List[str]]) -> str:
   url_pr = ToParseResult(url=url)
   if url_pr.scheme not in VALID_COMFY_SCHEME_SCHEMES:
     raise ValueError(
         f'URL {repr(url)} scheme does not start with one of {VALID_COMFY_SCHEME_SCHEMES}'
     )
 
   # TODO: check the path
@@ -82,19 +81,21 @@
 
   # /folder_type/subfolder/filename => ('folder_type', 'subfolder', 'filename')
   # /folder_type/filename => ('folder_type', '', 'filename')
   # /folder_type/subfolder/subsubfolder/filename => ('folder_type', 'subfolder/subsubfolder', 'filename')
   # /folder_type//subfolder/subsubfolder/filename => ('folder_type', '/subfolder/subsubfolder', 'filename')
   # /folder_type/subfolder/subsubfolder//filename => ('folder_type', 'subfolder/subsubfolder/', 'filename')
 
-  folder_type, _, rest = url_path[1:].partition('/')
-  if folder_type not in VALID_FOLDER_TYPES:
+  folder_type_str: str
+  folder_type_str, _, rest = url_path[1:].partition('/')
+  if folder_type_str not in VALID_FOLDER_TYPES:
     raise ValueError(
         f'URL {repr(url)} path {repr(url_path)} does not start with one of {VALID_FOLDER_TYPES}'
     )
+  folder_type = cast(Literal['input', 'output', 'temp'], folder_type_str)
   subfolder, _, filename = rest.rpartition('/')
 
   comfy_api_url_pr = url_pr._replace(scheme=api_scheme, path='')
 
   triplet = ComfyUIPathTriplet(type=folder_type,
                                subfolder=subfolder,
                                filename=filename)
@@ -162,28 +163,28 @@
 
   Uses the /view and /upload API endpoints.
 
   Maps comfy+http://comfy_host:port/folder_type/subfolder/filename to the
   endpoints.
   """
 
-  def __init__(self, *, comfy_api_urls: List[str] | None, overwrite: bool):
+  def __init__(self, *, comfy_api_urls: Optional[List[str]], overwrite: bool):
     """Upload and download files from the ComfyUI API directly.
 
     Args:
         comfy_api_urls (str): The URL to the ComfyUI API, e.g
           http://127.0.0.1:8188. This is used for blacklisting any other
           attempts at upload or download. If None, then any URL is allowed to be
           uploaded or downloaded.
         overwrite (bool): If a file already exists, should it be overwritten? If
           false, the server will rename the file to something else and return
           that file name.
     """
     super().__init__()
-    self._comfy_api_urls: List[str] | None = None
+    self._comfy_api_urls: Optional[List[str]] = None
     if comfy_api_urls is not None:
       self._comfy_api_urls = [
           _ValidateComfyAPITargetURL(url, any_api_targets=None)
           for url in comfy_api_urls
       ]
 
     self._overwrite = overwrite
@@ -271,15 +272,15 @@
   def TripletToURL(self, *, comfy_api_url: str,
                    triplet: ComfyUIPathTriplet) -> str:
     return TripletToComfySchemeURL(comfy_api_url=comfy_api_url, triplet=triplet)
 
   def URLToTriplet(self, *, url: str) -> Tuple[str, ComfyUIPathTriplet]:
     return ComfySchemeURLToTriplet(url=url)
 
-  def GetBases(self) -> list[str]:
+  def GetBases(self) -> 'list[str]':
     if self._comfy_api_urls is None:
       return [f'comfy+{scheme}://' for scheme in VALID_COMFY_API_SCHEMES]
 
     return [
         ParseResult(scheme=f'comfy+{url_pr.scheme}',
                     netloc=url_pr.netloc,
                     path='',
```

### Comparing `comfy_catapult-2.0.0/comfy_catapult/remote_file_api_comfy_test.py` & `comfy_catapult-2.2.0/comfy_catapult/remote_file_api_comfy_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 from tempfile import TemporaryDirectory
 from typing import List
 from unittest import IsolatedAsyncioTestCase
 
 import pydantic
 from anyio import Path
 
-from comfy_catapult.comfy_schema import (VALID_FOLDER_TYPES, ComfyFolderType,
-                                         ComfyUIPathTriplet)
-from comfy_catapult.comfy_schema_test import VALID_SUBFOLDER_EDGES
-from comfy_catapult.remote_file_api_comfy import (ComfySchemeRemoteFileAPI,
-                                                  TripletToComfySchemeURL)
-from comfy_catapult.url_utils import SmartURLJoin
+from .comfy_schema import (VALID_FOLDER_TYPES, ComfyFolderType,
+                           ComfyUIPathTriplet)
+from .comfy_schema_test import VALID_SUBFOLDER_EDGES
+from .remote_file_api_comfy import (ComfySchemeRemoteFileAPI,
+                                    TripletToComfySchemeURL)
+from .url_utils import SmartURLJoin
 
 COMFY_API_URL = os.environ.get('COMFY_API_URL')
 if COMFY_API_URL is None:
   raise ValueError('Please set COMFY_API_URL in the environment')
 
 
 class TestRemoteFileApiComfy(IsolatedAsyncioTestCase):
```

### Comparing `comfy_catapult-2.0.0/comfy_catapult/remote_file_api_generic.py` & `comfy_catapult-2.2.0/comfy_catapult/remote_file_api_generic.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,48 +6,48 @@
 # the license text.
 
 from collections import defaultdict
 from typing import Dict, List, Tuple
 
 from anyio import Path
 
-from comfy_catapult.comfy_schema import ComfyUIPathTriplet
-from comfy_catapult.remote_file_api_base import RemoteFileAPIBase
-from comfy_catapult.url_utils import IsWeaklyRelativeTo
+from .comfy_schema import ComfyUIPathTriplet
+from .remote_file_api_base import RemoteFileAPIBase
+from .url_utils import IsWeaklyRelativeTo
 
 
 class GenericRemoteFileAPI(RemoteFileAPIBase):
   """Download or upload files from a URL, using multiple schemss.
   """
 
   def __init__(self):
     super().__init__()
-    self._base_to_api: Dict[str, List[RemoteFileAPIBase]] = defaultdict(list)
+    self._base_to_apis: Dict[str, List[RemoteFileAPIBase]] = defaultdict(list)
 
   def Register(self, api: RemoteFileAPIBase):
     for base in api.GetBases():
-      self._base_to_api[base].append(api)
+      self._base_to_apis[base].append(api)
 
   def _GetAPIsForURL(self, *, url: str) -> List[RemoteFileAPIBase]:
-    apis = []
-    for base, api in self._base_to_api.items():
+    apis: List[RemoteFileAPIBase] = []
+    for base, apis in self._base_to_apis.items():
       if IsWeaklyRelativeTo(base=base, url=url):
-        apis.append(api)
+        apis.extend(apis)
     if apis:
       return apis
     raise ValueError(f'URL {url} is not relative to any of'
-                     f' {self._base_to_api.keys()}, there is no API registered'
+                     f' {self._base_to_apis.keys()}, there is no API registered'
                      f' to handle such URLs')
 
   def _GetAPIsForTriplet(
       self, *, comfy_api_url: str,
       triplet: ComfyUIPathTriplet) -> List[RemoteFileAPIBase]:
     relevant_apis = []
     convered_urls = []
-    for base, base_apis in self._base_to_api.items():
+    for base, base_apis in self._base_to_apis.items():
       for api in base_apis:
         try:
           url = api.TripletToURL(comfy_api_url=comfy_api_url, triplet=triplet)
         except NotImplementedError:
           continue
 
         convered_urls.append({'base': base, 'url': url})
@@ -143,9 +143,9 @@
       try:
         return api.URLToTriplet(url=url)
       except (NotImplementedError, ValueError):
         if i + 1 >= len(apis):
           raise
     raise AssertionError('unreachable')
 
-  def GetBases(self) -> list[str]:
-    return list(self._base_to_api.keys())
+  def GetBases(self) -> 'list[str]':
+    return list(self._base_to_apis.keys())
```

### Comparing `comfy_catapult-2.0.0/comfy_catapult/remote_file_api_local.py` & `comfy_catapult-2.2.0/comfy_catapult/remote_file_api_local.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 # the license text.
 
 from typing import List, Tuple
 
 import aioshutil
 from anyio import Path
 
-from comfy_catapult.comfy_schema import ComfyUIPathTriplet
-from comfy_catapult.remote_file_api_base import RemoteFileAPIBase
-from comfy_catapult.url_utils import ToParseResult, ValidateIsBasedURL
+from .comfy_schema import ComfyUIPathTriplet
+from .remote_file_api_base import RemoteFileAPIBase
+from .url_utils import ToParseResult, ValidateIsBasedURL
 
 
 async def _LocalFileURLToLocalPath(url: str) -> Path:
   url_pr = ToParseResult(url)
   if url_pr.scheme != 'file':
     raise ValueError(f'URL {repr(url)} is not a file:// URL')
   if url_pr.netloc != '':
@@ -114,15 +114,15 @@
     # download the file from the URL. But this is not necessary right now,
     # because you can use the ComfyAPIRemoteFileAPI to download triplets,
     # and the GenericRemoteFileAPI to handle it transparently by choosing
     # the RemoteAPIFileBase.
     raise NotImplementedError('Local files do not support triplets')
 
   async def UploadToTriplet(
-      self, *, src_triplet: ComfyUIPathTriplet, untrusted_comfy_api_url: str,
+      self, *, src_path: Path, untrusted_comfy_api_url: str,
       untrusted_dst_triplet: ComfyUIPathTriplet) -> ComfyUIPathTriplet:
     # TODO: Maybe we can make a mapper that maps triplets to urls, and then
     # download the file from the URL. But this is not necessary right now,
     # because you can use the ComfyAPIRemoteFileAPI to download triplets,
     # and the GenericRemoteFileAPI to handle it transparently by choosing
     # the RemoteAPIFileBase.
     raise NotImplementedError('Local files do not support triplets')
@@ -130,9 +130,9 @@
   def TripletToURL(self, *, comfy_api_url: str,
                    triplet: ComfyUIPathTriplet) -> str:
     raise NotImplementedError('Local files do not support triplets')
 
   def URLToTriplet(self, *, url: str) -> Tuple[str, ComfyUIPathTriplet]:
     raise NotImplementedError('Local files do not support triplets')
 
-  def GetBases(self) -> list[str]:
+  def GetBases(self) -> 'list[str]':
     return list(self._upload_to_bases + self._download_from_bases)
```

### Comparing `comfy_catapult-2.0.0/comfy_catapult/url_utils.py` & `comfy_catapult-2.2.0/comfy_catapult/url_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 # The Comfy Catapult project requires contributions made to this file be licensed
 # under the MIT license or a compatible open source license. See LICENSE.md for
 # the license text.
 
 from typing import List, Literal
 from urllib.parse import ParseResult, urljoin, urlparse, urlunparse
 
-from comfy_catapult.errors import (BasedURLValidationError,
-                                   URLDirectoryValidationError,
-                                   URLValidationError)
+from .errors import (BasedURLValidationError, URLDirectoryValidationError,
+                     URLValidationError)
 
 ComfyAPIScheme = Literal['http', 'https']
 VALID_COMFY_API_SCHEMES: List[ComfyAPIScheme] = ['http', 'https']
 
 
 def SmartURLJoin(base: str, url: str) -> str:
   """urljoin() but can handle relative paths even for custom schemes.
```

### Comparing `comfy_catapult-2.0.0/comfy_catapult.egg-info/SOURCES.txt` & `comfy_catapult-2.2.0/comfy_catapult.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,26 +2,25 @@
 README.md
 pyproject.toml
 comfy_catapult/__init__.py
 comfy_catapult/api_client.py
 comfy_catapult/api_client_base.py
 comfy_catapult/catapult.py
 comfy_catapult/catapult_base.py
+comfy_catapult/cli.py
 comfy_catapult/comfy_schema.py
 comfy_catapult/comfy_schema_test.py
 comfy_catapult/comfy_utils.py
 comfy_catapult/errors.py
-comfy_catapult/eta_estimator.py
+comfy_catapult/py.typed
 comfy_catapult/remote_file_api_base.py
 comfy_catapult/remote_file_api_comfy.py
 comfy_catapult/remote_file_api_comfy_test.py
 comfy_catapult/remote_file_api_generic.py
 comfy_catapult/remote_file_api_local.py
 comfy_catapult/url_utils.py
 comfy_catapult/url_utils_test.py
 comfy_catapult.egg-info/PKG-INFO
 comfy_catapult.egg-info/SOURCES.txt
 comfy_catapult.egg-info/dependency_links.txt
 comfy_catapult.egg-info/requires.txt
-comfy_catapult.egg-info/top_level.txt
-examples/utilities/__init__.py
-examples/utilities/sdxlturbo_parse_args.py
+comfy_catapult.egg-info/top_level.txt
```

### Comparing `comfy_catapult-2.0.0/comfy_catapult.egg-info/requires.txt` & `comfy_catapult-2.2.0/comfy_catapult.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,91 +1,140 @@
 aiofiles<24,>=23
 aiohttp<4,>=3
 aioshutil<2,>=1
 aiosignal<2,>=1
 annotated-types<1
 anyio<5,>=4
 attrs<24,>=23
+colorama<1,>=0.4
 frozenlist<2,>=1
 idna<4,>=3
 multidict<7,>=6
 pydantic<3,>=2
 pydantic_core<3,>=2
 pydash<8,>=7
 python-slugify<9,>=8
 PyYAML<7,>=6
+rich<14,>=13
+rich-argparse<2,>=1
 six<2,>=1
 sniffio<2,>=1
 text-unidecode<2,>=1
 toml<1
+types-aiofiles<24,>=23
+types-colorama<1,>=0.4
 typing_extensions<5,>=4
 websockets<13,>=12
 yarl<2,>=1
 
+[:python_version < "3.8"]
+importlib-metadata
+
 [dev]
 aiofiles==23.2.1
 aiohttp==3.9.3
 aioshutil==1.3
 aiosignal==1.3.1
 annotated-types==0.6.0
 anyio==4.3.0
 argcomplete==3.2.3
 async-timeout==4.0.3
 attrs==23.2.0
 autoflake==2.2.1
+backports-tarfile==1.1.1
+beautifulsoup4==4.12.3
+bs4==0.0.2
 build==1.0.3
+certifi==2024.2.2
+cffi==1.16.0
 cfgv==3.4.0
+changeguard==0.3.1
+charset-normalizer==3.3.2
 click==8.1.7
 colorama==0.4.6
+cryptography==42.0.7
 defusedxml==0.7.1
 distlib==0.3.8
+docutils==0.21.2
 exceptiongroup==1.2.0
 filelock==3.13.1
 frozenlist==1.4.1
 identify==2.5.33
 idna==3.6
 importlib-metadata==7.0.1
 isort==5.13.2
+jaraco-classes==3.4.0
+jaraco-context==5.3.0
+jaraco-functools==4.0.1
+jeepney==0.8.0
 jinja2==3.1.3
+keyring==25.2.1
 linkify-it-py==2.0.2
 markdown-it-py==3.0.0
 markupsafe==2.1.4
 mdit-py-plugins==0.4.0
+mdremotifier==0.3.2
 mdurl==0.1.2
+mistletoe==1.3.0
+more-itertools==10.2.0
 multidict==6.0.5
+mypy==1.8.0
+mypy-extensions==1.0.0
+nh3==0.2.17
 nodeenv==1.8.0
 packaging==23.2
+pathspec==0.12.1
 pexpect==4.9.0
 pip-tools==7.3.0
+pkginfo==1.10.0
 platformdirs==4.1.0
 pre-commit==3.6.0
 ptyprocess==0.7.0
+pycparser==2.22
 pydantic==2.6.4
 pydantic-core==2.16.3
 pydash==7.0.7
 pyflakes==3.2.0
 pygments==2.17.2
 pyproject-hooks==1.0.0
+pyright==1.1.352
 python-slugify==8.0.4
 pyyaml==6.0.1
+readme-renderer==43.0
+regex==2024.5.15
+requests==2.31.0
+requests-toolbelt==1.0.0
+rfc3986==2.0.0
 rich==13.7.0
 rich-argparse==1.4.0
 ruamel-yaml==0.18.5
 ruamel-yaml-clib==0.2.8
+secretstorage==3.3.3
+semver==3.0.2
+shellingham==1.5.4
 six==1.16.0
 sniffio==1.3.1
-snipinator==1.1.0
+snipinator==1.4.1
+soupsieve==2.5
 text-unidecode==1.3
 toml==0.10.2
+toml-cli==0.6.1
 toml-sort==0.23.1
 tomli==2.0.1
 tomlkit==0.12.4
+twine==5.1.0
+typer==0.12.3
+types-aiofiles==23.2.0.20240403
+types-beautifulsoup4==4.12.0.20240511
 types-colorama==0.4.15.20240311
+types-html5lib==1.1.11.20240228
+types-pyyaml==6.0.12.20240311
 typing-extensions==4.10.0
 uc-micro-py==1.0.2
+urllib3==2.2.1
 virtualenv==20.25.0
 websockets==12.0
 wheel==0.43.0
 xmltodict==0.13.0
 yapf==0.40.2
 yarl==1.9.4
 yq==3.2.3
@@ -96,23 +145,31 @@
 aiohttp==3.9.3
 aioshutil==1.3
 aiosignal==1.3.1
 annotated-types==0.6.0
 anyio==4.3.0
 async-timeout==4.0.3
 attrs==23.2.0
+colorama==0.4.6
 exceptiongroup==1.2.0
 frozenlist==1.4.1
 idna==3.6
+markdown-it-py==3.0.0
+mdurl==0.1.2
 multidict==6.0.5
 pydantic==2.6.4
 pydantic-core==2.16.3
 pydash==7.0.7
+pygments==2.18.0
 python-slugify==8.0.4
 pyyaml==6.0.1
+rich==13.7.1
+rich-argparse==1.4.0
 six==1.16.0
 sniffio==1.3.1
 text-unidecode==1.3
 toml==0.10.2
+types-aiofiles==23.2.0.20240403
+types-colorama==0.4.15.20240311
 typing-extensions==4.10.0
 websockets==12.0
 yarl==1.9.4
```

### Comparing `comfy_catapult-2.0.0/pyproject.toml` & `comfy_catapult-2.2.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=64", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "comfy_catapult"
-version = "2.0.0"
+version = "2.2.0"
 description = "Programmatically schedule ComfyUI workflows."
 authors = [{name = "AYF", email = "realazthat@gmail.com"}]
 license = {file = "LICENSE.md"}
-readme = "README.md"
+readme = "README.remotified.md"
 keywords = [
   "pipeline",
   "scheduler",
   "stable-diffusion",
   "generative-ai",
   "comfyui"
 ]
@@ -26,26 +26,32 @@
   "aiofiles >=23,<24",
   "aiohttp >=3,<4",
   "aioshutil >=1,<2",
   "aiosignal >=1,<2",
   "annotated-types <1",
   "anyio >=4,<5",
   "attrs >=23,<24",
+  "colorama >=0.4,<1",
   "frozenlist >=1,<2",
   "idna >=3,<4",
+  'importlib-metadata; python_version < "3.8"',
   "multidict >=6,<7",
   "pydantic >=2,<3",
   "pydantic_core >=2,<3",
   "pydash >=7,<8",
   "python-slugify >=8,<9",
   "PyYAML >=6,<7",
+  "rich >=13,<14",
+  "rich-argparse >=1,<2",
   "six >=1,<2",
   "sniffio >=1,<2",
   "text-unidecode >=1,<2",
   "toml <1",
+  "types-aiofiles >=23,<24",
+  "types-colorama >=0.4,<1",
   "typing_extensions >=4,<5",
   "websockets >=12,<13",
   "yarl >=1,<2"
 ]
 
 [project.optional-dependencies]
 # Set of dependencies that are known to work. To add a new dependency here, add
@@ -58,27 +64,35 @@
   "aiohttp==3.9.3",
   "aioshutil==1.3",
   "aiosignal==1.3.1",
   "annotated-types==0.6.0",
   "anyio==4.3.0",
   "async-timeout==4.0.3",
   "attrs==23.2.0",
+  "colorama==0.4.6",
   "exceptiongroup==1.2.0",
   "frozenlist==1.4.1",
   "idna==3.6",
+  "markdown-it-py==3.0.0",
+  "mdurl==0.1.2",
   "multidict==6.0.5",
   "pydantic==2.6.4",
   "pydantic-core==2.16.3",
   "pydash==7.0.7",
+  "pygments==2.18.0",
   "python-slugify==8.0.4",
   "pyyaml==6.0.1",
+  "rich==13.7.1",
+  "rich-argparse==1.4.0",
   "six==1.16.0",
   "sniffio==1.3.1",
   "text-unidecode==1.3",
   "toml==0.10.2",
+  "types-aiofiles==23.2.0.20240403",
+  "types-colorama==0.4.15.20240311",
   "typing-extensions==4.10.0",
   "websockets==12.0",
   "yarl==1.9.4"
 ]
 # Set of dev dependencies, all pinned, so that they are known to work. To add a
 # new dependency here, add the unpinned package name here, and then run
 # `EXTRA=dev bash scripts/utilties/pin-extra-reqs.sh`.
@@ -89,64 +103,105 @@
   "aiosignal==1.3.1",
   "annotated-types==0.6.0",
   "anyio==4.3.0",
   "argcomplete==3.2.3",
   "async-timeout==4.0.3",
   "attrs==23.2.0",
   "autoflake==2.2.1",
+  "backports-tarfile==1.1.1",
+  "beautifulsoup4==4.12.3",
+  "bs4==0.0.2",
   "build==1.0.3",
+  "certifi==2024.2.2",
+  "cffi==1.16.0",
   "cfgv==3.4.0",
+  "changeguard==0.3.1",
+  "charset-normalizer==3.3.2",
   "click==8.1.7",
   "colorama==0.4.6",
+  "cryptography==42.0.7",
   "defusedxml==0.7.1",
   "distlib==0.3.8",
+  "docutils==0.21.2",
   "exceptiongroup==1.2.0",
   "filelock==3.13.1",
   "frozenlist==1.4.1",
   "identify==2.5.33",
   "idna==3.6",
   "importlib-metadata==7.0.1",
   "isort==5.13.2",
+  "jaraco-classes==3.4.0",
+  "jaraco-context==5.3.0",
+  "jaraco-functools==4.0.1",
+  "jeepney==0.8.0",
   "jinja2==3.1.3",
+  "keyring==25.2.1",
   "linkify-it-py==2.0.2",
   "markdown-it-py==3.0.0",
   "markupsafe==2.1.4",
   "mdit-py-plugins==0.4.0",
+  "mdremotifier==0.3.2",
   "mdurl==0.1.2",
+  "mistletoe==1.3.0",
+  "more-itertools==10.2.0",
   "multidict==6.0.5",
+  "mypy==1.8.0",
+  "mypy-extensions==1.0.0",
+  "nh3==0.2.17",
   "nodeenv==1.8.0",
   "packaging==23.2",
+  "pathspec==0.12.1",
   "pexpect==4.9.0",
   "pip-tools==7.3.0",
+  "pkginfo==1.10.0",
   "platformdirs==4.1.0",
   "pre-commit==3.6.0",
   "ptyprocess==0.7.0",
+  "pycparser==2.22",
   "pydantic==2.6.4",
   "pydantic-core==2.16.3",
   "pydash==7.0.7",
   "pyflakes==3.2.0",
   "pygments==2.17.2",
   "pyproject-hooks==1.0.0",
+  "pyright==1.1.352",
   "python-slugify==8.0.4",
   "pyyaml==6.0.1",
+  "readme-renderer==43.0",
+  "regex==2024.5.15",
+  "requests==2.31.0",
+  "requests-toolbelt==1.0.0",
+  "rfc3986==2.0.0",
   "rich==13.7.0",
   "rich-argparse==1.4.0",
   "ruamel-yaml==0.18.5",
   "ruamel-yaml-clib==0.2.8",
+  "secretstorage==3.3.3",
+  "semver==3.0.2",
+  "shellingham==1.5.4",
   "six==1.16.0",
   "sniffio==1.3.1",
-  "snipinator==1.1.0",
+  "snipinator==1.4.1",
+  "soupsieve==2.5",
   "text-unidecode==1.3",
   "toml==0.10.2",
+  "toml-cli==0.6.1",
   "toml-sort==0.23.1",
   "tomli==2.0.1",
   "tomlkit==0.12.4",
+  "twine==5.1.0",
+  "typer==0.12.3",
+  "types-aiofiles==23.2.0.20240403",
+  "types-beautifulsoup4==4.12.0.20240511",
   "types-colorama==0.4.15.20240311",
+  "types-html5lib==1.1.11.20240228",
+  "types-pyyaml==6.0.12.20240311",
   "typing-extensions==4.10.0",
   "uc-micro-py==1.0.2",
+  "urllib3==2.2.1",
   "virtualenv==20.25.0",
   "websockets==12.0",
   "wheel==0.43.0",
   "xmltodict==0.13.0",
   "yapf==0.40.2",
   "yarl==1.9.4",
   "yq==3.2.3",
@@ -154,16 +209,19 @@
 ]
 
 [project.urls]
 Homepage = "https://github.com/realazthat/comfy-catapult"
 Documentation = "https://github.com/realazthat/comfy-catapult"
 Repository = "https://github.com/realazthat/comfy-catapult"
 
-[tool.comfy-catapult-project-metadata]
-last_unstable_release = "2.0.0"
-last_stable_release = "2.0.0"
+[tool.comfy_catapult-project-metadata]
+last_release = "2.2.0"
+last_stable_release = "2.2.0"
+
+[tool.setuptools.package-data]
+comfy_catapult = ["py.typed"]
 
 [tool.setuptools.packages.find]
 where = ["."]
 include = ["comfy_catapult"]
 exclude = []
 namespaces = false
```

