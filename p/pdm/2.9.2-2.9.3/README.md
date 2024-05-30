# Comparing `tmp/pdm-2.9.2.tar.gz` & `tmp/pdm-2.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm-2.9.2.tar", last modified: Tue Sep 12 09:45:29 2023, max compression
+gzip compressed data, was "pdm-2.9.3.tar", last modified: Mon Sep 25 09:23:06 2023, max compression
```

## Comparing `pdm-2.9.2.tar` & `pdm-2.9.3.tar`

### file list

```diff
@@ -1,283 +1,283 @@
--rw-r--r--   0        0        0   133255 2023-09-12 09:45:17.766704 pdm-2.9.2/CHANGELOG.md
--rw-r--r--   0        0        0     1075 2023-09-12 09:45:17.766704 pdm-2.9.2/LICENSE
--rw-r--r--   0        0        0     1075 2023-09-12 09:45:17.766704 pdm-2.9.2/LICENSE
--rw-r--r--   0        0        0     8002 2023-09-12 09:45:17.766704 pdm-2.9.2/README.md
--rw-r--r--   0        0        0     8002 2023-09-12 09:45:17.766704 pdm-2.9.2/README.md
--rw-r--r--   0        0        0     4709 2023-09-12 09:45:29.278976 pdm-2.9.2/pyproject.toml
--rw-r--r--   0        0        0       65 2023-09-12 09:45:17.770705 pdm-2.9.2/src/pdm/__main__.py
--rw-r--r--   0        0        0      316 2023-09-12 09:45:17.770705 pdm-2.9.2/src/pdm/__version__.py
--rw-r--r--   0        0        0     3413 2023-09-12 09:45:17.770705 pdm-2.9.2/src/pdm/_types.py
--rw-r--r--   0        0        0      237 2023-09-12 09:45:17.770705 pdm-2.9.2/src/pdm/builders/__init__.py
--rw-r--r--   0        0        0    11924 2023-09-12 09:45:17.770705 pdm-2.9.2/src/pdm/builders/base.py
--rw-r--r--   0        0        0     1791 2023-09-12 09:45:17.770705 pdm-2.9.2/src/pdm/builders/editable.py
--rw-r--r--   0        0        0      656 2023-09-12 09:45:17.770705 pdm-2.9.2/src/pdm/builders/sdist.py
--rw-r--r--   0        0        0     1073 2023-09-12 09:45:17.770705 pdm-2.9.2/src/pdm/builders/wheel.py
--rw-r--r--   0        0        0        0 2023-09-12 09:45:17.770705 pdm-2.9.2/src/pdm/cli/__init__.py
--rw-r--r--   0        0        0    16592 2023-09-12 09:45:17.770705 pdm-2.9.2/src/pdm/cli/actions.py
--rw-r--r--   0        0        0        0 2023-09-12 09:45:17.770705 pdm-2.9.2/src/pdm/cli/commands/__init__.py
--rw-r--r--   0        0        0     7146 2023-09-12 09:45:17.770705 pdm-2.9.2/src/pdm/cli/commands/add.py
--rw-r--r--   0        0        0     2871 2023-09-12 09:45:17.770705 pdm-2.9.2/src/pdm/cli/commands/base.py
--rw-r--r--   0        0        0     4236 2023-09-12 09:45:17.770705 pdm-2.9.2/src/pdm/cli/commands/build.py
--rw-r--r--   0        0        0     6542 2023-09-12 09:45:17.770705 pdm-2.9.2/src/pdm/cli/commands/cache.py
--rw-r--r--   0        0        0     1275 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/commands/completion.py
--rw-r--r--   0        0        0     7537 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/commands/config.py
--rw-r--r--   0        0        0     3066 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/commands/export.py
--rw-r--r--   0        0        0     3136 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/commands/fix/__init__.py
--rw-r--r--   0        0        0     2309 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/commands/fix/fixers.py
--rw-r--r--   0        0        0     3679 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/commands/import_cmd.py
--rw-r--r--   0        0        0     3032 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/commands/info.py
--rw-r--r--   0        0        0    10723 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/commands/init.py
--rw-r--r--   0        0        0     3931 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/commands/install.py
--rw-r--r--   0        0        0    16678 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/commands/list.py
--rw-r--r--   0        0        0     2645 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/commands/lock.py
--rw-r--r--   0        0        0     6596 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/commands/publish/__init__.py
--rw-r--r--   0        0        0     8112 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/commands/publish/package.py
--rw-r--r--   0        0        0     6954 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/commands/publish/repository.py
--rw-r--r--   0        0        0     4379 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/commands/remove.py
--rw-r--r--   0        0        0    15923 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/commands/run.py
--rw-r--r--   0        0        0     2437 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/commands/search.py
--rw-r--r--   0        0        0     9371 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/commands/self_cmd.py
--rw-r--r--   0        0        0     2896 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/commands/show.py
--rw-r--r--   0        0        0     1447 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/commands/sync.py
--rw-r--r--   0        0        0     7320 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/commands/update.py
--rw-r--r--   0        0        0     6484 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/commands/use.py
--rw-r--r--   0        0        0     1720 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/commands/venv/__init__.py
--rw-r--r--   0        0        0     2519 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/commands/venv/activate.py
--rw-r--r--   0        0        0     6149 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/commands/venv/backends.py
--rw-r--r--   0        0        0     2156 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/commands/venv/create.py
--rw-r--r--   0        0        0      820 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/commands/venv/list.py
--rw-r--r--   0        0        0     2196 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/commands/venv/purge.py
--rw-r--r--   0        0        0     1280 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/commands/venv/remove.py
--rw-r--r--   0        0        0     2652 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/commands/venv/utils.py
--rw-r--r--   0        0        0        0 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/completions/__init__.py
--rw-r--r--   0        0        0     5210 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/completions/pdm.bash
--rw-r--r--   0        0        0    51762 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/completions/pdm.fish
--rw-r--r--   0        0        0    18961 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/completions/pdm.ps1
--rw-r--r--   0        0        0    25885 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/completions/pdm.zsh
--rw-r--r--   0        0        0     3840 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/filters.py
--rw-r--r--   0        0        0     1481 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/hooks.py
--rw-r--r--   0        0        0    10746 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/options.py
--rw-r--r--   0        0        0     6718 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/templates/__init__.py
--rw-r--r--   0        0        0     3102 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/templates/default/.gitignore
--rw-r--r--   0        0        0       18 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/templates/default/README.md
--rw-r--r--   0        0        0        0 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/templates/default/__init__.py
--rw-r--r--   0        0        0      278 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/templates/default/pyproject.toml
--rw-r--r--   0        0        0        0 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/templates/default/src/example_package/__init__.py
--rw-r--r--   0        0        0        0 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/templates/default/tests/__init__.py
--rw-r--r--   0        0        0    29245 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/cli/utils.py
--rw-r--r--   0        0        0     2642 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/compat.py
--rw-r--r--   0        0        0    10620 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/core.py
--rw-r--r--   0        0        0      825 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/environments/__init__.py
--rw-r--r--   0        0        0     9734 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/environments/base.py
--rw-r--r--   0        0        0     4273 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/environments/local.py
--rw-r--r--   0        0        0     2047 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/environments/python.py
--rw-r--r--   0        0        0     1362 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/exceptions.py
--rw-r--r--   0        0        0     1268 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/formats/__init__.py
--rw-r--r--   0        0        0     3825 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/formats/base.py
--rw-r--r--   0        0        0     5788 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/formats/flit.py
--rw-r--r--   0        0        0     2614 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/formats/pipfile.py
--rw-r--r--   0        0        0     7490 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/formats/poetry.py
--rw-r--r--   0        0        0     7576 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/formats/requirements.py
--rw-r--r--   0        0        0     2336 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/formats/setup_py.py
--rw-r--r--   0        0        0      119 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/installers/__init__.py
--rw-r--r--   0        0        0     1367 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/installers/core.py
--rw-r--r--   0        0        0    11127 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/installers/installers.py
--rw-r--r--   0        0        0     2092 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/installers/manager.py
--rw-r--r--   0        0        0     2226 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/installers/packages.py
--rw-r--r--   0        0        0    18570 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/installers/synchronizers.py
--rw-r--r--   0        0        0    11150 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/installers/uninstallers.py
--rw-r--r--   0        0        0        6 2023-09-12 09:45:29.258975 pdm-2.9.2/src/pdm/models/VERSION
--rw-r--r--   0        0        0        0 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/models/__init__.py
--rw-r--r--   0        0        0     3162 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/models/auth.py
--rw-r--r--   0        0        0     4664 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/models/backends.py
--rw-r--r--   0        0        0    12157 2023-09-12 09:45:17.774705 pdm-2.9.2/src/pdm/models/caches.py
--rw-r--r--   0        0        0    26920 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/models/candidates.py
--rw-r--r--   0        0        0      287 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/models/environment.py
--rw-r--r--   0        0        0     2114 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/models/in_process/__init__.py
--rw-r--r--   0        0        0     2049 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/models/in_process/get_abi_tag.py
--rw-r--r--   0        0        0     6611 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/models/in_process/parse_setup.py
--rw-r--r--   0        0        0     1165 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/models/in_process/pep508.py
--rw-r--r--   0        0        0     1653 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/models/in_process/sysconfig_get_paths.py
--rw-r--r--   0        0        0     5701 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/models/markers.py
--rw-r--r--   0        0        0     3507 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/models/project_info.py
--rw-r--r--   0        0        0     2202 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/models/python.py
--rw-r--r--   0        0        0      318 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/models/python_max_versions.json
--rw-r--r--   0        0        0    22741 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/models/repositories.py
--rw-r--r--   0        0        0    18772 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/models/requirements.py
--rw-r--r--   0        0        0     2313 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/models/search.py
--rw-r--r--   0        0        0     3292 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/models/session.py
--rw-r--r--   0        0        0    14700 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/models/setup.py
--rw-r--r--   0        0        0    16725 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/models/specifiers.py
--rw-r--r--   0        0        0     2643 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/models/venv.py
--rw-r--r--   0        0        0     5924 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/models/versions.py
--rw-r--r--   0        0        0     3359 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/models/working_set.py
--rw-r--r--   0        0        0        0 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/pep582/__init__.py
--rw-r--r--   0        0        0     4481 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/pep582/sitecustomize.py
--rw-r--r--   0        0        0      134 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/project/__init__.py
--rw-r--r--   0        0        0    17114 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/project/config.py
--rw-r--r--   0        0        0    27025 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/project/core.py
--rw-r--r--   0        0        0     2194 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/project/lockfile.py
--rw-r--r--   0        0        0     3385 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/project/project_file.py
--rw-r--r--   0        0        0     1070 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/project/toml_file.py
--rw-r--r--   0        0        0        0 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/py.typed
--rw-r--r--   0        0        0    20149 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/pytest.py
--rw-r--r--   0        0        0       61 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/resolver/__init__.py
--rw-r--r--   0        0        0     2001 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/resolver/core.py
--rw-r--r--   0        0        0    13461 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/resolver/providers.py
--rw-r--r--   0        0        0     1577 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/resolver/python.py
--rw-r--r--   0        0        0     3790 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/resolver/reporters.py
--rw-r--r--   0        0        0     4027 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/signals.py
--rw-r--r--   0        0        0     8054 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/termui.py
--rw-r--r--   0        0        0    14441 2023-09-12 09:45:17.778705 pdm-2.9.2/src/pdm/utils.py
--rw-r--r--   0        0        0       72 2023-09-12 09:45:17.778705 pdm-2.9.2/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-09-12 09:45:17.778705 pdm-2.9.2/tests/cli/__init__.py
--rw-r--r--   0        0        0     3723 2023-09-12 09:45:17.778705 pdm-2.9.2/tests/cli/conftest.py
--rw-r--r--   0        0        0    12876 2023-09-12 09:45:17.778705 pdm-2.9.2/tests/cli/test_add.py
--rw-r--r--   0        0        0     5861 2023-09-12 09:45:17.778705 pdm-2.9.2/tests/cli/test_build.py
--rw-r--r--   0        0        0     5229 2023-09-12 09:45:17.778705 pdm-2.9.2/tests/cli/test_cache.py
--rw-r--r--   0        0        0     9286 2023-09-12 09:45:17.778705 pdm-2.9.2/tests/cli/test_config.py
--rw-r--r--   0        0        0     2029 2023-09-12 09:45:17.778705 pdm-2.9.2/tests/cli/test_fix.py
--rw-r--r--   0        0        0    10375 2023-09-12 09:45:17.778705 pdm-2.9.2/tests/cli/test_hooks.py
--rw-r--r--   0        0        0     4950 2023-09-12 09:45:17.778705 pdm-2.9.2/tests/cli/test_init.py
--rw-r--r--   0        0        0    11585 2023-09-12 09:45:17.778705 pdm-2.9.2/tests/cli/test_install.py
--rw-r--r--   0        0        0    30773 2023-09-12 09:45:17.778705 pdm-2.9.2/tests/cli/test_list.py
--rw-r--r--   0        0        0     6975 2023-09-12 09:45:17.778705 pdm-2.9.2/tests/cli/test_lock.py
--rw-r--r--   0        0        0     7796 2023-09-12 09:45:17.778705 pdm-2.9.2/tests/cli/test_others.py
--rw-r--r--   0        0        0     6060 2023-09-12 09:45:17.778705 pdm-2.9.2/tests/cli/test_publish.py
--rw-r--r--   0        0        0     4289 2023-09-12 09:45:17.778705 pdm-2.9.2/tests/cli/test_remove.py
--rw-r--r--   0        0        0    30204 2023-09-12 09:45:17.778705 pdm-2.9.2/tests/cli/test_run.py
--rw-r--r--   0        0        0     3599 2023-09-12 09:45:17.778705 pdm-2.9.2/tests/cli/test_self_command.py
--rw-r--r--   0        0        0     2796 2023-09-12 09:45:17.778705 pdm-2.9.2/tests/cli/test_template.py
--rw-r--r--   0        0        0     9260 2023-09-12 09:45:17.778705 pdm-2.9.2/tests/cli/test_update.py
--rw-r--r--   0        0        0     2997 2023-09-12 09:45:17.778705 pdm-2.9.2/tests/cli/test_use.py
--rw-r--r--   0        0        0    11698 2023-09-12 09:45:17.778705 pdm-2.9.2/tests/cli/test_venv.py
--rw-r--r--   0        0        0     3079 2023-09-12 09:45:17.778705 pdm-2.9.2/tests/conftest.py
--rw-r--r--   0        0        0      235 2023-09-12 09:45:17.778705 pdm-2.9.2/tests/fixtures/Pipfile
--rw-r--r--   0        0        0        0 2023-09-12 09:45:17.778705 pdm-2.9.2/tests/fixtures/__init__.py
--rw-r--r--   0        0        0    49497 2023-09-12 09:45:17.782705 pdm-2.9.2/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl
--rw-r--r--   0        0        0      546 2023-09-12 09:45:17.782705 pdm-2.9.2/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz
--rw-r--r--   0        0        0   422824 2023-09-12 09:45:17.782705 pdm-2.9.2/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1254 2023-09-12 09:45:17.782705 pdm-2.9.2/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl
--rw-r--r--   0        0        0     1254 2023-09-12 09:45:17.782705 pdm-2.9.2/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1038 2023-09-12 09:45:17.782705 pdm-2.9.2/tests/fixtures/artifacts/demo-0.0.1.tar.gz
--rw-r--r--   0        0        0     2615 2023-09-12 09:45:17.782705 pdm-2.9.2/tests/fixtures/artifacts/demo-0.0.1.zip
--rw-r--r--   0        0        0     4595 2023-09-12 09:45:17.782705 pdm-2.9.2/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl
--rw-r--r--   0        0        0     5359 2023-09-12 09:45:17.782705 pdm-2.9.2/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl
--rw-r--r--   0        0        0    56715 2023-09-12 09:45:17.782705 pdm-2.9.2/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl
--rw-r--r--   0        0        0     6138 2023-09-12 09:45:17.782705 pdm-2.9.2/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0     5786 2023-09-12 09:45:17.782705 pdm-2.9.2/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz
--rw-r--r--   0        0        0    17978 2023-09-12 09:45:17.782705 pdm-2.9.2/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl
--rw-r--r--   0        0        0    24489 2023-09-12 09:45:17.782705 pdm-2.9.2/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0    94569 2023-09-12 09:45:17.782705 pdm-2.9.2/tests/fixtures/artifacts/pdm_backend-2.1.4-py3-none-any.whl
--rw-r--r--   0        0        0     1401 2023-09-12 09:45:17.782705 pdm-2.9.2/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl
--rw-r--r--   0        0        0     1405 2023-09-12 09:45:17.782705 pdm-2.9.2/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl
--rw-r--r--   0        0        0   305481 2023-09-12 09:45:17.786705 pdm-2.9.2/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl
--rw-r--r--   0        0        0   531270 2023-09-12 09:45:17.790705 pdm-2.9.2/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl
--rw-r--r--   0        0        0  1232518 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl
--rw-r--r--   0        0        0    26662 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl
--rw-r--r--   0        0        0    35301 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl
--rw-r--r--   0        0        0     5312 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl
--rw-r--r--   0        0        0      326 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/index/demo.html
--rw-r--r--   0        0        0      511 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/index/future-fstrings.html
--rw-r--r--   0        0        0      262 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/index/pep345-legacy.html
--rw-r--r--   0        0        0      262 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/index/wheel.html
--rw-r--r--   0        0        0      285 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/poetry-error.toml
--rw-r--r--   0        0        0        0 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/__init__.py
--rw-r--r--   0        0        0       42 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-#-with-hash/demo.py
--rw-r--r--   0        0        0      332 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-#-with-hash/setup.py
--rw-r--r--   0        0        0       26 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-combined-extras/demo.py
--rw-r--r--   0        0        0      460 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-combined-extras/pyproject.toml
--rw-r--r--   0        0        0       42 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-failure-no-dep/demo.py
--rw-r--r--   0        0        0      246 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-failure-no-dep/setup.py
--rw-r--r--   0        0        0       42 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-failure/demo.py
--rw-r--r--   0        0        0      345 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-failure/setup.py
--rw-r--r--   0        0        0       12 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-module/LICENSE
--rw-r--r--   0        0        0       24 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-module/README.md
--rw-r--r--   0        0        0       14 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-module/bar_module.py
--rw-r--r--   0        0        0       36 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-module/foo_module.py
--rw-r--r--   0        0        0      450 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-module/pyproject.toml
--rw-r--r--   0        0        0     3983 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock
--rw-r--r--   0        0        0      316 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-package-has-dep-with-extras/pyproject.toml
--rw-r--r--   0        0        0      157 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-package-has-dep-with-extras/requirements.txt
--rw-r--r--   0        0        0       12 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-package/LICENSE
--rw-r--r--   0        0        0       13 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-package/README.md
--rw-r--r--   0        0        0       16 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-package/data_out.json
--rw-r--r--   0        0        0       22 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-package/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-package/my_package/data.json
--rw-r--r--   0        0        0    13807 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-package/pdm.lock
--rw-r--r--   0        0        0      580 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-package/pyproject.toml
--rw-r--r--   0        0        0      122 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-package/requirements.ini
--rw-r--r--   0        0        0     7521 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-package/requirements.txt
--rw-r--r--   0        0        0      211 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-package/requirements_simple.txt
--rw-r--r--   0        0        0      726 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-package/setup.txt
--rw-r--r--   0        0        0       21 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-package/single_module.py
--rw-r--r--   0        0        0       18 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-parent-package/README.md
--rw-r--r--   0        0        0       22 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-parent-package/package-a/foo.py
--rw-r--r--   0        0        0      120 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-parent-package/package-a/setup.py
--rw-r--r--   0        0        0       22 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-parent-package/package-b/bar.py
--rw-r--r--   0        0        0      202 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-parent-package/package-b/pyproject.toml
--rw-r--r--   0        0        0       42 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-prerelease/demo.py
--rw-r--r--   0        0        0      334 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-prerelease/setup.py
--rw-r--r--   0        0        0       12 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-src-package/LICENSE
--rw-r--r--   0        0        0       24 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-src-package/README.md
--rw-r--r--   0        0        0       16 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-src-package/data_out.json
--rw-r--r--   0        0        0      464 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-src-package/pyproject.toml
--rw-r--r--   0        0        0       21 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-src-package/single_module.py
--rw-r--r--   0        0        0       22 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo-src-package/src/my_package/data.json
--rw-r--r--   0        0        0       42 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo/demo.py
--rw-r--r--   0        0        0      344 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo/pyproject.toml
--rw-r--r--   0        0        0       26 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo_extras/demo.py
--rw-r--r--   0        0        0      250 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/demo_extras/setup.py
--rw-r--r--   0        0        0        0 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/flit-demo/README.rst
--rw-r--r--   0        0        0        0 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/flit-demo/doc/index.html
--rw-r--r--   0        0        0       49 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/flit-demo/flit.py
--rw-r--r--   0        0        0      969 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/flit-demo/pyproject.toml
--rw-r--r--   0        0        0       12 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/poetry-demo/mylib.py
--rw-r--r--   0        0        0      863 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/poetry-demo/pyproject.toml
--rw-r--r--   0        0        0        0 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/test-hatch-static/README.md
--rw-r--r--   0        0        0      386 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/test-hatch-static/pyproject.toml
--rw-r--r--   0        0        0       11 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/test-monorepo/README.md
--rw-r--r--   0        0        0        0 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/test-monorepo/core/core.py
--rw-r--r--   0        0        0      177 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/test-monorepo/core/pyproject.toml
--rw-r--r--   0        0        0        0 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/test-monorepo/package_a/alice.py
--rw-r--r--   0        0        0      229 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/test-monorepo/package_a/pyproject.toml
--rw-r--r--   0        0        0        0 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/test-monorepo/package_b/bob.py
--rw-r--r--   0        0        0      229 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/test-monorepo/package_b/pyproject.toml
--rw-r--r--   0        0        0      162 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/test-monorepo/pyproject.toml
--rw-r--r--   0        0        0      380 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/test-plugin-pdm/hello.py
--rw-r--r--   0        0        0      310 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/test-plugin-pdm/pyproject.toml
--rw-r--r--   0        0        0      380 2023-09-12 09:45:17.794705 pdm-2.9.2/tests/fixtures/projects/test-plugin/hello.py
--rw-r--r--   0        0        0      168 2023-09-12 09:45:17.798705 pdm-2.9.2/tests/fixtures/projects/test-plugin/setup.py
--rw-r--r--   0        0        0        0 2023-09-12 09:45:17.798705 pdm-2.9.2/tests/fixtures/projects/test-removal/__init__.py
--rw-r--r--   0        0        0        0 2023-09-12 09:45:17.798705 pdm-2.9.2/tests/fixtures/projects/test-removal/bar.py
--rw-r--r--   0        0        0        0 2023-09-12 09:45:17.798705 pdm-2.9.2/tests/fixtures/projects/test-removal/foo.py
--rw-r--r--   0        0        0        0 2023-09-12 09:45:17.798705 pdm-2.9.2/tests/fixtures/projects/test-removal/subdir/__init__.py
--rw-r--r--   0        0        0       10 2023-09-12 09:45:17.798705 pdm-2.9.2/tests/fixtures/projects/test-setuptools/AUTHORS
--rw-r--r--   0        0        0       12 2023-09-12 09:45:17.798705 pdm-2.9.2/tests/fixtures/projects/test-setuptools/README.md
--rw-r--r--   0        0        0       22 2023-09-12 09:45:17.798705 pdm-2.9.2/tests/fixtures/projects/test-setuptools/mymodule.py
--rw-r--r--   0        0        0      398 2023-09-12 09:45:17.798705 pdm-2.9.2/tests/fixtures/projects/test-setuptools/setup.cfg
--rw-r--r--   0        0        0      308 2023-09-12 09:45:17.798705 pdm-2.9.2/tests/fixtures/projects/test-setuptools/setup.py
--rw-r--r--   0        0        0     1525 2023-09-12 09:45:17.798705 pdm-2.9.2/tests/fixtures/pypi.json
--rw-r--r--   0        0        0     1330 2023-09-12 09:45:17.798705 pdm-2.9.2/tests/fixtures/pyproject.toml
--rw-r--r--   0        0        0       20 2023-09-12 09:45:17.798705 pdm-2.9.2/tests/fixtures/requirements-include.txt
--rw-r--r--   0        0        0      502 2023-09-12 09:45:17.798705 pdm-2.9.2/tests/fixtures/requirements.txt
--rw-r--r--   0        0        0        0 2023-09-12 09:45:17.798705 pdm-2.9.2/tests/models/__init__.py
--rw-r--r--   0        0        0     3800 2023-09-12 09:45:17.798705 pdm-2.9.2/tests/models/test_backends.py
--rw-r--r--   0        0        0    13450 2023-09-12 09:45:17.798705 pdm-2.9.2/tests/models/test_candidates.py
--rw-r--r--   0        0        0     1971 2023-09-12 09:45:17.798705 pdm-2.9.2/tests/models/test_marker.py
--rw-r--r--   0        0        0     2936 2023-09-12 09:45:17.798705 pdm-2.9.2/tests/models/test_requirements.py
--rw-r--r--   0        0        0     2556 2023-09-12 09:45:17.798705 pdm-2.9.2/tests/models/test_setup_parsing.py
--rw-r--r--   0        0        0     3590 2023-09-12 09:45:17.798705 pdm-2.9.2/tests/models/test_specifiers.py
--rw-r--r--   0        0        0     2703 2023-09-12 09:45:17.798705 pdm-2.9.2/tests/models/test_versions.py
--rw-r--r--   0        0        0        0 2023-09-12 09:45:17.798705 pdm-2.9.2/tests/resolver/__init__.py
--rw-r--r--   0        0        0    11567 2023-09-12 09:45:17.798705 pdm-2.9.2/tests/resolver/test_resolve.py
--rw-r--r--   0        0        0     8121 2023-09-12 09:45:17.798705 pdm-2.9.2/tests/test_formats.py
--rw-r--r--   0        0        0     7231 2023-09-12 09:45:17.798705 pdm-2.9.2/tests/test_installer.py
--rw-r--r--   0        0        0     1829 2023-09-12 09:45:17.798705 pdm-2.9.2/tests/test_integration.py
--rw-r--r--   0        0        0     3435 2023-09-12 09:45:17.798705 pdm-2.9.2/tests/test_plugin.py
--rw-r--r--   0        0        0    12115 2023-09-12 09:45:17.798705 pdm-2.9.2/tests/test_project.py
--rw-r--r--   0        0        0     1103 2023-09-12 09:45:17.798705 pdm-2.9.2/tests/test_signals.py
--rw-r--r--   0        0        0     4621 2023-09-12 09:45:17.798705 pdm-2.9.2/tests/test_utils.py
--rw-r--r--   0        0        0      203 2023-09-12 09:45:17.798705 pdm-2.9.2/tox.ini
--rw-r--r--   0        0        0    10130 1970-01-01 00:00:00.000000 pdm-2.9.2/PKG-INFO
+-rw-r--r--   0        0        0   133803 2023-09-25 09:22:56.551282 pdm-2.9.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1075 2023-09-25 09:22:56.551282 pdm-2.9.3/LICENSE
+-rw-r--r--   0        0        0     1075 2023-09-25 09:22:56.551282 pdm-2.9.3/LICENSE
+-rw-r--r--   0        0        0     8002 2023-09-25 09:22:56.551282 pdm-2.9.3/README.md
+-rw-r--r--   0        0        0     8002 2023-09-25 09:22:56.551282 pdm-2.9.3/README.md
+-rw-r--r--   0        0        0     4709 2023-09-25 09:23:06.859249 pdm-2.9.3/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/__main__.py
+-rw-r--r--   0        0        0      316 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/__version__.py
+-rw-r--r--   0        0        0     3413 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/_types.py
+-rw-r--r--   0        0        0      237 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/builders/__init__.py
+-rw-r--r--   0        0        0    11924 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/builders/base.py
+-rw-r--r--   0        0        0     1791 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/builders/editable.py
+-rw-r--r--   0        0        0      656 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/builders/sdist.py
+-rw-r--r--   0        0        0     1073 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/builders/wheel.py
+-rw-r--r--   0        0        0        0 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/__init__.py
+-rw-r--r--   0        0        0    16592 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/actions.py
+-rw-r--r--   0        0        0        0 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/commands/__init__.py
+-rw-r--r--   0        0        0     7146 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/commands/add.py
+-rw-r--r--   0        0        0     2871 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/commands/base.py
+-rw-r--r--   0        0        0     4236 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/commands/build.py
+-rw-r--r--   0        0        0     6542 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/commands/cache.py
+-rw-r--r--   0        0        0     1275 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/commands/completion.py
+-rw-r--r--   0        0        0     7537 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/commands/config.py
+-rw-r--r--   0        0        0     3066 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/commands/export.py
+-rw-r--r--   0        0        0     3136 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/commands/fix/__init__.py
+-rw-r--r--   0        0        0     2309 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/commands/fix/fixers.py
+-rw-r--r--   0        0        0     3679 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/commands/import_cmd.py
+-rw-r--r--   0        0        0     3032 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/commands/info.py
+-rw-r--r--   0        0        0    10723 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/commands/init.py
+-rw-r--r--   0        0        0     3961 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/commands/install.py
+-rw-r--r--   0        0        0    16678 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/commands/list.py
+-rw-r--r--   0        0        0     2645 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/commands/lock.py
+-rw-r--r--   0        0        0     6596 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/commands/publish/__init__.py
+-rw-r--r--   0        0        0     8112 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/commands/publish/package.py
+-rw-r--r--   0        0        0     6954 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/commands/publish/repository.py
+-rw-r--r--   0        0        0     4379 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/commands/remove.py
+-rw-r--r--   0        0        0    15923 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/commands/run.py
+-rw-r--r--   0        0        0     2437 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/commands/search.py
+-rw-r--r--   0        0        0     9371 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/commands/self_cmd.py
+-rw-r--r--   0        0        0     2896 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/commands/show.py
+-rw-r--r--   0        0        0     1507 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/commands/sync.py
+-rw-r--r--   0        0        0     7350 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/commands/update.py
+-rw-r--r--   0        0        0     6484 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/commands/use.py
+-rw-r--r--   0        0        0     1720 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/commands/venv/__init__.py
+-rw-r--r--   0        0        0     2519 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/commands/venv/activate.py
+-rw-r--r--   0        0        0     6149 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/commands/venv/backends.py
+-rw-r--r--   0        0        0     2156 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/commands/venv/create.py
+-rw-r--r--   0        0        0      820 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/commands/venv/list.py
+-rw-r--r--   0        0        0     2196 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/commands/venv/purge.py
+-rw-r--r--   0        0        0     1280 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/commands/venv/remove.py
+-rw-r--r--   0        0        0     2652 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/commands/venv/utils.py
+-rw-r--r--   0        0        0        0 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/completions/__init__.py
+-rw-r--r--   0        0        0     5210 2023-09-25 09:22:56.559281 pdm-2.9.3/src/pdm/cli/completions/pdm.bash
+-rw-r--r--   0        0        0    51762 2023-09-25 09:22:56.563282 pdm-2.9.3/src/pdm/cli/completions/pdm.fish
+-rw-r--r--   0        0        0    18961 2023-09-25 09:22:56.563282 pdm-2.9.3/src/pdm/cli/completions/pdm.ps1
+-rw-r--r--   0        0        0    25885 2023-09-25 09:22:56.563282 pdm-2.9.3/src/pdm/cli/completions/pdm.zsh
+-rw-r--r--   0        0        0     3840 2023-09-25 09:22:56.563282 pdm-2.9.3/src/pdm/cli/filters.py
+-rw-r--r--   0        0        0     1481 2023-09-25 09:22:56.563282 pdm-2.9.3/src/pdm/cli/hooks.py
+-rw-r--r--   0        0        0    10897 2023-09-25 09:22:56.563282 pdm-2.9.3/src/pdm/cli/options.py
+-rw-r--r--   0        0        0     6718 2023-09-25 09:22:56.563282 pdm-2.9.3/src/pdm/cli/templates/__init__.py
+-rw-r--r--   0        0        0     3102 2023-09-25 09:22:56.563282 pdm-2.9.3/src/pdm/cli/templates/default/.gitignore
+-rw-r--r--   0        0        0       18 2023-09-25 09:22:56.563282 pdm-2.9.3/src/pdm/cli/templates/default/README.md
+-rw-r--r--   0        0        0        0 2023-09-25 09:22:56.563282 pdm-2.9.3/src/pdm/cli/templates/default/__init__.py
+-rw-r--r--   0        0        0      278 2023-09-25 09:22:56.563282 pdm-2.9.3/src/pdm/cli/templates/default/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-09-25 09:22:56.563282 pdm-2.9.3/src/pdm/cli/templates/default/src/example_package/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-25 09:22:56.563282 pdm-2.9.3/src/pdm/cli/templates/default/tests/__init__.py
+-rw-r--r--   0        0        0    29245 2023-09-25 09:22:56.563282 pdm-2.9.3/src/pdm/cli/utils.py
+-rw-r--r--   0        0        0     2642 2023-09-25 09:22:56.563282 pdm-2.9.3/src/pdm/compat.py
+-rw-r--r--   0        0        0    10620 2023-09-25 09:22:56.563282 pdm-2.9.3/src/pdm/core.py
+-rw-r--r--   0        0        0      825 2023-09-25 09:22:56.563282 pdm-2.9.3/src/pdm/environments/__init__.py
+-rw-r--r--   0        0        0     9734 2023-09-25 09:22:56.563282 pdm-2.9.3/src/pdm/environments/base.py
+-rw-r--r--   0        0        0     4273 2023-09-25 09:22:56.563282 pdm-2.9.3/src/pdm/environments/local.py
+-rw-r--r--   0        0        0     2047 2023-09-25 09:22:56.563282 pdm-2.9.3/src/pdm/environments/python.py
+-rw-r--r--   0        0        0     1362 2023-09-25 09:22:56.563282 pdm-2.9.3/src/pdm/exceptions.py
+-rw-r--r--   0        0        0     1268 2023-09-25 09:22:56.563282 pdm-2.9.3/src/pdm/formats/__init__.py
+-rw-r--r--   0        0        0     3825 2023-09-25 09:22:56.563282 pdm-2.9.3/src/pdm/formats/base.py
+-rw-r--r--   0        0        0     5788 2023-09-25 09:22:56.563282 pdm-2.9.3/src/pdm/formats/flit.py
+-rw-r--r--   0        0        0     2614 2023-09-25 09:22:56.563282 pdm-2.9.3/src/pdm/formats/pipfile.py
+-rw-r--r--   0        0        0     7490 2023-09-25 09:22:56.563282 pdm-2.9.3/src/pdm/formats/poetry.py
+-rw-r--r--   0        0        0     7576 2023-09-25 09:22:56.563282 pdm-2.9.3/src/pdm/formats/requirements.py
+-rw-r--r--   0        0        0     2336 2023-09-25 09:22:56.563282 pdm-2.9.3/src/pdm/formats/setup_py.py
+-rw-r--r--   0        0        0      119 2023-09-25 09:22:56.563282 pdm-2.9.3/src/pdm/installers/__init__.py
+-rw-r--r--   0        0        0     1367 2023-09-25 09:22:56.563282 pdm-2.9.3/src/pdm/installers/core.py
+-rw-r--r--   0        0        0    11127 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/installers/installers.py
+-rw-r--r--   0        0        0     2092 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/installers/manager.py
+-rw-r--r--   0        0        0     2226 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/installers/packages.py
+-rw-r--r--   0        0        0    18570 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/installers/synchronizers.py
+-rw-r--r--   0        0        0    11150 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/installers/uninstallers.py
+-rw-r--r--   0        0        0        6 2023-09-25 09:23:06.835249 pdm-2.9.3/src/pdm/models/VERSION
+-rw-r--r--   0        0        0        0 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/models/__init__.py
+-rw-r--r--   0        0        0     3162 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/models/auth.py
+-rw-r--r--   0        0        0     4664 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/models/backends.py
+-rw-r--r--   0        0        0    12157 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/models/caches.py
+-rw-r--r--   0        0        0    26920 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/models/candidates.py
+-rw-r--r--   0        0        0      287 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/models/environment.py
+-rw-r--r--   0        0        0     2114 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/models/in_process/__init__.py
+-rw-r--r--   0        0        0     2049 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/models/in_process/get_abi_tag.py
+-rw-r--r--   0        0        0     6611 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/models/in_process/parse_setup.py
+-rw-r--r--   0        0        0     1165 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/models/in_process/pep508.py
+-rw-r--r--   0        0        0     1653 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/models/in_process/sysconfig_get_paths.py
+-rw-r--r--   0        0        0     5701 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/models/markers.py
+-rw-r--r--   0        0        0     3507 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/models/project_info.py
+-rw-r--r--   0        0        0     2202 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/models/python.py
+-rw-r--r--   0        0        0      318 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/models/python_max_versions.json
+-rw-r--r--   0        0        0    22741 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/models/repositories.py
+-rw-r--r--   0        0        0    18772 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/models/requirements.py
+-rw-r--r--   0        0        0     2313 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/models/search.py
+-rw-r--r--   0        0        0     3292 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/models/session.py
+-rw-r--r--   0        0        0    14700 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/models/setup.py
+-rw-r--r--   0        0        0    16725 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/models/specifiers.py
+-rw-r--r--   0        0        0     2643 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/models/venv.py
+-rw-r--r--   0        0        0     5924 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/models/versions.py
+-rw-r--r--   0        0        0     3359 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/models/working_set.py
+-rw-r--r--   0        0        0        0 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/pep582/__init__.py
+-rw-r--r--   0        0        0     4481 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/pep582/sitecustomize.py
+-rw-r--r--   0        0        0      134 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/project/__init__.py
+-rw-r--r--   0        0        0    17114 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/project/config.py
+-rw-r--r--   0        0        0    27049 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/project/core.py
+-rw-r--r--   0        0        0     2194 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/project/lockfile.py
+-rw-r--r--   0        0        0     3385 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/project/project_file.py
+-rw-r--r--   0        0        0     1070 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/project/toml_file.py
+-rw-r--r--   0        0        0        0 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/py.typed
+-rw-r--r--   0        0        0    20149 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/pytest.py
+-rw-r--r--   0        0        0       61 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/resolver/__init__.py
+-rw-r--r--   0        0        0     2001 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/resolver/core.py
+-rw-r--r--   0        0        0    14214 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/resolver/providers.py
+-rw-r--r--   0        0        0     1577 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/resolver/python.py
+-rw-r--r--   0        0        0     3945 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/resolver/reporters.py
+-rw-r--r--   0        0        0     4027 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/signals.py
+-rw-r--r--   0        0        0     8054 2023-09-25 09:22:56.567282 pdm-2.9.3/src/pdm/termui.py
+-rw-r--r--   0        0        0    14441 2023-09-25 09:22:56.571282 pdm-2.9.3/src/pdm/utils.py
+-rw-r--r--   0        0        0       72 2023-09-25 09:22:56.571282 pdm-2.9.3/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-25 09:22:56.571282 pdm-2.9.3/tests/cli/__init__.py
+-rw-r--r--   0        0        0     3723 2023-09-25 09:22:56.571282 pdm-2.9.3/tests/cli/conftest.py
+-rw-r--r--   0        0        0    12876 2023-09-25 09:22:56.571282 pdm-2.9.3/tests/cli/test_add.py
+-rw-r--r--   0        0        0     5861 2023-09-25 09:22:56.571282 pdm-2.9.3/tests/cli/test_build.py
+-rw-r--r--   0        0        0     5229 2023-09-25 09:22:56.571282 pdm-2.9.3/tests/cli/test_cache.py
+-rw-r--r--   0        0        0     9286 2023-09-25 09:22:56.571282 pdm-2.9.3/tests/cli/test_config.py
+-rw-r--r--   0        0        0     2029 2023-09-25 09:22:56.571282 pdm-2.9.3/tests/cli/test_fix.py
+-rw-r--r--   0        0        0    10375 2023-09-25 09:22:56.571282 pdm-2.9.3/tests/cli/test_hooks.py
+-rw-r--r--   0        0        0     4950 2023-09-25 09:22:56.571282 pdm-2.9.3/tests/cli/test_init.py
+-rw-r--r--   0        0        0    11585 2023-09-25 09:22:56.571282 pdm-2.9.3/tests/cli/test_install.py
+-rw-r--r--   0        0        0    30773 2023-09-25 09:22:56.571282 pdm-2.9.3/tests/cli/test_list.py
+-rw-r--r--   0        0        0     6975 2023-09-25 09:22:56.571282 pdm-2.9.3/tests/cli/test_lock.py
+-rw-r--r--   0        0        0     7796 2023-09-25 09:22:56.571282 pdm-2.9.3/tests/cli/test_others.py
+-rw-r--r--   0        0        0     6060 2023-09-25 09:22:56.571282 pdm-2.9.3/tests/cli/test_publish.py
+-rw-r--r--   0        0        0     4289 2023-09-25 09:22:56.571282 pdm-2.9.3/tests/cli/test_remove.py
+-rw-r--r--   0        0        0    30204 2023-09-25 09:22:56.571282 pdm-2.9.3/tests/cli/test_run.py
+-rw-r--r--   0        0        0     3599 2023-09-25 09:22:56.571282 pdm-2.9.3/tests/cli/test_self_command.py
+-rw-r--r--   0        0        0     2796 2023-09-25 09:22:56.571282 pdm-2.9.3/tests/cli/test_template.py
+-rw-r--r--   0        0        0     9260 2023-09-25 09:22:56.571282 pdm-2.9.3/tests/cli/test_update.py
+-rw-r--r--   0        0        0     2997 2023-09-25 09:22:56.571282 pdm-2.9.3/tests/cli/test_use.py
+-rw-r--r--   0        0        0    11698 2023-09-25 09:22:56.571282 pdm-2.9.3/tests/cli/test_venv.py
+-rw-r--r--   0        0        0     3079 2023-09-25 09:22:56.571282 pdm-2.9.3/tests/conftest.py
+-rw-r--r--   0        0        0      235 2023-09-25 09:22:56.571282 pdm-2.9.3/tests/fixtures/Pipfile
+-rw-r--r--   0        0        0        0 2023-09-25 09:22:56.571282 pdm-2.9.3/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0    49497 2023-09-25 09:22:56.571282 pdm-2.9.3/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl
+-rw-r--r--   0        0        0      546 2023-09-25 09:22:56.571282 pdm-2.9.3/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz
+-rw-r--r--   0        0        0   422824 2023-09-25 09:22:56.575281 pdm-2.9.3/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1254 2023-09-25 09:22:56.575281 pdm-2.9.3/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl
+-rw-r--r--   0        0        0     1254 2023-09-25 09:22:56.575281 pdm-2.9.3/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1038 2023-09-25 09:22:56.575281 pdm-2.9.3/tests/fixtures/artifacts/demo-0.0.1.tar.gz
+-rw-r--r--   0        0        0     2615 2023-09-25 09:22:56.575281 pdm-2.9.3/tests/fixtures/artifacts/demo-0.0.1.zip
+-rw-r--r--   0        0        0     4595 2023-09-25 09:22:56.575281 pdm-2.9.3/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl
+-rw-r--r--   0        0        0     5359 2023-09-25 09:22:56.575281 pdm-2.9.3/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl
+-rw-r--r--   0        0        0    56715 2023-09-25 09:22:56.575281 pdm-2.9.3/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl
+-rw-r--r--   0        0        0     6138 2023-09-25 09:22:56.575281 pdm-2.9.3/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     5786 2023-09-25 09:22:56.575281 pdm-2.9.3/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz
+-rw-r--r--   0        0        0    17978 2023-09-25 09:22:56.575281 pdm-2.9.3/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl
+-rw-r--r--   0        0        0    24489 2023-09-25 09:22:56.575281 pdm-2.9.3/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0    94569 2023-09-25 09:22:56.575281 pdm-2.9.3/tests/fixtures/artifacts/pdm_backend-2.1.4-py3-none-any.whl
+-rw-r--r--   0        0        0     1401 2023-09-25 09:22:56.575281 pdm-2.9.3/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl
+-rw-r--r--   0        0        0     1405 2023-09-25 09:22:56.575281 pdm-2.9.3/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl
+-rw-r--r--   0        0        0   305481 2023-09-25 09:22:56.579281 pdm-2.9.3/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl
+-rw-r--r--   0        0        0   531270 2023-09-25 09:22:56.583281 pdm-2.9.3/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl
+-rw-r--r--   0        0        0   804037 2023-09-25 09:22:56.587281 pdm-2.9.3/tests/fixtures/artifacts/setuptools-68.0.0-py3-none-any.whl
+-rw-r--r--   0        0        0    26662 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl
+-rw-r--r--   0        0        0    35301 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     5312 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl
+-rw-r--r--   0        0        0      326 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/index/demo.html
+-rw-r--r--   0        0        0      511 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/index/future-fstrings.html
+-rw-r--r--   0        0        0      262 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/index/pep345-legacy.html
+-rw-r--r--   0        0        0      262 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/index/wheel.html
+-rw-r--r--   0        0        0      285 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/poetry-error.toml
+-rw-r--r--   0        0        0        0 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/__init__.py
+-rw-r--r--   0        0        0       42 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-#-with-hash/demo.py
+-rw-r--r--   0        0        0      332 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-#-with-hash/setup.py
+-rw-r--r--   0        0        0       26 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-combined-extras/demo.py
+-rw-r--r--   0        0        0      460 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-combined-extras/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-failure-no-dep/demo.py
+-rw-r--r--   0        0        0      246 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-failure-no-dep/setup.py
+-rw-r--r--   0        0        0       42 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-failure/demo.py
+-rw-r--r--   0        0        0      345 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-failure/setup.py
+-rw-r--r--   0        0        0       12 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-module/LICENSE
+-rw-r--r--   0        0        0       24 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-module/README.md
+-rw-r--r--   0        0        0       14 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-module/bar_module.py
+-rw-r--r--   0        0        0       36 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-module/foo_module.py
+-rw-r--r--   0        0        0      450 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-module/pyproject.toml
+-rw-r--r--   0        0        0     3983 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock
+-rw-r--r--   0        0        0      316 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-package-has-dep-with-extras/pyproject.toml
+-rw-r--r--   0        0        0      157 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-package-has-dep-with-extras/requirements.txt
+-rw-r--r--   0        0        0       12 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-package/LICENSE
+-rw-r--r--   0        0        0       13 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-package/README.md
+-rw-r--r--   0        0        0       16 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-package/data_out.json
+-rw-r--r--   0        0        0       22 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-package/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-package/my_package/data.json
+-rw-r--r--   0        0        0    13807 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-package/pdm.lock
+-rw-r--r--   0        0        0      580 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-package/pyproject.toml
+-rw-r--r--   0        0        0      122 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-package/requirements.ini
+-rw-r--r--   0        0        0     7521 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-package/requirements.txt
+-rw-r--r--   0        0        0      211 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-package/requirements_simple.txt
+-rw-r--r--   0        0        0      726 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-package/setup.txt
+-rw-r--r--   0        0        0       21 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-package/single_module.py
+-rw-r--r--   0        0        0       18 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-parent-package/README.md
+-rw-r--r--   0        0        0       22 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-parent-package/package-a/foo.py
+-rw-r--r--   0        0        0      120 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-parent-package/package-a/setup.py
+-rw-r--r--   0        0        0       22 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-parent-package/package-b/bar.py
+-rw-r--r--   0        0        0      202 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-parent-package/package-b/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-prerelease/demo.py
+-rw-r--r--   0        0        0      334 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-prerelease/setup.py
+-rw-r--r--   0        0        0       12 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-src-package/LICENSE
+-rw-r--r--   0        0        0       24 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-src-package/README.md
+-rw-r--r--   0        0        0       16 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-src-package/data_out.json
+-rw-r--r--   0        0        0      464 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-src-package/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-src-package/single_module.py
+-rw-r--r--   0        0        0       22 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo-src-package/src/my_package/data.json
+-rw-r--r--   0        0        0       42 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo/demo.py
+-rw-r--r--   0        0        0      344 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo/pyproject.toml
+-rw-r--r--   0        0        0       26 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo_extras/demo.py
+-rw-r--r--   0        0        0      250 2023-09-25 09:22:56.591282 pdm-2.9.3/tests/fixtures/projects/demo_extras/setup.py
+-rw-r--r--   0        0        0        0 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/fixtures/projects/flit-demo/README.rst
+-rw-r--r--   0        0        0        0 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/fixtures/projects/flit-demo/doc/index.html
+-rw-r--r--   0        0        0       49 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/fixtures/projects/flit-demo/flit.py
+-rw-r--r--   0        0        0      969 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/fixtures/projects/flit-demo/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/fixtures/projects/poetry-demo/mylib.py
+-rw-r--r--   0        0        0      863 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/fixtures/projects/poetry-demo/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/fixtures/projects/test-hatch-static/README.md
+-rw-r--r--   0        0        0      386 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/fixtures/projects/test-hatch-static/pyproject.toml
+-rw-r--r--   0        0        0       11 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/fixtures/projects/test-monorepo/README.md
+-rw-r--r--   0        0        0        0 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/fixtures/projects/test-monorepo/core/core.py
+-rw-r--r--   0        0        0      177 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/fixtures/projects/test-monorepo/core/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/fixtures/projects/test-monorepo/package_a/alice.py
+-rw-r--r--   0        0        0      229 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/fixtures/projects/test-monorepo/package_a/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/fixtures/projects/test-monorepo/package_b/bob.py
+-rw-r--r--   0        0        0      229 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/fixtures/projects/test-monorepo/package_b/pyproject.toml
+-rw-r--r--   0        0        0      162 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/fixtures/projects/test-monorepo/pyproject.toml
+-rw-r--r--   0        0        0      380 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/fixtures/projects/test-plugin-pdm/hello.py
+-rw-r--r--   0        0        0      310 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/fixtures/projects/test-plugin-pdm/pyproject.toml
+-rw-r--r--   0        0        0      380 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/fixtures/projects/test-plugin/hello.py
+-rw-r--r--   0        0        0      168 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/fixtures/projects/test-plugin/setup.py
+-rw-r--r--   0        0        0        0 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/fixtures/projects/test-removal/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/fixtures/projects/test-removal/bar.py
+-rw-r--r--   0        0        0        0 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/fixtures/projects/test-removal/foo.py
+-rw-r--r--   0        0        0        0 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/fixtures/projects/test-removal/subdir/__init__.py
+-rw-r--r--   0        0        0       10 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/fixtures/projects/test-setuptools/AUTHORS
+-rw-r--r--   0        0        0       12 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/fixtures/projects/test-setuptools/README.md
+-rw-r--r--   0        0        0       22 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/fixtures/projects/test-setuptools/mymodule.py
+-rw-r--r--   0        0        0      398 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/fixtures/projects/test-setuptools/setup.cfg
+-rw-r--r--   0        0        0      308 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/fixtures/projects/test-setuptools/setup.py
+-rw-r--r--   0        0        0     1525 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/fixtures/pypi.json
+-rw-r--r--   0        0        0     1330 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/fixtures/pyproject.toml
+-rw-r--r--   0        0        0       20 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/fixtures/requirements-include.txt
+-rw-r--r--   0        0        0      502 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/fixtures/requirements.txt
+-rw-r--r--   0        0        0        0 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/models/__init__.py
+-rw-r--r--   0        0        0     3800 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/models/test_backends.py
+-rw-r--r--   0        0        0    13450 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/models/test_candidates.py
+-rw-r--r--   0        0        0     1971 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/models/test_marker.py
+-rw-r--r--   0        0        0     2936 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/models/test_requirements.py
+-rw-r--r--   0        0        0     2556 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/models/test_setup_parsing.py
+-rw-r--r--   0        0        0     3590 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/models/test_specifiers.py
+-rw-r--r--   0        0        0     2703 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/models/test_versions.py
+-rw-r--r--   0        0        0        0 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/resolver/__init__.py
+-rw-r--r--   0        0        0    11860 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/resolver/test_resolve.py
+-rw-r--r--   0        0        0     8121 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/test_formats.py
+-rw-r--r--   0        0        0     7231 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/test_installer.py
+-rw-r--r--   0        0        0     1829 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/test_integration.py
+-rw-r--r--   0        0        0     3435 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/test_plugin.py
+-rw-r--r--   0        0        0    12115 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/test_project.py
+-rw-r--r--   0        0        0     1103 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/test_signals.py
+-rw-r--r--   0        0        0     4621 2023-09-25 09:22:56.595281 pdm-2.9.3/tests/test_utils.py
+-rw-r--r--   0        0        0      203 2023-09-25 09:22:56.595281 pdm-2.9.3/tox.ini
+-rw-r--r--   0        0        0    10130 1970-01-01 00:00:00.000000 pdm-2.9.3/PKG-INFO
```

### Comparing `pdm-2.9.2/CHANGELOG.md` & `pdm-2.9.3/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Release v2.9.3 (2023-09-25)
+---------------------------
+
+### Bug Fixes
+
+- Revert the changes to the behavior of installing self, introduced in #2162.
+  Self package won't be installed when `--no-default` is requested. [#2230](https://github.com/pdm-project/pdm/issues/2230)
+- Reject the candidate if it contains invalid metadata, to avoid a crash in the process of resolution. [#2261](https://github.com/pdm-project/pdm/issues/2261)
+
+### Documentation
+
+- Clarify what `--no-isolated` does. [#2071](https://github.com/pdm-project/pdm/issues/2071)
+
+
 Release v2.9.2 (2023-09-12)
 ---------------------------
 
 ### Features & Improvements
 
 - Fix an issue that `--no-lock` option doesn't work as expected. Also support `--no-lock` option for `add`, `remove` and `update` commands. [#2245](https://github.com/pdm-project/pdm/issues/2245)
```

### Comparing `pdm-2.9.2/LICENSE` & `pdm-2.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/README.md` & `pdm-2.9.3/README.md`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/pyproject.toml` & `pdm-2.9.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "packaging>=20.9,!=22.0",
     "platformdirs",
     "rich>=12.3.0",
     "virtualenv>=20",
     "pyproject-hooks",
     "requests-toolbelt",
     "unearth>=0.10.0",
-    "findpython>=0.3.0,<1.0.0a0",
+    "findpython>=0.4.0,<1.0.0a0",
     "tomlkit>=0.11.1,<1",
     "shellingham>=1.3.2",
     "python-dotenv>=0.15",
     "resolvelib>=1.0.1",
     "installer<0.8,>=0.7",
     "cachecontrol[filecache]>=0.13.0",
     "truststore; python_version >= \"3.10\"",
@@ -39,15 +39,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-version = "2.9.2"
+version = "2.9.3"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://pdm.fming.dev"
 Repository = "https://github.com/pdm-project/pdm"
```

### Comparing `pdm-2.9.2/src/pdm/_types.py` & `pdm-2.9.3/src/pdm/_types.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/builders/base.py` & `pdm-2.9.3/src/pdm/builders/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/builders/editable.py` & `pdm-2.9.3/src/pdm/builders/editable.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/builders/sdist.py` & `pdm-2.9.3/src/pdm/builders/sdist.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/builders/wheel.py` & `pdm-2.9.3/src/pdm/builders/wheel.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/actions.py` & `pdm-2.9.3/src/pdm/cli/actions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/commands/add.py` & `pdm-2.9.3/src/pdm/cli/commands/add.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/commands/base.py` & `pdm-2.9.3/src/pdm/cli/commands/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/commands/build.py` & `pdm-2.9.3/src/pdm/cli/commands/build.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/commands/cache.py` & `pdm-2.9.3/src/pdm/cli/commands/cache.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/commands/completion.py` & `pdm-2.9.3/src/pdm/cli/commands/completion.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/commands/config.py` & `pdm-2.9.3/src/pdm/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/commands/export.py` & `pdm-2.9.3/src/pdm/cli/commands/export.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/commands/fix/__init__.py` & `pdm-2.9.3/src/pdm/cli/commands/fix/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/commands/fix/fixers.py` & `pdm-2.9.3/src/pdm/cli/commands/fix/fixers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/commands/import_cmd.py` & `pdm-2.9.3/src/pdm/cli/commands/import_cmd.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/commands/info.py` & `pdm-2.9.3/src/pdm/cli/commands/info.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/commands/init.py` & `pdm-2.9.3/src/pdm/cli/commands/init.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/commands/install.py` & `pdm-2.9.3/src/pdm/cli/commands/install.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,12 +97,12 @@
                 groups=lock_selection.all(),
             )
 
         actions.do_sync(
             project,
             selection=selection,
             no_editable=options.no_editable,
-            no_self=options.no_self,
+            no_self=options.no_self or "default" not in selection,
             dry_run=options.dry_run,
             fail_fast=options.fail_fast,
             hooks=hooks,
         )
```

### Comparing `pdm-2.9.2/src/pdm/cli/commands/list.py` & `pdm-2.9.3/src/pdm/cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/commands/lock.py` & `pdm-2.9.3/src/pdm/cli/commands/lock.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/commands/publish/__init__.py` & `pdm-2.9.3/src/pdm/cli/commands/publish/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/commands/publish/package.py` & `pdm-2.9.3/src/pdm/cli/commands/publish/package.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/commands/publish/repository.py` & `pdm-2.9.3/src/pdm/cli/commands/publish/repository.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/commands/remove.py` & `pdm-2.9.3/src/pdm/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/commands/run.py` & `pdm-2.9.3/src/pdm/cli/commands/run.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/commands/search.py` & `pdm-2.9.3/src/pdm/cli/commands/search.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/commands/self_cmd.py` & `pdm-2.9.3/src/pdm/cli/commands/self_cmd.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/commands/show.py` & `pdm-2.9.3/src/pdm/cli/commands/show.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/commands/sync.py` & `pdm-2.9.3/src/pdm/cli/commands/sync.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,18 +36,19 @@
             "--reinstall",
             action="store_true",
             help="Force reinstall existing dependencies",
         )
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:
         actions.check_lockfile(project)
+        selection = GroupSelection.from_options(project, options)
         actions.do_sync(
             project,
-            selection=GroupSelection.from_options(project, options),
+            selection=selection,
             dry_run=options.dry_run,
             clean=options.clean,
             no_editable=options.no_editable,
-            no_self=options.no_self,
+            no_self=options.no_self or "default" not in selection,
             reinstall=options.reinstall,
             only_keep=options.only_keep,
             hooks=HookManager(project, options.skip),
         )
```

### Comparing `pdm-2.9.2/src/pdm/cli/commands/update.py` & `pdm-2.9.3/src/pdm/cli/commands/update.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,11 +185,11 @@
                 project,
                 selection=selection,
                 clean=False,
                 dry_run=dry_run,
                 requirements=[r for deps in updated_deps.values() for r in deps.values()],
                 tracked_names=list(chain.from_iterable(updated_deps.values())) if top else None,
                 no_editable=no_editable,
-                no_self=no_self,
+                no_self=no_self or "default" not in selection,
                 fail_fast=fail_fast,
                 hooks=hooks,
             )
```

### Comparing `pdm-2.9.2/src/pdm/cli/commands/use.py` & `pdm-2.9.3/src/pdm/cli/commands/use.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/commands/venv/__init__.py` & `pdm-2.9.3/src/pdm/cli/commands/venv/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/commands/venv/activate.py` & `pdm-2.9.3/src/pdm/cli/commands/venv/activate.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/commands/venv/backends.py` & `pdm-2.9.3/src/pdm/cli/commands/venv/backends.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/commands/venv/create.py` & `pdm-2.9.3/src/pdm/cli/commands/venv/create.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/commands/venv/list.py` & `pdm-2.9.3/src/pdm/cli/commands/venv/list.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/commands/venv/purge.py` & `pdm-2.9.3/src/pdm/cli/commands/venv/purge.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/commands/venv/remove.py` & `pdm-2.9.3/src/pdm/cli/commands/venv/remove.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/commands/venv/utils.py` & `pdm-2.9.3/src/pdm/cli/commands/venv/utils.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/completions/pdm.bash` & `pdm-2.9.3/src/pdm/cli/completions/pdm.bash`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/completions/pdm.fish` & `pdm-2.9.3/src/pdm/cli/completions/pdm.fish`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/completions/pdm.ps1` & `pdm-2.9.3/src/pdm/cli/completions/pdm.ps1`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/completions/pdm.zsh` & `pdm-2.9.3/src/pdm/cli/completions/pdm.zsh`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/filters.py` & `pdm-2.9.3/src/pdm/cli/filters.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/hooks.py` & `pdm-2.9.3/src/pdm/cli/hooks.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/options.py` & `pdm-2.9.3/src/pdm/cli/options.py`

 * *Files 3% similar despite different names*

```diff
@@ -168,15 +168,21 @@
     default=bool(os.getenv("PDM_NO_SELF")),
     dest="no_self",
     help="Don't install the project itself. [env var: PDM_NO_SELF]",
 )
 install_group.add_argument("--fail-fast", "-x", action="store_true", help="Abort on first installation error")
 
 
-@Option("--no-isolation", dest="build_isolation", nargs=0, help="Do not isolate the build in a clean environment")
+@Option(
+    "--no-isolation",
+    dest="build_isolation",
+    nargs=0,
+    help="Disable isolation when building a source distribution that follows PEP 517, "
+    "as in: build dependencies specified by PEP 518 must be already installed if this option is used.",
+)
 def no_isolation_option(project: Project, namespace: argparse.Namespace, values: str | Sequence[Any] | None) -> None:
     os.environ["PDM_BUILD_ISOLATION"] = "no"
 
 
 install_group.options.append(no_isolation_option)
 
 groups_group = ArgumentGroup("Dependencies selection")
```

### Comparing `pdm-2.9.2/src/pdm/cli/templates/__init__.py` & `pdm-2.9.3/src/pdm/cli/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/templates/default/.gitignore` & `pdm-2.9.3/src/pdm/cli/templates/default/.gitignore`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/cli/utils.py` & `pdm-2.9.3/src/pdm/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/compat.py` & `pdm-2.9.3/src/pdm/compat.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/core.py` & `pdm-2.9.3/src/pdm/core.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/environments/__init__.py` & `pdm-2.9.3/src/pdm/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/environments/base.py` & `pdm-2.9.3/src/pdm/environments/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/environments/local.py` & `pdm-2.9.3/src/pdm/environments/local.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/environments/python.py` & `pdm-2.9.3/src/pdm/environments/python.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/exceptions.py` & `pdm-2.9.3/src/pdm/exceptions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/formats/__init__.py` & `pdm-2.9.3/src/pdm/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/formats/base.py` & `pdm-2.9.3/src/pdm/formats/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/formats/flit.py` & `pdm-2.9.3/src/pdm/formats/flit.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/formats/pipfile.py` & `pdm-2.9.3/src/pdm/formats/pipfile.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/formats/poetry.py` & `pdm-2.9.3/src/pdm/formats/poetry.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/formats/requirements.py` & `pdm-2.9.3/src/pdm/formats/requirements.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/formats/setup_py.py` & `pdm-2.9.3/src/pdm/formats/setup_py.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/installers/core.py` & `pdm-2.9.3/src/pdm/installers/core.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/installers/installers.py` & `pdm-2.9.3/src/pdm/installers/installers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/installers/manager.py` & `pdm-2.9.3/src/pdm/installers/manager.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/installers/packages.py` & `pdm-2.9.3/src/pdm/installers/packages.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/installers/synchronizers.py` & `pdm-2.9.3/src/pdm/installers/synchronizers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/installers/uninstallers.py` & `pdm-2.9.3/src/pdm/installers/uninstallers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/models/auth.py` & `pdm-2.9.3/src/pdm/models/auth.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/models/backends.py` & `pdm-2.9.3/src/pdm/models/backends.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/models/caches.py` & `pdm-2.9.3/src/pdm/models/caches.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/models/candidates.py` & `pdm-2.9.3/src/pdm/models/candidates.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/models/in_process/__init__.py` & `pdm-2.9.3/src/pdm/models/in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/models/in_process/get_abi_tag.py` & `pdm-2.9.3/src/pdm/models/in_process/get_abi_tag.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/models/in_process/parse_setup.py` & `pdm-2.9.3/src/pdm/models/in_process/parse_setup.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/models/in_process/pep508.py` & `pdm-2.9.3/src/pdm/models/in_process/pep508.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/models/in_process/sysconfig_get_paths.py` & `pdm-2.9.3/src/pdm/models/in_process/sysconfig_get_paths.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/models/markers.py` & `pdm-2.9.3/src/pdm/models/markers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/models/project_info.py` & `pdm-2.9.3/src/pdm/models/project_info.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/models/python.py` & `pdm-2.9.3/src/pdm/models/python.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/models/repositories.py` & `pdm-2.9.3/src/pdm/models/repositories.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/models/requirements.py` & `pdm-2.9.3/src/pdm/models/requirements.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/models/search.py` & `pdm-2.9.3/src/pdm/models/search.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/models/session.py` & `pdm-2.9.3/src/pdm/models/session.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/models/setup.py` & `pdm-2.9.3/src/pdm/models/setup.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/models/specifiers.py` & `pdm-2.9.3/src/pdm/models/specifiers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/models/venv.py` & `pdm-2.9.3/src/pdm/models/venv.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/models/versions.py` & `pdm-2.9.3/src/pdm/models/versions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/models/working_set.py` & `pdm-2.9.3/src/pdm/models/working_set.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/pep582/sitecustomize.py` & `pdm-2.9.3/src/pdm/pep582/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/project/config.py` & `pdm-2.9.3/src/pdm/project/config.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/project/core.py` & `pdm-2.9.3/src/pdm/project/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -643,15 +643,15 @@
                 if len(path.parts) == 1:  # only check for spec with only one part
                     python = shutil.which(python_spec)
                     if python:
                         yield PythonInfo.from_path(python)
                         return
             finder_arg = python_spec
         finder = self._get_python_finder()
-        for entry in finder.find_all(finder_arg):
+        for entry in finder.find_all(finder_arg, allow_prereleases=True):
             yield PythonInfo(entry)
         if not python_spec:
             # Lastly, return the host Python as well
             this_python = getattr(sys, "_base_executable", sys.executable)
             yield PythonInfo.from_path(this_python)
 
     def _get_python_finder(self) -> Finder:
```

### Comparing `pdm-2.9.2/src/pdm/project/lockfile.py` & `pdm-2.9.3/src/pdm/project/lockfile.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/project/project_file.py` & `pdm-2.9.3/src/pdm/project/project_file.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/project/toml_file.py` & `pdm-2.9.3/src/pdm/project/toml_file.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/pytest.py` & `pdm-2.9.3/src/pdm/pytest.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/resolver/core.py` & `pdm-2.9.3/src/pdm/resolver/core.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/resolver/providers.py` & `pdm-2.9.3/src/pdm/resolver/providers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from __future__ import annotations
 
 import itertools
 import os
 from typing import TYPE_CHECKING, Callable, cast
 
 from packaging.specifiers import InvalidSpecifier, SpecifierSet
-from resolvelib import AbstractProvider
+from resolvelib import AbstractProvider, RequirementsConflicted
+from resolvelib.resolvers import Criterion
 
+from pdm.exceptions import InvalidPyVersion, RequirementError
 from pdm.models.candidates import Candidate, make_candidate
 from pdm.models.repositories import LockedRepository
 from pdm.models.requirements import FileRequirement, parse_requirement, strip_extras
 from pdm.resolver.python import (
     PythonCandidate,
     PythonRequirement,
     find_python_matches,
     is_python_satisfied_by,
 )
+from pdm.termui import logger
 from pdm.utils import is_url, url_without_fragments
 
 if TYPE_CHECKING:
     from typing import Any, Iterable, Iterator, Mapping, Sequence
 
     from resolvelib.resolvers import RequirementInformation
 
@@ -77,17 +80,23 @@
         else:
             parent_depths = (
                 self._known_depth[parent.identify()] if parent is not None else 0
                 for _, parent in information[identifier]
             )
             dep_depth = min(parent_depths, default=0) + 1
         # Use the REAL identifier as it may be updated after candidate preparation.
-        candidate = next(candidates[identifier])
+        deps: list[Requirement] = []
+        for candidate in candidates[identifier]:
+            try:
+                deps = self.get_dependencies(candidate)
+            except RequirementsConflicted:
+                continue
+            break
         self._known_depth[self.identify(candidate)] = dep_depth
-        is_backtrack_cause = any(dep.identify() in backtrack_identifiers for dep in self.get_dependencies(candidate))
+        is_backtrack_cause = any(dep.identify() in backtrack_identifiers for dep in deps)
         is_file_or_url = any(not requirement.is_named for requirement, _ in information[identifier])
         operators = [
             spec.operator for req, _ in information[identifier] if req.specifier is not None for spec in req.specifier
         ]
         is_python = identifier == "python"
         is_pinned = any(op[:2] == "==" for op in operators)
         constraints = len(operators)
@@ -179,15 +188,21 @@
         # 2) the candidate doesn't come from PyPI index.
         allow_prereleases = self.allow_prereleases in (True, None) or not candidate.req.is_named
         return cast(SpecifierSet, requirement.specifier).contains(version, allow_prereleases)
 
     def get_dependencies(self, candidate: Candidate) -> list[Requirement]:
         if isinstance(candidate, PythonCandidate):
             return []
-        deps, requires_python, _ = self.repository.get_dependencies(candidate)
+        try:
+            deps, requires_python, _ = self.repository.get_dependencies(candidate)
+        except (RequirementError, InvalidPyVersion, InvalidSpecifier) as e:
+            # When the metadata is invalid, skip this candidate by marking it as conflicting.
+            # Here we pass an empty criterion so it doesn't provide any info to the resolution.
+            logger.error("Invalid metadata in %s: %s", candidate, e)
+            raise RequirementsConflicted(Criterion([], [], [])) from None
 
         # Filter out incompatible dependencies(e.g. functools32) early so that
         # we don't get errors when building wheels.
         valid_deps: list[Requirement] = []
         for dep in deps:
             if (
                 dep.requires_python
```

### Comparing `pdm-2.9.2/src/pdm/resolver/python.py` & `pdm-2.9.3/src/pdm/resolver/python.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/resolver/reporters.py` & `pdm-2.9.3/src/pdm/resolver/reporters.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,14 +68,17 @@
             dependency, or None if ``requirement`` is one of the root
             requirements passed in from ``Resolver.resolve()``.
         """
         parent_line = f"(from {parent.name} {parent.version})" if parent else ""
         logger.info("  Adding requirement %s%s", requirement.as_line(), parent_line)
 
     def rejecting_candidate(self, criterion: Criterion, candidate: Candidate) -> None:
+        if not criterion.information:
+            logger.info("Candidate rejected because it contains invalid metadata: %s", candidate)
+            return
         *others, last = criterion.information
         logger.info(
             "Candidate rejected: %s because it introduces a new requirement %s"
             " that conflicts with other requirements:\n  %s",
             candidate,
             last.requirement.as_line(),  # type: ignore[attr-defined]
             "  \n".join(
```

### Comparing `pdm-2.9.2/src/pdm/signals.py` & `pdm-2.9.3/src/pdm/signals.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/termui.py` & `pdm-2.9.3/src/pdm/termui.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/src/pdm/utils.py` & `pdm-2.9.3/src/pdm/utils.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/cli/conftest.py` & `pdm-2.9.3/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/cli/test_add.py` & `pdm-2.9.3/tests/cli/test_add.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/cli/test_build.py` & `pdm-2.9.3/tests/cli/test_build.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/cli/test_cache.py` & `pdm-2.9.3/tests/cli/test_cache.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/cli/test_config.py` & `pdm-2.9.3/tests/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/cli/test_fix.py` & `pdm-2.9.3/tests/cli/test_fix.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/cli/test_hooks.py` & `pdm-2.9.3/tests/cli/test_hooks.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/cli/test_init.py` & `pdm-2.9.3/tests/cli/test_init.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/cli/test_install.py` & `pdm-2.9.3/tests/cli/test_install.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/cli/test_list.py` & `pdm-2.9.3/tests/cli/test_list.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/cli/test_lock.py` & `pdm-2.9.3/tests/cli/test_lock.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/cli/test_others.py` & `pdm-2.9.3/tests/cli/test_others.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/cli/test_publish.py` & `pdm-2.9.3/tests/cli/test_publish.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/cli/test_remove.py` & `pdm-2.9.3/tests/cli/test_remove.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/cli/test_run.py` & `pdm-2.9.3/tests/cli/test_run.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/cli/test_self_command.py` & `pdm-2.9.3/tests/cli/test_self_command.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/cli/test_template.py` & `pdm-2.9.3/tests/cli/test_template.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/cli/test_update.py` & `pdm-2.9.3/tests/cli/test_update.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/cli/test_use.py` & `pdm-2.9.3/tests/cli/test_use.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/cli/test_venv.py` & `pdm-2.9.3/tests/cli/test_venv.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/conftest.py` & `pdm-2.9.3/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 @pytest.fixture(scope="session")
 def build_env_wheels() -> Iterable[Path]:
     return [
         FIXTURES / "artifacts" / wheel_name
         for wheel_name in (
             "pdm_pep517-1.0.0-py3-none-any.whl",
             "poetry_core-1.3.2-py3-none-any.whl",
-            "setuptools-65.4.1-py3-none-any.whl",
+            "setuptools-68.0.0-py3-none-any.whl",
             "wheel-0.37.1-py2.py3-none-any.whl",
             "flit_core-3.6.0-py3-none-any.whl",
             "pdm_backend-2.1.4-py3-none-any.whl",
             "importlib_metadata-4.8.3-py3-none-any.whl",
             "zipp-3.7.0-py3-none-any.whl",
             "typing_extensions-4.4.0-py3-none-any.whl",
         )
```

### Comparing `pdm-2.9.2/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl` & `pdm-2.9.3/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz` & `pdm-2.9.3/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl` & `pdm-2.9.3/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl` & `pdm-2.9.3/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl` & `pdm-2.9.3/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/fixtures/artifacts/demo-0.0.1.tar.gz` & `pdm-2.9.3/tests/fixtures/artifacts/demo-0.0.1.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/fixtures/artifacts/demo-0.0.1.zip` & `pdm-2.9.3/tests/fixtures/artifacts/demo-0.0.1.zip`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl` & `pdm-2.9.3/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl` & `pdm-2.9.3/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl` & `pdm-2.9.3/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl` & `pdm-2.9.3/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz` & `pdm-2.9.3/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl` & `pdm-2.9.3/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl` & `pdm-2.9.3/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/fixtures/artifacts/pdm_backend-2.1.4-py3-none-any.whl` & `pdm-2.9.3/tests/fixtures/artifacts/pdm_backend-2.1.4-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl` & `pdm-2.9.3/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl` & `pdm-2.9.3/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl` & `pdm-2.9.3/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl` & `pdm-2.9.3/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl` & `pdm-2.9.3/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl` & `pdm-2.9.3/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl` & `pdm-2.9.3/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock` & `pdm-2.9.3/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/fixtures/projects/demo-package/pdm.lock` & `pdm-2.9.3/tests/fixtures/projects/demo-package/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/fixtures/projects/demo-package/pyproject.toml` & `pdm-2.9.3/tests/fixtures/projects/demo-package/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/fixtures/projects/demo-package/requirements.txt` & `pdm-2.9.3/tests/fixtures/projects/demo-package/requirements.txt`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/fixtures/projects/demo-package/setup.txt` & `pdm-2.9.3/tests/fixtures/projects/demo-package/setup.txt`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/fixtures/projects/flit-demo/pyproject.toml` & `pdm-2.9.3/tests/fixtures/projects/flit-demo/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/fixtures/projects/poetry-demo/pyproject.toml` & `pdm-2.9.3/tests/fixtures/projects/poetry-demo/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/fixtures/pypi.json` & `pdm-2.9.3/tests/fixtures/pypi.json`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/fixtures/pyproject.toml` & `pdm-2.9.3/tests/fixtures/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/models/test_backends.py` & `pdm-2.9.3/tests/models/test_backends.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/models/test_candidates.py` & `pdm-2.9.3/tests/models/test_candidates.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/models/test_marker.py` & `pdm-2.9.3/tests/models/test_marker.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/models/test_requirements.py` & `pdm-2.9.3/tests/models/test_requirements.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/models/test_setup_parsing.py` & `pdm-2.9.3/tests/models/test_setup_parsing.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/models/test_specifiers.py` & `pdm-2.9.3/tests/models/test_specifiers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/models/test_versions.py` & `pdm-2.9.3/tests/models/test_versions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/resolver/test_resolve.py` & `pdm-2.9.3/tests/resolver/test_resolve.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,7 +316,14 @@
     repository.add_dependencies("foo", "0.1.0", ["chardet; extra=='enc'"])
     repository.add_candidate("foo", "0.2.0")
     repository.add_dependencies("foo", "0.2.0", ["chardet; extra=='enc'"])
     repository.add_candidate("bar", "0.1.0")
     repository.add_dependencies("bar", "0.1.0", ["foo[enc]>=0.1.0"])
     result = resolve(["foo==0.1.0", "bar"])
     assert result["foo"].version == result["foo[enc]"].version == "0.1.0"
+
+
+def test_resolve_skip_candidate_with_invalid_metadata(resolve, repository):
+    repository.add_candidate("sqlparse", "0.4.0")
+    repository.add_dependencies("sqlparse", "0.4.0", ["django>=1.11'"])
+    result = resolve(["sqlparse"], ">=3.6")
+    assert result["sqlparse"].version == "0.3.0"
```

### Comparing `pdm-2.9.2/tests/test_formats.py` & `pdm-2.9.3/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/test_installer.py` & `pdm-2.9.3/tests/test_installer.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/test_integration.py` & `pdm-2.9.3/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/test_plugin.py` & `pdm-2.9.3/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/test_project.py` & `pdm-2.9.3/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/test_signals.py` & `pdm-2.9.3/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/tests/test_utils.py` & `pdm-2.9.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pdm-2.9.2/PKG-INFO` & `pdm-2.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm
-Version: 2.9.2
+Version: 2.9.3
 Summary: A modern Python package and dependency manager supporting the latest PEP standards
 Keywords: packaging dependency workflow
 Author-Email: Frost Ming <mianghong@gmail.com>
 License: MIT
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -22,15 +22,15 @@
 Requires-Dist: packaging!=22.0,>=20.9
 Requires-Dist: platformdirs
 Requires-Dist: rich>=12.3.0
 Requires-Dist: virtualenv>=20
 Requires-Dist: pyproject-hooks
 Requires-Dist: requests-toolbelt
 Requires-Dist: unearth>=0.10.0
-Requires-Dist: findpython<1.0.0a0,>=0.3.0
+Requires-Dist: findpython<1.0.0a0,>=0.4.0
 Requires-Dist: tomlkit<1,>=0.11.1
 Requires-Dist: shellingham>=1.3.2
 Requires-Dist: python-dotenv>=0.15
 Requires-Dist: resolvelib>=1.0.1
 Requires-Dist: installer<0.8,>=0.7
 Requires-Dist: cachecontrol[filecache]>=0.13.0
 Requires-Dist: truststore; python_version >= "3.10"
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: pdm Version: 2.9.2 Summary: A modern Python package
+Metadata-Version: 2.1 Name: pdm Version: 2.9.3 Summary: A modern Python package
 and dependency manager supporting the latest PEP standards Keywords: packaging
 dependency workflow Author-Email: Frost Ming
 gmail.com> License: MIT Classifier: Topic :: Software Development :: Build
 Tools Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Homepage, https://pdm.fming.dev Project-URL: Repository, https://
 github.com/pdm-project/pdm Project-URL: Documentation, https://pdm.fming.dev
 Project-URL: Changelog, https://pdm.fming.dev/latest/dev/changelog/ Requires-
 Python: >=3.7 Requires-Dist: blinker Requires-Dist: certifi Requires-Dist:
 packaging!=22.0,>=20.9 Requires-Dist: platformdirs Requires-Dist: rich>=12.3.0
 Requires-Dist: virtualenv>=20 Requires-Dist: pyproject-hooks Requires-Dist:
 requests-toolbelt Requires-Dist: unearth>=0.10.0 Requires-Dist:
-findpython<1.0.0a0,>=0.3.0 Requires-Dist: tomlkit<1,>=0.11.1 Requires-Dist:
+findpython<1.0.0a0,>=0.4.0 Requires-Dist: tomlkit<1,>=0.11.1 Requires-Dist:
 shellingham>=1.3.2 Requires-Dist: python-dotenv>=0.15 Requires-Dist:
 resolvelib>=1.0.1 Requires-Dist: installer<0.8,>=0.7 Requires-Dist:
 cachecontrol[filecache]>=0.13.0 Requires-Dist: truststore; python_version >=
 "3.10" Requires-Dist: tomli>=1.1.0; python_version < "3.11" Requires-Dist:
 importlib-resources>=5; python_version < "3.9" Requires-Dist: importlib-
 metadata>=3.6; python_version < "3.10" Requires-Dist: pytest; extra == "pytest"
 Requires-Dist: pytest-mock; extra == "pytest" Requires-Dist: copier>=8.0.0;
```

