# Comparing `tmp/ragtime-0.0.37.tar.gz` & `tmp/ragtime-0.0.39.tar.gz`

## Comparing `ragtime-0.0.37.tar` & `ragtime-0.0.39.tar`

### file list

```diff
@@ -1,44 +1,46 @@
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 ragtime-0.0.37/CHANGELOG.md
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 ragtime-0.0.37/CONTRIBUTING.md
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ragtime-0.0.37/deploy/deploy.py
--rw-r--r--   0        0        0    20599 2020-02-02 00:00:00.000000 ragtime-0.0.37/img/Ragtime_logo.png
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 ragtime-0.0.37/src/ragtime/__init__.py
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 ragtime-0.0.37/src/ragtime/api.py
--rw-r--r--   0        0        0     8789 2020-02-02 00:00:00.000000 ragtime-0.0.37/src/ragtime/config.py
--rw-r--r--   0        0        0    22584 2020-02-02 00:00:00.000000 ragtime-0.0.37/src/ragtime/expe.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 ragtime-0.0.37/src/ragtime/pipeline.py
--rw-r--r--   0        0        0     5927 2020-02-02 00:00:00.000000 ragtime-0.0.37/src/ragtime/base/llm.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragtime-0.0.37/src/ragtime/base/prompter.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 ragtime-0.0.37/src/ragtime/base/retriever.py
--rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 ragtime-0.0.37/src/ragtime/base/text_generator.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ragtime-0.0.37/src/ragtime/base_folder/.gitignore
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragtime-0.0.37/src/ragtime/base_folder/LICENSE
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 ragtime-0.0.37/src/ragtime/base_folder/README.md
--rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 ragtime-0.0.37/src/ragtime/base_folder/classes.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 ragtime-0.0.37/src/ragtime/base_folder/main.py
--rw-r--r--   0        0        0    15410 2020-02-02 00:00:00.000000 ragtime-0.0.37/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx
--rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 ragtime-0.0.37/src/ragtime/base_folder/res/html_templates/basic_template.jinja
--rw-r--r--   0        0        0    91060 2020-02-02 00:00:00.000000 ragtime-0.0.37/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx
--rw-r--r--   0        0        0     9987 2020-02-02 00:00:00.000000 ragtime-0.0.37/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx
--rw-r--r--   0        0        0    21761 2020-02-02 00:00:00.000000 ragtime-0.0.37/src/ragtime/base_folder/res/spreadsheet_templates/test_facts.xlsx
--rw-r--r--   0        0        0    33574 2020-02-02 00:00:00.000000 ragtime-0.0.37/src/ragtime/base_folder/res/spreadsheet_templates/with_retriever.xlsx
--rw-r--r--   0        0        0    27639 2020-02-02 00:00:00.000000 ragtime-0.0.37/src/ragtime/base_folder/res/spreadsheet_templates/without_retriever.xlsx
--rw-r--r--   0        0        0    29959 2020-02-02 00:00:00.000000 ragtime-0.0.37/src/ragtime/base_folder/res/spreadsheet_templates/old/basic_template_old.xlsx
--rw-r--r--   0        0        0    33387 2020-02-02 00:00:00.000000 ragtime-0.0.37/src/ragtime/base_folder/res/spreadsheet_templates/old/spreadsheet_rich_template.xlsx
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 ragtime-0.0.37/src/ragtime/prompters/__init__.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 ragtime-0.0.37/src/ragtime/prompters/answer/base_fr.py
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 ragtime-0.0.37/src/ragtime/prompters/answer/with_retriever.py
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 ragtime-0.0.37/src/ragtime/prompters/eval/base_fr.py
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 ragtime-0.0.37/src/ragtime/prompters/fact/base_fr.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 ragtime-0.0.37/src/ragtime/text_generators/__init__.py
--rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 ragtime-0.0.37/src/ragtime/text_generators/answer_generator.py
--rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 ragtime-0.0.37/src/ragtime/text_generators/eval_generator.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 ragtime-0.0.37/src/ragtime/text_generators/fact_generator.py
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 ragtime-0.0.37/tests/full_test.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 ragtime-0.0.37/tests/run_tests.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 ragtime-0.0.37/tests/test_quest.json
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 ragtime-0.0.37/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 ragtime-0.0.37/LICENSE
--rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 ragtime-0.0.37/README.md
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 ragtime-0.0.37/pyproject.toml
--rw-r--r--   0        0        0     7516 2020-02-02 00:00:00.000000 ragtime-0.0.37/PKG-INFO
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 ragtime-0.0.39/CHANGELOG.md
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 ragtime-0.0.39/CONTRIBUTING.md
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ragtime-0.0.39/deploy/deploy.py
+-rw-r--r--   0        0        0    20599 2020-02-02 00:00:00.000000 ragtime-0.0.39/img/Ragtime_logo.png
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/__init__.py
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/base.py
+-rw-r--r--   0        0        0     8910 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/config.py
+-rw-r--r--   0        0        0    23158 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/expe.py
+-rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/pipeline.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/base_folder/.gitignore
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/base_folder/LICENSE
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/base_folder/README.md
+-rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/base_folder/classes.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/base_folder/main.py
+-rw-r--r--   0        0        0    15410 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx
+-rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/base_folder/res/html_templates/basic_template.jinja
+-rw-r--r--   0        0        0    91060 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx
+-rw-r--r--   0        0        0     9987 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx
+-rw-r--r--   0        0        0    21761 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/base_folder/res/spreadsheet_templates/test_facts.xlsx
+-rw-r--r--   0        0        0    33574 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/base_folder/res/spreadsheet_templates/with_retriever.xlsx
+-rw-r--r--   0        0        0    27639 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/base_folder/res/spreadsheet_templates/without_retriever.xlsx
+-rw-r--r--   0        0        0    29959 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/base_folder/res/spreadsheet_templates/old/basic_template_old.xlsx
+-rw-r--r--   0        0        0    33387 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/base_folder/res/spreadsheet_templates/old/spreadsheet_rich_template.xlsx
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/generators/__init__.py
+-rw-r--r--   0        0        0     5313 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/generators/answer_generator.py
+-rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/generators/eval_generator.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/generators/fact_generator.py
+-rw-r--r--   0        0        0     5328 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/generators/text_generator.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/llms/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/llms/lite_llm.py
+-rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/llms/llm.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/prompters/__init__.py
+-rw-r--r--   0        0        0     7667 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/prompters/answer_prompters.py
+-rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/prompters/eval_prompters.py
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/prompters/fact_prompters.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/prompters/prompter.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/retrievers/__init__.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/retrievers/retriever.py
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 ragtime-0.0.39/tests/full_test.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 ragtime-0.0.39/tests/run_tests.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 ragtime-0.0.39/tests/test_quest.json
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 ragtime-0.0.39/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 ragtime-0.0.39/LICENSE
+-rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 ragtime-0.0.39/README.md
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 ragtime-0.0.39/pyproject.toml
+-rw-r--r--   0        0        0     7516 2020-02-02 00:00:00.000000 ragtime-0.0.39/PKG-INFO
```

### Comparing `ragtime-0.0.37/CHANGELOG.md` & `ragtime-0.0.39/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+# v0.0.39
+- packages hierarchy updated
+- prompters renamed
+- pipeline in progress
+
+# v0.0.38
+- Fully functionnal pipeline described as a dictionary
+- Ability to start and stop a test suite at any point
+
 # v0.0.37
 - Small fixes
 
 # v0.0.36 
 - Module renamed
 - Removed deprecated prompter (see v0.0.33)
 
@@ -36,8 +45,8 @@
 
 # v0.0.29
 - Update min Python version to 3.9
 - Added dependancies
 - Uses `Union` typing instead of `|`
 - Added a logging instruction in the `main.py` from `base_folder`
 - Explicitly sets an extra argument for the Logger (not needed in Python v3.10)
-- Added this CHANGELOG.md
+- Added this CHANGELOG.md
```

### Comparing `ragtime-0.0.37/CONTRIBUTING.md` & `ragtime-0.0.39/CONTRIBUTING.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Thanks for being here! Glad you wish to contribute!
 
 This repo contains the main Ragtime🎹 package. You can contribute by proposing new features, ideas, optimizations and documentation :)
 
 # Backlog
 Here are the projects we currently have in mind:
-- `Async [AS]`: moving the answer generation step to `async` so as to speed it up. At the moment, the main loop in `TextGenerator.generate` runs questions iteratively and, for each question, each LLM. Running in async would allow to run all this more quickly. We have to make sure not too many parallel calls to LLMs are made so as not to have calls blocked. Hence a limit per LLM has to be included.
+- `Test [TEST]`: user only has to provide documents, and question are automatically generated, their answer are automatically validated, facts are automatically generated and finally an evaluation is returned
 - `User interface [UI]`: add a user interface on top of the JSON files...big stuff!
+- `Fine tuning models [FTM]`: fine-tune models to generate questions, answers, facts and evaluations so that the package does not have to connect to an API
+- `LLM Ops [OPS]`: add the required features to use Ragtime in a LLM Ops workflow
 - `Documentation [Doc]`: add a wiki in GitHub
+- `CI/CD [CICD]`: add a CI/CD pipeline in `ragtime-package`
 
 # Testing the PR
 Before releasing you can test your PR with `full_test.py` in `tests`.
 
 You can then test the package with Linux and Windows if you're running with Windows computer with the `run_tests.py` script.
 Just set the variable `script_dir` to the local `tests` folder on your computer and tun the script. Is will run `full_test.py` in your Windows environment and then run it on your Linux environment (assuming you already have installed WSL2 on your Windows).
```

### Comparing `ragtime-0.0.37/img/Ragtime_logo.png` & `ragtime-0.0.39/img/Ragtime_logo.png`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.37/src/ragtime/config.py` & `ragtime-0.0.39/src/ragtime/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,186 +1,235 @@
 from enum import IntEnum
 from typing import Literal
 import ragtime
 import logging
 import logging.config
-import inspect
 from pathlib import Path
 import shutil
 import sys, os
 from importlib import resources
-if os.name == 'nt':
+
+if os.name == "nt":
     from py_setenv import setenv
-   
+
+#################################
+## CONSTANTS
+
+UNKOWN_LLM: str = "unkown LLM (manual ?)"
+#################################
+
 # # # FOLDERS
-QUESTIONS_FOLDER_NAME:str = "01. Questions"
-ANSWERS_FOLDER_NAME:str = "02. Answers"
-FACTS_FOLDER_NAME:str = "03. Facts"
-EVALS_FOLDER_NAME:str = "04. Evals"
-ROOT_FOLDER:Path = ROOT_FOLDER if "ROOT_FOLDER" in globals() else None
-FOLDER_EXPE:Path = FOLDER_EXPE if "FOLDER_EXPE" in globals() else None
-FOLDER_QUESTIONS:Path = FOLDER_QUESTIONS if "FOLDER_QUESTIONS" in globals() else None
-FOLDER_ANSWERS:Path = FOLDER_ANSWERS if "FOLDER_ANSWERS" in globals() else None
-FOLDER_FACTS:Path = FOLDER_FACTS if "FOLDER_FACTS" in globals() else None
-FOLDER_EVALS:Path = FOLDER_EVALS if "FOLDER_EVALS" in globals() else None
-FOLDER_TEMPLATES:Path = FOLDER_TEMPLATES if "FOLDER_TEMPLATES" in globals() else None
-FOLDER_SST_TEMPLATES:Path = FOLDER_SST_TEMPLATES if "FOLDER_SST_TEMPLATES" in globals() else None
-FOLDER_HTML_TEMPLATES:Path = FOLDER_HTML_TEMPLATES if "FOLDER_HTML_TEMPLATES" in globals() else None
+QUESTIONS_FOLDER_NAME: str = "01. Questions"
+ANSWERS_FOLDER_NAME: str = "02. Answers"
+FACTS_FOLDER_NAME: str = "03. Facts"
+EVALS_FOLDER_NAME: str = "04. Evals"
+ROOT_FOLDER: Path = ROOT_FOLDER if "ROOT_FOLDER" in globals() else None
+FOLDER_EXPE: Path = FOLDER_EXPE if "FOLDER_EXPE" in globals() else None
+FOLDER_QUESTIONS: Path = FOLDER_QUESTIONS if "FOLDER_QUESTIONS" in globals() else None
+FOLDER_ANSWERS: Path = FOLDER_ANSWERS if "FOLDER_ANSWERS" in globals() else None
+FOLDER_FACTS: Path = FOLDER_FACTS if "FOLDER_FACTS" in globals() else None
+FOLDER_EVALS: Path = FOLDER_EVALS if "FOLDER_EVALS" in globals() else None
+FOLDER_TEMPLATES: Path = FOLDER_TEMPLATES if "FOLDER_TEMPLATES" in globals() else None
+FOLDER_SST_TEMPLATES: Path = (
+    FOLDER_SST_TEMPLATES if "FOLDER_SST_TEMPLATES" in globals() else None
+)
+FOLDER_HTML_TEMPLATES: Path = (
+    FOLDER_HTML_TEMPLATES if "FOLDER_HTML_TEMPLATES" in globals() else None
+)
 # # # HTML
-DEFAULT_HTML_RENDERING:dict[str,bool] = DEFAULT_HTML_RENDERING if "DEFAULT_HTML_RENDERING" in globals() else None
-DEFAULT_HTML_TEMPLATE:Path = DEFAULT_HTML_TEMPLATE if "DEFAULT_HTML_TEMPLATE" in globals() else None
+DEFAULT_HTML_RENDERING: dict[str, bool] = (
+    DEFAULT_HTML_RENDERING if "DEFAULT_HTML_RENDERING" in globals() else None
+)
+DEFAULT_HTML_TEMPLATE: Path = (
+    DEFAULT_HTML_TEMPLATE if "DEFAULT_HTML_TEMPLATE" in globals() else None
+)
 # # # Spreadheet
-DEFAULT_SPREADSHEET_TEMPLATE:Path = DEFAULT_SPREADSHEET_TEMPLATE if "DEFAULT_SPREADSHEET_TEMPLATE" in globals() else None
-DEFAULT_WORKSHEET:str = DEFAULT_WORKSHEET if "DEFAULT_WORKSHEET" in globals() else None
-DEFAULT_HEADER_SIZE:int = DEFAULT_HEADER_SIZE if "DEFAULT_HEADER_SIZE" in globals() else None
-DEFAULT_QUESTION_COL:int = DEFAULT_QUESTION_COL if "DEFAULT_QUESTION_COL" in globals() else None
-DEFAULT_FACTS_COL:int = DEFAULT_FACTS_COL if "DEFAULT_FACTS_COL" in globals() else None
-DEFAULT_ANSWERS_COL:int = DEFAULT_ANSWERS_COL if "DEFAULT_ANSWERS_COL" in globals() else None
-DEFAULT_HUMAN_EVAL_COL:int = DEFAULT_HUMAN_EVAL_COL if "DEFAULT_HUMAN_EVAL_COL" in globals() else None
+DEFAULT_SPREADSHEET_TEMPLATE: Path = (
+    DEFAULT_SPREADSHEET_TEMPLATE
+    if "DEFAULT_SPREADSHEET_TEMPLATE" in globals()
+    else None
+)
+DEFAULT_WORKSHEET: str = DEFAULT_WORKSHEET if "DEFAULT_WORKSHEET" in globals() else None
+DEFAULT_HEADER_SIZE: int = (
+    DEFAULT_HEADER_SIZE if "DEFAULT_HEADER_SIZE" in globals() else None
+)
+DEFAULT_QUESTION_COL: int = (
+    DEFAULT_QUESTION_COL if "DEFAULT_QUESTION_COL" in globals() else None
+)
+DEFAULT_FACTS_COL: int = DEFAULT_FACTS_COL if "DEFAULT_FACTS_COL" in globals() else None
+DEFAULT_ANSWERS_COL: int = (
+    DEFAULT_ANSWERS_COL if "DEFAULT_ANSWERS_COL" in globals() else None
+)
+DEFAULT_HUMAN_EVAL_COL: int = (
+    DEFAULT_HUMAN_EVAL_COL if "DEFAULT_HUMAN_EVAL_COL" in globals() else None
+)
 # # # LLMs
-DEFAULT_LITELLM_RETRIES:int = DEFAULT_LITELLM_RETRIES if "DEFAULT_LITELLM_RETRIES" in globals() else None
-DEFAULT_LITELLM_TEMP:int = DEFAULT_LITELLM_TEMP if "DEFAULT_LITELLM_TEMP" in globals() else None
-DEFAULT_MAX_TOKENS:int = DEFAULT_MAX_TOKENS if "DEFAULT_MAX_TOKENS" in globals() else None
+DEFAULT_LITELLM_RETRIES: int = (
+    DEFAULT_LITELLM_RETRIES if "DEFAULT_LITELLM_RETRIES" in globals() else None
+)
+DEFAULT_LITELLM_TEMP: int = (
+    DEFAULT_LITELLM_TEMP if "DEFAULT_LITELLM_TEMP" in globals() else None
+)
+DEFAULT_MAX_TOKENS: int = (
+    DEFAULT_MAX_TOKENS if "DEFAULT_MAX_TOKENS" in globals() else None
+)
+
 
 # Logging - class to add msg
 class RagtimeLogger(logging.LoggerAdapter):
-    prefix:str = ""
+    prefix: str = ""
+
     def process(self, msg, kwargs):
         return f'{self.prefix + " " if self.prefix else ""}{msg}', kwargs
 
+
 logger: RagtimeLogger = logger if "logger" in globals() else None
-    
-def init(root_folder:Path):
+
+
+def init(root_folder: Path):
     """Init global variables for folder locations, template parameters and logger"""
-    if isinstance(root_folder, str): root_folder = Path(root_folder)
+    if isinstance(root_folder, str):
+        root_folder = Path(root_folder)
     # FOLDERS
     global ROOT_FOLDER, FOLDER_EXPE, FOLDER_QUESTIONS, FOLDER_ANSWERS, FOLDER_FACTS, FOLDER_EVALS, FOLDER_TEMPLATES, FOLDER_SST_TEMPLATES, FOLDER_HTML_TEMPLATES
     # # # HTML
     global DEFAULT_HTML_RENDERING, DEFAULT_HTML_TEMPLATE
     # # # Spreadheet
     global DEFAULT_SPREADSHEET_TEMPLATE, DEFAULT_WORKSHEET, DEFAULT_HEADER_SIZE, DEFAULT_QUESTION_COL, DEFAULT_FACTS_COL
     global DEFAULT_ANSWERS_COL, DEFAULT_HUMAN_EVAL_COL
     # # # LLMs
     global DEFAULT_LITELLM_RETRIES, DEFAULT_LITELLM_TEMP, DEFAULT_MAX_TOKENS
     # Logger
     global logger
-    
+
     # Folders
     ROOT_FOLDER = root_folder
-    FOLDER_EXPE = root_folder / 'expe'
+    FOLDER_EXPE = root_folder / "expe"
     FOLDER_QUESTIONS = FOLDER_EXPE / QUESTIONS_FOLDER_NAME
     FOLDER_ANSWERS = FOLDER_EXPE / ANSWERS_FOLDER_NAME
     FOLDER_FACTS = FOLDER_EXPE / FACTS_FOLDER_NAME
     FOLDER_EVALS = FOLDER_EXPE / EVALS_FOLDER_NAME
-    FOLDER_TEMPLATES = root_folder / 'res'
-    FOLDER_SST_TEMPLATES = FOLDER_TEMPLATES / 'spreadsheet_templates'
-    FOLDER_HTML_TEMPLATES = FOLDER_TEMPLATES / 'html_templates'
+    FOLDER_TEMPLATES = root_folder / "res"
+    FOLDER_SST_TEMPLATES = FOLDER_TEMPLATES / "spreadsheet_templates"
+    FOLDER_HTML_TEMPLATES = FOLDER_TEMPLATES / "html_templates"
     # # # HTML
-    DEFAULT_HTML_RENDERING = {"show_answers": True, "show_chunks": True, "show_facts": True, "show_evals": True}
-    DEFAULT_HTML_TEMPLATE = FOLDER_HTML_TEMPLATES / 'basic_template.jinja'
+    DEFAULT_HTML_RENDERING = {
+        "show_answers": True,
+        "show_chunks": True,
+        "show_facts": True,
+        "show_evals": True,
+    }
+    DEFAULT_HTML_TEMPLATE = FOLDER_HTML_TEMPLATES / "basic_template.jinja"
     # # # Spreadheet
-    DEFAULT_SPREADSHEET_TEMPLATE = FOLDER_SST_TEMPLATES / 'basic_template.xlsx'
+    DEFAULT_SPREADSHEET_TEMPLATE = FOLDER_SST_TEMPLATES / "basic_template.xlsx"
     DEFAULT_WORKSHEET = "Expe"
     DEFAULT_HEADER_SIZE = 2
     DEFAULT_QUESTION_COL = 2
     DEFAULT_FACTS_COL = 4
     DEFAULT_ANSWERS_COL = 11
     DEFAULT_HUMAN_EVAL_COL = 24
     # # # LLMs
     DEFAULT_LITELLM_RETRIES = 3
     DEFAULT_LITELLM_TEMP = 0
-    DEFAULT_MAX_TOKENS = 1000 # empirically noticed the biggest answers are 4000 characters long - and 1 token is between 4 and 5 chars - keep the largest value, i.e. 4 chars per token
+    DEFAULT_MAX_TOKENS = 1000  # empirically noticed the biggest answers are 4000 characters long - and 1 token is between 4 and 5 chars - keep the largest value, i.e. 4 chars per token
 
     ####################
     # LOGGING
     # You can choose the file where the logs are written in "log_conf" dict, key "handlers"/"file"/"filename" - default is "logs/logs.txt"
     # You can otherwise change everything you need as detailed in https://docs.python.org/3/library/logging.config.html
 
-    log_conf:dict = {
+    log_conf: dict = {
         "version": 1,
         "disable_existing_loggers": False,
         "formatters": {
             "standard": {
                 "format": "[%(asctime)s %(levelname)-4s %(filename)s %(funcName)s l.%(lineno)s] %(message)s"
-                }
-            },
+            }
+        },
         "handlers": {
             "console": {
                 "class": "logging.StreamHandler",
                 "formatter": "standard",
-                "stream" : "ext://sys.stdout"
+                "stream": "ext://sys.stdout",
             },
             "file": {
                 "formatter": "standard",
                 "class": "logging.handlers.RotatingFileHandler",
                 "filename": f"{root_folder}/logs/logs.txt",
                 "maxBytes": 1000000,
-                "encoding": 'utf-8'
-            }
+                "encoding": "utf-8",
+            },
         },
         "loggers": {
             "ragtime_logger": {
                 "handlers": ["console", "file"],
                 "level": "DEBUG",
-                "propagate": False
-                }
-        }
+                "propagate": False,
+            }
+        },
     }
 
     # Logging - create the logs in the folder of the calling script (not ragtime)
-    log_path:Path = root_folder / "logs"
-    if not log_path.exists(): log_path.mkdir()
+    log_path: Path = root_folder / "logs"
+    if not log_path.exists():
+        log_path.mkdir()
     logging.config.dictConfig(log_conf)
     logger = RagtimeLogger(logging.getLogger("ragtime_logger"), extra=None)
     # below is simply a hack to turn off unexpected LiteLLM logging with Ragtime logging set to INFO or DEBUG
     logging.getLogger().setLevel(logging.WARNING)
 
-class RagtimeException(Exception):
-    pass
-
-def format_exc(msg: str) -> str:
-    """Format the message for Exceptions - adds the call stack among other"""
-    inspect_stack = inspect.stack()
-    class_name:str = inspect_stack[1][0].f_locals["self"].__class__.__name__
-    return f'[{class_name}.{inspect.stack()[1][3]}()] {msg}'
-
-def div0(num:float, denom:float) -> float:
-    return float(num/denom) if denom else 0.0
-
-def init_project(name:str, init_type:Literal["globals_only", "copy_base_files", "delete_if_exists"]="globals_only", dest_path:Path = None):
+def init_project(
+    name: str,
+    init_type: Literal[
+        "globals_only", "copy_base_files", "delete_if_exists"
+    ] = "globals_only",
+    dest_path: Path = None,
+):
     """Initiates a project : copy base files and and set global variables
     Args:
     - init_type
         "globals_only" = 0 # do not touch the files, only initiates the global variables (logger, folder variables...)
         "copy_base_files" = 1 # globals_only + copy files to create base_folder, raise an exception if already exists
-        "delete_if_exists" = 2 # copy_base_files + remove folder if existing before copying base_folder"""
+        "delete_if_exists" = 2 # copy_base_files + remove folder if existing before copying base_folder
+    """
     if not dest_path:
-        if init_type == 'globals_only':
+        if init_type == "globals_only":
             dest_path = Path(sys.argv[0]).parent
         else:
             dest_path = Path(sys.argv[0]).parent / name
     if init_type != "globals_only":
-        src_path:Path = Path(resources.files("ragtime")) / 'base_folder'
+        src_path: Path = Path(resources.files("ragtime")) / "base_folder"
         if init_type == "delete_if_exists" and dest_path.exists():
             shutil.rmtree(dest_path)
         shutil.copytree(src_path, dest_path)
         # Add empty folders
-        for sub_folder in [QUESTIONS_FOLDER_NAME, ANSWERS_FOLDER_NAME, FACTS_FOLDER_NAME, EVALS_FOLDER_NAME]:
-            if not Path(dest_path / 'expe' / sub_folder).exists():
-                Path(dest_path / 'expe' / sub_folder).mkdir()
+        for sub_folder in [
+            QUESTIONS_FOLDER_NAME,
+            ANSWERS_FOLDER_NAME,
+            FACTS_FOLDER_NAME,
+            EVALS_FOLDER_NAME,
+        ]:
+            if not Path(dest_path / "expe" / sub_folder).exists():
+                Path(dest_path / "expe" / sub_folder).mkdir()
 
     init(dest_path)
 
-def init_win_env(env_vars:list[str]):
+
+def init_win_env(env_vars: list[str]):
     """Used to init environment variables in Windows"""
-    if os.name == 'nt': # only if os is Windows
+    if os.name == "nt":  # only if os is Windows
         for env_var in env_vars:
-            api_key:str = setenv(env_var, user=True, suppress_echo=True)
+            api_key: str = setenv(env_var, user=True, suppress_echo=True)
             if api_key:
                 os.environ[env_var] = api_key
 
 
 # Default init values if first import (i.e. logger is None)
-if not logger: 
-    root_folder:Path=Path(sys.argv[0]).parent
+if not logger:
+    root_folder: Path = Path(sys.argv[0]).parent
     os.chdir(root_folder)
-    init(root_folder=root_folder)
+    init(root_folder=root_folder)
+
+import litellm
+
+litellm.telemetry = False
+litellm.set_verbose = False  # used for debuging purpose
```

### Comparing `ragtime-0.0.37/src/ragtime/expe.py` & `ragtime-0.0.39/src/ragtime/expe.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,142 +1,143 @@
-from collections import defaultdict
-from enum import Enum, IntEnum
-import json
-from pathlib import Path
-import re
-import shutil
-from openpyxl import load_workbook, Workbook
-from openpyxl.worksheet.worksheet import Worksheet
-from openpyxl.cell.cell import ILLEGAL_CHARACTERS_RE
-from copy import copy
-from datetime import datetime
-from typing import Any, Callable, Generic, Optional, TypeVar, Union
-from pydantic import BaseModel, Field
+from ragtime.base import (
+    RagtimeBase,
+    RagtimeText,
+    RagtimeList,
+    RagtimeException,
+)
+
 from ragtime.config import (
     DEFAULT_FACTS_COL,
     DEFAULT_HUMAN_EVAL_COL,
     DEFAULT_HEADER_SIZE,
     DEFAULT_HUMAN_EVAL_COL,
     DEFAULT_ANSWERS_COL,
     DEFAULT_QUESTION_COL,
     DEFAULT_SPREADSHEET_TEMPLATE,
     DEFAULT_WORKSHEET,
-    RagtimeException,
     logger,
     DEFAULT_HTML_RENDERING,
-    DEFAULT_HTML_TEMPLATE
-    )
+    DEFAULT_HTML_TEMPLATE,
+)
+
+from collections import defaultdict
+
+from openpyxl import load_workbook, Workbook
+from openpyxl.worksheet.worksheet import Worksheet
+from openpyxl.cell.cell import ILLEGAL_CHARACTERS_RE
+
+from copy import copy
+from datetime import datetime
+from typing import Optional
+from pydantic import BaseModel, Field
 from jinja2 import Environment, FileSystemLoader
 from tabulate import tabulate
+from pathlib import Path
+import shutil
+import json
+import re
 
-class RagtimeBase(BaseModel):
-    meta: dict[str, Any] = {}
-
-class RagtimeText(RagtimeBase):
-    text:str = ""
+from enum import Enum, IntEnum
+from datetime import datetime
+from typing import Any, Generic, Optional, TypeVar, Union
+from enum import IntEnum
 
-T = TypeVar('T')
-class RagtimeList(RagtimeBase, Generic[T]):
-    items: list[T] = []
-
-    def __iter__(self):
-        return iter(self.items)
-
-    def __getitem__(self, item):
-        return self.items[item]
-
-    def __getitem__(self, row:int) -> T:
-        return self.items[row]
-    
-    def __setitem__(self, row:int, t: T):
-        self.items[row] = t
-    
-    def append(self, t: T):
-        self.items.append(t)
-
-    def __len__(self) -> int:
-        return len(self.items)
-    
-    def empty(self):
-        self.items = []    
 
 class Question(RagtimeText):
     pass
 
+
 class Questions(RagtimeList[Question]):
     pass
 
+
 class Prompt(RagtimeBase):
-    user:Optional[str] = ""
-    system:Optional[str] = ""
+    user: Optional[str] = ""
+    system: Optional[str] = ""
+
 
 class LLMAnswer(RagtimeText):
-    prompt:Optional[Prompt] = None
-    name:Optional[str] = None
-    full_name:Optional[str] = None
+    prompt: Optional[Prompt] = None
+    name: Optional[str] = None
+    full_name: Optional[str] = None
     timestamp: datetime = Optional[datetime]  # timestamp indicating when the question has been sent to the LLM
-    duration: Optional[float] = None # time to get the answer in seconds
+    duration: Optional[float] = None  # time to get the answer in seconds
     cost: Optional[float] = None
 
+
 class WithLLMAnswer(BaseModel):
-    llm_answer:Optional[LLMAnswer] = None
+    llm_answer: Optional[LLMAnswer] = None
+
 
 class Eval(RagtimeText, WithLLMAnswer):
     """At first an Eval is made by a human, and then automatically generated from an LLM Answer"""
-    human:Optional[float] = None
-    auto:Optional[float] = None
+
+    human: Optional[float] = None
+    auto: Optional[float] = None
+
 
 class Answer(RagtimeText, WithLLMAnswer):
-    eval:Optional[Eval] = Eval()
+    eval: Optional[Eval] = Eval()
+
 
 class Answers(RagtimeList[Answer]):
     pass
 
+
 class Fact(RagtimeText):
     """A single fact contains only text - all the LLM data are in the Facts object
     since every single Fact is created with a single LLM generation"""
+
     pass
 
+
 class Facts(RagtimeList[Fact], WithLLMAnswer):
     pass
 
+
 class TypesWithLLMAnswer(Enum):
     answer = Answer
     facts = Facts
     eval = Eval
 
+
 class Chunk(RagtimeText):
     pass
 
+
 class Chunks(RagtimeList[Chunk]):
     pass
 
+
 class QA(RagtimeBase):
-    question:Question = Question()
-    facts:Optional[Facts] = Facts()
-    chunks:Optional[Chunks] = Chunks()
-    answers:Optional[Answers] = Answers()
+    question: Question = Question()
+    facts: Optional[Facts] = Facts()
+    chunks: Optional[Chunks] = Chunks()
+    answers: Optional[Answers] = Answers()
 
-    def get_attr(self, path:str) -> list[Any]:
+    def get_attr(self, path: str) -> list[Any]:
         """Returns the value within a QA object based on its path expressed as a string
         Useful for spreadhseets export - returns None if path is not found"""
-        result:Any = self
-        b_return_None:bool = False
-        for a in path.split('.'):
+        result: Any = self
+        b_return_None: bool = False
+        for a in path.split("."):
             if "[" in a:
-                index:Union[str,int] = a[a.find('[')+1:a.rfind(']')]
-                a_wo_index:str = a[:a.find('[')]
+                index: Union[str, int] = a[a.find("[") + 1 : a.rfind("]")]
+                a_wo_index: str = a[: a.find("[")]
 
                 if index.isdecimal():
-                    index = int(index) # if index is an int (list index), convert it
-                elif index == "i": # multi row
-                    result = [self.get_attr(path.replace("[i]", f"[{i}]")) for i in range(len(getattr(result, a_wo_index)))]
+                    index = int(index)  # if index is an int (list index), convert it
+                elif index == "i":  # multi row
+                    result = [
+                        self.get_attr(path.replace("[i]", f"[{i}]"))
+                        for i in range(len(getattr(result, a_wo_index)))
+                    ]
                     return result
-                else: # dict (key not decimal)
-                    index = index.replace('"', '').replace("'", '') # if it is a string (dict index), remove quotes
+                else:  # dict (key not decimal)
+                    index = index.replace('"', "").replace("'", "")  # if it is a string (dict index), remove quotes
 
                 try:
                     result = getattr(result, a_wo_index)[index]
                 except:
                     b_return_None = True
             else:
                 try:
@@ -144,337 +145,424 @@
                 except:
                     b_return_None = True
             if b_return_None:
                 return None
 
         return result
 
+
 class UpdateTypes(IntEnum):
     human_eval = 0
     facts = 1
 
+
+class StartFrom(IntEnum):
+    beginning = 0
+    chunks = 1
+    prompt = 2
+    llm = 3
+    post_process = 4
+
+
 class Expe(RagtimeList[QA]):
-    meta:Optional[dict] = {}
-    json_path:Path = Field(None, exclude=True)
+    meta: Optional[dict] = {}
+    json_path: Path = Field(None, exclude=True)
 
-    def __init__(self, json_path:Path=None):
+    def __init__(self, json_path: Path = None):
         super().__init__()
         if json_path:
             self.json_path = json_path
             self.load_from_json(path=json_path)
 
     def stats(self) -> dict:
         """Returns stats about the expe : nb models, nb questions, nb facts, nb answers, nb human eval, nb auto eval"""
-        res:dict = {}
-        res['questions'] = len([qa for qa in self if qa.question.text])
-        res['chunks'] = len([c for qa in self for c in qa.chunks if c])
-        res['facts'] = len([f for qa in self for f in qa.facts if f])
-        res['models'] = len(self[0].answers)
-        res['answers'] = len([a for qa in self for a in qa.answers if a.text])
-        res['human eval'] = len([a for qa in self for a in qa.answers if a.eval and a.eval.human])
-        res['auto eval'] = len([a for qa in self for a in qa.answers if a.eval and a.eval.auto])
+        res: dict = {}
+        res["questions"] = len([qa for qa in self if qa.question.text])
+        res["chunks"] = len([c for qa in self for c in qa.chunks if c])
+        res["facts"] = len([f for qa in self for f in qa.facts if f])
+        res["models"] = len(self[0].answers)
+        res["answers"] = len([a for qa in self for a in qa.answers if a.text])
+        res["human eval"] = len(
+            [a for qa in self for a in qa.answers if a.eval and a.eval.human]
+        )
+        res["auto eval"] = len(
+            [a for qa in self for a in qa.answers if a.eval and a.eval.auto]
+        )
         return res
-            
+
     def get_name(self) -> str:
         """Returns the name of the Expe based on the number of questions, answers..."""
-        date_to_time_format:str = "%Y-%m-%d_%Hh%M,%S"
-        stats:dict = self.stats()
-        name:str = f'{stats["questions"]}Q_{stats["chunks"]}C_{stats["facts"]}F_{stats["models"]}M_{stats["answers"]}A_{stats["human eval"]}HE_{stats["auto eval"]}AE_{datetime.now().strftime(date_to_time_format)}'
+        date_to_time_format: str = "%Y-%m-%d_%Hh%M,%S"
+        stats: dict = self.stats()
+        name: str = (
+            f'{stats["questions"]}Q_{stats["chunks"]}C_{stats["facts"]}F_{stats["models"]}M_{stats["answers"]}A_{stats["human eval"]}HE_{stats["auto eval"]}AE_{datetime.now().strftime(date_to_time_format)}'
+        )
         return name
 
-    def _file_check_before_writing(self, path:Path=None, b_overwrite:bool=False, b_add_suffix:bool = True, force_ext:str=None) -> Path:
+    def _file_check_before_writing(
+        self,
+        path: Path = None,
+        b_overwrite: bool = False,
+        b_add_suffix: bool = True,
+        force_ext: str = None,
+    ) -> Path:
+        if path and path.is_dir():
+            if self.json_path:
+                path = path / self.json_path.stem
+            else:
+                raise RagtimeException('No JSON file attached to this Expe and you provided only a folder Path')
         if not path:
             if self.json_path:
                 path = Path(self.json_path.parent) / self.json_path.stem
             else:
-                raise RagtimeException(f'Cannot save to JSON since no json_path is stored in expe and not path has been provided in argument.')        
+                raise RagtimeException(f"Cannot save to JSON since no json_path is stored in expe and not path has been provided in argument.")
 
         # Make sure at least 1 QA is here
         if len(self) == 0:
-            raise Exception("""The Expe object you're trying to write is empty! Please add at least one QA""")
-        
+            raise Exception("The Expe object you're trying to write is empty! Please add at least one QA")
+
         # Check and prepare the destination file path
-        if not(path):
-            raise Exception("""No file defined - please specify a file name to save the Expe into""")
-        
+        if not (path):
+            raise Exception("No file defined - please specify a file name to save the Expe into")
+
         # If the provided path is a string, convert it to a Path
         result_path = Path(path) if isinstance(path, str) else path
 
         # If a suffix is to be added, add it
         if b_add_suffix:
-            file_no_ext:str = result_path.stem
+            file_no_ext: str = result_path.stem
             # genrates the new suffix like --5M_50Q_141F_50A_38HE
-            sep:str = "--"
-            new_suf:str = self.get_name()
-            if file_no_ext.find(sep) != -1: # if already a suffix, replace it
-                old_suf:str = file_no_ext[file_no_ext.find(sep)+len(sep):]
+            sep: str = "--"
+            new_suf: str = self.get_name()
+            if file_no_ext.find(sep) != -1:  # if already a suffix, replace it
+                old_suf: str = file_no_ext[file_no_ext.find(sep) + len(sep) :]
                 file_no_ext = file_no_ext.replace(old_suf, new_suf)
             else:
-                file_no_ext = f'{file_no_ext}{sep}{new_suf}'
-            str_name:str = f'{file_no_ext}{result_path.suffix}'
-            result_path = result_path.parent / Path(str_name)            
+                file_no_ext = f"{file_no_ext}{sep}{new_suf}"
+            str_name: str = f"{file_no_ext}{result_path.suffix}"
+            result_path = result_path.parent / Path(str_name)
 
         # Force ext
         if force_ext:
-            if result_path.suffix: # if already an extension, replace it
-                result_path = Path(str(result_path).replace(result_path.suffix, force_ext))
-            else: # if no extension, just add it
-                result_path = Path(f'{result_path}{force_ext}')
-        
+            if result_path.suffix:  # if already an extension, replace it
+                result_path = Path(
+                    str(result_path).replace(result_path.suffix, force_ext)
+                )
+            else:  # if no extension, just add it
+                result_path = Path(f"{result_path}{force_ext}")
+
         # If path exists and overwrite not allowed, raise an Exception
-        if result_path.is_file() and not b_overwrite: 
-            raise FileExistsError(f'"{path}" already exists! Set b_overwrite=True to allow overwriting.')
+        if result_path.is_file() and not b_overwrite:
+            raise FileExistsError(
+                f'"{path}" already exists! Set b_overwrite=True to allow overwriting.'
+            )
 
         return result_path
 
-    def load_from_json(self, path:Path):
+    def load_from_json(self, path: Path):
         with open(path, mode="r", encoding="utf-8") as file:
-            data:list = json.load(file)
-            qa_list:dict = data
-            if 'meta' in data:
-                self.meta = data['meta']
-                qa_list = data['items']
+            data: list = json.load(file)
+            qa_list: dict = data
+            if "meta" in data:
+                self.meta = data["meta"]
+                qa_list = data["items"]
             for json_qa in qa_list:
-                qa:QA = QA(**json_qa)
+                qa: QA = QA(**json_qa)
                 self.append(qa)
 
     def filter_answer(self, llm_facts_name: str):
         """
         Filters the current Expe object to include only the QA pairs with answers from the specified LLM.
         """
         for qa in self:
-            filtered_answers = [a for a in qa.answers if a.llm_answer and a.llm_answer.name == llm_facts_name]
+            filtered_answers = [
+                a
+                for a in qa.answers
+                if a.llm_answer and a.llm_answer.name == llm_facts_name
+            ]
             qa.answers = Answers(items=filtered_answers)
-    
+
     # TODO: Cannot implement this function due to circular imports issue (need objects from generators.py objects and generators.py needs
     # expe.py objects too) - if someone finds a way, that would be nice since it would allow to easily chain Answer, Facts and Eval generation
     # def gen_Eval(self, folder_out:Path, prompter:Prompter, llm_names:list[str],
     #             start_from:StartFrom=StartFrom.beginning, b_missing_only:bool = False, only_llms:list[str] = None, save_every:int=0):
     #     eval_gen:EvalGenerator = EvalGenerator(llm_names=llm_names, prompter=prompter)
     #     eval_gen.generate(self, start_from=start_from,  b_missing_only=b_missing_only, only_llms=only_llms, save_every=save_every)
     #     self.save_to_json(path=folder_out / self.json_file)
-   
-    def update_from_spreadsheet(self, path:Path, update_type:UpdateTypes, data_col:int=None, 
-                                question_col:int = DEFAULT_QUESTION_COL-1, answer_col:int = DEFAULT_ANSWERS_COL-1,
-                                sheet_name:str = DEFAULT_WORKSHEET, header_size:int=DEFAULT_HEADER_SIZE):
+
+    def update_from_spreadsheet(
+        self,
+        path: Path,
+        update_type: UpdateTypes,
+        data_col: int = None,
+        question_col: int = DEFAULT_QUESTION_COL - 1,
+        answer_col: int = DEFAULT_ANSWERS_COL - 1,
+        sheet_name: str = DEFAULT_WORKSHEET,
+        header_size: int = DEFAULT_HEADER_SIZE,
+    ):
         """Updates data from a spreadsheet, e.g. human evaluation or facts
         Args:
         - data_col (int): indicates the column number (starts at 0) from where the data will be imported in the spreadsheet
         if None (default), default column values are used, i.e. DEFAULT_FACTS_COL if update_type==Facts and
         DEFAULT_HUMAN_EVAL_COL if update_type==human_eval
         - update_type (UpdateTypes): can be "human_eval" or "facts"
         - question_col (int): indicates the column number (starts at 0) where the questions are - default: DEFAULT_QUESTION_COL-1 (0 based)
         - answer_col (in): used if update_type==human_eval, since the eval entered in the spreadsheet has to be matched with a specific answer
         """
-        def starts_with_num(fact:str) -> bool:
-            result:bool = False
+
+        def starts_with_num(fact: str) -> bool:
+            result: bool = False
             if "." in fact:
                 try:
-                    dummy:int = int(fact[:fact.find('.')])
+                    dummy: int = int(fact[: fact.find(".")])
                     result = True
-                except (TypeError, ValueError): pass
+                except (TypeError, ValueError):
+                    pass
             return result
 
-
-        wb:Workbook = load_workbook(path)
-        ws:Worksheet = wb[sheet_name]
-        cur_qa:QA = None
+        wb: Workbook = load_workbook(path)
+        ws: Worksheet = wb[sheet_name]
+        cur_qa: QA = None
         if not data_col:
-            data_cols:dict = {UpdateTypes.facts: DEFAULT_FACTS_COL, UpdateTypes.human_eval: DEFAULT_HUMAN_EVAL_COL}
-            data_col = data_cols[update_type]-1
-
-        new_facts:Facts = Facts() # the new facts to replace the old ones in the current QA
+            data_cols: dict = {
+                UpdateTypes.facts: DEFAULT_FACTS_COL,
+                UpdateTypes.human_eval: DEFAULT_HUMAN_EVAL_COL,
+            }
+            data_col = data_cols[update_type] - 1
+
+        new_facts: Facts = (
+            Facts()
+        )  # the new facts to replace the old ones in the current QA
 
         # For each row in the worksheet
-        for i, row in enumerate(ws.iter_rows(min_row=header_size+1), start=1):
-            if row[question_col].value: # a question is in the current row, so a new question starts
-                if cur_qa: # not first question
+        for i, row in enumerate(ws.iter_rows(min_row=header_size + 1), start=1):
+            if row[
+                question_col
+            ].value:  # a question is in the current row, so a new question starts
+                if cur_qa:  # not first question
                     cur_qa.facts = new_facts
-                cur_qa = next((qa for qa in self if qa.question.text.lower() == row[question_col].value.lower()), None) # get the corresponding QA in the Expe
-                new_facts:Facts = Facts()
-            
-            if cur_qa: # QA and question in the worksheet is made
+                cur_qa = next(
+                    (
+                        qa
+                        for qa in self
+                        if qa.question.text.lower() == row[question_col].value.lower()
+                    ),
+                    None,
+                )  # get the corresponding QA in the Expe
+                new_facts: Facts = Facts()
+
+            if cur_qa:  # QA and question in the worksheet is made
                 data_in_ws = row[data_col].value
                 if data_in_ws:
-                    if update_type == UpdateTypes.facts: # Update FACTS
-                        if not starts_with_num(data_in_ws): # if the fact in the ws does not start with a number, add it
-                            data_in_ws = f'{len(new_facts) + 1}. {data_in_ws}'
+                    if update_type == UpdateTypes.facts:  # Update FACTS
+                        if not starts_with_num(
+                            data_in_ws
+                        ):  # if the fact in the ws does not start with a number, add it
+                            data_in_ws = f"{len(new_facts) + 1}. {data_in_ws}"
                         new_facts.append(Fact(text=data_in_ws))
-                    elif update_type == UpdateTypes.human_eval: # Update HUMAN EVAL
-                        answer_text:str = row[answer_col].value
-                        cur_ans:Answer = next((a for a in cur_qa.answers if a.text == answer_text), None)
-                        if cur_ans: # corresponding Answer has been found
+                    elif update_type == UpdateTypes.human_eval:  # Update HUMAN EVAL
+                        answer_text: str = row[answer_col].value
+                        cur_ans: Answer = next(
+                            (a for a in cur_qa.answers if a.text == answer_text), None
+                        )
+                        if cur_ans:  # corresponding Answer has been found
                             try:
-                                human_eval:int = int(data_in_ws)
+                                human_eval: int = int(data_in_ws)
                                 cur_ans.eval.human = human_eval
                             except (TypeError, ValueError):
-                                logger.warn(f'Human eval should be a value between 0 and 1 - cannot use "{data_in_ws}" as found in line {i}')
+                                logger.warn(
+                                    f'Human eval should be a value between 0 and 1 - cannot use "{data_in_ws}" as found in line {i}'
+                                )
                         else:
-                            logger.warn(f'Cannot find Answer corresponding with the human eval "{data_in_ws}" - Answer should contain the text "{answer_text}"')                
-
-    def save_temp(self, name:str = "TEMP_"):
-        '''Save the expe as is as a temporary backup. Useful to save the work already done
-        when an Exception occurs or if you want to create intermediate backups while computing.'''
+                            logger.warn(
+                                f'Cannot find Answer corresponding with the human eval "{data_in_ws}" - Answer should contain the text "{answer_text}"'
+                            )
+
+    def save_temp(self, name: str = "TEMP_"):
+        """Save the expe as is as a temporary backup. Useful to save the work already done
+        when an Exception occurs or if you want to create intermediate backups while computing.
+        """
         if self.json_path:
-            file_name:str = f'{name}{self.json_path.stem}'
-            file_path:str = self.json_path.parent
+            file_name: str = f"{name}{self.json_path.stem}"
+            file_path: str = self.json_path.parent
         else:
-            file_name:str = f'{name}.json'
-            file_path:str = ''
-        self.save_to_json(path=Path(file_path) / Path(file_name), b_overwrite=True, b_add_suffix=True)
+            file_name: str = f"{name}.json"
+            file_path: str = ""
+        self.save_to_json(
+            path=Path(file_path) / Path(file_name), b_overwrite=True, b_add_suffix=True
+        )
 
     def save_to_json(
-            self,
-            path:Path=None,
-            b_overwrite:bool=False,
-            b_add_suffix:bool = True
+        self, path: Path = None, b_overwrite: bool = False, b_add_suffix: bool = True
     ) -> Path:
         """
         Saves Expe to JSON - can generate a suffix for the filename
         Returns the Path of the file actually saved
         """
-        path:Path = self._file_check_before_writing(
-            path,
-            b_overwrite = b_overwrite,
-            b_add_suffix = b_add_suffix,
-            force_ext='.json'
+        path: Path = self._file_check_before_writing(
+            path, b_overwrite=b_overwrite, b_add_suffix=b_add_suffix, force_ext=".json"
         )
-        with open(path, mode='w', encoding='utf-8') as file:
+        with open(path, mode="w", encoding="utf-8") as file:
             file.write(self.model_dump_json(indent=2))
         self.json_path = path
-        logger.info(f'Expe saved as JSON to {path}')
+        logger.info(f"Expe saved as JSON to {path}")
         return path
 
     def save_to_html(
-            self,
-            path:Path = None,
-            b_overwrite:bool=False,
-            b_add_suffix:bool = True,
-            render_params:dict[str,bool] = DEFAULT_HTML_RENDERING,
-            template_path:Path = DEFAULT_HTML_TEMPLATE,
+        self,
+        path: Path = None,
+        b_overwrite: bool = False,
+        b_add_suffix: bool = True,
+        render_params: dict[str, bool] = DEFAULT_HTML_RENDERING,
+        template_path: Path = DEFAULT_HTML_TEMPLATE,
     ):
         """
         Saves Expe to an HTML file from a Jinja template - can generate a suffix for the filename
         Returns the Path of the file actually saved
         """
-        path:Path = self._file_check_before_writing(path, b_overwrite=b_overwrite, b_add_suffix=b_add_suffix, force_ext='.html')
-        environment = Environment(loader=FileSystemLoader(searchpath=template_path.parent,encoding='utf-8'))
+        path: Path = self._file_check_before_writing(
+            path, b_overwrite=b_overwrite, b_add_suffix=b_add_suffix, force_ext=".html"
+        )
+        environment = Environment(
+            loader=FileSystemLoader(searchpath=template_path.parent, encoding="utf-8")
+        )
         template = environment.get_template(template_path.name)
-        context = {"expe": self, **render_params, "report_name": self.get_name(), "sub": (lambda pattern, repl, s: re.sub(pattern, repl, s))}
-        with open(path, mode='w', encoding='utf-8') as file:
+        context = {
+            "expe": self,
+            **render_params,
+            "report_name": self.get_name(),
+            "sub": (lambda pattern, repl, s: re.sub(pattern, repl, s)),
+        }
+        with open(path, mode="w", encoding="utf-8") as file:
             file.write(template.render(context))
-        logger.info(f'Expe saved as HTML to {path}')
+        logger.info(f"Expe saved as HTML to {path}")
         return path
 
-    def save_to_spreadsheet(self, path: Path = None, template_path: Path = DEFAULT_SPREADSHEET_TEMPLATE,
-                        header_size: int = DEFAULT_HEADER_SIZE, sheet_name: str = DEFAULT_WORKSHEET,
-                        b_overwrite: bool = False, b_add_suffix: bool = True):
-            """Saves Expe to a spreadsheet - can generate a suffix for the filename
-            Returns the Path of the file actually saved"""
-            path: Path = self._file_check_before_writing(path, b_overwrite=b_overwrite, b_add_suffix=b_add_suffix,
-                                                        force_ext='.xlsx')
-
-            # Prepare the result file
-            # Copy template
-            shutil.copy(template_path, path)
-            wb: Workbook = load_workbook(path)
-            wb.iso_dates = True
-
-            # Create worksheet
-            ws: Worksheet = wb[sheet_name]
-
-            # Retrieve sst configuration from original file
-            # ws_conf is a list of str, each element describes the path of the data to be added in the current row
-            ws_conf: list[str] = [cell.value for cell in ws[header_size + 1]]
-
-            # Write the values at specific rows - they are defined in second row, below the one describing the value to insert
-            for cell in ws[header_size + 2]:  # read the row just after the conf row - it contains configuration for specific rows
-                # if a value is present, analyse it - it should contain a "row" indication e.g. "answers[0].full_name, row=1"
-                if cell.value:
-                    if cell.value == "#":
-                        continue  # special token # used to indicate question number
-                    val: str = cell.value
-                    row: int = int(val[val.find('row=') + len('row='):])
-                    if row < 1:
-                        raise RagtimeException(
-                            f'The row value "row={row}" specified in cell {cell.coordinate} is invalid and must be greater than 0')
-                    # write the value since it does not need to be done for each row
-                    p: str = val[:val.find(',')]
-                    # get the first non empty value in the required column
-                    val = next((qa.get_attr(p) for qa in self if qa.get_attr(p)), "")
-                    ws.cell(row=row, column=cell.column, value=val)
-
-            qa: QA
-            row: int = header_size + 1
-            col_with_formulas: dict[int, str] = {c: ws.cell(column=c, row=row).value
-                                                for c in range(1, ws.max_column)
-                                                if ws.cell(column=c, row=row).value and str(ws.cell(column=c, row=row).value)[
-                                                    0] == "="}
-            for num_q, qa in enumerate(self, start=1):  # write each row in expe
-                next_row: int = 0
-                for col, p in enumerate(ws_conf, start=1):
-                    if p == "#":  # special token # used to indicate question number
-                        val = [num_q]
-                    elif p[0] == "=":  # if a formula is here, write it as is in the formula field
-                        continue
-                    else:  # if it is a path to get a value in QA, get it
-                        # Get value in the QA object
-                        val = qa.get_attr(p)
-                        if val is None or val == []:
-                            val = [""]  # write a blank if nothing is found
-                    if not isinstance(val, list):
-                        val = [val]
-
-                    # Write the value(s)
-                    for offset, v in enumerate(val):
-                        # Do standard conversions to string
-                        if isinstance(v, list):
-                            v = str(v)
-                        elif isinstance(v, datetime):
-                            v = v.strftime("%d/%m/%Y %H:%M:%S")
-                        # Remove illegal characters before writing the value
-                        cleaned_value = ILLEGAL_CHARACTERS_RE.sub("", str(v))
-                        # Write value
-                        ws.cell(row=row + offset, column=col).value = cleaned_value
-                        # From second row copy cell style from the one up
-                        if row + offset > header_size + 1:
-                            ws.cell(row=row + offset, column=col)._style = copy(ws.cell(row=header_size + 1, column=col)._style)
-
-                    next_row = max(next_row, row + offset + 1)
-                row = next_row
-
-            # extend the formulas
-            for row in range(header_size + 1, ws.max_row):
-                for col, formula in col_with_formulas.items():
-                    # simply adjust the row number in the formula
-                    cell_refs: set = set(re.findall(r"[A-Z]+[0-9]+", formula))
-                    for cell_ref in cell_refs:
-                        new_cell_ref: str = cell_ref.replace(str(header_size + 1), str(row))
-                        formula = formula.replace(cell_ref, new_cell_ref)
-                    ws.cell(row=row, column=col, value=formula)
-
-            # save spreadsheet
-            wb.save(path)
-            logger.info(f'Expe saved as Spreadsheet to {path}')
-            return path
-    
+    def save_to_spreadsheet(
+        self,
+        path: Path = None,
+        template_path: Path = DEFAULT_SPREADSHEET_TEMPLATE,
+        header_size: int = DEFAULT_HEADER_SIZE,
+        sheet_name: str = DEFAULT_WORKSHEET,
+        b_overwrite: bool = False,
+        b_add_suffix: bool = True,
+    ):
+        """Saves Expe to a spreadsheet - can generate a suffix for the filename
+        Returns the Path of the file actually saved"""
+        path: Path = self._file_check_before_writing(
+            path, b_overwrite=b_overwrite, b_add_suffix=b_add_suffix, force_ext=".xlsx"
+        )
 
-def analyse_expe_folder(path:Path):
-    if not path.is_dir(): raise Exception(f'"{path}" is not a folder - please provide one')
+        # Prepare the result file
+        # Copy template
+        shutil.copy(template_path, path)
+        wb: Workbook = load_workbook(path)
+        wb.iso_dates = True
+
+        # Create worksheet
+        ws: Worksheet = wb[sheet_name]
+
+        # Retrieve sst configuration from original file
+        # ws_conf is a list of str, each element describes the path of the data to be added in the current row
+        ws_conf: list[str] = [cell.value for cell in ws[header_size + 1]]
+
+        # Write the values at specific rows - they are defined in second row, below the one describing the value to insert
+        for cell in ws[header_size + 2]:  # read the row just after the conf row - it contains configuration for specific rows
+            # if a value is present, analyse it - it should contain a "row" indication e.g. "answers[0].full_name, row=1"
+            if cell.value:
+                if cell.value == "#":
+                    continue  # special token # used to indicate question number
+                val: str = cell.value
+                row: int = int(val[val.find("row=") + len("row=") :])
+                if row < 1:
+                    raise RagtimeException(
+                        f'The row value "row={row}" specified in cell {cell.coordinate} is invalid and must be greater than 0'
+                    )
+                # write the value since it does not need to be done for each row
+                p: str = val[: val.find(",")]
+                # get the first non empty value in the required column
+                val = next((qa.get_attr(p) for qa in self if qa.get_attr(p)), "")
+                ws.cell(row=row, column=cell.column, value=val)
+
+        qa: QA
+        row: int = header_size + 1
+        col_with_formulas: dict[int, str] = {
+            c: ws.cell(column=c, row=row).value
+            for c in range(1, ws.max_column)
+            if ws.cell(column=c, row=row).value
+            and str(ws.cell(column=c, row=row).value)[0] == "="
+        }
+        for num_q, qa in enumerate(self, start=1):  # write each row in expe
+            next_row: int = 0
+            for col, p in enumerate(ws_conf, start=1):
+                if p == "#":  # special token # used to indicate question number
+                    val = [num_q]
+                elif p[0] == "=":  # if a formula is here, write it as is in the formula field
+                    continue
+                else:  # if it is a path to get a value in QA, get it
+                    # Get value in the QA object
+                    val = qa.get_attr(p)
+                    if val is None or val == []:
+                        val = [""]  # write a blank if nothing is found
+                if not isinstance(val, list):
+                    val = [val]
+
+                # Write the value(s)
+                for offset, v in enumerate(val):
+                    # Do standard conversions to string
+                    if isinstance(v, list):
+                        v = str(v)
+                    elif isinstance(v, datetime):
+                        v = v.strftime("%d/%m/%Y %H:%M:%S")
+                    # Remove illegal characters before writing the value
+                    cleaned_value = ILLEGAL_CHARACTERS_RE.sub("", str(v))
+                    # Write value
+                    ws.cell(row=row + offset, column=col).value = cleaned_value
+                    # From second row copy cell style from the one up
+                    if row + offset > header_size + 1:
+                        ws.cell(row=row + offset, column=col)._style = copy(
+                            ws.cell(row=header_size + 1, column=col)._style
+                        )
+
+                next_row = max(next_row, row + offset + 1)
+            row = next_row
+
+        # extend the formulas
+        for row in range(header_size + 1, ws.max_row):
+            for col, formula in col_with_formulas.items():
+                # simply adjust the row number in the formula
+                cell_refs: set = set(re.findall(r"[A-Z]+[0-9]+", formula))
+                for cell_ref in cell_refs:
+                    new_cell_ref: str = cell_ref.replace(str(header_size + 1), str(row))
+                    formula = formula.replace(cell_ref, new_cell_ref)
+                ws.cell(row=row, column=col, value=formula)
+
+        # save spreadsheet
+        wb.save(path)
+        logger.info(f"Expe saved as Spreadsheet to {path}")
+        return path
+
+
+def analyse_expe_folder(path: Path):
+    if not path.is_dir():
+        raise Exception(f'"{path}" is not a folder - please provide one')
     print(f'In "{path}":')
-    res:defaultdict = defaultdict(list)
-    for f in [f for f in path.iterdir() if f.is_file() and f.suffix == '.json']:
-        exp:Expe = Expe(json_path=f)
-        res['File'].append(f.name)
-        for k, v in exp.stats(): res[k].append(v)
+    res: defaultdict = defaultdict(list)
+    for f in [f for f in path.iterdir() if f.is_file() and f.suffix == ".json"]:
+        exp: Expe = Expe(json_path=f)
+        res["File"].append(f.name)
+        for k, v in exp.stats():
+            res[k].append(v)
 
     print(tabulate(res, headers="keys"))
 
-def export_to_html(json_path:Path, render_params:dict[str,bool]=DEFAULT_HTML_RENDERING,
-                     template_path:Path=DEFAULT_HTML_TEMPLATE):
-  expe:Expe = Expe(json_path=json_path)
-  expe.save_to_html(path=json_path, render_params=render_params, template_path=template_path, b_add_suffix=True)
-
-def export_to_spreadsheet(json_path:Path, template_path:Path=DEFAULT_SPREADSHEET_TEMPLATE,
-                            header_size:int=DEFAULT_HEADER_SIZE, sheet_name:str = DEFAULT_WORKSHEET,):
-  expe:Expe = Expe(json_path=json_path)
-  expe.save_to_spreadsheet(path=json_path, template_path=template_path, header_size=header_size, sheet_name=sheet_name, b_add_suffix=True)
+
+# DEPRECATED
+# def export_to_html(json_path:Path, render_params:dict[str,bool]=DEFAULT_HTML_RENDERING,
+#                     template_path:Path=DEFAULT_HTML_TEMPLATE):
+#  expe:Expe = Expe(json_path=json_path)
+#  expe.save_to_html(path=json_path, render_params=render_params, template_path=template_path, b_add_suffix=True)
+#
+# def export_to_spreadsheet(json_path:Path, template_path:Path=DEFAULT_SPREADSHEET_TEMPLATE,
+#                            header_size:int=DEFAULT_HEADER_SIZE, sheet_name:str = DEFAULT_WORKSHEET,):
+#  expe:Expe = Expe(json_path=json_path)
+#  expe.save_to_spreadsheet(path=json_path, template_path=template_path, header_size=header_size, sheet_name=sheet_name, b_add_suffix=True)
```

### Comparing `ragtime-0.0.37/src/ragtime/base/llm.py` & `ragtime-0.0.39/src/ragtime/llms/llm.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,159 +1,169 @@
-#!/usr/bin/env python3
-
 from abc import abstractmethod
 
-from ragtime.base.text_generator import ( StartFrom )
-from ragtime.base.prompter import *
+from ragtime.prompters.prompter import Prompter
 
-from ragtime.expe import (
-    LLMAnswer,
-    RagtimeBase,
-    QA,
-    Prompt,
-    WithLLMAnswer
-)
-from ragtime.config import (
-    RagtimeException,
-    logger,
-    DEFAULT_MAX_TOKENS,
-)
+from ragtime.base import RagtimeBase
+from ragtime.expe import QA, Prompt, LLMAnswer, WithLLMAnswer, StartFrom
+from ragtime.config import logger, DEFAULT_MAX_TOKENS
 
-from litellm import ( completion_cost, acompletion )
-from litellm.exceptions import ( RateLimitError )
+from litellm import completion_cost, acompletion
+from litellm.exceptions import RateLimitError
 
-from datetime import ( datetime )
-from typing import ( Optional )
+from datetime import datetime
+from typing import Optional
 import asyncio
 
+
 class LLM(RagtimeBase):
     """
     Base class for text to text LLMs.
     Class deriving from LLM must implement `complete`.
     A Prompter must be provided at creation time.
     Instantiates a get_prompt so as to be able change the prompt LLM-wise.
     """
-    name:Optional[str] = None
-    prompter:Prompter
-    max_tokens:int = DEFAULT_MAX_TOKENS
-    _semaphore:asyncio.Semaphore = asyncio.Semaphore(1)
+
+    name: Optional[str] = None
+    prompter: Prompter
+    max_tokens: int = DEFAULT_MAX_TOKENS
+    _semaphore: asyncio.Semaphore = asyncio.Semaphore(1)
 
     async def generate(
-            self,
-            cur_obj:WithLLMAnswer,
-            prev_obj:WithLLMAnswer,
-            qa:QA,
-            start_from:StartFrom,
-            b_missing_only:bool,
-            **kwargs
+        self,
+        cur_obj: WithLLMAnswer,
+        prev_obj: WithLLMAnswer,
+        qa: QA,
+        start_from: StartFrom,
+        b_missing_only: bool,
+        **kwargs,
     ) -> WithLLMAnswer:
         """
         Generate prompt and execute LLM
         Returns the retrieved or created object containing the LLMAnswer
         If None, LLMAnswer retrieval or generation went wrong and post-processing
         must be skipped
         """
-        await self._semaphore.acquire()
-        logger.prefix = f'[{self.name}]'
+        # await self._semaphore.acquire()
+        logger.prefix = f"[{self.name}]"
 
         assert not prev_obj or (cur_obj.__class__ == prev_obj.__class__)
-        cur_class_name:str = cur_obj.__class__.__name__
+        cur_class_name: str = cur_obj.__class__.__name__
 
         # Get prompt
-        if not(prev_obj and prev_obj.llm_answer and prev_obj.llm_answer.prompt) or \
-        (start_from <= StartFrom.prompt and not b_missing_only):
-            logger.debug(f'Either no {cur_class_name} / LLMAnswer / Prompt exists yet, or you asked to regenerate Prompt ==> generate prompt')
+        if not (prev_obj and prev_obj.llm_answer and prev_obj.llm_answer.prompt) or (
+            start_from <= StartFrom.prompt and not b_missing_only
+        ):
+            logger.debug(
+                f"Either no {cur_class_name} / LLMAnswer / Prompt exists yet, or you asked to regenerate Prompt ==> generate prompt"
+            )
             prompt = self.prompter.get_prompt(**kwargs)
         else:
-            logger.debug(f'Reuse existing Prompt')
+            logger.debug(f"Reuse existing Prompt")
             prompt = prev_obj.llm_answer.prompt
 
         # Generates text
-        result:WithLLMAnswer = cur_obj
-        if not(prev_obj and prev_obj.llm_answer) or \
-           (start_from <= StartFrom.llm and not b_missing_only):
-            logger.debug(f'Either no {cur_class_name} / LLMAnswer exists yet, or you asked to regenerate it ==> generate LLMAnswer')
+        result: WithLLMAnswer = cur_obj
+        if not (prev_obj and prev_obj.llm_answer) or (
+            start_from <= StartFrom.llm and not b_missing_only
+        ):
+            logger.debug(
+                f"Either no {cur_class_name} / LLMAnswer exists yet, or you asked to regenerate it ==> generate LLMAnswer"
+            )
             try:
                 result.llm_answer = await self.complete(prompt)
             except Exception as e:
-                logger.exception(f'Exception while generating - skip it\n{e}')
+                logger.exception(f"Exception while generating - skip it\n{e}")
                 result = None
         else:
-            logger.debug(f'Reuse existing LLMAnswer in {cur_class_name}')
+            logger.debug(f"Reuse existing LLMAnswer in {cur_class_name}")
             result = prev_obj
 
         # Post-process
-        if result.llm_answer and (not (prev_obj and prev_obj.llm_answer) or not b_missing_only and start_from <= StartFrom.post_process):
-            logger.debug(f'Post-process {cur_class_name}')
+        if result.llm_answer and (
+            not (prev_obj and prev_obj.llm_answer)
+            or not b_missing_only
+            and start_from <= StartFrom.post_process
+        ):
+            logger.debug(f"Post-process {cur_class_name}")
             self.prompter.post_process(qa=qa, cur_obj=result)
         else:
-            logger.debug('Reuse post-processing')
-        self._semaphore.release()
+            logger.debug("Reuse post-processing")
+        # self._semaphore.release()
 
         return result
 
     @abstractmethod
-    async def complete(self, prompt:Prompt) -> LLMAnswer:
-        raise NotImplementedError('Must implement this!')
+    async def complete(self, prompt: Prompt) -> LLMAnswer:
+        raise NotImplementedError("Must implement this!")
+
 
 class LiteLLM(LLM):
     """
     Simple extension of LLM based on the litellm library.
     Allows to call LLMs by their name in a stantardized way.
     The default get_prompt method is not changed.
     The generate method uses the standard litellm completion method.
     Default values of temperature (0.0)
     Number of retries when calling the API (3) can be changed.
     The proper API keys and endpoints have to be specified in the keys.py module.
     """
-    name:str
-    temperature:float = 0.0
-    num_retries:int = 3
-
-    async def complete(self, prompt:Prompt) -> LLMAnswer:
-        messages:list[dict] = [
-            {"content":prompt.system, "role":"system"},
-            {"content":prompt.user, "role":"user"}
+
+    name: str
+    temperature: float = 0.0
+    num_retries: int = 3
+
+    async def complete(self, prompt: Prompt) -> LLMAnswer:
+        messages: list[dict] = [
+            {"content": prompt.system, "role": "system"},
+            {"content": prompt.user, "role": "user"},
         ]
-        retry:int = 1
-        wait_step:float = 3.0
-        start_ts:datetime = datetime.now()
-        answer:dict = None
+        retry: int = 1
+        wait_step: float = 3.0
+        start_ts: datetime = datetime.now()
+        answer: dict = None
         while retry < self.num_retries:
             try:
-                time_to_wait:float = wait_step
+                time_to_wait: float = wait_step
                 answer = await acompletion(
-                    messages = messages,
-                    model = self.name,
-                    temperature = self.temperature,
-                    num_retries = self.num_retries,
-                    max_tokens = self.max_tokens,
+                    messages=messages,
+                    model=self.name,
+                    temperature=self.temperature,
+                    num_retries=self.num_retries,
+                    max_tokens=self.max_tokens,
                 )
                 break
             except RateLimitError as e:
-                logger.debug(f'Rate limit reached - will retry in {time_to_wait:.2f}s\n\t{str(e)}')
+                logger.debug(
+                    f"Rate limit reached - will retry in {time_to_wait:.2f}s\n\t{str(e)}"
+                )
                 await asyncio.sleep(time_to_wait)
                 retry += 1
             except Exception as e:
-                logger.exception(f'The following exception occurred with prompt {prompt}' + '\n' + str(e))
+                logger.exception(
+                    f"The following exception occurred with prompt {prompt}"
+                    + "\n"
+                    + str(e)
+                )
                 return None
 
         # TODO:
         # remove this patch to a better error handling
 
         try:
-            full_name:str = answer['model']
-            text:str = answer['choices'][0]['message']['content']
-            duration:float = answer._response_ms/1000 if hasattr(answer, "_response_ms") else None # sometimes _response_ms is not present
-            cost:float = float(completion_cost(answer))
+            full_name: str = answer["model"]
+            text: str = answer["choices"][0]["message"]["content"]
+            duration: float = (
+                answer._response_ms / 1000 if hasattr(answer, "_response_ms") else None
+            )  # sometimes _response_ms is not present
+            cost: float = float(completion_cost(answer))
             return LLMAnswer(
-                name = self.name,
-                full_name= full_name,
-                prompt = prompt,
-                text = text,
-                timestamp = start_ts,
-                duration = duration,
-                cost = cost
+                name=self.name,
+                full_name=full_name,
+                prompt=prompt,
+                text=text,
+                timestamp=start_ts,
+                duration=duration,
+                cost=cost,
             )
         except Exception as e:
-            logger.debug(f'Faile to process the Answer. {e}')
+            logger.debug(f"Faile to process the Answer. {e}")
         return LLMAnswer()
```

### Comparing `ragtime-0.0.37/src/ragtime/base/prompter.py` & `ragtime-0.0.39/src/ragtime/prompters/prompter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 #!/usr/bin/env python3
 
-from abc import ( ABC, abstractmethod )
-from ragtime.expe import ( RagtimeBase, Prompt, QA, WithLLMAnswer )
+from abc import ABC, abstractmethod
+from ragtime.base import RagtimeBase
+from ragtime.expe import Prompt, QA, WithLLMAnswer
+
 
 class Prompter(RagtimeBase, ABC):
     """
     Base Prompter class. Every Prompter must inherit from it.
     A Prompter is designed to generate prompts for Answers, Facts and Evals.
     It also contains a method to post-process text returned by an LLM, since post-processing is directly related to the prompt
     It must be provided to every LLM objects at creation time
     """
-
+    system:str = None
+    
     @abstractmethod
     def get_prompt(self) -> Prompt:
-        raise NotImplementedError('Must implement this!')
+        raise NotImplementedError("Must implement this!")
 
     @abstractmethod
-    def post_process(self, qa:QA, cur_obj:WithLLMAnswer) -> WithLLMAnswer:
-        raise NotImplementedError('Must implement this!')
+    def post_process(self, qa: QA, cur_obj: WithLLMAnswer) -> WithLLMAnswer:
+        raise NotImplementedError("Must implement this!")
```

### Comparing `ragtime-0.0.37/src/ragtime/base/text_generator.py` & `ragtime-0.0.39/src/ragtime/generators/text_generator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,74 @@
 #!/usr/bin/env python3
 
-from abc import ( abstractmethod, ABC )
+from abc import abstractmethod, ABC
 
-from ragtime.base.retriever import ( Retriever )
-from ragtime.base.llm import *
+from ragtime.base import RagtimeBase
+from ragtime.expe import StartFrom, QA
+from ragtime.llms import LLM, LiteLLM
+from ragtime.prompters.prompter import Prompter
+from ragtime.base import RagtimeException
+from ragtime.config import logger
+from ragtime.expe import Expe
 
-from ragtime.expe import ( Expe, RagtimeBase, QA )
-from ragtime.config import ( RagtimeException, logger )
-
-from typing import ( Optional )
+from typing import Optional
 import asyncio
 
-from ragtime.expe import ( Answer, Answers, QA ) # TODO: This double name can be miss leading
-
-from enum import IntEnum
-class StartFrom(IntEnum):
-	beginning = 0
-	chunks = 1
-	prompt = 2
-	llm = 3
-	post_process = 4
-
 
 class TextGenerator(RagtimeBase, ABC):
     """
-    Abstract class for AnswerGenerator, FactGenerator, EvalGenerator
+    Abstract class for QuestionGenerator, AnswerGenerator, FactGenerator, EvalGenerator
     """
-    llms:Optional[list[LLM]] = []
-    b_use_chunks:bool = False
 
-    def __init__(self, llms:list[LLM] = None):
+    llms: Optional[list[LLM]] = []
+    b_use_chunks: bool = False
+
+    def __init__(self, llms: list = None, prompter:Prompter = None):
         """
         Args
             llms(LLM or list[LLM]) : list of LLM objects
         """
         super().__init__()
-        if (not llms):
-            raise RagtimeException('llms lists is empty! Please provide at least one.')
-        if isinstance(llms, LLM): llms = [llms]
-        self.llms +=  llms
-
+        if not llms:
+            raise RagtimeException("llms list is empty! Please provide at least one.")
+        if isinstance(llms, str):
+            llms = [llms]
+        for llm in llms:
+            if isinstance(llm, str):
+                if prompter:
+                    self.llms.append(LiteLLM(name=llm, prompter=prompter))
+                else:
+                    raise RagtimeException('You must provide a Prompter to create LLMs from their names only')
+            elif isinstance(llm, LLM):
+                self.llms.append(llm)
+            else:
+                raise RagtimeException(f'Objects in the llms list must be either str or LLM - {llm} is not')
 
     @property
     def llm(self) -> LLM:
         """
         Helper function to get the first LLM when only one is provided (like for EvalGenerator and FactGenerator)
         """
         if not self.llms:
             return None
         return self.llms[0]
 
-
     def generate(
-            self,
-            expe:Expe,
-            save_every:int = 0,
-            b_missing_only:bool = False,
-            only_llms:list[str] = None,
-            start_from:StartFrom = StartFrom.beginning,
+        self,
+        expe: Expe,
+        save_every: int = 0,
+        b_missing_only: bool = False,
+        only_llms: list[str] = None,
+        start_from: StartFrom = StartFrom.beginning,
     ):
         """
         Main method calling "gen_for_qa" for each QA in an Expe. Returns False if completed with error, True otherwise
         The main step in generation are :
         - beginning: start of the process - when start_from=beginning, the whole process is executed
-	    - chunks: only for Answer generation - chunk retrieval, if a Retriever is associated with the Answer Generator object
+            - chunks: only for Answer generation - chunk retrieval, if a Retriever is associated with the Answer Generator object
         Takes a Question and returns the Chunks
         - prompt: prompt generation, either directly using the question or with the chunks if any
         Takes a Question + optional Chunks and return a Prompt
         - llm: calling the LLM(s) with the generated prompts
         Takes a Prompt and return a LLMAnswer
         - post_process: post-processing the aswer returned by the LLM(s)
         Takes LLMAnswer + other information and updates the Answer object
@@ -75,52 +76,55 @@
             - expe: Expe object to generate for
             - start_from: allows to start generation from a specific step in the process
             - b_missing_only: True to execute the steps only when the value is absent, False to execute everything
             even if a value already exists
             - only_llms: restrict the llms to be computed again - used in conjunction with start_from -
             if start from beginning, chunks or prompts, compute prompts and llm answers for the list only -
             if start from llm, recompute llm answers for these llm only - has not effect if start
-            """
+        """
+
+        nb_q: int = len(expe)
 
-        logger.prefix += f"[{self._name}]"
-        nb_q:int = len(expe)
-        async def _generate_for_qa(num_q:int, qa:QA):
+        async def _generate_for_qa(num_q: int, qa: QA):
             logger.prefix = f"({num_q}/{nb_q})"
-            logger.info(f'*** {self.__class__.__name__} for question \n"{qa.question.text}"')
+            logger.info(
+                f'*** {self.__class__.__name__} for question \n"{qa.question.text}"'
+            )
             try:
                 await self.gen_for_qa(
                     qa=qa,
                     start_from=start_from,
                     b_missing_only=b_missing_only,
-                    only_llms=only_llms
+                    only_llms=only_llms,
                 )
             except Exception as e:
-                logger.exception(f"Exception caught - saving what has been done so far:\n{e}")
+                logger.exception(
+                    f"Exception caught - saving what has been done so far:\n{e}"
+                )
                 expe.save_to_json()
                 expe.save_temp(name=f"Stopped_at_{num_q}_of_{nb_q}_")
                 return
             logger.info(f'End question "{qa.question.text}"')
-            if save_every and (num_q % save_every == 0): expe.save_to_json()
+            if save_every and (num_q % save_every == 0):
+                expe.save_to_json()
 
         loop = asyncio.get_event_loop()
         tasks = [_generate_for_qa(num_q, qa) for num_q, qa in enumerate(expe, start=1)]
-        logger.info(f'{len(tasks)} tasks created')
+        logger.info(f"{len(tasks)} tasks created")
         loop.run_until_complete(asyncio.gather(*tasks))
 
-    def write_chunks(self, qa:QA):
+    def write_chunks(self, qa: QA):
         """Write chunks in the current qa if a Retriever has been given when creating the object. Ignore otherwise"""
-        raise NotImplementedError('Must implement this if you want to use it!')
-
+        raise NotImplementedError("Must implement this if you want to use it!")
 
     @abstractmethod
     async def gen_for_qa(
-            self,
-            qa:QA,
-            start_from:StartFrom=StartFrom.beginning,
-            b_missing_only:bool = True,
-            only_llms:list[str] = None
+        self,
+        qa: QA,
+        start_from: StartFrom = StartFrom.beginning,
+        b_missing_only: bool = True,
+        only_llms: list[str] = None,
     ):
         """
         Method to be implemented to generate Answer, Fact and Eval
         """
-        raise NotImplementedError('Must implement this!')
-
+        raise NotImplementedError("Must implement this!")
```

### Comparing `ragtime-0.0.37/src/ragtime/base_folder/.gitignore` & `ragtime-0.0.39/src/ragtime/base_folder/.gitignore`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.37/src/ragtime/base_folder/LICENSE` & `ragtime-0.0.39/src/ragtime/base_folder/LICENSE`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.37/src/ragtime/base_folder/classes.py` & `ragtime-0.0.39/src/ragtime/base_folder/classes.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.37/src/ragtime/base_folder/main.py` & `ragtime-0.0.39/src/ragtime/base_folder/main.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.37/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx` & `ragtime-0.0.39/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.37/src/ragtime/base_folder/res/html_templates/basic_template.jinja` & `ragtime-0.0.39/src/ragtime/base_folder/res/html_templates/basic_template.jinja`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.37/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx` & `ragtime-0.0.39/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.37/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx` & `ragtime-0.0.39/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.37/src/ragtime/base_folder/res/spreadsheet_templates/test_facts.xlsx` & `ragtime-0.0.39/src/ragtime/base_folder/res/spreadsheet_templates/test_facts.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.37/src/ragtime/base_folder/res/spreadsheet_templates/with_retriever.xlsx` & `ragtime-0.0.39/src/ragtime/base_folder/res/spreadsheet_templates/with_retriever.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.37/src/ragtime/base_folder/res/spreadsheet_templates/without_retriever.xlsx` & `ragtime-0.0.39/src/ragtime/base_folder/res/spreadsheet_templates/without_retriever.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.37/src/ragtime/base_folder/res/spreadsheet_templates/old/basic_template_old.xlsx` & `ragtime-0.0.39/src/ragtime/base_folder/res/spreadsheet_templates/old/basic_template_old.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.37/src/ragtime/base_folder/res/spreadsheet_templates/old/spreadsheet_rich_template.xlsx` & `ragtime-0.0.39/src/ragtime/base_folder/res/spreadsheet_templates/old/spreadsheet_rich_template.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.37/src/ragtime/prompters/answer/with_retriever.py` & `ragtime-0.0.39/src/ragtime/prompters/answer_prompters.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,155 +1,199 @@
-#!/usr/bin/env python3
-
-from ragtime.base.prompter import ( Prompter )
-
-from ragtime.expe import ( QA, Prompt, Question, Chunks, Answer )
+from typing import Optional
+from ragtime.expe import QA, Prompt, Question, Chunks, Answer
+from ragtime.prompters import Prompter
 from ragtime.config import logger
 
 from langdetect import detect
 import json
 from unidecode import unidecode
 from typing import Optional
 
-
-class PptrAnsWithRetrieverFR(Prompter):
+class AnsPrompterBase(Prompter):
     """
-    This prompter uses a prompt asking the LLM to generate a JSON structure
-    and includes chunks in its prompt. It performs post-processing to exploit
-    the JSON structure the LLM is supposed to generate.
+    This simple prompter just send the question as is to the LLM
+    and does not perform any post-processing
     """
-    FLD_QUEST_OK:str = "q_ok"
-    FLD_CHUNKS_OK:str = "chunks_ok"
-    FLD_ANSWER:str = "answer"
+    system:str = ""
+
+    def get_prompt(self, question: Question, chunks: Optional[Chunks] = None) -> Prompt:
+        result: Prompt = Prompt()
+        result.user = f"{question.text}"
+        result.system = self.system
+        return result
 
-    def get_prompt( self, question:Question, chunks:Optional[Chunks] = None ) -> Prompt:
+    def post_process(self, qa: QA = None, cur_obj: Answer = None):
         """
-        This Answer prompt asks for a JSON answer
+        Does not do anything by default, but can be overridden to add fields in meta data for instance
         """
+        cur_obj.text = cur_obj.llm_answer.text
 
-        # Format string to convert a chunk into a string
-        fmt_chunk_to_str:str = """- {title} (p. {page})
-        {text}"""
-
-        # Format string to join the strings representing the different chunks
-        str_joint:str = "\n\n"
-
-        # Format string to convert the string containing all the chunks to a user prompt
-        fmt_chunks_to_user_msg:str = """{chunks}
-        La question est '{question}'"""
+class AnsPrompterWithRetrieverFR(Prompter):
+    """
+    This prompter uses a prompt asking the LLM to generate a JSON structure
+    and includes chunks in its prompt. It performs post-processing to exploit
+    the JSON structure the LLM is supposed to generate.
+    """
 
-        # System prompt
-        system_msg:str = f"""Tu es un expert qui doit répondre à des questions à l'aide de paragraphes qui te sont fournis.
+    FLD_QUEST_OK: str = "q_ok"
+    FLD_CHUNKS_OK: str = "chunks_ok"
+    FLD_ANSWER: str = "answer"
+    system:str = f"""Tu es un expert qui doit répondre à des questions à l'aide de paragraphes qui te sont fournis.
         Tu dois utiliser uniquement ces paragraphes pour répondre aux questions.
         Tu dois inclure les titres exacts de ces paragraphes dans la réponse que tu renvoies.
         Tu dois justifier tes réponses et expliquer comment tu les as construites.
         Tu dois détailler les phrases et les mots qui te permettent de générer ta réponse.
 
         Les paragraphes sont présentés ainsi :
         - Titre (Page X)
         Contenu
 
         La réponse générée doit indiquer clairement la source avec le Titre et la Page.
 
         La réponse doit utiliser le format JSON suivant :
         {{
-        "{self.FLD_QUEST_OK}": 0 ou 1,
-        "{self.FLD_CHUNKS_OK}": 0 ou 1,
-        "{self.FLD_ANSWER}": une chaîne de caractères contenant la réponse
+        "{FLD_QUEST_OK}": 0 ou 1,
+        "{FLD_CHUNKS_OK}": 0 ou 1,
+        "{FLD_ANSWER}": une chaîne de caractères contenant la réponse
         }}
 
-        Le champ "{self.FLD_QUEST_OK}" vaut 0 si la question n'est pas claire, 1 sinon.
-        Le champ "{self.FLD_CHUNKS_OK}" vaut 0 si les paragraphes fournis ne permettent pas de répondre à la question, 1 sinon.
-        Le champ "{self.FLD_ANSWER}" contient la réponse."""
+        Le champ "{FLD_QUEST_OK}" vaut 0 si la question n'est pas claire, 1 sinon.
+        Le champ "{FLD_CHUNKS_OK}" vaut 0 si les paragraphes fournis ne permettent pas de répondre à la question, 1 sinon.
+        Le champ "{FLD_ANSWER}" contient la réponse."""
+
+    def get_prompt(self, question: Question, chunks: Optional[Chunks] = None) -> Prompt:
+        """
+        This Answer prompt asks for a JSON answer
+        """
+
+        # Format string to convert a chunk into a string
+        fmt_chunk_to_str: str = """- {title} (p. {page})
+        {text}"""
+
+        # Format string to join the strings representing the different chunks
+        str_joint: str = "\n\n"
+
+        # Format string to convert the string containing all the chunks to a user prompt
+        fmt_chunks_to_user_msg: str = """{chunks}
+        La question est '{question}'"""
+
+        # System prompt
+        system_msg: str = self.system
 
-        result:Prompt = Prompt()
+        result: Prompt = Prompt()
         # Compute the user prompt
-        chunks_as_list:list[str] = [
+        chunks_as_list: list[str] = [
             fmt_chunk_to_str.format(
-                title = chunk.meta['display_name'],
-                page = chunk.meta['page_number'],
-                text = chunk.text
-            ) for chunk in chunks
+                title=chunk.meta["display_name"],
+                page=chunk.meta["page_number"],
+                text=chunk.text,
+            )
+            for chunk in chunks
         ]
-        chunks_as_str:str = str_joint.join(chunks_as_list)
+        chunks_as_str: str = str_joint.join(chunks_as_list)
         result.user = fmt_chunks_to_user_msg.format(
-            chunks = chunks_as_str,
-            question = question.text
+            chunks=chunks_as_str, question=question.text
         )
 
         # Get the system prompt
         result.system = system_msg
 
         return result
 
-    def post_process(self, qa:QA, cur_obj:Answer):
+    def post_process(self, qa: QA, cur_obj: Answer):
         """
         Do JSON post processing (i.e. tries to extract correct JSON in an incorrect
         format) and finds the sources chunks quoted in the generated answer
         """
 
-        def fmt_name(a_str:str) -> str:
+        def fmt_name(a_str: str) -> str:
             """
             Internal function used to format the documents' references
             """
             result: str = unidecode(a_str)
-            rep_str:list[tuple(str, str)] = [ # type: ignore
-                ('a la page', 'p'), ('aux pages', 'p'), ('page', 'p'),
-                (' ', ''), ('.pdf', ''), ('.pptx', ''), ('.', ''), ("'", ''), ('"', ''),
-                ('(', ''), (')', ''), (',', ''),
-                ('-', ''), ]
-            for c in rep_str: result = result.replace(*c)
+            rep_str: list[tuple(str, str)] = [  # type: ignore
+                ("a la page", "p"),
+                ("aux pages", "p"),
+                ("page", "p"),
+                (" ", ""),
+                (".pdf", ""),
+                (".pptx", ""),
+                (".", ""),
+                ("'", ""),
+                ('"', ""),
+                ("(", ""),
+                (")", ""),
+                (",", ""),
+                ("-", ""),
+            ]
+            for c in rep_str:
+                result = result.replace(*c)
             return result
 
         # deprecated answer.text_field = "answer" # tells the Answer to fetch the value from the meta "answer", not the original "text" field
         # which contains the raw text returned by the LLM in this case
         json_ok: bool = False
         # test JSON and tries to extract fields if needed
-        json_ans:dict = {}
+        json_ans: dict = {}
         if not cur_obj.llm_answer:
-            logger.error(f'Nothing to post-process! LLMAnswer is None for current Answer!')
+            logger.error(
+                f"Nothing to post-process! LLMAnswer is None for current Answer!"
+            )
             return
         cur_obj.text = cur_obj.llm_answer.text
         try:
-            json_ans:dict = json.loads(cur_obj.text)
+            json_ans: dict = json.loads(cur_obj.text)
             json_ok = True
         except:
-            ans_text:str = cur_obj.text[cur_obj.text.find('{'):cur_obj.text.find('}')+1]
-            ans_text = ans_text.replace('\n', '').replace('\\','').replace('   ', ' ')
+            ans_text: str = cur_obj.text[
+                cur_obj.text.find("{") : cur_obj.text.find("}") + 1
+            ]
+            ans_text = ans_text.replace("\n", "").replace("\\", "").replace("   ", " ")
             ans_text = ans_text.replace("'}", '"}')
-            t:str = ans_text
-            p1:int = t.find(f'"{self.FLD_ANSWER}"') + len(f'"{self.FLD_ANSWER}": "')
-            p2:int = t.rfind('"')
+            t: str = ans_text
+            p1: int = t.find(f'"{self.FLD_ANSWER}"') + len(f'"{self.FLD_ANSWER}": "')
+            p2: int = t.rfind('"')
             ans_text = t[:p1] + t[p1:p2].replace('"', "'") + t[p2:]
             try:
                 json_ans = json.loads(ans_text)
                 json_ok = True
             except:
                 pass
 
         # Fills the fields with values from the returned JSON if ok
-        cur_obj.meta['json_ok'] = json_ok
-        cur_obj.meta['question_ok'] = bool(json_ans[self.FLD_QUEST_OK]) if json_ok else None
-        cur_obj.meta['chunks_ok'] = bool(json_ans[self.FLD_CHUNKS_OK]) if json_ok else None
+        cur_obj.meta["json_ok"] = json_ok
+        cur_obj.meta["question_ok"] = (
+            bool(json_ans[self.FLD_QUEST_OK]) if json_ok else None
+        )
+        cur_obj.meta["chunks_ok"] = (
+            bool(json_ans[self.FLD_CHUNKS_OK]) if json_ok else None
+        )
         cur_obj.text = json_ans[self.FLD_ANSWER] if json_ok else cur_obj.llm_answer.text
 
         # Get Answers's lang
         try:
-            lang:str = detect(cur_obj.llm_answer.text)
-            cur_obj.meta['lang'] = lang
+            lang: str = detect(cur_obj.llm_answer.text)
+            cur_obj.meta["lang"] = lang
         except:
-            cur_obj.meta['lang'] = None
+            cur_obj.meta["lang"] = None
 
         # Calc nb sources in answer even if the JSON is not formatted well
-        ans_formatted:str = fmt_name(cur_obj.llm_answer.text)
-        docs_in_chunks:dict[str, str] = {c.meta["display_name"]:
-                                            fmt_name(c.meta["display_name"])
-                                            for c in qa.chunks}
-        docs_page_in_chunks:dict[str] = {f'{c.meta["display_name"]} p.{c.meta["page_number"]}':
-                                            fmt_name(f'{c.meta["display_name"]}p.{c.meta["page_number"]}')
-                                            for c in qa.chunks}
-        cur_obj.meta['docs_in_ans'] = [orig_name for (orig_name, fmt_name)
-                                    in docs_in_chunks.items()
-                                    if fmt_name in ans_formatted]
-        cur_obj.meta['docs_and_page_in_ans'] = [orig_name for (orig_name, fmt_name)
-                                        in docs_page_in_chunks.items()
-                                        if fmt_name in ans_formatted]
+        ans_formatted: str = fmt_name(cur_obj.llm_answer.text)
+        docs_in_chunks: dict[str, str] = {
+            c.meta["display_name"]: fmt_name(c.meta["display_name"]) for c in qa.chunks
+        }
+        docs_page_in_chunks: dict[str] = {
+            f'{c.meta["display_name"]} p.{c.meta["page_number"]}': fmt_name(
+                f'{c.meta["display_name"]}p.{c.meta["page_number"]}'
+            )
+            for c in qa.chunks
+        }
+        cur_obj.meta["docs_in_ans"] = [
+            orig_name
+            for (orig_name, fmt_name) in docs_in_chunks.items()
+            if fmt_name in ans_formatted
+        ]
+        cur_obj.meta["docs_and_page_in_ans"] = [
+            orig_name
+            for (orig_name, fmt_name) in docs_page_in_chunks.items()
+            if fmt_name in ans_formatted
+        ]
```

### Comparing `ragtime-0.0.37/src/ragtime/prompters/eval/base_fr.py` & `ragtime-0.0.39/src/ragtime/prompters/eval_prompters.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,67 @@
-#!/usr/bin/env python3
+from ragtime.prompters.prompter import Prompter
 
-from ragtime.base.prompter import ( Prompter )
-
-from ragtime.expe import ( QA, Prompt, Facts, Answer, Eval )
-from ragtime.config import ( div0 )
+from ragtime.expe import QA, Prompt, Facts, Answer, Eval
+from ragtime.base import div0
 
 import re
 
 
-class PptrEvalFR(Prompter):
+class EvalPrompterFR(Prompter):
     """
     Prompt: FAITS and REPONSE - expect the REPONSE to be rewritten including the FACTS in the text
     Post_process: analyse cited factsfacts not cited, and facts invented (?)
     """
-    def get_prompt(self, answer:Answer, facts:Facts) -> Prompt:
-        result:Prompt = Prompt()
-        facts_as_str:str = '\n'.join(f'{i}. {fact.text}' for i, fact in enumerate(facts, start=1))
-        result.user = f'-- FAITS --\n{facts_as_str}\n\n-- REPONSE --\n{answer.text}'
-        result.system = """Tu dois comparer une liste numérotée de FAITS avec une REPONSE.
+
+    system:str = """Tu dois comparer une liste numérotée de FAITS avec une REPONSE.
         Tu dois reprendre exactement la REPONSE en insérant dans le texte le numéro du FAIT auquel correspond exactement le passage ou la phrase.
         Si la phrase correspond à plusieurs FAITS, indique les entre parenthèses.
         Il ne faut pas insérer le FAIT s'il est en contradiction avec le passage ou la phrase.
         Si un passage ou une phrase dans la REPONSE ne correspond à aucun FAIT il faut mettre un point d'interrogation entre parenthèses (?)
         sauf si ce passage fait référence à un emplacement dans le document, auquel cas il ne faut rien indiquer."""
+    
+    def get_prompt(self, answer: Answer, facts: Facts) -> Prompt:
+        result: Prompt = Prompt()
+        facts_as_str: str = "\n".join(
+            f"{i}. {fact.text}" for i, fact in enumerate(facts, start=1)
+        )
+        result.user = f"-- FAITS --\n{facts_as_str}\n\n-- REPONSE --\n{answer.text}"
+        result.system = self.system
         return result
 
-    def post_process(self, qa:QA, cur_obj:Eval):
-        answer:str = cur_obj.llm_answer.text if cur_obj.llm_answer.text != "[]" else ""
-        answer = answer.replace('(FAIT ', '(') # removes the word FAIT before the fact number as it is sometimes generated in the answer
+    def post_process(self, qa: QA, cur_obj: Eval):
+        answer: str = cur_obj.llm_answer.text if cur_obj.llm_answer.text != "[]" else ""
+        answer = answer.replace(
+            "(FAIT ", "("
+        )  # removes the word FAIT before the fact number as it is sometimes generated in the answer
         # get the set of facts numbers from answer
-        facts_in_answer:set[int] = set([int(s) for s in ','.join(re.findall('\([\d+,+\s+]+\)',answer)).replace('(','').replace(')','').split(',') if s])
+        facts_in_answer: set[int] = set(
+            [
+                int(s)
+                for s in ",".join(re.findall("\([\d+,+\s+]+\)", answer))
+                .replace("(", "")
+                .replace(")", "")
+                .split(",")
+                if s
+            ]
+        )
         # get the numbers in the true facts
-        true_facts:set[int] = set([int(s.text[0] if s.text[1] == '.' else s.text[:2]) for s in qa.facts if s])
-        true_facts_in_answer:set[int] = facts_in_answer & true_facts
-        true_facts_not_in_answer:set[int] = true_facts - true_facts_in_answer
+        true_facts: set[int] = set(
+            [int(s.text[0] if s.text[1] == "." else s.text[:2]) for s in qa.facts if s]
+        )
+        true_facts_in_answer: set[int] = facts_in_answer & true_facts
+        true_facts_not_in_answer: set[int] = true_facts - true_facts_in_answer
         # get the number of hallucinations (?)
-        nb_false_facts_in_answer:int = len(re.findall("\(\?\)", answer))
+        nb_false_facts_in_answer: int = len(re.findall("\(\?\)", answer))
         # compute metrics
-        precision:float = div0(len(true_facts_in_answer), len(facts_in_answer)+nb_false_facts_in_answer)
-        recall:float = div0(len(true_facts_in_answer), len(true_facts))
+        precision: float = div0(
+            len(true_facts_in_answer), len(facts_in_answer) + nb_false_facts_in_answer
+        )
+        recall: float = div0(len(true_facts_in_answer), len(true_facts))
         cur_obj.meta["precision"] = precision
         cur_obj.meta["recall"] = recall
         cur_obj.meta["hallus"] = nb_false_facts_in_answer
-        cur_obj.meta["missing"] = ', '.join(list(true_facts_not_in_answer))
+        cur_obj.meta["missing"] = ", ".join(list(true_facts_not_in_answer))
         cur_obj.meta["nb_missing"] = len(cur_obj.meta["missing"])
         cur_obj.meta["facts_in_ans"] = str(sorted(facts_in_answer))
-        cur_obj.auto = div0(2*precision*recall, precision+recall)
+        cur_obj.auto = div0(2 * precision * recall, precision + recall)
         cur_obj.text = answer
```

### Comparing `ragtime-0.0.37/src/ragtime/prompters/fact/base_fr.py` & `ragtime-0.0.39/src/ragtime/prompters/fact_prompters.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,35 @@
-#!/usr/bin/env python3
+from ragtime.prompters import Prompter
+from ragtime.expe import QA, Prompt, Facts, Fact, Answer
 
-from ragtime.base.prompter import ( Prompter )
 
-from ragtime.expe import ( QA, Prompt, Facts, Fact, Answer )
-
-class PptrFactsFR(Prompter):
+class FactPrompterFR(Prompter):
     """
     New version of Facts Prompters
     Asks for 1 to 5 facts in French
     """
-    def get_prompt(self, answer:Answer) -> Prompt:
-        result:Prompt = Prompt()
-        result.user = f'{answer.text}'
-        result.system = """Génère un minimum de phrases numérotées courtes et simples qui décrivent ce paragraphe.
+
+    system:str = """Génère un minimum de phrases numérotées courtes et simples qui décrivent ce paragraphe.
         Chaque phrase doit être indépendante et aucune phrase ne doit contenir la même information qu'une autre phrase.
         Les phrases ne doivent pas contenir de référence au document source ni à sa page.
         Les phrases doivent être compréhensibles seules et donc ne pas contenir de référence aux autres phrases ni nécessiter les autres phrases pour être comprises."""
+
+    def get_prompt(self, answer: Answer) -> Prompt:
+        result: Prompt = Prompt()
+        result.user = f"{answer.text}"
+        result.system = self.system
         return result
 
-    def post_process(self, qa:QA, cur_obj:Facts):
+    def post_process(self, qa: QA, cur_obj: Facts):
         """
         Processes the answer returned by the LLM to return a list of Fact
         Can be overriden to fit specific prompts
         """
-        temp_list:list[str] = [t.strip() for t in cur_obj.llm_answer.text.split('\n') if t.strip()]
-        temp_list = [Fact(text=f'{i}. {t}' if t[1] != '.' and t[2] != '.' else t) for i, t in enumerate(temp_list, start=1) if len(t)>2]
+        temp_list: list[str] = [
+            t.strip() for t in cur_obj.llm_answer.text.split("\n") if t.strip()
+        ]
+        temp_list = [
+            Fact(text=f"{i}. {t}" if t[1] != "." and t[2] != "." else t)
+            for i, t in enumerate(temp_list, start=1)
+            if len(t) > 2
+        ]
         cur_obj.items = temp_list
```

### Comparing `ragtime-0.0.37/src/ragtime/text_generators/answer_generator.py` & `ragtime-0.0.39/src/ragtime/generators/answer_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,59 +1,49 @@
-#!/usr/bin/env python3
-
-from ragtime.base.text_generator import (
-    TextGenerator,
-    Retriever,
-    StartFrom,
-)
-
-from ragtime.base.llm import ( LLM )
-
-from ragtime.expe import ( Answer, Answers, QA ) # TODO: This double name can be miss leading
-from ragtime.config import ( logger )
-
-from typing import ( Optional )
+from ragtime.generators import TextGenerator
+from ragtime.retrievers.retriever import Retriever
+from ragtime.llms import LLM
+from ragtime.expe import QA, Answer, Answers, StartFrom
+from ragtime.config import logger
+from typing import Optional
 
 class AnsGenerator(TextGenerator):
-
     """
     Object to write answers in the expe
     To use a Retriever, first implement one and give it as parameter when constructing the object
     Besides, subclasses can override the following methods:
     - post_process : to add "meta" fields based on the llm_answer
     Prompts can be changed in the LLM subclass
     """
-    retriever:Optional[Retriever] = None
 
-    def __init__(self, retriever:Retriever = None, llms:list[LLM] = None):
+    retriever: Optional[Retriever] = None
+
+    def __init__(self, llms: list[LLM] = None, retriever: Retriever = None):
         """
         Args
             retriever(Retriever): the retriever to used to get the chunks before generating the answer - can be None if no Retriever is used
             llm_names(list[str]): a list of LLM names to be instantiated as LiteLLMs - the names come from https://litellm.vercel.app/docs/providers
             llms(list[LLM]) : list of LLM objects
             Either llms or llm_names or both can be used but at least one must be provided
         """
         super().__init__(llms=llms)
         if retriever:
             self.retriever = retriever
 
-
-    def write_chunks(self, qa:QA):
+    def write_chunks(self, qa: QA):
         """Write chunks in the current qa if a Retriever has been given when creating the object. Ignore otherwise"""
         if self.retriever:
             qa.chunks.empty()
             self.retriever.retrieve(qa=qa)
 
-
     async def gen_for_qa(
-            self,
-            qa:QA,
-            start_from:StartFrom=StartFrom.beginning,
-            b_missing_only:bool=False,
-            only_llms:list[str] = None
+        self,
+        qa: QA,
+        start_from: StartFrom = StartFrom.beginning,
+        b_missing_only: bool = False,
+        only_llms: list[str] = None,
     ):
         """
         Args
         - qa (QA) : the QA (expe row) to work on
         - start_from : a value in the StartFrom Enum, among:
             - beginning: retrieve chunks (if a Retriever is given, ignore otherwise), compute prompts,
         computer llm answers, compute meta on answers
@@ -62,51 +52,62 @@
             - post_process: reuse chunks, prompts and llm answers, compute meta only
         - b_missing_only: True to generate LLM Answers only when the Answer object has no "llm_answer"
         Useful to complete a previous experiment where all the Answers have not been generated (happens sometimes due
         to external server failures)
         - only_llms: restrict the llms to be computed again - used in conjunction with start_from - if start from beginning, chunks or prompts, compute prompts and llm answers for the list only - if start from llm, recompute llm answers for these llm only - has not effect if start
         """
         # Get chunks -> fills the Chunks in the QA
-        logger.prefix += '[AnsGen]'
+        logger.prefix += "[AnsGen]"
         if self.retriever:
             # Compute chunks if there are not any or there are some and user asked to start à Chunks step or before and did not mention to
             # complete only the missing ones
-            if (not qa.chunks) or (qa.chunks and start_from <= StartFrom.chunks and not b_missing_only):
-                logger.info(f'Compute chunks')
+            if (not qa.chunks) or (
+                qa.chunks and start_from <= StartFrom.chunks and not b_missing_only
+            ):
+                logger.info(f"Compute chunks")
                 self.write_chunks(qa=qa)
-            else: # otherwise reuse the chunks already in the QA object
-                logger.info(f'Reuse existing chunks')
+            else:  # otherwise reuse the chunks already in the QA object
+                logger.info(f"Reuse existing chunks")
 
         # Generation loop, for each LLM -> fills the Answers in the QA
         # Get list of LLMs sto actually use, if only_llms defined
-        new_answers:Answer = Answers()
-        actual_llms:list[LLM] = [l for l in self.llms if l in only_llms] if only_llms else self.llms
-        original_prefix:str = logger.prefix
+        new_answers: Answer = Answers()
+        actual_llms: list[LLM] = (
+            [l for l in self.llms if l in only_llms] if only_llms else self.llms
+        )
+        original_prefix: str = logger.prefix
 
         for llm in actual_llms:
-            logger.prefix = f'{original_prefix}[{llm.name}]'
-            logger.info(f'* Start with LLM')
+            logger.prefix = f"{original_prefix}[{llm.name}]"
+            logger.info(f"* Start with LLM")
 
             # Get existing Answer if any
-            prev_ans:Optional[Answer] = [a for a in qa.answers if a.llm_answer and (a.llm_answer.name == llm.name or a.llm_answer.full_name == llm.name)]
+            prev_ans: Optional[Answer] = [
+                a
+                for a in qa.answers
+                if a.llm_answer
+                and (
+                    a.llm_answer.name == llm.name or a.llm_answer.full_name == llm.name
+                )
+            ]
             if prev_ans:
-                prev_ans = prev_ans[0] # prev_ans is None if no previous Answer has been generated for the current LLM
-                logger.debug(f'An Answer has already been generated with this LLM')
+                prev_ans = prev_ans[0]  # prev_ans is None if no previous Answer has been generated for the current LLM
+                logger.debug(f"An Answer has already been generated with this LLM")
             else:
                 prev_ans = None
 
             # Get Answer from LLM
-            ans:Answer = await llm.generate(
-                cur_obj = Answer(),
-                prev_obj = prev_ans,
-                qa = qa,
-                start_from = start_from,
-                b_missing_only = b_missing_only,
-                question = qa.question,
-                chunks = qa.chunks
+            ans: Answer = await llm.generate(
+                cur_obj=Answer(),
+                prev_obj=prev_ans,
+                qa=qa,
+                start_from=start_from,
+                b_missing_only=b_missing_only,
+                question=qa.question,
+                chunks=qa.chunks,
             )
 
             # get previous human eval if any
             if prev_ans and prev_ans.eval:
                 ans.eval.human = prev_ans.eval.human
 
             new_answers.append(ans)
```

### Comparing `ragtime-0.0.37/src/ragtime/text_generators/eval_generator.py` & `ragtime-0.0.39/src/ragtime/generators/eval_generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,108 +1,128 @@
-#!/usr/bin/env python3
+from ragtime.generators.text_generator import *
+from ragtime.llms import LLM
+from ragtime.expe import StartFrom, QA, Eval, Facts
+from ragtime.base import RagtimeException
+from ragtime.config import logger, UNKOWN_LLM
 
-from ragtime.base.text_generator import (
-    TextGenerator,
-    StartFrom,
-)
-
-from ragtime.base.llm import ( LLM )
-
-from ragtime.expe import ( Eval, Facts, QA )
-from ragtime.config import ( RagtimeException, logger , UNKOWN_LLM)
 
 class EvalGenerator(TextGenerator):
     """
     Generate Eval from Answers and Facts.
     For a given QA, send the Answer and the Facts to the LLM to get the prompt back
     The default prompt returns all the valid facts given an answer, i.e. 1 prompt -> 1 Eval
     That could be overridden to have e.g. 1 prompt per Fact, i.e. N prompt -> 1 Eval
     The conversion between the LLM answer and the Eval is made in post_process
     """
 
     async def gen_for_qa(
-            self,
-            qa:QA,
-            start_from:StartFrom=StartFrom.beginning,
-            b_missing_only:bool=False,
-            only_llms:list[str] = None
+        self,
+        qa: QA,
+        start_from: StartFrom = StartFrom.beginning,
+        b_missing_only: bool = False,
+        only_llms: list[str] = None,
     ):
         """
         Create Eval for each QA where Facts are available
         """
 
         if len(qa.answers) == 0:
-            logger.error(f'No Answers, cannot generate Evals'); return
+            logger.error(f"No Answers, cannot generate Evals")
+            return
         if len(qa.facts) == 0:
-            logger.error(f'No Facts, cannot generate Evals'); return
+            logger.error(f"No Facts, cannot generate Evals")
+            return
 
         # Eval loop
-        logger.prefix += f'[EvalGen][{self.llm.name}]'
+        logger.prefix += f"[EvalGen][{self.llm.name}]"
         for ans in (a for a in qa.answers if a.text):
-            llm_name:str = ans.llm_answer.name if ans.llm_answer else UNKOWN_LLM
-            if only_llms and llm_name not in only_llms and llm_name != UNKOWN_LLM: continue
+            llm_name: str = ans.llm_answer.name if ans.llm_answer else UNKOWN_LLM
+            if only_llms and llm_name not in only_llms and llm_name != UNKOWN_LLM:
+                continue
             logger.debug(f'Generate Eval for answer generated with "{llm_name}"')
-            prev_eval:Eval = ans.eval
+            prev_eval: Eval = ans.eval
 
-            #2.a. and 2.b : prompt generation + Text generation with LLM
+            # 2.a. and 2.b : prompt generation + Text generation with LLM
             ans.eval = await self.llm.generate(
                 cur_obj=Eval(),
                 prev_obj=prev_eval,
-                qa=qa, start_from=start_from,
+                qa=qa,
+                start_from=start_from,
                 b_missing_only=b_missing_only,
-                answer=ans, facts=qa.facts
+                answer=ans,
+                facts=qa.facts,
             )
 
             # save previous human eval if any
-            if prev_eval and prev_eval.human: ans.eval.human = prev_eval.human
+            if prev_eval and prev_eval.human:
+                ans.eval.human = prev_eval.human
+
 
 class TwoFactsEvalGenerator(TextGenerator):
     """
     Generate Eval from Answers and Facts. Converts first the Answer to a list of Facts and
     perform evaluation
     """
 
-    def __init__(self, llms:list[LLM] = None):
+    def __init__(self, llms: list[LLM] = None):
         super().__init__(llms=llms)
         if len(self.llms) < 2:
-            raise RagtimeException("""Need at least 2 LLMs to run this generator!
+            raise RagtimeException(
+                """Need at least 2 LLMs to run this generator!
                                    1st LLM is used to generate Facts from the Answer.
-                                   2nd LLM is used to generate Eval from the golden Facts and the Facts from the Answer.""")
+                                   2nd LLM is used to generate Eval from the golden Facts and the Facts from the Answer."""
+            )
 
     async def gen_for_qa(
-            self,
-            qa:QA,
-            start_from:StartFrom=StartFrom.beginning,
-            b_missing_only:bool=False
+        self,
+        qa: QA,
+        start_from: StartFrom = StartFrom.beginning,
+        b_missing_only: bool = False,
     ):
         """
         Create Eval for each QA where Facts are available
         """
 
         if len(qa.answers) == 0:
-            logger.error(f'No Answers, cannot generate Evals'); return
+            logger.error(f"No Answers, cannot generate Evals")
+            return
         if len(qa.facts) == 0:
-            logger.error(f'No Facts, cannot generate Evals'); return
+            logger.error(f"No Facts, cannot generate Evals")
+            return
 
         # Eval loop
         for ans in (a for a in qa.answers if a.text):
-            llm_name:str = ans.llm_answer.name if ans.llm_answer else "unkown LLM (manual ?)"
+            llm_name: str = (
+                ans.llm_answer.name if ans.llm_answer else "unkown LLM (manual ?)"
+            )
             logger.debug(f'Generate Facts for answer generated with "{llm_name}"')
-            prev_eval:Eval = ans.eval
+            prev_eval: Eval = ans.eval
 
             # Use 1st LLM to generate facts from the Answer
-            ans_facts:Facts = await self.llms[0].generate(cur_obj=Facts(), prev_obj=None,
-                                    qa=qa, start_from=start_from,
-                                    b_missing_only=b_missing_only,
-                                    answer=ans)
+            ans_facts: Facts = await self.llms[0].generate(
+                cur_obj=Facts(),
+                prev_obj=None,
+                qa=qa,
+                start_from=start_from,
+                b_missing_only=b_missing_only,
+                answer=ans,
+            )
 
             # Use 2nd LLM to generate Eval
-            logger.debug(f'Then generate Eval using answer facts and gold facts')
-            cur_eval:Eval = Eval()
-            cur_eval.meta['answer_facts'] = [af.text for af in ans_facts] # stores the answer's facts in the current eval
-            ans.eval = await self.llms[1].generate(cur_obj=cur_eval, prev_obj=prev_eval,
-                                    qa=qa, start_from=start_from,
-                                    b_missing_only=b_missing_only,
-                                    answer_facts=ans_facts, gold_facts=qa.facts)
+            logger.debug(f"Then generate Eval using answer facts and gold facts")
+            cur_eval: Eval = Eval()
+            cur_eval.meta["answer_facts"] = [
+                af.text for af in ans_facts
+            ]  # stores the answer's facts in the current eval
+            ans.eval = await self.llms[1].generate(
+                cur_obj=cur_eval,
+                prev_obj=prev_eval,
+                qa=qa,
+                start_from=start_from,
+                b_missing_only=b_missing_only,
+                answer_facts=ans_facts,
+                gold_facts=qa.facts,
+            )
 
             # save previous human eval if any
-            if prev_eval and prev_eval.human: ans.eval.human = prev_eval.human
+            if prev_eval and prev_eval.human:
+                ans.eval.human = prev_eval.human
```

### Comparing `ragtime-0.0.37/src/ragtime/text_generators/fact_generator.py` & `ragtime-0.0.39/src/ragtime/generators/fact_generator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,47 @@
-#!/usr/bin/env python3
-
-from ragtime.base.text_generator import (
-    TextGenerator,
-    StartFrom,
-)
-
-from ragtime.expe import ( Answer, Facts, QA )
-from ragtime.config import ( logger )
+from ragtime.expe import StartFrom, QA, Answer, Facts
+from ragtime.generators import TextGenerator
+from ragtime.config import logger
 
 class FactGenerator(TextGenerator):
     """
     Generate Facts from existing Answers
     """
+
     async def gen_for_qa(
-            self,
-            qa:QA,
-            start_from:StartFrom=StartFrom.beginning,
-            b_missing_only:bool=False,
-            only_llms:list[str] = None
+        self,
+        qa: QA,
+        start_from: StartFrom = StartFrom.beginning,
+        b_missing_only: bool = False,
+        only_llms: list[str] = None,
     ):
         """
         Create Facts based on the first Answer in the QA having human Eval equals 1
         """
 
-        ans:Answer = next((a for a in qa.answers if a.eval and a.eval.human == 1.0))
+        ans: Answer = next((a for a in qa.answers if a.eval and a.eval.human == 1.0))
         if not ans:
-            logger.debug(f'No fact has been generated since no answer has been validated (human=1.0) for this question')
+            logger.debug(
+                f"No fact has been generated since no answer has been validated (human=1.0) for this question"
+            )
             return
 
-        logger.prefix += f'[FactGen][{self.llm.name}]'
-        model_str:str = f" associated with answer from model {ans.llm_answer.full_name}" if ans.llm_answer else ""
-        logger.info(f'Generate Facts since it has a human validated answer (eval.human == 1.0){model_str}')
-        prev_facts:Facts = qa.facts
+        logger.prefix += f"[FactGen][{self.llm.name}]"
+        model_str: str = (
+            f" associated with answer from model {ans.llm_answer.full_name}"
+            if ans.llm_answer
+            else ""
+        )
+        logger.info(
+            f"Generate Facts since it has a human validated answer (eval.human == 1.0){model_str}"
+        )
+        prev_facts: Facts = qa.facts
 
-        #2.a. and 2.b : prompt generation + Text generation with LLM
+        # 2.a. and 2.b : prompt generation + Text generation with LLM
         qa.facts = await self.llm.generate(
-            cur_obj = Facts(),
-            prev_obj = prev_facts,
-            qa = qa,
-            start_from = start_from,
-            b_missing_only = b_missing_only,
-            answer = ans
+            cur_obj=Facts(),
+            prev_obj=prev_facts,
+            qa=qa,
+            start_from=start_from,
+            b_missing_only=b_missing_only,
+            answer=ans,
         )
```

### Comparing `ragtime-0.0.37/tests/full_test.py` & `ragtime-0.0.39/tests/full_test.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.37/tests/run_tests.py` & `ragtime-0.0.39/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.37/tests/test_quest.json` & `ragtime-0.0.39/tests/test_quest.json`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.37/.gitignore` & `ragtime-0.0.39/.gitignore`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.37/LICENSE` & `ragtime-0.0.39/LICENSE`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.37/README.md` & `ragtime-0.0.39/README.md`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.37/pyproject.toml` & `ragtime-0.0.39/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ragtime"
-version = "0.0.37"
+version = "0.0.39"
 
 authors = [
   { name="Gilles Moyse", email="gilles@recital.ai" },
 ]
 maintainers = [
   { name="reciTAL", email="ragtime@recital.ai" },
 ]
@@ -25,8 +25,8 @@
 keywords = ["RAG", "LLM", "Evaluation"]
 dependencies = ['requests', 'retry', 'pathlib', 'openpyxl', 'langdetect',
 'pydantic', 'jinja2', 'tabulate', 'unidecode', 'litellm', 'setenv', 'py_setenv', 'lazy_import',
 'asyncio', 'toml']
 
 [project.urls]
 Homepage = "https://github.com/recitalAI/ragtime-package"
-Issues = "https://github.com/recitalAI/ragtime-package/issues"
+Issues = "https://github.com/recitalAI/ragtime-package/issues"
```

### Comparing `ragtime-0.0.37/PKG-INFO` & `ragtime-0.0.39/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragtime
-Version: 0.0.37
+Version: 0.0.39
 Summary: Ragtime 🎹 is an LLMOps framework to automatically evaluate Retrieval Augmented Generation (RAG) systems and compare different RAGs / LLMs
 Project-URL: Homepage, https://github.com/recitalAI/ragtime-package
 Project-URL: Issues, https://github.com/recitalAI/ragtime-package/issues
 Author-email: Gilles Moyse <gilles@recital.ai>
 Maintainer-email: reciTAL <ragtime@recital.ai>
 License: MIT License
```

