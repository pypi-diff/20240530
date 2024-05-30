# Comparing `tmp/sphinx-deployment-0.0.8.tar.gz` & `tmp/sphinx-deployment-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-deployment-0.0.8.tar", last modified: Wed Jan 17 06:34:02 2024, max compression
+gzip compressed data, was "sphinx-deployment-0.0.9.tar", last modified: Sun Jan 21 17:21:07 2024, max compression
```

## Comparing `sphinx-deployment-0.0.8.tar` & `sphinx-deployment-0.0.9.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 06:34:02.439344 sphinx-deployment-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 06:34:02.431344 sphinx-deployment-0.0.8/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 06:34:02.431344 sphinx-deployment-0.0.8/.github/matchers/
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/.github/matchers/pylint.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 06:34:02.431344 sphinx-deployment-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/.github/workflows/cd.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/.github/workflows/preview.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/.releaserc.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 06:34:02.431344 sphinx-deployment-0.0.8/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-01-17 06:34:02.439344 sphinx-deployment-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 06:34:02.435344 sphinx-deployment-0.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 06:34:02.435344 sphinx-deployment-0.0.8/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/docs/api/sphinx_deployment.rst
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/docs/getting_started.md
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-17 06:34:02.439344 sphinx-deployment-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 06:34:02.427344 sphinx-deployment-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 06:34:02.435344 sphinx-deployment-0.0.8/src/sphinx_deployment/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/src/sphinx_deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/src/sphinx_deployment/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 06:34:02.427344 sphinx-deployment-0.0.8/src/sphinx_deployment/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 06:34:02.435344 sphinx-deployment-0.0.8/src/sphinx_deployment/_static/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/src/sphinx_deployment/_static/templates/redirect.html
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/src/sphinx_deployment/_static/templates/rtd.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 06:34:02.427344 sphinx-deployment-0.0.8/src/sphinx_deployment/_static/theme/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 06:34:02.435344 sphinx-deployment-0.0.8/src/sphinx_deployment/_static/theme/rtd/
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/src/sphinx_deployment/_static/theme/rtd/rtd.css
--rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/src/sphinx_deployment/_static/theme/rtd/rtd.js_t
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-17 06:34:02.000000 sphinx-deployment-0.0.8/src/sphinx_deployment/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/src/sphinx_deployment/_version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    19036 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/src/sphinx_deployment/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/src/sphinx_deployment/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/src/sphinx_deployment/sphinx_ext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 06:34:02.439344 sphinx-deployment-0.0.8/src/sphinx_deployment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-01-17 06:34:02.000000 sphinx-deployment-0.0.8/src/sphinx_deployment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-01-17 06:34:02.000000 sphinx-deployment-0.0.8/src/sphinx_deployment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-17 06:34:02.000000 sphinx-deployment-0.0.8/src/sphinx_deployment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-01-17 06:34:02.000000 sphinx-deployment-0.0.8/src/sphinx_deployment.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-01-17 06:34:02.000000 sphinx-deployment-0.0.8/src/sphinx_deployment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-17 06:34:02.000000 sphinx-deployment-0.0.8/src/sphinx_deployment.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 06:34:02.435344 sphinx-deployment-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/tests/test_git.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-01-17 06:33:43.000000 sphinx-deployment-0.0.8/tests/test_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 17:21:07.303029 sphinx-deployment-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 17:21:07.295029 sphinx-deployment-0.0.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 17:21:07.295029 sphinx-deployment-0.0.9/.github/matchers/
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/.github/matchers/pylint.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 17:21:07.295029 sphinx-deployment-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/.github/workflows/cd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/.github/workflows/preview.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/.releaserc.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 17:21:07.295029 sphinx-deployment-0.0.9/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-01-21 17:21:07.303029 sphinx-deployment-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 17:21:07.295029 sphinx-deployment-0.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 17:21:07.299029 sphinx-deployment-0.0.9/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/docs/api/sphinx_deployment.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/docs/getting_started.md
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-21 17:21:07.303029 sphinx-deployment-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 17:21:07.291029 sphinx-deployment-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 17:21:07.299029 sphinx-deployment-0.0.9/src/sphinx_deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/src/sphinx_deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/src/sphinx_deployment/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 17:21:07.291029 sphinx-deployment-0.0.9/src/sphinx_deployment/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 17:21:07.299029 sphinx-deployment-0.0.9/src/sphinx_deployment/_static/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/src/sphinx_deployment/_static/templates/redirect.html
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/src/sphinx_deployment/_static/templates/rtd.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 17:21:07.291029 sphinx-deployment-0.0.9/src/sphinx_deployment/_static/theme/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 17:21:07.299029 sphinx-deployment-0.0.9/src/sphinx_deployment/_static/theme/rtd/
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/src/sphinx_deployment/_static/theme/rtd/rtd.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/src/sphinx_deployment/_static/theme/rtd/rtd.js_t
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-21 17:21:07.000000 sphinx-deployment-0.0.9/src/sphinx_deployment/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/src/sphinx_deployment/_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    19036 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/src/sphinx_deployment/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/src/sphinx_deployment/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/src/sphinx_deployment/sphinx_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 17:21:07.299029 sphinx-deployment-0.0.9/src/sphinx_deployment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-01-21 17:21:07.000000 sphinx-deployment-0.0.9/src/sphinx_deployment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-01-21 17:21:07.000000 sphinx-deployment-0.0.9/src/sphinx_deployment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-21 17:21:07.000000 sphinx-deployment-0.0.9/src/sphinx_deployment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-01-21 17:21:07.000000 sphinx-deployment-0.0.9/src/sphinx_deployment.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-01-21 17:21:07.000000 sphinx-deployment-0.0.9/src/sphinx_deployment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-21 17:21:07.000000 sphinx-deployment-0.0.9/src/sphinx_deployment.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 17:21:07.299029 sphinx-deployment-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/tests/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-01-21 17:20:48.000000 sphinx-deployment-0.0.9/tests/test_versions.py
```

### Comparing `sphinx-deployment-0.0.8/.github/CONTRIBUTING.md` & `sphinx-deployment-0.0.9/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sphinx-deployment-0.0.8/.github/matchers/pylint.json` & `sphinx-deployment-0.0.9/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `sphinx-deployment-0.0.8/.github/workflows/cd.yml` & `sphinx-deployment-0.0.9/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `sphinx-deployment-0.0.8/.github/workflows/ci.yml` & `sphinx-deployment-0.0.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `sphinx-deployment-0.0.8/.github/workflows/preview.yml` & `sphinx-deployment-0.0.9/.github/workflows/preview.yml`

 * *Files identical despite different names*

### Comparing `sphinx-deployment-0.0.8/.gitignore` & `sphinx-deployment-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `sphinx-deployment-0.0.8/.pre-commit-config.yaml` & `sphinx-deployment-0.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sphinx-deployment-0.0.8/.releaserc.js` & `sphinx-deployment-0.0.9/.releaserc.js`

 * *Files identical despite different names*

### Comparing `sphinx-deployment-0.0.8/.vscode/launch.json` & `sphinx-deployment-0.0.9/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `sphinx-deployment-0.0.8/CHANGELOG.md` & `sphinx-deployment-0.0.9/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+## [0.0.9](https://github.com/msclock/sphinx-deployment/compare/v0.0.8...v0.0.9) (2024-01-21)
+
+
+### Performance
+
+* opt js load ([#33](https://github.com/msclock/sphinx-deployment/issues/33)) ([2f1ea38](https://github.com/msclock/sphinx-deployment/commit/2f1ea38b95703a6917b5176ca5c171a3dd53e5b1)), closes [#32](https://github.com/msclock/sphinx-deployment/issues/32)
+
 ## [0.0.8](https://github.com/msclock/sphinx-deployment/compare/v0.0.7...v0.0.8) (2024-01-17)
 
 
 ### Bug Fixes
 
 * redirect to a new version ([#31](https://github.com/msclock/sphinx-deployment/issues/31)) ([40ab807](https://github.com/msclock/sphinx-deployment/commit/40ab807b278f55b17e9a48789c08658522cddbc8)), closes [#30](https://github.com/msclock/sphinx-deployment/issues/30)
```

### Comparing `sphinx-deployment-0.0.8/LICENSE` & `sphinx-deployment-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-deployment-0.0.8/PKG-INFO` & `sphinx-deployment-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-deployment
-Version: 0.0.8
+Version: 0.0.9
 Summary: A versioned documentation deployment tool for sphinx.
 Author-email: msclock <msclock@126.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/msclock/sphinx-deployment
 Project-URL: Bug Tracker, https://github.com/msclock/sphinx-deployment/issues
 Project-URL: Discussions, https://github.com/msclock/sphinx-deployment/discussions
 Project-URL: Changelog, https://github.com/msclock/sphinx-deployment/releases
```

### Comparing `sphinx-deployment-0.0.8/README.md` & `sphinx-deployment-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sphinx-deployment-0.0.8/docs/conf.py` & `sphinx-deployment-0.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx-deployment-0.0.8/docs/getting_started.md` & `sphinx-deployment-0.0.9/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `sphinx-deployment-0.0.8/docs/index.md` & `sphinx-deployment-0.0.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `sphinx-deployment-0.0.8/noxfile.py` & `sphinx-deployment-0.0.9/noxfile.py`

 * *Files identical despite different names*

### Comparing `sphinx-deployment-0.0.8/pyproject.toml` & `sphinx-deployment-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sphinx-deployment-0.0.8/src/sphinx_deployment/_static/templates/redirect.html` & `sphinx-deployment-0.0.9/src/sphinx_deployment/_static/templates/redirect.html`

 * *Files identical despite different names*

### Comparing `sphinx-deployment-0.0.8/src/sphinx_deployment/_static/theme/rtd/rtd.css` & `sphinx-deployment-0.0.9/src/sphinx_deployment/_static/theme/rtd/rtd.css`

 * *Files identical despite different names*

### Comparing `sphinx-deployment-0.0.8/src/sphinx_deployment/_static/theme/rtd/rtd.js_t` & `sphinx-deployment-0.0.9/src/sphinx_deployment/_static/theme/rtd/rtd.js_t`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,8 @@
 /**
- * Locates the URL of the versions.json file by recursively checking parent directories.
- *
- * @param {string} url - The URL of the current directory.
- * @return {string} The URL of the versions.json file, or null if not found.
- */
-async function locateVersionsJsonUrl(url) {
-  let checkUrl = url.endsWith("/") ? url.slice(0, -1) : url;
-  let response;
-
-  while (checkUrl !== "") {
-    try {
-      response = await fetch(checkUrl + "/versions.json");
-      if (response.ok) {
-        return checkUrl + "/versions.json";
-      }
-    } catch (error) {
-      console.warn("Failed to find versions.json at " + checkUrl + ":", error);
-    }
-
-    checkUrl = checkUrl.substring(0, checkUrl.lastIndexOf("/"));
-  }
-
-  return null;
-}
-
-/**
  * Change the version of the root URL to the specified version.
  *
  * @param {string} rootUrl - The root URL.
  * @param {string} currentVersion - The current version.
  * @param {string} currentVersionPath - The path to the current version.
  * @param {object} ver - The version object containing the name of the new version.
  * @return {void} This function does not return a value.
@@ -48,37 +22,22 @@
       .catch((_) => {
         window.location.href = rootUrl + "/" + ver.name + "/";
       });
   }
 };
 
 window.addEventListener("DOMContentLoaded", async function () {
-  var cur_href_path = this.window.location.href.substring(0, this.window.location.href.lastIndexOf("/"))
-  if (sphinx_deployment_versions_file) {
-    var versionsJsonUrl = new URL(cur_href_path + "/" + sphinx_deployment_versions_file).toString();
-  } else {
-    try {
-      var versionsJsonUrl = await locateVersionsJsonUrl(cur_href_path);
-    } catch (error) {
-      console.error("Failed to find versions.json");
-    }
-    if (versionsJsonUrl === null) {
-      console.error("Failed to find versions.json");
-      return;
-    }
+  if (!versionsJsonUrl || !sphinx_deployment_current_version) {
+    console.error("versionsJsonUrl or sphinx_deployment_current_version is not set");
+    return;
   }
 
   var rootUrl = versionsJsonUrl.slice(0, versionsJsonUrl.lastIndexOf("/"));
-  if (sphinx_deployment_current_version) {
-    var currentVersionPath = "/" + sphinx_deployment_current_version + "/";
-    var currentVersion = sphinx_deployment_current_version;
-  } else {
-    var currentVersionPath = this.window.location.href.substring(rootUrl.length);
-    var currentVersion = currentVersionPath.match(/\/([^\/]+)\//)[1];
-  }
+  var currentVersionPath = "/" + sphinx_deployment_current_version + "/";
+  var currentVersion = sphinx_deployment_current_version;
 
   const response = await fetch(versionsJsonUrl);
   if (!response.ok) {
     throw new Error("Failed to fetch versions.json");
   }
   const versionsJson = await response.json();
```

### Comparing `sphinx-deployment-0.0.8/src/sphinx_deployment/cli.py` & `sphinx-deployment-0.0.9/src/sphinx_deployment/cli.py`

 * *Files identical despite different names*

### Comparing `sphinx-deployment-0.0.8/src/sphinx_deployment/sphinx_ext.py` & `sphinx-deployment-0.0.9/src/sphinx_deployment/sphinx_ext.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,29 +69,30 @@
 
     Returns:
         None
     """
     _ = (pagename, templatename, context, doctree)
 
     # Get the path to the versions.json file
-    context["sphinx_deployment_versions_file"] = str(
+    sphinx_deployment_versions_file = str(
         Path(context["content_root"]) / ".." / "versions.json"
     )
 
     # Expose the current versiont to the template
     context[
         "sphinx_deployment_current_version"
     ] = app.config.sphinx_deployment_current_version
 
     # Register css and js files
     app.add_js_file(
         None,
         body=f"""
-        var sphinx_deployment_versions_file = '{context["sphinx_deployment_versions_file"]}';
         var sphinx_deployment_current_version = '{context["sphinx_deployment_current_version"]}';
+        var versionsJsonUrl = new URL(window.location.href + '{sphinx_deployment_versions_file}');
+        versionsJsonUrl  = versionsJsonUrl.toString()
         """,
         priority=0,
     )
 
     app.add_css_file("theme/rtd/rtd.css", priority=600)
     app.add_js_file("theme/rtd/rtd.js", priority=600)
```

### Comparing `sphinx-deployment-0.0.8/src/sphinx_deployment.egg-info/PKG-INFO` & `sphinx-deployment-0.0.9/src/sphinx_deployment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-deployment
-Version: 0.0.8
+Version: 0.0.9
 Summary: A versioned documentation deployment tool for sphinx.
 Author-email: msclock <msclock@126.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/msclock/sphinx-deployment
 Project-URL: Bug Tracker, https://github.com/msclock/sphinx-deployment/issues
 Project-URL: Discussions, https://github.com/msclock/sphinx-deployment/discussions
 Project-URL: Changelog, https://github.com/msclock/sphinx-deployment/releases
```

### Comparing `sphinx-deployment-0.0.8/src/sphinx_deployment.egg-info/SOURCES.txt` & `sphinx-deployment-0.0.9/src/sphinx_deployment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sphinx-deployment-0.0.8/tests/test_versions.py` & `sphinx-deployment-0.0.9/tests/test_versions.py`

 * *Files identical despite different names*

