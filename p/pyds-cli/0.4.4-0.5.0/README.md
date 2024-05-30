# Comparing `tmp/pyds-cli-0.4.4.tar.gz` & `tmp/pyds_cli-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyds-cli-0.4.4.tar", last modified: Mon Apr  8 22:26:59 2024, max compression
+gzip compressed data, was "pyds_cli-0.5.0.tar", last modified: Thu May 30 06:09:46 2024, max compression
```

## Comparing `pyds-cli-0.4.4.tar` & `pyds_cli-0.5.0.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:26:59.127802 pyds-cli-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-08 22:26:59.127802 pyds-cli-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:26:59.115801 pyds-cli-0.4.4/pyds/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:26:59.115801 pyds-cli-0.4.4/pyds/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/cli/conda.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/cli/docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/cli/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/cli/package.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/cli/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/cli/system.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/cli/talk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:26:59.111801 pyds-cli-0.4.4/pyds/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:26:59.115801 pyds-cli-0.4.4/pyds/templates/project/
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/project/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:26:59.119802 pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/.darglint
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:26:59.119802 pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:26:59.111801 pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:26:59.119802 pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/.github/workflows/code-style.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/.github/workflows/pr-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/.github/workflows/release-pypi-package.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:26:59.119802 pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/docs/api.md
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/docs/apidocs.css
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/docs/config.js
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/mkdocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:26:59.119802 pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/tests/test___init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/tests/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:26:59.119802 pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/{{ cookiecutter.__module_name }}/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/{{ cookiecutter.__module_name }}/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/{{ cookiecutter.__module_name }}/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/{{ cookiecutter.__module_name }}/models.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/{{ cookiecutter.__module_name }}/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/{{ cookiecutter.__module_name }}/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/{{ cookiecutter.__module_name }}/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:26:59.119802 pyds-cli-0.4.4/pyds/templates/talk/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/talk/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:26:59.123802 pyds-cli-0.4.4/pyds/templates/talk/{{ cookiecutter.__repo_name }}/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:26:59.111801 pyds-cli-0.4.4/pyds/templates/talk/{{ cookiecutter.__repo_name }}/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:26:59.123802 pyds-cli-0.4.4/pyds/templates/talk/{{ cookiecutter.__repo_name }}/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/talk/{{ cookiecutter.__repo_name }}/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/talk/{{ cookiecutter.__repo_name }}/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/talk/{{ cookiecutter.__repo_name }}/.markdownlint.json
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/talk/{{ cookiecutter.__repo_name }}/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/talk/{{ cookiecutter.__repo_name }}/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/templates/talk/{{ cookiecutter.__repo_name }}/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:26:59.123802 pyds-cli-0.4.4/pyds/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/utils/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/pyds/utils/project.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-08 22:17:59.000000 pyds-cli-0.4.4/pyds/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:26:59.127802 pyds-cli-0.4.4/pyds_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-08 22:26:59.000000 pyds-cli-0.4.4/pyds_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-08 22:26:59.000000 pyds-cli-0.4.4/pyds_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 22:26:59.000000 pyds-cli-0.4.4/pyds_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 22:26:59.000000 pyds-cli-0.4.4/pyds_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-08 22:26:59.000000 pyds-cli-0.4.4/pyds_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-08 22:26:59.000000 pyds-cli-0.4.4/pyds_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-08 22:17:59.000000 pyds-cli-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 22:26:59.127802 pyds-cli-0.4.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:26:59.115801 pyds-cli-0.4.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:26:59.123802 pyds-cli-0.4.4/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/tests/cli/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/tests/cli/test___init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/tests/cli/test_conda.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/tests/cli/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/tests/cli/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/tests/cli/test_package.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/tests/cli/test_project.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/tests/cli/test_system.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-08 22:17:56.000000 pyds-cli-0.4.4/tests/cli/test_talk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:09:46.253610 pyds_cli-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-30 06:09:46.253610 pyds_cli-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:09:46.245611 pyds_cli-0.5.0/pyds/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:09:46.245611 pyds_cli-0.5.0/pyds/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/cli/conda.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/cli/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/cli/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/cli/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/cli/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/cli/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/cli/talk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:09:46.241611 pyds_cli-0.5.0/pyds/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:09:46.245611 pyds_cli-0.5.0/pyds/templates/project/
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/project/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:09:46.245611 pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/.darglint
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:09:46.249611 pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:09:46.241611 pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:09:46.249611 pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/.github/workflows/code-style.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/.github/workflows/pr-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/.github/workflows/release-pypi-package.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:09:46.249611 pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/docs/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/docs/apidocs.css
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/docs/config.js
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/mkdocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:09:46.249611 pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/tests/test___init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:09:46.249611 pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/{{ cookiecutter.__module_name }}/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/{{ cookiecutter.__module_name }}/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/{{ cookiecutter.__module_name }}/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/{{ cookiecutter.__module_name }}/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/{{ cookiecutter.__module_name }}/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/{{ cookiecutter.__module_name }}/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/{{ cookiecutter.__module_name }}/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:09:46.249611 pyds_cli-0.5.0/pyds/templates/talk/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/talk/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:09:46.249611 pyds_cli-0.5.0/pyds/templates/talk/{{ cookiecutter.__repo_name }}/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:09:46.241611 pyds_cli-0.5.0/pyds/templates/talk/{{ cookiecutter.__repo_name }}/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:09:46.249611 pyds_cli-0.5.0/pyds/templates/talk/{{ cookiecutter.__repo_name }}/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/talk/{{ cookiecutter.__repo_name }}/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/talk/{{ cookiecutter.__repo_name }}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/talk/{{ cookiecutter.__repo_name }}/.markdownlint.json
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/talk/{{ cookiecutter.__repo_name }}/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/talk/{{ cookiecutter.__repo_name }}/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/templates/talk/{{ cookiecutter.__repo_name }}/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:09:46.253610 pyds_cli-0.5.0/pyds/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/utils/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/pyds/utils/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-30 06:05:45.000000 pyds_cli-0.5.0/pyds/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:09:46.253610 pyds_cli-0.5.0/pyds_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-30 06:09:46.000000 pyds_cli-0.5.0/pyds_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-30 06:09:46.000000 pyds_cli-0.5.0/pyds_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 06:09:46.000000 pyds_cli-0.5.0/pyds_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 06:09:46.000000 pyds_cli-0.5.0/pyds_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-30 06:09:46.000000 pyds_cli-0.5.0/pyds_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-30 06:09:46.000000 pyds_cli-0.5.0/pyds_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-30 06:05:45.000000 pyds_cli-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 06:09:46.253610 pyds_cli-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:09:46.241611 pyds_cli-0.5.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:09:46.253610 pyds_cli-0.5.0/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/tests/cli/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/tests/cli/test___init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/tests/cli/test_conda.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/tests/cli/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/tests/cli/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/tests/cli/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/tests/cli/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/tests/cli/test_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-30 06:05:42.000000 pyds_cli-0.5.0/tests/cli/test_talk.py
```

### Comparing `pyds-cli-0.4.4/PKG-INFO` & `pyds_cli-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyds-cli
-Version: 0.4.4
+Version: 0.5.0
 Description-Content-Type: text/markdown
 Requires-Dist: typer>=0.3.8
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: jinja2>=3.0.2
 Requires-Dist: loguru>=0.5.3
 Requires-Dist: pyprojroot
 Requires-Dist: python-dotenv>=0.19.1
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyds-cli Version: 0.4.4 Description-Content-Type:
+Metadata-Version: 2.1 Name: pyds-cli Version: 0.5.0 Description-Content-Type:
 text/markdown Requires-Dist: typer>=0.3.8 Requires-Dist: pyyaml>=6.0 Requires-
 Dist: jinja2>=3.0.2 Requires-Dist: loguru>=0.5.3 Requires-Dist: pyprojroot
 Requires-Dist: python-dotenv>=0.19.1 Requires-Dist: rich>=10.12.0 Requires-
 Dist: ruamel.yaml>=0.17.17 Requires-Dist: case-converter>=1.0.2 Requires-Dist:
 jinja2-strcase>=0.0.2 Requires-Dist: cookiecutter Requires-Dist: sh # PyDS CLI
 [![All Contributors](https://img.shields.io/badge/all_contributors-4-
 orange.svg?style=flat-square)](#contributors-) Helping you manage your data
```

### Comparing `pyds-cli-0.4.4/README.md` & `pyds_cli-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.4.4/pyds/cli/__init__.py` & `pyds_cli-0.5.0/pyds/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.4.4/pyds/cli/conda.py` & `pyds_cli-0.5.0/pyds/cli/conda.py`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.4.4/pyds/cli/environment.py` & `pyds_cli-0.5.0/pyds/cli/environment.py`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.4.4/pyds/cli/package.py` & `pyds_cli-0.5.0/pyds/cli/package.py`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.4.4/pyds/cli/project.py` & `pyds_cli-0.5.0/pyds/cli/project.py`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.4.4/pyds/cli/system.py` & `pyds_cli-0.5.0/pyds/cli/system.py`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.4.4/pyds/templates/project/cookiecutter.json` & `pyds_cli-0.5.0/pyds/templates/project/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/.devcontainer/Dockerfile` & `pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/.devcontainer/devcontainer.json` & `pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/.github/workflows/docs.yaml` & `pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/.github/workflows/pr-tests.yaml` & `pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/.github/workflows/pr-tests.yaml`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/.github/workflows/release-pypi-package.yaml` & `pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/.github/workflows/release-pypi-package.yaml`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/.gitignore` & `pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/.gitignore`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/.pre-commit-config.yaml` & `pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/docs/apidocs.css` & `pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/docs/apidocs.css`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/docs/index.md` & `pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/docs/index.md`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/environment.yml` & `pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/environment.yml`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/mkdocs.yaml` & `pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/pyproject.toml` & `pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,16 @@
 # See https://docs.astral.sh/ruff/configuration/#using-pyprojecttoml for configuration documentation
 select = ["E", "F", "I"]
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
-where = ["{{ cookiecutter.__module_name }}"]
+where = ["."]
+namespaces = false
 
 [project]
 name = "{{ cookiecutter.__package_name }}"
 version = "0.0.1"
 dependencies = [
     "matplotlib",
     "pandas",
```

### Comparing `pyds-cli-0.4.4/pyds/templates/project/{{ cookiecutter.__repo_name }}/{{ cookiecutter.__module_name }}/cli.py` & `pyds_cli-0.5.0/pyds/templates/project/{{ cookiecutter.__repo_name }}/{{ cookiecutter.__module_name }}/cli.py`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.4.4/pyds/templates/talk/cookiecutter.json` & `pyds_cli-0.5.0/pyds/templates/talk/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.4.4/pyds/utils/__init__.py` & `pyds_cli-0.5.0/pyds/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.4.4/pyds/utils/project.py` & `pyds_cli-0.5.0/pyds/utils/project.py`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.4.4/pyds_cli.egg-info/PKG-INFO` & `pyds_cli-0.5.0/pyds_cli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyds-cli
-Version: 0.4.4
+Version: 0.5.0
 Description-Content-Type: text/markdown
 Requires-Dist: typer>=0.3.8
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: jinja2>=3.0.2
 Requires-Dist: loguru>=0.5.3
 Requires-Dist: pyprojroot
 Requires-Dist: python-dotenv>=0.19.1
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyds-cli Version: 0.4.4 Description-Content-Type:
+Metadata-Version: 2.1 Name: pyds-cli Version: 0.5.0 Description-Content-Type:
 text/markdown Requires-Dist: typer>=0.3.8 Requires-Dist: pyyaml>=6.0 Requires-
 Dist: jinja2>=3.0.2 Requires-Dist: loguru>=0.5.3 Requires-Dist: pyprojroot
 Requires-Dist: python-dotenv>=0.19.1 Requires-Dist: rich>=10.12.0 Requires-
 Dist: ruamel.yaml>=0.17.17 Requires-Dist: case-converter>=1.0.2 Requires-Dist:
 jinja2-strcase>=0.0.2 Requires-Dist: cookiecutter Requires-Dist: sh # PyDS CLI
 [![All Contributors](https://img.shields.io/badge/all_contributors-4-
 orange.svg?style=flat-square)](#contributors-) Helping you manage your data
```

### Comparing `pyds-cli-0.4.4/pyds_cli.egg-info/SOURCES.txt` & `pyds_cli-0.5.0/pyds_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.4.4/pyproject.toml` & `pyds_cli-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 include-package-data = true
 
 [tool.setuptools.packages]
 find = {}  # Scanning implicit namespaces is active by default
 
 [project]
 name = "pyds-cli"
-version = "0.4.4"
+version = "0.5.0"
 dependencies = [
     "typer >=0.3.8",
     "pyyaml >=6.0",
     "jinja2 >=3.0.2",
     "loguru >=0.5.3",
     "pyprojroot",
     "python-dotenv >=0.19.1",
```

### Comparing `pyds-cli-0.4.4/tests/cli/conftest.py` & `pyds_cli-0.5.0/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.4.4/tests/cli/test___init__.py` & `pyds_cli-0.5.0/tests/cli/test___init__.py`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.4.4/tests/cli/test_conda.py` & `pyds_cli-0.5.0/tests/cli/test_conda.py`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.4.4/tests/cli/test_environment.py` & `pyds_cli-0.5.0/tests/cli/test_environment.py`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.4.4/tests/cli/test_talk.py` & `pyds_cli-0.5.0/tests/cli/test_talk.py`

 * *Files identical despite different names*

