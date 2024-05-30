# Comparing `tmp/scalexi-0.4.7.0.tar.gz` & `tmp/scalexi-0.4.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalexi-0.4.7.0.tar", last modified: Tue May 28 07:35:53 2024, max compression
+gzip compressed data, was "scalexi-0.4.7.1.tar", last modified: Thu May 30 11:17:22 2024, max compression
```

## Comparing `scalexi-0.4.7.0.tar` & `scalexi-0.4.7.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-28 07:35:53.886297 scalexi-0.4.7.0/
--rw-r--r--   0 akoubaa    (501) staff       (20)     2751 2023-11-18 18:27:29.000000 scalexi-0.4.7.0/LICENSE
--rw-r--r--   0 akoubaa    (501) staff       (20)     4525 2024-05-28 07:35:53.886165 scalexi-0.4.7.0/PKG-INFO
--rw-r--r--   0 akoubaa    (501) staff       (20)    15922 2023-11-22 16:53:27.000000 scalexi-0.4.7.0/README.md
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-28 07:35:53.870551 scalexi-0.4.7.0/scalexi/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.0/scalexi/__init__.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-28 07:35:53.872286 scalexi-0.4.7.0/scalexi/data/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.0/scalexi/data/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     4882 2024-05-27 15:01:35.000000 scalexi-0.4.7.0/scalexi/data/openai_pricing.json
--rw-r--r--   0 akoubaa    (501) staff       (20)     3723 2024-03-11 15:00:18.000000 scalexi-0.4.7.0/scalexi/data/openai_pricing_v1.json
--rw-r--r--   0 akoubaa    (501) staff       (20)     3517 2024-05-27 15:01:06.000000 scalexi-0.4.7.0/scalexi/data/openai_pricing_v2.json
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-28 07:35:53.872547 scalexi-0.4.7.0/scalexi/dataset_generation/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.0/scalexi/dataset_generation/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    32752 2023-11-20 18:15:53.000000 scalexi-0.4.7.0/scalexi/dataset_generation/prompt_completion.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-28 07:35:53.873353 scalexi-0.4.7.0/scalexi/document_loaders/
--rw-r--r--   0 akoubaa    (501) staff       (20)        0 2023-11-15 19:31:52.000000 scalexi-0.4.7.0/scalexi/document_loaders/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     3944 2023-11-20 17:59:39.000000 scalexi-0.4.7.0/scalexi/document_loaders/context_loaders.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     2167 2024-05-23 19:27:41.000000 scalexi-0.4.7.0/scalexi/document_loaders/pdf_loaders.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-28 07:35:53.875768 scalexi-0.4.7.0/scalexi/llm/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.0/scalexi/llm/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     4214 2024-01-29 23:03:40.000000 scalexi-0.4.7.0/scalexi/llm/google_gemini.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     9996 2024-01-29 23:59:01.000000 scalexi-0.4.7.0/scalexi/llm/openai_gpt.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-28 07:35:53.876700 scalexi-0.4.7.0/scalexi/llm_evaluation/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.0/scalexi/llm_evaluation/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    36889 2023-11-22 13:28:34.000000 scalexi-0.4.7.0/scalexi/llm_evaluation/evaluate.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-28 07:35:53.883692 scalexi-0.4.7.0/scalexi/openai/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.0/scalexi/openai/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    29566 2023-11-23 15:04:13.000000 scalexi-0.4.7.0/scalexi/openai/fine_tuning_api.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    34682 2024-05-27 16:10:27.000000 scalexi-0.4.7.0/scalexi/openai/pricing.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    12977 2024-05-27 16:28:54.000000 scalexi-0.4.7.0/scalexi/openai/utilities.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-28 07:35:53.885874 scalexi-0.4.7.0/scalexi/utilities/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.0/scalexi/utilities/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     1040 2024-05-25 09:44:04.000000 scalexi-0.4.7.0/scalexi/utilities/api.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    38655 2024-01-29 19:28:25.000000 scalexi-0.4.7.0/scalexi/utilities/data_formatter.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     2728 2024-01-29 21:41:32.000000 scalexi-0.4.7.0/scalexi/utilities/logger.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    19552 2024-05-27 15:18:11.000000 scalexi-0.4.7.0/scalexi/utilities/text_processing.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-28 07:35:53.871391 scalexi-0.4.7.0/scalexi.egg-info/
--rw-r--r--   0 akoubaa    (501) staff       (20)     4525 2024-05-28 07:35:53.000000 scalexi-0.4.7.0/scalexi.egg-info/PKG-INFO
--rw-r--r--   0 akoubaa    (501) staff       (20)      958 2024-05-28 07:35:53.000000 scalexi-0.4.7.0/scalexi.egg-info/SOURCES.txt
--rw-r--r--   0 akoubaa    (501) staff       (20)        1 2024-05-28 07:35:53.000000 scalexi-0.4.7.0/scalexi.egg-info/dependency_links.txt
--rw-r--r--   0 akoubaa    (501) staff       (20)      130 2024-05-28 07:35:53.000000 scalexi-0.4.7.0/scalexi.egg-info/requires.txt
--rw-r--r--   0 akoubaa    (501) staff       (20)        8 2024-05-28 07:35:53.000000 scalexi-0.4.7.0/scalexi.egg-info/top_level.txt
--rw-r--r--   0 akoubaa    (501) staff       (20)       38 2024-05-28 07:35:53.886333 scalexi-0.4.7.0/setup.cfg
--rw-r--r--   0 akoubaa    (501) staff       (20)     5404 2024-05-28 07:35:47.000000 scalexi-0.4.7.0/setup.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-30 11:17:22.902634 scalexi-0.4.7.1/
+-rw-r--r--   0 akoubaa    (501) staff       (20)     2751 2023-11-18 18:27:29.000000 scalexi-0.4.7.1/LICENSE
+-rw-r--r--   0 akoubaa    (501) staff       (20)     4525 2024-05-30 11:17:22.902427 scalexi-0.4.7.1/PKG-INFO
+-rw-r--r--   0 akoubaa    (501) staff       (20)    15922 2023-11-22 16:53:27.000000 scalexi-0.4.7.1/README.md
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-30 11:17:22.888454 scalexi-0.4.7.1/scalexi/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.1/scalexi/__init__.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-30 11:17:22.892992 scalexi-0.4.7.1/scalexi/data/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.1/scalexi/data/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     4882 2024-05-27 15:01:35.000000 scalexi-0.4.7.1/scalexi/data/openai_pricing.json
+-rw-r--r--   0 akoubaa    (501) staff       (20)     3723 2024-03-11 15:00:18.000000 scalexi-0.4.7.1/scalexi/data/openai_pricing_v1.json
+-rw-r--r--   0 akoubaa    (501) staff       (20)     3517 2024-05-27 15:01:06.000000 scalexi-0.4.7.1/scalexi/data/openai_pricing_v2.json
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-30 11:17:22.894322 scalexi-0.4.7.1/scalexi/dataset_generation/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.1/scalexi/dataset_generation/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    32752 2023-11-20 18:15:53.000000 scalexi-0.4.7.1/scalexi/dataset_generation/prompt_completion.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-30 11:17:22.895465 scalexi-0.4.7.1/scalexi/document_loaders/
+-rw-r--r--   0 akoubaa    (501) staff       (20)        0 2023-11-15 19:31:52.000000 scalexi-0.4.7.1/scalexi/document_loaders/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     3944 2023-11-20 17:59:39.000000 scalexi-0.4.7.1/scalexi/document_loaders/context_loaders.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     2167 2024-05-23 19:27:41.000000 scalexi-0.4.7.1/scalexi/document_loaders/pdf_loaders.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-30 11:17:22.897065 scalexi-0.4.7.1/scalexi/llm/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.1/scalexi/llm/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     4214 2024-01-29 23:03:40.000000 scalexi-0.4.7.1/scalexi/llm/google_gemini.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     9996 2024-01-29 23:59:01.000000 scalexi-0.4.7.1/scalexi/llm/openai_gpt.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-30 11:17:22.897747 scalexi-0.4.7.1/scalexi/llm_evaluation/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.1/scalexi/llm_evaluation/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    36889 2023-11-22 13:28:34.000000 scalexi-0.4.7.1/scalexi/llm_evaluation/evaluate.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-30 11:17:22.899696 scalexi-0.4.7.1/scalexi/openai/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.1/scalexi/openai/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    29566 2023-11-23 15:04:13.000000 scalexi-0.4.7.1/scalexi/openai/fine_tuning_api.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    34682 2024-05-27 16:10:27.000000 scalexi-0.4.7.1/scalexi/openai/pricing.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    12977 2024-05-27 16:28:54.000000 scalexi-0.4.7.1/scalexi/openai/utilities.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-30 11:17:22.901564 scalexi-0.4.7.1/scalexi/utilities/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.1/scalexi/utilities/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     1040 2024-05-25 09:44:04.000000 scalexi-0.4.7.1/scalexi/utilities/api.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    38655 2024-01-29 19:28:25.000000 scalexi-0.4.7.1/scalexi/utilities/data_formatter.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     2728 2024-01-29 21:41:32.000000 scalexi-0.4.7.1/scalexi/utilities/logger.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    19936 2024-05-29 16:14:23.000000 scalexi-0.4.7.1/scalexi/utilities/text_processing.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-30 11:17:22.891130 scalexi-0.4.7.1/scalexi.egg-info/
+-rw-r--r--   0 akoubaa    (501) staff       (20)     4525 2024-05-30 11:17:22.000000 scalexi-0.4.7.1/scalexi.egg-info/PKG-INFO
+-rw-r--r--   0 akoubaa    (501) staff       (20)      958 2024-05-30 11:17:22.000000 scalexi-0.4.7.1/scalexi.egg-info/SOURCES.txt
+-rw-r--r--   0 akoubaa    (501) staff       (20)        1 2024-05-30 11:17:22.000000 scalexi-0.4.7.1/scalexi.egg-info/dependency_links.txt
+-rw-r--r--   0 akoubaa    (501) staff       (20)      130 2024-05-30 11:17:22.000000 scalexi-0.4.7.1/scalexi.egg-info/requires.txt
+-rw-r--r--   0 akoubaa    (501) staff       (20)        8 2024-05-30 11:17:22.000000 scalexi-0.4.7.1/scalexi.egg-info/top_level.txt
+-rw-r--r--   0 akoubaa    (501) staff       (20)       38 2024-05-30 11:17:22.902684 scalexi-0.4.7.1/setup.cfg
+-rw-r--r--   0 akoubaa    (501) staff       (20)     5404 2024-05-29 10:05:42.000000 scalexi-0.4.7.1/setup.py
```

### Comparing `scalexi-0.4.7.0/LICENSE` & `scalexi-0.4.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.0/PKG-INFO` & `scalexi-0.4.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalexi
-Version: 0.4.7.0
+Version: 0.4.7.1
 Summary: The scalexi package is a versatile open-source Python library that focuses on facilitating low-code development and fine-tuning of diverse Large Language Models (LLMs). It extends beyond its initial OpenAI models integration, offering a scalable framework for various LLMs.
 Home-page: https://github.com/scalexi/scalexi
 Author: ScaleX Innovation
 Author-email: akoubaa@scalexi.ai
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `scalexi-0.4.7.0/README.md` & `scalexi-0.4.7.1/README.md`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.0/scalexi/data/openai_pricing.json` & `scalexi-0.4.7.1/scalexi/data/openai_pricing.json`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.0/scalexi/data/openai_pricing_v1.json` & `scalexi-0.4.7.1/scalexi/data/openai_pricing_v1.json`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.0/scalexi/data/openai_pricing_v2.json` & `scalexi-0.4.7.1/scalexi/data/openai_pricing_v2.json`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.0/scalexi/dataset_generation/prompt_completion.py` & `scalexi-0.4.7.1/scalexi/dataset_generation/prompt_completion.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.0/scalexi/document_loaders/context_loaders.py` & `scalexi-0.4.7.1/scalexi/document_loaders/context_loaders.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.0/scalexi/document_loaders/pdf_loaders.py` & `scalexi-0.4.7.1/scalexi/document_loaders/pdf_loaders.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.0/scalexi/llm/google_gemini.py` & `scalexi-0.4.7.1/scalexi/llm/google_gemini.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.0/scalexi/llm/openai_gpt.py` & `scalexi-0.4.7.1/scalexi/llm/openai_gpt.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.0/scalexi/llm_evaluation/evaluate.py` & `scalexi-0.4.7.1/scalexi/llm_evaluation/evaluate.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.0/scalexi/openai/fine_tuning_api.py` & `scalexi-0.4.7.1/scalexi/openai/fine_tuning_api.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.0/scalexi/openai/pricing.py` & `scalexi-0.4.7.1/scalexi/openai/pricing.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.0/scalexi/openai/utilities.py` & `scalexi-0.4.7.1/scalexi/openai/utilities.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.0/scalexi/utilities/api.py` & `scalexi-0.4.7.1/scalexi/utilities/api.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.0/scalexi/utilities/data_formatter.py` & `scalexi-0.4.7.1/scalexi/utilities/data_formatter.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.0/scalexi/utilities/logger.py` & `scalexi-0.4.7.1/scalexi/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.0/scalexi/utilities/text_processing.py` & `scalexi-0.4.7.1/scalexi/utilities/text_processing.py`

 * *Files 4% similar despite different names*

```diff
@@ -164,47 +164,48 @@
                 "total_tokens": response.usage.total_tokens
             }
         else:
             token_usage = {"error": "No token usage information available"}
 
         return token_usage
     
-def classify_text_binary(text, category_name, model_name="gpt-3.5-turbo-1106", 
+def classify_text_binary(text, category_name, criteria="", model_name="gpt-3.5-turbo-1106", 
                          openai_api_key=None, 
                          temperature=0.0, 
                          max_tokens=128, 
                          top_p=1.0, 
                          frequency_penalty=0.0, 
                          presence_penalty=0.0):
     """
     Classifies text using a specified model from OpenAI and checks if it matches the given category,
     also calculates the execution time, cost, and token usage.
     
     Args:
     text (str): The text to classify.
     category_name (str): The expected category name to validate against.
+    criteria: The criteria for the classification.
     model_name (str): Model identifier for OpenAI API.
     openai_api_key (str, optional): API key for OpenAI. If None, it fetches from environment variable.
     temperature (float): Sampling temperature.
     max_tokens (int): Maximum number of tokens to generate.
     top_p (float): Nucleus sampling parameter.
     frequency_penalty (float): Frequency penalty parameter.
     presence_penalty (float): Presence penalty parameter.
     
     Returns:
     dict: A dictionary with the classification results, execution time, cost, and token usage.
     """
     logger.info(f"[SCALEXI-classify_text_binary] Classifying text using model: {model_name}")
     # Define the system prompt
-    system_prompt = f"""You are a text classifier. 
-    Given a text, classify it into if it is a {category_name} category.
-    Your response should be in the valid JSON structure format without any markers (no ``` markers):
-    - "category": {category_name}
-    - "confidence": <float>
-    - "is_correct": <bool>
+    system_prompt = f"""You are a precise and strict text classifier for the "{category_name}" category. 
+Below are the specific criteria for the "{category_name}" category: {criteria}
+Provide your classification response in a valid JSON structure format, ensuring no use of code markers (e.g., no ``` markers). The response format should include:
+- "category": "{category_name}"
+- "reason": "<str>" (explanation for the classification decision)
+- "category_match": <bool> (True if the text clearly and explicitly belongs to the "{category_name}" category, otherwise False)
     """
     logger.debug(f"[SCALEXI-classify_text_binary] System prompt: {system_prompt}")
     
     # Define the prompt that contains the text
     prompt = f"Here is the text: {text}"
     
     # Measure the start time
@@ -251,16 +252,16 @@
     logger.debug(f'[SCALEXI-classify_text_binary] Response: {response}')
     
     #return response.choices[0].message.content, price, token_usage, execution_time
 
     # Prepare the final result
     final_result = {
         "category": completion['category'],
-        "confidence_score": completion['confidence'],
-        "is_correct": completion['is_correct'],
+        "category_match": completion['category_match'],
+        "reason": completion['reason'],  # "reason": "The text contains the word 'sports' multiple times.
         "execution_time": execution_time,
         "price": price,
         "token_usage": token_usage, 
         "model_name": model_name
     }
     logger.info(f'[SCALEXI-classify_text_binary] returning response, pricing, token_usage, execution_time')
     return final_result
```

### Comparing `scalexi-0.4.7.0/scalexi.egg-info/PKG-INFO` & `scalexi-0.4.7.1/scalexi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalexi
-Version: 0.4.7.0
+Version: 0.4.7.1
 Summary: The scalexi package is a versatile open-source Python library that focuses on facilitating low-code development and fine-tuning of diverse Large Language Models (LLMs). It extends beyond its initial OpenAI models integration, offering a scalable framework for various LLMs.
 Home-page: https://github.com/scalexi/scalexi
 Author: ScaleX Innovation
 Author-email: akoubaa@scalexi.ai
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `scalexi-0.4.7.0/scalexi.egg-info/SOURCES.txt` & `scalexi-0.4.7.1/scalexi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.0/setup.py` & `scalexi-0.4.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="scalexi",
-    version="0.4.7.0",
+    version="0.4.7.1",
     packages=find_packages(),
     include_package_data=True,
     package_data={'scalexi': ['data/*']},
     install_requires=[
         "pandas",  # Add any package dependencies here
         "openai>=1.10.0", #this package is not compatible with earlier versions of openai
         "sphinx",   # Add any other dependencies as needed
```

