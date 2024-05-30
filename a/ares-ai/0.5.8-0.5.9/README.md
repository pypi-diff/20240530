# Comparing `tmp/ares_ai-0.5.8.tar.gz` & `tmp/ares_ai-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ares_ai-0.5.8.tar", last modified: Tue May 21 12:11:56 2024, max compression
+gzip compressed data, was "ares_ai-0.5.9.tar", last modified: Thu May 30 03:20:40 2024, max compression
```

## Comparing `ares_ai-0.5.8.tar` & `ares_ai-0.5.9.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-21 12:11:56.356146 ares_ai-0.5.8/
--rw-rw-rw-   0 manihani (23549) future   (20099)     5118 2024-05-21 10:25:44.000000 ares_ai-0.5.8/.gitignore
--rw-rw-rw-   0 manihani (23549) future   (20099)      268 2024-04-22 03:39:34.000000 ares_ai-0.5.8/CHANGELOG.md
--rw-rw-rw-   0 manihani (23549) future   (20099)    11357 2024-01-08 23:19:52.000000 ares_ai-0.5.8/LICENSE
--rw-rw-rw-   0 manihani (23549) future   (20099)       51 2024-04-25 23:18:28.000000 ares_ai-0.5.8/MANIFEST.in
--rw-r--r--   0 manihani (23549) future   (20099)    28486 2024-05-21 12:11:56.355147 ares_ai-0.5.8/PKG-INFO
--rw-rw-rw-   0 manihani (23549) future   (20099)    12916 2024-05-21 10:19:09.000000 ares_ai-0.5.8/README.md
-drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-21 12:11:55.671177 ares_ai-0.5.8/ares/
-drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-21 12:11:55.729175 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/
--rw-rw-rw-   0 manihani (23549) future   (20099)    10726 2024-05-15 09:28:04.000000 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/Filter_Synthetic_Queries.py
--rw-rw-rw-   0 manihani (23549) future   (20099)    39458 2024-05-20 03:54:50.000000 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/General_Binary_Classifier.py
--rw-rw-rw-   0 manihani (23549) future   (20099)    26352 2024-05-16 09:44:16.000000 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/Generate_Synthetic_Queries_and_Answers.py
--rw-rw-rw-   0 manihani (23549) future   (20099)    27757 2024-05-15 04:45:07.000000 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/LLM_Generation_Functions.py
--rw-rw-rw-   0 manihani (23549) future   (20099)        0 2024-04-22 03:39:34.000000 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__init__.py
-drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-21 12:11:55.855169 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/
--rw-rw-rw-   0 manihani (23549) future   (20099)     7375 2024-05-15 22:43:28.000000 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     9231 2024-05-07 02:24:59.000000 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-311.pyc
--rw-r--r--   0 manihani (23549) future   (20099)    27821 2024-05-20 22:16:50.000000 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    37386 2024-05-07 02:24:59.000000 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    19424 2024-05-16 10:41:36.000000 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    21777 2024-05-07 02:24:37.000000 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    18303 2024-05-15 07:02:35.000000 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    17731 2024-05-07 02:24:59.000000 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      159 2024-04-24 01:00:10.000000 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      175 2024-05-07 02:24:37.000000 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     2243 2024-04-24 05:41:16.000000 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/pytorchtools.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     2109 2024-04-22 03:39:34.000000 ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/pytorchtools.py
-drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-21 12:11:55.951165 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/
--rw-rw-rw-   0 manihani (23549) future   (20099)    55776 2024-05-15 03:08:44.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/Evaluation_Functions.py
--rw-rw-rw-   0 manihani (23549) future   (20099)    65743 2024-05-21 11:18:53.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/LLMJudge_RAG_Compared_Scoring.py
--rw-rw-rw-   0 manihani (23549) future   (20099)       36 2024-05-18 12:00:35.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/Prepare_FinanceBench.py
--rw-rw-rw-   0 manihani (23549) future   (20099)    18046 2024-04-22 03:39:34.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/Prepare_KILT_Dataset.py
--rw-rw-rw-   0 manihani (23549) future   (20099)     7091 2024-04-30 23:25:14.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/Prepare_SuperGLUE_Datasets.py
--rw-rw-rw-   0 manihani (23549) future   (20099)        0 2024-04-22 03:39:34.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__init__.py
-drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-21 12:11:56.109158 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/
--rw-rw-rw-   0 manihani (23549) future   (20099)    31119 2024-05-15 03:09:09.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    32115 2024-05-07 02:30:43.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-311.pyc
--rw-r--r--   0 manihani (23549) future   (20099)    39819 2024-05-21 11:24:33.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    49640 2024-05-07 02:25:02.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     7856 2024-04-24 01:01:09.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    19694 2024-05-07 02:25:08.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-311.pyc
--rw-r--r--   0 manihani (23549) future   (20099)     4250 2024-04-30 23:25:39.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     9532 2024-05-07 02:25:08.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      158 2024-04-24 01:01:00.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      174 2024-05-07 02:25:02.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     5437 2024-01-20 22:01:06.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/ares.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      172 2024-05-07 22:44:26.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/counter.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)    17791 2024-05-21 10:44:15.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    19175 2024-05-07 02:25:02.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      494 2024-01-20 21:58:30.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/test.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    21593 2024-05-21 10:43:03.000000 ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/ppi.py
--rw-rw-rw-   0 manihani (23549) future   (20099)       22 2024-04-22 03:39:34.000000 ares_ai-0.5.8/ares/__init__.py
--rw-r--r--   0 manihani (23549) future   (20099)      152 2024-03-25 00:40:39.000000 ares_ai-0.5.8/ares/__init__.pyc
-drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-21 12:11:56.239152 ares_ai-0.5.8/ares/__pycache__/
--rw-rw-rw-   0 manihani (23549) future   (20099)      166 2024-04-24 01:00:10.000000 ares_ai-0.5.8/ares/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      196 2024-05-07 02:24:37.000000 ares_ai-0.5.8/ares/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 manihani (23549) future   (20099)     8166 2024-05-21 06:03:02.000000 ares_ai-0.5.8/ares/__pycache__/ares.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    10977 2024-05-07 02:55:57.000000 ares_ai-0.5.8/ares/__pycache__/ares.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     5615 2024-05-15 22:43:28.000000 ares_ai-0.5.8/ares/__pycache__/binary_classifier.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     7124 2024-05-07 02:24:59.000000 ares_ai-0.5.8/ares/__pycache__/binary_classifier.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      371 2024-04-24 01:01:09.000000 ares_ai-0.5.8/ares/__pycache__/kilt_filter.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      469 2024-05-07 02:25:08.000000 ares_ai-0.5.8/ares/__pycache__/kilt_filter.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     1908 2024-05-13 22:37:10.000000 ares_ai-0.5.8/ares/__pycache__/prompts.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)     4799 2024-05-21 06:06:29.000000 ares_ai-0.5.8/ares/__pycache__/rag_scoring.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     3941 2024-05-07 02:25:02.000000 ares_ai-0.5.8/ares/__pycache__/rag_scoring.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      356 2024-04-24 01:01:09.000000 ares_ai-0.5.8/ares/__pycache__/superglue_filter.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      442 2024-05-07 02:25:08.000000 ares_ai-0.5.8/ares/__pycache__/superglue_filter.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     4330 2024-05-16 10:41:36.000000 ares_ai-0.5.8/ares/__pycache__/synthetic_generator.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     3518 2024-05-07 02:24:37.000000 ares_ai-0.5.8/ares/__pycache__/synthetic_generator.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     9413 2024-05-15 09:11:08.000000 ares_ai-0.5.8/ares/__pycache__/ues_idp.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    10990 2024-05-07 03:18:13.000000 ares_ai-0.5.8/ares/__pycache__/ues_idp.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    11647 2024-05-21 06:01:01.000000 ares_ai-0.5.8/ares/ares.py
-drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-21 12:11:56.316148 ares_ai-0.5.8/ares/ares_ai.egg-info/
--rw-r--r--   0 manihani (23549) future   (20099)    26304 2024-04-05 05:20:31.000000 ares_ai-0.5.8/ares/ares_ai.egg-info/PKG-INFO
--rw-rw-rw-   0 manihani (23549) future   (20099)        0 2024-04-05 05:20:31.000000 ares_ai-0.5.8/ares/ares_ai.egg-info/SOURCES.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)        1 2024-04-05 05:20:31.000000 ares_ai-0.5.8/ares/ares_ai.egg-info/dependency_links.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)       43 2024-04-05 05:20:31.000000 ares_ai-0.5.8/ares/ares_ai.egg-info/entry_points.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)      627 2024-04-05 05:20:31.000000 ares_ai-0.5.8/ares/ares_ai.egg-info/requires.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)        5 2024-04-05 05:20:31.000000 ares_ai-0.5.8/ares/ares_ai.egg-info/top_level.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)     8374 2024-05-15 22:27:43.000000 ares_ai-0.5.8/ares/binary_classifier.py
--rw-rw-rw-   0 manihani (23549) future   (20099)      154 2024-04-22 03:39:34.000000 ares_ai-0.5.8/ares/kilt_filter.py
--rw-rw-rw-   0 manihani (23549) future   (20099)     1862 2024-05-13 05:25:48.000000 ares_ai-0.5.8/ares/prompts.py
--rw-rw-rw-   0 manihani (23549) future   (20099)     8433 2024-05-21 06:06:15.000000 ares_ai-0.5.8/ares/rag_scoring.py
--rw-rw-rw-   0 manihani (23549) future   (20099)      134 2024-04-22 03:39:34.000000 ares_ai-0.5.8/ares/superglue_filter.py
--rw-rw-rw-   0 manihani (23549) future   (20099)     5844 2024-05-16 09:46:01.000000 ares_ai-0.5.8/ares/synthetic_generator.py
--rw-rw-rw-   0 manihani (23549) future   (20099)    15573 2024-05-15 09:10:54.000000 ares_ai-0.5.8/ares/ues_idp.py
-drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-21 12:11:56.349147 ares_ai-0.5.8/ares_ai.egg-info/
--rw-r--r--   0 manihani (23549) future   (20099)    28486 2024-05-21 12:11:47.000000 ares_ai-0.5.8/ares_ai.egg-info/PKG-INFO
--rw-rw-rw-   0 manihani (23549) future   (20099)     4238 2024-05-21 12:11:55.000000 ares_ai-0.5.8/ares_ai.egg-info/SOURCES.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)        1 2024-05-21 12:11:47.000000 ares_ai-0.5.8/ares_ai.egg-info/dependency_links.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)       43 2024-05-21 12:11:47.000000 ares_ai-0.5.8/ares_ai.egg-info/entry_points.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)      698 2024-05-21 12:11:47.000000 ares_ai-0.5.8/ares_ai.egg-info/requires.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)        5 2024-05-21 12:11:47.000000 ares_ai-0.5.8/ares_ai.egg-info/top_level.txt
-drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-21 12:11:56.343147 ares_ai-0.5.8/checkpoints/
--rw-rw-rw-   0 manihani (23549) future   (20099)       71 2024-04-22 03:39:34.000000 ares_ai-0.5.8/checkpoints/.gitignore
--rw-rw-rw-   0 manihani (23549) future   (20099)     2929 2024-05-21 10:28:26.000000 ares_ai-0.5.8/pyproject.toml
--rw-rw-rw-   0 manihani (23549) future   (20099)     5082 2024-05-19 01:32:03.000000 ares_ai-0.5.8/requirements.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)       93 2024-05-21 12:11:56.359146 ares_ai-0.5.8/setup.cfg
-drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-21 12:11:56.346147 ares_ai-0.5.8/tests/
--rw-rw-rw-   0 manihani (23549) future   (20099)       71 2024-04-22 03:39:53.000000 ares_ai-0.5.8/tests/.gitignore
+drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-30 03:20:40.367965 ares_ai-0.5.9/
+-rw-rw-rw-   0 manihani (23549) future   (20099)     5118 2024-05-21 10:25:44.000000 ares_ai-0.5.9/.gitignore
+-rw-rw-rw-   0 manihani (23549) future   (20099)      268 2024-04-22 03:39:34.000000 ares_ai-0.5.9/CHANGELOG.md
+-rw-rw-rw-   0 manihani (23549) future   (20099)    11357 2024-01-08 23:19:52.000000 ares_ai-0.5.9/LICENSE
+-rw-rw-rw-   0 manihani (23549) future   (20099)       51 2024-04-25 23:18:28.000000 ares_ai-0.5.9/MANIFEST.in
+-rw-r--r--   0 manihani (23549) future   (20099)    28521 2024-05-30 03:20:40.366965 ares_ai-0.5.9/PKG-INFO
+-rw-rw-rw-   0 manihani (23549) future   (20099)    12913 2024-05-30 02:01:56.000000 ares_ai-0.5.9/README.md
+drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-30 03:20:40.234971 ares_ai-0.5.9/ares/
+drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-30 03:20:40.245971 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/
+-rw-rw-rw-   0 manihani (23549) future   (20099)    10726 2024-05-15 09:28:04.000000 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/Filter_Synthetic_Queries.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)    39458 2024-05-20 03:54:50.000000 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/General_Binary_Classifier.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)    26352 2024-05-16 09:44:16.000000 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/Generate_Synthetic_Queries_and_Answers.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)    27757 2024-05-15 04:45:07.000000 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/LLM_Generation_Functions.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)        0 2024-04-22 03:39:34.000000 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__init__.py
+drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-30 03:20:40.265970 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/
+-rw-rw-rw-   0 manihani (23549) future   (20099)     7375 2024-05-15 22:43:28.000000 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     9231 2024-05-07 02:24:59.000000 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-311.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)    27821 2024-05-20 22:16:50.000000 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    37386 2024-05-07 02:24:59.000000 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    19424 2024-05-16 10:41:36.000000 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    21777 2024-05-07 02:24:37.000000 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    18303 2024-05-15 07:02:35.000000 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    17731 2024-05-07 02:24:59.000000 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      159 2024-04-24 01:00:10.000000 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      175 2024-05-07 02:24:37.000000 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     2243 2024-04-24 05:41:16.000000 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/pytorchtools.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     2109 2024-04-22 03:39:34.000000 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/pytorchtools.py
+drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-30 03:20:40.278969 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/
+-rw-rw-rw-   0 manihani (23549) future   (20099)    55776 2024-05-15 03:08:44.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/Evaluation_Functions.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)    65867 2024-05-30 03:04:39.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/LLMJudge_RAG_Compared_Scoring.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)       36 2024-05-18 12:00:35.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/Prepare_FinanceBench.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)    18046 2024-04-22 03:39:34.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/Prepare_KILT_Dataset.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)     7091 2024-04-30 23:25:14.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/Prepare_SuperGLUE_Datasets.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)        0 2024-04-22 03:39:34.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__init__.py
+drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-30 03:20:40.306968 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/
+-rw-rw-rw-   0 manihani (23549) future   (20099)    31119 2024-05-15 03:09:09.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    32115 2024-05-07 02:30:43.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-311.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)    39869 2024-05-30 03:04:51.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    49640 2024-05-07 02:25:02.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     7856 2024-04-24 01:01:09.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    19694 2024-05-07 02:25:08.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-311.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)     4250 2024-04-30 23:25:39.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     9532 2024-05-07 02:25:08.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      158 2024-04-24 01:01:00.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      174 2024-05-07 02:25:02.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     5437 2024-01-20 22:01:06.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/ares.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      172 2024-05-07 22:44:26.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/counter.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)    17791 2024-05-21 10:44:15.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    19175 2024-05-07 02:25:02.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      494 2024-01-20 21:58:30.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/test.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    21593 2024-05-21 10:43:03.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/ppi.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)       22 2024-04-22 03:39:34.000000 ares_ai-0.5.9/ares/__init__.py
+-rw-r--r--   0 manihani (23549) future   (20099)      152 2024-03-25 00:40:39.000000 ares_ai-0.5.9/ares/__init__.pyc
+drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-30 03:20:40.335966 ares_ai-0.5.9/ares/__pycache__/
+-rw-rw-rw-   0 manihani (23549) future   (20099)      166 2024-04-24 01:00:10.000000 ares_ai-0.5.9/ares/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      196 2024-05-07 02:24:37.000000 ares_ai-0.5.9/ares/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)     8166 2024-05-21 06:03:02.000000 ares_ai-0.5.9/ares/__pycache__/ares.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    10977 2024-05-07 02:55:57.000000 ares_ai-0.5.9/ares/__pycache__/ares.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     5615 2024-05-15 22:43:28.000000 ares_ai-0.5.9/ares/__pycache__/binary_classifier.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     7124 2024-05-07 02:24:59.000000 ares_ai-0.5.9/ares/__pycache__/binary_classifier.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      371 2024-04-24 01:01:09.000000 ares_ai-0.5.9/ares/__pycache__/kilt_filter.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      469 2024-05-07 02:25:08.000000 ares_ai-0.5.9/ares/__pycache__/kilt_filter.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     1908 2024-05-13 22:37:10.000000 ares_ai-0.5.9/ares/__pycache__/prompts.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     4836 2024-05-30 02:34:05.000000 ares_ai-0.5.9/ares/__pycache__/rag_scoring.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     3941 2024-05-07 02:25:02.000000 ares_ai-0.5.9/ares/__pycache__/rag_scoring.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      356 2024-04-24 01:01:09.000000 ares_ai-0.5.9/ares/__pycache__/superglue_filter.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      442 2024-05-07 02:25:08.000000 ares_ai-0.5.9/ares/__pycache__/superglue_filter.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     4330 2024-05-16 10:41:36.000000 ares_ai-0.5.9/ares/__pycache__/synthetic_generator.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     3518 2024-05-07 02:24:37.000000 ares_ai-0.5.9/ares/__pycache__/synthetic_generator.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     9413 2024-05-15 09:11:08.000000 ares_ai-0.5.9/ares/__pycache__/ues_idp.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    10990 2024-05-07 03:18:13.000000 ares_ai-0.5.9/ares/__pycache__/ues_idp.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    11647 2024-05-21 06:01:01.000000 ares_ai-0.5.9/ares/ares.py
+drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-30 03:20:40.345966 ares_ai-0.5.9/ares/ares_ai.egg-info/
+-rw-r--r--   0 manihani (23549) future   (20099)    26304 2024-04-05 05:20:31.000000 ares_ai-0.5.9/ares/ares_ai.egg-info/PKG-INFO
+-rw-rw-rw-   0 manihani (23549) future   (20099)        0 2024-04-05 05:20:31.000000 ares_ai-0.5.9/ares/ares_ai.egg-info/SOURCES.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)        1 2024-04-05 05:20:31.000000 ares_ai-0.5.9/ares/ares_ai.egg-info/dependency_links.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)       43 2024-04-05 05:20:31.000000 ares_ai-0.5.9/ares/ares_ai.egg-info/entry_points.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)      627 2024-04-05 05:20:31.000000 ares_ai-0.5.9/ares/ares_ai.egg-info/requires.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)        5 2024-04-05 05:20:31.000000 ares_ai-0.5.9/ares/ares_ai.egg-info/top_level.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)     8374 2024-05-15 22:27:43.000000 ares_ai-0.5.9/ares/binary_classifier.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)      154 2024-04-22 03:39:34.000000 ares_ai-0.5.9/ares/kilt_filter.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)     1862 2024-05-13 05:25:48.000000 ares_ai-0.5.9/ares/prompts.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)     8523 2024-05-30 02:06:37.000000 ares_ai-0.5.9/ares/rag_scoring.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)      134 2024-04-22 03:39:34.000000 ares_ai-0.5.9/ares/superglue_filter.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)     5844 2024-05-16 09:46:01.000000 ares_ai-0.5.9/ares/synthetic_generator.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)    15573 2024-05-15 09:10:54.000000 ares_ai-0.5.9/ares/ues_idp.py
+drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-30 03:20:40.362965 ares_ai-0.5.9/ares_ai.egg-info/
+-rw-r--r--   0 manihani (23549) future   (20099)    28521 2024-05-30 03:20:31.000000 ares_ai-0.5.9/ares_ai.egg-info/PKG-INFO
+-rw-r--r--   0 manihani (23549) future   (20099)     4238 2024-05-30 03:20:40.000000 ares_ai-0.5.9/ares_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 manihani (23549) future   (20099)        1 2024-05-30 03:20:31.000000 ares_ai-0.5.9/ares_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 manihani (23549) future   (20099)       43 2024-05-30 03:20:31.000000 ares_ai-0.5.9/ares_ai.egg-info/entry_points.txt
+-rw-r--r--   0 manihani (23549) future   (20099)      706 2024-05-30 03:20:31.000000 ares_ai-0.5.9/ares_ai.egg-info/requires.txt
+-rw-r--r--   0 manihani (23549) future   (20099)        5 2024-05-30 03:20:31.000000 ares_ai-0.5.9/ares_ai.egg-info/top_level.txt
+drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-30 03:20:40.358965 ares_ai-0.5.9/checkpoints/
+-rw-rw-rw-   0 manihani (23549) future   (20099)       71 2024-04-22 03:39:34.000000 ares_ai-0.5.9/checkpoints/.gitignore
+-rw-rw-rw-   0 manihani (23549) future   (20099)     2966 2024-05-30 01:53:53.000000 ares_ai-0.5.9/pyproject.toml
+-rw-rw-rw-   0 manihani (23549) future   (20099)     5082 2024-05-30 02:07:52.000000 ares_ai-0.5.9/requirements.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)       93 2024-05-30 03:20:40.370965 ares_ai-0.5.9/setup.cfg
+drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-30 03:20:40.360965 ares_ai-0.5.9/tests/
+-rw-rw-rw-   0 manihani (23549) future   (20099)       71 2024-04-22 03:39:53.000000 ares_ai-0.5.9/tests/.gitignore
```

### Comparing `ares_ai-0.5.8/.gitignore` & `ares_ai-0.5.9/.gitignore`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/LICENSE` & `ares_ai-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/PKG-INFO` & `ares_ai-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ares-ai
-Version: 0.5.8
+Version: 0.5.9
 Summary: ARES is an advanced evaluation framework for Retrieval-Augmented Generation (RAG) systems, 
 Author-email: Jon Saad-Falcon <jonsaadfalcon@stanford.edu>, Robby Manihani <manihani@stanford.edu>, Omar Khattab <okhattab@stanford.edu>, Christopher Potts <cgpotts@stanford.edu>, Matei Zaharia <matei@berkeley.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -246,15 +246,16 @@
 Requires-Dist: sentencepiece==0.1.99
 Requires-Dist: sentence-transformers<3.0.0,>=2.2.2
 Requires-Dist: spacy<4.0.0,>=3.5.3
 Requires-Dist: torch>=2.2.1
 Requires-Dist: together>=1.1.0
 Requires-Dist: tokenizers>=0.13.3
 Requires-Dist: transformers==4.40.1
-Requires-Dist: vllm==0.4.1
+Provides-Extra: vllm
+Requires-Dist: vllm==0.4.1; extra == "vllm"
 
 <h2 align="center">ARES: An Automated Evaluation Framework for Retrieval-Augmented Generation Systems</h2>
 
 <p align="center">
   <a>Table of Contents:</a>
   <a href="#section1">Installation</a> |
   <a href="#section2">Requirements</a> |
@@ -284,15 +285,15 @@
   <a>
   <img alt="Static Badge" src="https://img.shields.io/badge/Made%20with-Python-red?style=flat&link=https%3A%2F%2Fpython.org%2F">
   </a>
 
 </p>
 
 
-ARES is a groundbreaking framework for evaluating Retrieval-Augmented Generation (RAG) models. The automated process combines synthetic data generation with fine-tuned classifiers to efficiently assess context relevance, answer faithfulness, and answer relevance, minimizing the need for extensive human annotations. ARES employs synthetic query generation and Precision-Performance Iteration (PPI), providing accurate evaluations with statistical confidence.
+ARES is a groundbreaking framework for evaluating Retrieval-Augmented Generation (RAG) models. The automated process combines synthetic data generation with fine-tuned classifiers to efficiently assess context relevance, answer faithfulness, and answer relevance, minimizing the need for extensive human annotations. ARES employs synthetic query generation and Prediction-Powered Inference (PPI), providing accurate evaluations with statistical confidence.
 
 
 ### 💬 Mini Q&A
 <hr>
 
 **What does ARES assess in RAG models?**
```

### Comparing `ares_ai-0.5.8/README.md` & `ares_ai-0.5.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
   <a>
   <img alt="Static Badge" src="https://img.shields.io/badge/Made%20with-Python-red?style=flat&link=https%3A%2F%2Fpython.org%2F">
   </a>
 
 </p>
 
 
-ARES is a groundbreaking framework for evaluating Retrieval-Augmented Generation (RAG) models. The automated process combines synthetic data generation with fine-tuned classifiers to efficiently assess context relevance, answer faithfulness, and answer relevance, minimizing the need for extensive human annotations. ARES employs synthetic query generation and Precision-Performance Iteration (PPI), providing accurate evaluations with statistical confidence.
+ARES is a groundbreaking framework for evaluating Retrieval-Augmented Generation (RAG) models. The automated process combines synthetic data generation with fine-tuned classifiers to efficiently assess context relevance, answer faithfulness, and answer relevance, minimizing the need for extensive human annotations. ARES employs synthetic query generation and Prediction-Powered Inference (PPI), providing accurate evaluations with statistical confidence.
 
 
 ### 💬 Mini Q&A
 <hr>
 
 **What does ARES assess in RAG models?**
```

#### html2text {}

```diff
@@ -2,16 +2,16 @@
                            GGeenneerraattiioonn SSyysstteemmss **********
     Table of Contents: _I_n_s_t_a_l_l_a_t_i_o_n | _R_e_q_u_i_r_e_m_e_n_t_s | _Q_u_i_c_k_ _S_t_a_r_t | _C_i_t_a_t_i_o_n
     _[_S_t_a_t_i_c_ _B_a_d_g_e_]_[_S_t_a_t_i_c_ _B_a_d_g_e_]_[_S_t_a_t_i_c_ _B_a_d_g_e_]_[_O_p_e_n_ _I_n_ _C_o_l_a_b_][Static Badge]
 ARES is a groundbreaking framework for evaluating Retrieval-Augmented
 Generation (RAG) models. The automated process combines synthetic data
 generation with fine-tuned classifiers to efficiently assess context relevance,
 answer faithfulness, and answer relevance, minimizing the need for extensive
-human annotations. ARES employs synthetic query generation and Precision-
-Performance Iteration (PPI), providing accurate evaluations with statistical
+human annotations. ARES employs synthetic query generation and Prediction-
+Powered Inference (PPI), providing accurate evaluations with statistical
 confidence. ### ð¬ Mini Q&A
 ===============================================================================
 **What does ARES assess in RAG models?** ARES conducts a comprehensive
 evaluation of Retrieval-Augmented Generation (RAG) models, assessing the
 systems for context relevance, answer faithfulness, and answer relevance. This
 thorough assessment ensures a complete understanding of the performance of the
 RAG system. **How does ARES automate the evaluation process?** ARES minimizes
```

### Comparing `ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/Filter_Synthetic_Queries.py` & `ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/Filter_Synthetic_Queries.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/General_Binary_Classifier.py` & `ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/General_Binary_Classifier.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/Generate_Synthetic_Queries_and_Answers.py` & `ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/Generate_Synthetic_Queries_and_Answers.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/LLM_Generation_Functions.py` & `ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/LLM_Generation_Functions.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-310.pyc` & `ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-311.pyc` & `ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-310.pyc` & `ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-311.pyc` & `ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-310.pyc` & `ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-311.pyc` & `ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-310.pyc` & `ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-311.pyc` & `ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/__pycache__/pytorchtools.cpython-310.pyc` & `ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/pytorchtools.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/LLM_as_a_Judge_Adaptation/pytorchtools.py` & `ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/pytorchtools.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/Evaluation_Functions.py` & `ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/Evaluation_Functions.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/LLMJudge_RAG_Compared_Scoring.py` & `ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/LLMJudge_RAG_Compared_Scoring.py`

 * *Files 1% similar despite different names*

```diff
@@ -1234,19 +1234,19 @@
         validation_set_ratios.append(round(Yhat_unlabeled_dataset[label_column].tolist().count(1) / len(Yhat_unlabeled_dataset), 3))
         accuracy_scores.append(round(results['accuracy'], 3))
         ground_truth_available = True
     else:
         ground_truth_available = False
 
     results = {
-        "ARES_Prediction": LLM_judge_ratio_predictions[0] if LLM_judge_ratio_predictions else None,
-        "ARES_Confidence_Interval": ppi_confidence_intervals[0] if ppi_confidence_intervals else None,
-        "Number_of_Examples_in_Evaluation_Set": validation_set_lengths[0] if validation_set_lengths else None,
-        "Ground_Truth_Performance": validation_set_ratios[0] if ground_truth_available and validation_set_ratios else None,
-        "ARES_LLM_Judge_Accuracy_on_Ground_Truth_Labels": accuracy_scores[0] if ground_truth_available and accuracy_scores else None,
+        "ARES_Prediction": LLM_judge_ratio_predictions[-1] if LLM_judge_ratio_predictions else None,
+        "ARES_Confidence_Interval": ppi_confidence_intervals[-1] if ppi_confidence_intervals else None,
+        "Number_of_Examples_in_Evaluation_Set": validation_set_lengths[-1] if validation_set_lengths else None,
+        "Ground_Truth_Performance": validation_set_ratios[-1] if ground_truth_available and validation_set_ratios else None,
+        "ARES_LLM_Judge_Accuracy_on_Ground_Truth_Labels": accuracy_scores[-1] if ground_truth_available and accuracy_scores else None,
         "Annotated_Examples_used_for_PPI": len(Y_labeled)
     }
     # Save the labeled dataset with predictions to a new TSV file
     if prediction_filepath != "None": 
         # Update the prediction column name based on the label column
         if label_column == "Context_Relevance_Label":
             prediction_column_name = "ARES_Context_Relevance_Prediction"
@@ -1260,20 +1260,20 @@
         print("--------------------------------------------------")
         print(f"Labeled dataset with predictions saved to {prediction_filepath}")
         print("--------------------------------------------------")
 
     print("--------------------------------------------------")
     print(label_column + " Scoring")
     print("ARES Ranking")
-    print("ARES Prediction: " + str(LLM_judge_ratio_predictions))
-    print("ARES Confidence Interval: " + str(ppi_confidence_intervals))
-    print("Number of Examples in Evaluation Set: " + str(validation_set_lengths))
+    print("ARES Prediction: " + str(results["ARES_Prediction"]))
+    print("ARES Confidence Interval: " + str(results["ARES_Confidence_Interval"]))
+    print("Number of Examples in Evaluation Set: " + str(results["Number_of_Examples_in_Evaluation_Set"]))
     if ground_truth_available:
-        print("Ground Truth Performance: " + str(validation_set_ratios))
+        print("Ground Truth Performance: " + str(results["Ground_Truth_Performance"]))
     if ground_truth_available:
-        print("ARES LLM Judge Accuracy on Ground Truth Labels: " + str(accuracy_scores))
-    print("Annotated Examples used for PPI: " + str(len(Y_labeled)))
+        print("ARES LLM Judge Accuracy on Ground Truth Labels: " + str(results["ARES_LLM_Judge_Accuracy_on_Ground_Truth_Labels"]))
+    print("Annotated Examples used for PPI: " + str(results["Annotated_Examples_used_for_PPI"]))
     print("--------------------------------------------------\n")
 
     return results
```

### Comparing `ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/Prepare_KILT_Dataset.py` & `ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/Prepare_KILT_Dataset.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/Prepare_SuperGLUE_Datasets.py` & `ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/Prepare_SuperGLUE_Datasets.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-310.pyc` & `ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-311.pyc` & `ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-310.pyc` & `ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue May 21 11:18:53 2024 UTC, .py size: 65743 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 1d83 4c66 cf00 0100  o.........Lf....
+00000000: 6f0d 0d0a 0000 0000 c7ec 5766 4b01 0100  o.........WfK...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 001a 0000 0040 0000 0073 1204 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0f 5a0f 6d10 5a10 0100 6400 6401 6c11  m.Z.m.Z...d.d.l.
@@ -2122,15 +2122,15 @@
 00008490: 0108 0108 0108 0108 0108 0108 0108 0108  ................
 000084a0: 0108 0108 0108 0108 0108 0108 0108 0108  ................
 000084b0: 0108 0108 020c 010a 0210 0108 0208 0110  ................
 000084c0: 0102 8010 031a 010e 010c 010e 0216 0104  ................
 000084d0: 0208 0120 011e 0210 0204 0212 0104 0210  ... ............
 000084e0: 0204 0110 0272 7c01 0000 6301 0000 0000  .....r|...c.....
 000084f0: 0000 0000 0000 003a 0000 000e 0000 0043  .......:.......C
-00008500: 0000 0073 1e09 0000 7c00 6401 1900 7d01  ...s....|.d...}.
+00008500: 0000 0073 3209 0000 7c00 6401 1900 7d01  ...s2...|.d...}.
 00008510: 7c00 6402 1900 7d02 7c00 6403 1900 7d03  |.d...}.|.d...}.
 00008520: 7c00 6404 1900 7d04 7c00 6405 1900 7d05  |.d...}.|.d...}.
 00008530: 7c00 6406 1900 7d06 7c00 6407 1900 7d07  |.d...}.|.d...}.
 00008540: 7c00 6408 1900 7d08 7c00 6409 1900 7d09  |.d...}.|.d...}.
 00008550: 7c00 640a 1900 7d0a 7c00 640b 1900 7d0b  |.d...}.|.d...}.
 00008560: 7c00 640c 1900 7d0c 7c00 640d 1900 7d0d  |.d...}.|.d...}.
 00008570: 7c00 640e 1900 7d0e 7c00 640f 1900 7d0f  |.d...}.|.d...}.
@@ -2147,15 +2147,15 @@
 00008620: 8d03 8f83 7d21 7c21 4400 5d78 7d22 7402  ....}!|!D.]x}"t.
 00008630: a003 a100 8f69 0100 7c22 6425 1900 a004  .....i..|"d%....
 00008640: 7c09 a101 7c0a 6426 7600 72ab 7c22 6427  |...|.d&v.r.|"d'
 00008650: 1900 a005 a100 a004 7c09 a101 6e06 7c22  ........|...n.|"
 00008660: 6427 1900 a004 7c09 a101 6428 9c02 7d23  d'....|...d(..}#
 00008670: 7c0a 6429 7600 72ca 7c22 642a 1900 a006  |.d)v.r.|"d*....
 00008680: 7c22 642a 1900 6a07 6421 1900 642b a102  |"d*..j.d!..d+..
-00008690: a004 7c09 a101 7c23 642c 3c00 7c08 6454  ..|...|#d,<.|.dT
+00008690: a004 7c09 a101 7c23 642c 3c00 7c08 645a  ..|...|#d,<.|.dZ
 000086a0: 6900 7c23 a401 8e01 7d24 7c24 7d25 7402  i.|#....}$|$}%t.
 000086b0: 6a08 7c25 642d 642e 8d02 7d26 642a 7c22  j.|%d-d...}&d*|"
 000086c0: 7600 72ec 7c22 642a 1900 a004 7c09 a101  v.r.|"d*....|...
 000086d0: 7d27 7c0f 6a09 7c26 7c27 642f 8d02 0100  }'|.j.|&|'d/....
 000086e0: 7402 a00a 7c02 7c26 6602 6421 a102 7d02  t...|.|&f.d!..}.
 000086f0: 7c21 a00b 642b a101 0100 5700 6400 0400  |!..d+....W.d...
 00008700: 0400 8303 0100 6e09 3100 9001 7304 7701  ......n.1...s.w.
@@ -2245,245 +2245,248 @@
 00008c40: 8400 7c34 4400 8301 a101 0100 7c11 7c05  ..|4D.......|.|.
 00008c50: 6a12 7600 9003 72d1 7c05 7c11 1900 a02a  j.v...r.|.|....*
 00008c60: a100 a02b a100 9003 73d1 7c15 a022 742c  ...+....s.|.."t,
 00008c70: 7c05 7c11 1900 a00f a100 a02d 642b a101  |.|........-d+..
 00008c80: 7413 7c05 8301 1b00 643f 8302 a101 0100  t.|.....d?......
 00008c90: 7c17 a022 742c 7c18 6440 1900 643f 8302  |.."t,|.d@..d?..
 00008ca0: a101 0100 6441 7d38 6e02 6423 7d38 7c13  ....dA}8n.d#}8|.
-00008cb0: 9003 72da 7c13 6421 1900 6e01 6400 7c16  ..r.|.d!..n.d.|.
-00008cc0: 9003 72e2 7c16 6421 1900 6e01 6400 7c14  ..r.|.d!..n.d.|.
-00008cd0: 9003 72ea 7c14 6421 1900 6e01 6400 7c38  ..r.|.d!..n.d.|8
-00008ce0: 9003 72f5 7c15 9003 72f5 7c15 6421 1900  ..r.|...r.|.d!..
+00008cb0: 9003 72da 7c13 642d 1900 6e01 6400 7c16  ..r.|.d-..n.d.|.
+00008cc0: 9003 72e2 7c16 642d 1900 6e01 6400 7c14  ..r.|.d-..n.d.|.
+00008cd0: 9003 72ea 7c14 642d 1900 6e01 6400 7c38  ..r.|.d-..n.d.|8
+00008ce0: 9003 72f5 7c15 9003 72f5 7c15 642d 1900  ..r.|...r.|.d-..
 00008cf0: 6e01 6400 7c38 9004 7200 7c17 9004 7200  n.d.|8..r.|...r.
-00008d00: 7c17 6421 1900 6e01 6400 7413 7c31 8301  |.d!..n.d.t.|1..
+00008d00: 7c17 642d 1900 6e01 6400 7413 7c31 8301  |.d-..n.d.t.|1..
 00008d10: 6442 9c06 7d18 7c1f 6430 6b03 9004 7243  dB..}.|.d0k...rC
 00008d20: 7c11 643a 6b02 9004 7214 6443 7d39 6e0f  |.d:k...r.dC}9n.
 00008d30: 7c11 643c 6b02 9004 721c 6444 7d39 6e07  |.d<k...r.dD}9n.
 00008d40: 7c11 643b 6b02 9004 7223 6445 7d39 7c05  |.d;k...r#dE}9|.
 00008d50: 6a2e 7c10 7c39 6901 6441 6446 8d02 0100  j.|.|9i.dAdF....
 00008d60: 7c05 6a2f 7c1f 6447 6423 6448 8d03 0100  |.j/|.dGd#dH....
 00008d70: 7430 6449 8301 0100 7430 644a 7c1f 9b00  t0dI....t0dJ|...
 00008d80: 9d02 8301 0100 7430 6449 8301 0100 7430  ......t0dI....t0
 00008d90: 6449 8301 0100 7430 7c11 644b 1700 8301  dI....t0|.dK....
 00008da0: 0100 7430 644c 8301 0100 7430 644d 7431  ..t0dL....t0dMt1
-00008db0: 7c13 8301 1700 8301 0100 7430 644e 7431  |.........t0dNt1
-00008dc0: 7c16 8301 1700 8301 0100 7430 644f 7431  |.........t0dOt1
-00008dd0: 7c14 8301 1700 8301 0100 7c38 9004 7274  |.........|8..rt
-00008de0: 7430 6450 7431 7c15 8301 1700 8301 0100  t0dPt1|.........
-00008df0: 7c38 9004 727f 7430 6451 7431 7c17 8301  |8..r.t0dQt1|...
-00008e00: 1700 8301 0100 7430 6452 7431 7413 7c31  ......t0dRt1t.|1
-00008e10: 8301 8301 1700 8301 0100 7430 6453 8301  ..........t0dS..
-00008e20: 0100 7c18 5300 2955 4e72 eb00 0000 727a  ..|.S.)UNr....rz
-00008e30: 0100 0072 7701 0000 7279 0100 0072 7b01  ...rw...ry...r{.
-00008e40: 0000 72b1 0000 0072 b200 0000 720e 0100  ..r....r....r...
-00008e50: 0072 1401 0000 722b 0000 0072 de00 0000  .r....r+...r....
-00008e60: 72df 0000 0072 e000 0000 72d6 0000 0072  r....r....r....r
-00008e70: 4a01 0000 7278 0100 0072 8700 0000 72e2  J...rx...r....r.
-00008e80: 0000 00da 1b4c 4c4d 5f6a 7564 6765 5f72  .....LLM_judge_r
-00008e90: 6174 696f 5f70 7265 6469 6374 696f 6e73  atio_predictions
-00008ea0: da16 7661 6c69 6461 7469 6f6e 5f73 6574  ..validation_set
-00008eb0: 5f6c 656e 6774 6873 da15 7661 6c69 6461  _lengths..valida
-00008ec0: 7469 6f6e 5f73 6574 5f72 6174 696f 73da  tion_set_ratios.
-00008ed0: 1870 7069 5f63 6f6e 6669 6465 6e63 655f  .ppi_confidence_
-00008ee0: 696e 7465 7276 616c 73da 0f61 6363 7572  intervals..accur
-00008ef0: 6163 795f 7363 6f72 6573 7252 0100 0072  acy_scoresrR...r
-00008f00: 1001 0000 721a 0100 0072 0901 0000 721b  ....r....r....r.
-00008f10: 0100 0072 1c01 0000 721d 0100 00da 1370  ...r....r......p
-00008f20: 7265 6469 6374 696f 6e5f 6669 6c65 7061  rediction_filepa
-00008f30: 7468 7270 0100 0072 0100 0000 5a07 5363  thrp...r....Z.Sc
-00008f40: 6f72 696e 6746 7220 0100 0072 5400 0000  oringFr ...rT...
-00008f50: 7232 0000 0072 5500 0000 7222 0100 0072  r2...rU...r"...r
-00008f60: 2301 0000 7250 0000 0072 fb00 0000 7251  #...rP...r....rQ
-00008f70: 0000 0072 5800 0000 7224 0100 0072 2601  ...rX...r$...r&.
-00008f80: 0000 72d2 0000 007a 1c45 7272 6f72 3a20  ..r....z.Error: 
-00008f90: 4e6f 206c 6c6d 5f6a 7564 6765 2070 726f  No llm_judge pro
-00008fa0: 7669 6465 6472 0a01 0000 720b 0100 0072  videdr....r....r
-00008fb0: e700 0000 7229 0100 0072 1f01 0000 2903  ....r)...r....).
-00008fc0: 726b 0100 0072 b500 0000 7221 0100 0072  rk...r....r!...r
-00008fd0: e800 0000 72ee 0000 0072 2a01 0000 7233  ....r....r*...r3
-00008fe0: 0100 0072 3a01 0000 6301 0000 0000 0000  ...r:...c.......
-00008ff0: 0000 0000 0002 0000 0005 0000 0053 0000  .............S..
-00009000: 0073 1600 0000 6700 7c00 5d07 7d01 7400  .s....g.|.].}.t.
-00009010: 7c01 6400 8302 9102 7102 5300 2901 72f9  |.d.....q.S.).r.
-00009020: 0000 0029 01da 0572 6f75 6e64 2902 728d  ...)...round).r.
-00009030: 0000 00da 0576 616c 7565 724c 0000 0072  .....valuerL...r
-00009040: 4c00 0000 724d 0000 0072 8f00 0000 ce04  L...rM...r......
-00009050: 0000 7302 0000 0016 007a 2d65 7661 6c75  ..s......z-evalu
-00009060: 6174 655f 616e 645f 7363 6f72 696e 675f  ate_and_scoring_
-00009070: 6461 7461 2e3c 6c6f 6361 6c73 3e2e 3c6c  data.<locals>.<l
-00009080: 6973 7463 6f6d 703e 72f9 0000 0072 1e01  istcomp>r....r..
-00009090: 0000 5429 065a 0f41 5245 535f 5072 6564  ..T).Z.ARES_Pred
-000090a0: 6963 7469 6f6e da18 4152 4553 5f43 6f6e  iction..ARES_Con
-000090b0: 6669 6465 6e63 655f 496e 7465 7276 616c  fidence_Interval
-000090c0: 5a24 4e75 6d62 6572 5f6f 665f 4578 616d  Z$Number_of_Exam
-000090d0: 706c 6573 5f69 6e5f 4576 616c 7561 7469  ples_in_Evaluati
-000090e0: 6f6e 5f53 6574 5a18 4772 6f75 6e64 5f54  on_SetZ.Ground_T
-000090f0: 7275 7468 5f50 6572 666f 726d 616e 6365  ruth_Performance
-00009100: 5a2e 4152 4553 5f4c 4c4d 5f4a 7564 6765  Z.ARES_LLM_Judge
-00009110: 5f41 6363 7572 6163 795f 6f6e 5f47 726f  _Accuracy_on_Gro
-00009120: 756e 645f 5472 7574 685f 4c61 6265 6c73  und_Truth_Labels
-00009130: 5a1f 416e 6e6f 7461 7465 645f 4578 616d  Z.Annotated_Exam
-00009140: 706c 6573 5f75 7365 645f 666f 725f 5050  ples_used_for_PP
-00009150: 495a 2141 5245 535f 436f 6e74 6578 745f  IZ!ARES_Context_
-00009160: 5265 6c65 7661 6e63 655f 5072 6564 6963  Relevance_Predic
-00009170: 7469 6f6e 5a20 4152 4553 5f41 6e73 7765  tionZ ARES_Answe
-00009180: 725f 5265 6c65 7661 6e63 655f 5072 6564  r_Relevance_Pred
-00009190: 6963 7469 6f6e 5a23 4152 4553 5f41 6e73  ictionZ#ARES_Ans
-000091a0: 7765 725f 4661 6974 6866 756c 6e65 7373  wer_Faithfulness
-000091b0: 5f50 7265 6469 6374 696f 6e29 0272 9700  _Prediction).r..
-000091c0: 0000 da07 696e 706c 6163 6572 6c00 0000  ....inplacerl...
-000091d0: 7271 0100 007a 322d 2d2d 2d2d 2d2d 2d2d  rq...z2---------
-000091e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00008db0: 7c18 644e 1900 8301 1700 8301 0100 7430  |.dN..........t0
+00008dc0: 644f 7431 7c18 6450 1900 8301 1700 8301  dOt1|.dP........
+00008dd0: 0100 7430 6451 7431 7c18 6452 1900 8301  ..t0dQt1|.dR....
+00008de0: 1700 8301 0100 7c38 9004 727c 7430 6453  ......|8..r|t0dS
+00008df0: 7431 7c18 6454 1900 8301 1700 8301 0100  t1|.dT..........
+00008e00: 7c38 9004 7289 7430 6455 7431 7c18 6456  |8..r.t0dUt1|.dV
+00008e10: 1900 8301 1700 8301 0100 7430 6457 7431  ..........t0dWt1
+00008e20: 7c18 6458 1900 8301 1700 8301 0100 7430  |.dX..........t0
+00008e30: 6459 8301 0100 7c18 5300 295b 4e72 eb00  dY....|.S.)[Nr..
+00008e40: 0000 727a 0100 0072 7701 0000 7279 0100  ..rz...rw...ry..
+00008e50: 0072 7b01 0000 72b1 0000 0072 b200 0000  .r{...r....r....
+00008e60: 720e 0100 0072 1401 0000 722b 0000 0072  r....r....r+...r
+00008e70: de00 0000 72df 0000 0072 e000 0000 72d6  ....r....r....r.
+00008e80: 0000 0072 4a01 0000 7278 0100 0072 8700  ...rJ...rx...r..
+00008e90: 0000 72e2 0000 00da 1b4c 4c4d 5f6a 7564  ..r......LLM_jud
+00008ea0: 6765 5f72 6174 696f 5f70 7265 6469 6374  ge_ratio_predict
+00008eb0: 696f 6e73 da16 7661 6c69 6461 7469 6f6e  ions..validation
+00008ec0: 5f73 6574 5f6c 656e 6774 6873 da15 7661  _set_lengths..va
+00008ed0: 6c69 6461 7469 6f6e 5f73 6574 5f72 6174  lidation_set_rat
+00008ee0: 696f 73da 1870 7069 5f63 6f6e 6669 6465  ios..ppi_confide
+00008ef0: 6e63 655f 696e 7465 7276 616c 73da 0f61  nce_intervals..a
+00008f00: 6363 7572 6163 795f 7363 6f72 6573 7252  ccuracy_scoresrR
+00008f10: 0100 0072 1001 0000 721a 0100 0072 0901  ...r....r....r..
+00008f20: 0000 721b 0100 0072 1c01 0000 721d 0100  ..r....r....r...
+00008f30: 00da 1370 7265 6469 6374 696f 6e5f 6669  ...prediction_fi
+00008f40: 6c65 7061 7468 7270 0100 0072 0100 0000  lepathrp...r....
+00008f50: 5a07 5363 6f72 696e 6746 7220 0100 0072  Z.ScoringFr ...r
+00008f60: 5400 0000 7232 0000 0072 5500 0000 7222  T...r2...rU...r"
+00008f70: 0100 0072 2301 0000 7250 0000 0072 fb00  ...r#...rP...r..
+00008f80: 0000 7251 0000 0072 5800 0000 7224 0100  ..rQ...rX...r$..
+00008f90: 0072 2601 0000 72d2 0000 007a 1c45 7272  .r&...r....z.Err
+00008fa0: 6f72 3a20 4e6f 206c 6c6d 5f6a 7564 6765  or: No llm_judge
+00008fb0: 2070 726f 7669 6465 6472 0a01 0000 720b   providedr....r.
+00008fc0: 0100 0072 e700 0000 7229 0100 0072 1f01  ...r....r)...r..
+00008fd0: 0000 2903 726b 0100 0072 b500 0000 7221  ..).rk...r....r!
+00008fe0: 0100 0072 e800 0000 72ee 0000 0072 2a01  ...r....r....r*.
+00008ff0: 0000 7233 0100 0072 3a01 0000 6301 0000  ..r3...r:...c...
+00009000: 0000 0000 0000 0000 0002 0000 0005 0000  ................
+00009010: 0053 0000 0073 1600 0000 6700 7c00 5d07  .S...s....g.|.].
+00009020: 7d01 7400 7c01 6400 8302 9102 7102 5300  }.t.|.d.....q.S.
+00009030: 2901 72f9 0000 0029 01da 0572 6f75 6e64  ).r....)...round
+00009040: 2902 728d 0000 00da 0576 616c 7565 724c  ).r......valuerL
+00009050: 0000 0072 4c00 0000 724d 0000 0072 8f00  ...rL...rM...r..
+00009060: 0000 ce04 0000 7302 0000 0016 007a 2d65  ......s......z-e
+00009070: 7661 6c75 6174 655f 616e 645f 7363 6f72  valuate_and_scor
+00009080: 696e 675f 6461 7461 2e3c 6c6f 6361 6c73  ing_data.<locals
+00009090: 3e2e 3c6c 6973 7463 6f6d 703e 72f9 0000  >.<listcomp>r...
+000090a0: 0072 1e01 0000 5429 06da 0f41 5245 535f  .r....T)...ARES_
+000090b0: 5072 6564 6963 7469 6f6e da18 4152 4553  Prediction..ARES
+000090c0: 5f43 6f6e 6669 6465 6e63 655f 496e 7465  _Confidence_Inte
+000090d0: 7276 616c da24 4e75 6d62 6572 5f6f 665f  rval.$Number_of_
+000090e0: 4578 616d 706c 6573 5f69 6e5f 4576 616c  Examples_in_Eval
+000090f0: 7561 7469 6f6e 5f53 6574 da18 4772 6f75  uation_Set..Grou
+00009100: 6e64 5f54 7275 7468 5f50 6572 666f 726d  nd_Truth_Perform
+00009110: 616e 6365 da2e 4152 4553 5f4c 4c4d 5f4a  ance..ARES_LLM_J
+00009120: 7564 6765 5f41 6363 7572 6163 795f 6f6e  udge_Accuracy_on
+00009130: 5f47 726f 756e 645f 5472 7574 685f 4c61  _Ground_Truth_La
+00009140: 6265 6c73 da1f 416e 6e6f 7461 7465 645f  bels..Annotated_
+00009150: 4578 616d 706c 6573 5f75 7365 645f 666f  Examples_used_fo
+00009160: 725f 5050 495a 2141 5245 535f 436f 6e74  r_PPIZ!ARES_Cont
+00009170: 6578 745f 5265 6c65 7661 6e63 655f 5072  ext_Relevance_Pr
+00009180: 6564 6963 7469 6f6e 5a20 4152 4553 5f41  edictionZ ARES_A
+00009190: 6e73 7765 725f 5265 6c65 7661 6e63 655f  nswer_Relevance_
+000091a0: 5072 6564 6963 7469 6f6e 5a23 4152 4553  PredictionZ#ARES
+000091b0: 5f41 6e73 7765 725f 4661 6974 6866 756c  _Answer_Faithful
+000091c0: 6e65 7373 5f50 7265 6469 6374 696f 6e29  ness_Prediction)
+000091d0: 0272 9700 0000 da07 696e 706c 6163 6572  .r......inplacer
+000091e0: 6c00 0000 7271 0100 007a 322d 2d2d 2d2d  l...rq...z2-----
 000091f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009200: 2d2d 2d2d 2d2d 2d2d 2d7a 2a4c 6162 656c  ---------z*Label
-00009210: 6564 2064 6174 6173 6574 2077 6974 6820  ed dataset with 
-00009220: 7072 6564 6963 7469 6f6e 7320 7361 7665  predictions save
-00009230: 6420 746f 207a 0820 5363 6f72 696e 677a  d to z. Scoringz
-00009240: 0c41 5245 5320 5261 6e6b 696e 677a 1141  .ARES Rankingz.A
-00009250: 5245 5320 5072 6564 6963 7469 6f6e 3a20  RES Prediction: 
-00009260: 7a1a 4152 4553 2043 6f6e 6669 6465 6e63  z.ARES Confidenc
-00009270: 6520 496e 7465 7276 616c 3a20 7a26 4e75  e Interval: z&Nu
-00009280: 6d62 6572 206f 6620 4578 616d 706c 6573  mber of Examples
-00009290: 2069 6e20 4576 616c 7561 7469 6f6e 2053   in Evaluation S
-000092a0: 6574 3a20 7a1a 4772 6f75 6e64 2054 7275  et: z.Ground Tru
-000092b0: 7468 2050 6572 666f 726d 616e 6365 3a20  th Performance: 
-000092c0: 7a30 4152 4553 204c 4c4d 204a 7564 6765  z0ARES LLM Judge
-000092d0: 2041 6363 7572 6163 7920 6f6e 2047 726f   Accuracy on Gro
-000092e0: 756e 6420 5472 7574 6820 4c61 6265 6c73  und Truth Labels
-000092f0: 3a20 7a21 416e 6e6f 7461 7465 6420 4578  : z!Annotated Ex
-00009300: 616d 706c 6573 2075 7365 6420 666f 7220  amples used for 
-00009310: 5050 493a 207a 332d 2d2d 2d2d 2d2d 2d2d  PPI: z3---------
-00009320: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009330: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009340: 2d2d 2d2d 2d2d 2d2d 2d0a 724c 0000 0029  ---------.rL...)
-00009350: 3272 4200 0000 7212 0000 0072 3e00 0000  2rB...r....r>...
-00009360: 723e 0100 0072 1501 0000 723f 0100 0072  r>...r....r?...r
-00009370: 4001 0000 72b8 0000 0072 4101 0000 7242  @...r....rA...rB
-00009380: 0100 0072 4301 0000 7244 0100 00da 0664  ...rC...rD.....d
-00009390: 6574 6163 68da 0363 7075 da05 6e75 6d70  etach..cpu..nump
-000093a0: 7972 9800 0000 72dc 0000 0072 dd00 0000  yr....r....r....
-000093b0: 7297 0000 0072 7800 0000 726c 0100 0072  r....rx...rl...r
-000093c0: 2600 0000 721d 0000 0072 d900 0000 7223  &...r....r....r#
-000093d0: 0000 0072 2000 0000 7228 0000 0072 1e00  ...r ...r(...r..
-000093e0: 0000 7224 0000 0072 2100 0000 7227 0000  ..r$...r!...r'..
-000093f0: 0072 1f00 0000 7225 0000 0072 2200 0000  .r....r%...r"...
-00009400: 72ff 0000 0072 b900 0000 da05 6172 7261  r....r......arra
-00009410: 79da 0676 616c 7565 7372 bb00 0000 7262  y..valuesr....rb
-00009420: 0000 0072 ce00 0000 72bc 0000 00da 0669  ...r....r......i
-00009430: 736e 756c 6cda 0361 6c6c 7283 0100 00da  snull..allr.....
-00009440: 0563 6f75 6e74 da06 7265 6e61 6d65 7263  .count..renamerc
-00009450: 0100 0072 7a00 0000 7263 0000 0029 3a72  ...rz...rc...):r
-00009460: 1901 0000 72eb 0000 0072 7a01 0000 7277  ....r....rz...rw
-00009470: 0100 0072 7901 0000 727b 0100 0072 b100  ...ry...r{...r..
-00009480: 0000 72b2 0000 0072 0e01 0000 7214 0100  ..r....r....r...
-00009490: 0072 2b00 0000 72de 0000 0072 df00 0000  .r+...r....r....
-000094a0: 72e0 0000 0072 d600 0000 724a 0100 0072  r....r....rJ...r
-000094b0: 7801 0000 7287 0000 0072 e200 0000 727d  x...r....r....r}
-000094c0: 0100 0072 7e01 0000 727f 0100 0072 8001  ...r~...r....r..
-000094d0: 0000 7281 0100 0072 5201 0000 7210 0100  ..r....rR...r...
-000094e0: 0072 1a01 0000 7209 0100 0072 1b01 0000  .r....r....r....
-000094f0: 721c 0100 0072 1d01 0000 7282 0100 0072  r....r....r....r
-00009500: 2c01 0000 724d 0100 0072 4e01 0000 724f  ,...rM...rN...rO
-00009510: 0100 0072 5001 0000 7256 0000 0072 2701  ...rP...rV...r'.
-00009520: 0000 7250 0000 0072 2f01 0000 5a10 7175  ..rP...r/...Z.qu
-00009530: 6572 795f 6c61 6265 6c65 645f 6964 7251  ery_labeled_idrQ
-00009540: 0100 0072 6e01 0000 7266 0000 0072 6700  ...rn...rf...rg.
-00009550: 0000 727b 0000 00da 0573 636f 7265 5a18  ..r{.....scoreZ.
-00009560: 595f 6c61 6265 6c65 645f 7072 6564 6963  Y_labeled_predic
-00009570: 7469 6f6e 735f 6e70 72ae 0000 0072 af00  tions_npr....r..
-00009580: 0000 72b0 0000 0072 cc00 0000 72cb 0000  ..r....r....r...
-00009590: 0072 cd00 0000 5a14 4c4c 4d5f 6a75 6467  .r....Z.LLM_judg
-000095a0: 655f 7072 6564 6963 7469 6f6e 5a16 6772  e_predictionZ.gr
-000095b0: 6f75 6e64 5f74 7275 7468 5f61 7661 696c  ound_truth_avail
-000095c0: 6162 6c65 5a16 7072 6564 6963 7469 6f6e  ableZ.prediction
-000095d0: 5f63 6f6c 756d 6e5f 6e61 6d65 724c 0000  _column_namerL..
-000095e0: 0072 4c00 0000 724d 0000 00da 1965 7661  .rL...rM.....eva
-000095f0: 6c75 6174 655f 616e 645f 7363 6f72 696e  luate_and_scorin
-00009600: 675f 6461 7461 2f04 0000 7350 0100 0008  g_data/...sP....
-00009610: 0108 0108 0108 0108 0108 0108 0108 0108  ................
-00009620: 0108 0108 0108 0108 0108 0108 0108 0108  ................
-00009630: 0108 0108 0108 0108 0108 0108 0108 0108  ................
-00009640: 0108 0108 0108 0108 0108 0108 0108 0206  ................
-00009650: 0208 0110 0108 010a 010c 0226 0106 fe08  ...........&....
-00009660: 0424 010e 0204 010e 0108 020e 020e 0310  .$..............
-00009670: 030c 011e eb02 8002 ff1e ff18 1908 010a  ................
-00009680: 020e 0114 0204 0114 0214 0116 0212 0108  ................
-00009690: 0108 0108 010a 0206 011e 010a 0120 010a  ............. ..
-000096a0: 0120 011e 020a 0206 0120 010a 0122 010a  . ....... ..."..
-000096b0: 0122 0120 020a 0206 011e 010a 0120 010a  .". ......... ..
-000096c0: 0120 011e 020a 020e 0102 dc1e ff0a 270e  . ............'.
-000096d0: 0104 0214 0214 0114 0210 0108 0108 0108  ................
-000096e0: 010a 0206 011e 011e 020a 0206 0120 0120  ............. . 
-000096f0: 020a 0206 011e 011e 020a 020e 0102 e81e  ................
-00009700: ff0a 1b0c 0110 0210 0110 0116 0210 010a  ................
-00009710: 010e 0114 011e 0326 0114 0106 0104 0210  .......&........
-00009720: 0310 0110 0116 0116 0106 0106 fa0a 090a  ................
-00009730: 0206 010a 0106 010a 0104 0112 0210 0108  ................
-00009740: 010e 0108 0108 020c 0108 0110 0110 0110  ................
-00009750: 0106 0110 0106 0110 0114 0108 0104 0272  ...............r
-00009760: 9101 0000 7292 0000 0029 0172 da00 0000  ....r....).r....
-00009770: 296b da08 746f 7263 682e 6e6e 7243 0000  )k..torch.nnrC..
-00009780: 00da 0c74 7261 6e73 666f 726d 6572 7372  ...transformersr
-00009790: 0200 0000 7203 0000 0072 0400 0000 7205  ....r....r....r.
-000097a0: 0000 0072 0600 0000 7207 0000 0072 0800  ...r....r....r..
-000097b0: 0000 7209 0000 0072 0a00 0000 720b 0000  ..r....r....r...
-000097c0: 0072 0c00 0000 720d 0000 0072 0e00 0000  .r....r....r....
-000097d0: 720f 0000 0072 dc00 0000 da06 7061 6e64  r....r......pand
-000097e0: 6173 7299 0000 0072 8901 0000 72b9 0000  asr....r....r...
-000097f0: 0072 6401 0000 da03 6173 7472 9e00 0000  .rd.....astr....
-00009800: 723c 0100 00da 0770 7961 7272 6f77 729b  r<.....pyarrowr.
-00009810: 0000 00da 0f70 7961 7272 6f77 2e64 6174  .....pyarrow.dat
-00009820: 6173 6574 da07 6461 7461 7365 74da 0264  aset..dataset..d
-00009830: 73da 0b74 6f72 6368 2e6f 7074 696d 7210  s..torch.optimr.
-00009840: 0000 00da 1074 6f72 6368 2e75 7469 6c73  .....torch.utils
-00009850: 2e64 6174 6172 1100 0000 723e 0000 00da  .datar....r>....
-00009860: 0974 7164 6d2e 6175 746f 7212 0000 00da  .tqdm.autor.....
-00009870: 0a73 7461 7469 7374 6963 73da 0474 696d  .statistics..tim
-00009880: 6572 fc00 0000 da02 7370 720c 0100 00da  er......spr.....
-00009890: 1773 6b6c 6561 726e 2e6d 6f64 656c 5f73  .sklearn.model_s
-000098a0: 656c 6563 7469 6f6e 7213 0000 00da 046a  electionr......j
-000098b0: 736f 6e72 bf00 0000 7272 0000 00da 0b73  sonr....rr.....s
-000098c0: 6369 7079 2e73 7461 7473 da05 7374 6174  cipy.stats..stat
-000098d0: 73da 0861 7267 7061 7273 65da 066f 7065  s..argparse..ope
-000098e0: 6e61 69da 0c72 616e 646f 6d5f 7374 6174  nai..random_stat
-000098f0: 65da 0473 6565 64da 0b6d 616e 7561 6c5f  e..seed..manual_
-00009900: 7365 6564 7263 0000 00da 0765 6e76 6972  seedrc.....envir
-00009910: 6f6e 5a21 6172 6573 2e52 4147 5f41 7574  onZ!ares.RAG_Aut
-00009920: 6f6d 6174 6963 5f45 7661 6c75 6174 696f  omatic_Evaluatio
-00009930: 6e2e 7070 6972 1900 0000 721a 0000 0072  n.ppir....r....r
-00009940: 1b00 0000 5a32 6172 6573 2e52 4147 5f41  ....Z2ares.RAG_A
+00009200: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00009210: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7a 2a4c  -------------z*L
+00009220: 6162 656c 6564 2064 6174 6173 6574 2077  abeled dataset w
+00009230: 6974 6820 7072 6564 6963 7469 6f6e 7320  ith predictions 
+00009240: 7361 7665 6420 746f 207a 0820 5363 6f72  saved to z. Scor
+00009250: 696e 677a 0c41 5245 5320 5261 6e6b 696e  ingz.ARES Rankin
+00009260: 677a 1141 5245 5320 5072 6564 6963 7469  gz.ARES Predicti
+00009270: 6f6e 3a20 7285 0100 007a 1a41 5245 5320  on: r....z.ARES 
+00009280: 436f 6e66 6964 656e 6365 2049 6e74 6572  Confidence Inter
+00009290: 7661 6c3a 2072 8601 0000 7a26 4e75 6d62  val: r....z&Numb
+000092a0: 6572 206f 6620 4578 616d 706c 6573 2069  er of Examples i
+000092b0: 6e20 4576 616c 7561 7469 6f6e 2053 6574  n Evaluation Set
+000092c0: 3a20 7287 0100 007a 1a47 726f 756e 6420  : r....z.Ground 
+000092d0: 5472 7574 6820 5065 7266 6f72 6d61 6e63  Truth Performanc
+000092e0: 653a 2072 8801 0000 7a30 4152 4553 204c  e: r....z0ARES L
+000092f0: 4c4d 204a 7564 6765 2041 6363 7572 6163  LM Judge Accurac
+00009300: 7920 6f6e 2047 726f 756e 6420 5472 7574  y on Ground Trut
+00009310: 6820 4c61 6265 6c73 3a20 7289 0100 007a  h Labels: r....z
+00009320: 2141 6e6e 6f74 6174 6564 2045 7861 6d70  !Annotated Examp
+00009330: 6c65 7320 7573 6564 2066 6f72 2050 5049  les used for PPI
+00009340: 3a20 728a 0100 007a 332d 2d2d 2d2d 2d2d  : r....z3-------
+00009350: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00009360: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00009370: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 724c 0000  -----------.rL..
+00009380: 0029 3272 4200 0000 7212 0000 0072 3e00  .)2rB...r....r>.
+00009390: 0000 723e 0100 0072 1501 0000 723f 0100  ..r>...r....r?..
+000093a0: 0072 4001 0000 72b8 0000 0072 4101 0000  .r@...r....rA...
+000093b0: 7242 0100 0072 4301 0000 7244 0100 00da  rB...rC...rD....
+000093c0: 0664 6574 6163 68da 0363 7075 da05 6e75  .detach..cpu..nu
+000093d0: 6d70 7972 9800 0000 72dc 0000 0072 dd00  mpyr....r....r..
+000093e0: 0000 7297 0000 0072 7800 0000 726c 0100  ..r....rx...rl..
+000093f0: 0072 2600 0000 721d 0000 0072 d900 0000  .r&...r....r....
+00009400: 7223 0000 0072 2000 0000 7228 0000 0072  r#...r ...r(...r
+00009410: 1e00 0000 7224 0000 0072 2100 0000 7227  ....r$...r!...r'
+00009420: 0000 0072 1f00 0000 7225 0000 0072 2200  ...r....r%...r".
+00009430: 0000 72ff 0000 0072 b900 0000 da05 6172  ..r....r......ar
+00009440: 7261 79da 0676 616c 7565 7372 bb00 0000  ray..valuesr....
+00009450: 7262 0000 0072 ce00 0000 72bc 0000 00da  rb...r....r.....
+00009460: 0669 736e 756c 6cda 0361 6c6c 7283 0100  .isnull..allr...
+00009470: 00da 0563 6f75 6e74 da06 7265 6e61 6d65  ...count..rename
+00009480: 7263 0100 0072 7a00 0000 7263 0000 0029  rc...rz...rc...)
+00009490: 3a72 1901 0000 72eb 0000 0072 7a01 0000  :r....r....rz...
+000094a0: 7277 0100 0072 7901 0000 727b 0100 0072  rw...ry...r{...r
+000094b0: b100 0000 72b2 0000 0072 0e01 0000 7214  ....r....r....r.
+000094c0: 0100 0072 2b00 0000 72de 0000 0072 df00  ...r+...r....r..
+000094d0: 0000 72e0 0000 0072 d600 0000 724a 0100  ..r....r....rJ..
+000094e0: 0072 7801 0000 7287 0000 0072 e200 0000  .rx...r....r....
+000094f0: 727d 0100 0072 7e01 0000 727f 0100 0072  r}...r~...r....r
+00009500: 8001 0000 7281 0100 0072 5201 0000 7210  ....r....rR...r.
+00009510: 0100 0072 1a01 0000 7209 0100 0072 1b01  ...r....r....r..
+00009520: 0000 721c 0100 0072 1d01 0000 7282 0100  ..r....r....r...
+00009530: 0072 2c01 0000 724d 0100 0072 4e01 0000  .r,...rM...rN...
+00009540: 724f 0100 0072 5001 0000 7256 0000 0072  rO...rP...rV...r
+00009550: 2701 0000 7250 0000 0072 2f01 0000 5a10  '...rP...r/...Z.
+00009560: 7175 6572 795f 6c61 6265 6c65 645f 6964  query_labeled_id
+00009570: 7251 0100 0072 6e01 0000 7266 0000 0072  rQ...rn...rf...r
+00009580: 6700 0000 727b 0000 00da 0573 636f 7265  g...r{.....score
+00009590: 5a18 595f 6c61 6265 6c65 645f 7072 6564  Z.Y_labeled_pred
+000095a0: 6963 7469 6f6e 735f 6e70 72ae 0000 0072  ictions_npr....r
+000095b0: af00 0000 72b0 0000 0072 cc00 0000 72cb  ....r....r....r.
+000095c0: 0000 0072 cd00 0000 5a14 4c4c 4d5f 6a75  ...r....Z.LLM_ju
+000095d0: 6467 655f 7072 6564 6963 7469 6f6e 5a16  dge_predictionZ.
+000095e0: 6772 6f75 6e64 5f74 7275 7468 5f61 7661  ground_truth_ava
+000095f0: 696c 6162 6c65 5a16 7072 6564 6963 7469  ilableZ.predicti
+00009600: 6f6e 5f63 6f6c 756d 6e5f 6e61 6d65 724c  on_column_namerL
+00009610: 0000 0072 4c00 0000 724d 0000 00da 1965  ...rL...rM.....e
+00009620: 7661 6c75 6174 655f 616e 645f 7363 6f72  valuate_and_scor
+00009630: 696e 675f 6461 7461 2f04 0000 7350 0100  ing_data/...sP..
+00009640: 0008 0108 0108 0108 0108 0108 0108 0108  ................
+00009650: 0108 0108 0108 0108 0108 0108 0108 0108  ................
+00009660: 0108 0108 0108 0108 0108 0108 0108 0108  ................
+00009670: 0108 0108 0108 0108 0108 0108 0108 0108  ................
+00009680: 0206 0208 0110 0108 010a 010c 0226 0106  .............&..
+00009690: fe08 0424 010e 0204 010e 0108 020e 020e  ...$............
+000096a0: 0310 030c 011e eb02 8002 ff1e ff18 1908  ................
+000096b0: 010a 020e 0114 0204 0114 0214 0116 0212  ................
+000096c0: 0108 0108 0108 010a 0206 011e 010a 0120  ............... 
+000096d0: 010a 0120 011e 020a 0206 0120 010a 0122  ... ....... ..."
+000096e0: 010a 0122 0120 020a 0206 011e 010a 0120  ...". ......... 
+000096f0: 010a 0120 011e 020a 020e 0102 dc1e ff0a  ... ............
+00009700: 270e 0104 0214 0214 0114 0210 0108 0108  '...............
+00009710: 0108 010a 0206 011e 011e 020a 0206 0120  ............... 
+00009720: 0120 020a 0206 011e 011e 020a 020e 0102  . ..............
+00009730: e81e ff0a 1b0c 0110 0210 0110 0116 0210  ................
+00009740: 010a 010e 0114 011e 0326 0114 0106 0104  .........&......
+00009750: 0210 0310 0110 0116 0116 0106 0106 fa0a  ................
+00009760: 090a 0206 010a 0106 010a 0104 0112 0210  ................
+00009770: 0108 010e 0108 0108 020c 0108 0114 0114  ................
+00009780: 0114 0106 0114 0106 0114 0114 0108 0104  ................
+00009790: 0272 9601 0000 7292 0000 0029 0172 da00  .r....r....).r..
+000097a0: 0000 296b da08 746f 7263 682e 6e6e 7243  ..)k..torch.nnrC
+000097b0: 0000 00da 0c74 7261 6e73 666f 726d 6572  .....transformer
+000097c0: 7372 0200 0000 7203 0000 0072 0400 0000  sr....r....r....
+000097d0: 7205 0000 0072 0600 0000 7207 0000 0072  r....r....r....r
+000097e0: 0800 0000 7209 0000 0072 0a00 0000 720b  ....r....r....r.
+000097f0: 0000 0072 0c00 0000 720d 0000 0072 0e00  ...r....r....r..
+00009800: 0000 720f 0000 0072 dc00 0000 da06 7061  ..r....r......pa
+00009810: 6e64 6173 7299 0000 0072 8e01 0000 72b9  ndasr....r....r.
+00009820: 0000 0072 6401 0000 da03 6173 7472 9e00  ...rd.....astr..
+00009830: 0000 723c 0100 00da 0770 7961 7272 6f77  ..r<.....pyarrow
+00009840: 729b 0000 00da 0f70 7961 7272 6f77 2e64  r......pyarrow.d
+00009850: 6174 6173 6574 da07 6461 7461 7365 74da  ataset..dataset.
+00009860: 0264 73da 0b74 6f72 6368 2e6f 7074 696d  .ds..torch.optim
+00009870: 7210 0000 00da 1074 6f72 6368 2e75 7469  r......torch.uti
+00009880: 6c73 2e64 6174 6172 1100 0000 723e 0000  ls.datar....r>..
+00009890: 00da 0974 7164 6d2e 6175 746f 7212 0000  ...tqdm.autor...
+000098a0: 00da 0a73 7461 7469 7374 6963 73da 0474  ...statistics..t
+000098b0: 696d 6572 fc00 0000 da02 7370 720c 0100  imer......spr...
+000098c0: 00da 1773 6b6c 6561 726e 2e6d 6f64 656c  ...sklearn.model
+000098d0: 5f73 656c 6563 7469 6f6e 7213 0000 00da  _selectionr.....
+000098e0: 046a 736f 6e72 bf00 0000 7272 0000 00da  .jsonr....rr....
+000098f0: 0b73 6369 7079 2e73 7461 7473 da05 7374  .scipy.stats..st
+00009900: 6174 73da 0861 7267 7061 7273 65da 066f  ats..argparse..o
+00009910: 7065 6e61 69da 0c72 616e 646f 6d5f 7374  penai..random_st
+00009920: 6174 65da 0473 6565 64da 0b6d 616e 7561  ate..seed..manua
+00009930: 6c5f 7365 6564 7263 0000 00da 0765 6e76  l_seedrc.....env
+00009940: 6972 6f6e 5a21 6172 6573 2e52 4147 5f41  ironZ!ares.RAG_A
 00009950: 7574 6f6d 6174 6963 5f45 7661 6c75 6174  utomatic_Evaluat
-00009960: 696f 6e2e 4576 616c 7561 7469 6f6e 5f46  ion.Evaluation_F
-00009970: 756e 6374 696f 6e73 721c 0000 0072 1d00  unctionsr....r..
-00009980: 0000 721e 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
-00009990: 0072 2100 0000 7222 0000 0072 2300 0000  .r!...r"...r#...
-000099a0: 7224 0000 0072 2500 0000 7226 0000 0072  r$...r%...r&...r
-000099b0: 2700 0000 7228 0000 00da 064d 6f64 756c  '...r(.....Modul
-000099c0: 6572 2900 0000 727e 0000 00da 0464 6963  er)...r~.....dic
-000099d0: 7472 8500 0000 729a 0000 0072 6200 0000  tr....r....rb...
-000099e0: 72ad 0000 00da 076e 6461 7272 6179 72c1  r......ndarrayr.
-000099f0: 0000 00da 0574 7570 6c65 72ce 0000 0072  .....tupler....r
-00009a00: f600 0000 72d7 0000 0072 d800 0000 72d9  ....r....r....r.
-00009a10: 0000 0072 e100 0000 72f2 0000 0072 0701  ...r....r....r..
-00009a20: 0000 723f 0100 0072 0f01 0000 7218 0100  ..r?...r....r...
-00009a30: 0072 5301 0000 7256 0100 0072 5801 0000  .rS...rV...rX...
-00009a40: 7268 0100 0072 6901 0000 da06 5365 7269  rh...ri.....Seri
-00009a50: 6573 726f 0100 0072 7201 0000 727c 0100  esro...rr...r|..
-00009a60: 0072 9101 0000 724c 0000 0072 4c00 0000  .r....rL...rL...
-00009a70: 724c 0000 0072 4d00 0000 da08 3c6d 6f64  rL...rM.....<mod
-00009a80: 756c 653e 0100 0000 73fe 0000 000c 0040  ule>....s......@
-00009a90: 0108 0708 0108 0108 0108 0108 0108 0108  ................
-00009aa0: 010c 010c 010c 0108 010c 0108 0108 0108  ................
-00009ab0: 0108 010c 0108 0108 0108 010c 0108 0108  ................
-00009ac0: 010c 0108 0104 030c 020a 010a 010e 010a  ................
-00009ad0: 010a 0114 023c 0112 0a14 5d12 150c 0e02  .....<....].....
-00009ae0: 0102 ff02 0102 ff02 010a ff0e 3404 0102  ............4...
-00009af0: ff02 0102 ff02 0102 ff02 010a ff0e 3802  ..............8.
-00009b00: 0102 ff04 010a ff12 1c12 1a1e 1016 4f12  ..............O.
-00009b10: 2f16 251c 1812 2400 7f16 1312 111c 0c16  /.%...$.........
-00009b20: 2502 2004 0102 ff04 0202 fe02 0302 fd02  %. .............
-00009b30: 0402 fc02 0502 fb02 0602 fa02 0702 f902  ................
-00009b40: 0802 f802 0902 f704 0a02 f602 0b02 f502  ................
-00009b50: 0c02 f402 0d0a f300 7f02 0202 0102 ff04  ................
-00009b60: 0202 fe02 0302 fd02 0402 fc02 0502 fb02  ................
-00009b70: 0602 fa02 0702 f902 0802 f802 0902 f702  ................
-00009b80: 0a02 f602 0b0a f50e 3712 39              ........7.9
+00009960: 696f 6e2e 7070 6972 1900 0000 721a 0000  ion.ppir....r...
+00009970: 0072 1b00 0000 5a32 6172 6573 2e52 4147  .r....Z2ares.RAG
+00009980: 5f41 7574 6f6d 6174 6963 5f45 7661 6c75  _Automatic_Evalu
+00009990: 6174 696f 6e2e 4576 616c 7561 7469 6f6e  ation.Evaluation
+000099a0: 5f46 756e 6374 696f 6e73 721c 0000 0072  _Functionsr....r
+000099b0: 1d00 0000 721e 0000 0072 1f00 0000 7220  ....r....r....r 
+000099c0: 0000 0072 2100 0000 7222 0000 0072 2300  ...r!...r"...r#.
+000099d0: 0000 7224 0000 0072 2500 0000 7226 0000  ..r$...r%...r&..
+000099e0: 0072 2700 0000 7228 0000 00da 064d 6f64  .r'...r(.....Mod
+000099f0: 756c 6572 2900 0000 727e 0000 00da 0464  uler)...r~.....d
+00009a00: 6963 7472 8500 0000 729a 0000 0072 6200  ictr....r....rb.
+00009a10: 0000 72ad 0000 00da 076e 6461 7272 6179  ..r......ndarray
+00009a20: 72c1 0000 00da 0574 7570 6c65 72ce 0000  r......tupler...
+00009a30: 0072 f600 0000 72d7 0000 0072 d800 0000  .r....r....r....
+00009a40: 72d9 0000 0072 e100 0000 72f2 0000 0072  r....r....r....r
+00009a50: 0701 0000 723f 0100 0072 0f01 0000 7218  ....r?...r....r.
+00009a60: 0100 0072 5301 0000 7256 0100 0072 5801  ...rS...rV...rX.
+00009a70: 0000 7268 0100 0072 6901 0000 da06 5365  ..rh...ri.....Se
+00009a80: 7269 6573 726f 0100 0072 7201 0000 727c  riesro...rr...r|
+00009a90: 0100 0072 9601 0000 724c 0000 0072 4c00  ...r....rL...rL.
+00009aa0: 0000 724c 0000 0072 4d00 0000 da08 3c6d  ..rL...rM.....<m
+00009ab0: 6f64 756c 653e 0100 0000 73fe 0000 000c  odule>....s.....
+00009ac0: 0040 0108 0708 0108 0108 0108 0108 0108  .@..............
+00009ad0: 0108 010c 010c 010c 0108 010c 0108 0108  ................
+00009ae0: 0108 0108 010c 0108 0108 0108 010c 0108  ................
+00009af0: 0108 010c 0108 0104 030c 020a 010a 010e  ................
+00009b00: 010a 010a 0114 023c 0112 0a14 5d12 150c  .......<....]...
+00009b10: 0e02 0102 ff02 0102 ff02 010a ff0e 3404  ..............4.
+00009b20: 0102 ff02 0102 ff02 0102 ff02 010a ff0e  ................
+00009b30: 3802 0102 ff04 010a ff12 1c12 1a1e 1016  8...............
+00009b40: 4f12 2f16 251c 1812 2400 7f16 1312 111c  O./.%...$.......
+00009b50: 0c16 2502 2004 0102 ff04 0202 fe02 0302  ..%. ...........
+00009b60: fd02 0402 fc02 0502 fb02 0602 fa02 0702  ................
+00009b70: f902 0802 f802 0902 f704 0a02 f602 0b02  ................
+00009b80: f502 0c02 f402 0d0a f300 7f02 0202 0102  ................
+00009b90: ff04 0202 fe02 0302 fd02 0402 fc02 0502  ................
+00009ba0: fb02 0602 fa02 0702 f902 0802 f802 0902  ................
+00009bb0: f702 0a02 f602 0b0a f50e 3712 39         ..........7.9
```

### Comparing `ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-311.pyc` & `ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-310.pyc` & `ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-311.pyc` & `ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-310.pyc` & `ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-311.pyc` & `ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/ares.cpython-310.pyc` & `ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/ares.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-310.pyc` & `ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-311.pyc` & `ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/RAG_Automatic_Evaluation/ppi.py` & `ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/ppi.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/__pycache__/ares.cpython-310.pyc` & `ares_ai-0.5.9/ares/__pycache__/ares.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/__pycache__/ares.cpython-311.pyc` & `ares_ai-0.5.9/ares/__pycache__/ares.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/__pycache__/binary_classifier.cpython-310.pyc` & `ares_ai-0.5.9/ares/__pycache__/binary_classifier.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/__pycache__/binary_classifier.cpython-311.pyc` & `ares_ai-0.5.9/ares/__pycache__/binary_classifier.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/__pycache__/prompts.cpython-310.pyc` & `ares_ai-0.5.9/ares/__pycache__/prompts.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/__pycache__/rag_scoring.cpython-310.pyc` & `ares_ai-0.5.9/ares/__pycache__/rag_scoring.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue May 21 06:06:15 2024 UTC, .py size: 8433 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 d739 4c66 f120 0000  o........9Lf. ..
+00000000: 6f0d 0d0a 0000 0000 2ddf 5766 4b21 0000  o.......-.WfK!..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 7000 0000 6400  .....@...sp...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c00  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c00 6d03 5a03  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c00 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c00 6d05 5a05 0100 6400 6406 6c00  d.l.m.Z...d.d.l.
 00000070: 6d06 5a06 0100 6400 6407 6c00 6d07 5a07  m.Z...d.d.l.m.Z.
@@ -43,258 +43,261 @@
 000002a0: 6174 3a20 275b 5b59 6573 5d5d 2720 6966  at: '[[Yes]]' if
 000002b0: 2074 6865 2064 6f63 756d 656e 7420 6973   the document is
 000002c0: 2073 7566 6669 6369 656e 7420 616e 6420   sufficient and 
 000002d0: 275b 5b4e 6f5d 5d27 2069 6620 7468 6520  '[[No]]' if the 
 000002e0: 646f 6375 6d65 6e74 2070 726f 7669 6465  document provide
 000002f0: 6420 6973 206e 6f74 2073 7566 6669 6369  d is not suffici
 00000300: 656e 742e 6313 0000 0000 0000 0000 0000  ent.c...........
-00000310: 0032 0000 0012 0000 0003 0000 0073 a602  .2...........s..
+00000310: 0033 0000 0012 0000 0003 0000 0073 aa02  .3...........s..
 00000320: 0000 7c03 6401 6b02 7210 8800 6401 6b03  ..|.d.k.r...d.k.
 00000330: 730c 7c10 6401 6b03 7210 7400 6402 8301  s.|.d.k.r.t.d...
 00000340: 8201 7c0a 6401 6b02 721c 7c11 6401 6b02  ..|.d.k.r.|.d.k.
 00000350: 721c 7400 6403 8301 8201 7c04 7230 8800  r.t.d.....|.r0..
 00000360: 7228 8800 6401 6b03 7228 7401 6404 8301  r(..d.k.r(t.d...
 00000370: 0100 8701 8702 6602 6405 6406 8408 7d13  ......f.d.d...}.
 00000380: 6e12 8800 723e 8800 6401 6b03 723e 8700  n...r>..d.k.r>..
 00000390: 8703 6602 6407 6406 8408 7d13 6e04 7400  ..f.d.d...}.n.t.
 000003a0: 6408 8301 8201 7c04 724a 7402 7c04 7c05  d.....|.rJt.|.|.
 000003b0: 8302 7d14 6e07 6409 640a 8400 7c05 4400  ..}.n.d.d...|.D.
-000003c0: 8301 7d14 7c14 4400 5dfd 5c02 7d15 7d16  ..}.|.D.].\.}.}.
-000003d0: 6700 7d17 6700 7d18 6700 7d19 6700 7d1a  g.}.g.}.g.}.g.}.
-000003e0: 6700 7d1b 7c02 4400 5dec 7d1c 7403 7c02  g.}.|.D.].}.t.|.
-000003f0: 7c04 7c05 7c03 8304 7d1d 7404 7c0b 8301  |.|.|...}.t.|...
-00000400: 5c03 7d1e 7d1f 7d20 7405 7c1c 7c16 7c05  \.}.}.} t.|.|.|.
-00000410: 8303 5c02 7d21 7d22 7c13 7c15 8301 5c03  ..\.}!}"|.|...\.
-00000420: 7d23 7d24 7d25 6900 640b 7c21 9301 640c  }#}$}%i.d.|!..d.
-00000430: 7c16 9301 640d 7c22 9301 640e 7c25 9301  |...d.|"..d.|%..
-00000440: 640f 7c15 9301 6410 7c24 9301 6411 7c23  d.|...d.|$..d.|#
-00000450: 9301 6412 7c08 9301 6413 8801 9301 6414  ..d.|...d.....d.
-00000460: 7c1e 9301 6415 7c1f 9301 6416 7c20 9301  |...d.|...d.| ..
-00000470: 6417 7c03 9301 6418 8800 9301 6419 8803  d.|...d.....d...
-00000480: 9301 641a 7c0d 9301 641b 7c0e 9301 641c  ..d.|...d.|...d.
-00000490: 7c0f 6901 a501 7d26 7406 7c26 8301 5c04  |.i...}&t.|&..\.
-000004a0: 7d27 7d28 7d29 7d2a 6900 640f 7c15 9301  }'}(})}*i.d.|...
-000004b0: 640b 7c21 9301 640c 7c16 9301 641d 7c27  d.|!..d.|...d.|'
-000004c0: 9301 641e 7c05 9301 641f 7c0a 9301 6410  ..d.|...d.|...d.
-000004d0: 7c24 9301 6412 7c08 9301 640e 7c25 9301  |$..d.|...d.|%..
-000004e0: 6420 7c11 9301 6421 7407 9301 6422 7c10  d |...d!t...d"|.
-000004f0: 9301 6419 8803 9301 641a 7c0d 9301 641c  ..d.....d.|...d.
-00000500: 7c0f 9301 641b 7c0e 9301 6423 7c1d 9301  |...d.|...d#|...
-00000510: 7d2b 7408 7c2b 8301 5c06 7d21 7d2c 7d2d  }+t.|+..\.}!},}-
-00000520: 7d2e 7d2f 7d30 6900 640b 7c21 9301 6424  }.}/}0i.d.|!..d$
-00000530: 7c2e 9301 6425 7c2c 9301 6426 7c2d 9301  |...d%|,..d&|-..
-00000540: 6427 7c2f 9301 6428 7c00 9301 6429 7c01  d'|/..d(|...d)|.
-00000550: 9301 6411 7c23 9301 640e 7c25 9301 6413  ..d.|#..d.|%..d.
-00000560: 8801 9301 6414 7c1e 9301 6415 7c1f 9301  ....d.|...d.|...
-00000570: 6416 7c20 9301 6423 7c1d 9301 642a 7c2a  d.| ..d#|...d*|*
-00000580: 9301 642b 7c30 9301 640c 7c16 9301 7c1c  ..d+|0..d.|...|.
-00000590: 7c17 7c18 7c19 7c1a 7c1b 7c29 7c15 8800  |.|.|.|.|.|)|...
-000005a0: 8803 7c0d 7c0e 7c0f 7c12 642c 9c0e a501  ..|.|.|.|.d,....
-000005b0: 7d31 7409 7c31 8301 0200 0100 0200 0100  }1t.|1..........
-000005c0: 5300 7153 642d 5300 292e 6164 0300 000a  S.qSd-S.).ad....
-000005d0: 2020 2020 436f 6e66 6967 7572 6573 2061      Configures a
-000005e0: 6e64 2072 756e 7320 7468 6520 5241 4720  nd runs the RAG 
-000005f0: 7363 6f72 696e 6720 7072 6f63 6573 732e  scoring process.
-00000600: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
-00000610: 3a0a 2020 2020 2d20 616c 7068 613a 2054  :.    - alpha: T
-00000620: 6865 2061 6c70 6861 2076 616c 7565 2066  he alpha value f
-00000630: 6f72 2074 6865 2073 636f 7269 6e67 2070  or the scoring p
-00000640: 726f 6365 7373 2e0a 2020 2020 2d20 6e75  rocess..    - nu
-00000650: 6d5f 7472 6961 6c73 3a20 4e75 6d62 6572  m_trials: Number
-00000660: 206f 6620 7472 6961 6c73 2074 6f20 7275   of trials to ru
-00000670: 6e2e 0a20 2020 202d 2065 7661 6c75 6174  n..    - evaluat
-00000680: 696f 6e5f 6461 7461 7365 7473 3a20 4c69  ion_datasets: Li
-00000690: 7374 206f 6620 6461 7461 7365 7473 2074  st of datasets t
-000006a0: 6f20 6576 616c 7561 7465 2e0a 2020 2020  o evaluate..    
-000006b0: 2d20 6665 775f 7368 6f74 5f65 7861 6d70  - few_shot_examp
-000006c0: 6c65 735f 6669 6c65 7061 7468 3a20 4669  les_filepath: Fi
-000006d0: 6c65 7061 7468 2066 6f72 2066 6577 2d73  lepath for few-s
-000006e0: 686f 7420 6578 616d 706c 6573 2e0a 2020  hot examples..  
-000006f0: 2020 2d20 6368 6563 6b70 6f69 6e74 733a    - checkpoints:
-00000700: 204c 6973 7420 6f66 206d 6f64 656c 2063   List of model c
-00000710: 6865 636b 706f 696e 7473 2e0a 2020 2020  heckpoints..    
-00000720: 2d20 6c61 6265 6c73 3a20 4c69 7374 206f  - labels: List o
-00000730: 6620 6c61 6265 6c73 2e0a 2020 2020 2d20  f labels..    - 
-00000740: 6d6f 6465 6c5f 6368 6f69 6365 3a20 4368  model_choice: Ch
-00000750: 6f69 6365 206f 6620 6d6f 6465 6c2e 0a20  oice of model.. 
-00000760: 2020 202d 206c 6c6d 5f6a 7564 6765 3a20     - llm_judge: 
-00000770: 4c4c 4d20 6a75 6467 6520 746f 2075 7365  LLM judge to use
-00000780: 2e0a 2020 2020 2d20 6173 7369 676e 6564  ..    - assigned
-00000790: 5f62 6174 6368 5f73 697a 653a 2042 6174  _batch_size: Bat
-000007a0: 6368 2073 697a 6520 746f 2075 7365 2e0a  ch size to use..
-000007b0: 2020 2020 2d20 6e75 6d62 6572 5f6f 665f      - number_of_
-000007c0: 6c61 6265 6c73 3a20 4e75 6d62 6572 206f  labels: Number o
-000007d0: 6620 6c61 6265 6c73 2e0a 2020 2020 2d20  f labels..    - 
-000007e0: 676f 6c64 5f6c 6162 656c 5f70 6174 683a  gold_label_path:
-000007f0: 2050 6174 6820 746f 2074 6865 2067 6f6c   Path to the gol
-00000800: 6420 6c61 6265 6c73 2e0a 2020 2020 2d20  d labels..    - 
-00000810: 7261 675f 7479 7065 3a20 5479 7065 206f  rag_type: Type o
-00000820: 6620 5241 472e 0a20 2020 202d 2076 6c6c  f RAG..    - vll
-00000830: 6d3a 2056 4c4c 4d20 746f 2075 7365 2e0a  m: VLLM to use..
-00000840: 2020 2020 2d20 686f 7374 5f75 726c 3a20      - host_url: 
-00000850: 486f 7374 2055 524c 2e0a 2020 2020 2d20  Host URL..    - 
-00000860: 7265 7175 6573 745f 6465 6c61 793a 2044  request_delay: D
-00000870: 656c 6179 2062 6574 7765 656e 2072 6571  elay between req
-00000880: 7565 7374 732e 0a20 2020 202d 2064 6562  uests..    - deb
-00000890: 7567 5f6d 6f64 653a 2057 6865 7468 6572  ug_mode: Whether
-000008a0: 2074 6f20 7275 6e20 696e 2064 6562 7567   to run in debug
-000008b0: 206d 6f64 652e 0a20 2020 202d 206d 6163   mode..    - mac
-000008c0: 6869 6e65 5f6c 6162 656c 5f6c 6c6d 5f6d  hine_label_llm_m
-000008d0: 6f64 656c 3a20 4d61 6368 696e 6520 6c61  odel: Machine la
-000008e0: 6265 6c20 4c4c 4d20 6d6f 6465 6c2e 0a20  bel LLM model.. 
-000008f0: 2020 202d 2067 6f6c 645f 6d61 6368 696e     - gold_machin
-00000900: 655f 6c61 6265 6c5f 7061 7468 3a20 5061  e_label_path: Pa
-00000910: 7468 2074 6f20 7468 6520 676f 6c64 206d  th to the gold m
-00000920: 6163 6869 6e65 206c 6162 656c 732e 0a20  achine labels.. 
-00000930: 2020 20da 044e 6f6e 657a 4927 6665 775f     ..NonezI'few_
-00000940: 7368 6f74 5f65 7861 6d70 6c65 735f 6669  shot_examples_fi
-00000950: 6c65 7061 7468 2720 6361 6e6e 6f74 2062  lepath' cannot b
-00000960: 6520 4e6f 6e65 2069 6620 6765 6e65 7261  e None if genera
-00000970: 7469 6e67 206d 6163 6869 6e65 206c 6162  ting machine lab
-00000980: 656c 732e 7a47 4569 7468 6572 2027 676f  els.zGEither 'go
-00000990: 6c64 5f6c 6162 656c 5f70 6174 6827 206f  ld_label_path' o
-000009a0: 7220 2767 6f6c 645f 6d61 6368 696e 655f  r 'gold_machine_
-000009b0: 6c61 6265 6c5f 7061 7468 2720 6d75 7374  label_path' must
-000009c0: 2062 6520 7072 6f76 6964 6564 2e7a 4857   be provided.zHW
-000009d0: 6172 6e69 6e67 3a20 426f 7468 2063 6865  arning: Both che
-000009e0: 636b 706f 696e 7420 616e 6420 6c6c 6d5f  ckpoint and llm_
-000009f0: 6a75 6467 6520 7765 7265 2070 726f 7669  judge were provi
-00000a00: 6465 642e 2055 7369 6e67 2063 6865 636b  ded. Using check
-00000a10: 706f 696e 7473 2e63 0100 0000 0000 0000  points.c........
-00000a20: 0000 0000 0100 0000 0400 0000 1300 0000  ................
-00000a30: 730c 0000 0074 0088 0088 017c 0083 0353  s....t.....|...S
-00000a40: 00a9 014e 7207 0000 0029 01da 0363 686b  ...Nr....)...chk
-00000a50: 2902 da0c 6d6f 6465 6c5f 6368 6f69 6365  )...model_choice
-00000a60: da10 6e75 6d62 6572 5f6f 665f 6c61 6265  ..number_of_labe
-00000a70: 6c73 a900 fa2b 2f66 7574 7572 652f 752f  ls...+/future/u/
-00000a80: 6d61 6e69 6861 6e69 2f41 5245 532f 6172  manihani/ARES/ar
-00000a90: 6573 2f72 6167 5f73 636f 7269 6e67 2e70  es/rag_scoring.p
-00000aa0: 79da 083c 6c61 6d62 6461 3e38 0000 0073  y..<lambda>8...s
-00000ab0: 0200 0000 0c00 7a24 7261 675f 7363 6f72  ......z$rag_scor
-00000ac0: 696e 675f 636f 6e66 6967 2e3c 6c6f 6361  ing_config.<loca
-00000ad0: 6c73 3e2e 3c6c 616d 6264 613e 6301 0000  ls>.<lambda>c...
-00000ae0: 0000 0000 0000 0000 0001 0000 0003 0000  ................
-00000af0: 0013 0000 0073 0a00 0000 7400 8800 8801  .....s....t.....
-00000b00: 8302 5300 720d 0000 0072 0500 0000 2901  ..S.r....r....).
-00000b10: da01 5f29 02da 096c 6c6d 5f6a 7564 6765  .._)...llm_judge
-00000b20: da04 766c 6c6d 7211 0000 0072 1200 0000  ..vllmr....r....
-00000b30: 7213 0000 003a 0000 0073 0200 0000 0a00  r....:...s......
-00000b40: 7a26 4e6f 2076 616c 6964 206d 6f64 656c  z&No valid model
-00000b50: 206f 7220 6368 6563 6b70 6f69 6e74 2070   or checkpoint p
-00000b60: 726f 7669 6465 642e 6301 0000 0000 0000  rovided.c.......
-00000b70: 0000 0000 0002 0000 0003 0000 0073 0000  .............s..
-00000b80: 0073 1800 0000 8100 7c00 5d07 7d01 6400  .s......|.].}.d.
-00000b90: 7c01 6602 5600 0100 7102 6400 5300 720d  |.f.V...q.d.S.r.
-00000ba0: 0000 0072 1100 0000 2902 da02 2e30 da05  ...r....)....0..
-00000bb0: 6c61 6265 6c72 1100 0000 7211 0000 0072  labelr....r....r
-00000bc0: 1200 0000 da09 3c67 656e 6578 7072 3e44  ......<genexpr>D
-00000bd0: 0000 0073 0400 0000 0280 1600 7a25 7261  ...s........z%ra
-00000be0: 675f 7363 6f72 696e 675f 636f 6e66 6967  g_scoring_config
-00000bf0: 2e3c 6c6f 6361 6c73 3e2e 3c67 656e 6578  .<locals>.<genex
-00000c00: 7072 3eda 0874 6573 745f 7365 74da 0c6c  pr>..test_set..l
-00000c10: 6162 656c 5f63 6f6c 756d 6eda 0b74 6578  abel_column..tex
-00000c20: 745f 636f 6c75 6d6e da06 6465 7669 6365  t_column..device
-00000c30: da0a 6368 6563 6b70 6f69 6e74 da09 746f  ..checkpoint..to
-00000c40: 6b65 6e69 7a65 72da 056d 6f64 656c da13  kenizer..model..
-00000c50: 6173 7369 676e 6564 5f62 6174 6368 5f73  assigned_batch_s
-00000c60: 697a 6572 0f00 0000 da1f 636f 6e74 6578  izer......contex
-00000c70: 745f 7265 6c65 7661 6e63 655f 7379 7374  t_relevance_syst
-00000c80: 656d 5f70 726f 6d70 74da 2161 6e73 7765  em_prompt.!answe
-00000c90: 725f 6661 6974 6866 756c 6e65 7373 5f73  r_faithfulness_s
-00000ca0: 7973 7465 6d5f 7072 6f6d 7074 da1e 616e  ystem_prompt..an
-00000cb0: 7377 6572 5f72 656c 6576 616e 6365 5f73  swer_relevance_s
-00000cc0: 7973 7465 6d5f 7072 6f6d 7074 da1a 6665  ystem_prompt..fe
-00000cd0: 775f 7368 6f74 5f65 7861 6d70 6c65 735f  w_shot_examples_
-00000ce0: 6669 6c65 7061 7468 7215 0000 0072 1600  filepathr....r..
-00000cf0: 0000 da08 686f 7374 5f75 726c da0d 7265  ....host_url..re
-00000d00: 7175 6573 745f 6465 6c61 79da 0a64 6562  quest_delay..deb
-00000d10: 7567 5f6d 6f64 65da 1174 6f74 616c 5f70  ug_mode..total_p
-00000d20: 7265 6469 6374 696f 6e73 da06 6c61 6265  redictions..labe
-00000d30: 6c73 da0f 676f 6c64 5f6c 6162 656c 5f70  ls..gold_label_p
-00000d40: 6174 68da 1767 6f6c 645f 6d61 6368 696e  ath..gold_machin
-00000d50: 655f 6c61 6265 6c5f 7061 7468 da1b 6d61  e_label_path..ma
-00000d60: 6368 696e 655f 6c61 6265 6c5f 7379 7374  chine_label_syst
-00000d70: 656d 5f70 726f 6d70 74da 176d 6163 6869  em_prompt..machi
-00000d80: 6e65 5f6c 6162 656c 5f6c 6c6d 5f6d 6f64  ne_label_llm_mod
-00000d90: 656c da11 6665 775f 7368 6f74 5f65 7861  el..few_shot_exa
-00000da0: 6d70 6c65 73da 1559 5f6c 6162 656c 6564  mples..Y_labeled
-00000db0: 5f70 7265 6469 6374 696f 6e73 da11 595f  _predictions..Y_
-00000dc0: 6c61 6265 6c65 645f 6461 7461 7365 74da  labeled_dataset.
-00000dd0: 1459 5f6c 6162 656c 6564 5f64 6174 616c  .Y_labeled_datal
-00000de0: 6f61 6465 72da 1659 6861 745f 756e 6c61  oader..Yhat_unla
-00000df0: 6265 6c65 645f 6461 7461 7365 74da 0561  beled_dataset..a
-00000e00: 6c70 6861 da0a 6e75 6d5f 7472 6961 6c73  lpha..num_trials
-00000e10: da06 6d65 7472 6963 da11 7072 6564 6963  ..metric..predic
-00000e20: 7469 6f6e 5f63 6f6c 756d 6e29 0eda 1274  tion_column)...t
-00000e30: 6573 745f 7365 745f 7365 6c65 6374 696f  est_set_selectio
-00000e40: 6eda 1b4c 4c4d 5f6a 7564 6765 5f72 6174  n..LLM_judge_rat
-00000e50: 696f 5f70 7265 6469 6374 696f 6e73 da16  io_predictions..
-00000e60: 7661 6c69 6461 7469 6f6e 5f73 6574 5f6c  validation_set_l
-00000e70: 656e 6774 6873 da15 7661 6c69 6461 7469  engths..validati
-00000e80: 6f6e 5f73 6574 5f72 6174 696f 73da 1870  on_set_ratios..p
-00000e90: 7069 5f63 6f6e 6669 6465 6e63 655f 696e  pi_confidence_in
-00000ea0: 7465 7276 616c 73da 0f61 6363 7572 6163  tervals..accurac
-00000eb0: 795f 7363 6f72 6573 da07 7265 7375 6c74  y_scores..result
-00000ec0: 7372 1e00 0000 7215 0000 0072 1600 0000  sr....r....r....
-00000ed0: 7226 0000 0072 2700 0000 7228 0000 00da  r&...r'...r(....
-00000ee0: 1370 7265 6469 6374 696f 6e5f 6669 6c65  .prediction_file
-00000ef0: 7061 7468 4e29 0ada 0a56 616c 7565 4572  pathN)...ValueEr
-00000f00: 726f 72da 0570 7269 6e74 da03 7a69 7072  ror..print..zipr
-00000f10: 0200 0000 7203 0000 0072 0400 0000 7209  ....r....r....r.
-00000f20: 0000 0072 2d00 0000 720a 0000 0072 0b00  ...r-...r....r..
-00000f30: 0000 2932 7234 0000 0072 3500 0000 da13  ..)2r4...r5.....
-00000f40: 6576 616c 7561 7469 6f6e 5f64 6174 6173  evaluation_datas
-00000f50: 6574 7372 2500 0000 da0b 6368 6563 6b70  etsr%.....checkp
-00000f60: 6f69 6e74 7372 2a00 0000 720f 0000 0072  ointsr*...r....r
-00000f70: 1500 0000 7221 0000 0072 1000 0000 722b  ....r!...r....r+
-00000f80: 0000 00da 0872 6167 5f74 7970 6572 1600  .....rag_typer..
-00000f90: 0000 7226 0000 0072 2700 0000 7228 0000  ..r&...r'...r(..
-00000fa0: 0072 2e00 0000 722c 0000 0072 3f00 0000  .r....r,...r?...
-00000fb0: 5a0c 6d6f 6465 6c5f 6c6f 6164 6572 da08  Z.model_loader..
-00000fc0: 7061 6972 696e 6773 721e 0000 0072 1b00  pairingsr....r..
-00000fd0: 0000 7239 0000 0072 3a00 0000 723b 0000  ..r9...r:...r;..
-00000fe0: 0072 3c00 0000 723d 0000 0072 3800 0000  .r<...r=...r8...
-00000ff0: 722f 0000 0072 2200 0000 7223 0000 0072  r/...r"...r#...r
-00001000: 2400 0000 721a 0000 0072 1c00 0000 7220  $...r....r....r 
-00001010: 0000 0072 1f00 0000 721d 0000 005a 1365  ...r....r....Z.e
-00001020: 7661 6c5f 6d6f 6465 6c5f 7365 7474 696e  val_model_settin
-00001030: 6773 7229 0000 00da 1074 6f74 616c 5f72  gsr).....total_r
-00001040: 6566 6572 656e 6365 7372 3e00 0000 7236  eferencesr>...r6
-00001050: 0000 005a 1570 6f73 745f 7072 6f63 6573  ...Z.post_proces
-00001060: 735f 7365 7474 696e 6773 7231 0000 0072  s_settingsr1...r
-00001070: 3200 0000 7230 0000 0072 3300 0000 7237  2...r0...r3...r7
-00001080: 0000 005a 1965 7661 6c75 6174 655f 7363  ...Z.evaluate_sc
-00001090: 6f72 696e 675f 7365 7474 696e 6773 7211  oring_settingsr.
-000010a0: 0000 0029 0472 1500 0000 720f 0000 0072  ...).r....r....r
-000010b0: 1000 0000 7216 0000 0072 1200 0000 da12  ....r....r......
-000010c0: 7261 675f 7363 6f72 696e 675f 636f 6e66  rag_scoring_conf
-000010d0: 6967 1200 0000 7330 0100 0018 1b08 0110  ig....s0........
-000010e0: 0308 0104 030c 0108 0110 010c 0110 0108  ................
-000010f0: 0204 030c 020e 030c 0204 0104 0104 0104  ................
-00001100: 0104 0108 010e 020e 0210 020e 0202 0204  ................
-00001110: 0102 ff04 0202 fe04 0302 fd04 0402 fc04  ................
-00001120: 0502 fb04 0602 fa04 0702 f904 0802 f804  ................
-00001130: 0902 f704 0a02 f604 0b02 f504 0c02 f404  ................
-00001140: 0d02 f304 0e02 f204 0f02 f104 1002 f004  ................
-00001150: 1102 ef04 1206 ee10 1502 0204 0102 ff04  ................
-00001160: 0202 fe04 0302 fd04 0402 fc04 0502 fb04  ................
-00001170: 0602 fa04 0702 f904 0802 f804 0902 f704  ................
-00001180: 0a02 f604 0b02 f504 0c02 f404 0d02 f304  ................
-00001190: 0e02 f204 0f02 f104 1002 f004 1104 ef14  ................
-000011a0: 1402 0204 0102 ff04 0202 fe04 0302 fd04  ................
-000011b0: 0402 fc04 0502 fb04 0602 fa04 0702 f904  ................
-000011c0: 0802 f804 0902 f704 0a02 f604 0b02 f504  ................
-000011d0: 0c02 f404 0d02 f304 0e02 f204 0f02 f104  ................
-000011e0: 1002 f004 1102 ef02 1202 0102 0102 0102  ................
-000011f0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-00001200: 0102 0108 e110 2202 a704 fa72 4800 0000  ......"....rH...
-00001210: 4e29 0b5a 3b61 7265 732e 5241 475f 4175  N).Z;ares.RAG_Au
-00001220: 746f 6d61 7469 635f 4576 616c 7561 7469  tomatic_Evaluati
-00001230: 6f6e 2e4c 4c4d 4a75 6467 655f 5241 475f  on.LLMJudge_RAG_
-00001240: 436f 6d70 6172 6564 5f53 636f 7269 6e67  Compared_Scoring
-00001250: 7202 0000 0072 0300 0000 7204 0000 0072  r....r....r....r
-00001260: 0600 0000 7208 0000 0072 0900 0000 720a  ....r....r....r.
-00001270: 0000 0072 0b00 0000 722d 0000 0072 4800  ...r....r-...rH.
-00001280: 0000 7211 0000 0072 1100 0000 7211 0000  ..r....r....r...
-00001290: 0072 1200 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-000012a0: 0100 0000 7316 0000 000c 000c 010c 010c  ....s...........
-000012b0: 010c 010c 010c 010c 0102 0302 ff0c 08    ...............
+000003c0: 8301 7d14 6700 7d15 7c14 4400 5dfd 5c02  ..}.g.}.|.D.].\.
+000003d0: 7d16 7d17 6700 7d18 6700 7d19 6700 7d1a  }.}.g.}.g.}.g.}.
+000003e0: 6700 7d1b 6700 7d1c 7c02 4400 5dec 7d1d  g.}.g.}.|.D.].}.
+000003f0: 7403 7c02 7c04 7c05 7c03 8304 7d1e 7404  t.|.|.|.|...}.t.
+00000400: 7c0b 8301 5c03 7d1f 7d20 7d21 7405 7c1d  |...\.}.} }!t.|.
+00000410: 7c17 7c05 8303 5c02 7d22 7d23 7c13 7c16  |.|...\.}"}#|.|.
+00000420: 8301 5c03 7d24 7d25 7d26 6900 640b 7c22  ..\.}$}%}&i.d.|"
+00000430: 9301 640c 7c17 9301 640d 7c23 9301 640e  ..d.|...d.|#..d.
+00000440: 7c26 9301 640f 7c16 9301 6410 7c25 9301  |&..d.|...d.|%..
+00000450: 6411 7c24 9301 6412 7c08 9301 6413 8801  d.|$..d.|...d...
+00000460: 9301 6414 7c1f 9301 6415 7c20 9301 6416  ..d.|...d.| ..d.
+00000470: 7c21 9301 6417 7c03 9301 6418 8800 9301  |!..d.|...d.....
+00000480: 6419 8803 9301 641a 7c0d 9301 641b 7c0e  d.....d.|...d.|.
+00000490: 9301 641c 7c0f 6901 a501 7d27 7406 7c27  ..d.|.i...}'t.|'
+000004a0: 8301 5c04 7d28 7d29 7d2a 7d2b 6900 640f  ..\.}(})}*}+i.d.
+000004b0: 7c16 9301 640b 7c22 9301 640c 7c17 9301  |...d.|"..d.|...
+000004c0: 641d 7c28 9301 641e 7c05 9301 641f 7c0a  d.|(..d.|...d.|.
+000004d0: 9301 6410 7c25 9301 6412 7c08 9301 640e  ..d.|%..d.|...d.
+000004e0: 7c26 9301 6420 7c11 9301 6421 7407 9301  |&..d |...d!t...
+000004f0: 6422 7c10 9301 6419 8803 9301 641a 7c0d  d"|...d.....d.|.
+00000500: 9301 641c 7c0f 9301 641b 7c0e 9301 6423  ..d.|...d.|...d#
+00000510: 7c1e 9301 7d2c 7408 7c2c 8301 5c06 7d22  |...},t.|,..\.}"
+00000520: 7d2d 7d2e 7d2f 7d30 7d31 6900 640b 7c22  }-}.}/}0}1i.d.|"
+00000530: 9301 6424 7c2f 9301 6425 7c2d 9301 6426  ..d$|/..d%|-..d&
+00000540: 7c2e 9301 6427 7c30 9301 6428 7c00 9301  |...d'|0..d(|...
+00000550: 6429 7c01 9301 6411 7c24 9301 640e 7c26  d)|...d.|$..d.|&
+00000560: 9301 6413 8801 9301 6414 7c1f 9301 6415  ..d.....d.|...d.
+00000570: 7c20 9301 6416 7c21 9301 6423 7c1e 9301  | ..d.|!..d#|...
+00000580: 642a 7c2b 9301 642b 7c31 9301 640c 7c17  d*|+..d+|1..d.|.
+00000590: 9301 7c1d 7c18 7c19 7c1a 7c1b 7c1c 7c2a  ..|.|.|.|.|.|.|*
+000005a0: 7c16 8800 8803 7c0d 7c0e 7c0f 7c12 642c  |.....|.|.|.|.d,
+000005b0: 9c0e a501 7d32 7c15 a009 740a 7c32 8301  ....}2|...t.|2..
+000005c0: a101 0100 7165 7155 7c15 5300 292d 6164  ....qeqU|.S.)-ad
+000005d0: 0300 000a 2020 2020 436f 6e66 6967 7572  ....    Configur
+000005e0: 6573 2061 6e64 2072 756e 7320 7468 6520  es and runs the 
+000005f0: 5241 4720 7363 6f72 696e 6720 7072 6f63  RAG scoring proc
+00000600: 6573 732e 0a0a 2020 2020 5061 7261 6d65  ess...    Parame
+00000610: 7465 7273 3a0a 2020 2020 2d20 616c 7068  ters:.    - alph
+00000620: 613a 2054 6865 2061 6c70 6861 2076 616c  a: The alpha val
+00000630: 7565 2066 6f72 2074 6865 2073 636f 7269  ue for the scori
+00000640: 6e67 2070 726f 6365 7373 2e0a 2020 2020  ng process..    
+00000650: 2d20 6e75 6d5f 7472 6961 6c73 3a20 4e75  - num_trials: Nu
+00000660: 6d62 6572 206f 6620 7472 6961 6c73 2074  mber of trials t
+00000670: 6f20 7275 6e2e 0a20 2020 202d 2065 7661  o run..    - eva
+00000680: 6c75 6174 696f 6e5f 6461 7461 7365 7473  luation_datasets
+00000690: 3a20 4c69 7374 206f 6620 6461 7461 7365  : List of datase
+000006a0: 7473 2074 6f20 6576 616c 7561 7465 2e0a  ts to evaluate..
+000006b0: 2020 2020 2d20 6665 775f 7368 6f74 5f65      - few_shot_e
+000006c0: 7861 6d70 6c65 735f 6669 6c65 7061 7468  xamples_filepath
+000006d0: 3a20 4669 6c65 7061 7468 2066 6f72 2066  : Filepath for f
+000006e0: 6577 2d73 686f 7420 6578 616d 706c 6573  ew-shot examples
+000006f0: 2e0a 2020 2020 2d20 6368 6563 6b70 6f69  ..    - checkpoi
+00000700: 6e74 733a 204c 6973 7420 6f66 206d 6f64  nts: List of mod
+00000710: 656c 2063 6865 636b 706f 696e 7473 2e0a  el checkpoints..
+00000720: 2020 2020 2d20 6c61 6265 6c73 3a20 4c69      - labels: Li
+00000730: 7374 206f 6620 6c61 6265 6c73 2e0a 2020  st of labels..  
+00000740: 2020 2d20 6d6f 6465 6c5f 6368 6f69 6365    - model_choice
+00000750: 3a20 4368 6f69 6365 206f 6620 6d6f 6465  : Choice of mode
+00000760: 6c2e 0a20 2020 202d 206c 6c6d 5f6a 7564  l..    - llm_jud
+00000770: 6765 3a20 4c4c 4d20 6a75 6467 6520 746f  ge: LLM judge to
+00000780: 2075 7365 2e0a 2020 2020 2d20 6173 7369   use..    - assi
+00000790: 676e 6564 5f62 6174 6368 5f73 697a 653a  gned_batch_size:
+000007a0: 2042 6174 6368 2073 697a 6520 746f 2075   Batch size to u
+000007b0: 7365 2e0a 2020 2020 2d20 6e75 6d62 6572  se..    - number
+000007c0: 5f6f 665f 6c61 6265 6c73 3a20 4e75 6d62  _of_labels: Numb
+000007d0: 6572 206f 6620 6c61 6265 6c73 2e0a 2020  er of labels..  
+000007e0: 2020 2d20 676f 6c64 5f6c 6162 656c 5f70    - gold_label_p
+000007f0: 6174 683a 2050 6174 6820 746f 2074 6865  ath: Path to the
+00000800: 2067 6f6c 6420 6c61 6265 6c73 2e0a 2020   gold labels..  
+00000810: 2020 2d20 7261 675f 7479 7065 3a20 5479    - rag_type: Ty
+00000820: 7065 206f 6620 5241 472e 0a20 2020 202d  pe of RAG..    -
+00000830: 2076 6c6c 6d3a 2056 4c4c 4d20 746f 2075   vllm: VLLM to u
+00000840: 7365 2e0a 2020 2020 2d20 686f 7374 5f75  se..    - host_u
+00000850: 726c 3a20 486f 7374 2055 524c 2e0a 2020  rl: Host URL..  
+00000860: 2020 2d20 7265 7175 6573 745f 6465 6c61    - request_dela
+00000870: 793a 2044 656c 6179 2062 6574 7765 656e  y: Delay between
+00000880: 2072 6571 7565 7374 732e 0a20 2020 202d   requests..    -
+00000890: 2064 6562 7567 5f6d 6f64 653a 2057 6865   debug_mode: Whe
+000008a0: 7468 6572 2074 6f20 7275 6e20 696e 2064  ther to run in d
+000008b0: 6562 7567 206d 6f64 652e 0a20 2020 202d  ebug mode..    -
+000008c0: 206d 6163 6869 6e65 5f6c 6162 656c 5f6c   machine_label_l
+000008d0: 6c6d 5f6d 6f64 656c 3a20 4d61 6368 696e  lm_model: Machin
+000008e0: 6520 6c61 6265 6c20 4c4c 4d20 6d6f 6465  e label LLM mode
+000008f0: 6c2e 0a20 2020 202d 2067 6f6c 645f 6d61  l..    - gold_ma
+00000900: 6368 696e 655f 6c61 6265 6c5f 7061 7468  chine_label_path
+00000910: 3a20 5061 7468 2074 6f20 7468 6520 676f  : Path to the go
+00000920: 6c64 206d 6163 6869 6e65 206c 6162 656c  ld machine label
+00000930: 732e 0a20 2020 20da 044e 6f6e 657a 4927  s..    ..NonezI'
+00000940: 6665 775f 7368 6f74 5f65 7861 6d70 6c65  few_shot_example
+00000950: 735f 6669 6c65 7061 7468 2720 6361 6e6e  s_filepath' cann
+00000960: 6f74 2062 6520 4e6f 6e65 2069 6620 6765  ot be None if ge
+00000970: 6e65 7261 7469 6e67 206d 6163 6869 6e65  nerating machine
+00000980: 206c 6162 656c 732e 7a47 4569 7468 6572   labels.zGEither
+00000990: 2027 676f 6c64 5f6c 6162 656c 5f70 6174   'gold_label_pat
+000009a0: 6827 206f 7220 2767 6f6c 645f 6d61 6368  h' or 'gold_mach
+000009b0: 696e 655f 6c61 6265 6c5f 7061 7468 2720  ine_label_path' 
+000009c0: 6d75 7374 2062 6520 7072 6f76 6964 6564  must be provided
+000009d0: 2e7a 4857 6172 6e69 6e67 3a20 426f 7468  .zHWarning: Both
+000009e0: 2063 6865 636b 706f 696e 7420 616e 6420   checkpoint and 
+000009f0: 6c6c 6d5f 6a75 6467 6520 7765 7265 2070  llm_judge were p
+00000a00: 726f 7669 6465 642e 2055 7369 6e67 2063  rovided. Using c
+00000a10: 6865 636b 706f 696e 7473 2e63 0100 0000  heckpoints.c....
+00000a20: 0000 0000 0000 0000 0100 0000 0400 0000  ................
+00000a30: 1300 0000 730c 0000 0074 0088 0088 017c  ....s....t.....|
+00000a40: 0083 0353 00a9 014e 7207 0000 0029 01da  ...S...Nr....)..
+00000a50: 0363 686b 2902 da0c 6d6f 6465 6c5f 6368  .chk)...model_ch
+00000a60: 6f69 6365 da10 6e75 6d62 6572 5f6f 665f  oice..number_of_
+00000a70: 6c61 6265 6c73 a900 fa2b 2f66 7574 7572  labels...+/futur
+00000a80: 652f 752f 6d61 6e69 6861 6e69 2f41 5245  e/u/manihani/ARE
+00000a90: 532f 6172 6573 2f72 6167 5f73 636f 7269  S/ares/rag_scori
+00000aa0: 6e67 2e70 79da 083c 6c61 6d62 6461 3e38  ng.py..<lambda>8
+00000ab0: 0000 0073 0200 0000 0c00 7a24 7261 675f  ...s......z$rag_
+00000ac0: 7363 6f72 696e 675f 636f 6e66 6967 2e3c  scoring_config.<
+00000ad0: 6c6f 6361 6c73 3e2e 3c6c 616d 6264 613e  locals>.<lambda>
+00000ae0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00000af0: 0003 0000 0013 0000 0073 0a00 0000 7400  .........s....t.
+00000b00: 8800 8801 8302 5300 720d 0000 0072 0500  ......S.r....r..
+00000b10: 0000 2901 da01 5f29 02da 096c 6c6d 5f6a  ..)..._)...llm_j
+00000b20: 7564 6765 da04 766c 6c6d 7211 0000 0072  udge..vllmr....r
+00000b30: 1200 0000 7213 0000 003a 0000 0073 0200  ....r....:...s..
+00000b40: 0000 0a00 7a26 4e6f 2076 616c 6964 206d  ....z&No valid m
+00000b50: 6f64 656c 206f 7220 6368 6563 6b70 6f69  odel or checkpoi
+00000b60: 6e74 2070 726f 7669 6465 642e 6301 0000  nt provided.c...
+00000b70: 0000 0000 0000 0000 0002 0000 0003 0000  ................
+00000b80: 0073 0000 0073 1800 0000 8100 7c00 5d07  .s...s......|.].
+00000b90: 7d01 6400 7c01 6602 5600 0100 7102 6400  }.d.|.f.V...q.d.
+00000ba0: 5300 720d 0000 0072 1100 0000 2902 da02  S.r....r....)...
+00000bb0: 2e30 da05 6c61 6265 6c72 1100 0000 7211  .0..labelr....r.
+00000bc0: 0000 0072 1200 0000 da09 3c67 656e 6578  ...r......<genex
+00000bd0: 7072 3e44 0000 0073 0400 0000 0280 1600  pr>D...s........
+00000be0: 7a25 7261 675f 7363 6f72 696e 675f 636f  z%rag_scoring_co
+00000bf0: 6e66 6967 2e3c 6c6f 6361 6c73 3e2e 3c67  nfig.<locals>.<g
+00000c00: 656e 6578 7072 3eda 0874 6573 745f 7365  enexpr>..test_se
+00000c10: 74da 0c6c 6162 656c 5f63 6f6c 756d 6eda  t..label_column.
+00000c20: 0b74 6578 745f 636f 6c75 6d6e da06 6465  .text_column..de
+00000c30: 7669 6365 da0a 6368 6563 6b70 6f69 6e74  vice..checkpoint
+00000c40: da09 746f 6b65 6e69 7a65 72da 056d 6f64  ..tokenizer..mod
+00000c50: 656c da13 6173 7369 676e 6564 5f62 6174  el..assigned_bat
+00000c60: 6368 5f73 697a 6572 0f00 0000 da1f 636f  ch_sizer......co
+00000c70: 6e74 6578 745f 7265 6c65 7661 6e63 655f  ntext_relevance_
+00000c80: 7379 7374 656d 5f70 726f 6d70 74da 2161  system_prompt.!a
+00000c90: 6e73 7765 725f 6661 6974 6866 756c 6e65  nswer_faithfulne
+00000ca0: 7373 5f73 7973 7465 6d5f 7072 6f6d 7074  ss_system_prompt
+00000cb0: da1e 616e 7377 6572 5f72 656c 6576 616e  ..answer_relevan
+00000cc0: 6365 5f73 7973 7465 6d5f 7072 6f6d 7074  ce_system_prompt
+00000cd0: da1a 6665 775f 7368 6f74 5f65 7861 6d70  ..few_shot_examp
+00000ce0: 6c65 735f 6669 6c65 7061 7468 7215 0000  les_filepathr...
+00000cf0: 0072 1600 0000 da08 686f 7374 5f75 726c  .r......host_url
+00000d00: da0d 7265 7175 6573 745f 6465 6c61 79da  ..request_delay.
+00000d10: 0a64 6562 7567 5f6d 6f64 65da 1174 6f74  .debug_mode..tot
+00000d20: 616c 5f70 7265 6469 6374 696f 6e73 da06  al_predictions..
+00000d30: 6c61 6265 6c73 da0f 676f 6c64 5f6c 6162  labels..gold_lab
+00000d40: 656c 5f70 6174 68da 1767 6f6c 645f 6d61  el_path..gold_ma
+00000d50: 6368 696e 655f 6c61 6265 6c5f 7061 7468  chine_label_path
+00000d60: da1b 6d61 6368 696e 655f 6c61 6265 6c5f  ..machine_label_
+00000d70: 7379 7374 656d 5f70 726f 6d70 74da 176d  system_prompt..m
+00000d80: 6163 6869 6e65 5f6c 6162 656c 5f6c 6c6d  achine_label_llm
+00000d90: 5f6d 6f64 656c da11 6665 775f 7368 6f74  _model..few_shot
+00000da0: 5f65 7861 6d70 6c65 73da 1559 5f6c 6162  _examples..Y_lab
+00000db0: 656c 6564 5f70 7265 6469 6374 696f 6e73  eled_predictions
+00000dc0: da11 595f 6c61 6265 6c65 645f 6461 7461  ..Y_labeled_data
+00000dd0: 7365 74da 1459 5f6c 6162 656c 6564 5f64  set..Y_labeled_d
+00000de0: 6174 616c 6f61 6465 72da 1659 6861 745f  ataloader..Yhat_
+00000df0: 756e 6c61 6265 6c65 645f 6461 7461 7365  unlabeled_datase
+00000e00: 74da 0561 6c70 6861 da0a 6e75 6d5f 7472  t..alpha..num_tr
+00000e10: 6961 6c73 da06 6d65 7472 6963 da11 7072  ials..metric..pr
+00000e20: 6564 6963 7469 6f6e 5f63 6f6c 756d 6e29  ediction_column)
+00000e30: 0eda 1274 6573 745f 7365 745f 7365 6c65  ...test_set_sele
+00000e40: 6374 696f 6eda 1b4c 4c4d 5f6a 7564 6765  ction..LLM_judge
+00000e50: 5f72 6174 696f 5f70 7265 6469 6374 696f  _ratio_predictio
+00000e60: 6e73 da16 7661 6c69 6461 7469 6f6e 5f73  ns..validation_s
+00000e70: 6574 5f6c 656e 6774 6873 da15 7661 6c69  et_lengths..vali
+00000e80: 6461 7469 6f6e 5f73 6574 5f72 6174 696f  dation_set_ratio
+00000e90: 73da 1870 7069 5f63 6f6e 6669 6465 6e63  s..ppi_confidenc
+00000ea0: 655f 696e 7465 7276 616c 73da 0f61 6363  e_intervals..acc
+00000eb0: 7572 6163 795f 7363 6f72 6573 da07 7265  uracy_scores..re
+00000ec0: 7375 6c74 7372 1e00 0000 7215 0000 0072  sultsr....r....r
+00000ed0: 1600 0000 7226 0000 0072 2700 0000 7228  ....r&...r'...r(
+00000ee0: 0000 00da 1370 7265 6469 6374 696f 6e5f  .....prediction_
+00000ef0: 6669 6c65 7061 7468 290b da0a 5661 6c75  filepath)...Valu
+00000f00: 6545 7272 6f72 da05 7072 696e 74da 037a  eError..print..z
+00000f10: 6970 7202 0000 0072 0300 0000 7204 0000  ipr....r....r...
+00000f20: 0072 0900 0000 722d 0000 0072 0a00 0000  .r....r-...r....
+00000f30: da06 6170 7065 6e64 720b 0000 0029 3372  ..appendr....)3r
+00000f40: 3400 0000 7235 0000 00da 1365 7661 6c75  4...r5.....evalu
+00000f50: 6174 696f 6e5f 6461 7461 7365 7473 7225  ation_datasetsr%
+00000f60: 0000 00da 0b63 6865 636b 706f 696e 7473  .....checkpoints
+00000f70: 722a 0000 0072 0f00 0000 7215 0000 0072  r*...r....r....r
+00000f80: 2100 0000 7210 0000 0072 2b00 0000 da08  !...r....r+.....
+00000f90: 7261 675f 7479 7065 7216 0000 0072 2600  rag_typer....r&.
+00000fa0: 0000 7227 0000 0072 2800 0000 722e 0000  ..r'...r(...r...
+00000fb0: 0072 2c00 0000 723f 0000 005a 0c6d 6f64  .r,...r?...Z.mod
+00000fc0: 656c 5f6c 6f61 6465 72da 0870 6169 7269  el_loader..pairi
+00000fd0: 6e67 735a 1661 6c6c 5f65 7661 6c75 6174  ngsZ.all_evaluat
+00000fe0: 696f 6e5f 7265 7375 6c74 7372 1e00 0000  ion_resultsr....
+00000ff0: 721b 0000 0072 3900 0000 723a 0000 0072  r....r9...r:...r
+00001000: 3b00 0000 723c 0000 0072 3d00 0000 7238  ;...r<...r=...r8
+00001010: 0000 0072 2f00 0000 7222 0000 0072 2300  ...r/...r"...r#.
+00001020: 0000 7224 0000 0072 1a00 0000 721c 0000  ..r$...r....r...
+00001030: 0072 2000 0000 721f 0000 0072 1d00 0000  .r ...r....r....
+00001040: 5a13 6576 616c 5f6d 6f64 656c 5f73 6574  Z.eval_model_set
+00001050: 7469 6e67 7372 2900 0000 da10 746f 7461  tingsr).....tota
+00001060: 6c5f 7265 6665 7265 6e63 6573 723e 0000  l_referencesr>..
+00001070: 0072 3600 0000 5a15 706f 7374 5f70 726f  .r6...Z.post_pro
+00001080: 6365 7373 5f73 6574 7469 6e67 7372 3100  cess_settingsr1.
+00001090: 0000 7232 0000 0072 3000 0000 7233 0000  ..r2...r0...r3..
+000010a0: 0072 3700 0000 5a19 6576 616c 7561 7465  .r7...Z.evaluate
+000010b0: 5f73 636f 7269 6e67 5f73 6574 7469 6e67  _scoring_setting
+000010c0: 7372 1100 0000 2904 7215 0000 0072 0f00  sr....).r....r..
+000010d0: 0000 7210 0000 0072 1600 0000 7212 0000  ..r....r....r...
+000010e0: 00da 1272 6167 5f73 636f 7269 6e67 5f63  ...rag_scoring_c
+000010f0: 6f6e 6669 6712 0000 0073 3201 0000 181b  onfig....s2.....
+00001100: 0801 1003 0801 0403 0c01 0801 1001 0c01  ................
+00001110: 1001 0802 0403 0c02 0e03 0402 0c01 0401  ................
+00001120: 0401 0401 0401 0401 0801 0e02 0e02 1002  ................
+00001130: 0e02 0202 0401 02ff 0402 02fe 0403 02fd  ................
+00001140: 0404 02fc 0405 02fb 0406 02fa 0407 02f9  ................
+00001150: 0408 02f8 0409 02f7 040a 02f6 040b 02f5  ................
+00001160: 040c 02f4 040d 02f3 040e 02f2 040f 02f1  ................
+00001170: 0410 02f0 0411 02ef 0412 06ee 1015 0202  ................
+00001180: 0401 02ff 0402 02fe 0403 02fd 0404 02fc  ................
+00001190: 0405 02fb 0406 02fa 0407 02f9 0408 02f8  ................
+000011a0: 0409 02f7 040a 02f6 040b 02f5 040c 02f4  ................
+000011b0: 040d 02f3 040e 02f2 040f 02f1 0410 02f0  ................
+000011c0: 0411 04ef 1414 0202 0401 02ff 0402 02fe  ................
+000011d0: 0403 02fd 0404 02fc 0405 02fb 0406 02fa  ................
+000011e0: 0407 02f9 0408 02f8 0409 02f7 040a 02f6  ................
+000011f0: 040b 02f5 040c 02f4 040d 02f3 040e 02f2  ................
+00001200: 040f 02f1 0410 02f0 0411 02ef 0212 0201  ................
+00001210: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00001220: 0201 0201 0201 0201 08e1 1022 02a7 045b  ..........."...[
+00001230: 7249 0000 004e 290b 5a3b 6172 6573 2e52  rI...N).Z;ares.R
+00001240: 4147 5f41 7574 6f6d 6174 6963 5f45 7661  AG_Automatic_Eva
+00001250: 6c75 6174 696f 6e2e 4c4c 4d4a 7564 6765  luation.LLMJudge
+00001260: 5f52 4147 5f43 6f6d 7061 7265 645f 5363  _RAG_Compared_Sc
+00001270: 6f72 696e 6772 0200 0000 7203 0000 0072  oringr....r....r
+00001280: 0400 0000 7206 0000 0072 0800 0000 7209  ....r....r....r.
+00001290: 0000 0072 0a00 0000 720b 0000 0072 2d00  ...r....r....r-.
+000012a0: 0000 7249 0000 0072 1100 0000 7211 0000  ..rI...r....r...
+000012b0: 0072 1100 0000 7212 0000 00da 083c 6d6f  .r....r......<mo
+000012c0: 6475 6c65 3e01 0000 0073 1600 0000 0c00  dule>....s......
+000012d0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0203  ................
+000012e0: 02ff 0c08                                ....
```

### Comparing `ares_ai-0.5.8/ares/__pycache__/rag_scoring.cpython-311.pyc` & `ares_ai-0.5.9/ares/__pycache__/rag_scoring.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/__pycache__/synthetic_generator.cpython-310.pyc` & `ares_ai-0.5.9/ares/__pycache__/synthetic_generator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/__pycache__/synthetic_generator.cpython-311.pyc` & `ares_ai-0.5.9/ares/__pycache__/synthetic_generator.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/__pycache__/ues_idp.cpython-310.pyc` & `ares_ai-0.5.9/ares/__pycache__/ues_idp.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/__pycache__/ues_idp.cpython-311.pyc` & `ares_ai-0.5.9/ares/__pycache__/ues_idp.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/ares.py` & `ares_ai-0.5.9/ares/ares.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/ares_ai.egg-info/PKG-INFO` & `ares_ai-0.5.9/ares/ares_ai.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/ares_ai.egg-info/requires.txt` & `ares_ai-0.5.9/ares/ares_ai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/binary_classifier.py` & `ares_ai-0.5.9/ares/binary_classifier.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/prompts.py` & `ares_ai-0.5.9/ares/prompts.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/rag_scoring.py` & `ares_ai-0.5.9/ares/rag_scoring.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     if checkpoints:
         # Here we assume that the length of checkpoints and labels is the same
         pairings = zip(checkpoints, labels)
     else:
         # If no checkpoints, create dummy pairs for labels with None for checkpoint
         pairings = ((None, label) for label in labels)
 
+    all_evaluation_results = []
     for checkpoint, label_column in pairings:
         LLM_judge_ratio_predictions = []
         validation_set_lengths = []
         validation_set_ratios = []
         ppi_confidence_intervals = []
         accuracy_scores = []
         for test_set_selection in evaluation_datasets:
@@ -158,9 +159,10 @@
                 "vllm": vllm,
                 "host_url": host_url,
                 "request_delay": request_delay,
                 "debug_mode": debug_mode,
                 "prediction_filepath": prediction_filepath
             }
             
-            return evaluate_and_scoring_data(evaluate_scoring_settings)
-            
+            all_evaluation_results.append(evaluate_and_scoring_data(evaluate_scoring_settings))
+            
+    return all_evaluation_results
```

### Comparing `ares_ai-0.5.8/ares/synthetic_generator.py` & `ares_ai-0.5.9/ares/synthetic_generator.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares/ues_idp.py` & `ares_ai-0.5.9/ares/ues_idp.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares_ai.egg-info/PKG-INFO` & `ares_ai-0.5.9/ares_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ares-ai
-Version: 0.5.8
+Version: 0.5.9
 Summary: ARES is an advanced evaluation framework for Retrieval-Augmented Generation (RAG) systems, 
 Author-email: Jon Saad-Falcon <jonsaadfalcon@stanford.edu>, Robby Manihani <manihani@stanford.edu>, Omar Khattab <okhattab@stanford.edu>, Christopher Potts <cgpotts@stanford.edu>, Matei Zaharia <matei@berkeley.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -246,15 +246,16 @@
 Requires-Dist: sentencepiece==0.1.99
 Requires-Dist: sentence-transformers<3.0.0,>=2.2.2
 Requires-Dist: spacy<4.0.0,>=3.5.3
 Requires-Dist: torch>=2.2.1
 Requires-Dist: together>=1.1.0
 Requires-Dist: tokenizers>=0.13.3
 Requires-Dist: transformers==4.40.1
-Requires-Dist: vllm==0.4.1
+Provides-Extra: vllm
+Requires-Dist: vllm==0.4.1; extra == "vllm"
 
 <h2 align="center">ARES: An Automated Evaluation Framework for Retrieval-Augmented Generation Systems</h2>
 
 <p align="center">
   <a>Table of Contents:</a>
   <a href="#section1">Installation</a> |
   <a href="#section2">Requirements</a> |
@@ -284,15 +285,15 @@
   <a>
   <img alt="Static Badge" src="https://img.shields.io/badge/Made%20with-Python-red?style=flat&link=https%3A%2F%2Fpython.org%2F">
   </a>
 
 </p>
 
 
-ARES is a groundbreaking framework for evaluating Retrieval-Augmented Generation (RAG) models. The automated process combines synthetic data generation with fine-tuned classifiers to efficiently assess context relevance, answer faithfulness, and answer relevance, minimizing the need for extensive human annotations. ARES employs synthetic query generation and Precision-Performance Iteration (PPI), providing accurate evaluations with statistical confidence.
+ARES is a groundbreaking framework for evaluating Retrieval-Augmented Generation (RAG) models. The automated process combines synthetic data generation with fine-tuned classifiers to efficiently assess context relevance, answer faithfulness, and answer relevance, minimizing the need for extensive human annotations. ARES employs synthetic query generation and Prediction-Powered Inference (PPI), providing accurate evaluations with statistical confidence.
 
 
 ### 💬 Mini Q&A
 <hr>
 
 **What does ARES assess in RAG models?**
```

### Comparing `ares_ai-0.5.8/ares_ai.egg-info/SOURCES.txt` & `ares_ai-0.5.9/ares_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.8/ares_ai.egg-info/requires.txt` & `ares_ai-0.5.9/ares_ai.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -26,8 +26,10 @@
 sentencepiece==0.1.99
 sentence-transformers<3.0.0,>=2.2.2
 spacy<4.0.0,>=3.5.3
 torch>=2.2.1
 together>=1.1.0
 tokenizers>=0.13.3
 transformers==4.40.1
+
+[vllm]
 vllm==0.4.1
```

### Comparing `ares_ai-0.5.8/pyproject.toml` & `ares_ai-0.5.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=45", "wheel", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ares-ai"
-version = "0.5.8"
+version = "0.5.9"
 description = """ 
 ARES is an advanced evaluation framework for Retrieval-Augmented Generation (RAG) systems, 
 utilizing fine-tuned classifiers and synthetic data to assess performance efficiently. It streamlines 
 the evaluation of context relevance, answer faithfulness, and answer relevance with minimal human annotations.
 """
 readme = "README.md"
 authors = [
@@ -61,17 +61,19 @@
     "sentencepiece==0.1.99",
     "sentence-transformers >=2.2.2,<3.0.0",
     "spacy >=3.5.3,<4.0.0",
     "torch >= 2.2.1",
     "together >= 1.1.0",
     "tokenizers >=0.13.3",
     "transformers == 4.40.1",
-    "vllm == 0.4.1",
 ]
 
+[project.optional-dependencies]
+vllm = ["vllm == 0.4.1"]
+
 [project.urls]
 documentation = "https://github.com/stanford-futuredata/ARES/tree/new-dev/docs"
 repository = "https://github.com/stanford-futuredata/ARES/tree/main"
 changelog = "https://github.com/stanford-futuredata/ARES/blob/new-dev/CHANGELOG.md"
 
 [project.scripts]
 ares-cli = "ares.cli:main"
```

### Comparing `ares_ai-0.5.8/requirements.txt` & `ares_ai-0.5.9/requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -206,15 +206,15 @@
 pyzmq==25.0.2
 pyzstd==0.15.7
 qtconsole==5.4.3
 QtPy==2.3.1
 questionary==1.10.0
 rank-bm25==0.2.2
 regex==2023.5.5
-requests==2.31.0
+requests==2.32.0
 responses==0.18.0
 rfc3339-validator==0.1.4
 rfc3986-validator==0.1.1
 rich==13.5.2
 ruamel.yaml.clib==0.2.7
 ruamel.yaml==0.17.32
 s3transfer==0.6.2
```

