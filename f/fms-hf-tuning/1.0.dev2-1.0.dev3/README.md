# Comparing `tmp/fms-hf-tuning-1.0.dev2.tar.gz` & `tmp/fms-hf-tuning-1.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fms-hf-tuning-1.0.dev2.tar", last modified: Wed Apr  3 23:57:30 2024, max compression
+gzip compressed data, was "fms-hf-tuning-1.0.dev3.tar", last modified: Thu Apr  4 00:01:33 2024, max compression
```

## Comparing `fms-hf-tuning-1.0.dev2.tar` & `fms-hf-tuning-1.0.dev3.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:57:30.246816 fms-hf-tuning-1.0.dev2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:57:30.238816 fms-hf-tuning-1.0.dev2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:57:30.238816 fms-hf-tuning-1.0.dev2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/.github/ISSUE_TEMPLATE/user_story.md
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:57:30.242816 fms-hf-tuning-1.0.dev2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/.github/workflows/build-and-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    21494 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    14241 2024-04-03 23:57:30.246816 fms-hf-tuning-1.0.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13064 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:57:30.242816 fms-hf-tuning-1.0.dev2/architecture_records/
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/architecture_records/template.md
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/code-of-conduct.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:57:30.234816 fms-hf-tuning-1.0.dev2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:57:30.242816 fms-hf-tuning-1.0.dev2/examples/prompt_tuning_twitter_complaints/
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/examples/prompt_tuning_twitter_complaints/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:57:30.242816 fms-hf-tuning-1.0.dev2/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/fixtures/accelerate_fsdp_defaults.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:57:30.246816 fms-hf-tuning-1.0.dev2/fms_hf_tuning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14241 2024-04-03 23:57:30.000000 fms-hf-tuning-1.0.dev2/fms_hf_tuning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-03 23:57:30.000000 fms-hf-tuning-1.0.dev2/fms_hf_tuning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 23:57:30.000000 fms-hf-tuning-1.0.dev2/fms_hf_tuning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-03 23:57:30.000000 fms-hf-tuning-1.0.dev2/fms_hf_tuning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 23:57:30.000000 fms-hf-tuning-1.0.dev2/fms_hf_tuning.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-03 23:54:11.000000 fms-hf-tuning-1.0.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:57:30.242816 fms-hf-tuning-1.0.dev2/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      720 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/scripts/fmt.sh
--rw-r--r--   0 runner    (1001) docker     (127)    10833 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/scripts/run_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 23:57:30.246816 fms-hf-tuning-1.0.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/setup_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:57:30.242816 fms-hf-tuning-1.0.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:57:30.242816 fms-hf-tuning-1.0.dev2/tests/build/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/tests/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/tests/build/dummy_job_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/tests/build/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:57:30.242816 fms-hf-tuning-1.0.dev2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/tests/data/twitter_complaints_small.json
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/tests/test_sft_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:57:30.242816 fms-hf-tuning-1.0.dev2/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/tests/utils/test_data_type_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:57:30.246816 fms-hf-tuning-1.0.dev2/tuning/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/tuning/aim_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:57:30.246816 fms-hf-tuning-1.0.dev2/tuning/config/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/tuning/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/tuning/config/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/tuning/config/peft_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:57:30.246816 fms-hf-tuning-1.0.dev2/tuning/data/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/tuning/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/tuning/data/tokenizer_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11268 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/tuning/sft_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:57:30.246816 fms-hf-tuning-1.0.dev2/tuning/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/tuning/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/tuning/utils/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/tuning/utils/data_type_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/tuning/utils/import_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-04-03 23:54:04.000000 fms-hf-tuning-1.0.dev2/tuning/utils/merge_model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:01:33.571713 fms-hf-tuning-1.0.dev3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:01:33.567713 fms-hf-tuning-1.0.dev3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:01:33.567713 fms-hf-tuning-1.0.dev3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/.github/ISSUE_TEMPLATE/user_story.md
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:01:33.567713 fms-hf-tuning-1.0.dev3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/.github/workflows/build-and-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    21494 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    14241 2024-04-04 00:01:33.571713 fms-hf-tuning-1.0.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13064 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:01:33.567713 fms-hf-tuning-1.0.dev3/architecture_records/
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/architecture_records/template.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/code-of-conduct.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:01:33.559713 fms-hf-tuning-1.0.dev3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:01:33.567713 fms-hf-tuning-1.0.dev3/examples/prompt_tuning_twitter_complaints/
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/examples/prompt_tuning_twitter_complaints/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:01:33.567713 fms-hf-tuning-1.0.dev3/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/fixtures/accelerate_fsdp_defaults.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:01:33.571713 fms-hf-tuning-1.0.dev3/fms_hf_tuning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14241 2024-04-04 00:01:33.000000 fms-hf-tuning-1.0.dev3/fms_hf_tuning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-04 00:01:33.000000 fms-hf-tuning-1.0.dev3/fms_hf_tuning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 00:01:33.000000 fms-hf-tuning-1.0.dev3/fms_hf_tuning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-04 00:01:33.000000 fms-hf-tuning-1.0.dev3/fms_hf_tuning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-04 00:01:33.000000 fms-hf-tuning-1.0.dev3/fms_hf_tuning.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-03 23:59:11.000000 fms-hf-tuning-1.0.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:01:33.567713 fms-hf-tuning-1.0.dev3/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      720 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/scripts/fmt.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    10833 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/scripts/run_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 00:01:33.571713 fms-hf-tuning-1.0.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/setup_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:01:33.567713 fms-hf-tuning-1.0.dev3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:01:33.567713 fms-hf-tuning-1.0.dev3/tests/build/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/tests/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/tests/build/dummy_job_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/tests/build/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:01:33.567713 fms-hf-tuning-1.0.dev3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/tests/data/twitter_complaints_small.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/tests/test_sft_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:01:33.567713 fms-hf-tuning-1.0.dev3/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/tests/utils/test_data_type_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:01:33.571713 fms-hf-tuning-1.0.dev3/tuning/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/tuning/aim_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:01:33.571713 fms-hf-tuning-1.0.dev3/tuning/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/tuning/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/tuning/config/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/tuning/config/peft_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:01:33.571713 fms-hf-tuning-1.0.dev3/tuning/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/tuning/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/tuning/data/tokenizer_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11268 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/tuning/sft_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:01:33.571713 fms-hf-tuning-1.0.dev3/tuning/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/tuning/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/tuning/utils/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/tuning/utils/data_type_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/tuning/utils/import_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-04-03 23:59:04.000000 fms-hf-tuning-1.0.dev3/tuning/utils/merge_model_utils.py
```

### Comparing `fms-hf-tuning-1.0.dev2/.github/ISSUE_TEMPLATE/bug_report.md` & `fms-hf-tuning-1.0.dev3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/.github/ISSUE_TEMPLATE/feature_request.md` & `fms-hf-tuning-1.0.dev3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/.github/workflows/build-and-publish.yaml` & `fms-hf-tuning-1.0.dev3/.github/workflows/build-and-publish.yaml`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/.github/workflows/format.yml` & `fms-hf-tuning-1.0.dev3/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/.pylintrc` & `fms-hf-tuning-1.0.dev3/.pylintrc`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/CONTRIBUTING.md` & `fms-hf-tuning-1.0.dev3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/LICENSE` & `fms-hf-tuning-1.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/PKG-INFO` & `fms-hf-tuning-1.0.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fms-hf-tuning
-Version: 1.0.dev2
+Version: 1.0.dev3
 Summary: FMS HF Tuning
 Author-email: Sukriti Sharma <sukriti.sharma4@ibm.com>, Anh Uong <anh.uong@ibm.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/foundation-model-stack/fms-hf-tuning
 Project-URL: Repository, https://github.com/foundation-model-stack/fms-hf-tuning
 Project-URL: Issues, https://github.com/foundation-model-stack/fms-hf-tuning/issues
 Keywords: fms-hf-tuning,python,tuning
```

### Comparing `fms-hf-tuning-1.0.dev2/README.md` & `fms-hf-tuning-1.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/architecture_records/template.md` & `fms-hf-tuning-1.0.dev3/architecture_records/template.md`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/code-of-conduct.md` & `fms-hf-tuning-1.0.dev3/code-of-conduct.md`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/examples/prompt_tuning_twitter_complaints/README.md` & `fms-hf-tuning-1.0.dev3/examples/prompt_tuning_twitter_complaints/README.md`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/fixtures/accelerate_fsdp_defaults.yaml` & `fms-hf-tuning-1.0.dev3/fixtures/accelerate_fsdp_defaults.yaml`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/fms_hf_tuning.egg-info/PKG-INFO` & `fms-hf-tuning-1.0.dev3/fms_hf_tuning.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fms-hf-tuning
-Version: 1.0.dev2
+Version: 1.0.dev3
 Summary: FMS HF Tuning
 Author-email: Sukriti Sharma <sukriti.sharma4@ibm.com>, Anh Uong <anh.uong@ibm.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/foundation-model-stack/fms-hf-tuning
 Project-URL: Repository, https://github.com/foundation-model-stack/fms-hf-tuning
 Project-URL: Issues, https://github.com/foundation-model-stack/fms-hf-tuning/issues
 Keywords: fms-hf-tuning,python,tuning
```

### Comparing `fms-hf-tuning-1.0.dev2/fms_hf_tuning.egg-info/SOURCES.txt` & `fms-hf-tuning-1.0.dev3/fms_hf_tuning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/pyproject.toml` & `fms-hf-tuning-1.0.dev3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "setuptools>=61",
     "setuptools-scm>=8.0"]
 
 [project]
 name = "fms-hf-tuning"
-version = "1.0.dev2"
+version = "1.0.dev3"
 description = "FMS HF Tuning"
 authors = [
   {name = "Sukriti Sharma", email = "sukriti.sharma4@ibm.com"},
   {name = "Anh Uong", email = "anh.uong@ibm.com"},
 ]
 license = {text = "Apache-2.0"}
 readme = "README.md"
```

### Comparing `fms-hf-tuning-1.0.dev2/scripts/fmt.sh` & `fms-hf-tuning-1.0.dev3/scripts/fmt.sh`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/scripts/run_inference.py` & `fms-hf-tuning-1.0.dev3/scripts/run_inference.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/setup.py` & `fms-hf-tuning-1.0.dev3/setup.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/tests/__init__.py` & `fms-hf-tuning-1.0.dev3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/tests/build/__init__.py` & `fms-hf-tuning-1.0.dev3/tests/build/__init__.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/tests/build/dummy_job_config.json` & `fms-hf-tuning-1.0.dev3/tests/build/dummy_job_config.json`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/tests/build/test_utils.py` & `fms-hf-tuning-1.0.dev3/tests/build/test_utils.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/tests/data/__init__.py` & `fms-hf-tuning-1.0.dev3/tests/data/__init__.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/tests/data/twitter_complaints_small.json` & `fms-hf-tuning-1.0.dev3/tests/data/twitter_complaints_small.json`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/tests/helpers.py` & `fms-hf-tuning-1.0.dev3/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/tests/test_sft_trainer.py` & `fms-hf-tuning-1.0.dev3/tests/test_sft_trainer.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/tests/utils/__init__.py` & `fms-hf-tuning-1.0.dev3/tests/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/tests/utils/test_data_type_utils.py` & `fms-hf-tuning-1.0.dev3/tests/utils/test_data_type_utils.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/tox.ini` & `fms-hf-tuning-1.0.dev3/tox.ini`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/tuning/__init__.py` & `fms-hf-tuning-1.0.dev3/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/tuning/aim_loader.py` & `fms-hf-tuning-1.0.dev3/tuning/aim_loader.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/tuning/config/__init__.py` & `fms-hf-tuning-1.0.dev3/tuning/config/__init__.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/tuning/config/configs.py` & `fms-hf-tuning-1.0.dev3/tuning/config/configs.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/tuning/config/peft_config.py` & `fms-hf-tuning-1.0.dev3/tuning/config/peft_config.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/tuning/data/__init__.py` & `fms-hf-tuning-1.0.dev3/tuning/data/__init__.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/tuning/data/tokenizer_data_utils.py` & `fms-hf-tuning-1.0.dev3/tuning/data/tokenizer_data_utils.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/tuning/sft_trainer.py` & `fms-hf-tuning-1.0.dev3/tuning/sft_trainer.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/tuning/utils/__init__.py` & `fms-hf-tuning-1.0.dev3/tuning/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/tuning/utils/config_utils.py` & `fms-hf-tuning-1.0.dev3/tuning/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/tuning/utils/data_type_utils.py` & `fms-hf-tuning-1.0.dev3/tuning/utils/data_type_utils.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/tuning/utils/import_utils.py` & `fms-hf-tuning-1.0.dev3/tuning/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `fms-hf-tuning-1.0.dev2/tuning/utils/merge_model_utils.py` & `fms-hf-tuning-1.0.dev3/tuning/utils/merge_model_utils.py`

 * *Files identical despite different names*

