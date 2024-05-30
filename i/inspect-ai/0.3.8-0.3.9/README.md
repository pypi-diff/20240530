# Comparing `tmp/inspect_ai-0.3.8.tar.gz` & `tmp/inspect_ai-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inspect_ai-0.3.8.tar", last modified: Tue May  7 22:49:42 2024, max compression
+gzip compressed data, was "inspect_ai-0.3.9.tar", last modified: Tue May 14 19:33:59 2024, max compression
```

## Comparing `inspect_ai-0.3.8.tar` & `inspect_ai-0.3.9.tar`

### file list

```diff
@@ -1,491 +1,515 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.446029 inspect_ai-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.374029 inspect_ai-0.3.8/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.374029 inspect_ai-0.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/.github/workflows/vscode.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.374029 inspect_ai-0.3.8/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-07 22:49:42.446029 inspect_ai-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.374029 inspect_ai-0.3.8/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/benchmarks/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/benchmarks/arc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.374029 inspect_ai-0.3.8/benchmarks/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/benchmarks/datasets/math_test.csv
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/benchmarks/datasets/mmlu.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/benchmarks/gpqa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/benchmarks/gsm8k.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/benchmarks/hellaswag.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/benchmarks/mathematics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/benchmarks/mmlu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.378029 inspect_ai-0.3.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.378029 inspect_ai-0.3.8/docs/_examples/
--rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/_examples/arc.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/_examples/biology_qa.qmd
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/_examples/footer.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/_examples/gsm8k.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/_examples/hellaswag.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/_examples/index.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/_examples/mathematics.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/_examples/popularity.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/_examples/security_guide.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/_examples/theory_of_mind.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/_examples/tool_use.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.378029 inspect_ai-0.3.8/docs/_format/
--rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/_format/pre-render.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/_variables.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11333 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/datasets.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     9905 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/eval-logs.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/eval-suites.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    10373 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/eval-tuning.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    35808 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/examples.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.386029 inspect_ai-0.3.8/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)   170128 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/images/aisi-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    68030 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/images/eval-log.png
--rw-r--r--   0 runner    (1001) docker     (127)   314093 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/images/inspect-view-answers.png
--rw-r--r--   0 runner    (1001) docker     (127)   280184 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/images/inspect-view-filter.png
--rw-r--r--   0 runner    (1001) docker     (127)   284131 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/images/inspect-view-history.png
--rw-r--r--   0 runner    (1001) docker     (127)   413188 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/images/inspect-view-home.png
--rw-r--r--   0 runner    (1001) docker     (127)   241738 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/images/inspect-view-info.png
--rw-r--r--   0 runner    (1001) docker     (127)   143202 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/images/inspect-view-logging-console.png
--rw-r--r--   0 runner    (1001) docker     (127)   155304 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/images/inspect-view-logging.png
--rw-r--r--   0 runner    (1001) docker     (127)   373146 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/images/inspect-view-main.png
--rw-r--r--   0 runner    (1001) docker     (127)   321793 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/images/inspect-view-messages.png
--rw-r--r--   0 runner    (1001) docker     (127)   165394 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/images/inspect-view-metadata.png
--rw-r--r--   0 runner    (1001) docker     (127)   272733 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/images/inspect-view-scoring.png
--rw-r--r--   0 runner    (1001) docker     (127)   274383 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/images/inspect-view-sort.png
--rw-r--r--   0 runner    (1001) docker     (127)    90624 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/images/inspect-view-splash.png
--rw-r--r--   0 runner    (1001) docker     (127)    68787 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/images/popularity.png
--rw-r--r--   0 runner    (1001) docker     (127)    54252 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/images/rate-limit.png
--rw-r--r--   0 runner    (1001) docker     (127)    48461 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/images/running-theory.png
--rw-r--r--   0 runner    (1001) docker     (127)    10437 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/index.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     9421 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/log-viewer.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    18564 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/models.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    15801 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/scorers.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    14283 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/solvers.qmd
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/theme.scss
--rw-r--r--   0 runner    (1001) docker     (127)    15937 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/tools.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    12752 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/docs/workflow.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.390029 inspect_ai-0.3.8/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.362029 inspect_ai-0.3.8/examples/agents/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.390029 inspect_ai-0.3.8/examples/agents/langchain/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/examples/agents/langchain/.env.example
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/examples/agents/langchain/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/examples/agents/langchain/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/examples/agents/langchain/inspect_langchain.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/examples/agents/langchain/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/examples/agents/langchain/wikipedia.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/examples/agents/langchain/wikipedia.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/examples/biology_qa.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/examples/popularity.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/examples/security_guide.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/examples/theory_of_mind.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/examples/tool_use.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 22:49:42.446029 inspect_ai-0.3.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.362029 inspect_ai-0.3.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.390029 inspect_ai-0.3.8/src/inspect_ai/
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.390029 inspect_ai-0.3.8/src/inspect_ai/_cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_cli/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7669 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_cli/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_cli/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_cli/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_cli/score.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_cli/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_cli/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.394029 inspect_ai-0.3.8/src/inspect_ai/_display/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_display/_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_display/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_display/rich.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.394029 inspect_ai-0.3.8/src/inspect_ai/_eval/
--rw-r--r--   0 runner    (1001) docker     (127)    16214 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_eval/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_eval/images.py
--rw-r--r--   0 runner    (1001) docker     (127)    11631 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_eval/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_eval/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_eval/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_eval/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_eval/score.py
--rw-r--r--   0 runner    (1001) docker     (127)    22961 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_eval/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.398029 inspect_ai-0.3.8/src/inspect_ai/_util/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/appdirs.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/docstring.py
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/dotenv.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     8512 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/samples.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/text.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/url.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_util/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.398029 inspect_ai-0.3.8/src/inspect_ai/_view/
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     9191 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.398029 inspect_ai-0.3.8/src/inspect_ai/_view/www/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    10687 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/App.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.398029 inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.362029 inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.398029 inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/bootstrap/css/
--rw-r--r--   0 runner    (1001) docker     (127)    85877 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   232903 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.402029 inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   176196 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff
--rw-r--r--   0 runner    (1001) docker     (127)   130764 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.402029 inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/bootstrap/js/
--rw-r--r--   0 runner    (1001) docker     (127)    80615 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/bootstrap/js/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/clipboard.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    31629 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/json5.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.402029 inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/prism/
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/prism/prism-dark.css
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/prism/prism.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    16934 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/prism/prism.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    21104 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/purify.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    75207 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/showdown.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    34863 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/log-schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/log.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.402029 inspect_ai-0.3.8/src/inspect_ai/_view/www/preact/
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/preact/hooks.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.402029 inspect_ai-0.3.8/src/inspect_ai/_view/www/preact/htm/
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/preact/htm/htm.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/preact/htm/preact.js
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/preact/htm/preact.mjs
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/preact/preact-hooks.mjs
--rw-r--r--   0 runner    (1001) docker     (127)    11268 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/preact/preact.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.402029 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/
--rw-r--r--   0 runner    (1001) docker     (127)    12181 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/App.css
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/Constants.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/Register.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.402029 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/api/api-browser.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/api/api-vscode.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/api/index.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/api/jsonrpc.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.406029 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/AnsiDisplay.css
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/AnsiDisplay.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/AppErrorBoundary.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/Card.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/ChatView.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/CopyButton.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/Dialog.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/EmptyPanel.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/ErrorPanel.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/LabeledValue.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/LoadingScreen.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/MarkdownDiv.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/MessageContent.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/MetaDataView.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/RenderedContent.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/TabSet.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/ToolButton.mjs
--rw-r--r--   0 runner    (1001) docker     (127)    20289 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/ansi-output.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.406029 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/log-reader/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/log-reader/Log-Reader.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/log-reader/Native-Log-Reader.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/log-reader/Open-AI-Log-Reader.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.406029 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/logging/
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/logging/LoggingPanel.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.406029 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/plan/
--rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/plan/PlanCard.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.406029 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/samples/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/samples/SampleGroupSeparator.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/samples/SampleScoreView.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/samples/SampleView.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/samples/SamplesCard.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.406029 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/title/
--rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/title/TitleBlock.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.410029 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/usage/
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/usage/ModelTokenTable.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/usage/UsageCard.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.410029 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/utils/Format.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/utils/Git.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/utils/Path.mjs
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/utils/Type.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.410029 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/workspace/
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/workspace/EpochFilter.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/workspace/SampleFilter.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/workspace/SamplesDescriptor.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/workspace/SortFilter.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/workspace/TaskErrorPanel.mjs
--rw-r--r--   0 runner    (1001) docker     (127)    15531 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/_view/www/src/workspace/WorkSpace.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.410029 inspect_ai-0.3.8/src/inspect_ai/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/dataset/_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.410029 inspect_ai-0.3.8/src/inspect_ai/dataset/_examples/
--rw-r--r--   0 runner    (1001) docker     (127)    20756 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/dataset/_examples/bias_detection.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/dataset/_examples/biology_qa.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)    32773 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/dataset/_examples/popularity.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/dataset/_examples/security_guide.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)    31831 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/dataset/_examples/theory_of_mind.jsonl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.410029 inspect_ai-0.3.8/src/inspect_ai/dataset/_sources/
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/dataset/_sources/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/dataset/_sources/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/dataset/_sources/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/dataset/_sources/hf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/dataset/_sources/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/dataset/_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.414029 inspect_ai-0.3.8/src/inspect_ai/log/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/log/_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     9174 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/log/_log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.414029 inspect_ai-0.3.8/src/inspect_ai/model/
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33705 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/model/_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.414029 inspect_ai-0.3.8/src/inspect_ai/model/_providers/
--rw-r--r--   0 runner    (1001) docker     (127)    29810 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/model/_providers/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7885 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/model/_providers/azureai.py
--rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/model/_providers/bedrock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/model/_providers/cloudflare.py
--rw-r--r--   0 runner    (1001) docker     (127)    10170 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/model/_providers/google.py
--rw-r--r--   0 runner    (1001) docker     (127)    12608 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/model/_providers/hf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7859 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/model/_providers/mistral.py
--rw-r--r--   0 runner    (1001) docker     (127)    13793 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/model/_providers/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/model/_providers/providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/model/_providers/together.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/model/_providers/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/model/_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/model/_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/model/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.414029 inspect_ai-0.3.8/src/inspect_ai/scorer/
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/scorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/scorer/_answer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/scorer/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/scorer/_match.py
--rw-r--r--   0 runner    (1001) docker     (127)     7209 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/scorer/_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.418029 inspect_ai-0.3.8/src/inspect_ai/scorer/_metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/scorer/_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/scorer/_metrics/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/scorer/_metrics/mean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/scorer/_metrics/std.py
--rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/scorer/_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/scorer/_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/scorer/_scorer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.418029 inspect_ai-0.3.8/src/inspect_ai/solver/
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/solver/_critique.py
--rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/solver/_multiple_choice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/solver/_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/solver/_prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/solver/_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.418029 inspect_ai-0.3.8/src/inspect_ai/solver/_tool/
--rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/solver/_tool/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/solver/_tool/tool_def.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/solver/_tool/use_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/solver/_tool/web_search.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/solver/_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.418029 inspect_ai-0.3.8/src/inspect_ai/util/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.418029 inspect_ai-0.3.8/src/inspect_ai/util/_context/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/util/_context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/util/_context/concurrency.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/util/_context/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/util/_context/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/src/inspect_ai/util/_context/subprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.442029 inspect_ai-0.3.8/src/inspect_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-07 22:49:42.000000 inspect_ai-0.3.8/src/inspect_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15007 2024-05-07 22:49:42.000000 inspect_ai-0.3.8/src/inspect_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 22:49:42.000000 inspect_ai-0.3.8/src/inspect_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-07 22:49:42.000000 inspect_ai-0.3.8/src/inspect_ai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-07 22:49:42.000000 inspect_ai-0.3.8/src/inspect_ai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-07 22:49:42.000000 inspect_ai-0.3.8/src/inspect_ai.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.422029 inspect_ai-0.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_cloudlfare.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_collapse_assistant_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_collapse_user_message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.422029 inspect_ai-0.3.8/tests/test_dataset/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_dataset/samples.csv
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_dataset/samples.json
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_dataset/samples.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_eval_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_hf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.422029 inspect_ai-0.3.8/tests/test_images/
--rw-r--r--   0 runner    (1001) docker     (127)   732622 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_images/images.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_list_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_logprobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_num_choices.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_scorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_stop_reason.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_subprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.426029 inspect_ai-0.3.8/tests/test_task_list/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_task_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_task_list/attribs.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_task_list/multiple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.426029 inspect_ai-0.3.8/tests/test_task_list/multiple_dir/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.426029 inspect_ai-0.3.8/tests/test_task_list/multiple_dir/_decoy/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_task_list/multiple_dir/_decoy/testit.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_task_list/multiple_dir/_decoy2.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_task_list/multiple_dir/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_task_list/multiple_dir/foo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.366029 inspect_ai-0.3.8/tests/test_task_list/recurse/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.426029 inspect_ai-0.3.8/tests/test_task_list/recurse/.folder3/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_task_list/recurse/.folder3/epsilon.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.426029 inspect_ai-0.3.8/tests/test_task_list/recurse/folder1/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_task_list/recurse/folder1/_decoy.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_task_list/recurse/folder1/theta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.426029 inspect_ai-0.3.8/tests/test_task_list/recurse/folder2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.426029 inspect_ai-0.3.8/tests/test_task_list/recurse/folder2/.folder3/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_task_list/recurse/folder2/.folder3/epsilon.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_task_list/recurse/folder2/another.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_task_list/recurse/folder2/first.py
--rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.366029 inspect_ai-0.3.8/tools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.426029 inspect_ai-0.3.8/tools/vscode/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/.eslintrc.json
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.430029 inspect_ai-0.3.8/tools/vscode/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/.vscode-test.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/.vscodeignore
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/.yarnrc
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.370029 inspect_ai-0.3.8/tools/vscode/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.430029 inspect_ai-0.3.8/tools/vscode/assets/logo/
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/assets/logo/inspect.png
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/assets/logo/inspect.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.430029 inspect_ai-0.3.8/tools/vscode/assets/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/assets/templates/task.py.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.370029 inspect_ai-0.3.8/tools/vscode/assets/www/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.430029 inspect_ai-0.3.8/tools/vscode/assets/www/codicon/
--rw-r--r--   0 runner    (1001) docker     (127)    27023 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/assets/www/codicon/codicon.css
--rw-r--r--   0 runner    (1001) docker     (127)    72860 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/assets/www/codicon/codicon.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    10197 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.430029 inspect_ai-0.3.8/tools/vscode/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.430029 inspect_ai-0.3.8/tools/vscode/src/components/
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/components/debugger.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/components/document.ts
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/components/error.ts
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/components/focus.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/components/notebook.ts
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/components/templates.ts
--rw-r--r--   0 runner    (1001) docker     (127)     7419 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/components/webview.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.434029 inspect_ai-0.3.8/tools/vscode/src/core/
--rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/appdirs.ts
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/command.ts
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/dispose.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/env.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/git.ts
--rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/jsonrpc.ts
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/log.ts
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/nonce.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/path.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/port.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/process.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.434029 inspect_ai-0.3.8/tools/vscode/src/core/python/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/python/code.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/python/exec.ts
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/python/index.ts
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/python/interpreter.ts
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/random.ts
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/string.ts
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/text.ts
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/wait.ts
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/core/workspace.ts
--rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/extension.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.434029 inspect_ai-0.3.8/tools/vscode/src/inspect/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/inspect/index.ts
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/inspect/list.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/inspect/logs.ts
--rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/inspect/props.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.370029 inspect_ai-0.3.8/tools/vscode/src/providers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.434029 inspect_ai-0.3.8/tools/vscode/src/providers/active-task/
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/active-task/active-task-command.ts
--rw-r--r--   0 runner    (1001) docker     (127)     6213 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/active-task/active-task-provider.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.434029 inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/activity-bar-provider.ts
--rw-r--r--   0 runner    (1001) docker     (127)    12825 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/env-config-provider.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/task-config-commands.ts
--rw-r--r--   0 runner    (1001) docker     (127)     9569 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/task-config-provider.ts
--rw-r--r--   0 runner    (1001) docker     (127)     7284 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/task-outline-commands.ts
--rw-r--r--   0 runner    (1001) docker     (127)    10312 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/task-outline-provider.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.438029 inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/webview/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/webview/env-config-webview.css
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/webview/env-config-webview.ts
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/webview/task-config-webview.css
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/webview/task-config-webview.ts
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/webview/vscode-controls.css
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/webview/webview-utils.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.438029 inspect_ai-0.3.8/tools/vscode/src/providers/codelens/
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/codelens/codelens-provider.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.438029 inspect_ai-0.3.8/tools/vscode/src/providers/inspect/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/inspect/inspect-constants.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/inspect/inspect-eval-commands.ts
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/inspect/inspect-eval.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/inspect/inspect-manager.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.438029 inspect_ai-0.3.8/tools/vscode/src/providers/logview/
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/logview/commands.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/logview/logview-file-watcher.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/logview/logview-link-provider.ts
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/logview/logview-manager.ts
--rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/logview/logview-webview.ts
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/logview/logview.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.438029 inspect_ai-0.3.8/tools/vscode/src/providers/settings/
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/settings/inspect-settings.ts
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/settings/user-settings.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.438029 inspect_ai-0.3.8/tools/vscode/src/providers/workspace/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/workspace/workspace-env-commands.ts
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/workspace/workspace-env-provider.ts
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/workspace/workspace-init.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/workspace/workspace-state-provider.ts
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/providers/workspace/workspace-task-provider.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.438029 inspect_ai-0.3.8/tools/vscode/src/test/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/src/test/extension.test.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.370029 inspect_ai-0.3.8/tools/vscode/tools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.442029 inspect_ai-0.3.8/tools/vscode/tools/ts-to-mjs/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/tools/ts-to-mjs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/tools/ts-to-mjs/package.json
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/tools/ts-to-mjs/rollup.config.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:49:42.442029 inspect_ai-0.3.8/tools/vscode/tools/ts-to-mjs/src/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/tools/ts-to-mjs/src/index.ts
--rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/tools/ts-to-mjs/src/jsonrpc.ts
--rw-r--r--   0 runner    (1001) docker     (127)   129610 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/tools/ts-to-mjs/yarn.lock
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/webpack.config.js
--rw-r--r--   0 runner    (1001) docker     (127)   158647 2024-05-07 22:49:37.000000 inspect_ai-0.3.8/tools/vscode/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.524143 inspect_ai-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.444143 inspect_ai-0.3.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.448143 inspect_ai-0.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/.github/workflows/vscode.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.448143 inspect_ai-0.3.9/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-14 19:33:59.524143 inspect_ai-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.448143 inspect_ai-0.3.9/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/benchmarks/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/benchmarks/arc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.448143 inspect_ai-0.3.9/benchmarks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/benchmarks/datasets/math_test.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/benchmarks/datasets/mmlu.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/benchmarks/gpqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/benchmarks/gsm8k.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/benchmarks/hellaswag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/benchmarks/mathematics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/benchmarks/mmlu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.452143 inspect_ai-0.3.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.452143 inspect_ai-0.3.9/docs/_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/_examples/arc.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/_examples/biology_qa.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/_examples/footer.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/_examples/gsm8k.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/_examples/hellaswag.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/_examples/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/_examples/mathematics.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/_examples/popularity.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/_examples/security_guide.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/_examples/theory_of_mind.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/_examples/tool_use.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.452143 inspect_ai-0.3.9/docs/_format/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/_format/pre-render.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/_variables.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11332 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/datasets.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     9907 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/eval-logs.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     8390 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/eval-suites.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    10373 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/eval-tuning.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    35808 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/examples.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.464143 inspect_ai-0.3.9/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   170128 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/images/aisi-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68030 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/images/eval-log.png
+-rw-r--r--   0 runner    (1001) docker     (127)   314093 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/images/inspect-view-answers.png
+-rw-r--r--   0 runner    (1001) docker     (127)   280184 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/images/inspect-view-filter.png
+-rw-r--r--   0 runner    (1001) docker     (127)   284131 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/images/inspect-view-history.png
+-rw-r--r--   0 runner    (1001) docker     (127)   413188 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/images/inspect-view-home.png
+-rw-r--r--   0 runner    (1001) docker     (127)   241738 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/images/inspect-view-info.png
+-rw-r--r--   0 runner    (1001) docker     (127)   143202 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/images/inspect-view-logging-console.png
+-rw-r--r--   0 runner    (1001) docker     (127)   155304 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/images/inspect-view-logging.png
+-rw-r--r--   0 runner    (1001) docker     (127)   373146 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/images/inspect-view-main.png
+-rw-r--r--   0 runner    (1001) docker     (127)   321793 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/images/inspect-view-messages.png
+-rw-r--r--   0 runner    (1001) docker     (127)   165394 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/images/inspect-view-metadata.png
+-rw-r--r--   0 runner    (1001) docker     (127)   272733 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/images/inspect-view-scoring.png
+-rw-r--r--   0 runner    (1001) docker     (127)   274383 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/images/inspect-view-sort.png
+-rw-r--r--   0 runner    (1001) docker     (127)    90624 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/images/inspect-view-splash.png
+-rw-r--r--   0 runner    (1001) docker     (127)   274024 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/images/inspect-vscode-config.png
+-rw-r--r--   0 runner    (1001) docker     (127)   167250 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/images/inspect-vscode-install.png
+-rw-r--r--   0 runner    (1001) docker     (127)   375738 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/images/inspect-vscode-logview.png
+-rw-r--r--   0 runner    (1001) docker     (127)    90401 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/images/inspect-vscode-output-channel.png
+-rw-r--r--   0 runner    (1001) docker     (127)    62834 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/images/inspect-vscode-run-task.png
+-rw-r--r--   0 runner    (1001) docker     (127)   545567 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/images/inspect.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68787 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/images/popularity.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54252 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/images/rate-limit.png
+-rw-r--r--   0 runner    (1001) docker     (127)    48461 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/images/running-theory.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10293 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     9418 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/log-viewer.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    19351 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/models.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    17745 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/scorers.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    14294 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/solvers.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/theme.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    15944 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/tools.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/vscode.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    12988 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/docs/workflow.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.464143 inspect_ai-0.3.9/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.436143 inspect_ai-0.3.9/examples/agents/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.464143 inspect_ai-0.3.9/examples/agents/langchain/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/examples/agents/langchain/.env.example
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/examples/agents/langchain/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/examples/agents/langchain/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/examples/agents/langchain/inspect_langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/examples/agents/langchain/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/examples/agents/langchain/wikipedia.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/examples/agents/langchain/wikipedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/examples/biology_qa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/examples/popularity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/examples/security_guide.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/examples/theory_of_mind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/examples/tool_use.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 19:33:59.524143 inspect_ai-0.3.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.436143 inspect_ai-0.3.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.464143 inspect_ai-0.3.9/src/inspect_ai/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.468143 inspect_ai-0.3.9/src/inspect_ai/_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7670 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_cli/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_cli/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_cli/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_cli/score.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_cli/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.468143 inspect_ai-0.3.9/src/inspect_ai/_display/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_display/_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_display/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_display/rich.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.468143 inspect_ai-0.3.9/src/inspect_ai/_eval/
+-rw-r--r--   0 runner    (1001) docker     (127)    16427 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_eval/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_eval/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_eval/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_eval/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_eval/score.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.468143 inspect_ai-0.3.9/src/inspect_ai/_eval/task/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_eval/task/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_eval/task/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_eval/task/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_eval/task/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_eval/task/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10911 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_eval/task/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_eval/task/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_eval/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.472143 inspect_ai-0.3.9/src/inspect_ai/_util/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_util/_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_util/appdirs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_util/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_util/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_util/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_util/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_util/dotenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_util/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_util/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_util/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_util/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_util/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_util/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_util/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_util/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_util/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_util/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8512 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_util/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_util/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_util/samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_util/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_util/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.472143 inspect_ai-0.3.9/src/inspect_ai/_view/
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9193 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.476143 inspect_ai-0.3.9/src/inspect_ai/_view/www/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    10687 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/App.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.476143 inspect_ai-0.3.9/src/inspect_ai/_view/www/libs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.440143 inspect_ai-0.3.9/src/inspect_ai/_view/www/libs/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.476143 inspect_ai-0.3.9/src/inspect_ai/_view/www/libs/bootstrap/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    85877 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   232903 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.476143 inspect_ai-0.3.9/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   176196 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   130764 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.476143 inspect_ai-0.3.9/src/inspect_ai/_view/www/libs/bootstrap/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    80615 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/libs/bootstrap/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/libs/clipboard.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    31629 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/libs/json5.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.476143 inspect_ai-0.3.9/src/inspect_ai/_view/www/libs/prism/
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/libs/prism/prism-dark.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/libs/prism/prism.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    16934 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/libs/prism/prism.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21104 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/libs/purify.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    75207 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/libs/showdown.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    34863 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/log-schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/log.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.476143 inspect_ai-0.3.9/src/inspect_ai/_view/www/preact/
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/preact/hooks.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.480143 inspect_ai-0.3.9/src/inspect_ai/_view/www/preact/htm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/preact/htm/htm.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/preact/htm/preact.js
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/preact/htm/preact.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/preact/preact-hooks.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)    11268 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/preact/preact.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.480143 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    12180 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/App.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/Constants.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/Register.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.480143 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/api/api-browser.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/api/api-vscode.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/api/index.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/api/jsonrpc.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.484143 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/components/AnsiDisplay.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/components/AnsiDisplay.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/components/AppErrorBoundary.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/components/Card.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/components/ChatView.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/components/CopyButton.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/components/Dialog.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/components/EmptyPanel.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/components/ErrorPanel.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/components/LabeledValue.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/components/LoadingScreen.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/components/MarkdownDiv.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/components/MessageContent.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/components/MetaDataView.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/components/RenderedContent.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/components/TabSet.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/components/ToolButton.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)    20289 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/components/ansi-output.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.484143 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/log-reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/log-reader/Log-Reader.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/log-reader/Native-Log-Reader.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/log-reader/Open-AI-Log-Reader.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.484143 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/logging/LoggingPanel.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.484143 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/plan/
+-rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/plan/PlanCard.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.484143 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/samples/SampleGroupSeparator.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/samples/SampleScoreView.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/samples/SampleView.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/samples/SamplesCard.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.484143 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/title/
+-rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/title/TitleBlock.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.484143 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/usage/ModelTokenTable.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/usage/UsageCard.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.484143 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/utils/Format.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/utils/Git.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/utils/Path.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/utils/Type.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.484143 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/workspace/EpochFilter.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/workspace/SampleFilter.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/workspace/SamplesDescriptor.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/workspace/SortFilter.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/workspace/TaskErrorPanel.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)    15531 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/_view/www/src/workspace/WorkSpace.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.488143 inspect_ai-0.3.9/src/inspect_ai/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/dataset/_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.488143 inspect_ai-0.3.9/src/inspect_ai/dataset/_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    20756 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/dataset/_examples/bias_detection.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/dataset/_examples/biology_qa.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)    32773 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/dataset/_examples/popularity.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/dataset/_examples/security_guide.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)    31831 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/dataset/_examples/theory_of_mind.jsonl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.488143 inspect_ai-0.3.9/src/inspect_ai/dataset/_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/dataset/_sources/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/dataset/_sources/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/dataset/_sources/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/dataset/_sources/hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/dataset/_sources/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/dataset/_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.488143 inspect_ai-0.3.9/src/inspect_ai/log/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11497 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/log/_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9175 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/log/_log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.488143 inspect_ai-0.3.9/src/inspect_ai/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33625 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/model/_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.492143 inspect_ai-0.3.9/src/inspect_ai/model/_providers/
+-rw-r--r--   0 runner    (1001) docker     (127)    29814 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/model/_providers/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7885 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/model/_providers/azureai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/model/_providers/bedrock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/model/_providers/cloudflare.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10170 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/model/_providers/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12829 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/model/_providers/hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7859 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/model/_providers/mistral.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/model/_providers/ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13793 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/model/_providers/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/model/_providers/providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/model/_providers/together.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/model/_providers/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/model/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/model/_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/model/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.492143 inspect_ai-0.3.9/src/inspect_ai/scorer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/scorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/scorer/_answer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/scorer/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/scorer/_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7208 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/scorer/_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.492143 inspect_ai-0.3.9/src/inspect_ai/scorer/_metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/scorer/_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/scorer/_metrics/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/scorer/_metrics/mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/scorer/_metrics/std.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8212 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/scorer/_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/scorer/_multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/scorer/_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/scorer/_scorer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.496143 inspect_ai-0.3.9/src/inspect_ai/solver/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/solver/_critique.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/solver/_multiple_choice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/solver/_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/solver/_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/solver/_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.496143 inspect_ai-0.3.9/src/inspect_ai/solver/_tool/
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/solver/_tool/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/solver/_tool/tool_def.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/solver/_tool/use_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/solver/_tool/web_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/solver/_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.496143 inspect_ai-0.3.9/src/inspect_ai/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.496143 inspect_ai-0.3.9/src/inspect_ai/util/_context/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/util/_context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/util/_context/concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/util/_context/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/util/_context/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/src/inspect_ai/util/_context/subprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.520143 inspect_ai-0.3.9/src/inspect_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-14 19:33:59.000000 inspect_ai-0.3.9/src/inspect_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15765 2024-05-14 19:33:59.000000 inspect_ai-0.3.9/src/inspect_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:33:59.000000 inspect_ai-0.3.9/src/inspect_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-14 19:33:59.000000 inspect_ai-0.3.9/src/inspect_ai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-14 19:33:59.000000 inspect_ai-0.3.9/src/inspect_ai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 19:33:59.000000 inspect_ai-0.3.9/src/inspect_ai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.500143 inspect_ai-0.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_cloudflare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_collapse_assistant_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_collapse_user_message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.500143 inspect_ai-0.3.9/tests/test_dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_dataset/samples.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_dataset/samples.json
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_dataset/samples.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.500143 inspect_ai-0.3.9/tests/test_eval_log/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_eval_log/log_invalid.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_eval_log/log_version_2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_eval_log/log_with_nan.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_eval_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_hf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.500143 inspect_ai-0.3.9/tests/test_images/
+-rw-r--r--   0 runner    (1001) docker     (127)   732622 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_images/images.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_list_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_logprobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_num_choices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_scorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_stop_reason.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_subprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.504143 inspect_ai-0.3.9/tests/test_task_list/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_task_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_task_list/attribs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_task_list/multiple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.504143 inspect_ai-0.3.9/tests/test_task_list/multiple_dir/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.504143 inspect_ai-0.3.9/tests/test_task_list/multiple_dir/_decoy/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_task_list/multiple_dir/_decoy/testit.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_task_list/multiple_dir/_decoy2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_task_list/multiple_dir/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_task_list/multiple_dir/foo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.440143 inspect_ai-0.3.9/tests/test_task_list/recurse/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.504143 inspect_ai-0.3.9/tests/test_task_list/recurse/.folder3/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_task_list/recurse/.folder3/epsilon.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.504143 inspect_ai-0.3.9/tests/test_task_list/recurse/folder1/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_task_list/recurse/folder1/_decoy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_task_list/recurse/folder1/theta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.504143 inspect_ai-0.3.9/tests/test_task_list/recurse/folder2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.504143 inspect_ai-0.3.9/tests/test_task_list/recurse/folder2/.folder3/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_task_list/recurse/folder2/.folder3/epsilon.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_task_list/recurse/folder2/another.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_task_list/recurse/folder2/first.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.440143 inspect_ai-0.3.9/tools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.508143 inspect_ai-0.3.9/tools/vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/.eslintrc.json
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.508143 inspect_ai-0.3.9/tools/vscode/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/.vscode-test.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/.vscodeignore
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/.yarnrc
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.444143 inspect_ai-0.3.9/tools/vscode/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.508143 inspect_ai-0.3.9/tools/vscode/assets/logo/
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/assets/logo/inspect.png
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/assets/logo/inspect.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.508143 inspect_ai-0.3.9/tools/vscode/assets/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/assets/templates/task.py.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.444143 inspect_ai-0.3.9/tools/vscode/assets/www/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.508143 inspect_ai-0.3.9/tools/vscode/assets/www/codicon/
+-rw-r--r--   0 runner    (1001) docker     (127)    27023 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/assets/www/codicon/codicon.css
+-rw-r--r--   0 runner    (1001) docker     (127)    72860 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/assets/www/codicon/codicon.ttf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.508143 inspect_ai-0.3.9/tools/vscode/assets/www/view/
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/assets/www/view/view-overrides.css
+-rw-r--r--   0 runner    (1001) docker     (127)    10445 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.508143 inspect_ai-0.3.9/tools/vscode/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.512143 inspect_ai-0.3.9/tools/vscode/src/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/components/document.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/components/error.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/components/focus.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/components/notebook.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/components/symbol.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/components/task.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/components/templates.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     7419 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/components/webview.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.512143 inspect_ai-0.3.9/tools/vscode/src/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/core/appdirs.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/core/command.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/core/dispose.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/core/env.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/core/git.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/core/jsonrpc.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/core/log.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/core/nonce.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/core/path.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/core/port.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/core/process.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.512143 inspect_ai-0.3.9/tools/vscode/src/core/python/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/core/python/code.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/core/python/exec.ts
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/core/python/index.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/core/python/interpreter.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/core/random.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/core/string.ts
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/core/text.ts
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/core/wait.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/core/workspace.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/extension.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.512143 inspect_ai-0.3.9/tools/vscode/src/inspect/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/inspect/index.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/inspect/list.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/inspect/logs.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/inspect/props.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.444143 inspect_ai-0.3.9/tools/vscode/src/providers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.516143 inspect_ai-0.3.9/tools/vscode/src/providers/active-task/
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/providers/active-task/active-task-command.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/providers/active-task/active-task-provider.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.516143 inspect_ai-0.3.9/tools/vscode/src/providers/activity-bar/
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/providers/activity-bar/activity-bar-provider.ts
+-rw-r--r--   0 runner    (1001) docker     (127)    14105 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/providers/activity-bar/env-config-provider.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/providers/activity-bar/task-config-commands.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     9720 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/providers/activity-bar/task-config-provider.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     8251 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/providers/activity-bar/task-outline-commands.ts
+-rw-r--r--   0 runner    (1001) docker     (127)    11527 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/providers/activity-bar/task-outline-provider.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.516143 inspect_ai-0.3.9/tools/vscode/src/providers/activity-bar/webview/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/providers/activity-bar/webview/env-config-webview.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/providers/activity-bar/webview/env-config-webview.ts
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/providers/activity-bar/webview/task-config-webview.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/providers/activity-bar/webview/task-config-webview.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/providers/activity-bar/webview/vscode-controls.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/providers/activity-bar/webview/webview-utils.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.516143 inspect_ai-0.3.9/tools/vscode/src/providers/codelens/
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/providers/codelens/codelens-provider.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.516143 inspect_ai-0.3.9/tools/vscode/src/providers/inspect/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/providers/inspect/inspect-constants.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/providers/inspect/inspect-eval-commands.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/providers/inspect/inspect-eval.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/providers/inspect/inspect-manager.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.520143 inspect_ai-0.3.9/tools/vscode/src/providers/logview/
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/providers/logview/commands.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/providers/logview/logview-file-watcher.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/providers/logview/logview-link-provider.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/providers/logview/logview-manager.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/providers/logview/logview-webview.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/providers/logview/logview.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.520143 inspect_ai-0.3.9/tools/vscode/src/providers/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/providers/settings/inspect-settings.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/providers/settings/user-settings.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.520143 inspect_ai-0.3.9/tools/vscode/src/providers/workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/providers/workspace/workspace-env-commands.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/providers/workspace/workspace-env-provider.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/providers/workspace/workspace-init.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/providers/workspace/workspace-state-provider.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/providers/workspace/workspace-task-provider.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.520143 inspect_ai-0.3.9/tools/vscode/src/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/src/test/extension.test.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.444143 inspect_ai-0.3.9/tools/vscode/tools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.520143 inspect_ai-0.3.9/tools/vscode/tools/ts-to-mjs/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/tools/ts-to-mjs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/tools/ts-to-mjs/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/tools/ts-to-mjs/rollup.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:33:59.520143 inspect_ai-0.3.9/tools/vscode/tools/ts-to-mjs/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/tools/ts-to-mjs/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/tools/ts-to-mjs/src/jsonrpc.ts
+-rw-r--r--   0 runner    (1001) docker     (127)   129610 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/tools/ts-to-mjs/yarn.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/webpack.config.js
+-rw-r--r--   0 runner    (1001) docker     (127)   158644 2024-05-14 19:33:54.000000 inspect_ai-0.3.9/tools/vscode/yarn.lock
```

### Comparing `inspect_ai-0.3.8/.github/workflows/build.yml` & `inspect_ai-0.3.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/.github/workflows/docs.yml` & `inspect_ai-0.3.9/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/.github/workflows/pypi.yml` & `inspect_ai-0.3.9/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/.github/workflows/vscode.yml` & `inspect_ai-0.3.9/.github/workflows/vscode.yml`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/.gitignore` & `inspect_ai-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/.pre-commit-config.yaml` & `inspect_ai-0.3.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/CHANGELOG.md` & `inspect_ai-0.3.9/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # Changelog
 
+## v0.3.9 (14 May 2024)
+
+- Add `ollama` local model provider.
+- Add `multi_scorer()` and `majority_vote()` functions for combining multiple scorers into a single score.
+- Add support for multiple model graders in `model_graded_qa()`.
+- Raise `TypeError` for solvers and scorers not declared as `async`.
+- Fallback to standard parase if `NaN` or `Inf` is encountered while reading log file header.
+- Remove deprecated support for matching partial model names (e.g. "gpt" or "claude").
+
 ## v0.3.8 (07 May 2024)
 
 - Exclude null config values from listings in log viewer.
 
 ## v0.3.7 (07 May 2024)
 
 - Add support for logprobs to HF provider, and create uniform API for other providers that support logprobs (Together and OpenAI).
```

### Comparing `inspect_ai-0.3.8/LICENSE` & `inspect_ai-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/PKG-INFO` & `inspect_ai-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspect_ai
-Version: 0.3.8
+Version: 0.3.9
 Summary: Framework for large language model evaluations
 Author: UK AI Safety Institute
 License: MIT License
 Project-URL: Documentation, https://UKGovernmentBEIS.github.io/inspect_ai/
 Project-URL: Source Code, https://github.com/UKGovernmentBEIS/inspect_ai
 Project-URL: Issue Tracker, https://github.com/UKGovernmentBEIS/inspect_ai/issues
 Classifier: Development Status :: 4 - Beta
@@ -95,8 +95,8 @@
 
 ```         
 $ git clone https://github.com/UKGovernmentBEIS/inspect_ai.git
 $ cd inspect_ai
 $ pip install -e ".[dev]"
 ```
 
-If you use VS Code, you should be sure to have installed the recommended extensions (Python, Ruff, and MyPy). Note that you'll be promoted to install these when you open the project in VS Code.
+If you use VS Code, you should be sure to have installed the recommended extensions (Python, Ruff, and MyPy). Note that you'll be prompted to install these when you open the project in VS Code.
```

### Comparing `inspect_ai-0.3.8/README.md` & `inspect_ai-0.3.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 ```         
 $ git clone https://github.com/UKGovernmentBEIS/inspect_ai.git
 $ cd inspect_ai
 $ pip install -e ".[dev]"
 ```
 
-If you use VS Code, you should be sure to have installed the recommended extensions (Python, Ruff, and MyPy). Note that you'll be promoted to install these when you open the project in VS Code.
+If you use VS Code, you should be sure to have installed the recommended extensions (Python, Ruff, and MyPy). Note that you'll be prompted to install these when you open the project in VS Code.
```

### Comparing `inspect_ai-0.3.8/benchmarks/README.md` & `inspect_ai-0.3.9/benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/benchmarks/arc.py` & `inspect_ai-0.3.9/benchmarks/arc.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/benchmarks/gpqa.py` & `inspect_ai-0.3.9/benchmarks/gpqa.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/benchmarks/gsm8k.py` & `inspect_ai-0.3.9/benchmarks/gsm8k.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/benchmarks/hellaswag.py` & `inspect_ai-0.3.9/benchmarks/hellaswag.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/benchmarks/mathematics.py` & `inspect_ai-0.3.9/benchmarks/mathematics.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/benchmarks/mmlu.py` & `inspect_ai-0.3.9/benchmarks/mmlu.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/docs/_examples/arc.qmd` & `inspect_ai-0.3.9/docs/_examples/arc.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/docs/_examples/biology_qa.qmd` & `inspect_ai-0.3.9/docs/_examples/biology_qa.qmd`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 -   `GOOGLE_CSE_ID` — Google Custom Search Engine ID
 
 -   `GOOGLE_CSE_API_KEY` — Google API key used to enable the Search API
 
 
 ### Eval {.unlisted}
 
-Note that in the sample records above the dataset columns are not **input** and **target** so wee'll use a custom `FieldSpec` in our call to `example_dataset`. We also call the `use_tools()` function, passing `web_search()` as a tool---this gives the model access to a Google Search API that can be used to fill in background knowledge or specific facts. We use a `model_graded_qa()` scorer to more reliably score longer form model output.
+Note that in the sample records above the dataset columns are not **input** and **target** so we'll use a custom `FieldSpec` in our call to `example_dataset`. We also call the `use_tools()` function, passing `web_search()` as a tool---this gives the model access to a Google Search API that can be used to fill in background knowledge or specific facts. We use a `model_graded_qa()` scorer to more reliably score longer form model output.
 
 ```{python}
 from inspect_ai import Task, eval, task
 from inspect_ai.dataset import FieldSpec, example_dataset
 from inspect_ai.scorer import model_graded_qa
 from inspect_ai.solver import generate, use_tools, web_search
 
@@ -45,15 +45,15 @@
 
 ```bash
 inspect eval biology_qa.py
 ```
 
 Note that you may not be able to run this example as it requires that you setup a Google Custom Search Engine and provide the `GOOGLE_API_KEY` and `GOOGLE_CSE_ID` environment variables.
 
-The `web_search()` tool uses a model to summarize search results. By defualt it will use the same model as the one being evaluated, however you can choose a different model like this:
+The `web_search()` tool uses a model to summarize search results. By default it will use the same model as the one being evaluated, however you can choose a different model like this:
 
 ``` python
 plan=[
     use_tools(
         web_search(model="anthropic/claude-3-opus-20240229")
     ), 
     generate()
```

### Comparing `inspect_ai-0.3.8/docs/_examples/footer.qmd` & `inspect_ai-0.3.9/docs/_examples/footer.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/docs/_examples/gsm8k.qmd` & `inspect_ai-0.3.9/docs/_examples/gsm8k.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/docs/_examples/hellaswag.qmd` & `inspect_ai-0.3.9/docs/_examples/hellaswag.qmd`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ## HellaSwag {#sec-hellaswag}
 
-[HellaSwag](https://rowanzellers.com/hellaswag/) is a dataset designed to test commonsense natural language inference (NLI) about physical situations. It includes samples that are adversarially constructed to violate common sense about the physical world, so can be a challange for some language models.
+[HellaSwag](https://rowanzellers.com/hellaswag/) is a dataset designed to test commonsense natural language inference (NLI) about physical situations. It includes samples that are adversarially constructed to violate common sense about the physical world, so can be a challenge for some language models.
 
 For example, here is one of the questions in the dataset along with its set of possible answer (the correct answer is C):
 
 > In home pet groomers demonstrate how to groom a pet. the person
 >
 > A) puts a setting engage on the pets tongue and leash.
 > B) starts at their butt rise, combing out the hair with a brush from a red.
@@ -47,15 +47,15 @@
     )
 ```
 
 Note that even though we don't use it for the evaluation, we save the `source_id` as metadata as a way to reference samples in the underlying dataset.
 
 ### Eval {.unlisted}
 
-We'll load the datasat from [HuggingFace](https://huggingface.co/datasets/Rowan/hellaswag) using the `hf_dataset()` function. We'll draw data from the validation split, and use the `record_to_sample()` function to parse the records (we'll also pass `trust=True` to indicate that we are okay with Hugging Face executing the dataset loading code provided by hellaswag):
+We'll load the dataset from [HuggingFace](https://huggingface.co/datasets/Rowan/hellaswag) using the `hf_dataset()` function. We'll draw data from the validation split, and use the `record_to_sample()` function to parse the records (we'll also pass `trust=True` to indicate that we are okay with Hugging Face executing the dataset loading code provided by hellaswag):
 
 ```{python}
 @task
 def hellaswag():
    
     # dataset
     dataset = hf_dataset(
```

### Comparing `inspect_ai-0.3.8/docs/_examples/index.qmd` & `inspect_ai-0.3.9/docs/_examples/index.qmd`

 * *Files 1% similar despite different names*

```diff
@@ -30,9 +30,9 @@
 :::
 
 Many of these examples are simple for the purposes of illustration. However, Inspect is designed for the creation of considerably more complicated evaluations. See [Solvers](#sec-solvers), [Tools](#sec-tools), and [Scorers](#sec-scorers) to learn more.
 
 Several of the examples implement language model benchmarks. The code for these benchmarks and some others can be found in the [benchmarks directory](https://github.com/UKGovernmentBEIS/inspect_ai/tree/main/benchmarks) of the Inspect repository.
 
 ::: {.callout-note appearance="simple"}
-Note that in these examples we won't show a `--model` command line argument when we call `inspect eval` (the presumtion being that it has been already established via the `INSPECT_EVAL_MODEL` environment variable).
+Note that in these examples we won't show a `--model` command line argument when we call `inspect eval` (the presumption being that it has been already established via the `INSPECT_EVAL_MODEL` environment variable).
 :::
```

### Comparing `inspect_ai-0.3.8/docs/_examples/mathematics.qmd` & `inspect_ai-0.3.9/docs/_examples/mathematics.qmd`

 * *Files 3% similar despite different names*

```diff
@@ -75,32 +75,32 @@
             ),
             shuffle=shuffle,
         ),
         plan=[
             prompt_template(PROMPT_TEMPLATE),
             generate(),
         ],
-        scorer=expression_equivalance(),
+        scorer=expression_equivalence(),
         config=GenerateConfig(temperature=0.5),
     )
 
 ```
 
-The heart of this eval isn't in the task definition though, rather its in how we grade the output. Math expressions can be logically equivalent but not literally the same. Consequently, we'll use a model to assess whether the output and the target are logically equivalent. the `expression_equivalance()` custom scorer implements this:
+The heart of this eval isn't in the task definition though, rather it's in how we grade the output. Math expressions can be logically equivalent but not literally the same. Consequently, we'll use a model to assess whether the output and the target are logically equivalent. the `expression_equivalence()` custom scorer implements this:
 
 ```{python}
 @scorer(metrics=[accuracy(), bootstrap_std()])
-def expression_equivalance():
+def expression_equivalence():
     async def score(state: TaskState, target: Target):
         # extract answer
         match = re.search(AnswerPattern.LINE, state.output.completion)
         if match:
-            # ask the model to judge equivalance
+            # ask the model to judge equivalence
             answer = match.group(1)
-            prompt = EQUIVALANCE_TEMPLATE % (
+            prompt = EQUIVALENCE_TEMPLATE % (
                 {"expression1": target.text, "expression2": answer}
             )
             result = await get_model().generate(prompt)
 
             # return the score
             correct = result.completion.lower() == "yes"
             return Score(
@@ -114,18 +114,18 @@
                 explanation="Answer not found in model output: "
                 + f"{state.output.completion}",
             )
 
     return score
 ```
 
-We are making a separate call to the model to assess equivalence. We prompt for this using an `EQUIVALANCE_TEMPLATE`. Here's a general flavor for how that template looks (there are more examples in the real template):
+We are making a separate call to the model to assess equivalence. We prompt for this using an `EQUIVALENCE_TEMPLATE`. Here's a general flavor for how that template looks (there are more examples in the real template):
 
 ``` python
-EQUIVALANCE_TEMPLATE = r"""
+EQUIVALENCE_TEMPLATE = r"""
 Look at the following two expressions (answers to a math problem)
 and judge whether they are equivalent. Only perform trivial 
 simplifications
 
 Examples:
 
     Expression 1: $2x+3$
@@ -165,15 +165,15 @@
 
 ``` bash
 $ inspect eval arc.py --limit 100,200 -T shuffle=false
 ```
 
 ::: content-hidden
 ```{python}
-EQUIVALANCE_TEMPLATE = r"""
+EQUIVALENCE_TEMPLATE = r"""
 Look at the following two expressions (answers to a math problem) and
 judge whether they are equivalent. Only perform trivial simplifications
 
 Examples:
 
     Expression 1: $2x+3$
     Expression 2: $3+2x$
```

### Comparing `inspect_ai-0.3.8/docs/_examples/popularity.qmd` & `inspect_ai-0.3.9/docs/_examples/popularity.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/docs/_examples/security_guide.qmd` & `inspect_ai-0.3.9/docs/_examples/security_guide.qmd`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ## Security Guide {#sec-security-guide}
 
-The security guide example contains 16 question-answer pairs taken from the security guide dataset published in the [Open AI Evals](https://github.com/openai/evals) repository. This eval tests how well models are doing at providing cybersecurity guidance. Here are some examples from the dataset:
+The security guide example contains 16 question-answer pairs taken from the security guide dataset published in the [OpenAI Evals](https://github.com/openai/evals) repository. This eval tests how well models are doing at providing cybersecurity guidance. Here are some examples from the dataset:
 
 | input                                                                        | target                                                    |
 |-----------------------------------------|-------------------------------|
 | What attributes should I set on cookies for strong security?                 | secure samesite and httponly                              |
 | How should I store passwords securely for an authentication system database? | strong hashing algorithms with salt like Argon2 or bcrypt |
 
 ### Setup {.unlisted}
@@ -23,15 +23,15 @@
 Please assume that the reader is also well versed in
 computer security and provide a short response in a few words.
 """
 ```
 
 ### Eval {.unlisted}
 
-Discering whether the correct security guideance was provided by the model might provide difficult using only text matching algorithms. Here we use a model to read the response and assess the quality of the answer.
+Discerning whether the correct security guidance was provided by the model might provide difficult using only text matching algorithms. Here we use a model to read the response and assess the quality of the answer.
 
 ```{python}
 @task
 def security_guide():
     return Task(
         dataset=example_dataset("security_guide"),
         plan=[system_message(SYSTEM_MESSAGE), generate()],
```

### Comparing `inspect_ai-0.3.8/docs/_examples/theory_of_mind.qmd` & `inspect_ai-0.3.9/docs/_examples/theory_of_mind.qmd`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 | input                                                                                                                                                                                                                                   | target  |
 |---------------------------------------------------------|---------------|
 | Jackson entered the hall. Chloe entered the hall. The boots is in the bathtub. Jackson exited the hall. Jackson entered the dining_room. Chloe moved the boots to the pantry. Where was the boots at the beginning?                     | bathtub |
 | Hannah entered the patio. Noah entered the patio. The sweater is in the bucket. Noah exited the patio. Ethan entered the study. Ethan exited the study. Hannah moved the sweater to the pantry. Where will Hannah look for the sweater? | pantry  |
 
 ### Eval {.unlisted}
 
-This example demonstrates adding parameters to a `@task` function to create dynamic variants of an evaluation. Here we use a `critique` parameter to deterine whether a `self_critique()` solver is able to improve on the model's baseline answer.
+This example demonstrates adding parameters to a `@task` function to create dynamic variants of an evaluation. Here we use a `critique` parameter to determine whether a `self_critique()` solver is able to improve on the model's baseline answer.
 
 ```{python}
 from inspect_ai import Task, eval, task
 from inspect_ai.dataset import example_dataset
 from inspect_ai.scorer import model_graded_fact
 from inspect_ai.solver import (
     chain_of_thought, generate, self_critique
```

### Comparing `inspect_ai-0.3.8/docs/_examples/tool_use.qmd` & `inspect_ai-0.3.9/docs/_examples/tool_use.qmd`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
 ```bash
 inspect eval addition_problem.py
 ```
 
 ## File Listing {.unlisted}
 
-The next examples demonstrates how to define a tool that calls an external processs.
+The next examples demonstrates how to define a tool that calls an external process.
 
 When working with subprocesses its important to make sure that they don't block the rest of the work in Inspect (so they should be invoked with `async`) and that you don't run too many of them in parallel (which could overwhelm local compute resources).
 
 To assist with this, Inspect provides the `subprocess()` function. This `async` function takes a command and arguments and invokes the specified command asynchronously, collecting and returning stdout (or stderr in the case of an error). The `subprocess()` function also automatically limits concurrent child processes to the number of CPUs on your system (`os.cpu_count()`).
 
 Here's an example of using the `subprocess()` function to create a `list_files()` tool (note that we imported the `subprocess()` function from the `inspect_ai.util` module above):
```

### Comparing `inspect_ai-0.3.8/docs/_quarto.yml` & `inspect_ai-0.3.9/docs/_quarto.yml`

 * *Files 18% similar despite different names*

```diff
@@ -6,19 +6,24 @@
 book:
    title: "Inspect"
    subtitle: "An open-source framework for large language model evaluations"
    page-navigation: true
    repo-url: https://github.com/UKGovernmentBEIS/inspect_ai
    site-url: https://UKGovernmentBEIS.github.io/inspect_ai/
    repo-actions: [issue]
-   downloads: [pdf, epub, docx]
+   # downloads: [pdf, epub, docx]
    twitter-card:
+      title: "Inspect"
       description: "Open-source framework for large language model evaluations"
+      image: images/inspect.png
+      card-style: summary_large_image
    open-graph: 
+      title: "Inspect"
       description: "Open-source framework for large language model evaluations"
+      image: images/inspect.png
    sidebar:
       header: >
          [![](images/aisi-logo.png){fig-alt="UK AI Safety Institute Website"}](https://www.gov.uk/government/organisations/ai-safety-institute)
 
    page-footer: 
       left: 
          - text: UK AI Safety Institute
@@ -43,14 +48,16 @@
       
    chapters: 
       - "index.qmd"     
       - part: "Basics"
         chapters:
            - workflow.qmd
            - log-viewer.qmd
+           - text: "VS Code"
+             href: vscode.qmd
            - examples.qmd
 
       - part: "Components"
         chapters: 
            - solvers.qmd
            - tools.qmd
            - scorers.qmd
@@ -69,23 +76,23 @@
 
 format:
    html:
      theme: [cosmo, theme.scss]
      toc-depth: 3
      number-sections: false
      code-annotations: select
-   pdf: 
-      number-depth: 1
-      listings: false
-      author: UK AI Safety Institute
-      date: today
-   docx: 
-      author: UK AI Safety Institute
-      date: today
-   epub: 
-      author: UK AI Safety Institute
-      date: today
+   # pdf: 
+   #    number-depth: 1
+   #    listings: false
+   #    author: UK AI Safety Institute
+   #    date: today
+   # docx: 
+   #    author: UK AI Safety Institute
+   #    date: today
+   # epub: 
+   #    author: UK AI Safety Institute
+   #    date: today
 
 execute: 
   enabled: false
```

### Comparing `inspect_ai-0.3.8/docs/datasets.qmd` & `inspect_ai-0.3.9/docs/datasets.qmd`

 * *Files 0% similar despite different names*

```diff
@@ -206,15 +206,15 @@
 ChatMessageUser(content = [
     ContentText(text="What is this a picture of?"),
     ContentImage(image="picture.png")
 ])
 ```
 
 ::: {.callout-note appearance="simple"}
-Note that image input is currently only supported for Open AI vision models (e.g. [gpt-4-vision-preview](https://platform.openai.com/docs/guides/vision)), Google Gemini vision models (e.g. [gemini-pro-vision](https://console.cloud.google.com/vertex-ai/publishers/google/model-garden/gemini-pro-vision)), and Anthropic Claude 3 models.
+Note that image input is currently only supported for OpenAI vision models (e.g. [gpt-4-vision-preview](https://platform.openai.com/docs/guides/vision)), Google Gemini vision models (e.g. [gemini-pro-vision](https://console.cloud.google.com/vertex-ai/publishers/google/model-garden/gemini-pro-vision)), and Anthropic Claude 3 models.
 :::
 
 ## Custom Reader
 
 You are not restricted to the built in dataset functions for reading samples. Since the `dataset` field of the `Task` class takes either a `Dataset` or a sequences of`Sample`, the following is also valid:
 
 ``` python
```

### Comparing `inspect_ai-0.3.8/docs/eval-logs.qmd` & `inspect_ai-0.3.9/docs/eval-logs.qmd`

 * *Files 1% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 
 You can also use the Inspect log viewer for interactive exploration of logs. Run this command once at the beginning of a working session (the view will update automatically when new evaluations are run):
 
 ```bash
 $ inspect view
 ```
 
-![](images/inspect-view-main.png){.border .lightbox fig-alt="The Inspect log viewer, displahing a summary of results for the task as well as 8 individual samples."}
+![](images/inspect-view-main.png){.border .lightbox fig-alt="The Inspect log viewer, displaying a summary of results for the task as well as 8 individual samples."}
 
 This section won't cover using `inspect view` though. Rather, it will cover the details of managing log usage from the CLI as well as the Python API for reading logs. See the [Log Viewer](#sec-log-viewer)  section for details on interactively exploring logs.
 
 
 ## Log Location
 
-By default, logs are written to the `./logs` sub-directory of the current working directory You can change where logs are written using eval options or an environment variable
+By default, logs are written to the `./logs` sub-directory of the current working directory You can change where logs are written using eval options or an environment variable:
 
 ``` bash
 $ inspect eval popularity.py --model openai/gpt-4 --log-dir ./experiment-log
 ```
 
 Or:
 
@@ -94,25 +94,25 @@
 # setup log dir context
 os.environ["INSPECT_LOG_DIR"] = "./experiment-logs"
 
 # do a bunch of evals
 eval(popularity, model="openai/gpt-4")
 eval(security_guide, model="openai/gpt-4")
 
-# analyze the reuslts in the logs
+# analyze the results in the logs
 logs = list_eval_logs()
 ```
 
 Note that `list_eval_logs()` lists log files recursively. Pass `recursive=False` to list only the log files at the root level.
 
 ## Errors and Retries
 
 The example above isn't quite complete as it doesn't demonstrate checking the log for success status. This also begs the question of what to do with failed evaluation tasks. In some cases failed tasks need further debugging, but in other cases they may have failed due to connectivity or API rate limiting. For these cases, Inspect includes an `eval_retry()` function that you can pass a log to.
 
-Here's an example of checking for logs with errors and retrying them with a lower number of max connections(the theory in this case being that too many concurrent connections may have caused a rate limit error:
+Here's an example of checking for logs with errors and retrying them with a lower number of max connections(the theory in this case being that too many concurrent connections may have caused a rate limit error):
 
 ``` python
 logs = list_eval_logs(filter = lambda log: log.status == "error")
 eval_retry(logs, max_connections = 3)
 ```
 
 ## Amazon S3 {#sec-amazon-s3}
@@ -127,15 +127,15 @@
 ```
 
 One thing to keep in mind if you are storing logs on S3 is that they will no longer be easily viewable using a local text editor. You will likely want to configure a [FUSE filesystem](https://github.com/s3fs-fuse/s3fs-fuse) so you can easily browse the S3 logs locally.
 
 
 ## Log CLI Commands
 
-We've shown a number of Python functions that let you work with eval logs from code. However, you may be writing an orchestration or visualisation tool in another language (e.g. Typescript) where its not particularly convenient to call the Python API. The Inspect CLI has a few commands intended to make it easier to work with Inspect logs from other languages.
+We've shown a number of Python functions that let you work with eval logs from code. However, you may be writing an orchestration or visualisation tool in another language (e.g. TypeScript) where its not particularly convenient to call the Python API. The Inspect CLI has a few commands intended to make it easier to work with Inspect logs from other languages.
 
 ### Listing Logs
 
 You can use the `inspect list logs` command to enumerate all of the logs for a given log directory. This command will utilise the `INSPECT_LOG_DIR` if it is set (alternatively you can specify a `--log-dir` directly). You'll likely also want to use the `--json` flag to get more granular and structured information on the log files. For example:
 
 ``` bash
 $ inspect list logs --json           # uses INSPECT_LOG_DIR
@@ -156,15 +156,15 @@
 For example, here we read a local log file and a log file on Amazon S3:
 
 ``` bash
 $ inspect info log-file file:///home/user/log/logfile.json
 $ inspect info log-file s3://my-evals-bucket/logfile.json
 ```
 
-Log files are stored in JSON. You can get the JSON schema and Typescript type definitions for the log file format with the following calls to `inspect info`:
+Log files are stored in JSON. You can get the JSON schema and TypeScript type definitions for the log file format with the following calls to `inspect info`:
 
 ``` bash
 $ inspect info log-schema
 $ inspect info log-types
 ```
 
 ::: {.callout-important appearance="simple"}
```

### Comparing `inspect_ai-0.3.8/docs/eval-suites.qmd` & `inspect_ai-0.3.9/docs/eval-suites.qmd`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 This is a natural and convenient way to run evals during development, but in a task suite you'll want `inspect eval` to do the execution rather than direct calls to `eval()` (as this allows for varying the model, generation config, and task parameters dynamically). You can keep your existing code more or less as-is, but you'll just want to add one line above `eval()`:
 
 ``` python
 if __name__ == "__main__":
     eval(security_guide, model="google/gemini-1.0-pro")
 ```
 
-Doing this allows your source file to be both a Python script that is convenient to run during development as well as be a Python module that tasks can be read from without executing the eval. There is no real downside to this, and it's a good way in general to write all of your eval scripts and notebooks (see the docs on [\_\_main\_\_](https://docs.python.org/3/library/main.html) for additional details).
+Doing this allows your source file to be both a Python script that is convenient to run during development as well as be a Python module that tasks can be read from without executing the eval. There is no real downside to this, and it's a good way in general to write all of your eval scripts and notebooks (see the docs on [\_\_main\_\_](https://docs.python.org/3/library/__main__.html) for additional details.)
 
 ## Use Cases
 
 ### Multiple Tasks in a File
 
 The simplest possible eval suite would be multiple tasks defined in a single source file. Consider this source file (`ctf.py`) with two tasks in it:
 
@@ -64,15 +64,15 @@
 @task
 def attack_defense():
   return Task(
     ...
   )
 ```
 
-We can run both of these tasks with the following command (note for this and the remainder of examples we'll assume that you have let an `INSPECT_EVAL_MODEL` environment variable so you don't need to pass the `--model` argument explicitly).
+We can run both of these tasks with the following command (note for this and the remainder of examples we'll assume that you have let an `INSPECT_EVAL_MODEL` environment variable so you don't need to pass the `--model` argument explicitly):
 
 ``` bash
 $ inspect eval ctf.py 
 ```
 
 Note we could also run the tasks individually as follows (e.g. for development and debugging):
 
@@ -114,28 +114,28 @@
 ```
 
 Note that some of the files in this directory don't contain evals (e.g. `import.py` and `analyze.py`). These files are not read or executed by `inspect eval` (which only executes files that contain `@task` definitions).
 
 If we wanted to run more than one directory we could do so by just passing multiple directory names. For example:
 
 ``` bash
-$ inspect eval security pursuasion
+$ inspect eval security persuasion
 ```
 
 ### Eval Function
 
 Note that all of the above example uses of `inspect eval` apply equally to the `eval()` function. in the context of the above, all of these statements would work as expected:
 
 ``` python
 eval("ctf.py")
 eval("ctf.py@jeopardy")
 eval("ctf.py@attack_defense")
 
 eval("security")
-eval(["security", "pursuasion"])
+eval(["security", "persuasion"])
 ```
 
 ## Listing and Filtering
 
 ### Recursive Listings
 
 Note that directories or expanded globs of directory names passed to `eval` are recursively scanned for tasks. So you could have a very deep hierarchy of directories, with a mix of task and non task scripts, and the `eval` command or function will discover all of the tasks automatically.
```

### Comparing `inspect_ai-0.3.8/docs/eval-tuning.qmd` & `inspect_ai-0.3.9/docs/eval-tuning.qmd`

 * *Files 1% similar despite different names*

```diff
@@ -63,24 +63,24 @@
 from inspect_ai.solver import Generate, TaskState
 
 client = httpx.AsyncClient()
 
 async def solve(state: TaskState, generate: Generate):
   ...
   # wrap the call to client.get() in an async concurrency 
-  # block to limit simulaneous connections to 10
+  # block to limit simultaneous connections to 10
   async with concurrency("my-rest-api", 10):
     response = await client.get("https://example.com/api")
 ```
 
 Note that we pass a name ("my-rest-api") to the `concurrency()` function. This provides a named scope for managing concurrency for calls to that specific API/service.
 
 ## Subprocesses
 
-It's possible that your custom solvers, tools, or scorers will need to launch child processes to perform various tasks. Subprocesses have similar considerations as calling APIs: you want to make sure that they don't block the rest of the work in Inspect (so they should be invoked with `async`) and you also want to make sure they don't provide *too much* concurrency (i.e. you wouldn't want to launch 200 processes at once on a 4 core machine!).
+It's possible that your custom solvers, tools, or scorers will need to launch child processes to perform various tasks. Subprocesses have similar considerations as calling APIs: you want to make sure that they don't block the rest of the work in Inspect (so they should be invoked with `async`) and you also want to make sure they don't provide *too much* concurrency (i.e. you wouldn't want to launch 200 processes at once on a 4 core machine!)
 
 To assist with this, Inspect provides the `subprocess()` function. This `async` function takes a command and arguments and invokes the specified command asynchronously, collecting and returning stdout and stderr. The `subprocess()` function also automatically limits concurrent child processes to the number of CPUs on your system (`os.cpu_count()`). Here's an example from the implementation of a `list_files()` tool:
 
 ``` python
 @tool(prompt=(
    "If you are asked to list the files in a directory you "
    + "should call the list_files function to access the listing."
```

### Comparing `inspect_ai-0.3.8/docs/examples.qmd` & `inspect_ai-0.3.9/docs/examples.qmd`

 * *Files 0% similar despite different names*

```diff
@@ -30,20 +30,20 @@
 :::
 
 Many of these examples are simple for the purposes of illustration. However, Inspect is designed for the creation of considerably more complicated evaluations. See [Solvers](#sec-solvers), [Tools](#sec-tools), and [Scorers](#sec-scorers) to learn more.
 
 Several of the examples implement language model benchmarks. The code for these benchmarks and some others can be found in the [benchmarks directory](https://github.com/UKGovernmentBEIS/inspect_ai/tree/main/benchmarks) of the Inspect repository.
 
 ::: {.callout-note appearance="simple"}
-Note that in these examples we won't show a `--model` command line argument when we call `inspect eval` (the presumtion being that it has been already established via the `INSPECT_EVAL_MODEL` environment variable).
+Note that in these examples we won't show a `--model` command line argument when we call `inspect eval` (the presumption being that it has been already established via the `INSPECT_EVAL_MODEL` environment variable).
 :::
 
 ## Security Guide {#sec-security-guide}
 
-The security guide example contains 16 question-answer pairs taken from the security guide dataset published in the [Open AI Evals](https://github.com/openai/evals) repository. This eval tests how well models are doing at providing cybersecurity guidance. Here are some examples from the dataset:
+The security guide example contains 16 question-answer pairs taken from the security guide dataset published in the [OpenAI Evals](https://github.com/openai/evals) repository. This eval tests how well models are doing at providing cybersecurity guidance. Here are some examples from the dataset:
 
 | input                                                                        | target                                                    |
 |-----------------------------------------|-------------------------------|
 | What attributes should I set on cookies for strong security?                 | secure samesite and httponly                              |
 | How should I store passwords securely for an authentication system database? | strong hashing algorithms with salt like Argon2 or bcrypt |
 
 ### Setup {.unlisted}
@@ -62,15 +62,15 @@
 Please assume that the reader is also well versed in
 computer security and provide a short response in a few words.
 """
 ```
 
 ### Eval {.unlisted}
 
-Discering whether the correct security guideance was provided by the model might provide difficult using only text matching algorithms. Here we use a model to read the response and assess the quality of the answer.
+Discerning whether the correct security guidance was provided by the model might provide difficult using only text matching algorithms. Here we use a model to read the response and assess the quality of the answer.
 
 ```{python}
 @task
 def security_guide():
     return Task(
         dataset=example_dataset("security_guide"),
         plan=[system_message(SYSTEM_MESSAGE), generate()],
@@ -87,15 +87,15 @@
 ```
 
 
 
 
 ## HellaSwag {#sec-hellaswag}
 
-[HellaSwag](https://rowanzellers.com/hellaswag/) is a dataset designed to test commonsense natural language inference (NLI) about physical situations. It includes samples that are adversarially constructed to violate common sense about the physical world, so can be a challange for some language models.
+[HellaSwag](https://rowanzellers.com/hellaswag/) is a dataset designed to test commonsense natural language inference (NLI) about physical situations. It includes samples that are adversarially constructed to violate common sense about the physical world, so can be a challenge for some language models.
 
 For example, here is one of the questions in the dataset along with its set of possible answer (the correct answer is C):
 
 > In home pet groomers demonstrate how to groom a pet. the person
 >
 > A) puts a setting engage on the pets tongue and leash.
 > B) starts at their butt rise, combing out the hair with a brush from a red.
@@ -138,15 +138,15 @@
     )
 ```
 
 Note that even though we don't use it for the evaluation, we save the `source_id` as metadata as a way to reference samples in the underlying dataset.
 
 ### Eval {.unlisted}
 
-We'll load the datasat from [HuggingFace](https://huggingface.co/datasets/Rowan/hellaswag) using the `hf_dataset()` function. We'll draw data from the validation split, and use the `record_to_sample()` function to parse the records (we'll also pass `trust=True` to indicate that we are okay with Hugging Face executing the dataset loading code provided by hellaswag):
+We'll load the dataset from [HuggingFace](https://huggingface.co/datasets/Rowan/hellaswag) using the `hf_dataset()` function. We'll draw data from the validation split, and use the `record_to_sample()` function to parse the records (we'll also pass `trust=True` to indicate that we are okay with Hugging Face executing the dataset loading code provided by hellaswag):
 
 ```{python}
 @task
 def hellaswag():
    
     # dataset
     dataset = hf_dataset(
@@ -185,15 +185,15 @@
 | input                                                                                                                                                                                                                                   | target  |
 |---------------------------------------------------------|---------------|
 | Jackson entered the hall. Chloe entered the hall. The boots is in the bathtub. Jackson exited the hall. Jackson entered the dining_room. Chloe moved the boots to the pantry. Where was the boots at the beginning?                     | bathtub |
 | Hannah entered the patio. Noah entered the patio. The sweater is in the bucket. Noah exited the patio. Ethan entered the study. Ethan exited the study. Hannah moved the sweater to the pantry. Where will Hannah look for the sweater? | pantry  |
 
 ### Eval {.unlisted}
 
-This example demonstrates adding parameters to a `@task` function to create dynamic variants of an evaluation. Here we use a `critique` parameter to deterine whether a `self_critique()` solver is able to improve on the model's baseline answer.
+This example demonstrates adding parameters to a `@task` function to create dynamic variants of an evaluation. Here we use a `critique` parameter to determine whether a `self_critique()` solver is able to improve on the model's baseline answer.
 
 ```{python}
 from inspect_ai import Task, eval, task
 from inspect_ai.dataset import example_dataset
 from inspect_ai.scorer import model_graded_fact
 from inspect_ai.solver import (
     chain_of_thought, generate, self_critique
@@ -300,32 +300,32 @@
             ),
             shuffle=shuffle,
         ),
         plan=[
             prompt_template(PROMPT_TEMPLATE),
             generate(),
         ],
-        scorer=expression_equivalance(),
+        scorer=expression_equivalence(),
         config=GenerateConfig(temperature=0.5),
     )
 
 ```
 
-The heart of this eval isn't in the task definition though, rather its in how we grade the output. Math expressions can be logically equivalent but not literally the same. Consequently, we'll use a model to assess whether the output and the target are logically equivalent. the `expression_equivalance()` custom scorer implements this:
+The heart of this eval isn't in the task definition though, rather it's in how we grade the output. Math expressions can be logically equivalent but not literally the same. Consequently, we'll use a model to assess whether the output and the target are logically equivalent. the `expression_equivalence()` custom scorer implements this:
 
 ```{python}
 @scorer(metrics=[accuracy(), bootstrap_std()])
-def expression_equivalance():
+def expression_equivalence():
     async def score(state: TaskState, target: Target):
         # extract answer
         match = re.search(AnswerPattern.LINE, state.output.completion)
         if match:
-            # ask the model to judge equivalance
+            # ask the model to judge equivalence
             answer = match.group(1)
-            prompt = EQUIVALANCE_TEMPLATE % (
+            prompt = EQUIVALENCE_TEMPLATE % (
                 {"expression1": target.text, "expression2": answer}
             )
             result = await get_model().generate(prompt)
 
             # return the score
             correct = result.completion.lower() == "yes"
             return Score(
@@ -339,18 +339,18 @@
                 explanation="Answer not found in model output: "
                 + f"{state.output.completion}",
             )
 
     return score
 ```
 
-We are making a separate call to the model to assess equivalence. We prompt for this using an `EQUIVALANCE_TEMPLATE`. Here's a general flavor for how that template looks (there are more examples in the real template):
+We are making a separate call to the model to assess equivalence. We prompt for this using an `EQUIVALENCE_TEMPLATE`. Here's a general flavor for how that template looks (there are more examples in the real template):
 
 ``` python
-EQUIVALANCE_TEMPLATE = r"""
+EQUIVALENCE_TEMPLATE = r"""
 Look at the following two expressions (answers to a math problem)
 and judge whether they are equivalent. Only perform trivial 
 simplifications
 
 Examples:
 
     Expression 1: $2x+3$
@@ -390,15 +390,15 @@
 
 ``` bash
 $ inspect eval arc.py --limit 100,200 -T shuffle=false
 ```
 
 ::: content-hidden
 ```{python}
-EQUIVALANCE_TEMPLATE = r"""
+EQUIVALENCE_TEMPLATE = r"""
 Look at the following two expressions (answers to a math problem) and
 judge whether they are equivalent. Only perform trivial simplifications
 
 Examples:
 
     Expression 1: $2x+3$
     Expression 2: $3+2x$
@@ -477,15 +477,15 @@
 -   `GOOGLE_CSE_ID` — Google Custom Search Engine ID
 
 -   `GOOGLE_CSE_API_KEY` — Google API key used to enable the Search API
 
 
 ### Eval {.unlisted}
 
-Note that in the sample records above the dataset columns are not **input** and **target** so wee'll use a custom `FieldSpec` in our call to `example_dataset`. We also call the `use_tools()` function, passing `web_search()` as a tool---this gives the model access to a Google Search API that can be used to fill in background knowledge or specific facts. We use a `model_graded_qa()` scorer to more reliably score longer form model output.
+Note that in the sample records above the dataset columns are not **input** and **target** so we'll use a custom `FieldSpec` in our call to `example_dataset`. We also call the `use_tools()` function, passing `web_search()` as a tool---this gives the model access to a Google Search API that can be used to fill in background knowledge or specific facts. We use a `model_graded_qa()` scorer to more reliably score longer form model output.
 
 ```{python}
 from inspect_ai import Task, eval, task
 from inspect_ai.dataset import FieldSpec, example_dataset
 from inspect_ai.scorer import model_graded_qa
 from inspect_ai.solver import generate, use_tools, web_search
 
@@ -508,15 +508,15 @@
 
 ```bash
 inspect eval biology_qa.py
 ```
 
 Note that you may not be able to run this example as it requires that you setup a Google Custom Search Engine and provide the `GOOGLE_API_KEY` and `GOOGLE_CSE_ID` environment variables.
 
-The `web_search()` tool uses a model to summarize search results. By defualt it will use the same model as the one being evaluated, however you can choose a different model like this:
+The `web_search()` tool uses a model to summarize search results. By default it will use the same model as the one being evaluated, however you can choose a different model like this:
 
 ``` python
 plan=[
     use_tools(
         web_search(model="anthropic/claude-3-opus-20240229")
     ), 
     generate()
@@ -695,15 +695,15 @@
 
 ```bash
 inspect eval addition_problem.py
 ```
 
 ## File Listing {.unlisted}
 
-The next examples demonstrates how to define a tool that calls an external processs.
+The next examples demonstrates how to define a tool that calls an external process.
 
 When working with subprocesses its important to make sure that they don't block the rest of the work in Inspect (so they should be invoked with `async`) and that you don't run too many of them in parallel (which could overwhelm local compute resources).
 
 To assist with this, Inspect provides the `subprocess()` function. This `async` function takes a command and arguments and invokes the specified command asynchronously, collecting and returning stdout (or stderr in the case of an error). The `subprocess()` function also automatically limits concurrent child processes to the number of CPUs on your system (`os.cpu_count()`).
 
 Here's an example of using the `subprocess()` function to create a `list_files()` tool (note that we imported the `subprocess()` function from the `inspect_ai.util` module above):
```

### Comparing `inspect_ai-0.3.8/docs/images/aisi-logo.png` & `inspect_ai-0.3.9/docs/images/aisi-logo.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/docs/images/eval-log.png` & `inspect_ai-0.3.9/docs/images/eval-log.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/docs/images/inspect-view-answers.png` & `inspect_ai-0.3.9/docs/images/inspect-view-answers.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/docs/images/inspect-view-filter.png` & `inspect_ai-0.3.9/docs/images/inspect-view-filter.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/docs/images/inspect-view-history.png` & `inspect_ai-0.3.9/docs/images/inspect-view-history.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/docs/images/inspect-view-home.png` & `inspect_ai-0.3.9/docs/images/inspect-view-home.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/docs/images/inspect-view-info.png` & `inspect_ai-0.3.9/docs/images/inspect-view-info.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/docs/images/inspect-view-logging-console.png` & `inspect_ai-0.3.9/docs/images/inspect-view-logging-console.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/docs/images/inspect-view-logging.png` & `inspect_ai-0.3.9/docs/images/inspect-view-logging.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/docs/images/inspect-view-main.png` & `inspect_ai-0.3.9/docs/images/inspect-view-main.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/docs/images/inspect-view-messages.png` & `inspect_ai-0.3.9/docs/images/inspect-view-messages.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/docs/images/inspect-view-metadata.png` & `inspect_ai-0.3.9/docs/images/inspect-view-metadata.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/docs/images/inspect-view-scoring.png` & `inspect_ai-0.3.9/docs/images/inspect-view-scoring.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/docs/images/inspect-view-sort.png` & `inspect_ai-0.3.9/docs/images/inspect-view-sort.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/docs/images/inspect-view-splash.png` & `inspect_ai-0.3.9/docs/images/inspect-view-splash.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/docs/images/popularity.png` & `inspect_ai-0.3.9/docs/images/popularity.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/docs/images/rate-limit.png` & `inspect_ai-0.3.9/docs/images/rate-limit.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/docs/images/running-theory.png` & `inspect_ai-0.3.9/docs/images/running-theory.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/docs/index.qmd` & `inspect_ai-0.3.9/docs/index.qmd`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,19 @@
 ---
-toc: false
+toc: true
 ---
 
-::: {layout=[45,55] .splash}
-
-- Easy creation of simple benchmark-style evaluations.
-
-- Scale up to more sophsisticated evals with multi-turn dialog, agent scaffolds and model grading.
-
-- Interactive workflows for researchers; production workflows for larger evaluation suites. 
-
-- Adapt and extend the framework with custom Python components.
-
-![](images/inspect-view-splash.png){.lightbox .border fig-alt="The Inspect log viewer, displahing a summary of results for the task as well as 5 individual samples."}
-
-:::
-
 ## Welcome
 
 Welcome to Inspect, a framework for large language model evaluations created by the [UK AI Safety Institute](https://www.gov.uk/government/organisations/ai-safety-institute).
 
-Inspect provides many built-in components, including facilities for prompt engineering, tool usage, multi-turn dialog, and model graded evaluations. Extensions to Inspect (e.g. to support new elicitation and scoring techniques) can be provided by other Python packages.
+Inspect provides many built-in components, including facilities for prompt engineering, tool usage, multi-turn dialog, and model graded evaluations. Extensions to Inspect (e.g. to support new elicitation and scoring techniques) can be provided by other Python packages. 
+
+![](images/inspect.png){.lightbox .border fig-alt="Inspect running inside Visual Studio Code. The editor shows the ARC evaluation and the log viewer at right shows results from the evaluation."}
+
 
 We'll walk through a fairly trivial "Hello, Inspect" example below. Read on to learn the basics, then read the documentation on [Workflow](#sec-workflow), [Solvers](#sec-solvers), [Tools](#sec-tools), [Scorers](#sec-scorers), [Datasets](#sec-datasets), and [Models](#sec-models) to learn how to create more advanced evaluations.
 
 ## Getting Started
 
 First, install Inspect with:
 
@@ -82,21 +71,21 @@
 ``` bash
 $ pip install openai
 $ export TOGETHER_API_KEY=your-together-api-key
 $ inspect eval ctf.py --model together/Qwen/Qwen1.5-72B-Chat
 ```
 :::
 
-In addition to the model providers shown above, Inspect also supports models hosted on Azure AI, AWS Bedrock, and CloudFlare. See the documentation on [Models](#sec-models) for additional detals.
+In addition to the model providers shown above, Inspect also supports models hosted on Azure AI, AWS Bedrock, and Cloudflare, as well as local models with Ollama. See the documentation on [Models](#sec-models) for additional details.
 
 ## Hello, Inspect {#sec-hello-inspect}
 
 Inspect evaluations have three main components:
 
-1.  **Datasets** contain a set of labeled samples. Datasets are typically just a table with `input` and `target` columns, where `input` is a prompt and `target` is either literal value(s) or grading guideance.
+1.  **Datasets** contain a set of labeled samples. Datasets are typically just a table with `input` and `target` columns, where `input` is a prompt and `target` is either literal value(s) or grading guidance.
 
 2.  **Solvers** are composed together in a *plan* to evaluate the `input` in the dataset. The most elemental solver, `generate()`, just calls the model with a prompt and collects the output. Other solvers might do prompt engineering, multi-turn dialog, critique, etc.
 
 3.  **Scorers** evaluate the final output of solvers. They may use text comparisons, model grading, or other custom schemes
 
 Let's take a look at a simple evaluation that aims to see how models perform on the [Sally-Anne](https://en.wikipedia.org/wiki/Sally%E2%80%93Anne_test) test, which assesses the ability of a person to infer false beliefs in others. Here are some samples from the dataset:
 
@@ -148,44 +137,46 @@
 
 You can also explore eval results using the Inspect log viewer. Run `inspect view` to open the viewer (you only need to do this once as the viewer will automatically updated when new evals are run):
 
 ```bash
 $ inspect view
 ```
 
-![](images/inspect-view-home.png){.border .lightbox fig-alt="The Inspect log viewer, displahing a summary of results for the task as well as 7 individual samples."}
+![](images/inspect-view-home.png){.border .lightbox fig-alt="The Inspect log viewer, displaying a summary of results for the task as well as 7 individual samples."}
 
 See the [Log Viewer](#sec-log-viewer) section for additional details on using Inspect View.
 
 ::: {.callout-note appearance="simple"}
 This example demonstrates evals being run from the terminal with the `inspect eval` command. There is also an `eval()` function which can be used for exploratory work---this is covered further in [Workflow](#sec-workflow).
 :::
 
 ## Learning More
 
-To get stared with Inspect, we highly recommend you read at least these sections for a high level overview of the system:
+To get started with Inspect, we highly recommend you read at least these sections for a high level overview of the system:
 
 -   [Workflow](#sec-workflow) covers the mechanics of running evaluations, including how to create evals in both scripts and notebooks, specifying configuration and options, how to parameterise tasks for different scenarios, and how to work with eval log files.
 
 -   [Log Viewer](#sec-log-viewer) goes into more depth on how to use Inspect View to develop and debug evaluations, including how to provide additional log metadata and how to integrate it with Python's standard logging module.
 
--   [Examples](#sec-examples) provides several complete examples with commentary on the use of various features (as with the above example, they are fairly simplistic for the purposes of illustration). You can also find implementations of a few popular [LLM benchmarks](https://github.com/UKGovernmentBEIS/inspect_ai/tree/main/benchmarks) in the Inspect repository.
+-   [VS Code](#sec-vscode) provides documentation on using the Inspect VS Code Extension to run, tune, debug, and visualise evaluations.
+
+-   [Examples](#sec-examples) includes several complete examples with commentary on the use of various features (as with the above example, they are fairly simplistic for the purposes of illustration). You can also find implementations of a few popular [LLM benchmarks](https://github.com/UKGovernmentBEIS/inspect_ai/tree/main/benchmarks) in the Inspect repository.
 
 These sections provide a more in depth treatment of the various components used in evals. Read them as required as you learn to build evaluations.
 
 -   [Solvers](#sec-solvers) are the heart of Inspect, and encompass prompt engineering and various other elicitation strategies (the `plan` in the example above). Here we cover using the built-in solvers and creating your own more sophisticated ones.
 
 -   [Tools](#sec-tools) provide a means of extending the capabilities of models by registering Python functions for them to call. This section describes how to create custom tools as well as how to run tools within an agent scaffold.
 
 -   [Scorers](#sec-scorers) evaluate the work of solvers and aggregate scores into metrics. Sophisticated evals often require custom scorers that use models to evaluate output. This section covers how to create them.
 
 -   [Datasets](#sec-datasets) provide samples to evaluation tasks. This section illustrates how to adapt various data sources for use with Inspect, as well as how to include multi-modal data (images, etc.) in your datasets.
 
 -   [Models](#sec-models) provide a uniform API for both evaluating a variety of large language models and using models within evaluations (e.g. for critique or grading).
 
-These sections discuss more advanced features and workflow. You don't need to review them at the outset, but be sure to revist them as you get more comfortable with the basics.
+These sections discuss more advanced features and workflow. You don't need to review them at the outset, but be sure to revisit them as you get more comfortable with the basics.
 
 -   [Eval Logs](#sec-eval-logs) describes how to get the most out of evaluation logs for developing, debugging, and analyzing evaluations.
 
 -   [Eval Tuning](#sec-eval-tuning) delves into how to obtain maximum performance for evaluations. Inspect uses a highly parallel async architecture---here we cover how to tune this parallelism (e.g to stay under API rate limits or to not overburden local compute) for optimal throughput.
 
 -   [Eval Suites](#sec-eval-suites) cover Inspect's features for describing, running, and analysing larger sets of evaluation tasks.
```

### Comparing `inspect_ai-0.3.8/docs/log-viewer.qmd` & `inspect_ai-0.3.9/docs/log-viewer.qmd`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Log Viewer {#sec-log-viewer}
 
 ## Overview
 
-Inspect View provides a convenient way to visualise evaluation logs, including drilling into message histories, scoring decisions, and additional metadata written to the log. Here's what the main view of an evaluation log looks like:
+Inspect View provides a convenient way to visualize evaluation logs, including drilling into message histories, scoring decisions, and additional metadata written to the log. Here's what the main view of an evaluation log looks like:
 
-![](images/inspect-view-main.png){.border .lightbox fig-alt="The Inspect log viewer, displahing a summary of results for the task as well as 8 individual samples."}
+![](images/inspect-view-main.png){.border .lightbox fig-alt="The Inspect log viewer, displaying a summary of results for the task as well as 8 individual samples."}
 
 Below we'll describe how to get the most out of using Inspect View.
 
 Note that this section covers *interactively* exploring log files. You can also use the `EvalLog` API to compute on log files (e.g. to compare across runs or to more systematically traverse results). See the section on [Eval Logs](#sec-eval-logs) to learn more about how to process log files with code.
 
 ## View Basics
 
@@ -54,15 +54,15 @@
 
 The scoring tab shows additional details including the full input and full model explanation for answers:
 
 ![](images/inspect-view-scoring.png){.border .lightbox fig-alt="The Inspect log viewer showing a sample expanded, with details on the scoring of the sample, including the input, target, answer, and explanation."}
 
 ### Metadata
 
-The metadata tab shows additional data made available by solvers, tools, an scorers (in this case the `web_search()` tool records which URLs it visited to retreive additional context):
+The metadata tab shows additional data made available by solvers, tools, an scorers (in this case the `web_search()` tool records which URLs it visited to retrieve additional context):
 
 ![](images/inspect-view-metadata.png){.border .lightbox fig-alt="The Inspect log viewer showing a sample expanded, with details on the metadata recorded by the web search tool during the evaluation (specifically, the URLs queried by the web search tool for the sample)."}
 
 ## Scores and Answers
 
 Reliable, high quality scoring is a critical component of every evaluation, and developing custom scorers that deliver this can be challenging. One major difficulty lies in the free form text nature of model output: we have a very specific target we are comparing against and we sometimes need to pick the answer out of a sea of text. Model graded output introduces another set of challenges entirely.
 
@@ -125,15 +125,15 @@
 
 It is important to note that the Inspect View will show all log entries level `info` or higher. However, printing every `info` message to the console during an eval might be too distracting, so the default log level for printing is `warning`. If you change it to `info` then you'll also see these log messages in the console:
 
 ``` bash
 $ inspect eval biology_qa.py --log-level info
 ```
 
-![](images/inspect-view-logging-console.png){.lightbox fig-alt="This Inspect task display in the terminal, with several info log messages from the web search tool printed above the the task diplay."}
+![](images/inspect-view-logging-console.png){.lightbox fig-alt="This Inspect task display in the terminal, with several info log messages from the web search tool printed above the task display."}
 
 A default log level of `warning` enables you to include many calls to `logger.info()` in your code without having them show by default, while also making them available in the log viewer should you need them.
 
 Note that you can also set the log level using the `INSPECT_LOG_LEVEL` environment variable (which is often included in a [.env configuration file](#sec-workflow-configuration)).
 
 ## Task Information
```

### Comparing `inspect_ai-0.3.8/docs/models.qmd` & `inspect_ai-0.3.9/docs/models.qmd`

 * *Files 4% similar despite different names*

```diff
@@ -7,50 +7,56 @@
 | Model API    | Dependencies                      | Environment Variables                                                  |
 |-------------------|----------------------|-------------------------------|
 | OpenAI       | `pip install openai`              | `OPENAI_API_KEY`                                                       |
 | Anthropic    | `pip install anthropic`           | `ANTHROPIC_API_KEY`                                                    |
 | Google       | `pip install google-generativeai` | `GOOGLE_API_KEY`                                                       |
 | Mistral      | `pip install mistralai`           | `MISTRAL_API_KEY`                                                      |
 | Hugging Face | `pip install transformers`        | `HF_TOKEN`                                                             |
+| Ollama       | `pip install openai`              | None required                                                          |
 | TogetherAI   | `pip install openai`              | `TOGETHER_API_KEY`                                                     |
 | AWS Bedrock  | `pip install boto3`               | `AWS_ACCESS_KEY_ID`, `AWS_SECRET_ACCESS_KEY`, and `AWS_DEFAULT_REGION` |
 | Azure AI     | None required                     | `AZURE_API_KEY` and `INSPECT_EVAL_MODEL_BASE_URL`                      |
-| CloudFlare   | None required                     | `CLOUDFLARE_ACCOUNT_ID` and `CLOUDFLARE_API_TOKEN`                     |
+| Cloudflare   | None required                     | `CLOUDFLARE_ACCOUNT_ID` and `CLOUDFLARE_API_TOKEN`                     |
 
 : {tbl-colwidths="\[18,45,37\]"}
 
+::: {.callout-note appearance="minimal"}
+Note that some providers ([Ollama](https://github.com/ollama/ollama/blob/main/docs/openai.md) and [TogetherAI](https://docs.together.ai/docs/openai-api-compatibility)) support the OpenAI Python package as a client, which is why you need to `pip install openai` for these providers even though you aren't actually interacting with the OpenAI service when you use them.
+:::
+
 ## Using Models
 
 To select a model for use in an evaluation task you specify it using a *model name*. Model names include their API provider and the specific model to use (e.g. `openai/gpt-4`) Here are the supported providers along with example model names and links to documentation on all available models:
 
 | Provider     | Model Name                        | Docs                                                                                            |
 |-------------------|---------------------------|---------------------------|
 | OpenAI       | `openai/gpt-3.5-turbo`            | [OpenAI Models](https://platform.openai.com/docs/models/overview)                               |
 | Anthropic    | `anthropic/claude-2.1`            | [Anthropic Models](https://docs.anthropic.com/claude/docs/models-overview)                      |
 | Google       | `google/gemini-1.0-pro`           | [Google Models](https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models)             |
 | Mistral      | `mistral/mistral-large-latest`    | [Mistral Models](https://docs.mistral.ai/platform/endpoints/)                                   |
 | Hugging Face | `hf/openai-community/gpt2`        | [Hugging Face Models](https://huggingface.co/models?pipeline_tag=text-generation&sort=trending) |
+| Ollama       | `ollama/llama3`                   | [Ollama Models](https://ollama.com/library)                                                     |
 | TogetherAI   | `together/lmsys/vicuna-13b-v1.5`  | [TogetherAI Models](https://docs.together.ai/docs/inference-models#chat-models)                 |
 | AWS Bedrock  | `bedrock/meta.llama2-70b-chat-v1` | [AWS Bedrock Models](https://aws.amazon.com/bedrock/)                                           |
 | Azure AI     | `azureai/azure-deployment-name`   | [Azure AI Models](https://ai.azure.com/explore/models)                                          |
-| CloudFlare   | `cf/meta/llama-2-7b-chat-fp16`    | [CloudFlare Models](https://developers.cloudflare.com/workers-ai/models/#text-generation)       |
+| Cloudflare   | `cf/meta/llama-2-7b-chat-fp16`    | [Cloudflare Models](https://developers.cloudflare.com/workers-ai/models/#text-generation)       |
 
 : {tbl-colwidths="\[18,45,37\]"}
 
 To select a model for an evaluation, pass it's name on the command line or use the `model` argument of the `eval()` function:
 
 ``` bash
 $ inspect eval security_guide --model openai/gpt-3.5-turbo
 $ inspect eval security_guide --model anthropic/claude-instant-1.2
 ```
 
 Or:
 
 ``` python
-eval(security_guide, model="openai/opeangpt-3.5-turbo")
+eval(security_guide, model="openai/gpt-3.5-turbo")
 eval(security_guide, model="anthropic/claude-instant-1.2")
 ```
 
 Alternatively, you can set the `INSPECT_EVAL_MODEL` environment variable (either in the shell or a `.env` file) to select a model externally:
 
 ``` bash
 INSPECT_EVAL_MODEL=google/gemini-1.0-pro
@@ -67,17 +73,18 @@
 | Provider    | Environment Variable  |
 |-------------|-----------------------|
 | OpenAI      | `OPENAI_BASE_URL`     |
 | Anthropic   | `ANTHROPIC_BASE_URL`  |
 | Google      | `GOOGLE_BASE_URL`     |
 | Mistral     | `MISTRAL_BASE_URL`    |
 | TogetherAI  | `TOGETHER_BASE_URL`   |
+| Ollama      | `OLLAMA_BASE_URL`     |
 | AWS Bedrock | `BEDROCK_BASE_URL`    |
 | Azure AI    | `AZUREAI_BASE_URL`    |
-| CloudFlare  | `CLOUDFLARE_BASE_URL` |
+| Cloudflare  | `CLOUDFLARE_BASE_URL` |
 
 : {tbl-colwidths="\[50,50\]"}
 
 In addition, there are separate base URL variables for running various frontier models on Azure and Bedrock:
 
 | Provider (Model)    | Environment Variable         |
 |---------------------|------------------------------|
@@ -169,15 +176,15 @@
 $ export AZUREAI_MISTRAL_API_KEY=key
 $ export AZUREAI_MISTRAL_BASE_URL=https://your-url-at.azure.com
 $ inspect eval --model mistral/mistral-large-ctwi
 ```
 
 #### Other Models
 
-Azure AI supports many other model types, you can access these using the `azureai` model provider. As with OpenAI and Mistral, you'll need to specify an `AZUREAI_API_KEY` along with an `AZUREAI_BASE_URL`, as well as use the the [Azure Deployment Name](https://learn.microsoft.com/en-us/azure/ai-services/openai/how-to/create-resource?pivots=web-portal#deploy-a-model) of your model as the model name. For example:
+Azure AI supports many other model types, you can access these using the `azureai` model provider. As with OpenAI and Mistral, you'll need to specify an `AZUREAI_API_KEY` along with an `AZUREAI_BASE_URL`, as well as use the [Azure Deployment Name](https://learn.microsoft.com/en-us/azure/ai-services/openai/how-to/create-resource?pivots=web-portal#deploy-a-model) of your model as the model name. For example:
 
 ``` bash
 $ export AZUREAI_API_KEY=key
 $ export AZUREAI_BASE_URL=https://your-url-at.azure.com
 $ inspect eval --model azureai/llama-2-70b-chat-wnsnw
 ```
 
@@ -306,21 +313,22 @@
 | Provider     | Forwarded to                           |
 |--------------|----------------------------------------|
 | OpenAI       | `AsyncOpenAI`                          |
 | Anthropic    | `AsyncAnthropic`                       |
 | Google       | `genai.configure`                      |
 | Mistral      | `MistralAsyncClient`                   |
 | Hugging Face | `AutoModelForCausalLM.from_pretrained` |
+| Ollama       | `AsyncOpenAI`                          |
 | TogetherAI   | `AsyncOpenAI`                          |
 | AzureAI      | Chat HTTP Post Body                    |
-| CloudFlare   | Chat HTTP Post Body                    |
+| Cloudflare   | Chat HTTP Post Body                    |
 
 : {tbl-colwidths="\[30,70\]"}
 
-See the OpenAI, Anthropic, Google, Mistral, Hugging Face, TogetherAI, Azure AI, and CloudFlare provider documentation for more information on the additional options available.
+See the OpenAI, Anthropic, Google, Mistral, Hugging Face, Ollama, TogetherAI, Azure AI, and Cloudflare provider documentation for more information on the additional options available.
 
 ## Custom Models
 
 You can add a model provider by deriving a new class from `ModelAPI` and adding the `@modelapi` decorator to it. For example:
 
 ``` python
 @modelapi(name="custom")
@@ -354,8 +362,8 @@
 # get a model instance
 model = get_model("custom/name-of-model")
 
 # run an eval with the model
 eval(math, model = "custom/name-of-model")
 ```
 
-In this example, the `model_name` argument passed to `__init__()` will be "name-of-model".
+In this example, the `model_name` argument passed to `__init__()` will be "name-of-model".
```

### Comparing `inspect_ai-0.3.8/docs/scorers.qmd` & `inspect_ai-0.3.9/docs/scorers.qmd`

 * *Files 9% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         multiple_choice()
     ],
     scorer=match(),
     metrics=[custom_metric()]
 )
 ```
 
-### Model Graded
+## Model Graded
 
 Model graded scorers are well suited to assessing open ended answers as well as factual answers that are embedded in a longer narrative. The built-in model graded scorers can be customised in several ways—you can also create entirely new model scorers (see the model graded example below for a starting point).
 
 Here is the declaration for the `model_graded_qa()` function:
 
 ``` python
 @scorer(metrics=[accuracy(), bootstrap_std()])
@@ -83,15 +83,33 @@
 1.  Provide alternate `instructions`—the default instructions ass the model to use chain of thought reasoning and provide grades in the format `GRADE: C` or `GRADE: I`. Note that if you provide instructions that ask the model to format grades in a different way, you will also want to customise the `grade_pattern`.
 2.  Specify `partial_credit = True` to prompt the model to assign partial credit to answers that are not entirely right but come close (metrics by default convert this to a value of 0.5). Note that this parameter is only valid when using the default `instructions`.
 3.  Specify an alternate `model` to perform the grading (e.g. a more powerful model or a model fine tuned for grading).
 4.  Specify a different `template`—note that templates are passed these variables: `question`, `criterion`, `answer`, and `instructions.`
 
 The `model_graded_fact()` scorer works identically to `model_graded_qa()`, and simply provides an alternate `template` oriented around judging whether a fact is included in the model output.
 
-If you want to understand how the default templates for `model_graded_qa()` and `model_graded_fact()` work, see their [source code](https://github.com/AI-Safety-Institute/inspect_ai/blob/main/src/inspect_ai/scorer/_model.py).
+If you want to understand how the default templates for `model_graded_qa()` and `model_graded_fact()` work, see their [source code](https://github.com/UKGovernmentBEIS/inspect_ai/blob/main/src/inspect_ai/scorer/_model.py).
+
+### Multiple Models
+
+The built-in model graded scorers also support using multiple grader models (whereby the final grade is chosen by majority vote). For example, here we specify that 3 models should be used for grading:
+
+```python
+model_graded_qa(
+    models = [
+        "google/gemini-1.0-pro",
+        "anthropic/claude-3-opus-20240229" 
+        "together/meta-llama/Llama-3-70b-chat-hf",
+    ]
+)
+```
+
+The implementation of multiple grader models takes advantage of the `multi_scorer()` and `majority_vote()` functions, both of which can be used in your own scorers (as described in the [Multi Scorer](#sec-multi-scorer) section below).
+
+
 
 ## Custom Scorers
 
 Custom scorers are functions that take a `TaskState` and `Target`, and yield a `Score`.
 
 ``` python
 async def score(state: TaskState, target: Target):
@@ -233,15 +251,52 @@
             )
 
     return score
 ```
 
 Note that the call to `model_grader.generate()` is done with `await`—this is critical to ensure that the scorer participates correctly in the scheduling of generation work.
 
-Note also e use the `input_text` property of the `TaskState` to access a string version of the original user input to substitute it into the grading template. Using the `input_text` has two benefits: (1) It is guaranteed to cover the original input from the dataset (rather than a transformed prompt in `messages`); and (2) It normalises the input to a string (as it could have been a message list).
+Note also we use the `input_text` property of the `TaskState` to access a string version of the original user input to substitute it into the grading template. Using the `input_text` has two benefits: (1) It is guaranteed to cover the original input from the dataset (rather than a transformed prompt in `messages`); and (2) It normalises the input to a string (as it could have been a message list).
+
+## Multi Scorer
+
+It's possible to use multiple scorers in parallel, then combine their output into a final overall score. This is done using the `multi_scorer()` function. For example, this is roughly how the built in model graders use multiple models for grading:
+
+```python
+multi_scorer(
+    scorers = [model_graded_qa(model=model) for model in models],
+    reducer = majority_vote
+)
+```
+
+Use of `multi_scorer()` requires both a list of scorers as well as a _reducer_ which is a function that takes a list of scores and turns it into a single score. In this case we use the built in `majority_vote()` reducer which returns the score that appeared most frequently in the answers.
+
+You can imagine a variety of different strategies for reducing scores (take the average, take the high or low, majority vote, etc.). For example, here's a reducer that computes the average score:
+
+```python
+import numpy as np
+
+def average_score(scores: list[Score]) -> Score:
+    values = [score.as_float() for score in scores]
+    avg = np.mean(values).item()
+    return Score(
+        value=avg,
+        explanation=f"average of {', '.join(values)}"
+    )
+```
+
+Which might be used like this:
+
+```python
+multi_scorer(
+    scorers = [model_graded_qa(model=model) for model in models],
+    reducer = average_score
+)
+```
+
 
 ## Metrics
 
 Each scorer provides one or more built-in metrics (typically `accuracy` and `bootstrap_std`). In addition, you can specify other metrics (either built-in or custom) to compute when defining a `Task`:
 
 ``` python
 Task(
```

### Comparing `inspect_ai-0.3.8/docs/solvers.qmd` & `inspect_ai-0.3.9/docs/solvers.qmd`

 * *Files 1% similar despite different names*

```diff
@@ -27,36 +27,36 @@
         scorer=model_graded_fact(),
     )
 ```
 
 Typically, a call to `generate()` is included in the list of solvers (this solver is just a simple call to the model). You can also create a more sophisticated solver that calls `generate()` internally, perhaps even more than once (this is often required for more complex evaluations). Next, we'll describe how solvers operate on *task states* to do their work.
 
 ::: {.callout-note appearance="simple"}
-The concept of using solvers and task states for evals was originally introduced in [Open AI Evals](https://github.com/openai/evals/blob/main/evals/solvers/README.md). Inspect solvers are an evolution of this core design.
+The concept of using solvers and task states for evals was originally introduced in [OpenAI Evals](https://github.com/openai/evals/blob/main/evals/solvers/README.md). Inspect solvers are an evolution of this core design.
 :::
 
 ## Task States
 
 Before we get into the specifics of how solvers work, we should describe `TaskState`, which is the fundamental data structure they act upon. A `TaskState` consists principally of chat history (derived from `input` and then extended by model interactions) and model output:
 
 ``` python
 class TaskState:
     messages: list[ChatMessage],
     output: ModelOutput
 ```
 
 ::: {.callout-note appearance="simple"}
-Note that the above is a bit of simplification, there are other fields in a `TaskState` but we're excluding them here for clarity.
+Note that the `TaskState` definition above is simplified: there are other fields in a `TaskState` but we're excluding them here for clarity.
 :::
 
 A prompt engineering solver will modify the content of `messages`. A model generation solver will call the model, append an assistant `message`, and set the `output` (a multi-turn dialog solver might do this in a loop).
 
 ## Solver Function
 
-We've covered the role of solvers in the system, but what exactly are solvers technically? A solver is a Python function that tasks a `TaskState` and `generate` function, and then transforms and returns the `TaskState` (the `generate` function may or may not be called depending on the solver).
+We've covered the role of solvers in the system, but what exactly are solvers technically? A solver is a Python function that takes a `TaskState` and `generate` function, and then transforms and returns the `TaskState` (the `generate` function may or may not be called depending on the solver).
 
 ``` python
 async def solve(state: TaskState, generate: Generate):
     # do something useful with state (possibly 
     # calling generate for more advanced solvers)
     # then return the state
     return state
@@ -75,15 +75,15 @@
     ``` python
     async def solve(state: TaskState, generate: Generate):
         return await generate(state)
     ```
 
 4.  The `self_critique()` solver takes the `ModelOutput` and then sends it to another model for critique. It then replays this critique back within the `messages` stream and re-calls `generate` to get a refined answer.
 
-You can also imagine solvers that call other models to help come up with a better prompt, or solvers the implement a multi-turn dialog. Anything you can imagine is possible.
+You can also imagine solvers that call other models to help come up with a better prompt, or solvers that implement a multi-turn dialog. Anything you can imagine is possible.
 
 ## Built-In Solvers
 
 Inspect has a number of built-in solvers, each of which can be customised in some fashion. Built in solvers can be imported from the `inspect_ai.solver` module. Below is a summary of these solvers. There is not (yet) reference documentation on these functions so the best way to learn about how they can be customised, etc. is to use the **Go to Definition** command in your source editor.
 
 -   `system_message()`
 
@@ -312,15 +312,15 @@
 )
 ```
 
 In this example the `finish_up()` solver will always be called even if the plan doesn't run all of its steps.
 
 ## Plan Cleanup
 
-If your solvers allocate resources (for example, run a Docker container or mount a drive), you will want to make sure that these resources are cleaned up even in the case of an error occurring during the evaluaton. To arrange for this, use a `Plan` object with a `cleanup` function:
+If your solvers allocate resources (for example, run a Docker container or mount a drive), you will want to make sure that these resources are cleaned up even in the case of an error occurring during the evaluation. To arrange for this, use a `Plan` object with a `cleanup` function:
 
 ```python
 
 async def cleanup(state):
     # cleanup resources
     ...
```

### Comparing `inspect_ai-0.3.8/docs/theme.scss` & `inspect_ai-0.3.9/docs/theme.scss`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/docs/tools.qmd` & `inspect_ai-0.3.9/docs/tools.qmd`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Many models now have the ability to interact with client-side Python functions in order to expand their capabilities. This enables you to equip models with your own set of custom tools so they can perform a wider variety of tasks.
 
 Inspect natively supports registering Python functions as tools and providing these tools to models that support them (currently OpenAI, Claude 3, Google Gemini, and Mistral). Inspect also includes one built-in tool (web search).
 
 ::: {.callout-note}
 ### Tools and Agents
 
-One application of tools is to run them within an agent scaffold that pursues an objective over multiple interactions with a model. The scaffold uses the model to help make decisions about which tools to use and when, and orchestrates calls to the model to use the tools. We'll cover how to use agent scaffolds in [Agent Solvers](#agents) below.
+One application of tools is to run them within an agent scaffold that pursues an objective over multiple interactions with a model. The scaffold uses the model to help make decisions about which tools to use and when, and orchestrates calls to the model to use the tools. We'll cover how to use agent scaffolds in [Agent Solvers](#agent-solvers) below.
 :::
 
 ## Tool Basics
 
 To demonstrate the use of tools, we'll define a simple tool that adds two numbers. We use the `@tool` decorator to register it with the system, and we provide a documentation comment (including argument types) that is used to provide details to the model about the tool:
 
 ``` python
@@ -118,15 +118,15 @@
         ],
         scorer=includes(),
     )
 ```
 
 ## Tool Choice
 
-By default models will use a tool if they think it's appropriate for the given task. You can override this behavior using the `tool_choice` parmaeter of the `use_tools()` Solver. For example:
+By default models will use a tool if they think it's appropriate for the given task. You can override this behavior using the `tool_choice` parameter of the `use_tools()` Solver. For example:
 
 ``` python
 # let the model decide whether to use the tool
 use_tools(addition(), tool_choice="auto")
 
 # force the use of a tool
 use_tools(addition(), tool_choice=ToolFunction(name="addition"))
@@ -145,15 +145,15 @@
   use_tools(tool_choice="none"),
   generate()
 ]
 ```
 
 ## Web Search
 
-Inspect has a built in `web_search()` tool that provides models with the ability to enhance their context window by performing a search. By default web searches retreives 10 results from a provider, uses a model to determine if the contents is relevant then returns the top 3 relevant search results to the main model. Here is the definition of the `web_search()` function:
+Inspect has a built in `web_search()` tool that provides models with the ability to enhance their context window by performing a search. By default web searches retrieve 10 results from a provider, uses a model to determine if the contents is relevant then returns the top 3 relevant search results to the main model. Here is the definition of the `web_search()` function:
 
 ``` python
 def web_search(
     provider: Literal["google"] = "google",
     num_results: int = 3,
     max_provider_calls: int = 3,
     max_connections: int = 10,
@@ -173,15 +173,15 @@
 
 Web search options include:
 
 -   `provider`---Web search provider (currently only Google is supported, see below for instructions on setup and configuration for Google).
 
 -   `num_results`---How many search results to return to the main model (defaults to 5).
 
--   `max_provider_calls`---Number of times to retrieve more links from the search provider incase previous ones were irrelevant (defaults to 3)
+-   `max_provider_calls`---Number of times to retrieve more links from the search provider in case previous ones were irrelevant (defaults to 3).
 
 -   `max_connections`---Maximum number of concurrent connections to the search API provider (defaults to 10).
 
 -   `model`---Model to use to determine if search results are relevant (defaults to the model currently being evaluated).
 
 ### Google Provider
 
@@ -201,15 +201,15 @@
 
 1.  Implement your own scaffolding (potentially implementing the ReAct algorithm or a derivative). This will involve repeated calls to `generate()` with various `tools` being made available in the `TaskState` for each call. It will also involve using the model to help determine what actions to take next.
 
 2.  Adapt another scaffolding scheme provided by a research paper or open source library.
 
 3.  Integrate a 3rd party agent library like [LangChain](https://python.langchain.com/docs/modules/agents/) and [Langroid](https://langroid.github.io/langroid/).
 
-If you are adapting research code or using a 3rd party library, it's important that the agent scaffolding use Inspect's model API rather than whatever interface is built in to the existing code or library (otherwise you might be evaluating the wrong model!). We'll describe how to do that for [LangChain](https://python.langchain.com/docs/modules/agents/) in the example below.
+If you are adapting research code or using a 3rd party library, it's important that the agent scaffolding use Inspect's model API rather than whatever interface is built in to the existing code or library (otherwise you might be evaluating the wrong model!) We'll describe how to do that for [LangChain](https://python.langchain.com/docs/modules/agents/) in the example below.
 
 ### Example: Wikipedia Search
 
 In this example we'll demonstrate how to integrate a LangChain OpenAI tools agent with Inspect. This agent will use Wikipedia via the [Tavili Search API](https://tavily.com/) to perform question answering tasks. If you want to start by getting some grounding in the code *without* the Inspect integration, see [this article](https://brightinventions.pl/blog/introducing-langchain-agents-tutorial-with-example/) upon which the example is based.
 
 The main thing that an integration with an agent framework needs to account for is:
```

### Comparing `inspect_ai-0.3.8/docs/workflow.qmd` & `inspect_ai-0.3.9/docs/workflow.qmd`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,21 @@
 
 ``` bash
 $ inspect eval theory.py --model openai/gpt-4
 ```
 
 ![](images/running-theory.png){fig-alt="The Inspect task results displayed in the terminal. A progress bar indicates that the evaluation is about 60% complete."}
 
-Immediately after an evaluation completes, a link to the log for the evaluation is written to the terminal (if you are running in VS Code this link will open the log in an editor within the IDE).
+Immediately after an evaluation completes, a link to the log for the evaluation is written to the terminal.
+
+::: {.callout-note title="VS Code Extension"}
+
+If you are using VS Code, we also recommend installing the VS Code Extension, which includes tools for running, tuning, debugging, and visualising evals. See the article on the [VS Code Extension](#sec-vscode) for more details on installing and using the extension.
+
+:::
 
 ### Models
 
 Run the evaluation against other models as follows:
 
 ``` bash
 $ inspect eval theory.py --model anthropic/claude-3-opus-20240229
@@ -63,15 +69,15 @@
 
 As you iterate on an evaluation, you'll typically want to dig further into message histories, scoring decisions, and other diagnostics. Typically at the outset of working session you'll run `inspect view` to open the Inspect [Log Viewer](#sec-log-viewer):
 
 ``` bash
 $ inspect view
 ```
 
-![](images/inspect-view-main.png){.border .lightbox fig-alt="The Inspect log viewer, displahing a summary of results for the task as well as 8 individual samples."}
+![](images/inspect-view-main.png){.border .lightbox fig-alt="The Inspect log viewer, displaying a summary of results for the task as well as 8 individual samples."}
 
 
 The log viewer will update automatically whenever a new evaluation is completed (you can also navigate back to previous evaluations). The log viewer summarises aggregate data and also provides a detailed view into each sample. For example, here we zoom in on the model's scoring explanation for a specific sample:
 
 ![](images/inspect-view-scoring.png){.border .lightbox fig-alt="The Inspect log viewer showing a sample expanded, with details on the scoring of the sample, including the input, target, answer, and explanation."}
 
 See the [Log Viewer](#sec-log-viewer) section for additional details on using Inspect View.
@@ -224,15 +230,15 @@
         security_guide(system=prompt)
         for prompt in ["devops.txt", "researcher.txt"]
     ]
     eval(tasks, model = "openai/gpt-4")
 ```
 
 ::: {.callout-note appearance="minimal"}
-If you aren't familliar with the `__name__ == "__main__"` idiom, see the docs on [\_\_main\_\_](https://docs.python.org/3/library/main.html) for additional details.
+If you aren't familiar with the `__name__ == "__main__"` idiom, see the docs on [\_\_main\_\_](https://docs.python.org/3/library/__main__.html) for additional details.
 :::
 
 Now we can take the same script and use it with `inspect eval` (while leaving our exploratory code intact and protected by the `__main__` check):
 
 ``` bash
 $ inspect eval security.py 
 ```
@@ -245,28 +251,28 @@
 
 ### Notebooks
 
 We refer to notebooks above but show scripts in all of the examples. Everything demonstrated for scripts will work similarly in notebooks, specifically:
 
 1.  You can use the `__name__ == "__main__"` check to protect cells that should only be run in exploratory mode.
 
-2.  You can pass a notebook to `insect eval` just the same as a script (including passing task parameters)
+2.  You can pass a notebook to `inspect eval` just the same as a script (including passing task parameters)
 
 For example, imagine that all of the code shown above for `security.py` was in `security.ipynb`. You could run the eval and optionally pass a task parameter as follows:
 
 ``` bash
 $ inspect eval security.ipynb 
 $ inspect eval security.ipynb -T system=devops.txt
 ```
 
-Once you've stabilized the definition of an eval, you might also prefer to keep exploratory code and eval task definitions entirely separate. In that case, keep your `@task` function in `security.py` and then just import it into one or more noteoboks used to try out variations, analyze logs, etc.
+Once you've stabilized the definition of an eval, you might also prefer to keep exploratory code and eval task definitions entirely separate. In that case, keep your `@task` function in `security.py` and then just import it into one or more notebooks used to try out variations, analyze logs, etc.
 
 ## Eval Suites
 
-The examples above either run a single evaluation task from a script or notebook, or perhaps run a dynamic set of tasks within an interactive session. While this is a good workflow for the development of evaluations, eventually you may want to compose a set of evalutions into a suite that you run repeadedly for different models.
+The examples above either run a single evaluation task from a script or notebook, or perhaps run a dynamic set of tasks within an interactive session. While this is a good workflow for the development of evaluations, eventually you may want to compose a set of evaluations into a suite that you run repeatedly for different models.
 
 For example, the left/right listing below shows a project with multiple Python scripts, some of which include eval tasks. At right, there is a call to `inspect list tasks` to enumerate all the tasks:
 
 ::: {layout-ncol="2"}
 ``` bash
 security/
   jeopardy/
```

### Comparing `inspect_ai-0.3.8/examples/agents/langchain/README.md` & `inspect_ai-0.3.9/examples/agents/langchain/README.md`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/examples/agents/langchain/inspect_langchain.py` & `inspect_ai-0.3.9/examples/agents/langchain/inspect_langchain.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/examples/agents/langchain/wikipedia.jsonl` & `inspect_ai-0.3.9/examples/agents/langchain/wikipedia.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/examples/agents/langchain/wikipedia.py` & `inspect_ai-0.3.9/examples/agents/langchain/wikipedia.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/examples/biology_qa.py` & `inspect_ai-0.3.9/examples/biology_qa.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/examples/popularity.py` & `inspect_ai-0.3.9/examples/popularity.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/examples/security_guide.py` & `inspect_ai-0.3.9/examples/security_guide.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/examples/theory_of_mind.py` & `inspect_ai-0.3.9/examples/theory_of_mind.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/examples/tool_use.py` & `inspect_ai-0.3.9/examples/tool_use.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/pyproject.toml` & `inspect_ai-0.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/__init__.py` & `inspect_ai-0.3.9/src/inspect_ai/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from importlib.metadata import version as importlib_version
 
 from inspect_ai._eval.eval import eval, eval_async, eval_retry, eval_retry_async
 from inspect_ai._eval.list import list_tasks
 from inspect_ai._eval.registry import task
 from inspect_ai._eval.score import score, score_async
-from inspect_ai._eval.task import Task, TaskInfo, Tasks
+from inspect_ai._eval.types import Task, TaskInfo, Tasks
 from inspect_ai._util.constants import PKG_NAME
 
 __version__ = importlib_version(PKG_NAME)
 
 
 __all__ = [
     "__version__",
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_cli/common.py` & `inspect_ai-0.3.9/src/inspect_ai/_cli/common.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_cli/eval.py` & `inspect_ai-0.3.9/src/inspect_ai/_cli/eval.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     "--system-message",
     type=str,
     help="Override the default system message.",
 )
 @click.option(
     "--best-of",
     type=int,
-    help="Generates best_of completions server-side and returns the 'best' (the one withthe highest log probability per token). OpenAI only.",
+    help="Generates best_of completions server-side and returns the 'best' (the one with the highest log probability per token). OpenAI only.",
 )
 @click.option(
     "--frequency-penalty",
     type=float,
     help="Number between -2.0 and 2.0. Positive values penalize new tokens based on their existing frequency in the text so far, decreasing the model's likelihood to repeat the same line verbatim. OpenAI only.",
 )
 @click.option(
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_cli/info.py` & `inspect_ai-0.3.9/src/inspect_ai/_cli/info.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_cli/list.py` & `inspect_ai-0.3.9/src/inspect_ai/_cli/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from fsspec.core import split_protocol  # type: ignore
 from pydantic_core import to_jsonable_python
 from typing_extensions import Unpack
 
 from inspect_ai._cli.common import CommonOptions, common_options, resolve_common_options
 from inspect_ai._cli.util import parse_cli_args
 from inspect_ai._eval.list import list_tasks
-from inspect_ai._eval.task import TaskInfo
+from inspect_ai._eval.types import TaskInfo
 from inspect_ai.log import list_eval_logs
 
 
 @click.group("list")
 def list_command() -> None:
     """List tasks or eval logs."""
     return None
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_cli/main.py` & `inspect_ai-0.3.9/src/inspect_ai/_cli/main.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_cli/score.py` & `inspect_ai-0.3.9/src/inspect_ai/_cli/score.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import click
 from typing_extensions import Unpack
 
 from inspect_ai._display import display
 from inspect_ai._display.logger import init_logger
 from inspect_ai._eval.loader import load_tasks
+from inspect_ai._eval.score import task_score
 from inspect_ai._util.constants import SCORED_SUFFIX
 from inspect_ai._util.dotenv import init_dotenv
 from inspect_ai.log._file import JSONRecorder
 from inspect_ai.model import get_model
 from inspect_ai.model._model import init_async_context_model
 from inspect_ai.util._context import init_async_context
 
@@ -72,15 +73,15 @@
     init_async_context()
     init_async_context_model(model)
 
     # instantiate the task so we can get its scorer and metrics
     score_task = load_tasks([task], model)[0]
 
     # re-score the task
-    eval_log = await score_task.score(eval_log)
+    eval_log = await task_score(score_task, eval_log)
 
     # re-write the log (w/ a -score suffix if requested)
     scored = f"{SCORED_SUFFIX}.json"
     if not overwrite and not log_file.endswith(scored):
         log_file = log_file.removesuffix(".json") + scored
     recorder.write_log(log_file, eval_log)
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_cli/util.py` & `inspect_ai-0.3.9/src/inspect_ai/_cli/util.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_cli/view.py` & `inspect_ai-0.3.9/src/inspect_ai/_cli/view.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_display/_display.py` & `inspect_ai-0.3.9/src/inspect_ai/_display/_display.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_display/logger.py` & `inspect_ai-0.3.9/src/inspect_ai/_display/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 class LogHandler(RichHandler):
     def __init__(self, levelno: int) -> None:
         super().__init__(levelno, console=rich_console())
         self.display_level = WARNING
 
     @override
     def emit(self, record: LogRecord) -> None:
-        # demote httpx and retury notifications to log_level http
+        # demote httpx and return notifications to log_level http
         if record.name == "httpx" or "Retrying request" in record.getMessage():
             record.levelno = HTTP
             record.levelname = HTTP_LOG_LEVEL
 
         # skip httpx event loop is closed errors
         if "Event loop is closed" in record.getMessage():
             return
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_display/rich.py` & `inspect_ai-0.3.9/src/inspect_ai/_display/rich.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,23 +215,23 @@
         Text(task_targets(profile), style=theme.meta),
     )
 
     # config
     if config:
         table.add_row(config)
 
-    # footer if sepecified
+    # footer if specified
     if footer:
         table.add_row()
         table.add_row(footer[0], footer[1])
 
     # enclose in outer table for log link footer
     root = table
     if log_location:
-        # if we are in jupyter then use a real hyperink
+        # if we are in jupyter then use a real hyperlink
         if options.jupyter:
             log_location = f"[link={log_location}]{log_location}[/link]"
 
         root = Table.grid(expand=True)
         root.add_column()
         root.add_row(table)
         root.add_row()
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_eval/eval.py` & `inspect_ai-0.3.9/src/inspect_ai/_eval/eval.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,18 @@
     get_model,
 )
 from inspect_ai.model._model import init_async_context_model
 from inspect_ai.solver import Solver
 from inspect_ai.util._context import init_async_context
 
 from .loader import resolve_tasks
-from .log import EvalLogger
-from .task import Tasks, TaskSpec, task_file, task_run_dir
+from .task.log import TaskLogger
+from .task.run import task_run
+from .task.util import task_file, task_run_dir
+from .types import Tasks, TaskSpec
 
 log = logging.getLogger(__name__)
 
 
 def eval(
     tasks: Tasks,
     model: str | Model | None = None,
@@ -126,42 +128,43 @@
     log_samples: bool | None = None,
     log_images: bool | None = None,
     score: bool = True,
     **kwargs: Unpack[GenerateConfigArgs],
 ) -> list[EvalLog]:
     r"""Evaluate tasks using a Model (async).
 
-    tasks: (Tasks): Task(s) to evaluate. If None, attempt
-        to evaluate a task in the current working directory
-    model (str | Model | None): Model for evaluation. If not
-        specified uses the current eval's model, or failing that
-        the value of the INSPECT_EVAL_MODEL environment variable.
-    model_base_url: (str | None): Base URL for communicating
-        with the model API.
-    model_args (dict[str,Any]): Model creation parameters
-    task_args (dict[str,Any]): Task arguments
-    plan (Solver | list[Solver] | None): Alternative plan
-        for evaluating task(s). Optional (uses task plan by default).
-    log_level (str | None): "debug", "http", "info", "warning", "error",
-        or "critical" (defaults to "info")
-    log_dir (str | None): Output path for logging results
-        (defaults to file log in ./logs directory).
-    limit (int | tuple[int, int] | None): Limit evaluated samples
-        (defaults to all samples).
-    epochs (int | None): Number of times to repeat evaluation of
-        samples (defaults to 1)
-    max_messages (int | None): Maximum number of messages to allow
-        in a task conversation.
-    max_subprocesses (int | None): Maximum number of subprocesses to
-        run in parallel (default is os.cpu_count())
-    log_samples: (bool | None): Log detailed samples and scores (defaults to True)
-    log_images: (bool | None): Log base64 encoded version of images,
-        even if specified as a filename or URL (defaults to True)
-    score (bool): Score output (defaults to True)
-    **kwargs (GenerateConfigArgs): Model generation options.
+    Args:
+        tasks: (Tasks): Task(s) to evaluate. If None, attempt
+            to evaluate a task in the current working directory
+        model (str | Model | None): Model for evaluation. If not
+            specified uses the current eval's model, or failing that
+            the value of the INSPECT_EVAL_MODEL environment variable.
+        model_base_url: (str | None): Base URL for communicating
+            with the model API.
+        model_args (dict[str,Any]): Model creation parameters
+        task_args (dict[str,Any]): Task arguments
+        plan (Solver | list[Solver] | None): Alternative plan
+            for evaluating task(s). Optional (uses task plan by default).
+        log_level (str | None): "debug", "http", "info", "warning", "error",
+            or "critical" (defaults to "info")
+        log_dir (str | None): Output path for logging results
+            (defaults to file log in ./logs directory).
+        limit (int | tuple[int, int] | None): Limit evaluated samples
+            (defaults to all samples).
+        epochs (int | None): Number of times to repeat evaluation of
+            samples (defaults to 1)
+        max_messages (int | None): Maximum number of messages to allow
+            in a task conversation.
+        max_subprocesses (int | None): Maximum number of subprocesses to
+            run in parallel (default is os.cpu_count())
+        log_samples: (bool | None): Log detailed samples and scores (defaults to True)
+        log_images: (bool | None): Log base64 encoded version of images,
+            even if specified as a filename or URL (defaults to True)
+        score (bool): Score output (defaults to True)
+        **kwargs (GenerateConfigArgs): Model generation options.
 
     Returns:
         List of EvalLog (one for each task)
     """
     # Provide .env and log support bootstrap for notebooks and invoking
     # an eval as a plain Python script (as opposed to via inspect eval)
     init_dotenv()
@@ -185,15 +188,15 @@
         tasks = tasks.task
     else:
         task_id = None
 
     # resolve tasks
     eval_tasks = resolve_tasks(tasks, model, task_args)
 
-    # warn and return empty string if we resovled no tasks
+    # warn and return empty string if we resolved no tasks
     if len(eval_tasks) == 0:
         log.warning("No inspect tasks were found at the specified paths.")
         return []
 
     # resolve recorder
     log_dir = log_dir if log_dir else os.environ.get("INSPECT_LOG_DIR", "./logs")
     log_dir = cwd_relative_path(log_dir)
@@ -210,46 +213,47 @@
         max_messages=max_messages,
         max_subprocesses=max_subprocesses,
         log_samples=log_samples,
         log_images=log_images,
     )
 
     run_id = uuid()
-    loggers: list[EvalLogger] = []
+    loggers: list[TaskLogger] = []
     results: list[EvalLog] = []
     for index, name, version, task in zip(
         range(0, len(task_names)), task_names, task_versions, eval_tasks
     ):
         # tasks can provide their own epochs and max_messages
         task_eval_config = eval_config.model_copy()
         if task.epochs is not None:
             task_eval_config.epochs = task.epochs
         if task.max_messages is not None:
             task_eval_config.max_messages = task.max_messages
 
         # create and track the logger
-        logger = EvalLogger(
+        logger = TaskLogger(
             task_name=name,
             task_version=version,
-            task_file=task_file(task, True),
+            task_file=task_file(task, relative=True),
             task_run_dir=task_run_dir(task),
             task_id=task_id if task_id else uuid(),
             run_id=run_id,
             model=model,
             dataset=task.dataset,
             task_attribs=task.attribs,
             task_args=task_args,
             model_args=model_args,
             eval_config=task_eval_config,
             recorder=recorder,
         )
         loggers.append(logger)
 
         # run the eval
-        result = await task.run(
+        result = await task_run(
+            task=task,
             sequence=(index + 1, len(task_names)),
             model=model,
             logger=logger,
             config=task_eval_config,
             plan=plan,
             score=score,
             **kwargs,
@@ -427,15 +431,15 @@
         # add it to our results
         eval_logs.append(log)
 
     return EvalLogs(eval_logs)
 
 
 # A list of eval logs is returned from eval(). We've already displayed
-# all of the ouptut we need to to though, so we make the return
+# all of the output we need to to though, so we make the return
 # value 'invisible'
 class EvalLogs(list[EvalLog]):
     def _ipython_display_(self) -> None:
         pass
 
     def __repr__(self) -> str:
         return ""
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_eval/images.py` & `inspect_ai-0.3.9/src/inspect_ai/_eval/task/images.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 import asyncio
 
 from inspect_ai._util.images import image_as_data_uri
 from inspect_ai.dataset import Sample
 from inspect_ai.model import ChatMessage, ChatMessageUser, Content, ContentImage
+from inspect_ai.solver import TaskState
+
+
+async def states_with_base64_images(states: list[TaskState]) -> list[TaskState]:
+    return await asyncio.gather(*[state_with_base64_images(state) for state in states])
+
+
+async def state_with_base64_images(state: TaskState) -> TaskState:
+    state.messages = await messages_with_base64_images(state.messages)
+    return state
 
 
 async def samples_with_base64_images(samples: list[Sample]) -> list[Sample]:
     return await asyncio.gather(
         *[sample_with_base64_images(sample) for sample in samples]
     )
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_eval/log.py` & `inspect_ai-0.3.9/src/inspect_ai/_eval/task/log.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,49 @@
 from importlib import metadata as importlib_metadata
+from logging import LogRecord
 from typing import Any
 
 from shortuuid import uuid
 
 from inspect_ai._util.constants import PKG_NAME
 from inspect_ai._util.datetime import iso_now
 from inspect_ai._util.git import git_context
 from inspect_ai._util.path import cwd_relative_path
+from inspect_ai._util.registry import (
+    registry_log_name,
+    registry_params,
+)
 from inspect_ai.dataset import Dataset, Sample
 from inspect_ai.log import (
     EvalConfig,
     EvalDataset,
     EvalError,
     EvalLog,
     EvalPlan,
+    EvalPlanStep,
     EvalResults,
     EvalRevision,
     EvalSample,
     EvalSpec,
     EvalStats,
     LoggingMessage,
 )
 from inspect_ai.log._log import LogEvent, Recorder
-from inspect_ai.model import Model, ModelName
+from inspect_ai.model import (
+    GenerateConfig,
+    Model,
+    ModelName,
+)
+from inspect_ai.model._model import collect_model_usage
 from inspect_ai.scorer import Score
-from inspect_ai.solver import TaskState
+from inspect_ai.solver import Plan, Solver, TaskState
+from inspect_ai.util._context.logger import collect_logger_records
 
 
-class EvalLogger:
+class TaskLogger:
     def __init__(
         self,
         task_name: str,
         task_version: int,
         task_file: str | None,
         task_run_dir: str,
         task_id: str | None,
@@ -119,7 +131,54 @@
         self.log_event("results", results)
 
     def log_success(self, stats: EvalStats) -> EvalLog:
         return self.recorder.log_success(self.eval, stats)
 
     def log_failure(self, stats: EvalStats, error: EvalError) -> EvalLog:
         return self.recorder.log_failure(self.eval, stats, error)
+
+
+def log_output(
+    logger: TaskLogger,
+    epoch: int,
+    samples: list[Sample],
+    states: list[TaskState],
+    scores: list[Score | None],
+) -> None:
+    for i in range(len(samples)):
+        logger.log_sample(epoch, samples[i], states[i], scores[i])
+
+
+def log_plan(
+    logger: TaskLogger,
+    plan: Plan,
+    config: GenerateConfig,
+) -> None:
+    def eval_plan_step(solver: Solver) -> EvalPlanStep:
+        return EvalPlanStep(
+            solver=registry_log_name(solver), params=registry_params(solver)
+        )
+
+    eval_plan = EvalPlan(
+        name=plan.name,
+        steps=[eval_plan_step(solver) for solver in plan.steps],
+        finish=eval_plan_step(plan.finish) if plan.finish else None,
+        config=config,
+    )
+    if plan.finish:
+        eval_plan.steps.append(eval_plan_step(plan.finish))
+
+    logger.log_event("plan", eval_plan)
+
+
+def collect_eval_data(stats: EvalStats, logger: TaskLogger) -> None:
+    # collect stats
+    stats.completed_at = iso_now()
+    stats.model_usage = collect_model_usage()
+
+    # collect log output
+    log_logger_records(logger, collect_logger_records())
+
+
+def log_logger_records(logger: TaskLogger, records: list[LogRecord]) -> None:
+    for record in records:
+        logger.log_event("logging", LoggingMessage.from_log_record(record))
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_eval/registry.py` & `inspect_ai-0.3.9/src/inspect_ai/_eval/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     registry_info,
     registry_lookup,
     registry_name,
     registry_tag,
 )
 from inspect_ai.model import ModelName
 
-from .task import Task
+from .types import Task
 
 MODEL_PARAM = "model"
 
 logger = logging.getLogger(__name__)
 
 
 TaskType = TypeVar("TaskType", bound=Callable[..., Task])
@@ -65,15 +65,15 @@
     """
     # bring in model arg (first deepcopy as we will mutate it)
     # add model to task_args
     kwargs = deepcopy(kwargs)
     kwargs[MODEL_PARAM] = model
 
     # match kwargs params to signature (warn if param not found)
-    # (note that we always pass the 'model' param but tasks arne't
+    # (note that we always pass the 'model' param but tasks aren't
     # required to consume it, so we don't warn for 'model')
     task = registry_lookup("task", name)
     task_info = registry_info(task)
     task_params: list[str] = task_info.metadata["params"]
     task_args: dict[str, Any] = {}
     for param in kwargs.keys():
         if param in task_params:
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_util/dotenv.py` & `inspect_ai-0.3.9/src/inspect_ai/_util/dotenv.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_util/error.py` & `inspect_ai-0.3.9/src/inspect_ai/_util/error.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_util/file.py` & `inspect_ai-0.3.9/src/inspect_ai/_util/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,15 @@
 
 def filesystem(path: str, fs_options: dict[str, Any] = {}) -> FileSystem:
     """Return the filesystem used to host the specified path.
 
     Args:
       path (str): Local path or remote URL e.g. s3://).  The
         `fsspec` package is used to resolve filesystem URLs.
-      fs_options (dict[str, Any]): Optional. Addional arguments to pass through
+      fs_options (dict[str, Any]): Optional. Additional arguments to pass through
         to the filesystem provider (e.g. `S3FileSystem`). Use `{"anon": True }`
         if you are accessing a public S3 bucket with no credentials.
 
     Returns:
        An tuple with an `fsspec` compatible filesystem and the
        file-systems-specific URL for file.
     """
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_util/git.py` & `inspect_ai-0.3.9/src/inspect_ai/_util/git.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_util/http.py` & `inspect_ai-0.3.9/src/inspect_ai/_util/http.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_util/images.py` & `inspect_ai-0.3.9/src/inspect_ai/_util/images.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_util/json.py` & `inspect_ai-0.3.9/src/inspect_ai/_util/json.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
             return "boolean"
         case "list":
             return "array"
         case "dict":
             return "object"
         case "None":
             return "null"
-        # treat 'unknown' as string as anyting can be converted to string
+        # treat 'unknown' as string as anything can be converted to string
         case None:
             return "string"
         case _:
             raise ValueError(
                 f"Unsupported type: {python_type} for Python to JSON conversion."
             )
 
@@ -44,9 +44,9 @@
             return "list"
         case "object":
             return "dict"
         case "null":
             return "None"
         case _:
             raise ValueError(
-                f"Unsupported type: {json_type} for JSON to Python converstion."
+                f"Unsupported type: {json_type} for JSON to Python conversion."
             )
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_util/notebook.py` & `inspect_ai-0.3.9/src/inspect_ai/_util/notebook.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_util/path.py` & `inspect_ai-0.3.9/src/inspect_ai/_util/path.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_util/platform.py` & `inspect_ai-0.3.9/src/inspect_ai/_util/platform.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_util/registry.py` & `inspect_ai-0.3.9/src/inspect_ai/_util/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     metadata: dict[str, Any] = Field(default={})
 
 
 def registry_add(o: object, info: RegistryInfo) -> None:
     r"""Add an object to the registry.
 
     Add the passed object to the registry using the RegistryInfo
-    to index it for retreival. The RegistryInfo is also added
-    to the object as an attribute, which can retrevied by calling
+    to index it for retrieval. The RegistryInfo is also added
+    to the object as an attribute, which can retrieved by calling
     registry_info() on an object instance.
 
     Args:
         o (object): Object to be registered (Metric, Solver, etc.)
         info (RegistryInfo): Metadata (name, etc.) for object.
     """
     # tag the object
@@ -51,15 +51,15 @@
     **kwargs: dict[str, Any],
 ) -> None:
     r"""Tag an object w/ registry info.
 
     Tag the passed object with RegistryInfo. This function DOES NOT
     add the object to the registry (call registry_add() to both
     tag and add an object to the registry). Call registry_info()
-    on a tagged/registered object to retreive its info
+    on a tagged/registered object to retrieve its info
 
     Args:
         type (T): type of object being tagged
         o (object): Object to be registered (Metric, Solver, etc.)
         info (RegistryInfo): Metadata (name, etc.) for object.
         *args (list[Any]): Creation arguments
         **kwargs (dict[str,Any]): Creation keyword arguments
@@ -85,16 +85,16 @@
     setattr(o, REGISTRY_INFO, info)
     setattr(o, REGISTRY_PARAMS, named_params)
 
 
 def registry_name(o: object, name: str) -> str:
     r"""Compute the registry name of an object.
 
-    This function checks whether the passsed object is in a package,
-    and if it is, preprends the package name as a namespace
+    This function checks whether the passed object is in a package,
+    and if it is, prepends the package name as a namespace
     """
     package = get_package_name(o)
     return f"{package}/{name}" if package else name
 
 
 def registry_lookup(type: RegistryType, name: str) -> object | None:
     r"""Lookup an object in the registry by type and name.
@@ -213,21 +213,21 @@
         Name of object for logging.
     """
     name = registry_info(o).name
     return name.replace(f"{PKG_NAME}/", "", 1)
 
 
 def registry_unqualified_name(o: object) -> str:
-    r"""Unqualfied name of object (i.e. without package prefix).
+    r"""Unqualified name of object (i.e. without package prefix).
 
     Args:
-        o (object): Object to get unqualfied name for
+        o (object): Object to get unqualified name for
 
     Returns:
-        Unqualfieid name of object
+        Unqualified name of object
     """
     parts = registry_info(o).name.split("/")
     if len(parts) == 1:
         return parts[0]
     else:
         return "/".join(parts[1:])
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_util/retry.py` & `inspect_ai-0.3.9/src/inspect_ai/_util/retry.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_util/url.py` & `inspect_ai-0.3.9/src/inspect_ai/_util/url.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/schema.py` & `inspect_ai-0.3.9/src/inspect_ai/_view/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from inspect_ai.log import EvalLog
 
 WWW_DIR = os.path.abspath((Path(__file__).parent / "www").as_posix())
 
 
 def sync_view_schema() -> None:
-    """Genreate a JSON schema and Typescript types for EvalLog.
+    """Generate a JSON schema and Typescript types for EvalLog.
 
     This is useful for keeping log file viewer JS development
     in sync w/ Python development
     """
     # export schema file
     schema_path = Path(WWW_DIR, "log-schema.json")
     types_path = Path(WWW_DIR, "log.d.ts")
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/view.py` & `inspect_ai-0.3.9/src/inspect_ai/_view/view.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     port: int = DEFAULT_VIEW_PORT,
     log_level: str | None = None,
     fs_options: dict[str, Any] = {},
 ) -> None:
     init_dotenv()
     init_logger(log_level)
 
-    # intialize the right filesytem for this log_dir
+    # initialize the right filesystem for this log_dir
     log_dir = log_dir if log_dir else os.getenv("INSPECT_LOG_DIR", "./logs")
     fs = filesystem(log_dir, fs_options)
 
     # list the logs and confirm that there are logs to view (this also ensures
     # that the right e.g. S3 credentials are present before we run the server)
     files = list_eval_logs(log_dir, recursive=recursive, fs_options=fs_options)
     if len(files) == 0:
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/App.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/App.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/favicon.svg` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/favicon.svg`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/index.html` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/index.html`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap-icons.min.css` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap-icons.min.css`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap.min.css` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff2` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/bootstrap/js/bootstrap.bundle.min.js` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/libs/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/clipboard.min.js` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/libs/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/json5.min.js` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/libs/json5.min.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/prism/prism-dark.css` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/libs/prism/prism-dark.css`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/prism/prism.min.css` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/libs/prism/prism.min.css`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/prism/prism.min.js` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/libs/prism/prism.min.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/purify.min.js` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/libs/purify.min.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/libs/showdown.min.js` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/libs/showdown.min.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/log-schema.json` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/log-schema.json`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/log.d.ts` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/log.d.ts`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/preact/hooks.js` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/preact/hooks.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/preact/htm/htm.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/preact/htm/htm.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/preact/preact.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/preact/preact.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/App.css` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/App.css`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,14 @@
   --bs-secondary-color: var(--vscode-foreground);
   --bs-list-group-active-bg: var(--vscode-sideBarSectionHeader-background);
   --bs-list-group-active-border-color: var(--vscode-sideBarSectionHeader-background);
   --bs-list-group-action-active-bg: var(--vscode-sideBarSectionHeader-background);
   --bs-list-group-active-color: var(--vscode-sideBarSectionHeader-foreground);
 }
 
-
 :root {
   --bs-navbar-padding-y: 0;
   --bs-navbar-brand-padding-y: 0;
   --navbar-height: 40px;
   --sidebar-width: 500px;
 }
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/Constants.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/Constants.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/api/api-browser.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/api/api-browser.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/api/api-vscode.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/api/api-vscode.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/api/jsonrpc.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/api/jsonrpc.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/AnsiDisplay.css` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/components/AnsiDisplay.css`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/AnsiDisplay.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/components/AnsiDisplay.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/AppErrorBoundary.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/components/AppErrorBoundary.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/Card.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/components/Card.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/ChatView.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/components/ChatView.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/CopyButton.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/components/CopyButton.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/Dialog.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/components/Dialog.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/ErrorPanel.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/components/ErrorPanel.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/LabeledValue.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/components/LabeledValue.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/LoadingScreen.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/components/LoadingScreen.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/MarkdownDiv.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/components/MarkdownDiv.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/MessageContent.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/components/MessageContent.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/MetaDataView.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/components/MetaDataView.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/RenderedContent.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/components/RenderedContent.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/TabSet.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/components/TabSet.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/components/ansi-output.js` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/components/ansi-output.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/log-reader/Log-Reader.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/log-reader/Log-Reader.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/log-reader/Open-AI-Log-Reader.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/log-reader/Open-AI-Log-Reader.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/logging/LoggingPanel.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/logging/LoggingPanel.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/plan/PlanCard.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/plan/PlanCard.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/samples/SampleScoreView.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/samples/SampleScoreView.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/samples/SampleView.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/samples/SampleView.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/samples/SamplesCard.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/samples/SamplesCard.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/title/TitleBlock.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/title/TitleBlock.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/usage/ModelTokenTable.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/usage/ModelTokenTable.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/usage/UsageCard.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/usage/UsageCard.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/utils/Format.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/utils/Format.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/workspace/EpochFilter.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/workspace/EpochFilter.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/workspace/SampleFilter.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/workspace/SampleFilter.mjs`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
       return undefined;
     }
   }
 };
 
 const SelectFilter = ({ options, filterFn }) => {
   return html`
-    <div style=${{ display: "flex", marginRight: "0.5rem" }}>
+    <div style=${{ display: "flex" }}>
       <span
         class="sample-label"
         style=${{ alignSelf: "center", marginRight: "0.5em" }}
         >Scores:</span
       >
       <select
         class="form-select form-select-sm"
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/workspace/SamplesDescriptor.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/workspace/SamplesDescriptor.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/workspace/SortFilter.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/workspace/SortFilter.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/workspace/TaskErrorPanel.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/workspace/TaskErrorPanel.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/_view/www/src/workspace/WorkSpace.mjs` & `inspect_ai-0.3.9/src/inspect_ai/_view/www/src/workspace/WorkSpace.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/dataset/__init__.py` & `inspect_ai-0.3.9/src/inspect_ai/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/dataset/_dataset.py` & `inspect_ai-0.3.9/src/inspect_ai/dataset/_dataset.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/dataset/_examples/bias_detection.jsonl` & `inspect_ai-0.3.9/src/inspect_ai/dataset/_examples/bias_detection.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/dataset/_examples/biology_qa.jsonl` & `inspect_ai-0.3.9/src/inspect_ai/dataset/_examples/biology_qa.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/dataset/_examples/popularity.jsonl` & `inspect_ai-0.3.9/src/inspect_ai/dataset/_examples/popularity.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/dataset/_examples/security_guide.jsonl` & `inspect_ai-0.3.9/src/inspect_ai/dataset/_examples/security_guide.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/dataset/_examples/theory_of_mind.jsonl` & `inspect_ai-0.3.9/src/inspect_ai/dataset/_examples/theory_of_mind.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/dataset/_sources/csv.py` & `inspect_ai-0.3.9/src/inspect_ai/dataset/_sources/csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         shuffle (bool): Randomly shuffle the dataset order.
         seed: (int | None): Seed used for random shuffle.
         limit (int | None): Limit the number of records to read.
         dialect (str): CSV dialect ("unix" or "excel", defaults to "unix").
         encoding (str): Text encoding for file (defaults to "utf-8").
         name (str): Optional name for dataset (for logging). If not specified,
             defaults to the stem of the filename
-        fs_options (dict[str, Any]): Optional. Addional arguments to pass through
+        fs_options (dict[str, Any]): Optional. Additional arguments to pass through
             to the filesystem provider (e.g. `S3FileSystem`). Use `{"anon": True }`
             if you are accessing a public S3 bucket with no credentials.
 
     Returns:
         Dataset read from CSV file.
     """
     # resolve data_to_sample function
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/dataset/_sources/example.py` & `inspect_ai-0.3.9/src/inspect_ai/dataset/_sources/example.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/dataset/_sources/file.py` & `inspect_ai-0.3.9/src/inspect_ai/dataset/_sources/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             `SampleFieldSpec` to specify mapping fields by name; Pass a `RecordToSample` to
             handle mapping with a custom function.
         dialect (str): CSV dialect ("unix" or "excel", defaults to "unix"). Only
             applies to reading CSV files.
         encoding (str): Text encoding for file (defaults to "utf-8").
         name (str): Optional name for dataset (for logging). If not specified,
             defaults to the stem of the filename
-        fs_options (dict[str, Any]): Optional. Addional arguments to pass through
+        fs_options (dict[str, Any]): Optional. Additional arguments to pass through
             to the filesystem provider (e.g. `S3FileSystem`). Use `{"anon": True }`
             if you are accessing a public S3 bucket with no credentials.
 
     Returns:
         Dataset read from JSON or CSV file.
     """
     ext = os.path.splitext(file)[1].lower()
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/dataset/_sources/hf.py` & `inspect_ai-0.3.9/src/inspect_ai/dataset/_sources/hf.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/dataset/_sources/json.py` & `inspect_ai-0.3.9/src/inspect_ai/dataset/_sources/json.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         handle mapping with a custom function.
       shuffle (bool): Randomly shuffle the dataset order.
       seed: (int | None): Seed used for random shuffle.
       limit (int | None): Limit the number of records to read.
       encoding (str): Text encoding for file (defaults to "utf-8").
       name (str): Optional name for dataset (for logging). If not specified,
         defaults to the stem of the filename.
-      fs_options (dict[str, Any]): Optional. Addional arguments to pass through
+      fs_options (dict[str, Any]): Optional. Additional arguments to pass through
         to the filesystem provider (e.g. `S3FileSystem`). Use `{"anon": True }`
         if you are accessing a public S3 bucket with no credentials.
 
     Returns:
         Dataset read from JSON file.
     """
     # resolve data_to_sample function
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/dataset/_util.py` & `inspect_ai-0.3.9/src/inspect_ai/dataset/_util.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/log/__init__.py` & `inspect_ai-0.3.9/src/inspect_ai/log/__init__.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/log/_file.py` & `inspect_ai-0.3.9/src/inspect_ai/log/_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-import json
 import os
 import re
 from pathlib import Path
 from typing import Any, Callable, cast
 from urllib.parse import urlparse
 
 import json_stream  # type: ignore
 from pydantic import BaseModel, Field
-from pydantic_core import to_json
+from pydantic_core import from_json, to_json
 
 from inspect_ai._util.file import FileInfo, file, filesystem
 
 from ._log import (
     EvalError,
     EvalLog,
     EvalPlan,
@@ -50,16 +49,16 @@
       log_dir (str): Log directory (defaults to INSPECT_LOG_DIR)
       filter (Callable[[EvalLog], bool]): Filter to limit logs returned.
          Note that the EvalLog instance passed to the filter has only
          the EvalLog header (i.e. does not have the samples or logging output).
       recursive (bool): List log files recursively (defaults to True).
 
       extensions (list[str]): File extension to scan for logs
-      descending (bool): List in descening order.
-      fs_options (dict[str, Any]): Optional. Addional arguments to pass through
+      descending (bool): List in descending order.
+      fs_options (dict[str, Any]): Optional. Additional arguments to pass through
           to the filesystem provider (e.g. `S3FileSystem`).
 
     Returns:
        List of EvalLog Info.
 
     """
     # get the eval logs
@@ -112,46 +111,77 @@
        log_file (str | FileInfo): Log file to read.
        header_only (bool): Read only the header (i.e. exclude
          the "samples" and "logging" fields). Defaults to False.
 
     Returns:
        EvalLog object read from file.
     """
+    # resolve to file path
     log_file = log_file if isinstance(log_file, str) else log_file.name
-    with file(log_file, "r") as f:
-        # header-only uses json-stream
-        if header_only:
-            data = json_stream.load(f, persistent=True)
 
-            def read_field(field: str) -> Any:
-                if field in data.keys():
-                    return json_stream.to_standard_types(data[field])
+    # verify we know about this version of the log file format
+    def validate_version(ver: int) -> None:
+        if ver > 1:
+            raise ValueError(f"Unable to read version {ver} of log format.")
+
+    # header-only uses json-stream
+    if header_only:
+        with file(log_file, "r") as f:
+            try:
+                data = json_stream.load(f, persistent=True)
+
+                def read_field(field: str) -> Any:
+                    if field in data.keys():
+                        return json_stream.to_standard_types(data[field])
+                    else:
+                        return None
+
+                # fail for unknown version
+                version = read_field("version")
+                validate_version(version)
+
+                results = read_field("results")
+                error = read_field("error")
+
+                return EvalLog(
+                    version=version,
+                    status=read_field("status"),
+                    eval=EvalSpec(**read_field("eval")),
+                    plan=EvalPlan(**read_field("plan")),
+                    results=EvalResults(**results) if results else None,
+                    stats=EvalStats(**read_field("stats")),
+                    error=EvalError(**error) if error else None,
+                )
+            # The Python JSON serializer supports NaN and Inf, however
+            # this isn't technically part of the JSON spec. The json-stream
+            # library shares this limitation, so if we fail with an
+            # invalid character then we move on and and parse w/ pydantic
+            # (which does support NaN and Inf by default)
+            except ValueError as ex:
+                if str(ex).find("Invalid JSON character") != -1:
+                    pass
                 else:
-                    return None
+                    raise ex
+
+    # parse full log (also used as a fallback for header_only encountering NaN or Inf)
+    with file(log_file, "r") as f:
+        # parse w/ pydantic
+        raw_data = from_json(f.read())
+        log = EvalLog(**raw_data)
+
+        # fail for unknown version
+        validate_version(log.version)
 
-            results = read_field("results")
-            error = read_field("error")
+        # prune if header_only
+        if header_only:
+            log.samples = None
+            log.logging.clear()
 
-            return EvalLog(
-                version=read_field("version"),
-                status=read_field("status"),
-                eval=EvalSpec(**read_field("eval")),
-                plan=EvalPlan(**read_field("plan")),
-                results=EvalResults(**results) if results else None,
-                stats=EvalStats(**read_field("stats")),
-                error=EvalError(**error) if error else None,
-            )
-
-        # otherwise normal json parse
-        else:
-            raw_data = json.load(f)
-            log = EvalLog(**raw_data)
-            if log.version > 1:
-                raise ValueError(f"Unable to read version {log.version} of log format.")
-            return log
+        # return log
+        return log
 
 
 def read_eval_log_headers(log_files: list[str] | list[FileInfo]) -> list[EvalLog]:
     return [read_eval_log(log_file, header_only=True) for log_file in log_files]
 
 
 class FileRecorder(Recorder):
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/log/_log.py` & `inspect_ai-0.3.9/src/inspect_ai/log/_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
     task_file: str | None = Field(default=None)
     """Task source file."""
 
     task_id: str = Field(default="")
     """Unique task id."""
 
     run_id: str = Field(default="")
-    """Unqiue run id"""
+    """Unique run id"""
 
     created: str
     """Time created."""
 
     dataset: EvalDataset
     """Dataset used for eval."""
 
@@ -178,15 +178,15 @@
     model_base_url: str | None = Field(default=None)
     """Optional override of model base url"""
 
     task_attribs: dict[str, Any] = Field(default={})
     """Attributes of the @task decorator."""
 
     task_args: dict[str, Any] = Field(default={})
-    """Arguments used for involing the task."""
+    """Arguments used for invoking the task."""
 
     model_args: dict[str, Any] = Field(default={})
     """Model specific arguments."""
 
     config: EvalConfig
     """Configuration values for eval."""
 
@@ -305,15 +305,15 @@
     status: Literal["started", "success", "error"] = Field(default="started")
     """Status of evaluation (did it succeed or fail)."""
 
     eval: EvalSpec
     """Eval identity and configuration."""
 
     plan: EvalPlan = Field(default=EvalPlan())
-    """Eval plan (sovers and config)"""
+    """Eval plan (solvers and config)"""
 
     results: EvalResults | None = None
     """Eval results (scores and metrics)."""
 
     stats: EvalStats = Field(default=EvalStats())
     """Eval stats (runtime, model usage)"""
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/model/__init__.py` & `inspect_ai-0.3.9/src/inspect_ai/model/__init__.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/model/_model.py` & `inspect_ai-0.3.9/src/inspect_ai/model/_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     suffix: str | None
     """The suffix that comes after a completion of inserted text. OpenAI only."""
 
     top_k: int | None
     """Randomly sample the next word from the top_k most likely next words. Anthropic, Google, and HuggingFace only."""
 
     num_choices: int | None
-    """How many chat completion choices to generate for each input message. Open AI, Google, and TogetherAI only."""
+    """How many chat completion choices to generate for each input message. OpenAI, Google, and TogetherAI only."""
 
     logprobs: bool | None
     """Return log probabilities of the output tokens. OpenAI, TogetherAI, and Huggingface only."""
 
     top_logprobs: int | None
     """Number of most likely tokens (0-20) to return at each token position, each with an associated log probability. OpenAI and Huggingface only."""
 
@@ -133,15 +133,15 @@
     suffix: str | None = Field(default=None)
     """The suffix that comes after a completion of inserted text. OpenAI only."""
 
     top_k: int | None = Field(default=None)
     """Randomly sample the next word from the top_k most likely next words. Anthropic, Google, and HuggingFace only."""
 
     num_choices: int | None = Field(default=None)
-    """How many chat completion choices to generate for each input message. Open AI, Google, and TogetherAI only."""
+    """How many chat completion choices to generate for each input message. OpenAI, Google, and TogetherAI only."""
 
     logprobs: bool | None = Field(default=None)
     """Return log probabilities of the output tokens. OpenAI, TogetherAI, and Huggingface only."""
 
     top_logprobs: int | None = Field(default=None)
     """Number of most likely tokens (0-20) to return at each token position, each with an associated log probability. OpenAI and Huggingface only."""
 
@@ -300,39 +300,45 @@
 
 
 StopReason = Literal["stop", "length", "tool_calls", "content_filter", "unknown"]
 """Reason that the model stopped generating."""
 
 
 class TopLogprob(BaseModel):
+    """List of the most likely tokens and their log probability, at this token position."""
+
     token: str
     """The top-kth token represented as a string."""
 
     logprob: float
     """The log probability value of the model for the top-kth token."""
 
     bytes: list[int]
     """The top-kth token represented as a byte array (a list of integers)."""
 
 
 class Logprob(BaseModel):
+    """Log probability for a token."""
+
     token: str
     """The predicted token represented as a string."""
 
     logprob: float
     """The log probability value of the model for the predicted token."""
 
     bytes: list[int]
     """The predicted token represented as a byte array (a list of integers)."""
 
     top_logprobs: list[TopLogprob] | None
     """If the `top_logprobs` argument is greater than 0, this will contain an ordered list of the top K most likely tokens and their log probabilities."""
 
 
 class Logprobs(BaseModel):
+    """Log probability information for a completion choice."""
+
     content: list[Logprob]
     """a (num_generated_tokens,) length list containing the individual log probabilities for each generated token."""
 
 
 class ChatCompletionChoice(BaseModel):
     message: ChatMessageAssistant
     """Assistant message."""
@@ -426,15 +432,15 @@
         tool_choice: ToolChoice,
         config: GenerateConfig,
     ) -> ModelOutput:
         """Generate output from the model.
 
         Args:
           input (str | list[ChatMessage]): Chat message
-            input (if a `str` is passed it is convereted
+            input (if a `str` is passed it is converted
             to a `ChatUserMessage`).
           tools (list[ToolInfo]): Tools available for the
             model to call.
           tool_choice (ToolChoice): Directives to the model
             as to which tools to prefer.
           config (GenerateConfig): Model configuration.
 
@@ -500,15 +506,15 @@
         tool_choice: ToolChoice | None = None,
         config: GenerateConfig = GenerateConfig(),
     ) -> ModelOutput:
         """Generate output from the model.
 
         Args:
           input (str | list[ChatMessage]): Chat message
-            input (if a `str` is passed it is convereted
+            input (if a `str` is passed it is converted
             to a `ChatUserMessage`).
           tools (list[ToolInfo]): Tools available for the
             model to call.
           tool_choice (ToolChoice): Directives to the model
             as to which tools to prefer.
           config (GenerateConfig): Model configuration.
 
@@ -534,15 +540,15 @@
         # see if we have a connection semaphore (we won't if we
         # are running outside of an eval()). this is how we enforce
         # concurrency limits (max_connections) for the model
         if using_concurrency():
             async with self._connection_concurrency(config):
                 return await self._generate(input, tools, tool_choice, config)
 
-        # no connection semaphore, just proceed straight ot the call
+        # no connection semaphore, just proceed straight to the call
         else:
             return await self._generate(input, tools, tool_choice, config)
 
     async def _generate(
         self,
         input: list[ChatMessage],
         tools: list[ToolInfo],
@@ -581,15 +587,15 @@
             # filter out inactive tool system messages
             input = [
                 message
                 for message in input
                 if not is_inactive_tool_system_message(message)
             ]
 
-            # optionally collapse *consecutive* messages into one - some apis eg anthropic require this
+            # optionally collapse *consecutive* messages into one - some apis e.g. anthropic require this
             if self.api.collapse_user_messages():
                 input = collapse_consecutive_user_messages(input)
 
             if self.api.collapse_assistant_messages():
                 input = collapse_consecutive_assistant_messages(input)
 
         # retry for rate limit errors
@@ -640,15 +646,15 @@
     # (which would likely cause the rate limit to be exceeded). conversely if
     # you are using distinct models/endpoints/accounts within an eval you should
     # be able get the full max_connections for each of them. subclasses can
     # override the _connection_key() argument to provide a scope within which
     # to enforce max_connections (e.g. by account/api_key, by endpoint, etc.)
 
     def _connection_concurrency(self, config: GenerateConfig) -> asyncio.Semaphore:
-        """Get the appropiate connection semaphore for this model instance."""
+        """Get the appropriate connection semaphore for this model instance."""
         max_connections = (
             config.max_connections
             if config.max_connections
             else self.api.max_connections()
         )
         model_name = ModelName(self)
         return concurrency(
@@ -660,15 +666,15 @@
 
 class ModelName:
     r"""Model name (api and specific model served by the api).
 
     Can be used for structural pattern matching of models against
     various string specifications of models. Used primarily by
     tasks to allow them to condition their behavior on models or
-    model famillies.
+    model families.
 
     String specifications can be fully specified (e.g. openai/gpt-4),
     partially specified by model name only (e.g. gpt-4) or even
     partially specified by a substring of model name (e.g. gpt).
     """
 
     def __init__(self, model: str | Model) -> None:
@@ -755,40 +761,33 @@
     api_name = None
     parts = model.split("/")
     if len(parts) > 1:
         api_name = parts[0]
         model = "/".join(parts[1:])
 
     # predicate to match model
-    def match_model(info: RegistryInfo) -> bool:
+    def match_modelapi_type(info: RegistryInfo) -> bool:
         # strip package name (we use the 'api' as the namespace, we will
         # introduce package scoping if it proves necessary)
-        if info.type == "modelapi":
-            # model patterns for this provider
-            models = info.metadata.get("models", [])
-
-            # if there is an api_name explicitly specified that
-            # matches the registered api then trust the model name
-            # TODO: this is ugly, we need to clarify the relationship
-            # and registraiton semantics of pkg -> provider -> model
-            if (
-                info.name == api_name
-                or info.name.replace(f"{PKG_NAME}/", "") == api_name
-            ):
-                return True
-            # otherwise check for a name match
-            else:
-                return len([name for name in models if name in model]) > 0
+
+        # if there is an api_name explicitly specified that
+        # matches the registered api then trust the model name
+        # TODO: this is ugly, we need to clarify the relationship
+        # and registration semantics of pkg -> provider -> model
+        if info.type == "modelapi" and (
+            info.name == api_name or info.name.replace(f"{PKG_NAME}/", "") == api_name
+        ):
+            return True
         else:
             return False
 
     # find a matching model type
-    model_types = registry_find(match_model)
-    if len(model_types) > 0:
-        modelapi_type = cast(type[ModelAPI], model_types[0])
+    modelapi_types = registry_find(match_modelapi_type)
+    if len(modelapi_types) > 0:
+        modelapi_type = cast(type[ModelAPI], modelapi_types[0])
         modelapi_instance = modelapi_type(
             model_name=model, base_url=base_url, config=config, **model_args
         )
         return Model(modelapi_instance, config)
 
     else:
         from_api = f" from {api_name}" if api_name else ""
@@ -875,15 +874,15 @@
     else:
         messages.append(message)
     return messages
 
 
 def combine_messages(
     a: ChatMessage, b: ChatMessage, message_type: Type[ChatMessage]
-) -> ChatMessageUser:
+) -> ChatMessage:
     if isinstance(a.content, str) and isinstance(b.content, str):
         return message_type(content=f"{a.content}\n{b.content}")
     elif isinstance(a.content, list) and isinstance(b.content, list):
         return message_type(content=a.content + b.content)
     elif isinstance(a.content, str) and isinstance(b.content, list):
         return message_type(content=b.content + [ContentText(text=a.content)])
     else:
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/model/_providers/anthropic.py` & `inspect_ai-0.3.9/src/inspect_ai/model/_providers/anthropic.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,27 +178,27 @@
             top_p=config.top_p if config.top_p is not None else NOT_GIVEN,
             top_k=config.top_k if config.top_k is not None else NOT_GIVEN,
             timeout=float(config.timeout) if config.timeout is not None else NOT_GIVEN,
         )
 
     @override
     def max_tokens(self) -> int | None:
-        # anthropic requires you to expicitly specify max_tokens (most others
+        # anthropic requires you to explicitly specify max_tokens (most others
         # set it to the maximum allowable output tokens for the model).
         return DEFAULT_MAX_TOKENS
 
     @override
     def connection_key(self) -> str:
         return self.api_key
 
     @override
     def is_rate_limit(self, ex: BaseException) -> bool:
         # We have observed that anthropic will frequently return InternalServerError
-        # seeminly in place of RateLimitError (at the very least the errors seem to
-        # always be transient). Equating this to rate limit errors may occationally
+        # seemingly in place of RateLimitError (at the very least the errors seem to
+        # always be transient). Equating this to rate limit errors may occasionally
         # result in retrying too many times, but much more often will avert a failed
         # eval that just needed to survive a transient error
         return (
             isinstance(ex, RateLimitError)
             or isinstance(ex, InternalServerError)
             or isinstance(ex, APIConnectionError)
         )
@@ -265,18 +265,18 @@
         for function in chat_functions
     ]
 
     return system_message, beta_tools, beta_messages
 
 
 async def tools_beta_message_param(message: ChatMessage) -> ToolsBetaMessageParam:
-    # no system role for anthropic (this is more like an asseration,
+    # no system role for anthropic (this is more like an assertion,
     # as these should have already been filtered out)
     if message.role == "system":
-        raise ValueError("Antropic models do not support the system role")
+        raise ValueError("Anthropic models do not support the system role")
 
     # "tool" means serving a tool call result back to claude
     elif message.role == "tool":
         if message.tool_error is not None:
             content: str | list[TextBlockParam] = message.tool_error
         if isinstance(message.content, str):
             content = [TextBlockParam(type="text", text=message.content)]
@@ -422,16 +422,16 @@
     return system_message, cast(list[ChatMessage], messages)
 
 
 #######################################################################################
 # Resolve input, tools, and config into the right shape of input for Anthropic models.
 #
 # Anthropic tools are defined not using a tools component of their API, but rather by
-# defineing all available tools in the system message. If there are tools then there
-# is also a requirement to define a custom stop sequence. This fucntion sorts all of
+# defining all available tools in the system message. If there are tools then there
+# is also a requirement to define a custom stop sequence. This function sorts all of
 # that out and returns a system message, a stop sequence (if necessary) and the list
 # of anthropic-native MessageParam objects (including converting role="tool" messages
 # into XML encoded role="user" messages for Claude
 #######################################################################################
 
 FUNCTIONS_STOP_SEQ = "</function_calls>"
 
@@ -504,15 +504,15 @@
 """
 
 
 async def message_param(message: ChatMessage) -> MessageParam:
     # no system role for anthropic (this is more like an assertion,
     # as these should have already been filtered out)
     if message.role == "system":
-        raise ValueError("Antropic models do not support the system role")
+        raise ValueError("Anthropic models do not support the system role")
 
     # "tool" means serving a tool call result back to claude
     elif message.role == "tool":
         return tool_message_param(message)
 
     # tool_calls means claude is attempting to call our tools
     elif message.role == "assistant" and message.tool_calls:
@@ -755,15 +755,15 @@
             )
 
         parameters = re.findall(
             r"<parameters>.*?</parameters>", invoke_string, re.DOTALL
         )
         if not parameters:
             raise ValueError(
-                "Missing <parameters></paraeters> tags inside of <invoke></invoke> tags."
+                "Missing <parameters></parameters> tags inside of <invoke></invoke> tags."
             )
 
         if len(parameters) > 1:
             raise ValueError(
                 "More than one set of <parameters></parameters> tags specified inside single set of <invoke></invoke> tags."
             )
 
@@ -804,15 +804,15 @@
             )
         )
 
     return ContentWithFunctionCalls(func_call_prefix_content, invokes)
 
 
 #######################################################################################
-# Thse functions deal with converting Anthropic <function_call> to our native ToolCall
+# These functions deal with converting Anthropic <function_call> to our native ToolCall
 #######################################################################################
 
 
 def tool_call(invoke: FunctionCall, tools: list[ToolInfo]) -> ToolCall:
     tool_def = next((tool for tool in tools if invoke.function == tool.name), None)
     return ToolCall(
         id=invoke.function,
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/model/_providers/azureai.py` & `inspect_ai-0.3.9/src/inspect_ai/model/_providers/azureai.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/model/_providers/bedrock.py` & `inspect_ai-0.3.9/src/inspect_ai/model/_providers/bedrock.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/model/_providers/cloudflare.py` & `inspect_ai-0.3.9/src/inspect_ai/model/_providers/cloudflare.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from .._tool import ToolChoice, ToolInfo
 from .._util import (
     chat_api_input,
     chat_api_request,
     is_chat_api_rate_limit,
 )
 
-# CloudFlare supported models:
+# Cloudflare supported models:
 # https://developers.cloudflare.com/workers-ai/models/#text-generation
 
 
 class CloudFlareAPI(ModelAPI):
     def __init__(
         self,
         model_name: str,
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/model/_providers/google.py` & `inspect_ai-0.3.9/src/inspect_ai/model/_providers/google.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,15 +275,15 @@
     candidates: list[Candidate],
 ) -> list[ChatCompletionChoice]:
     candidates = copy(candidates)
     candidates.sort(key=lambda c: c.index)
     return [completion_choice_from_candidate(candidate) for candidate in candidates]
 
 
-# google deson't export FinishReason (it's in a sub-namespace with a beta
+# google doesn't export FinishReason (it's in a sub-namespace with a beta
 # designation that seems destined to change, so we vendor the enum here)
 class FinishReason:
     FINISH_REASON_UNSPECIFIED = 0
     STOP = 1
     MAX_TOKENS = 2
     SAFETY = 3
     RECITATION = 4
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/model/_providers/hf.py` & `inspect_ai-0.3.9/src/inspect_ai/model/_providers/hf.py`

 * *Files 4% similar despite different names*

```diff
@@ -149,27 +149,27 @@
         )
 
         # gather logprobs
         final_logprobs = None
         if config.logprobs is not None:
             final_logprobs = extract_logprobs(
                 response=response,
-                top_logprobs=config.top_logprobs,
+                top=config.top_logprobs,
                 tokenizer=self.tokenizer,
             )
 
         # construct choice
         choice = ChatCompletionChoice(
             message=ChatMessageAssistant(
                 content=response.output,
                 source="generate",
             ),
-            logprobs=Logprobs(content=final_logprobs)
-            if final_logprobs is not None
-            else None,
+            logprobs=(
+                Logprobs(content=final_logprobs) if final_logprobs is not None else None
+            ),
         )
 
         # return output
         return ModelOutput(
             model=self.model_name,
             choices=[choice],
             usage=ModelUsage(
@@ -210,14 +210,20 @@
         seed = np.random.default_rng().integers(2**32 - 1)
     # python hash seed
     os.environ["PYTHONHASHSEED"] = str(seed)
     # transformers seed
     set_seed(seed)
 
 
+# return value from generate as a result of specifying return_dict_in_generate
+class ModelGenerateOutput:
+    sequences: Tensor
+    logits: tuple[Tensor]
+
+
 class Tokenizer(Protocol):
     def __call__(
         self, input: list[str]
     ) -> dict[Literal["input_ids", "attention_mask"], Tensor]: ...
 
 
 class Generator(Protocol):
@@ -262,29 +268,29 @@
 async def batched_generate(input: GenerateInput) -> GenerateOutput:
     # start the background thread if necessary
     global batch_thread
     if batch_thread is None:
         batch_thread = Thread(target=process_batches, daemon=True)
         batch_thread.start()
 
-    # enque the job
+    # enqueue the job
     loop = asyncio.get_event_loop()
     future: asyncio.Future[GenerateOutput] = loop.create_future()
     batch_queue.put(_QueueItem(input=input, future=future, loop=loop))
 
     # await the job
     await future
 
     # return it
     return future.result()
 
 
 def process_batches() -> None:
     while True:
-        # drain the queue (wait until no new messages have shown up for 2 secones)
+        # drain the queue (wait until no new messages have shown up for 2 seconds)
         inputs: list[tuple[GenerateInput, asyncio.Future[GenerateOutput]]] = []
         while True:
             try:
                 input = batch_queue.get(timeout=2)
                 loop = input.loop
                 inputs.append((input.input, input.future))
                 if len(inputs) == input.input.batch_size:
@@ -311,25 +317,26 @@
             input_ids = tokenized_inputs["input_ids"]
             attention_mask = tokenized_inputs["attention_mask"]
             input_ids = input_ids.to(device)
             attention_mask = attention_mask.to(device)
 
             # generate
             with torch.inference_mode():
-                generation_outputs = generator(
-                    input_ids=input_ids, attention_mask=attention_mask
+                generation_outputs = cast(
+                    ModelGenerateOutput,
+                    generator(input_ids=input_ids, attention_mask=attention_mask),
                 )
                 generate_ids = generation_outputs.sequences
                 logits = generation_outputs.logits
 
             # get logprobs from logits
             logprobs = None
             if logits is not None:
-                logits = torch.stack(logits).transpose(0, 1)
-                logprobs = torch.nn.functional.log_softmax(logits, dim=-1)
+                stacked_logits = torch.stack(logits).transpose(0, 1)
+                logprobs = torch.nn.functional.log_softmax(stacked_logits, dim=-1)
 
             # decode
             generated_tokens = generate_ids[:, input_ids.size(dim=1) :]
             if logprobs is not None:
                 assert logprobs.shape[1] == generated_tokens.shape[1]
             outputs = decoder(sequences=generated_tokens)
 
@@ -357,23 +364,23 @@
             for inp in inputs:
                 future = inp[1]
                 loop.call_soon_threadsafe(future.set_exception, ex)
 
 
 def extract_logprobs(
     response: GenerateOutput,
-    top_logprobs: int | None,
+    top: int | None,
     tokenizer: PreTrainedTokenizerBase,
 ) -> list[Logprob]:
     assert response.logprobs is not None
-    k = top_logprobs or 1
+    k = top or 1
     topk_values, topk_inds = response.logprobs.topk(k=k, dim=-1)
     final_logprobs = []
     for toks, vals in zip(topk_inds, topk_values):
-        top_logprobs = []
+        top_logprobs: list[TopLogprob] = []
         for tok, val in zip(toks, vals):
             # TODO: you get byte artifacts converting single ids to tokens like this...
             # but `tokenizer.decode` strips spaces. There must be a better way to do this.
             token_str = tokenizer.convert_ids_to_tokens(tok.item())
             top_logprobs.append(
                 TopLogprob(
                     token=token_str,
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/model/_providers/mistral.py` & `inspect_ai-0.3.9/src/inspect_ai/model/_providers/mistral.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/model/_providers/openai.py` & `inspect_ai-0.3.9/src/inspect_ai/model/_providers/openai.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/model/_providers/providers.py` & `inspect_ai-0.3.9/src/inspect_ai/model/_providers/providers.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 from inspect_ai._util.version import verify_required_version
 
 from .._model import ModelAPI
 from .._registry import modelapi
 
 # Defer importing model api classes until they are actually used
 # (this allows the package to load without the optional deps)
-# Note that some api providers (e.g. CloudFlare, AzureAI) don't
-# strictly require this treament but we do it anyway for uniformity,
+# Note that some api providers (e.g. Cloudflare, AzureAI) don't
+# strictly require this treatment but we do it anyway for uniformity,
 
 
-@modelapi(name="openai", models=["gpt"])
+@modelapi(name="openai")
 def openai() -> type[ModelAPI]:
     # validate
     validate_openai_client("OpenAI API")
 
     # in the clear
     from .openai import OpenAIAPI
 
     return OpenAIAPI
 
 
-@modelapi(name="anthropic", models=["claude"])
+@modelapi(name="anthropic")
 def anthropic() -> type[ModelAPI]:
     FEATURE = "Anthropic API"
     PACKAGE = "anthropic"
     MIN_VERSION = "0.23.0"
 
     # verify we have the package
     try:
@@ -38,15 +38,15 @@
 
     # in the clear
     from .anthropic import AnthropicAPI
 
     return AnthropicAPI
 
 
-@modelapi(name="google", models=["gemini", "bison", "gdm"])
+@modelapi(name="google")
 def google() -> type[ModelAPI]:
     FEATURE = "Google API"
     PACKAGE = "google-generativeai"
     MIN_VERSION = "0.4.0"
 
     # verify we have the package
     try:
@@ -64,15 +64,17 @@
 
 
 @modelapi(name="hf")
 def hf() -> type[ModelAPI]:
     try:
         from .hf import HuggingFaceAPI
     except ImportError:
-        raise pip_dependency_error("Hugging Face Models", ["torch", "transformers"])
+        raise pip_dependency_error(
+            "Hugging Face Models", ["torch", "transformers", "accelerate"]
+        )
 
     return HuggingFaceAPI
 
 
 @modelapi(name="cf")
 def cf() -> type[ModelAPI]:
     from .cloudflare import CloudFlareAPI
@@ -108,14 +110,25 @@
 
     # in the clear
     from .together import TogetherAIAPI
 
     return TogetherAIAPI
 
 
+@modelapi(name="ollama")
+def ollama() -> type[ModelAPI]:
+    # validate
+    validate_openai_client("Ollama API")
+
+    # in the clear
+    from .ollama import OllamaAPI
+
+    return OllamaAPI
+
+
 @modelapi(name="azureai")
 def azureai() -> type[ModelAPI]:
     from .azureai import AzureAIAPI
 
     return AzureAIAPI
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/model/_providers/together.py` & `inspect_ai-0.3.9/src/inspect_ai/model/_providers/together.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/model/_providers/util.py` & `inspect_ai-0.3.9/src/inspect_ai/model/_providers/util.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/model/_registry.py` & `inspect_ai-0.3.9/src/inspect_ai/model/_registry.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,42 +6,36 @@
     registry_name,
     registry_tag,
 )
 
 from ._model import ModelAPI
 
 
-def modelapi_register(
-    model_type: type[ModelAPI], name: str, models: list[str]
-) -> type[ModelAPI]:
+def modelapi_register(model_type: type[ModelAPI], name: str) -> type[ModelAPI]:
     r"""Register a model api.
 
     Args:
         model_type (type[Model]): Class deriving from Model
         name (str): API serving this model
-        models (list[str]): Model names by this API
 
     Returns:
         Model API with registry attributes.
     """
     registry_add(
         model_type,
-        RegistryInfo(type="modelapi", name=name, metadata=dict(models=models)),
+        RegistryInfo(type="modelapi", name=name),
     )
     return model_type
 
 
-def modelapi(name: str, models: list[str] = []) -> Callable[..., type[ModelAPI]]:
+def modelapi(name: str) -> Callable[..., type[ModelAPI]]:
     r"""Decorator for registering model APIs.
 
     Args:
         name (str): Name of API
-        models (list[str]): Model names that should match this API.
-          If no `models` are provided then this model type will always
-          require an API prefix (e.g. "hf/openai-community/gpt2")
 
     Returns:
         Model API with registry attributes.
     """
 
     # create_model_wrapper:
     #  (a) Add the type[Model] to the registry using the appropriately
@@ -62,22 +56,21 @@
             model = model_type(*args, **kwargs)
             registry_tag(
                 model_type,
                 model,
                 RegistryInfo(
                     type="modelapi",
                     name=model_api,
-                    metadata=dict(models=models),
                 ),
                 *args,
                 **kwargs,
             )
             return model
 
-        return modelapi_register(cast(type[ModelAPI], model_wrapper), model_api, models)
+        return modelapi_register(cast(type[ModelAPI], model_wrapper), model_api)
 
     def wrapper(
         model_type: type[ModelAPI] | Callable[..., type[ModelAPI]],
     ) -> type[ModelAPI]:
         return create_model_wrapper(model_type, name)
 
     return wrapper
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/model/_tool.py` & `inspect_ai-0.3.9/src/inspect_ai/model/_tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     params: list[ToolParam]
     """Tool parameters"""
 
 
 @dataclass
 class ToolCall:
     id: str
-    """Unique identifer for tool call."""
+    """Unique identifier for tool call."""
 
     function: str
     """Function called."""
 
     arguments: dict[str, Any]
     """Arguments to function."""
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/model/_util.py` & `inspect_ai-0.3.9/src/inspect_ai/model/_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     # make the call
     return await call_api()
 
 
 def chat_api_input(input: list[ChatMessage]) -> list[dict[str, str]]:
     """Prepare chat prompt data for sending in an HTTP POST request.
 
-    Many chat APIs (e.g. Mistral and CloudFlare) take the OpenAI
+    Many chat APIs (e.g. Mistral and Cloudflare) take the OpenAI
     role/content data structure. This is a convenience function that
     takes the `input` to `generate()` and converts it into a JSON
     serializable object that conforms to this structure.
 
     Args:
         input (list[ChatMessage]): Input to generate from
 
@@ -141,15 +141,15 @@
             ),
         ),
     )
 
 
 # When calling chat_api_request() we use tenacity as the retry wrapper, so
 # checking for rate limit errors needs to punch through the RetryError and
-# look at its `__cause__`. we've observed CloudFlare giving transient 500
+# look at its `__cause__`. we've observed Cloudflare giving transient 500
 # status as well as a ReadTimeout, so we count these as rate limit errors
 def is_chat_api_rate_limit(ex: BaseException) -> bool:
     return isinstance(ex, RetryError) and (
         (
             isinstance(ex.__cause__, httpx.HTTPStatusError)
             and (
                 ex.__cause__.response.status_code == 429
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/scorer/__init__.py` & `inspect_ai-0.3.9/src/inspect_ai/scorer/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     metric,
     value_to_float,
 )
 from ._metrics.accuracy import accuracy
 from ._metrics.mean import mean
 from ._metrics.std import bootstrap_std
 from ._model import model_graded_fact, model_graded_qa
+from ._multi import ScoreReducer, majority_vote, multi_scorer
 from ._pattern import pattern
 from ._scorer import (
     Scorer,
     Target,
     scorer,
 )
 
@@ -43,8 +44,11 @@
     "Value",
     "ValueToFloat",
     "value_to_float",
     "CORRECT",
     "INCORRECT",
     "PARTIAL",
     "NOANSWER",
+    "multi_scorer",
+    "majority_vote",
+    "ScoreReducer",
 ]
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/scorer/_answer.py` & `inspect_ai-0.3.9/src/inspect_ai/scorer/_answer.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/scorer/_common.py` & `inspect_ai-0.3.9/src/inspect_ai/scorer/_common.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/scorer/_match.py` & `inspect_ai-0.3.9/src/inspect_ai/scorer/_match.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,18 @@
     """Scorer which matches text or a number.
 
     Args:
        location (Literal["begin", "end", "any", "exact"]):
           Location to match at. "any" matches anywhere in the
           output; "exact" requires the output be exactly
           equal to the target (module whitespace, etc.)
-       ignore_case (bool): Do case insenstive comparison.
+       ignore_case (bool): Do case insensitive comparison.
        numeric (bool): Is this a numeric match? (in this
           case different punctuation removal rules are
-          used and numbers are normalized before comparisoin).
+          used and numbers are normalized before comparison).
     """
 
     def check(value: str, target: str) -> tuple[str, bool]:
         return match_str(
             value=value,
             target=target,
             location=location,
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/scorer/_metric.py` & `inspect_ai-0.3.9/src/inspect_ai/scorer/_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 logger = getLogger(__name__)
 
 CORRECT = "C"
 """Value to assign for correct answers."""
 
 INCORRECT = "I"
-"""Value to assing for incorrect answers."""
+"""Value to assign for incorrect answers."""
 
 PARTIAL = "P"
 """Value to assign for partial credit."""
 
 NOANSWER = "N"
 """Value to assign for no answer or refusal to answer."""
 
@@ -83,15 +83,15 @@
         return int(self._as_scalar())
 
     def as_float(self) -> float:
         """Read the score as a float."""
         return float(self._as_scalar())
 
     def as_bool(self) -> bool:
-        """Read the score as a boolan."""
+        """Read the score as a boolean."""
         return bool(self._as_scalar())
 
     def _as_scalar(self) -> str | int | float | bool:
         if (
             isinstance(self.value, str)
             or isinstance(self.value, int)
             or isinstance(self.value, float)
@@ -161,15 +161,15 @@
     def __call__(self, scores: list[Score]) -> int | float: ...
 
 
 MetricType = TypeVar("MetricType", Callable[..., Metric], type[Metric])
 r"""Metric type.
 Valid metric types include:
  - Functions that return a Metric
- - Classes derivied from Metric
+ - Classes derived from Metric
 """
 
 
 def metric_register(metric: MetricType, name: str = "") -> MetricType:
     r"""Register a function or class as a metric.
 
     Args:
@@ -254,11 +254,11 @@
     if isinstance(name, str):
 
         def wrapper(metric_type: MetricType) -> MetricType:
             return create_metric_wrapper(metric_type, name)
 
         return wrapper
 
-    # create a metric wrapper for the passsed metric_type
+    # create a metric wrapper for the passed metric_type
     else:
         metric_type = name
         return create_metric_wrapper(metric_type)
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/scorer/_metrics/accuracy.py` & `inspect_ai-0.3.9/src/inspect_ai/scorer/_metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/scorer/_metrics/mean.py` & `inspect_ai-0.3.9/src/inspect_ai/scorer/_metrics/mean.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/scorer/_metrics/std.py` & `inspect_ai-0.3.9/src/inspect_ai/scorer/_metrics/std.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/scorer/_model.py` & `inspect_ai-0.3.9/src/inspect_ai/scorer/_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import re
+from functools import partial
 
 from inspect_ai.model import ChatMessageUser, Model, get_model
 from inspect_ai.solver import TaskState
 from inspect_ai.util import resource
 
 from ._metric import INCORRECT, Score
 from ._metrics import accuracy, bootstrap_std
+from ._multi import majority_vote, multi_scorer
 from ._scorer import Scorer, Target, scorer
 
 
 @scorer(metrics=[accuracy(), bootstrap_std()])
 def model_graded_fact(
     template: str | None = None,
     instructions: str | None = None,
     grade_pattern: str | None = None,
     partial_credit: bool = False,
-    model: str | Model | None = None,
+    model: list[str | Model] | str | Model | None = None,
 ) -> Scorer:
     """Score a question/answer task with a fact response using a model.
 
     Args:
       template (str): Template for grading prompt. This template uses
         four variables: `question`, `criterion`, `answer`, and
         `instructions` (which is fed from the `instructions` parameter)
@@ -34,16 +36,15 @@
         The regex should have a single capture group that
         extracts exactly the letter C, P, or I.
       partial_credit (bool): Whether to allow for "partial" credit for
          answers (by default assigned a score of 0.5). Defaults
          to `False`. Note that this parameter is only used
          with the default `instructions` (as custom instructions
          provide their own prompts for grades).
-      model (str | Model | none): Model to use for grading
-         (by default the model being evaluated is used).
+      model (list[str | Model] | str | Model | None): Model or Models to use for grading. If multiple models are passed, a majority vote of their grade will be returned. By default the model being evaluated is used.
     """
     return model_graded_qa(
         template=template if template else DEFAULT_MODEL_GRADED_FACT_TEMPLATE,
         instructions=instructions,
         grade_pattern=grade_pattern,
         partial_credit=partial_credit,
         model=model,
@@ -52,15 +53,15 @@
 
 @scorer(metrics=[accuracy(), bootstrap_std()])
 def model_graded_qa(
     template: str | None = None,
     instructions: str | None = None,
     grade_pattern: str | None = None,
     partial_credit: bool = False,
-    model: str | Model | None = None,
+    model: list[str | Model] | str | Model | None = None,
 ) -> Scorer:
     """Score a question/answer task using a model.
 
     Args:
       template (str): Template for grading prompt. This template uses
         four variables: `question`, `criterion`, `answer`, and
         `instructions` (which is fed from the `instructions` parameter)
@@ -75,17 +76,40 @@
         The regex should have a single capture group that
         extracts exactly the letter C, P, I.
       partial_credit (bool): Whether to allow for "partial" credit for
         answers (by default assigned a score of 0.5). Defaults
         to `False`. Note that this parameter is only used
         with the default `instructions` (as custom instructions
         provide their own prompts for grades).
-      model (str | Model | None): Model to use for grading
-        (by default the model being evaluated is used).
+      model (list[str | Model] | str | Model | None): Model or Models to use for grading. If     multiple models are passed, a majority vote of their grade will be returned. By default the model being evaluated is used.
     """
+    # bind variables
+    get_scorer = partial(
+        _model_graded_qa_single, template, instructions, grade_pattern, partial_credit
+    )
+    # if only a single model is passed, return a single scorer
+    if model is None or not isinstance(model, list):
+        return get_scorer(model)
+
+    # otherwise, use multi scorer
+    assert isinstance(model, list)
+    scorers = [get_scorer(model) for model in model]
+    return multi_scorer(scorers, majority_vote)
+
+
+@scorer(metrics=[accuracy(), bootstrap_std()])
+def _model_graded_qa_single(
+    template: str | None = None,
+    instructions: str | None = None,
+    grade_pattern: str | None = None,
+    partial_credit: bool = False,
+    model: str | Model | None = None,
+) -> Scorer:
+    # returns a scorer that does model graded qa for a single model
+
     # resolve model
     grader_model = get_model(model)
 
     # resolve grading template, instructions, and grade_pattern
     template = template if template else DEFAULT_MODEL_GRADED_QA_TEMPLATE
     grading_template = resource(template)
     instructions = (
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/scorer/_pattern.py` & `inspect_ai-0.3.9/src/inspect_ai/scorer/_pattern.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         # extract the answer
         match = re.search(
             pattern, state.output.completion, re.IGNORECASE if ignore_case else 0
         )
 
         # got a match
         if match:
-            # handle case insentitive
+            # handle case insensitive
             answer = match.group(1) if len(match.groups()) == 1 else match.group(2)
             input = answer
             if ignore_case:
                 input = input.lower()
                 target = Target([t.lower() for t in target])
 
             # return score
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/scorer/_scorer.py` & `inspect_ai-0.3.9/src/inspect_ai/scorer/_scorer.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     TypeVar,
     Union,
     cast,
     overload,
     runtime_checkable,
 )
 
+from inspect_ai._util._async import is_callable_coroutine
 from inspect_ai._util.registry import (
     RegistryInfo,
     registry_add,
     registry_create,
     registry_info,
     registry_name,
     registry_tag,
@@ -66,15 +67,15 @@
 
 
 ScorerType = TypeVar("ScorerType", Callable[..., Scorer], type[Scorer])
 r"""Scorer type.
 
 Valid scorer types include:
  - Functions that return a Scorer
- - Classes derivied from Scorer
+ - Classes derived from Scorer
 """
 
 
 def scorer_register(scorer: ScorerType, name: str = "") -> ScorerType:
     r"""Register a function or class as a scorer.
 
     Args:
@@ -126,18 +127,23 @@
 
     def wrapper(scorer_type: ScorerType) -> ScorerType:
         # determine the name (explicit or implicit from object)
         scorer_name = registry_name(
             scorer_type, name if name else getattr(scorer_type, "__name__")
         )
 
-        # wrap instatiations of scorer so they carry registry info and metrics
+        # wrap instantiations of scorer so they carry registry info and metrics
         def scorer_wrapper(*args: Any, **kwargs: Any) -> Scorer:
             scorer = scorer_type(*args, **kwargs)
 
+            if not is_callable_coroutine(scorer):
+                raise TypeError(
+                    f"'{scorer_name}' is not declared as an async callable."
+                )
+
             registry_tag(
                 scorer_type,
                 scorer,
                 RegistryInfo(
                     type="scorer",
                     name=scorer_name,
                     metadata={SCORER_METRICS: metrics} | metadata,
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/solver/__init__.py` & `inspect_ai-0.3.9/src/inspect_ai/solver/__init__.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/solver/_critique.py` & `inspect_ai-0.3.9/src/inspect_ai/solver/_critique.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/solver/_multiple_choice.py` & `inspect_ai-0.3.9/src/inspect_ai/solver/_multiple_choice.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 {question}
 
 {choices}
 """
 
 
-# max tokens for differnet variations
+# max tokens for different variations
 MULTIPLE_CHOICE_MAX_TOKENS = 32
 MULTIPLE_CHOICE_MAX_TOKENS_COT = 1024
 
 
 @solver
 def multiple_choice(
     *,
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/solver/_plan.py` & `inspect_ai-0.3.9/src/inspect_ai/solver/_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         else:
             return "plan"
 
     steps: list[Solver]
     """Solvers to run for this plan."""
 
     finish: Solver | None = None
-    """Finishing sover that is always run even for early exit."""
+    """Finishing solver that is always run even for early exit."""
 
     cleanup: Callable[[TaskState], Awaitable[None]] | None = None
     """Function  called at the end of the plan (even if an exception occurs).
 
     Note that this function takes a `TaskState` but does not return one
     (it is only for cleanup not for transforming the state). Note also that
     this function should be declared `async`.
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/solver/_prompt.py` & `inspect_ai-0.3.9/src/inspect_ai/solver/_prompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """Parameterized prompt template.
 
     Prompt template containing a `{prompt}` placeholder and any
     number of additional `params`.
 
     Args:
       template (str | list[Message]):
-          The conversation template to use. A sipmle string or
+          The conversation template to use. A simple string or
           a list of messages
       **params (dict[str,Any]):
           A mapping of the parameters to fill into the template
           excluding the `{prompt}` parameter which is taken
           from the input.
 
     Returns:
@@ -38,15 +38,15 @@
 
 
 @solver
 def system_message(message: str) -> Solver:
     """Solver which inserts a system message into the conversation.
 
     The new message will go after other system messages (if there
-    are none it will be inserted at the beginnign of the conversation).
+    are none it will be inserted at the beginning of the conversation).
 
     Args:
        message (str): System message.
     """
     # read template
     content = resource(message)
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/solver/_solver.py` & `inspect_ai-0.3.9/src/inspect_ai/solver/_solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     cast,
     overload,
     runtime_checkable,
 )
 
 from typing_extensions import Unpack
 
+from inspect_ai._util._async import is_callable_coroutine
 from inspect_ai._util.registry import (
     RegistryInfo,
     registry_add,
     registry_create,
     registry_name,
     registry_tag,
 )
@@ -99,15 +100,15 @@
     @property
     def user_prompt(self) -> ChatMessageUser:
         """User prompt for this state.
 
         Tasks are very general and can have may types of inputs.
         However, in many cases solvers assume they can interact with
         the state as a "chat" in a predictable fashion (e.g. prompt
-        engineering solvers). This propery enables easy read and
+        engineering solvers). This property enables easy read and
         write access to the user chat prompt. Raises an
         exception if there is no user prompt
 
         Returns:
            First user `ChatMessage` if the current state has one, else `None`
         """
         prompt = next(
@@ -137,15 +138,15 @@
 
 
 @runtime_checkable
 class Solver(Protocol):
     r"""Contribute to solving an evaluation task.
 
     Contribute to the solution of a task by transforming a TaskState
-    (e.g. prompt enhancement, eliciation, etc.). Solvers return a
+    (e.g. prompt enhancement, elicitation, etc.). Solvers return a
     TaskState (which could simply be a modified version of the one
     they were passed) and optionally may call the generate() function
     to generate output (and a new TaskState with that output).
 
 
     Args:
         state (TaskState): States for tasks being evaluated.
@@ -163,15 +164,15 @@
 
 
 SolverType = TypeVar("SolverType", Callable[..., Solver], type[Solver])
 r"""Solver type.
 
 Valid solver types include:
  - Functions that return a Solver
- - Classes derivied from Solver
+ - Classes derived from Solver
 """
 
 
 def solver_register(solver: SolverType, name: str = "") -> SolverType:
     r"""Register a function or class as a solver.
 
     Args:
@@ -221,15 +222,15 @@
             Optional name for solver. If the decorator has no name
             argument then the name of the underlying SolverType
             object will be used to automatically assign a name.
 
     Returns:
         Solver with registry attributes.
 
-    Exmaples:
+    Examples:
         @solver
         def prompt_cot(state: TaskState, generate: Generate) -> None:
             ...
 
         @solver(name = "prompt_cot")
         def cot(state: TaskState, generate: Generate) -> None:
             ...
@@ -252,14 +253,17 @@
         solver_name = registry_name(
             solver_type, name if name else getattr(solver_type, "__name__")
         )
 
         def solver_wrapper(*args: Any, **kwargs: dict[str, Any]) -> Solver:
             solver = solver_type(*args, **kwargs)
 
+            if not is_callable_coroutine(solver):
+                raise TypeError(f"'{solver}' is not declared as an async callable.")
+
             registry_tag(
                 solver_type,
                 solver,
                 RegistryInfo(type="solver", name=solver_name),
                 *args,
                 **kwargs,
             )
@@ -272,15 +276,15 @@
     if isinstance(name, str):
 
         def wrapper(solver_type: SolverType) -> SolverType:
             return create_solver_wrapper(solver_type, name)
 
         return wrapper
 
-    # create a solver wrapper for the passsed solver_type
+    # create a solver wrapper for the passed solver_type
     else:
         solver_type = name
         return create_solver_wrapper(solver_type)
 
 
 @solver
 def generate() -> Solver:
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/solver/_tool/tool.py` & `inspect_ai-0.3.9/src/inspect_ai/solver/_tool/tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 
 ToolType = TypeVar("ToolType", Callable[..., Tool], type[Tool])
 r"""Tool type.
 
 Valid tool types include:
  - Functions that return a Tool
- - Classes derivied from Tool
+ - Classes derived from Tool
 """
 
 
 def tool_register(tool: ToolType, name: str) -> ToolType:
     r"""Register a function or class as a tool.
 
     Args:
@@ -73,15 +73,15 @@
     name: str | None = None,
 ) -> Callable[[Callable[..., Tool]], Callable[..., Tool]]:
     r"""Decorator for registering tools.
 
     Args:
         prompt (str):
             System prompt associated with this tool (provides
-            guideance to the LLM on how to use the tool)
+            guidance to the LLM on how to use the tool)
         name (str | None):
             Optional name for tool. If the decorator has no name
             argument then the name of the underlying ToolType
             object will be used to automatically assign a name.
         params (params): Parameters to be passed automatically to
             the tool. This currently allows only for mapping metadata
             fields from the input / task state onto parameters. These
@@ -98,26 +98,26 @@
                 return execute
 
             ```
 
     Returns:
         Tool with registry attributes.
     """
-    # remove spurous spacing from prompt (can occur if a multline string
+    # remove spurious spacing from prompt (can occur if a multiline string
     # is used to specify the prompt)
     if prompt:
         prompt = re.sub(r"\s+", " ", prompt)
 
     def wrapper(tool_type: ToolType) -> ToolType:
         # determine the name (explicit or implicit from object)
         tool_name = registry_name(
             tool_type, name if name else getattr(tool_type, "__name__")
         )
 
-        # wrap instatiations of scorer so they carry registry info and metrics
+        # wrap instantiations of scorer so they carry registry info and metrics
         def tool_wrapper(*args: Any, **kwargs: Any) -> Tool:
             tool = tool_type(*args, **kwargs)
             registry_tag(
                 tool_type,
                 tool,
                 RegistryInfo(
                     type="tool",
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/solver/_tool/tool_def.py` & `inspect_ai-0.3.9/src/inspect_ai/solver/_tool/tool_def.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/solver/_tool/use_tools.py` & `inspect_ai-0.3.9/src/inspect_ai/solver/_tool/use_tools.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/solver/_tool/web_search.py` & `inspect_ai-0.3.9/src/inspect_ai/solver/_tool/web_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
         query (str): Search query.
         relevance_model (Model): Model used to parse web pages for relevance.
         client: (httpx.Client): HTTP client to use to fetch the page
 
     Returns:
         str: Web page contents if relevant, else None.
     """
-    # retreive document
+    # retrieve document
     try:
         response = await client.get(link)
         response.raise_for_status()
     except httpx.HTTPError as exc:
         raise Exception(f"HTTP error occurred: {exc}")
 
     # parse it
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/util/_context/concurrency.py` & `inspect_ai-0.3.9/src/inspect_ai/util/_context/concurrency.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,16 @@
     Note that concurrency for model API access is handled internally
     via the `max_connections` generation config option. Concurrency
     for launching subprocesses is handled via the `subprocess` function.
 
     Args:
       name (str): Name for concurrency context. This serves as the
          display name for the context, and also the unique context
-         key (if the `key` parameter is ommitted)
-      concurrency (int): Maximum number of couroutines that can
+         key (if the `key` parameter is omitted)
+      concurrency (int): Maximum number of coroutines that can
          enter the context.
       key (str | None): Unique context key for this context. Optional.
          Used if the unique key isn't human readable -- e.g. includes
          api tokens or account ids so that the more readable `name`
          can be presented to users e.g in console UI>
 
     Returns:
@@ -39,15 +39,15 @@
     """
     # sort out key
     key = key if key else name
 
     # get semaphores dict (only valid when an eval is running)
     concurrency_semaphores = concurrency_semaphores_context_var.get(None)
     if concurrency_semaphores is None:
-        raise RuntimeError("Attempted to get eval sempahore when eval not running")
+        raise RuntimeError("Attempted to get eval semaphore when eval not running")
 
     # do we have an existing semaphore? if not create one and store it
     semaphore = concurrency_semaphores.get(key, None)
     if semaphore is None:
         semaphore = ConcurencySempahore(
             name, concurrency, asyncio.Semaphore(concurrency)
         )
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/util/_context/logger.py` & `inspect_ai-0.3.9/src/inspect_ai/util/_context/logger.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai/util/_context/resource.py` & `inspect_ai-0.3.9/src/inspect_ai/util/_context/resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         resource (str): Path to local or remote (e.g. s3://)
           resource, or for `type="auto"` (the default),
           a string containing the literal resource value.
         type (Literal["auto", "file"]): For "auto" (the default),
           interpret the resource as a literal string if its not
           a valid path. For "file", always interpret it as
           a file path.
-        fs_options (dict[str, Any]): Optional. Addional
+        fs_options (dict[str, Any]): Optional. Additional
           arguments to pass through to the `fsspec` filesystem
           provider (e.g. `S3FileSystem`). Use `{"anon": True }`
           if you are accessing a public S3 bucket with no
           credentials.
 
     Returns:
        Text content of resource.
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai/util/_context/subprocess.py` & `inspect_ai-0.3.9/src/inspect_ai/util/_context/subprocess.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/src/inspect_ai.egg-info/PKG-INFO` & `inspect_ai-0.3.9/src/inspect_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspect_ai
-Version: 0.3.8
+Version: 0.3.9
 Summary: Framework for large language model evaluations
 Author: UK AI Safety Institute
 License: MIT License
 Project-URL: Documentation, https://UKGovernmentBEIS.github.io/inspect_ai/
 Project-URL: Source Code, https://github.com/UKGovernmentBEIS/inspect_ai
 Project-URL: Issue Tracker, https://github.com/UKGovernmentBEIS/inspect_ai/issues
 Classifier: Development Status :: 4 - Beta
@@ -95,8 +95,8 @@
 
 ```         
 $ git clone https://github.com/UKGovernmentBEIS/inspect_ai.git
 $ cd inspect_ai
 $ pip install -e ".[dev]"
 ```
 
-If you use VS Code, you should be sure to have installed the recommended extensions (Python, Ruff, and MyPy). Note that you'll be promoted to install these when you open the project in VS Code.
+If you use VS Code, you should be sure to have installed the recommended extensions (Python, Ruff, and MyPy). Note that you'll be prompted to install these when you open the project in VS Code.
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai.egg-info/SOURCES.txt` & `inspect_ai-0.3.9/src/inspect_ai.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 docs/index.qmd
 docs/log-viewer.qmd
 docs/models.qmd
 docs/scorers.qmd
 docs/solvers.qmd
 docs/theme.scss
 docs/tools.qmd
+docs/vscode.qmd
 docs/workflow.qmd
 docs/_examples/arc.qmd
 docs/_examples/biology_qa.qmd
 docs/_examples/footer.qmd
 docs/_examples/gsm8k.qmd
 docs/_examples/hellaswag.qmd
 docs/_examples/index.qmd
@@ -62,14 +63,20 @@
 docs/images/inspect-view-logging.png
 docs/images/inspect-view-main.png
 docs/images/inspect-view-messages.png
 docs/images/inspect-view-metadata.png
 docs/images/inspect-view-scoring.png
 docs/images/inspect-view-sort.png
 docs/images/inspect-view-splash.png
+docs/images/inspect-vscode-config.png
+docs/images/inspect-vscode-install.png
+docs/images/inspect-vscode-logview.png
+docs/images/inspect-vscode-output-channel.png
+docs/images/inspect-vscode-run-task.png
+docs/images/inspect.png
 docs/images/popularity.png
 docs/images/rate-limit.png
 docs/images/running-theory.png
 examples/biology_qa.py
 examples/popularity.py
 examples/security_guide.py
 examples/theory_of_mind.py
@@ -99,21 +106,27 @@
 src/inspect_ai/_cli/util.py
 src/inspect_ai/_cli/view.py
 src/inspect_ai/_display/__init__.py
 src/inspect_ai/_display/_display.py
 src/inspect_ai/_display/logger.py
 src/inspect_ai/_display/rich.py
 src/inspect_ai/_eval/eval.py
-src/inspect_ai/_eval/images.py
 src/inspect_ai/_eval/list.py
 src/inspect_ai/_eval/loader.py
-src/inspect_ai/_eval/log.py
 src/inspect_ai/_eval/registry.py
 src/inspect_ai/_eval/score.py
-src/inspect_ai/_eval/task.py
+src/inspect_ai/_eval/types.py
+src/inspect_ai/_eval/task/constants.py
+src/inspect_ai/_eval/task/generate.py
+src/inspect_ai/_eval/task/images.py
+src/inspect_ai/_eval/task/log.py
+src/inspect_ai/_eval/task/results.py
+src/inspect_ai/_eval/task/run.py
+src/inspect_ai/_eval/task/util.py
+src/inspect_ai/_util/_async.py
 src/inspect_ai/_util/appdirs.py
 src/inspect_ai/_util/constants.py
 src/inspect_ai/_util/datetime.py
 src/inspect_ai/_util/dev.py
 src/inspect_ai/_util/docstring.py
 src/inspect_ai/_util/dotenv.py
 src/inspect_ai/_util/error.py
@@ -229,24 +242,26 @@
 src/inspect_ai/model/_providers/anthropic.py
 src/inspect_ai/model/_providers/azureai.py
 src/inspect_ai/model/_providers/bedrock.py
 src/inspect_ai/model/_providers/cloudflare.py
 src/inspect_ai/model/_providers/google.py
 src/inspect_ai/model/_providers/hf.py
 src/inspect_ai/model/_providers/mistral.py
+src/inspect_ai/model/_providers/ollama.py
 src/inspect_ai/model/_providers/openai.py
 src/inspect_ai/model/_providers/providers.py
 src/inspect_ai/model/_providers/together.py
 src/inspect_ai/model/_providers/util.py
 src/inspect_ai/scorer/__init__.py
 src/inspect_ai/scorer/_answer.py
 src/inspect_ai/scorer/_common.py
 src/inspect_ai/scorer/_match.py
 src/inspect_ai/scorer/_metric.py
 src/inspect_ai/scorer/_model.py
+src/inspect_ai/scorer/_multi.py
 src/inspect_ai/scorer/_pattern.py
 src/inspect_ai/scorer/_scorer.py
 src/inspect_ai/scorer/_metrics/__init__.py
 src/inspect_ai/scorer/_metrics/accuracy.py
 src/inspect_ai/scorer/_metrics/mean.py
 src/inspect_ai/scorer/_metrics/std.py
 src/inspect_ai/solver/__init__.py
@@ -263,15 +278,15 @@
 src/inspect_ai/util/__init__.py
 src/inspect_ai/util/_context/__init__.py
 src/inspect_ai/util/_context/concurrency.py
 src/inspect_ai/util/_context/logger.py
 src/inspect_ai/util/_context/resource.py
 src/inspect_ai/util/_context/subprocess.py
 tests/test_anthropic.py
-tests/test_cloudlfare.py
+tests/test_cloudflare.py
 tests/test_collapse_assistant_message.py
 tests/test_collapse_user_message.py
 tests/test_dataset.py
 tests/test_eval_log.py
 tests/test_examples.py
 tests/test_hf.py
 tests/test_images.py
@@ -288,14 +303,17 @@
 tests/test_stop_reason.py
 tests/test_subprocess.py
 tests/test_tools.py
 tests/utils.py
 tests/test_dataset/samples.csv
 tests/test_dataset/samples.json
 tests/test_dataset/samples.jsonl
+tests/test_eval_log/log_invalid.txt
+tests/test_eval_log/log_version_2.txt
+tests/test_eval_log/log_with_nan.txt
 tests/test_images/images.jsonl
 tests/test_task_list/__init__.py
 tests/test_task_list/attribs.ipynb
 tests/test_task_list/multiple.py
 tests/test_task_list/multiple_dir/_decoy2.py
 tests/test_task_list/multiple_dir/bar.py
 tests/test_task_list/multiple_dir/foo.py
@@ -307,14 +325,15 @@
 tests/test_task_list/recurse/folder2/first.py
 tests/test_task_list/recurse/folder2/.folder3/epsilon.py
 tools/vscode/.eslintrc.json
 tools/vscode/.gitignore
 tools/vscode/.vscode-test.mjs
 tools/vscode/.vscodeignore
 tools/vscode/.yarnrc
+tools/vscode/CHANGELOG.md
 tools/vscode/LICENSE
 tools/vscode/README.md
 tools/vscode/package.json
 tools/vscode/tsconfig.json
 tools/vscode/webpack.config.js
 tools/vscode/yarn.lock
 tools/vscode/.vscode/extensions.json
@@ -322,20 +341,22 @@
 tools/vscode/.vscode/settings.json
 tools/vscode/.vscode/tasks.json
 tools/vscode/assets/logo/inspect.png
 tools/vscode/assets/logo/inspect.svg
 tools/vscode/assets/templates/task.py.template
 tools/vscode/assets/www/codicon/codicon.css
 tools/vscode/assets/www/codicon/codicon.ttf
+tools/vscode/assets/www/view/view-overrides.css
 tools/vscode/src/extension.ts
-tools/vscode/src/components/debugger.ts
 tools/vscode/src/components/document.ts
 tools/vscode/src/components/error.ts
 tools/vscode/src/components/focus.ts
 tools/vscode/src/components/notebook.ts
+tools/vscode/src/components/symbol.ts
+tools/vscode/src/components/task.ts
 tools/vscode/src/components/templates.ts
 tools/vscode/src/components/webview.ts
 tools/vscode/src/core/appdirs.ts
 tools/vscode/src/core/command.ts
 tools/vscode/src/core/dispose.ts
 tools/vscode/src/core/env.ts
 tools/vscode/src/core/git.ts
```

### Comparing `inspect_ai-0.3.8/src/inspect_ai.egg-info/requires.txt` & `inspect_ai-0.3.9/src/inspect_ai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tests/test_collapse_assistant_message.py` & `inspect_ai-0.3.9/tests/test_collapse_assistant_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,12 +45,12 @@
     messages = [user_message_str, assistant_message_str, user_message_str]
     assert collapse_consecutive_assistant_messages(messages) == messages
 
     messages = [user_message_str, assistant_message_str, user_message_image_and_str]
     assert collapse_consecutive_assistant_messages(messages) == messages
 
 
-def test_collapse_consecutive_assistant_messages_consecutive_assistaht_messages(
+def test_collapse_consecutive_assistant_messages_consecutive_assistant_messages(
     assistant_message_str,
 ):
     messages = [assistant_message_str, assistant_message_str, assistant_message_str]
     assert len(collapse_consecutive_assistant_messages(messages)) == 1
```

### Comparing `inspect_ai-0.3.8/tests/test_collapse_user_message.py` & `inspect_ai-0.3.9/tests/test_collapse_user_message.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tests/test_dataset.py` & `inspect_ai-0.3.9/tests/test_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # test reading a dataset using default configuration
 @pytest.mark.parametrize("type,file", dataset_params)
 def test_dataset(type: Type[T_ds], file: str) -> None:
     dataset: Dataset = type.__call__(dataset_path(file))
     assert_sample(dataset[0])
 
 
-# test reading a dataset with an explcit fields specification
+# test reading a dataset with an explicit fields specification
 @pytest.mark.parametrize("type,file", dataset_params)
 def test_dataset_fields(type: Type[T_ds], file: str) -> None:
     dataset: Dataset = type.__call__(
         dataset_path(file), sample_fields=sample_field_spec
     )
     assert_sample(dataset[0])
```

### Comparing `inspect_ai-0.3.8/tests/test_hf.py` & `inspect_ai-0.3.9/tests/test_hf.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tests/test_images/images.jsonl` & `inspect_ai-0.3.9/tests/test_images/images.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tests/test_images.py` & `inspect_ai-0.3.9/tests/test_images.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 @skip_if_no_google
 def test_google_images():
     check_images("google/gemini-pro-vision")
 
 
 @skip_if_no_openai
 def test_openai_images():
-    check_images("opeanai/gpt-4")
+    check_images("openai/gpt-4")
 
 
 @skip_if_no_anthropic
 def test_anthropic_images():
     check_images("anthropic/claude-3-sonnet-20240229")
```

### Comparing `inspect_ai-0.3.8/tests/test_list_task.py` & `inspect_ai-0.3.9/tests/test_list_task.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from pathlib import Path
 from typing import Callable
 
-from inspect_ai._eval.list import list_tasks
-from inspect_ai._eval.task import TaskInfo
+from inspect_ai import TaskInfo, list_tasks
 
 TEST_TASKS_DIR = Path("tests/test_task_list")
 
 
 def list_test_tasks_dir(
     globs: list[str], filter: Callable[[TaskInfo], bool] | None = None
 ):
```

### Comparing `inspect_ai-0.3.8/tests/test_logprobs.py` & `inspect_ai-0.3.9/tests/test_logprobs.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tests/test_metric.py` & `inspect_ai-0.3.9/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tests/test_num_choices.py` & `inspect_ai-0.3.9/tests/test_num_choices.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tests/test_openai.py` & `inspect_ai-0.3.9/tests/test_openai.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tests/test_plan.py` & `inspect_ai-0.3.9/tests/test_plan.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tests/test_registry.py` & `inspect_ai-0.3.9/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tests/test_retry.py` & `inspect_ai-0.3.9/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tests/test_solver.py` & `inspect_ai-0.3.9/tests/test_solver.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import pytest
 from utils import skip_if_no_openai
 
 from inspect_ai import Task, eval
 from inspect_ai.dataset import Sample
 from inspect_ai.model import ChatMessageUser, ModelOutput, get_model
 from inspect_ai.scorer import match
 from inspect_ai.solver import (
@@ -63,7 +64,42 @@
     log = eval(task, model=model)[0]
     assert len(log.samples[0].messages) == 4
     assert log.samples[0].output.completion == "finished"
 
     log = eval(task, model=model, max_messages=2)[0]
     assert len(log.samples[0].messages) == 2
     assert log.samples[0].output.completion == "finished"
+
+
+def test_invalid_solvers_error():
+    def not_async():
+        def inner(state: TaskState, generate: Generate) -> TaskState:
+            return state
+
+        return inner
+
+    class NotCallable:
+        async def inner(self, state: TaskState, generate: Generate) -> TaskState:
+            return state
+
+    class NotAsyncCallable:
+        def __call__(self, state: TaskState, target: Generate) -> TaskState:
+            return state
+
+    for f in [not_async, NotCallable, NotAsyncCallable]:
+        with pytest.raises(TypeError):
+            solver(name=f.__name__)(f)()
+
+
+def test_valid_solvers_succeed():
+    def is_async():
+        async def inner(self, state: TaskState, generate: Generate) -> TaskState:
+            return state
+
+        return inner
+
+    class IsAsyncCallable:
+        async def __call__(self, state: TaskState, generate: Generate) -> TaskState:
+            return state
+
+    for f in [is_async, IsAsyncCallable]:
+        solver(name=f.__name__)(f)()
```

### Comparing `inspect_ai-0.3.8/tests/test_stop_reason.py` & `inspect_ai-0.3.9/tests/test_stop_reason.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tests/test_subprocess.py` & `inspect_ai-0.3.9/tests/test_subprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,30 +9,30 @@
 @pytest.mark.asyncio
 async def test_subprocess_execute():
     result = await subprocess(["python3", "-c", "print('foo')"])
     assert result.stdout.strip() == "foo"
 
 
 @pytest.mark.asyncio
-async def test_suprocess_fail():
+async def test_subprocess_fail():
     result = await subprocess(["python4"])
     assert result.success is False
 
 
 @pytest.mark.asyncio
-async def test_suprocess_stdin():
+async def test_subprocess_stdin():
     input = "tell me a story"
     result = await subprocess(
         ["python3", "-c", "import sys; print(sys.stdin.read())"], input=input
     )
     assert result.stdout.strip() == input
 
 
 @pytest.mark.asyncio
-async def test_suprocess_binary():
+async def test_subprocess_binary():
     input = "tell me a story".encode()
     result = await subprocess(
         ["python3", "-c", "import sys; print(sys.stdin.read())"],
         text=False,
         input=input,
     )
     assert result.stdout.decode().strip() == input.decode()
```

### Comparing `inspect_ai-0.3.8/tests/test_tools.py` & `inspect_ai-0.3.9/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tests/utils.py` & `inspect_ai-0.3.9/tests/utils.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/.eslintrc.json` & `inspect_ai-0.3.9/tools/vscode/.eslintrc.json`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/.vscode/launch.json` & `inspect_ai-0.3.9/tools/vscode/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/.vscode/settings.json` & `inspect_ai-0.3.9/tools/vscode/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/.vscode/tasks.json` & `inspect_ai-0.3.9/tools/vscode/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/LICENSE` & `inspect_ai-0.3.9/tools/vscode/LICENSE`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/README.md` & `inspect_ai-0.3.9/tools/vscode/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # inspect-vscode
 
 VS Code extension for the Inspect framework for large language model evaluations. This extension provides support for developing evaluations using Inspect, including:
 
 - Integrated viewer for evaluation log files
 - Panel to browse, run, and debug tasks in the workspace
-- Panel for editting Inspect `.env` file
+- Panel for editing Inspect `.env` file
 - Panel for configuring task CLI options and args
 - Commands and key-bindings for running tasks
 - Commands and key-bindings for debugging tasks
 
 ## Log Viewer
 
 The `inspect view` command is used to automatically display the log for tasks executed within the workspace (this behavior can be controlled with an option).
```

### Comparing `inspect_ai-0.3.8/tools/vscode/assets/logo/inspect.png` & `inspect_ai-0.3.9/tools/vscode/assets/logo/inspect.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/assets/logo/inspect.svg` & `inspect_ai-0.3.9/tools/vscode/assets/logo/inspect.svg`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/assets/www/codicon/codicon.css` & `inspect_ai-0.3.9/tools/vscode/assets/www/codicon/codicon.css`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/assets/www/codicon/codicon.ttf` & `inspect_ai-0.3.9/tools/vscode/assets/www/codicon/codicon.ttf`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/package.json` & `inspect_ai-0.3.9/tools/vscode/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9363324496465253%*

 * *Differences: {"'contributes'": "{'commands': {0: {'icon': '$(code-oss)'}}, 'views': {'inspect_ai-activity-bar': "*

 * *                  "{2: {'when': 'workspaceFolderCount != 0'}}}, 'viewsWelcome': {0: {'contents': "*

 * *                  "'The Inspect extension requires the inspect-ai package. Please install "*

 * *                  "with\\n\\n pip install --upgrade inspect-ai'}, 1: {'when': "*

 * *                  "'workspaceFolderCount != 0 && inspect_ai.task-outline-view.tasksLoaded && "*

 * *                  'inspect_ai.task-outline-vi […]*

```diff
@@ -20,14 +20,15 @@
     ],
     "contributes": {
         "commands": [
             {
                 "category": "Inspect",
                 "command": "inspect.showLogview",
                 "enablement": "workspaceFolderCount != 0",
+                "icon": "$(code-oss)",
                 "title": "Show Logs"
             },
             {
                 "category": "Inspect",
                 "command": "inspect.createTask",
                 "enablement": "workspaceFolderCount != 0",
                 "title": "Create Task"
@@ -233,14 +234,19 @@
                     "when": "view == inspect_ai.task-outline-view && config.inspect_ai.taskListView == 'tree'"
                 },
                 {
                     "command": "inspect.taskOutlineTree",
                     "when": "view == inspect_ai.task-outline-view && config.inspect_ai.taskListView == 'list'"
                 },
                 {
+                    "command": "inspect.showLogview",
+                    "group": "navigation",
+                    "when": "view == inspect_ai.task-outline-view"
+                },
+                {
                     "command": "inspect.debugConfigTask",
                     "group": "navigation",
                     "when": "view == inspect_ai.task-configuration && inspect_ai.activeTask"
                 },
                 {
                     "command": "inspect.runConfigTask",
                     "group": "navigation",
@@ -261,37 +267,37 @@
                     "name": "Task",
                     "type": "webview",
                     "when": "workspaceFolderCount != 0 && inspect_ai.task-outline-view.noInspect == false"
                 },
                 {
                     "id": "inspect_ai.task-outline-view",
                     "name": "Tasks",
-                    "when": "workspaceFolderCount != 0 && inspect_ai.task-outline-view.noInspect == false"
+                    "when": "workspaceFolderCount != 0"
                 }
             ]
         },
         "viewsContainers": {
             "activitybar": [
                 {
                     "icon": "assets/logo/inspect.svg",
                     "id": "inspect_ai-activity-bar",
                     "title": "Inspect"
                 }
             ]
         },
         "viewsWelcome": [
             {
-                "contents": "Inspect Package not Installed",
+                "contents": "The Inspect extension requires the inspect-ai package. Please install with\n\n pip install --upgrade inspect-ai",
                 "view": "inspect_ai.task-outline-view",
                 "when": "workspaceFolderCount != 0 && inspect_ai.task-outline-view.noInspect"
             },
             {
                 "contents": "No tasks were found for this workspace.\n[Create a Task](command:inspect.createTask)",
                 "view": "inspect_ai.task-outline-view",
-                "when": "workspaceFolderCount != 0 && inspect_ai.task-outline-view.tasksLoaded && inspect_ai.task-outline-view.noTasks"
+                "when": "workspaceFolderCount != 0 && inspect_ai.task-outline-view.tasksLoaded && inspect_ai.task-outline-view.noTasks && inspect_ai.task-outline-view.noInspect == false"
             }
         ]
     },
     "dependencies": {
         "@microsoft/fast-components": "^2.30.6",
         "@microsoft/fast-element": "^1.13.0",
         "@vscode/webview-ui-toolkit": "^1.4.0",
@@ -299,32 +305,32 @@
         "semver": "^7.6.0"
     },
     "description": "Extension for the Inspect large language model evaluation framework.",
     "devDependencies": {
         "@types/lodash": "^4.17.0",
         "@types/mocha": "^10.0.6",
         "@types/node": "18.x",
-        "@types/vscode": "^1.87.0",
+        "@types/vscode": "1.85",
         "@typescript-eslint/eslint-plugin": "^7.4.0",
         "@typescript-eslint/parser": "^7.4.0",
         "@vscode/test-cli": "^0.0.8",
         "@vscode/test-electron": "^2.3.9",
         "@vscode/vsce": "^2.26.1",
         "css-loader": "^7.1.1",
         "eslint": "^8.57.0",
         "global": "^4.4.0",
         "style-loader": "^4.0.0",
         "ts-loader": "^9.5.1",
         "typescript": "^5.3.3",
         "webpack": "^5.91.0",
         "webpack-cli": "^5.1.4"
     },
-    "displayName": "Inspect",
+    "displayName": "Inspect AI",
     "engines": {
-        "vscode": "^1.87.0"
+        "vscode": "^1.85.0"
     },
     "extensionDependencies": [
         "ms-python.python"
     ],
     "homepage": "https://ukgovernmentbeis.github.io/inspect_ai/",
     "icon": "assets/logo/inspect.png",
     "license": "MIT",
@@ -342,9 +348,9 @@
         "package": "webpack --mode production --devtool hidden-source-map",
         "pretest": "yarn run compile-tests && yarn run compile && yarn run lint",
         "test": "vscode-test",
         "vscode:prepublish": "yarn run package",
         "watch": "webpack --watch",
         "watch-tests": "tsc -p . -w --outDir out"
     },
-    "version": "0.3.6"
+    "version": "0.3.13"
 }
```

### Comparing `inspect_ai-0.3.8/tools/vscode/src/components/templates.ts` & `inspect_ai-0.3.9/tools/vscode/src/components/templates.ts`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/src/components/webview.ts` & `inspect_ai-0.3.9/tools/vscode/src/components/webview.ts`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/src/core/appdirs.ts` & `inspect_ai-0.3.9/tools/vscode/src/core/appdirs.ts`

 * *Files 9% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 }
 
 export function userRuntimeDir(appName: string) {
   switch (process.platform) {
     case "darwin":
       return darwinUserCacheDir(appName);
     case "win32":
-      return windowsUserDataDir(appName);
+      return windowsUserCacheDir(appName);
     case "linux":
     default:
       return xdgUserRuntimeDir(appName);
   }
 }
 
 function darwinUserDataDir(appName: string) {
@@ -92,47 +92,51 @@
 }
 
 function darwinUserCacheDir(appName: string) {
   return path.join(
     process.env.HOME || "",
     "Library",
     "Caches",
+    "TemporaryItems",
     appName,
   );
 }
 
 function xdgUserDataDir(appName: string) {
   const dataHome = process.env.XDG_DATA_HOME ||
-    path.join(process.env.HOME  || "", ".local", "share");
+    path.join(process.env.HOME || "", ".local", "share");
   return path.join(dataHome, appName);
 }
 
 function xdgUserConfigDir(appName: string) {
   const configHome = process.env.XDG_CONFIG_HOME ||
-    path.join(process.env.HOME  || "", ".config");
+    path.join(process.env.HOME || "", ".config");
   return path.join(configHome, appName);
 }
 
 function xdgUserCacheDir(appName: string) {
   const cacheHome = process.env.XDG_CACHE_HOME ||
-    path.join(process.env.HOME  || "", ".cache");
+    path.join(process.env.HOME || "", ".cache");
   return path.join(cacheHome, appName);
 }
 
 function xdgUserRuntimeDir(appName: string) {
   const runtimeDir = process.env.XDG_RUNTIME_DIR;
   if (runtimeDir) {
-    return runtimeDir;
+    return path.join(runtimeDir, appName);
   } else {
     return xdgUserDataDir(appName);
   }
 }
 
 function windowsUserDataDir(appName: string, roaming = false) {
   const dir =
     (roaming ? process.env.APPDATA : process.env.LOCALAPPDATA) || "";
   return path.join(dir, appName);
 }
 
-
+function windowsUserCacheDir(appName: string) {
+  const dir = process.env.LOCALAPPDATA || "";
+  return path.join(dir, "Temp", appName, appName);
+}
```

### Comparing `inspect_ai-0.3.8/tools/vscode/src/core/command.ts` & `inspect_ai-0.3.9/tools/vscode/src/core/command.ts`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/src/core/dispose.ts` & `inspect_ai-0.3.9/tools/vscode/src/core/dispose.ts`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/src/core/env.ts` & `inspect_ai-0.3.9/tools/vscode/src/core/env.ts`

 * *Files 2% similar despite different names*

```diff
@@ -72,30 +72,29 @@
   if (eqIdx < 0) {
     return undefined;
   }
 
   const key = trimmed.substring(0, eqIdx).trim();
   let value = trimmed.substring(eqIdx + 1).trim();
 
-  ["'", "'"].forEach((quote) => {
+  ["'", '"'].forEach((quote) => {
     if (value.startsWith(quote) && value.endsWith(quote)) {
       value = value.substring(quote.length, value.length - quote.length);
     }
   });
 
   return { key, value };
 }
 
 function readEnvLines(file: Uri) {
   const envRaw = readFileSync(file.fsPath, { encoding: "utf-8" });
   return lines(envRaw);
 }
 
 function toLine(key: string, value: string) {
-  const needsQuote = [" ", "'", "\""].some((char) => {
+  const needsQuote = [" ", "'", '"'].some((char) => {
     return value.indexOf(char) > -1;
   });
 
-  const quoteChar =
-    !needsQuote ? "" : value.indexOf('"') > -1 ? "'" : '"';
+  const quoteChar = !needsQuote ? "" : value.indexOf('"') > -1 ? "'" : '"';
   return `${key}=${quoteChar}${value}${quoteChar}`;
 }
```

### Comparing `inspect_ai-0.3.8/tools/vscode/src/core/git.ts` & `inspect_ai-0.3.9/tools/vscode/src/core/git.ts`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/src/core/jsonrpc.ts` & `inspect_ai-0.3.9/tools/vscode/src/core/jsonrpc.ts`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/src/core/path.ts` & `inspect_ai-0.3.9/tools/vscode/src/core/path.ts`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/src/core/port.ts` & `inspect_ai-0.3.9/tools/vscode/src/core/port.ts`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/src/core/process.ts` & `inspect_ai-0.3.9/tools/vscode/src/core/process.ts`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/src/core/python/code.ts` & `inspect_ai-0.3.9/tools/vscode/src/core/python/code.ts`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/src/core/python/interpreter.ts` & `inspect_ai-0.3.9/tools/vscode/src/core/python/interpreter.ts`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/src/core/random.ts` & `inspect_ai-0.3.9/tools/vscode/src/core/random.ts`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/src/extension.ts` & `inspect_ai-0.3.9/tools/vscode/src/extension.ts`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import { ExtensionContext, MessageItem, OutputChannel, window } from "vscode";
+import { ExtensionContext, MessageItem, window } from "vscode";
 
 import { CommandManager } from "./core/command";
 import { activateCodeLens } from "./providers/codelens/codelens-provider";
 import { activateLogview } from "./providers/logview/logview";
 import { LogViewFileWatcher } from "./providers/logview/logview-file-watcher";
 import { logviewTerminalLinkProvider } from "./providers/logview/logview-link-provider";
 import { InspectLogviewManager } from "./providers/logview/logview-manager";
@@ -17,16 +17,14 @@
 import { activateWorkspaceEnv } from "./providers/workspace/workspace-env-provider";
 import { initPythonInterpreter } from "./core/python";
 import { initInspectProps } from "./inspect";
 import { activateInspectManager } from "./providers/inspect/inspect-manager";
 import { checkActiveWorkspaceFolder } from "./core/workspace";
 import { inspectBinPath, inspectVersion } from "./inspect/props";
 
-export const kInspectViewOutputChannelName = "Inspect View";
-export const kInspectEnvironmentOutputChannelName = "Inspect Environment";
 const kInspectMinimumVersion = "0.3.8";
 
 // This method is called when your extension is activated
 // Your extension is activated the very first time the command is executed
 export async function activate(context: ExtensionContext) {
 
   // we don't activate anything if there is no workspace
@@ -48,18 +46,15 @@
   // Warn the user if they don't have a recent enough version
   void checkInspectVersion();
 
   // Activate the workspacestate manager
   const [stateCommands, stateManager] = activateWorkspaceState(context);
 
   // For now, create an output channel for env changes
-  const envOutputChannel = window.createOutputChannel(
-    kInspectEnvironmentOutputChannelName
-  );
-  const workspaceActivationResult = activateWorkspaceEnv(envOutputChannel);
+  const workspaceActivationResult = activateWorkspaceEnv();
   const [envComands, workspaceEnvManager] = workspaceActivationResult;
   context.subscriptions.push(workspaceEnvManager);
 
   // Initial the workspace
   await initializeWorkspace(stateManager);
 
   // Inspect Manager watches for changes to inspect binary
@@ -72,30 +67,25 @@
   // Activate a watcher which inspects the active document and determines
   // the active task (if any)
   const [taskCommands, activeTaskManager] = activateActiveTaskProvider(inspectEvalMgr, context);
 
   // Active the workspace manager to watch for tasks
   const workspaceTaskMgr = activateWorkspaceTaskProvider(inspectManager, context);
 
-  // Create the inspect view output channel
-  const viewOutputChannel = window.createOutputChannel(
-    kInspectViewOutputChannelName
-  );
-
   // Read the extension configuration
   const settingsMgr = new InspectSettingsManager(() => {
     // If settings have changed, see if we need to stop or start the file watcher
     if (logFileWatcher && !settingsMgr.getSettings().logViewAuto) {
       stopLogWatcher();
     } else if (
       !logFileWatcher &&
       settingsMgr.getSettings().logViewAuto &&
       inspectLogviewManager
     ) {
-      startLogWatcher(logviewWebviewManager, viewOutputChannel);
+      startLogWatcher(logviewWebviewManager);
     }
   });
 
   // Activate the log view
   const [logViewCommands, logviewWebviewManager] = activateLogview(
     inspectManager,
     settingsMgr,
@@ -119,15 +109,15 @@
   // Register the log view link provider
   window.registerTerminalLinkProvider(
     logviewTerminalLinkProvider(logviewWebviewManager)
   );
 
   // Activate the file watcher for this workspace
   if (settingsMgr.getSettings().logViewAuto) {
-    startLogWatcher(logviewWebviewManager, viewOutputChannel);
+    startLogWatcher(logviewWebviewManager);
   }
 
   // Activate Code Lens
   activateCodeLens(context);
 
   // Activate commands
   [
@@ -150,19 +140,17 @@
 }
 
 // Log file watching
 let logFileWatcher: LogViewFileWatcher | undefined;
 
 const startLogWatcher = (
   logviewWebviewManager: InspectLogviewManager,
-  viewOutputChannel: OutputChannel
 ) => {
   logFileWatcher = new LogViewFileWatcher(
-    logviewWebviewManager,
-    viewOutputChannel
+    logviewWebviewManager
   );
 };
 
 const stopLogWatcher = () => {
   if (logFileWatcher) {
     logFileWatcher.dispose();
     logFileWatcher = undefined;
@@ -173,13 +161,13 @@
   if (inspectBinPath()) {
     const version = inspectVersion();
     if (version && version.compare(kInspectMinimumVersion) === -1) {
 
       const close: MessageItem = { title: "Close" };
       await window.showInformationMessage<MessageItem>(
         "The VS Code extension requires a newer version of Inspect. Please update " +
-        "with pip install —upgrade inspect-ai",
+        "with pip install --upgrade inspect-ai",
         close
       );
     }
   }
 };
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `inspect_ai-0.3.8/tools/vscode/src/inspect/list.ts` & `inspect_ai-0.3.9/tools/vscode/src/inspect/list.ts`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/src/inspect/logs.ts` & `inspect_ai-0.3.9/tools/vscode/src/inspect/logs.ts`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/src/inspect/props.ts` & `inspect_ai-0.3.9/tools/vscode/src/inspect/props.ts`

 * *Files 7% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 import { SemVer, coerce } from "semver";
 
 import { log } from "../core/log";
 import { pythonBinaryPath, pythonInterpreter } from "../core/python";
 import { AbsolutePath, toAbsolutePath } from "../core/path";
 import { Disposable } from "vscode";
 import { runProcess } from "../core/process";
+import { join } from "path";
+import { userRuntimeDir } from "../core/appdirs";
 
-
+const kPythonPackageName = "inspect_ai";
 
 // we cache the results of these functions so long as 
 // they (a) return success, and (b) the active python 
 // interpreter hasn't been changed
 class InspectPropsCache implements Disposable {
 
   private readonly eventHandle_: Disposable;
@@ -121,24 +123,22 @@
       }
     } else {
       return null;
     }
   }
 }
 
-
-
 export function inspectBinPath(): AbsolutePath | null {
   if (inspectPropsCache_.binPath) {
     return inspectPropsCache_.binPath;
   } else {
     const interpreter = pythonInterpreter();
-    if (interpreter.available && interpreter.pythonBinDir) {
+    if (interpreter.available) {
       try {
-        const binPath = pythonBinaryPath(interpreter.pythonBinDir, inspectFileName());
+        const binPath = pythonBinaryPath(interpreter, inspectFileName());
         if (binPath) {
           inspectPropsCache_.setBinPath(binPath);
         }
         return binPath;
       } catch (error) {
         log.error("Error attempting to read Inspect version.");
         log.error(error instanceof Error ? error : String(error));
@@ -146,14 +146,19 @@
       }
     } else {
       return null;
     }
   }
 }
 
+export function inspectLastEvalPath(): AbsolutePath | null {
+  const lastEvalFile = join(userRuntimeDir(kPythonPackageName), "view", "last-eval");
+  return toAbsolutePath(lastEvalFile);
+}
+
 function inspectFileName(): string {
   switch (process.platform) {
     case "darwin":
       return "inspect";
     case "win32":
       return "inspect.exe";
     case "linux":
```

### Comparing `inspect_ai-0.3.8/tools/vscode/src/providers/active-task/active-task-command.ts` & `inspect_ai-0.3.9/tools/vscode/src/providers/active-task/active-task-command.ts`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/src/providers/active-task/active-task-provider.ts` & `inspect_ai-0.3.9/tools/vscode/src/providers/active-task/active-task-provider.ts`

 * *Files 12% similar despite different names*

```diff
@@ -1,216 +1,195 @@
 import {
-  DocumentSymbol,
   Event,
   EventEmitter,
   ExtensionContext,
   Position,
-  Range,
   Selection,
-  SymbolKind,
   TextDocument,
   Uri,
   commands,
   window,
+  workspace,
+
 } from "vscode";
-import { sleep } from "../../core/wait";
 import {
   DebugActiveTaskCommand,
   RunActiveTaskCommand,
 } from "./active-task-command";
 import { InspectEvalManager } from "../inspect/inspect-eval";
 import { Command } from "../../core/command";
+import { DocumentTaskInfo, readTaskData } from "../../components/task";
+import { cellTasks, isNotebook } from "../../components/notebook";
 
-// Activates the provider which tracks the curently active task (document and task name)
+// Activates the provider which tracks the currently active task (document and task name)
 export function activateActiveTaskProvider(
   inspectEvalManager: InspectEvalManager,
   context: ExtensionContext
 ): [Command[], ActiveTaskManager] {
   const activeTaskManager = new ActiveTaskManager(context);
 
   const commands = [
     new RunActiveTaskCommand(activeTaskManager, inspectEvalManager),
     new DebugActiveTaskCommand(activeTaskManager, inspectEvalManager),
   ];
   return [commands, activeTaskManager];
 }
 
-// Task information for a document
-export interface ActiveTaskInfo {
-  document: Uri;
-  tasks: TaskData[];
-  activeTask?: TaskData;
-}
-
-// Describes the current active task
-export interface TaskData {
-  name: string;
-  params: string[];
-}
-
 // Fired when the active task changes
 export interface ActiveTaskChangedEvent {
-  activeTaskInfo?: ActiveTaskInfo;
+  activeTaskInfo?: DocumentTaskInfo;
 }
 
 // Tracks task information for the current editor
 export class ActiveTaskManager {
   constructor(context: ExtensionContext) {
-    // Listen for the editor changing and udpate task state
+    // Listen for the editor changing and update task state
     // when there is a new selection
     context.subscriptions.push(
       window.onDidChangeTextEditorSelection(async (event) => {
-        await this.updateActiveTask(
+        await this.updateActiveTaskWithDocument(
           event.textEditor.document,
           event.selections[0]
         );
       })
     );
 
+    context.subscriptions.push(
+      window.onDidChangeActiveNotebookEditor(async (event) => {
+        if (window.activeNotebookEditor?.selection.start) {
+          const cell = event?.notebook.cellAt(window.activeNotebookEditor.selection.start);
+          await this.updateActiveTaskWithDocument(
+            cell?.document,
+            new Selection(new Position(0, 0), new Position(0, 0))
+          );
+        }
+      })
+    );
+
     context.subscriptions.push(window.onDidChangeActiveTextEditor(async (event) => {
       if (event) {
-        await this.updateActiveTask(
+        await this.updateActiveTaskWithDocument(
           event.document
         );
       }
     }));
   }
-  private activeTaskInfo_: ActiveTaskInfo | undefined;
+  private activeTaskInfo_: DocumentTaskInfo | undefined;
   private readonly onActiveTaskChanged_ = new EventEmitter<ActiveTaskChangedEvent>();
 
   // Event to be notified when task information changes
   public readonly onActiveTaskChanged: Event<ActiveTaskChangedEvent> = this.onActiveTaskChanged_.event;
 
   // Get the task information for the current selection
-  public getActiveTaskInfo(): ActiveTaskInfo | undefined {
+  public getActiveTaskInfo(): DocumentTaskInfo | undefined {
     return this.activeTaskInfo_;
   }
 
   // Refresh the task information for the current editor
   public async refresh() {
     const currentSelection = window.activeTextEditor?.selection;
     const currentDocument = window.activeTextEditor?.document;
-    await this.updateActiveTask(currentDocument, currentSelection);
+    await this.updateActiveTaskWithDocument(currentDocument, currentSelection);
   }
 
-  async updateActiveTask(document?: TextDocument, selection?: Selection) {
+  private async updateTask(activeTaskInfo?: DocumentTaskInfo) {
     let taskActive = false;
+    if (activeTaskInfo) {
+      this.setActiveTaskInfo(activeTaskInfo);
+      taskActive = activeTaskInfo !== undefined;
+    }
+    await commands.executeCommand(
+      "setContext",
+      "inspect_ai.activeTask",
+      taskActive
+    );
+  }
+
+  async updateActiveTaskWithDocument(document?: TextDocument, selection?: Selection) {
     if (document && selection) {
-      if (document.languageId === "python") {
-        const activeTaskInfo = await getTaskInfo(document, selection);
-        this.setActiveTaskInfo(activeTaskInfo);
-        taskActive = activeTaskInfo !== undefined;
+      const activeTaskInfo = document.languageId === "python" ? getTaskInfoFromDocument(document, selection) : undefined;
+      await this.updateTask(activeTaskInfo);
+    }
+  }
+
+  async updateActiveTask(documentUri: Uri, task: string) {
+    if (isNotebook(documentUri)) {
+      // Compute the cell and position of the task
+      const notebookDocument = await workspace.openNotebookDocument(documentUri);
+      const cells = cellTasks(notebookDocument);
+      const cellTask = cells.find((c) => {
+        return c.tasks.find((t) => { return t.name === task; });
+      });
+      if (cellTask) {
+        const cell = notebookDocument.cellAt(cellTask?.cellIndex);
+        const taskInfo = getTaskInfo(cell.document, task);
+        await this.updateTask(taskInfo);
       }
-      await commands.executeCommand(
-        "setContext",
-        "inspect_ai.activeTask",
-        taskActive
-      );
+    } else {
+      const document = await workspace.openTextDocument(documentUri);
+      const taskInfo = getTaskInfo(document, task);
+      await this.updateTask(taskInfo);
     }
   }
 
   // Set the task information
-  setActiveTaskInfo(task?: ActiveTaskInfo) {
+  setActiveTaskInfo(task?: DocumentTaskInfo) {
     if (this.activeTaskInfo_ !== task) {
       this.activeTaskInfo_ = task;
       this.onActiveTaskChanged_.fire({ activeTaskInfo: this.activeTaskInfo_ });
     }
   }
 }
 
-async function getTaskInfo(
+function getTaskInfoFromDocument(
   document: TextDocument,
-  selection: Selection
-): Promise<ActiveTaskInfo | undefined> {
+  selection?: Selection
+): DocumentTaskInfo | undefined {
   // Try to get symbols to read task info for this document
   // Note that the retry is here since the symbol provider
   // has latency in loading and there wasn't a way to wait
   // on it specifically (waiting on the Python extension didn't work)
-  let symbols: DocumentSymbol[] | undefined;
-  let count = 0;
-  do {
-    symbols = await commands.executeCommand<DocumentSymbol[]>(
-      "vscode.executeDocumentSymbolProvider",
-      document.uri
-    );
-    count++;
-    await sleep(500);
-  } while (count <= 5 && !symbols);
-
-  if (symbols) {
-    const functionSymbols = symbols.filter(
-      (symbol) => symbol.kind === SymbolKind.Function
-    );
+  const tasks = readTaskData(document);
 
-    const tasks: TaskData[] = [];
-    let activeTask = undefined;
+  // If there are no tasks in this document, return undefined
+  if (tasks.length === 0) {
+    return undefined;
+  }
 
-    if (functionSymbols) {
-      functionSymbols.forEach((symbol) => {
-        if (isTask(document, symbol)) {
-          const signatureRange = getSignatureRange(document, symbol);
 
-          const variables = symbol.children.filter(
-            (child) => child.kind === SymbolKind.Variable
-          );
-          const params = variables
-            .filter((variable) => {
-              return signatureRange?.contains(variable.range);
-            })
-            .map((variable) => variable.name);
-
-          const task = {
-            name: symbol.name,
-            params,
-          };
-          tasks.push(task);
-
-          if (symbol.range.contains(selection.start)) {
-            activeTask = task;
-          }
-        }
-      });
-    }
+  const selectionLine = selection?.start.line || 0;
 
-    // If there are tasks in this file, just consider the first task active
-    if (tasks.length > 0 && !activeTask) {
-      activeTask = tasks[0];
-    }
+  // Find the first task that appears before the selection
+  // or otherwise the first task
 
-    return {
-      document: document.uri,
-      tasks,
-      activeTask,
-    };
-  }
+  const activeTask = [...tasks].reverse().find((task) => {
+    return task.line <= selectionLine;
+  });
+  return {
+    document: document.uri,
+    tasks,
+    activeTask: activeTask || (tasks.length > 0 ? tasks[0] : undefined)
+  };
 }
 
-function isTask(document: TextDocument, symbol: DocumentSymbol) {
-  const functionText = document.getText(symbol.range);
-  if (functionText.startsWith("@task")) {
-    return true;
-  }
-}
+function getTaskInfo(
+  document: TextDocument,
+  task: string
+): DocumentTaskInfo | undefined {
+  // Try to get symbols to read task info for this document
+  // Note that the retry is here since the symbol provider
+  // has latency in loading and there wasn't a way to wait
+  // on it specifically (waiting on the Python extension didn't work)
+  const tasks = readTaskData(document);
 
-function getSignatureRange(document: TextDocument, symbol: DocumentSymbol) {
-  const functionText = document.getText(symbol.range);
+  // Find the first task that appears before the selection
+  // or otherwise the first task
 
-  // Split the text into lines to process it line-by-line
-  const lines = functionText.split("\n");
-  for (let i = 0; i < lines.length; i++) {
-    const line = lines[i];
-    if (line.trim().startsWith("def") && line.trim().endsWith(":")) {
-      // Calculate the end position of the function definition line
-      const startLine = symbol.range.start.line + i;
-      const endLine = startLine;
-
-      // End at the end of the definition line
-      const endCharacter = line.length;
-
-      // Create a new range for just the definition
-      return new Range(
-        new Position(startLine, 0),
-        new Position(endLine, endCharacter)
-      );
-    }
-  }
-}
+  const activeTask = [...tasks].reverse().find((t) => {
+    return t.name === task;
+  });
+  return {
+    document: document.uri,
+    tasks,
+    activeTask: activeTask || (tasks.length > 0 ? tasks[0] : undefined)
+  };
+}
```

### Comparing `inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/activity-bar-provider.ts` & `inspect_ai-0.3.9/tools/vscode/src/providers/activity-bar/activity-bar-provider.ts`

 * *Files 0% similar despite different names*

```diff
@@ -26,17 +26,17 @@
   context.subscriptions.push(treeDataProvider);
 
   const envProvider = new EnvConfigurationProvider(context.extensionUri, workspaceEnvMgr, workspaceStateMgr, inspectManager);
   context.subscriptions.push(
     window.registerWebviewViewProvider(EnvConfigurationProvider.viewType, envProvider)
   );
 
-  const taskConfigPRovider = new TaskConfigurationProvider(context.extensionUri, workspaceStateMgr, activeTaskManager, inspectManager);
+  const taskConfigProvider = new TaskConfigurationProvider(context.extensionUri, workspaceStateMgr, activeTaskManager, inspectManager);
   context.subscriptions.push(
-    window.registerWebviewViewProvider(TaskConfigurationProvider.viewType, taskConfigPRovider)
+    window.registerWebviewViewProvider(TaskConfigurationProvider.viewType, taskConfigProvider)
   );
   const taskConfigCommands = [
     new RunConfigTaskCommand(activeTaskManager, inspectEvalMgr),
     new DebugConfigTaskCommand(activeTaskManager, inspectEvalMgr),
   ];
 
   return [...outlineCommands, ...taskConfigCommands];
```

### Comparing `inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/env-config-provider.ts` & `inspect_ai-0.3.9/tools/vscode/src/providers/activity-bar/env-config-provider.ts`

 * *Files 16% similar despite different names*

```diff
@@ -39,14 +39,42 @@
   maxRetries?: string;
   timeout?: string;
   logDir?: string;
   logLevel?: string;
   modelBaseUrl?: string;
 }
 
+// A list of the auto-complete models and the minimum
+// version required in order to support the model
+const kInspectModels: Record<string, string> = {
+  "openai": "0.3.8",
+  "anthropic": "0.3.8",
+  "google": "0.3.8",
+  "mistral": "0.3.8",
+  "hf": "0.3.8",
+  "together": "0.3.8",
+  "bedrock": "0.3.8",
+  "ollama": "0.3.9",
+  "azureai": "0.3.8",
+  "cf": "0.3.8"
+};
+
+const inspectModels = () => {
+  const currentVersion = inspectVersion();
+  return Object.keys(kInspectModels).filter((key) => {
+    const ver = kInspectModels[key];
+    if (currentVersion !== null) {
+      return currentVersion.compare(ver) > -1;
+    } else {
+      return false;
+    }
+  });
+};
+
+
 export class EnvConfigurationProvider implements WebviewViewProvider {
   public static readonly viewType = "inspect_ai.env-configuration-view";
 
   constructor(
     private readonly extensionUri_: Uri,
     private readonly envManager_: WorkspaceEnvManager,
     private readonly stateManager_: WorkspaceStateManager,
@@ -74,17 +102,49 @@
               await noInspectMsg();
             } else {
               await initMsg();
             }
             break;
           }
           case "setEnvValue":
-            setConfiguration(data.default, data.value, this.env);
-            this.envManager_.setValues(configToEnv(this.env));
-            break;
+            {
+              // Set the value
+              setConfiguration(data.default, data.value, this.env);
+
+              // Special case for provider, potentially restoring the 
+              // previously used model
+              let updateWebview = false;
+              if (data.default === "provider") {
+                const modelState = this.stateManager_.getModelState(data.value);
+                setConfiguration("model", modelState.lastModel || "", this.env);
+                updateWebview = true;
+              }
+
+              // Save the most recently used model for this provider
+              if (this.env.provider && data.default === "model") {
+                const modelState = this.stateManager_.getModelState(this.env.provider);
+                modelState.lastModel = data.value;
+                await this.stateManager_.setModelState(this.env.provider, modelState);
+              }
+
+              // Save the env
+              this.envManager_.setValues(configToEnv(this.env));
+
+
+              if (updateWebview) {
+                await webviewView.webview.postMessage({
+                  type: kEnvChanged,
+                  message: {
+                    env: this.env,
+                  },
+                });
+              }
+
+              break;
+            }
           case "openUrl":
             await env.openExternal(Uri.parse(data.url));
             break;
         }
       }
     );
 
@@ -164,14 +224,18 @@
         "codicon.ttf"
       )
     );
 
     // Use a nonce to only allow a specific script to be run.
     const nonce = getNonce();
 
+    const modelOptions = inspectModels().map((model) => {
+      return `<fast-option value="${model}">${model}</fast-option>`;
+    });
+
     return `<!DOCTYPE html>
               <html lang="en">
               <head>
                   <meta charset="UTF-8">
   
                   <!--
                       Use a content security policy to only allow loading styles from our extension directory,
@@ -202,23 +266,15 @@
 
                     <div class="group rows full-width" >
                       <div class="dropdown-container full-width">
                         <label id="provider-label" for="provider">Model</label>
                         <div class="cols full-width no-wrap">
                           <fast-combobox autocomplete="both" id="provider" placeholder="Provider">
                             <fast-option value="">None</fast-option>
-                            <fast-option value="openai">OpenAI</fast-option>
-                            <fast-option value="anthropic">Anthropic</fast-option>
-                            <fast-option value="google">Google</fast-option>
-                            <fast-option value="mistral">Mistral</fast-option>
-                            <fast-option value="hf">Hugging Face</fast-option>
-                            <fast-option value="together">TogetherAI</fast-option>
-                            <fast-option value="bedrock">AWS Bedrock</fast-option>
-                            <fast-option value="azureai">Azure AI</fast-option>
-                            <fast-option value="cf">CloudFlare</fast-option>
+                            ${modelOptions.join("\n")}
                           </fast>
                         </div>
                       </div>
                       <div id="model-container">  
                         <vscode-text-field placeholder="Model Name" id="model"></vscode-text-field>
                       </div>
                       <div id="show-base-url-container">
```

### Comparing `inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/task-config-commands.ts` & `inspect_ai-0.3.9/tools/vscode/src/providers/activity-bar/task-config-commands.ts`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/task-config-provider.ts` & `inspect_ai-0.3.9/tools/vscode/src/providers/activity-bar/task-config-provider.ts`

 * *Files 3% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 import { getNonce } from "../../core/nonce";
 import {
   DocumentState,
   WorkspaceStateManager,
 } from "../workspace/workspace-state-provider";
 import {
   ActiveTaskChangedEvent,
-  ActiveTaskInfo,
   ActiveTaskManager,
 } from "../active-task/active-task-provider";
 import { basename } from "path";
 import { inspectVersion } from "../../inspect";
 import { InspectManager } from "../inspect/inspect-manager";
+import { DocumentTaskInfo } from "../../components/task";
 
 export type SetActiveTaskCommand = {
   type: "setActiveTask";
-  task: ActiveTaskInfo;
+  task: DocumentTaskInfo;
   state: DocumentState;
 } & Record<string, unknown>;
 
 export type SetStateCmd = {
   command: "setStateValue";
   key: string;
   value: string;
@@ -70,14 +70,22 @@
 
     const initMsg = async () => {
       await webviewView.webview.postMessage({
         type: "initialize",
       });
     };
 
+    const updateTaskInfo = async (activeTaskInfo?: DocumentTaskInfo) => {
+      if (activeTaskInfo) {
+        await postActiveTaskMsg(activeTaskInfo);
+      } else {
+        webviewView.description = "";
+      }
+    };
+
     this.disposables_.push(
       this.taskManager_.onActiveTaskChanged(
         async (e: ActiveTaskChangedEvent) => {
           await updateSidebarState(e.activeTaskInfo);
         }
       )
     );
@@ -90,25 +98,24 @@
       } else {
         await noInspectMsg();
       }
     }));
 
     this.disposables_.push(webviewView.onDidChangeVisibility(async () => {
       const activeTask = this.taskManager_.getActiveTaskInfo();
-      if (activeTask) {
-        await postActiveTaskMsg(activeTask);
-      }
+      await updateTaskInfo(activeTask);
     }));
 
     webviewView.webview.html = this.htmlForWebview(webviewView.webview);
     webviewView.title = "Task";
 
     await initMsg();
 
-    const postActiveTaskMsg = async (activeTaskInfo: ActiveTaskInfo) => {
+
+    const postActiveTaskMsg = async (activeTaskInfo: DocumentTaskInfo) => {
       // Ignore active task changes that don't include a task (e.g. they are files)
       if (
         !activeTaskInfo.activeTask ||
         inspectVersion() === null
       ) {
         return;
       }
@@ -126,27 +133,24 @@
         activeTaskInfo.activeTask?.name ||
         basename(activeTaskInfo.document.fsPath);
     };
 
     this.disposables_.push(
       this.taskManager_.onActiveTaskChanged(async (e) => {
         await updateSidebarState(e.activeTaskInfo);
-        if (e.activeTaskInfo) {
-          await postActiveTaskMsg(e.activeTaskInfo);
-        }
+        await updateTaskInfo(e.activeTaskInfo);
       })
     );
 
     if (inspectVersion() === null) {
       await noInspectMsg();
     }
+
     const activeTask = this.taskManager_.getActiveTaskInfo();
-    if (activeTask) {
-      await postActiveTaskMsg(activeTask);
-    }
+    await updateTaskInfo(activeTask);
 
     // Process UI messages
     webviewView.webview.onDidReceiveMessage(
       async (data: SetStateCmd | SetStateParamCmd) => {
         const activeTask = this.taskManager_.getActiveTaskInfo();
         if (activeTask) {
           const path = activeTask.document.fsPath;
@@ -283,14 +287,14 @@
             
               <script type="module" nonce="${nonce}" src="${scriptUri.toString()}"></script>
               </body>
               </html>`;
   }
 }
 
-const updateSidebarState = async (taskInfo?: ActiveTaskInfo) => {
+const updateSidebarState = async (taskInfo?: DocumentTaskInfo) => {
   await commands.executeCommand(
     "setContext",
     "inspect_ai.task-configuration.task-active",
     taskInfo !== undefined
   );
 };
```

### Comparing `inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/task-outline-commands.ts` & `inspect_ai-0.3.9/tools/vscode/src/providers/activity-bar/task-outline-commands.ts`

 * *Files 16% similar despite different names*

```diff
@@ -2,31 +2,41 @@
   TreeView,
   Uri,
   window,
   workspace,
   ConfigurationTarget,
   ExtensionContext,
   ViewColumn,
+  commands,
 } from "vscode";
 
 import { Command } from "../../core/command";
 import {
   TaskOutLineTreeDataProvider,
   TaskTreeItem,
 } from "./task-outline-provider";
 import { InspectEvalManager } from "../inspect/inspect-eval";
 import { pathExists, toAbsolutePath, workspacePath } from "../../core/path";
 import { writeFileSync } from "fs";
 
 import { readTemplate, templates } from "../../components/templates";
 import { isValidPythonFnName } from "../../core/python";
-import { documentHasTasks, taskRangeForDocument } from "../../components/document";
-import { isNotebook, taskRangeForNotebook } from "../../components/notebook";
+import {
+  documentHasTasks,
+  firstTaskRangeForDocument,
+  taskRangeForDocument,
+} from "../../components/document";
+import {
+  firstTaskRangeForNotebook,
+  isNotebook,
+  taskRangeForNotebook,
+} from "../../components/notebook";
 import { scheduleReturnFocus } from "../../components/focus";
 import { InspectLogviewManager } from "../logview/logview-manager";
+import { ActiveTaskManager } from "../active-task/active-task-provider";
 
 export class ShowTaskTree implements Command {
   constructor(private readonly provider_: TaskOutLineTreeDataProvider) { }
   async execute(): Promise<void> {
     await workspace
       .getConfiguration("inspect_ai")
       .update("taskListView", "tree", ConfigurationTarget.Global);
@@ -51,15 +61,19 @@
 export class RunSelectedEvalCommand implements Command {
   constructor(private readonly inspectEvalMgr_: InspectEvalManager) { }
   async execute(treeItem: TaskTreeItem): Promise<void> {
     const path = treeItem.taskPath.path;
     const task =
       treeItem.taskPath.type === "task" ? treeItem.taskPath.name : undefined;
 
-    const evalPromise = this.inspectEvalMgr_.startEval(toAbsolutePath(path), task, false);
+    const evalPromise = this.inspectEvalMgr_.startEval(
+      toAbsolutePath(path),
+      task,
+      false
+    );
     const resumeFocusCommand = "inspect_ai.task-outline-view.focus";
     scheduleReturnFocus(resumeFocusCommand);
     await evalPromise;
   }
   private static readonly id = "inspect.runSelectedTask";
   public readonly id = RunSelectedEvalCommand.id;
 }
@@ -73,15 +87,19 @@
     await this.inspectEvalMgr_.startEval(toAbsolutePath(path), task, true);
   }
   private static readonly id = "inspect.debugSelectedTask";
   public readonly id = DebugSelectedEvalCommand.id;
 }
 
 export class EditSelectedTaskCommand implements Command {
-  constructor(private readonly tree_: TreeView<TaskTreeItem>, private inspectLogviewManager_: InspectLogviewManager) { }
+  constructor(
+    private readonly tree_: TreeView<TaskTreeItem>,
+    private inspectLogviewManager_: InspectLogviewManager,
+    private activeTaskManager_: ActiveTaskManager
+  ) { }
   async execute() {
     if (this.tree_.selection.length > 1) {
       throw new Error("Expected only a single selector for the task tree");
     }
 
     if (this.tree_.selection.length === 1) {
       const treeItem = this.tree_.selection[0];
@@ -90,37 +108,66 @@
       // If this is a folder, there is no edit action
       if (treeItem.taskPath.type === "folder") {
         return;
       }
 
       // If this is a specific task, go right to that
       const task =
-        treeItem.taskPath.type === "task" ? treeItem.taskPath.name : undefined;
+        treeItem.taskPath.type === "task" ? treeItem.taskPath.name : treeItem.taskPath.children?.[0].name;
 
       // Note if/where the logview is showing
       const logViewColumn = this.inspectLogviewManager_.viewColumn();
 
+      // Update the active task
+      if (task) {
+        await this.activeTaskManager_.updateActiveTask(fileUri, task);
+      }
+
       if (isNotebook(fileUri)) {
         // Compute the cell and position of the task
         const notebookDocument = await workspace.openNotebookDocument(fileUri);
-        const taskSelection = task
-          ? await taskRangeForNotebook(task, notebookDocument)
-          : undefined;
+
+        const findTaskSelection = (task: string | undefined) => {
+          if (task) {
+            return taskRangeForNotebook(task, notebookDocument);
+          } else {
+            return firstTaskRangeForNotebook(notebookDocument);
+          }
+        };
+        const taskSelection = findTaskSelection(task);
 
         // Open the notebook to the specified cell, if any
-        const selections = taskSelection?.cell ? [taskSelection?.cell] : undefined;
-        await window.showNotebookDocument(notebookDocument, { selections, preview: false, viewColumn: findTargetViewColumn(logViewColumn) });
+        const selections = taskSelection?.cell
+          ? [taskSelection?.cell]
+          : undefined;
+        await window.showNotebookDocument(notebookDocument, {
+          selections,
+          preview: false,
+          viewColumn: findTargetViewColumn(logViewColumn),
+        });
+        if (selections) {
+          await commands.executeCommand("notebook.cell.edit");
+        }
       } else {
         // Find the task selection for the document (if any)
-        const taskSelection = task
-          ? await taskRangeForDocument(task, fileUri)
-          : undefined;
+        const findTaskSelection = async (task: string | undefined) => {
+          if (task) {
+            return taskRangeForDocument(task, fileUri);
+          } else {
+            return await firstTaskRangeForDocument(fileUri);
+          }
+        };
+        const selection = await findTaskSelection(task);
 
         // Show the document
-        await window.showTextDocument(fileUri, { selection: taskSelection, viewColumn: findTargetViewColumn(logViewColumn), preview: false });
+        await window.showTextDocument(fileUri, {
+          selection,
+          viewColumn: findTargetViewColumn(logViewColumn),
+          preview: false,
+        });
       }
     }
   }
 
   public static readonly id = "inspect.editSelectedTask";
   public readonly id = EditSelectedTaskCommand.id;
 }
@@ -136,24 +183,24 @@
     const targetEditor = visibleEditors.find((editor) => {
       return documentHasTasks(editor.document);
     });
     if (targetEditor) {
       return targetEditor.viewColumn;
     }
 
-    // There are no editors with tasks, but if there is any active 
+    // There are no editors with tasks, but if there is any active
     // editor, let's use that
     if (visibleEditors.length > 0) {
       return visibleEditors[0].viewColumn;
     }
   }
 
   // If we get here, there are no editors open at all
   // so as a last ditch, just open next to the logview
-  // (if it showing) or in the first column 
+  // (if it showing) or in the first column
   // (who knows what it showing in this case)
   if (logViewColumn) {
     // The log view is open, but not any editors
     return ViewColumn.Beside;
   } else {
     // No idea, just go into the first column
     return ViewColumn.One;
@@ -175,15 +222,14 @@
           return `There is already a file in this workspace named '${input}'`;
         }
         return null;
       },
     });
 
     if (taskName) {
-
       // force the task name to lower case
       const taskNameLower = taskName.toLowerCase();
 
       // Read the new task template
       const content = await readTemplate(templates.python_task, this.context_, {
         taskName: taskNameLower,
       });
@@ -192,14 +238,13 @@
       const absPath = workspacePath(`${taskNameLower}.py`);
 
       writeFileSync(absPath.path, content, { encoding: "utf-8" });
 
       // Create empty document
       const document = await workspace.openTextDocument(absPath.path);
       await window.showTextDocument(document);
-
     }
   }
 
   private static readonly id = "inspect.createTask";
   public readonly id = CreateTaskCommand.id;
 }
```

### Comparing `inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/task-outline-provider.ts` & `inspect_ai-0.3.9/tools/vscode/src/providers/activity-bar/task-outline-provider.ts`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,15 @@
   workspace,
   ThemeIcon,
   commands,
   ExtensionContext,
   Disposable,
   TreeView,
   TreeViewVisibilityChangeEvent,
+  Uri,
 } from "vscode";
 import {
   RunSelectedEvalCommand,
   DebugSelectedEvalCommand,
   EditSelectedTaskCommand,
   ShowTaskList,
   ShowTaskTree,
@@ -28,21 +29,21 @@
 import {
   TaskPath,
   TasksChangedEvent,
   WorkspaceTaskManager,
 } from "../workspace/workspace-task-provider";
 import { basename, relative, sep } from "path";
 import {
-  ActiveTaskInfo,
   ActiveTaskManager,
 } from "../active-task/active-task-provider";
 import { throttle } from "lodash";
 import { inspectVersion } from "../../inspect";
 import { InspectManager } from "../inspect/inspect-manager";
 import { InspectLogviewManager } from "../logview/logview-manager";
+import { DocumentTaskInfo } from "../../components/task";
 
 // Activation function for the task outline
 export async function activateTaskOutline(
   context: ExtensionContext,
   inspectEvalMgr: InspectEvalManager,
   workspaceTaskMgr: WorkspaceTaskManager,
   activeTaskManager: ActiveTaskManager,
@@ -66,84 +67,118 @@
       treeDataProvider.refresh();
     } else {
       treeDataProvider.clear();
     }
   };
 
   // If the interpreter changes, refresh the tasks
-  context.subscriptions.push(inspectManager.onInspectChanged(async () => {
-    await checkInspect();
-  }));
+  context.subscriptions.push(
+    inspectManager.onInspectChanged(async () => {
+      await checkInspect();
+    })
+  );
   await checkInspect();
 
   const tree = window.createTreeView(TaskOutLineTreeDataProvider.viewType, {
     treeDataProvider,
     showCollapseAll: true,
     canSelectMany: false,
   });
 
-  // Activate task tracking
   context.subscriptions.push(
-    ...await activateTaskTracking(treeDataProvider, tree, activeTaskManager)
+    tree.onDidChangeVisibility(async (e: TreeViewVisibilityChangeEvent) => {
+      // If the tree becomes visible with nothing selected, try selecting
+      if (e.visible && tree.selection.length === 0) {
+        const activeTask = activeTaskManager.getActiveTaskInfo();
+        if (activeTask) {
+          await showTreeItem(treeDataProvider, tree, activeTask);
+        } else {
+          const first = await findFirstTask(treeDataProvider);
+          if (first) {
+            await activeTaskManager.updateActiveTask(Uri.file(first.taskPath.path), first.taskPath.name);
+          }
+        }
+      } else if (e.visible) {
+        // Tree just became visible, be sure selection matches the active task
+        await showTreeItem(
+          treeDataProvider,
+          tree,
+          activeTaskManager.getActiveTaskInfo()
+        );
+      }
+    })
   );
 
+  // Activate task tracking
+  context.subscriptions.push(
+    ...(await activateTaskTracking(treeDataProvider, tree, activeTaskManager))
+  );
 
   return [
     [
       new ShowTaskList(treeDataProvider),
       new ShowTaskTree(treeDataProvider),
       new RunSelectedEvalCommand(inspectEvalMgr),
       new DebugSelectedEvalCommand(inspectEvalMgr),
-      new EditSelectedTaskCommand(tree, inspectLogviewManager),
+      new EditSelectedTaskCommand(tree, inspectLogviewManager, activeTaskManager),
       new CreateTaskCommand(context),
     ],
     treeDataProvider,
   ];
 }
 
-
 const activateTaskTracking = async (
   treeDataProvider: TaskOutLineTreeDataProvider,
   tree: TreeView<TaskTreeItem>,
   activeTaskManager: ActiveTaskManager
 ) => {
-
-  const showTreeItem = async (activeTask?: ActiveTaskInfo) => {
-    if (!activeTask) {
-      return;
-    }
-
-    const treeItem = await findTreeItem(activeTask, treeDataProvider);
-    if (treeItem && treeItem.taskPath.type === "task") {
-      // Don't reveal the item if the tree isn't visible (this will force the
-      // activity bar containing the tree to become visible, which is very jarring)
-      if (tree.visible) {
-        await tree.reveal(treeItem, { select: true, focus: false });
-      }
-    }
-  };
-
   // Listen for changes to the active task and drive the tree to the item
   const activeTaskChanged = activeTaskManager.onActiveTaskChanged(async (e) => {
-    await showTreeItem(e.activeTaskInfo);
+    await showTreeItem(treeDataProvider, tree, e.activeTaskInfo);
   });
 
-  const treeVisibilityChanged = tree.onDidChangeVisibility(async (e: TreeViewVisibilityChangeEvent) => {
-    // Since we may have been ignoring activation events for tasks, when the tree reveals
-    // itself, ensure that we select the currently activate task, if any
-    if (e.visible) {
-      await showTreeItem(activeTaskManager.getActiveTaskInfo());
+  const currentlyActive = activeTaskManager.getActiveTaskInfo();
+  await showTreeItem(treeDataProvider, tree, currentlyActive);
+  return [activeTaskChanged];
+};
+
+const showTreeItem = async (
+  treeDataProvider: TaskOutLineTreeDataProvider,
+  tree: TreeView<TaskTreeItem>,
+  activeTask?: DocumentTaskInfo
+) => {
+  if (!activeTask) {
+    return;
+  }
+
+  const treeItem = await findTreeItem(activeTask, treeDataProvider);
+  if (treeItem && treeItem.taskPath.type === "task") {
+    // Don't reveal the item if the tree isn't visible (this will force the
+    // activity bar containing the tree to become visible, which is very jarring)
+    if (tree.visible) {
+      await tree.reveal(treeItem, { select: true, focus: false });
     }
-  });
+  }
+};
 
-  const currentlyActive = activeTaskManager.getActiveTaskInfo();
-  await showTreeItem(currentlyActive);
-  return [activeTaskChanged, treeVisibilityChanged];
+const findFirstTask = async (
+  treeDataProvider: TaskOutLineTreeDataProvider,
+  element?: TaskTreeItem
+): Promise<TaskTreeItem | undefined> => {
+  const children = await treeDataProvider.getChildren(element);
+  for (const child of children) {
+    if (child.taskPath.type === "task") {
+      return child;
+    } else {
+      return await findFirstTask(treeDataProvider, child);
+    }
+  }
 };
 
+
 // A tree item for a task, file, or folder
 export class TaskTreeItem extends TreeItem {
   constructor(
     public readonly taskPath: TaskPath,
     command?: VsCodeCommand,
     public readonly parent?: TaskTreeItem
   ) {
@@ -195,31 +230,36 @@
 export class TaskOutLineTreeDataProvider
   implements TreeDataProvider<TaskTreeItem>, Disposable {
   public static readonly viewType = "inspect_ai.task-outline-view";
   constructor(
     private readonly workspaceMgr: WorkspaceTaskManager,
     private readonly command_?: VsCodeCommand
   ) {
-
     this.disposables_.push(
-      this.workspaceMgr.onTasksChanged(throttle(async (e: TasksChangedEvent) => {
-        this.setTasks(e.tasks || []);
-        await commands.executeCommand(
-          "setContext",
-          "inspect_ai.task-outline-view.tasksLoaded",
-          true
-        );
-        await commands.executeCommand(
-          "setContext",
-          "inspect_ai.task-outline-view.noTasks",
-          e.tasks?.length === 0
-        );
-      }, 500, { leading: true, trailing: true })));
+      this.workspaceMgr.onTasksChanged(
+        throttle(
+          async (e: TasksChangedEvent) => {
+            this.setTasks(e.tasks || []);
+            await commands.executeCommand(
+              "setContext",
+              "inspect_ai.task-outline-view.tasksLoaded",
+              true
+            );
+            await commands.executeCommand(
+              "setContext",
+              "inspect_ai.task-outline-view.noTasks",
+              e.tasks?.length === 0
+            );
+          },
+          500,
+          { leading: true, trailing: true }
+        )
+      )
+    );
     this.workspaceMgr.refresh();
-
   }
   private disposables_: Disposable[] = [];
   dispose() {
     this.disposables_.forEach((disposable) => {
       disposable.dispose();
     });
   }
@@ -311,15 +351,15 @@
     return parts.join(" > ");
   }
 }
 
 // Find a task in the tree based upon its
 // path (e.g. document path and task name)
 async function findTreeItem(
-  activeTask: ActiveTaskInfo,
+  activeTask: DocumentTaskInfo,
   treeDataProvider: TaskOutLineTreeDataProvider
 ) {
   const filePath = activeTask.document.fsPath;
   const taskName = activeTask.activeTask?.name;
   const taskTreeItem = await findTask(filePath, treeDataProvider, taskName);
   if (taskTreeItem) {
     return taskTreeItem;
@@ -341,14 +381,16 @@
       taskEl = el;
     } else if (el.taskPath.type === "file" && filePath === el.taskPath.path) {
       if (taskName) {
         taskEl = await findTask(filePath, treeDataProvider, taskName, el);
       } else {
         taskEl = el;
       }
-      break;
     } else if (el.taskPath.type === "folder") {
       taskEl = await findTask(filePath, treeDataProvider, taskName, el);
     }
+    if (taskEl) {
+      return taskEl;
+    }
   }
   return taskEl;
 }
```

### Comparing `inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/webview/env-config-webview.css` & `inspect_ai-0.3.9/tools/vscode/src/providers/activity-bar/webview/env-config-webview.css`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/webview/env-config-webview.ts` & `inspect_ai-0.3.9/tools/vscode/src/providers/activity-bar/webview/env-config-webview.ts`

 * *Files 6% similar despite different names*

```diff
@@ -83,17 +83,15 @@
 
 function getProviderEl() {
   return document.getElementById("provider") as HTMLSelectElement;
 }
 
 function getProviderText() {
   const providerEl = getProviderEl();
-
-  const index = providerEl.selectedIndex;
-  return index > -1 ? providerEl.options[index].value : providerEl.value;
+  return providerEl.value;
 }
 
 function resetModel() {
   const modelEl = getModelEl();
   modelEl.value = "";
 }
 
@@ -153,27 +151,23 @@
   const providerChanged = (e: Event) => {
     // If the user chooses 'none' from the dropdown, this will fire
     const txt = getProviderText();
     if (txt === "") {
       getProviderEl().value = "";
     }
     if (e.target) {
-      const index = el.selectedIndex;
-      const value = index > -1 ? el.options[index].value : el.value;
-      setEnvValue("provider", value);
-      setEnvValue("model", "");
+      setEnvValue("provider", txt);
       resetModel();
       showProviderHelp();
     }
   }
 
   const el = document.getElementById("provider") as HTMLSelectElement;
 
   el.addEventListener("change", providerChanged);
-  el.addEventListener("keyup", debounce(providerChanged, kBounceInterval));
 
   setEnvWhenKeyup("model", "model");
 
   setEnvWhenKeyup("model-base-url", "modelBaseUrl");
 
   const showBaseUrlEl = document.getElementById("show-base-url") as HTMLAnchorElement;
   showBaseUrlEl.addEventListener("click", () => {
```

### Comparing `inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/webview/task-config-webview.ts` & `inspect_ai-0.3.9/tools/vscode/src/providers/activity-bar/webview/task-config-webview.ts`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/webview/vscode-controls.css` & `inspect_ai-0.3.9/tools/vscode/src/providers/activity-bar/webview/vscode-controls.css`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/src/providers/activity-bar/webview/webview-utils.ts` & `inspect_ai-0.3.9/tools/vscode/src/providers/activity-bar/webview/webview-utils.ts`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/src/providers/codelens/codelens-provider.ts` & `inspect_ai-0.3.9/tools/vscode/src/providers/codelens/codelens-provider.ts`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/src/providers/inspect/inspect-eval-commands.ts` & `inspect_ai-0.3.9/tools/vscode/src/providers/inspect/inspect-eval-commands.ts`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/src/providers/inspect/inspect-eval.ts` & `inspect_ai-0.3.9/tools/vscode/src/providers/inspect/inspect-eval.ts`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,41 @@
-import { window, workspace } from "vscode";
-import { findOpenPort } from "../../core/port";
-import { DebuggerManager } from "../../components/debugger";
+import { DebugConfiguration, debug, window, workspace } from "vscode";
 import { inspectEvalCommands } from "./inspect-eval-commands";
 import { Command } from "../../core/command";
-import { AbsolutePath, activeWorkspacePath, workspaceRelativePath } from "../../core/path";
+import {
+  AbsolutePath,
+  activeWorkspacePath,
+  workspaceRelativePath,
+} from "../../core/path";
 import { WorkspaceStateManager } from "../workspace/workspace-state-provider";
 import { inspectVersion } from "../../inspect";
+import { inspectBinPath } from "../../inspect/props";
+import { activeWorkspaceFolder } from "../../core/workspace";
+import { findOpenPort } from "../../core/port";
 
-
-const kDebugSessionName = "Inspect Eval";
-
-export function activateEvalManager(stateManager: WorkspaceStateManager): [Command[], InspectEvalManager] {
+export function activateEvalManager(
+  stateManager: WorkspaceStateManager
+): [Command[], InspectEvalManager] {
   const inspectEvalMgr = new InspectEvalManager(stateManager);
   return [inspectEvalCommands(inspectEvalMgr), inspectEvalMgr];
 }
 
 export class InspectEvalManager {
   constructor(private readonly stateManager_: WorkspaceStateManager) {
-    this.debuggerManager_ = new DebuggerManager(kDebugSessionName);
   }
-  private debuggerManager_: DebuggerManager;
 
   public async startEval(file: AbsolutePath, task?: string, debug = false) {
-
     // if we don't have inspect bail and let the user know
     if (!inspectVersion()) {
       await window.showWarningMessage(
-        `Unable to ${debug ? "Debug" : "Run"} Eval (Inspect Package Not Installed)`,
+        `Unable to ${debug ? "Debug" : "Run"
+        } Eval (Inspect Package Not Installed)`,
         {
           modal: true,
-          detail: "pip install --upgrade inspect-ai"
+          detail: "pip install --upgrade inspect-ai",
         }
       );
       return;
     }
 
     const workspaceDir = activeWorkspacePath();
     const relativePath = workspaceRelativePath(file);
@@ -43,15 +45,18 @@
     const args = ["eval", taskArg];
 
     // Read the document state to determine flags
     const docState = this.stateManager_.getTaskState(file.path, task);
 
     // Forward the various doc state args
     const limit = docState.limit;
-    if (debug === true && workspace.getConfiguration("inspect_ai").get("debugSingleSample")) {
+    if (
+      debug === true &&
+      workspace.getConfiguration("inspect_ai").get("debugSingleSample")
+    ) {
       args.push(...["--limit", "1"]);
     } else if (limit) {
       args.push(...["--limit", limit]);
     }
 
     const epochs = docState.epochs;
     if (epochs) {
@@ -83,40 +88,55 @@
     if (taskParams) {
       Object.keys(taskParams).forEach((key) => {
         const value = taskParams[key];
         args.push(...["-T", `${key}=${value}`]);
       });
     }
 
-    // Handle debugging
-    let debugPort = 5678;
-    if (debug === true) {
-      // Provision a port
-      debugPort = await findOpenPort(debugPort);
-
-      args.push("--debug");
-      args.push("--debug-port");
-      args.push(debugPort.toString());
-    }
-
-    // Run the command
-    runEvalCmd("inspect", args, workspaceDir.path);
-
-    // If we're debugging, attach the debugger
+    // If we're debugging, launch using the debugger
     if (debug) {
-      await this.debuggerManager_.attach(debugPort);
+
+      // Handle debugging
+      let debugPort = 5678;
+      if (debug === true) {
+        // Provision a port
+        debugPort = await findOpenPort(debugPort);
+
+        args.push("--debug-port");
+        args.push(debugPort.toString());
+      }
+
+      await runDebugger(inspectBinPath()?.path || "inspect", args, workspaceDir.path, debugPort);
+    } else {
+      // Run the command
+      runEvalCmd(args, workspaceDir.path);
     }
   }
 }
 
-const runEvalCmd = (cmd: string, args: string[], cwd: string) => {
+const runEvalCmd = (args: string[], cwd: string) => {
   // See if there a non-busy terminal that we can re-use
   const name = "Inspect Eval";
   let terminal = window.terminals.find((t) => {
     return t.name === name;
   });
   if (!terminal) {
     terminal = window.createTerminal({ name, cwd });
   }
   terminal.show();
-  terminal.sendText([cmd, ...args].join(" "));
+  terminal.sendText(["inspect", ...args].join(" "));
+};
+
+const runDebugger = async (program: string, args: string[], cwd: string, port: number) => {
+  const name = "Inspect Eval";
+  const debugConfiguration: DebugConfiguration = {
+    name,
+    type: "python",
+    request: "launch",
+    program,
+    args,
+    console: "internalConsole",
+    cwd,
+    port
+  };
+  await debug.startDebugging(activeWorkspaceFolder(), debugConfiguration);
 };
```

### Comparing `inspect_ai-0.3.8/tools/vscode/src/providers/logview/commands.ts` & `inspect_ai-0.3.9/tools/vscode/src/providers/logview/commands.ts`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/src/providers/logview/logview-link-provider.ts` & `inspect_ai-0.3.9/tools/vscode/src/providers/logview/logview-link-provider.ts`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/src/providers/logview/logview-manager.ts` & `inspect_ai-0.3.9/tools/vscode/src/providers/logview/logview-manager.ts`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/src/providers/logview/logview-webview.ts` & `inspect_ai-0.3.9/tools/vscode/src/providers/logview/logview-webview.ts`

 * *Files 12% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
   protected override onViewStateChanged(): void {
     this.updatePreview(this.lastState_).catch(() => { });
   }
 
   private async updatePreview(state?: LogviewState) {
     if (this.isVisible()) {
-      // see if there is an explcit state update (otherwise inspect hte active editor)
+      // see if there is an explicit state update (otherwise inspect the active editor)
       if (state) {
         await this.updateViewState(state);
       } else {
         await this.updateViewState({});
       }
     }
   }
@@ -123,20 +123,20 @@
             }
             break;
         }
       })
     );
 
 
-    const disconnecct = webviewPanelJsonRpcServer(this._webviewPanel, {
+    const disconnect = webviewPanelJsonRpcServer(this._webviewPanel, {
       [kMethodEvalLogs]: evalLogs,
       [kMethodEvalLog]: (params: unknown[]) => evalLog(params[0] as string, params[1] as boolean),
       [kMethodEvalLogHeaders]: (params: unknown[]) => evalLogHeaders(params[0] as string[])
     });
-    this._register(new Disposable(disconnecct));
+    this._register(new Disposable(disconnect));
 
   }
 
 
 
   public async update(state: LogviewState) {
     await this._webviewPanel.webview.postMessage({
@@ -156,20 +156,28 @@
 
       // file uri for view dir
       const viewDirUri = Uri.file(viewDir.path);
 
       // get base html
       let indexHtml = readFileSync(viewDir.child("index.html").path, "utf-8");
 
+      // Add a stylesheet to further customize the view appearance
+      const overrideCssPath = this.extensionResourceUrl(["assets",
+        "www",
+        "view",
+        "view-overrides.css"]);
+
+
       // add content security policy
       indexHtml = indexHtml.replace("<head>\n", `<head>
     <meta http-equiv="Content-Security-Policy" content="default-src 'none'; img-src ${this._webviewPanel.webview.cspSource} data:; font-src ${this._webviewPanel.webview.cspSource}; style-src ${this._webviewPanel.webview.cspSource} 'unsafe-inline'; script-src 'nonce-${nonce}';">
-  `);
+    <link rel="stylesheet" type ="text/css" href="${overrideCssPath.toString()}" >
+    `);
 
-      // funtion to resolve resource uri
+      // function to resolve resource uri
       const resourceUri = (path: string) => this._webviewPanel.webview.asWebviewUri(
         Uri.joinPath(viewDirUri, path)
       ).toString();
 
       // fixup css references
       indexHtml = indexHtml.replace(/href="\.([^"]+)"/g, (_, p1: string) => {
         return `href="${resourceUri(p1)}"`;
```

### Comparing `inspect_ai-0.3.8/tools/vscode/src/providers/logview/logview.ts` & `inspect_ai-0.3.9/tools/vscode/src/providers/logview/logview.ts`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/src/providers/settings/inspect-settings.ts` & `inspect_ai-0.3.9/tools/vscode/src/providers/settings/inspect-settings.ts`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/src/providers/settings/user-settings.ts` & `inspect_ai-0.3.9/tools/vscode/src/providers/settings/user-settings.ts`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/src/providers/workspace/workspace-env-commands.ts` & `inspect_ai-0.3.9/tools/vscode/src/providers/workspace/workspace-env-commands.ts`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   constructor() { }
   async execute(): Promise<void> {
 
     // The path to the env file
     const absPath = workspacePath(`.env`);
 
 
-    // Ensure env file actuall exists
+    // Ensure env file actually exists
     if (!existsSync(absPath.path)) {
       writeFileSync(absPath.path,
         "",
         { encoding: "utf-8" }
       );
     }
```

### Comparing `inspect_ai-0.3.8/tools/vscode/src/providers/workspace/workspace-init.ts` & `inspect_ai-0.3.9/tools/vscode/src/providers/workspace/workspace-init.ts`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/src/providers/workspace/workspace-state-provider.ts` & `inspect_ai-0.3.9/tools/vscode/src/providers/workspace/workspace-state-provider.ts`

 * *Files 11% similar despite different names*

```diff
@@ -14,14 +14,18 @@
   temperature?: string;
   topP?: string;
   topK?: string;
   maxTokens?: string;
   params?: Record<string, string>;
 }
 
+export interface ModelState {
+  lastModel?: string;
+}
+
 export class WorkspaceStateManager {
   constructor(private readonly context_: ExtensionContext) {
   }
 
   public getState(key: string) {
     return this.context_.workspaceState.get(key);
   }
@@ -33,17 +37,29 @@
   public getTaskState(taskFilePath: string, taskName?: string): DocumentState {
     return this.context_.workspaceState.get(taskKey(taskFilePath, taskName)) || {};
   }
 
   public async setTaskState(taskFilePath: string, state: DocumentState, taskName?: string) {
     await this.context_.workspaceState.update(taskKey(taskFilePath, taskName), state);
   }
+
+  public getModelState(provider: string): ModelState {
+    return this.context_.workspaceState.get(modelKey(provider)) || {};
+  }
+
+  public async setModelState(provider: string, state: ModelState) {
+    await this.context_.workspaceState.update(modelKey(provider), state);
+  }
 }
 
 function taskKey(file: string, task?: string) {
   if (task) {
     return `${file}@${task}`;
   } else {
     return `${file}`;
   }
 }
 
+function modelKey(provider: string) {
+  return `provider-${provider}`;
+}
+
```

### Comparing `inspect_ai-0.3.8/tools/vscode/src/providers/workspace/workspace-task-provider.ts` & `inspect_ai-0.3.9/tools/vscode/src/providers/workspace/workspace-task-provider.ts`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import { AbsolutePath, activeWorkspacePath } from "../../core/path";
 import { inspectListTasks } from "../../inspect/list";
 import { Event, EventEmitter, ExtensionContext, FileSystemWatcher, workspace } from "vscode";
 
 import { throttle } from "lodash";
 import { InspectChangedEvent, InspectManager } from "../inspect/inspect-manager";
 
-// Activates the provider which tracks the curently active task (document and task name)
+// Activates the provider which tracks the currently active task (document and task name)
 export function activateWorkspaceTaskProvider(inspectManager: InspectManager, context: ExtensionContext) {
 
   // The task manager
   const taskManager = new WorkspaceTaskManager();
 
   // If the interpreter changes, refresh the tasks
   context.subscriptions.push(inspectManager.onInspectChanged((e: InspectChangedEvent) => {
```

### Comparing `inspect_ai-0.3.8/tools/vscode/tools/ts-to-mjs/src/jsonrpc.ts` & `inspect_ai-0.3.9/tools/vscode/tools/ts-to-mjs/src/jsonrpc.ts`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/tools/ts-to-mjs/yarn.lock` & `inspect_ai-0.3.9/tools/vscode/tools/ts-to-mjs/yarn.lock`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/tsconfig.json` & `inspect_ai-0.3.9/tools/vscode/tsconfig.json`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/webpack.config.js` & `inspect_ai-0.3.9/tools/vscode/webpack.config.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.8/tools/vscode/yarn.lock` & `inspect_ai-0.3.9/tools/vscode/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -371,18 +371,18 @@
     undici-types "~5.26.4"
 
 "@types/semver@^7.5.0":
   version "7.5.8"
   resolved "https://registry.yarnpkg.com/@types/semver/-/semver-7.5.8.tgz#8268a8c57a3e4abd25c165ecd36237db7948a55e"
   integrity sha512-I8EUhyrgfLrcTkzV3TSsGyl1tSuPrEDzr0yd5m90UgNxQkyDXULk3b6MlQqTCpZpNtWe1K0hzclnZkTcLBe2UQ==
 
-"@types/vscode@^1.87.0":
-  version "1.87.0"
-  resolved "https://registry.yarnpkg.com/@types/vscode/-/vscode-1.87.0.tgz#ee9b163f3d2115fb0b20619b34dd3abc5a923361"
-  integrity sha512-y3yYJV2esWr8LNjp3VNbSMWG7Y43jC8pCldG8YwiHGAQbsymkkMMt0aDT1xZIOFM2eFcNiUc+dJMx1+Z0UT8fg==
+"@types/vscode@1.85":
+  version "1.85.0"
+  resolved "https://registry.yarnpkg.com/@types/vscode/-/vscode-1.85.0.tgz#46beb07f0f626665b52d1e2294382b2bc63b602e"
+  integrity sha512-CF/RBon/GXwdfmnjZj0WTUMZN5H6YITOfBCP4iEZlOtVQXuzw6t7Le7+cR+7JzdMrnlm7Mfp49Oj2TuSXIWo3g==
 
 "@typescript-eslint/eslint-plugin@^7.4.0":
   version "7.4.0"
   resolved "https://registry.yarnpkg.com/@typescript-eslint/eslint-plugin/-/eslint-plugin-7.4.0.tgz#de61c3083842fc6ac889d2fc83c9a96b55ab8328"
   integrity sha512-yHMQ/oFaM7HZdVrVm/M2WHaNPgyuJH4WelkSVEWSSsir34kxW2kDJCxlXRhhGWEsMN0WAW/vLpKfKVcm8k+MPw==
   dependencies:
     "@eslint-community/regexpp" "^4.5.1"
```

