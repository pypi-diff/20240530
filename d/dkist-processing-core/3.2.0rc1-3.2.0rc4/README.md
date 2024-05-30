# Comparing `tmp/dkist-processing-core-3.2.0rc1.tar.gz` & `tmp/dkist-processing-core-3.2.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-processing-core-3.2.0rc1.tar", last modified: Wed May 29 15:51:01 2024, max compression
+gzip compressed data, was "dkist-processing-core-3.2.0rc4.tar", last modified: Thu May 30 18:01:40 2024, max compression
```

## Comparing `dkist-processing-core-3.2.0rc1.tar` & `dkist-processing-core-3.2.0rc4.tar`

### file list

```diff
@@ -1,62 +1,65 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 15:51:01.800341 dkist-processing-core-3.2.0rc1/
--rw-rw-rw-   0 root         (0) root         (0)     2448 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      811 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      306 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)     5659 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     8063 2024-05-29 15:51:01.800341 dkist-processing-core-3.2.0rc1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7449 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2913 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 15:51:01.796341 dkist-processing-core-3.2.0rc1/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/changelog/.gitempty
--rw-rw-rw-   0 root         (0) root         (0)       70 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/changelog/33.bugfix.rst
--rw-rw-rw-   0 root         (0) root         (0)      166 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/changelog/34.misc.rst
--rwxrwxrwx   0 root         (0) root         (0)      436 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 15:51:01.796341 dkist-processing-core-3.2.0rc1/dkist_processing_core/
--rw-rw-rw-   0 root         (0) root         (0)      440 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3033 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/_config.py
--rw-rw-rw-   0 root         (0) root         (0)     3311 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/_failure_callback.py
--rw-rw-rw-   0 root         (0) root         (0)     5532 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/_node.py
--rw-rw-rw-   0 root         (0) root         (0)     6096 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/build_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      256 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/resource_queue.py
--rw-rw-rw-   0 root         (0) root         (0)     9294 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/task.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 15:51:01.796341 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/
--rw-rw-rw-   0 root         (0) root         (0)       12 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4505 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/conftest.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 15:51:01.800341 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/invalid_workflow_package/
--rw-rw-rw-   0 root         (0) root         (0)       12 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/invalid_workflow_package/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      470 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/invalid_workflow_package/workflow.py
--rw-rw-rw-   0 root         (0) root         (0)     1039 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/task_example.py
--rw-rw-rw-   0 root         (0) root         (0)     3490 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/test_build_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2563 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/test_export.py
--rw-rw-rw-   0 root         (0) root         (0)     3118 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/test_failure_callback.py
--rw-rw-rw-   0 root         (0) root         (0)     4565 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/test_node.py
--rw-rw-rw-   0 root         (0) root         (0)     2487 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/test_task.py
--rw-rw-rw-   0 root         (0) root         (0)     4348 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/test_workflow.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 15:51:01.800341 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/valid_workflow_package/
--rw-rw-rw-   0 root         (0) root         (0)       12 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/valid_workflow_package/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      721 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/valid_workflow_package/workflow.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 15:51:01.800341 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/zero_node_workflow_package/
--rw-rw-rw-   0 root         (0) root         (0)       32 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/zero_node_workflow_package/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      227 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/zero_node_workflow_package/workflow.py
--rw-rw-rw-   0 root         (0) root         (0)    10181 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/workflow.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 15:51:01.796341 dkist-processing-core-3.2.0rc1/dkist_processing_core.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     8063 2024-05-29 15:51:01.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1733 2024-05-29 15:51:01.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-29 15:51:01.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      348 2024-05-29 15:51:01.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-05-29 15:51:01.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 15:51:01.800341 dkist-processing-core-3.2.0rc1/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)    85295 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/docs/auto-proc-concept-model.png
--rw-rw-rw-   0 root         (0) root         (0)    26060 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/docs/auto_proc_brick.png
--rw-rw-rw-   0 root         (0) root         (0)   267222 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/docs/automated-processing-deployed.png
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1854 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      103 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/docs/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 15:51:01.800341 dkist-processing-core-3.2.0rc1/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      776 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1549 2024-05-29 15:51:01.800341 dkist-processing-core-3.2.0rc1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-30 18:01:40.271090 dkist-processing-core-3.2.0rc4/
+-rw-rw-rw-   0 root         (0) root         (0)     2448 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      811 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      306 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5659 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8804 2024-05-30 18:01:40.271090 dkist-processing-core-3.2.0rc4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     8190 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2913 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-30 18:01:40.267090 dkist-processing-core-3.2.0rc4/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/changelog/.gitempty
+-rw-rw-rw-   0 root         (0) root         (0)       70 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/changelog/33.bugfix.rst
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/changelog/34.misc.rst
+-rwxrwxrwx   0 root         (0) root         (0)      436 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-30 18:01:40.267090 dkist-processing-core-3.2.0rc4/dkist_processing_core/
+-rw-rw-rw-   0 root         (0) root         (0)      440 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/dkist_processing_core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3088 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/dkist_processing_core/_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3311 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/dkist_processing_core/_failure_callback.py
+-rw-rw-rw-   0 root         (0) root         (0)     5532 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/dkist_processing_core/_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     5477 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/dkist_processing_core/build_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      256 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/dkist_processing_core/resource_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     9294 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/dkist_processing_core/task.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-30 18:01:40.267090 dkist-processing-core-3.2.0rc4/dkist_processing_core/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/dkist_processing_core/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4505 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/dkist_processing_core/tests/conftest.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-30 18:01:40.267090 dkist-processing-core-3.2.0rc4/dkist_processing_core/tests/invalid_workflow_cyclic/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/dkist_processing_core/tests/invalid_workflow_cyclic/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      620 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/dkist_processing_core/tests/invalid_workflow_cyclic/workflow.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-30 18:01:40.267090 dkist-processing-core-3.2.0rc4/dkist_processing_core/tests/invalid_workflow_for_docker_multi_category/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/dkist_processing_core/tests/invalid_workflow_for_docker_multi_category/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      499 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/dkist_processing_core/tests/invalid_workflow_for_docker_multi_category/workflow.py
+-rw-rw-rw-   0 root         (0) root         (0)     1039 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/dkist_processing_core/tests/task_example.py
+-rw-rw-rw-   0 root         (0) root         (0)     4280 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/dkist_processing_core/tests/test_build_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2563 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/dkist_processing_core/tests/test_export.py
+-rw-rw-rw-   0 root         (0) root         (0)     3118 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/dkist_processing_core/tests/test_failure_callback.py
+-rw-rw-rw-   0 root         (0) root         (0)     4565 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/dkist_processing_core/tests/test_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     2487 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/dkist_processing_core/tests/test_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     4935 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/dkist_processing_core/tests/test_workflow.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-30 18:01:40.267090 dkist-processing-core-3.2.0rc4/dkist_processing_core/tests/valid_workflow_package/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/dkist_processing_core/tests/valid_workflow_package/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      721 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/dkist_processing_core/tests/valid_workflow_package/workflow.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-30 18:01:40.271090 dkist-processing-core-3.2.0rc4/dkist_processing_core/tests/zero_node_workflow_package/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/dkist_processing_core/tests/zero_node_workflow_package/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      227 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/dkist_processing_core/tests/zero_node_workflow_package/workflow.py
+-rw-rw-rw-   0 root         (0) root         (0)    10067 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/dkist_processing_core/workflow.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-30 18:01:40.267090 dkist-processing-core-3.2.0rc4/dkist_processing_core.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     8804 2024-05-30 18:01:40.000000 dkist-processing-core-3.2.0rc4/dkist_processing_core.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1897 2024-05-30 18:01:40.000000 dkist-processing-core-3.2.0rc4/dkist_processing_core.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-30 18:01:40.000000 dkist-processing-core-3.2.0rc4/dkist_processing_core.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      348 2024-05-30 18:01:40.000000 dkist-processing-core-3.2.0rc4/dkist_processing_core.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-05-30 18:01:40.000000 dkist-processing-core-3.2.0rc4/dkist_processing_core.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-30 18:01:40.271090 dkist-processing-core-3.2.0rc4/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)    85295 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/docs/auto-proc-concept-model.png
+-rw-rw-rw-   0 root         (0) root         (0)    26060 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/docs/auto_proc_brick.png
+-rw-rw-rw-   0 root         (0) root         (0)   267222 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/docs/automated-processing-deployed.png
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1854 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      103 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/docs/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-30 18:01:40.271090 dkist-processing-core-3.2.0rc4/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      776 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1549 2024-05-30 18:01:40.271090 dkist-processing-core-3.2.0rc4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2024-05-30 18:01:35.000000 dkist-processing-core-3.2.0rc4/setup.py
```

### Comparing `dkist-processing-core-3.2.0rc1/.gitignore` & `dkist-processing-core-3.2.0rc4/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.2.0rc1/.pre-commit-config.yaml` & `dkist-processing-core-3.2.0rc4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.2.0rc1/CHANGELOG.rst` & `dkist-processing-core-3.2.0rc4/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.2.0rc1/PKG-INFO` & `dkist-processing-core-3.2.0rc4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-core
-Version: 3.2.0rc1
+Version: 3.2.0rc4
 Summary: Abstraction layer that is used by the DKIST Science Data Processing pipelines to process DKIST data using Apache Airflow.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-core/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/core
 Classifier: Programming Language :: Python
@@ -110,27 +110,47 @@
    * - BUILD_VERSION
      - Build/Export pipelines only.  This is the value that will be appended to all artifacts and represents their unique version
      - STR
      - dev
    * - MESH_CONFIG
      - Provides the dkistdc cloud mesh configuration.  Specifically the location of the message broker
      - JSON
-     -
+     - ``{}``
    * - ISB_USERNAME
      - Message broker user name
      - STR
-     -
+     - guest
    * - ISB_PASSWORD
      - Message broker password
      - STR
-     -
+     - guest
    * - ISB_EXCHANGE
      - Message Broker Exchange name for publishing messages
      - STR
+     - master.direct.x
+   * - ISB_QUEUE_TYPE
+     - Message Broker queue type for transporting messages
+     - STR
+     - classic
+   * - ELASTIC_APM_SERVICE_NAME
+     - Service Name used by Elastic Application Performance Monitoring
+     - STR
      -
+   * - ELASTIC_APM_OTHER_OPTIONS
+     - Dictionary of configuration for the Elastic Application Performance Monitoring client
+     - STR
+     - ``{}``
+   * - ELASTIC_APM_ENABLED
+     - Flag to disable/enable Elastic Application Performance Monitoring client calls which are chatty if not connected to an APM server.
+     - BOOL
+     - FALSE
+   * - BUILD_VERSION
+     - Version of the pipeline.  When built this makes its way into the workflow or dag name.
+     - STR
+     - dev
 
 Development
 -----------
 .. code-block:: bash
 
     git clone git@bitbucket.org:dkistdc/dkist-processing-core.git
     cd dkist-processing-core
```

### Comparing `dkist-processing-core-3.2.0rc1/README.rst` & `dkist-processing-core-3.2.0rc4/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -94,27 +94,47 @@
    * - BUILD_VERSION
      - Build/Export pipelines only.  This is the value that will be appended to all artifacts and represents their unique version
      - STR
      - dev
    * - MESH_CONFIG
      - Provides the dkistdc cloud mesh configuration.  Specifically the location of the message broker
      - JSON
-     -
+     - ``{}``
    * - ISB_USERNAME
      - Message broker user name
      - STR
-     -
+     - guest
    * - ISB_PASSWORD
      - Message broker password
      - STR
-     -
+     - guest
    * - ISB_EXCHANGE
      - Message Broker Exchange name for publishing messages
      - STR
+     - master.direct.x
+   * - ISB_QUEUE_TYPE
+     - Message Broker queue type for transporting messages
+     - STR
+     - classic
+   * - ELASTIC_APM_SERVICE_NAME
+     - Service Name used by Elastic Application Performance Monitoring
+     - STR
      -
+   * - ELASTIC_APM_OTHER_OPTIONS
+     - Dictionary of configuration for the Elastic Application Performance Monitoring client
+     - STR
+     - ``{}``
+   * - ELASTIC_APM_ENABLED
+     - Flag to disable/enable Elastic Application Performance Monitoring client calls which are chatty if not connected to an APM server.
+     - BOOL
+     - FALSE
+   * - BUILD_VERSION
+     - Version of the pipeline.  When built this makes its way into the workflow or dag name.
+     - STR
+     - dev
 
 Development
 -----------
 .. code-block:: bash
 
     git clone git@bitbucket.org:dkistdc/dkist-processing-core.git
     cd dkist-processing-core
```

### Comparing `dkist-processing-core-3.2.0rc1/bitbucket-pipelines.yml` & `dkist-processing-core-3.2.0rc4/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.2.0rc1/dkist_processing_core/_config.py` & `dkist-processing-core-3.2.0rc4/dkist_processing_core/_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,21 +6,22 @@
 from talus import Exchange
 from talus.models.connection_parameters import ConnectionParameterFactory
 
 
 class DKISTProcessingCoreConfiguration(MeshServiceConfigurationBase):
     """Environment configurations for dkist_processing_core."""
 
-    isb_username: str = "guest"
-    isb_password: str = "guest"
-    isb_exchange: str = "master.direct.x"
-    isb_queue_type: str = "classic"  # "quorum" or "classic"
-    elastic_apm_service_name: str = "dkist-processing-core"
+    isb_username: str = Field(default="guest")
+    isb_password: str = Field(default="guest")
+    isb_exchange: str = Field(default="master.direct.x")
+    isb_queue_type: str = Field(default="classic")
+    elastic_apm_service_name: str = Field(default="dkist-processing-core")
     elastic_apm_other_options: dict = Field(default_factory=dict)
     elastic_apm_enabled: bool = False
+    build_version: str = Field(default="dev")
 
     @property
     def isb_mesh_service(self) -> MeshService:
         """Return the mesh service details for the interservice-bus."""
         return self.service_mesh_detail(
             service_name="interservice-bus",
             default_mesh_service=MeshService(mesh_address="localhost", mesh_port=5672),
@@ -75,8 +76,7 @@
             "SERVER_URL": self.elastic_apm_server_url,
             "ENVIRONMENT": "Workflows",
             **self.elastic_apm_other_options,
         }
 
 
 core_configurations = DKISTProcessingCoreConfiguration()
-core_configurations.log_configurations()
```

### Comparing `dkist-processing-core-3.2.0rc1/dkist_processing_core/_failure_callback.py` & `dkist-processing-core-3.2.0rc4/dkist_processing_core/_failure_callback.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.2.0rc1/dkist_processing_core/_node.py` & `dkist-processing-core-3.2.0rc4/dkist_processing_core/_node.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.2.0rc1/dkist_processing_core/build_utils.py` & `dkist-processing-core-3.2.0rc4/dkist_processing_core/build_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """Utilities for the build pipeline."""
 import importlib
 from pathlib import Path
 from shutil import rmtree
 from types import ModuleType
 
-from airflow.models import DAG
-
 from dkist_processing_core import Workflow
 
 
 __all__ = ["validate_workflows", "export_dags", "export_notebook_dockerfile", "export_notebooks"]
 
 
 def validate_workflows(workflow_package: ModuleType, export_path: Path | None = None) -> None:
@@ -20,16 +18,14 @@
         export_path = Path("export/")
     workflows = _extract_workflows_from_package(workflow_package)
     try:
         _validate_workflows(workflows, export_path)
     finally:
         if rm_export_path_after_test:
             rmtree(export_path)
-    dags = [w.load() for w in workflows]
-    _validate_dags(dags)
 
 
 def export_dags(workflow_package: ModuleType, path: str | Path) -> list[Path]:
     """Export Airflow DAG files."""
     return [w.export_dag(path=path) for w in _extract_workflows_from_package(workflow_package)]
 
 
@@ -75,47 +71,33 @@
 
 
 def _parse_unprotected_modules_names_from_package(package: ModuleType) -> list[str]:
     package_path = Path(package.__path__[0])
     return [m.stem for m in package_path.glob("[!_]*.py")]
 
 
-def _validate_dags(dags: list[DAG]) -> None:
-    """Validate dags by ensuring they can be traversed without cycles and are syntactically correct."""
-    for d in dags:
-        try:
-            d.topological_sort()
-        except Exception as e:
-            raise SyntaxError(f"DAG {d.dag_id} malformed.  Parsing resulted in error: {e=}") from e
-
-
 def _validate_workflows(workflows: list[Workflow], export_path: Path) -> None:
     """Validate workflows by ensuring their exported version compiles as python and that there is at least one node."""
     for w in workflows:
-        try:
-            workflow_py = w.export_dag(path=export_path)
-            with workflow_py.open(mode="r") as f:
-                compile(f.read(), filename=f"{workflow_py.stem}.pyc", mode="exec")
-        except Exception as e:
-            raise SyntaxError(
-                f"Workflow {w.workflow_name} malformed. "
-                f"Parsing exported workflow resulted in error: {e=}"
-            ) from e
+        workflow_py = w.export_dag(path=export_path)
+        with workflow_py.open(mode="r") as f:
+            compile(f.read(), filename=f"{workflow_py.stem}.pyc", mode="exec")
         if len(w.nodes) == 0:
             raise ValueError(f"Workflow {w.workflow_name} has 0 nodes.")
 
 
 class NotebookDockerfile:
     """Build a Dockerfile for deployment as a Manual Processing Worker."""
 
     def __init__(self, notebook_paths: list[Path], category: str):
         self.notebook_paths = notebook_paths
+        self.validate_notebook_paths_are_relative()
         self.category = category
 
-    def notebook_paths_are_relative(self):
+    def validate_notebook_paths_are_relative(self):
         """Validate that the notebook paths are all relative."""
         return all([not p.is_absolute() for p in self.notebook_paths])
 
     @property
     def contents(self) -> str:
         """Return the Dockerfile body."""
         return "\n".join(self.preamble + self.setup + self.notebooks + self.command)
```

### Comparing `dkist-processing-core-3.2.0rc1/dkist_processing_core/task.py` & `dkist-processing-core-3.2.0rc4/dkist_processing_core/task.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/conftest.py` & `dkist-processing-core-3.2.0rc4/dkist_processing_core/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/task_example.py` & `dkist-processing-core-3.2.0rc4/dkist_processing_core/tests/task_example.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/test_build_utils.py` & `dkist-processing-core-3.2.0rc4/dkist_processing_core/tests/test_build_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,42 +2,51 @@
 import os
 import subprocess
 from pathlib import Path
 from shutil import rmtree
 
 import pytest
 from airflow.exceptions import AirflowException
+from airflow.exceptions import DuplicateTaskIdFound
 
 from dkist_processing_core.build_utils import export_dags
 from dkist_processing_core.build_utils import export_notebook_dockerfile
 from dkist_processing_core.build_utils import export_notebooks
 from dkist_processing_core.build_utils import validate_workflows
-from dkist_processing_core.tests import invalid_workflow_package
+from dkist_processing_core.tests import invalid_workflow_cyclic
+from dkist_processing_core.tests import invalid_workflow_for_docker_multi_category
 from dkist_processing_core.tests import valid_workflow_package
 from dkist_processing_core.tests import zero_node_workflow_package
 
 
 def test_validate_workflow_valid():
     """
     Given: A workflow package with a valid workflow.
     When: validating the workflow.
     Then: No errors raised.
     """
     validate_workflows(valid_workflow_package)
 
 
-def test_validate_workflow_invalid():
+@pytest.mark.parametrize(
+    "workflow_package",
+    [
+        invalid_workflow_cyclic,
+        zero_node_workflow_package,
+    ],
+)
+def test_validate_workflow_invalid(workflow_package):
     """
     Given: A workflow package with an invalid workflow.
     When: validating the workflow.
     Then: Errors raised.
     """
-    exceptions = (SyntaxError, AirflowException)
+    exceptions = (ValueError, DuplicateTaskIdFound)
     with pytest.raises(exceptions):
-        validate_workflows(invalid_workflow_package)
+        validate_workflows(workflow_package)
 
 
 def test_validate_workflow_zero_nodes():
     """
     Given: A workflow package with an invalid workflow of zero nodes.
     When: validating the workflow.
     Then: Errors raised.
@@ -99,7 +108,21 @@
     os.chdir(str(repository_root_path))
     print(Path.cwd())
     dockerfile_path = export_notebook_dockerfile(valid_workflow_package, notebook_export_path)
     assert dockerfile_path.exists()
     image_name = "test_export_notebook_dockerfile:latest"
     subprocess.run(["docker", "build", "-t", image_name, dockerfile_path.parent], check=True)
     dockerfile_path.unlink()
+
+
+@pytest.mark.long()
+def test_export_notebook_dockerfile_invalid_workflow_package(
+    repository_root_path, notebook_export_path
+):
+    """
+    Given: A path to export to and a package containing a valid workflow.
+    When: Workflows in the package are exported as a valid Dockerfile.
+    Then: Expected export file exists.
+    """
+    os.chdir(str(repository_root_path))
+    with pytest.raises(ValueError):
+        export_notebook_dockerfile(invalid_workflow_for_docker_multi_category, notebook_export_path)
```

### Comparing `dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/test_export.py` & `dkist-processing-core-3.2.0rc4/dkist_processing_core/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/test_failure_callback.py` & `dkist-processing-core-3.2.0rc4/dkist_processing_core/tests/test_failure_callback.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/test_node.py` & `dkist-processing-core-3.2.0rc4/dkist_processing_core/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/test_task.py` & `dkist-processing-core-3.2.0rc4/dkist_processing_core/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/test_workflow.py` & `dkist-processing-core-3.2.0rc4/dkist_processing_core/tests/test_workflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Callable
 
 import pytest
 from airflow import DAG
 
 from dkist_processing_core import ResourceQueue
 from dkist_processing_core import Workflow
+from dkist_processing_core.workflow import MAXIMUM_ALLOWED_WORKFLOW_NAME_LENGTH
 
 
 def test_workflow_metadata(workflow):
     """
     Given: A workflow instance.
     When: accessing attributes.
     Then: Tha values are properly assigned.
@@ -100,14 +101,32 @@
         )
         assert task.upstream_task_ids == task_upstream_expectations[task.task_id]
 
     ordered_nodes = workflow_instance.topological_sort()
     assert [node.task for node in ordered_nodes] == [TaskA, TaskB, TaskC, TaskD]
 
 
+def test_workflow_name_too_long():
+    """
+    Given: A workflow instance with a long name.
+    When: Accessing the workflow_name attribute.
+    Then: Get a ValueError.
+    """
+    with pytest.raises(ValueError):
+        Workflow(
+            input_data="".join(["a" for _ in range(MAXIMUM_ALLOWED_WORKFLOW_NAME_LENGTH)]),
+            output_data="",
+            category="",
+            detail="",
+            workflow_version="",
+            workflow_package=__package__,
+            tags="",
+        )
+
+
 def test_invalid_workflow_add_node(workflow):
     """
     Given: An invalid task (not inheriting from TaskBase)and a workflow instance.
     When: Adding the task to the workflow.
     Then: Get a TypeError.
     """
     workflow_instance, *args = workflow
```

### Comparing `dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/valid_workflow_package/workflow.py` & `dkist-processing-core-3.2.0rc4/dkist_processing_core/tests/valid_workflow_package/workflow.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.2.0rc1/dkist_processing_core/workflow.py` & `dkist-processing-core-3.2.0rc4/dkist_processing_core/workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Abstraction layer to construct a workflow as an airflow DAG."""
 import json
 import string
 from graphlib import TopologicalSorter
-from os import environ
 from pathlib import Path
 
 import nbformat as nbf
 from airflow import DAG
 
 from dkist_processing_core import ResourceQueue
+from dkist_processing_core._config import core_configurations
 from dkist_processing_core._node import Node
 from dkist_processing_core._node import task_type_hint
 from dkist_processing_core._node import upstreams_type_hint
 
 __all__ = ["Workflow"]
 
 MAXIMUM_ALLOWED_WORKFLOW_NAME_LENGTH = 100
@@ -52,15 +52,15 @@
         self,
         *,
         input_data: str,
         output_data: str,
         category: str,
         workflow_package: str,
         detail: str | None = None,
-        tags: list[str] | None = None,
+        tags: list[str] | str | None = None,
         workflow_version: str | None = None,
     ):
         """
         Create a workflow instance.
 
         Parameters
         ----------
@@ -76,46 +76,41 @@
 
         """
         self.workflow_package = workflow_package
         self.category = category
         self.input_data = input_data
         self.output_data = output_data
         self.detail = detail
-        self.workflow_name = self.get_workflow_name(
-            input_data=self.input_data,
-            output_data=self.output_data,
-            category=self.category,
-            detail=self.detail,
-        )
-        self.workflow_version = workflow_version or environ.get("BUILD_VERSION", "dev")
-        self.tags = tags or []
-        self._dag_name = f"{self.workflow_name}_{self.workflow_version}"
-        self.check_dag_name_characters(self._dag_name)
+        self.workflow_version = workflow_version or core_configurations.build_version
+        if isinstance(tags, str):
+            tags = [tags]
+        self.tags: list[str] = tags or []
         self._dag = self._initialize_local_dag()
         self.nodes = []
 
-    @staticmethod
-    def get_workflow_name(
-        *,
-        input_data: str,
-        output_data: str,
-        category: str,
-        detail: str = None,
-        **kwargs,
-    ) -> str:
-        """Create the workflow name from its constituent parts."""
-        workflow_name = f"{input_data}_to_{output_data}_{category}"
-        if detail:
-            workflow_name += f"_{detail}"
-        if len(workflow_name) > MAXIMUM_ALLOWED_WORKFLOW_NAME_LENGTH:
+    @property
+    def workflow_name(self) -> str:
+        """Return the workflow name created from its constituent parts."""
+        result = f"{self.input_data}_to_{self.output_data}_{self.category}"
+        if self.detail:
+            result += f"_{self.detail}"
+        workflow_name_too_long = len(result) > MAXIMUM_ALLOWED_WORKFLOW_NAME_LENGTH
+        if workflow_name_too_long:
             raise ValueError(
-                f"Workflow name {workflow_name} is {len(workflow_name)} characters long. "
+                f"Workflow name {result} is {len(result)} characters long. "
                 f"Limit is {MAXIMUM_ALLOWED_WORKFLOW_NAME_LENGTH} characters."
             )
-        return workflow_name
+        return result
+
+    @property
+    def _dag_name(self) -> str:
+        """Return the dag name created from its constituent parts."""
+        result = f"{self.workflow_name}_{self.workflow_version}"
+        self.check_dag_name_characters(result)  # raise an error if in valid
+        return result
 
     @staticmethod
     def check_dag_name_characters(dag_name: str):
         """
         Figure out if the dag name is an Airflow-allowed name.
 
         Can only contain
@@ -141,16 +136,14 @@
     def _dag_tags(self) -> str:
         """
         Return the list of dag tags to be used in Airflow's UI.
 
         Equal to the list of supplied tags plus the workflow version, input and output data,
         and category.
         """
-        if isinstance(self.tags, str):
-            self.tags = [self.tags]
         tags = self.tags + [self.workflow_version, self.input_data, self.output_data, self.category]
         # Make sure there are no duplicate tags
         tags = list(set(tags))
         return json.dumps(tags)
 
     @property
     def _dag_definition(self) -> str:
```

### Comparing `dkist-processing-core-3.2.0rc1/dkist_processing_core.egg-info/PKG-INFO` & `dkist-processing-core-3.2.0rc4/dkist_processing_core.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-core
-Version: 3.2.0rc1
+Version: 3.2.0rc4
 Summary: Abstraction layer that is used by the DKIST Science Data Processing pipelines to process DKIST data using Apache Airflow.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-core/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/core
 Classifier: Programming Language :: Python
@@ -110,27 +110,47 @@
    * - BUILD_VERSION
      - Build/Export pipelines only.  This is the value that will be appended to all artifacts and represents their unique version
      - STR
      - dev
    * - MESH_CONFIG
      - Provides the dkistdc cloud mesh configuration.  Specifically the location of the message broker
      - JSON
-     -
+     - ``{}``
    * - ISB_USERNAME
      - Message broker user name
      - STR
-     -
+     - guest
    * - ISB_PASSWORD
      - Message broker password
      - STR
-     -
+     - guest
    * - ISB_EXCHANGE
      - Message Broker Exchange name for publishing messages
      - STR
+     - master.direct.x
+   * - ISB_QUEUE_TYPE
+     - Message Broker queue type for transporting messages
+     - STR
+     - classic
+   * - ELASTIC_APM_SERVICE_NAME
+     - Service Name used by Elastic Application Performance Monitoring
+     - STR
      -
+   * - ELASTIC_APM_OTHER_OPTIONS
+     - Dictionary of configuration for the Elastic Application Performance Monitoring client
+     - STR
+     - ``{}``
+   * - ELASTIC_APM_ENABLED
+     - Flag to disable/enable Elastic Application Performance Monitoring client calls which are chatty if not connected to an APM server.
+     - BOOL
+     - FALSE
+   * - BUILD_VERSION
+     - Version of the pipeline.  When built this makes its way into the workflow or dag name.
+     - STR
+     - dev
 
 Development
 -----------
 .. code-block:: bash
 
     git clone git@bitbucket.org:dkistdc/dkist-processing-core.git
     cd dkist-processing-core
```

### Comparing `dkist-processing-core-3.2.0rc1/dkist_processing_core.egg-info/SOURCES.txt` & `dkist-processing-core-3.2.0rc4/dkist_processing_core.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -29,16 +29,18 @@
 dkist_processing_core/tests/task_example.py
 dkist_processing_core/tests/test_build_utils.py
 dkist_processing_core/tests/test_export.py
 dkist_processing_core/tests/test_failure_callback.py
 dkist_processing_core/tests/test_node.py
 dkist_processing_core/tests/test_task.py
 dkist_processing_core/tests/test_workflow.py
-dkist_processing_core/tests/invalid_workflow_package/__init__.py
-dkist_processing_core/tests/invalid_workflow_package/workflow.py
+dkist_processing_core/tests/invalid_workflow_cyclic/__init__.py
+dkist_processing_core/tests/invalid_workflow_cyclic/workflow.py
+dkist_processing_core/tests/invalid_workflow_for_docker_multi_category/__init__.py
+dkist_processing_core/tests/invalid_workflow_for_docker_multi_category/workflow.py
 dkist_processing_core/tests/valid_workflow_package/__init__.py
 dkist_processing_core/tests/valid_workflow_package/workflow.py
 dkist_processing_core/tests/zero_node_workflow_package/__init__.py
 dkist_processing_core/tests/zero_node_workflow_package/workflow.py
 docs/Makefile
 docs/auto-proc-concept-model.png
 docs/auto_proc_brick.png
```

### Comparing `dkist-processing-core-3.2.0rc1/docs/Makefile` & `dkist-processing-core-3.2.0rc4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.2.0rc1/docs/auto-proc-concept-model.png` & `dkist-processing-core-3.2.0rc4/docs/auto-proc-concept-model.png`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.2.0rc1/docs/auto_proc_brick.png` & `dkist-processing-core-3.2.0rc4/docs/auto_proc_brick.png`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.2.0rc1/docs/automated-processing-deployed.png` & `dkist-processing-core-3.2.0rc4/docs/automated-processing-deployed.png`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.2.0rc1/docs/conf.py` & `dkist-processing-core-3.2.0rc4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.2.0rc1/docs/make.bat` & `dkist-processing-core-3.2.0rc4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.2.0rc1/licenses/LICENSE.rst` & `dkist-processing-core-3.2.0rc4/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.2.0rc1/pyproject.toml` & `dkist-processing-core-3.2.0rc4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.2.0rc1/setup.cfg` & `dkist-processing-core-3.2.0rc4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 install_requires = 
 	apache-airflow[postgres, celery] == 2.9.1
 	elastic-apm < 7.0.0
 	requests >= 2.23
 	talus >= 1.1.0, <2.0
 	pendulum
 	nbformat >= 5.9.2
-	dkist-service-configuration >=2.0.1, <3.0
+	dkist-service-configuration >=2.0.2, <3.0
 	pydantic > 2.0
 
 [options.extras_require]
 test = 
 	pytest
 	pytest-cov
 	pytest-mock
```

