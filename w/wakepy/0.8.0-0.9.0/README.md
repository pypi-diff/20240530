# Comparing `tmp/wakepy-0.8.0.tar.gz` & `tmp/wakepy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wakepy-0.8.0.tar", last modified: Sun May 26 16:10:15 2024, max compression
+gzip compressed data, was "wakepy-0.9.0.tar", last modified: Thu May 30 21:31:53 2024, max compression
```

## Comparing `wakepy-0.8.0.tar` & `wakepy-0.9.0.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:10:15.906432 wakepy-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-26 16:09:59.000000 wakepy-0.8.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:10:15.882432 wakepy-0.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:10:15.890432 wakepy-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-05-26 16:09:59.000000 wakepy-0.8.0/.github/workflows/build-and-run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-26 16:09:59.000000 wakepy-0.8.0/.github/workflows/publish-a-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-26 16:09:59.000000 wakepy-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-26 16:09:59.000000 wakepy-0.8.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-05-26 16:09:59.000000 wakepy-0.8.0/DEV.md
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-26 16:09:59.000000 wakepy-0.8.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-05-26 16:10:15.906432 wakepy-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-26 16:09:59.000000 wakepy-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:10:15.890432 wakepy-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-26 16:09:59.000000 wakepy-0.8.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-26 16:09:59.000000 wakepy-0.8.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:10:15.890432 wakepy-0.8.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:10:15.894432 wakepy-0.8.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-26 16:09:59.000000 wakepy-0.8.0/docs/source/_static/wakepy-docs.css
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-26 16:09:59.000000 wakepy-0.8.0/docs/source/_static/wakepy-docs.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:10:15.894432 wakepy-0.8.0/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 16:09:59.000000 wakepy-0.8.0/docs/source/_templates/author.html
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-26 16:09:59.000000 wakepy-0.8.0/docs/source/_templates/sbt-sidebar-nav.html
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-26 16:09:59.000000 wakepy-0.8.0/docs/source/api-reference.md
--rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-05-26 16:09:59.000000 wakepy-0.8.0/docs/source/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-26 16:09:59.000000 wakepy-0.8.0/docs/source/cli-api.md
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-26 16:09:59.000000 wakepy-0.8.0/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:10:15.894432 wakepy-0.8.0/docs/source/img/
--rw-r--r--   0 runner    (1001) docker     (127)    19633 2024-05-26 16:09:59.000000 wakepy-0.8.0/docs/source/img/activate-mode-activity-diagram.svg
--rw-r--r--   0 runner    (1001) docker     (127)    34844 2024-05-26 16:09:59.000000 wakepy-0.8.0/docs/source/img/activate-mode-using-method-activity-diagram.svg
--rw-r--r--   0 runner    (1001) docker     (127)    35437 2024-05-26 16:09:59.000000 wakepy-0.8.0/docs/source/img/mode-activity-diagram.svg
--rw-r--r--   0 runner    (1001) docker     (127)    18172 2024-05-26 16:09:59.000000 wakepy-0.8.0/docs/source/img/mode-state-diagram.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-05-26 16:09:59.000000 wakepy-0.8.0/docs/source/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    11918 2024-05-26 16:09:59.000000 wakepy-0.8.0/docs/source/methods-reference.md
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-26 16:09:59.000000 wakepy-0.8.0/docs/source/migration.md
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-26 16:09:59.000000 wakepy-0.8.0/docs/source/modes.md
--rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-05-26 16:09:59.000000 wakepy-0.8.0/docs/source/test-manually.md
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-26 16:09:59.000000 wakepy-0.8.0/docs/source/tests-and-ci.md
--rw-r--r--   0 runner    (1001) docker     (127)     8509 2024-05-26 16:09:59.000000 wakepy-0.8.0/docs/source/user-guide.md
--rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-05-26 16:09:59.000000 wakepy-0.8.0/docs/source/wakepy-mode-lifecycle.md
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-26 16:09:59.000000 wakepy-0.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:10:15.894432 wakepy-0.8.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-26 16:09:59.000000 wakepy-0.8.0/requirements/requirements-check.txt
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-26 16:09:59.000000 wakepy-0.8.0/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-26 16:09:59.000000 wakepy-0.8.0/requirements/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-26 16:09:59.000000 wakepy-0.8.0/requirements/requirements-mypy.txt
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-26 16:09:59.000000 wakepy-0.8.0/requirements/requirements-test.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:10:15.894432 wakepy-0.8.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-26 16:09:59.000000 wakepy-0.8.0/scripts/example-test.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 16:10:15.910432 wakepy-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:10:15.886432 wakepy-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:10:15.894432 wakepy-0.8.0/src/wakepy/
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-26 16:09:59.000000 wakepy-0.8.0/src/wakepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-05-26 16:09:59.000000 wakepy-0.8.0/src/wakepy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-26 16:10:15.000000 wakepy-0.8.0/src/wakepy/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:10:15.898432 wakepy-0.8.0/src/wakepy/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-26 16:09:59.000000 wakepy-0.8.0/src/wakepy/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9278 2024-05-26 16:09:59.000000 wakepy-0.8.0/src/wakepy/core/activationresult.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-26 16:09:59.000000 wakepy-0.8.0/src/wakepy/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    13527 2024-05-26 16:09:59.000000 wakepy-0.8.0/src/wakepy/core/dbus.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-26 16:09:59.000000 wakepy-0.8.0/src/wakepy/core/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (127)    21036 2024-05-26 16:09:59.000000 wakepy-0.8.0/src/wakepy/core/method.py
--rw-r--r--   0 runner    (1001) docker     (127)    22236 2024-05-26 16:09:59.000000 wakepy-0.8.0/src/wakepy/core/mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-26 16:09:59.000000 wakepy-0.8.0/src/wakepy/core/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     8990 2024-05-26 16:09:59.000000 wakepy-0.8.0/src/wakepy/core/prioritization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-05-26 16:09:59.000000 wakepy-0.8.0/src/wakepy/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-26 16:09:59.000000 wakepy-0.8.0/src/wakepy/core/strenum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:10:15.898432 wakepy-0.8.0/src/wakepy/dbus_adapters/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-26 16:09:59.000000 wakepy-0.8.0/src/wakepy/dbus_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-26 16:09:59.000000 wakepy-0.8.0/src/wakepy/dbus_adapters/jeepney.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:10:15.902432 wakepy-0.8.0/src/wakepy/methods/
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-26 16:09:59.000000 wakepy-0.8.0/src/wakepy/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-26 16:09:59.000000 wakepy-0.8.0/src/wakepy/methods/_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-26 16:09:59.000000 wakepy-0.8.0/src/wakepy/methods/freedesktop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-26 16:09:59.000000 wakepy-0.8.0/src/wakepy/methods/gnome.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-26 16:09:59.000000 wakepy-0.8.0/src/wakepy/methods/macos.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-26 16:09:59.000000 wakepy-0.8.0/src/wakepy/methods/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:10:15.902432 wakepy-0.8.0/src/wakepy/modes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 16:09:59.000000 wakepy-0.8.0/src/wakepy/modes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-05-26 16:09:59.000000 wakepy-0.8.0/src/wakepy/modes/keep.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 16:09:59.000000 wakepy-0.8.0/src/wakepy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:10:15.906432 wakepy-0.8.0/src/wakepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-05-26 16:10:15.000000 wakepy-0.8.0/src/wakepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-05-26 16:10:15.000000 wakepy-0.8.0/src/wakepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 16:10:15.000000 wakepy-0.8.0/src/wakepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-26 16:10:15.000000 wakepy-0.8.0/src/wakepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-26 16:10:15.000000 wakepy-0.8.0/src/wakepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-26 16:10:15.000000 wakepy-0.8.0/src/wakepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-26 16:09:59.000000 wakepy-0.8.0/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:10:15.902432 wakepy-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 16:09:59.000000 wakepy-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-26 16:09:59.000000 wakepy-0.8.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:10:15.902432 wakepy-0.8.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 16:09:59.000000 wakepy-0.8.0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-26 16:09:59.000000 wakepy-0.8.0/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-05-26 16:09:59.000000 wakepy-0.8.0/tests/integration/dbus_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     7382 2024-05-26 16:09:59.000000 wakepy-0.8.0/tests/integration/test_dbus_adapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-26 16:09:59.000000 wakepy-0.8.0/tests/tox_build_wakepy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:10:15.902432 wakepy-0.8.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 16:09:59.000000 wakepy-0.8.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-26 16:09:59.000000 wakepy-0.8.0/tests/unit/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-26 16:09:59.000000 wakepy-0.8.0/tests/unit/test__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:10:15.906432 wakepy-0.8.0/tests/unit/test_core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 16:09:59.000000 wakepy-0.8.0/tests/unit/test_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-26 16:09:59.000000 wakepy-0.8.0/tests/unit/test_core/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    15382 2024-05-26 16:09:59.000000 wakepy-0.8.0/tests/unit/test_core/test_activationresult.py
--rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-05-26 16:09:59.000000 wakepy-0.8.0/tests/unit/test_core/test_calls.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-26 16:09:59.000000 wakepy-0.8.0/tests/unit/test_core/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-26 16:09:59.000000 wakepy-0.8.0/tests/unit/test_core/test_dbus.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-26 16:09:59.000000 wakepy-0.8.0/tests/unit/test_core/test_heartbeat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:10:15.906432 wakepy-0.8.0/tests/unit/test_core/test_method/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 16:09:59.000000 wakepy-0.8.0/tests/unit/test_core/test_method/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19101 2024-05-26 16:09:59.000000 wakepy-0.8.0/tests/unit/test_core/test_method/test_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-05-26 16:09:59.000000 wakepy-0.8.0/tests/unit/test_core/test_method/test_method.py
--rw-r--r--   0 runner    (1001) docker     (127)    14463 2024-05-26 16:09:59.000000 wakepy-0.8.0/tests/unit/test_core/test_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-26 16:09:59.000000 wakepy-0.8.0/tests/unit/test_core/test_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)    14593 2024-05-26 16:09:59.000000 wakepy-0.8.0/tests/unit/test_core/test_prioritization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-26 16:09:59.000000 wakepy-0.8.0/tests/unit/test_core/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-26 16:09:59.000000 wakepy-0.8.0/tests/unit/test_core/test_strenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-05-26 16:09:59.000000 wakepy-0.8.0/tests/unit/test_core/testmethods.py
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-26 16:09:59.000000 wakepy-0.8.0/tests/unit/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:10:15.906432 wakepy-0.8.0/tests/unit/test_methods/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-26 16:09:59.000000 wakepy-0.8.0/tests/unit/test_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-26 16:09:59.000000 wakepy-0.8.0/tests/unit/test_methods/test_freedesktop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-26 16:09:59.000000 wakepy-0.8.0/tests/unit/test_methods/test_gnome.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-26 16:09:59.000000 wakepy-0.8.0/tests/unit/test_methods/test_macos.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-26 16:09:59.000000 wakepy-0.8.0/tests/unit/test_methods/test_windows.py
--rw-r--r--   0 runner    (1001) docker     (127)     5908 2024-05-26 16:09:59.000000 wakepy-0.8.0/tests/unit/test_modes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-05-26 16:09:59.000000 wakepy-0.8.0/tox.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-26 16:09:59.000000 wakepy-0.8.0/toxfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.440820 wakepy-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 21:31:40.000000 wakepy-0.9.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.416820 wakepy-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.424820 wakepy-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-05-30 21:31:40.000000 wakepy-0.9.0/.github/workflows/build-and-run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-30 21:31:40.000000 wakepy-0.9.0/.github/workflows/publish-a-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-30 21:31:40.000000 wakepy-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-30 21:31:40.000000 wakepy-0.9.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-05-30 21:31:40.000000 wakepy-0.9.0/DEV.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-30 21:31:40.000000 wakepy-0.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-05-30 21:31:53.440820 wakepy-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-30 21:31:40.000000 wakepy-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.424820 wakepy-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.424820 wakepy-0.9.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.424820 wakepy-0.9.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/_static/wakepy-docs.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/_static/wakepy-docs.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.424820 wakepy-0.9.0/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/_templates/author.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/_templates/sbt-sidebar-nav.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/api-reference.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13097 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/cli-api.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.428820 wakepy-0.9.0/docs/source/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    19633 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/img/activate-mode-activity-diagram.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    34844 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/img/activate-mode-using-method-activity-diagram.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    35437 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/img/mode-activity-diagram.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    18172 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/img/mode-state-diagram.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    14784 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/methods-reference.md
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/migration.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/modes.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/test-manually.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/tests-and-ci.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8509 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/user-guide.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-05-30 21:31:40.000000 wakepy-0.9.0/docs/source/wakepy-mode-lifecycle.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-30 21:31:40.000000 wakepy-0.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.428820 wakepy-0.9.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-30 21:31:40.000000 wakepy-0.9.0/requirements/requirements-check.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-30 21:31:40.000000 wakepy-0.9.0/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-30 21:31:40.000000 wakepy-0.9.0/requirements/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-30 21:31:40.000000 wakepy-0.9.0/requirements/requirements-mypy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-30 21:31:40.000000 wakepy-0.9.0/requirements/requirements-test.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.428820 wakepy-0.9.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-30 21:31:40.000000 wakepy-0.9.0/scripts/example-test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 21:31:53.440820 wakepy-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.420820 wakepy-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.428820 wakepy-0.9.0/src/wakepy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-30 21:31:53.000000 wakepy-0.9.0/src/wakepy/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.432820 wakepy-0.9.0/src/wakepy/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9278 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/core/activationresult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13527 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/core/dbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/core/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21036 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/core/method.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22236 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/core/mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/core/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8990 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/core/prioritization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/core/strenum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.432820 wakepy-0.9.0/src/wakepy/dbus_adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/dbus_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/dbus_adapters/jeepney.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.436820 wakepy-0.9.0/src/wakepy/methods/
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/methods/_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/methods/freedesktop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/methods/gnome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/methods/macos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/methods/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.436820 wakepy-0.9.0/src/wakepy/modes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/modes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/modes/keep.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:40.000000 wakepy-0.9.0/src/wakepy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.440820 wakepy-0.9.0/src/wakepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-05-30 21:31:53.000000 wakepy-0.9.0/src/wakepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-05-30 21:31:53.000000 wakepy-0.9.0/src/wakepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 21:31:53.000000 wakepy-0.9.0/src/wakepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-30 21:31:53.000000 wakepy-0.9.0/src/wakepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-30 21:31:53.000000 wakepy-0.9.0/src/wakepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-30 21:31:53.000000 wakepy-0.9.0/src/wakepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-30 21:31:40.000000 wakepy-0.9.0/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.436820 wakepy-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.436820 wakepy-0.9.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/integration/dbus_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7382 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/integration/test_dbus_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/tox_build_wakepy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.436820 wakepy-0.9.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.440820 wakepy-0.9.0/tests/unit/test_core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_core/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15382 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_core/test_activationresult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_core/test_calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_core/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_core/test_dbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_core/test_heartbeat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.440820 wakepy-0.9.0/tests/unit/test_core/test_method/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_core/test_method/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19101 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_core/test_method/test_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_core/test_method/test_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14463 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_core/test_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_core/test_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14593 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_core/test_prioritization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_core/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_core/test_strenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_core/testmethods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:31:53.440820 wakepy-0.9.0/tests/unit/test_methods/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_methods/test_freedesktop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_methods/test_gnome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_methods/test_macos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_methods/test_windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5908 2024-05-30 21:31:40.000000 wakepy-0.9.0/tests/unit/test_modes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-05-30 21:31:40.000000 wakepy-0.9.0/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-30 21:31:40.000000 wakepy-0.9.0/toxfile.py
```

### Comparing `wakepy-0.8.0/.github/workflows/build-and-run-tests.yml` & `wakepy-0.9.0/.github/workflows/build-and-run-tests.yml`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/.github/workflows/publish-a-release.yml` & `wakepy-0.9.0/.github/workflows/publish-a-release.yml`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/LICENSE.txt` & `wakepy-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/PKG-INFO` & `wakepy-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wakepy
-Version: 0.8.0
+Version: 0.9.0
 Summary: wakelock / keep-awake / stay-awake
 Author-email: Niko Föhr <fohrloop@gmail.com>
 License: MIT License
         
         Copyright (c) 2021-2024 Niko Föhr
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `wakepy-0.8.0/README.md` & `wakepy-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/docs/Makefile` & `wakepy-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/docs/make.bat` & `wakepy-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/docs/source/_static/wakepy-docs.js` & `wakepy-0.9.0/docs/source/_static/wakepy-docs.js`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/docs/source/_templates/sbt-sidebar-nav.html` & `wakepy-0.9.0/docs/source/_templates/sbt-sidebar-nav.html`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/docs/source/api-reference.md` & `wakepy-0.9.0/docs/source/api-reference.md`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/docs/source/changelog.md` & `wakepy-0.9.0/docs/source/changelog.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,22 @@
 # Changelog
 
+## wakepy 0.9.0
+🗓️ 2024-05-31
+
+### ✨ Features
+- Support keep.running mode in KDE Plasma 5.12.90 and newer through the [org.freedesktop.PowerManagement](#keep-running-org-freedesktop-powermanagement) method. It may also be used on other DEs which implement this older freedesktop.org D-Bus interface (but not Xcfe). ([#324](https://github.com/fohrloop/wakepy/pull/324))
+- Cooler CLI spinner ([#309](https://github.com/fohrloop/wakepy/pull/309), [#323](https://github.com/fohrloop/wakepy/pull/323))
+
+### 📖 Documentation
+- Document that the [org.freedesktop.ScreenSaver](keep-presenting-org-freedesktop-screensaver) method for keep.presenting mode also supports KDE Plasma. ([#324](https://github.com/fohrloop/wakepy/pull/324))
+- Update dev docs ([#308](https://github.com/fohrloop/wakepy/pull/308))
+- Mention that shell should be restarted for wakepy CLI tool ([#321](https://github.com/fohrloop/wakepy/pull/321))
+- Fix: Supported Platforms table background does not support dark mode ([#316](https://github.com/fohrloop/wakepy/pull/316))
+
 ## wakepy 0.8.0
 🗓️ 2024-05-26
 
 ### 🏆 Highlights
 - This is a basically a complete rewrite of wakepy. It adds support for keep.running mode on Gnome, on-fail action, possibility to control the used methods and their priority, more information about the used methods and the activation process and possibility to exit the mode early. In addition, testing and CI pipelines were updated to ease maintenance.
 
 ### ✨ Features
```

### Comparing `wakepy-0.8.0/docs/source/cli-api.md` & `wakepy-0.9.0/docs/source/cli-api.md`

 * *Files 24% similar despite different names*

```diff
@@ -19,8 +19,15 @@
 
 options:
   -h, --help               show this help message and exit
   -k, --keep-running       Keep programs running; inhibit automatic sleep/suspend. This
                            is used as a default if no modes are selected.
   -p, --presentation       Presentation mode; inhibit automatic sleep, screensaver and
                            screenlock
-```
+```
+
+
+````{admonition} Command "wakepy" not found?
+:class: note
+
+If you just installed `wakepy`, you might need to restart shell / terminal application to make added to the PATH.
+````
```

### Comparing `wakepy-0.8.0/docs/source/conf.py` & `wakepy-0.9.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/docs/source/img/activate-mode-activity-diagram.svg` & `wakepy-0.9.0/docs/source/img/activate-mode-activity-diagram.svg`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/docs/source/img/activate-mode-using-method-activity-diagram.svg` & `wakepy-0.9.0/docs/source/img/activate-mode-using-method-activity-diagram.svg`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/docs/source/img/mode-activity-diagram.svg` & `wakepy-0.9.0/docs/source/img/mode-activity-diagram.svg`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/docs/source/img/mode-state-diagram.svg` & `wakepy-0.9.0/docs/source/img/mode-state-diagram.svg`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/docs/source/index.md` & `wakepy-0.9.0/docs/source/index.md`

 * *Files 10% similar despite different names*

```diff
@@ -34,34 +34,39 @@
       <td>Windows Server 2003 or higher</td>
     </tr>
     <tr>
       <td>Mac OS</td>
       <td>Mac OS X 10.8 Mountain Lion (July 2012) or newer</td>
     </tr>
     <tr>
-      <td class="hoverable" rowspan="2">Linux<sup>[1]</sup></td>
+      <td class="hoverable" rowspan="3">Linux<sup>[1]</sup></td>
       <td>Distributions using <a href="https://en.wikipedia.org/wiki/GNOME">GNOME</a></td>
     </tr>
     <tr>
-      <td>Desktop Environments which implement the <a href="https://en.wikipedia.org/wiki/Freedesktop.org">Freedesktop.org</a> ScreenSaver interface (<code>org.freedesktop.ScreenSaver</code>)</td>
+      <td>Distributions using <a href="https://en.wikipedia.org/wiki/KDE_Plasma">KDE Plasma</a><sup>[2]</sup></td>
+    </tr>
+    <tr>
+      <td>Any other Desktop Environments which implement the <a href="https://en.wikipedia.org/wiki/Freedesktop.org">Freedesktop.org</a> <a href="https://people.freedesktop.org/~hadess/idle-inhibition-spec/re01.html">ScreenSaver</a> interface<sup>[2]</sup></td>
     </tr>
   </tbody>
 </table>
 
 <p style="margin-top:1em;">
-<sup>[1]</sup> The Linux support is under active development. Target is to support at least GNOME, KDE, Xfce, Cinnamon, LXQt and MATE Desktop Environments.<p>
+<sup>[1]</sup> The Linux support is under active development. Target is to support at least GNOME, KDE, Xfce, Cinnamon, LXQt and MATE Desktop Environments. <sup>[2]</sup> Only the presentation mode currently.<p>
 
 ## Installing
 
 Wakepy supports CPython 3.7 to 3.13, and may be installed with
 
 ```
 pip install wakepy
 ```
 
+To get the `wakepy` [CLI command](#cli-api) working, you might need to restart the shell / terminal application.
+
 ## Why wakepy?
 Here's some reasons why you might want to consider using wakepy:
 
 🛡️ For security reasons
 : When you don't want to use a technique which keeps the screen awake and disables the automatic screen lock. I.e. you *only* want to disable the automatic suspend. 
 
 🦸 You need a cross-platform solution
```

#### html2text {}

```diff
@@ -7,60 +7,63 @@
 inhibited. (See: [keep.presenting](#keep-presenting-mode)) ## Supported
 platforms Wakepy may keep the following systems awake:
 PPllaattffoorrmm DDeettaaiillss
 Windows  Windows XP to Windows 11
          Windows Server 2003 or higher
 Mac OS   Mac OS X 10.8 Mountain Lion (July 2012) or newer
          Distributions using _G_N_O_M_E
-Linux[1] Desktop Environments which implement the _F_r_e_e_d_e_s_k_t_o_p_._o_r_g ScreenSaver
-         interface (org.freedesktop.ScreenSaver)
+Linux[1] Distributions using _K_D_E_ _P_l_a_s_m_a[2]
+         Any other Desktop Environments which implement the _F_r_e_e_d_e_s_k_t_o_p_._o_r_g
+         _S_c_r_e_e_n_S_a_v_e_r interface[2]
 [1] The Linux support is under active development. Target is to support at
-least GNOME, KDE, Xfce, Cinnamon, LXQt and MATE Desktop Environments.
+least GNOME, KDE, Xfce, Cinnamon, LXQt and MATE Desktop Environments. [2] Only
+the presentation mode currently.
 ## Installing Wakepy supports CPython 3.7 to 3.13, and may be installed with
-``` pip install wakepy ``` ## Why wakepy? Here's some reasons why you might
-want to consider using wakepy: ð¡ï¸ For security reasons : When you don't
-want to use a technique which keeps the screen awake and disables the automatic
-screen lock. I.e. you *only* want to disable the automatic suspend. ð¦¸ You
-need a cross-platform solution : Same code works on Windows, macOS and Linux.
-âï¸ You want to have more control : It is possible to whitelist or blacklist
-the used wakepy Methods. It is also possible to prioritize them and define a
-on-fail action in case activating a wakepy mode fails. âï¸ You want to keep
-the amount of dependencies low : If you're running wakepy on Linux, [jeepney]
-(https://jeepney.readthedocs.io/) is required for D-Bus based methods. On
-Python 3.7, [typing-extensions](https://pypi.org/project/typing-extensions/) is
-needed for typing. Otherwise: wakepy has no python dependencies. âï¸ Package
-needs to have a permissive licence : Wakepy is licenced under permissive [MIT
-License](https://github.com/fohrloop/wakepy/blob/main/LICENSE.txt). ## Command
-line interface (CLI) To keep system from sleeping, run ``` wakepy ``` For
-presentation mode, add `-p` flag. See also: [CLI API](#cli-api) ## Basic usage
-within Python In the simplest case, keeping a system running long running task
-with wakepy would be in python (See: [`keep.running`](#keep-running-mode)): ```
-{code-block} python from wakepy import keep with keep.running(): # Do something
-that takes a long time. The system may start screensaver # / screenlock or
-blank the screen, but CPU will keep running. ``` If you want to *also* prevent
-screen lock and screen blank, use the [`keep.presenting`](#keep-presenting-
-mode) mode: ```{code-block} python from wakepy import keep with keep.presenting
-(): # Do something that takes a long time and requires the screen to be awake
-``` ```{admonition} Next Steps :class: seealso See the [User Guide](#user-
-guide) and the available wakepy [Modes](#wakepy-modes) and [Methods](#wakepy-
-methods) ``` ```{admonition} Wakepy API is still experimental ð§ :class: note
-Since wakepy is still 0.x.x, the API might change without further notice from
-one release to another. After that, breaking changes should occur only part of
-a major release (e.g. 1.x.x -> 2.0.0). ``` ## Where wakepy is used? -
-[viskillz-blender](https://github.com/viskillz/viskillz-blender) â Generating
-assets of Mental Cutting Test exercises - [mpc-autofill](https://github.com/
-chilli-axe/mpc-autofill) â Automating MakePlayingCards' online ordering
-system - [lakeshorecryotronics/python-driver](https://github.com/
-lakeshorecryotronics/python-driver) â Lake Shore instruments python Driver -
-[UCSD-E4E/baboon-tracking](https://github.com/UCSD-E4E/baboon-tracking) â In
-pipelines of a Computer Vision project tracking baboons - [davlee1972/
-upscale_video](https://github.com/davlee1972/upscale_video) â Upscaling video
-using AI - [minarca](https://github.com/ikus060/minarca) â Cross-platform
-data backup software ## Links - GitHub: [github.com/fohrloop/wakepy](https://
-github.com/fohrloop/wakepy) - PyPI: [pypi.org/project/wakepy](https://pypi.org/
-project/wakepy/) ```{toctree} :hidden: :maxdepth: 2 :numbered: -1 :titlesonly:
-user-guide tests-and-ci ``` ```{toctree} :hidden: :caption: 'Reference Manual:
-' :maxdepth: 2 :numbered: -1 :titlesonly: modes methods-reference api-reference
-cli-api ``` ```{toctree} :hidden: :caption: 'Technical Details:' :maxdepth: 2 :
-numbered: -1 :titlesonly: wakepy-mode-lifecycle test-manually ``` ```{toctree}
-:hidden: :caption: 'Development:' :maxdepth: 2 :numbered: -1 :titlesonly:
-changelog migration ```
+``` pip install wakepy ``` To get the `wakepy` [CLI command](#cli-api) working,
+you might need to restart the shell / terminal application. ## Why wakepy?
+Here's some reasons why you might want to consider using wakepy: ð¡ï¸ For
+security reasons : When you don't want to use a technique which keeps the
+screen awake and disables the automatic screen lock. I.e. you *only* want to
+disable the automatic suspend. ð¦¸ You need a cross-platform solution : Same
+code works on Windows, macOS and Linux. âï¸ You want to have more control :
+It is possible to whitelist or blacklist the used wakepy Methods. It is also
+possible to prioritize them and define a on-fail action in case activating a
+wakepy mode fails. âï¸ You want to keep the amount of dependencies low : If
+you're running wakepy on Linux, [jeepney](https://jeepney.readthedocs.io/) is
+required for D-Bus based methods. On Python 3.7, [typing-extensions](https://
+pypi.org/project/typing-extensions/) is needed for typing. Otherwise: wakepy
+has no python dependencies. âï¸ Package needs to have a permissive licence :
+Wakepy is licenced under permissive [MIT License](https://github.com/fohrloop/
+wakepy/blob/main/LICENSE.txt). ## Command line interface (CLI) To keep system
+from sleeping, run ``` wakepy ``` For presentation mode, add `-p` flag. See
+also: [CLI API](#cli-api) ## Basic usage within Python In the simplest case,
+keeping a system running long running task with wakepy would be in python (See:
+[`keep.running`](#keep-running-mode)): ```{code-block} python from wakepy
+import keep with keep.running(): # Do something that takes a long time. The
+system may start screensaver # / screenlock or blank the screen, but CPU will
+keep running. ``` If you want to *also* prevent screen lock and screen blank,
+use the [`keep.presenting`](#keep-presenting-mode) mode: ```{code-block} python
+from wakepy import keep with keep.presenting(): # Do something that takes a
+long time and requires the screen to be awake ``` ```{admonition} Next Steps :
+class: seealso See the [User Guide](#user-guide) and the available wakepy
+[Modes](#wakepy-modes) and [Methods](#wakepy-methods) ``` ```{admonition}
+Wakepy API is still experimental ð§ :class: note Since wakepy is still 0.x.x,
+the API might change without further notice from one release to another. After
+that, breaking changes should occur only part of a major release (e.g. 1.x.x -
+> 2.0.0). ``` ## Where wakepy is used? - [viskillz-blender](https://github.com/
+viskillz/viskillz-blender) â Generating assets of Mental Cutting Test
+exercises - [mpc-autofill](https://github.com/chilli-axe/mpc-autofill) â
+Automating MakePlayingCards' online ordering system - [lakeshorecryotronics/
+python-driver](https://github.com/lakeshorecryotronics/python-driver) â Lake
+Shore instruments python Driver - [UCSD-E4E/baboon-tracking](https://
+github.com/UCSD-E4E/baboon-tracking) â In pipelines of a Computer Vision
+project tracking baboons - [davlee1972/upscale_video](https://github.com/
+davlee1972/upscale_video) â Upscaling video using AI - [minarca](https://
+github.com/ikus060/minarca) â Cross-platform data backup software ## Links -
+GitHub: [github.com/fohrloop/wakepy](https://github.com/fohrloop/wakepy) -
+PyPI: [pypi.org/project/wakepy](https://pypi.org/project/wakepy/) ```{toctree}
+:hidden: :maxdepth: 2 :numbered: -1 :titlesonly: user-guide tests-and-ci ```
+```{toctree} :hidden: :caption: 'Reference Manual:' :maxdepth: 2 :numbered: -
+1 :titlesonly: modes methods-reference api-reference cli-api ``` ```{toctree} :
+hidden: :caption: 'Technical Details:' :maxdepth: 2 :numbered: -1 :titlesonly:
+wakepy-mode-lifecycle test-manually ``` ```{toctree} :hidden: :caption:
+'Development:' :maxdepth: 2 :numbered: -1 :titlesonly: changelog migration ```
```

### Comparing `wakepy-0.8.0/docs/source/methods-reference.md` & `wakepy-0.9.0/docs/source/methods-reference.md`

 * *Files 17% similar despite different names*

```diff
@@ -30,14 +30,28 @@
 
 ````{admonition} May slow down system if called repeatedly
 :class: warning
 
 If used hundreds or thousands of times, may slow down system. See: [wakepy/#277](https://github.com/fohrloop/wakepy/issues/277)
 ````
 
+
+(keep-running-org-freedesktop-powermanagement)=
+### org.freedesktop.PowerManagement
+- **Name**: `org.freedesktop.PowerManagement`
+- **Introduced in**: wakepy 0.9.0
+- **How it works**: Uses the Inhibit method of the org.freedesktop.PowerManagement D-Bus service when activating and saves the returned cookie on the Method instance. Uses UnInhibit method of the same service with the cookie when deactivating. The org.freedesktop.PowerManagement is an obsolete spec, but certain Desktop Environments provide that as the only option for inhibiting the suspend action. The documentation was previously hosted on [freedesktop.org](https://www.freedesktop.org/wiki/Specifications/power-management-spec/) but the links on the page are dead. The spec has three versions: 0.1, 0.2 and 0.3. The 0.3 is not found anywhere but the version 0.2 of the spec can be read in the [Internet Archive](https://web.archive.org/web/20090417010057/http://people.freedesktop.org/~hughsient/temp/power-management-spec-0.2.html)
+- **Multiprocess safe?**: Yes
+- **What if the process holding the lock dies?**: The lock is automatically removed.
+- **How to check it?**:  You may check if there are *any* inhibitors using the HasInhibit method of the `/org/freedesktop/PowerManagement/Inhibit` object on the `org.freedesktop.PowerManagement.Inhibit` interface. Note that updating the inhibit flag from `false` to `true` may take a few seconds. A good tool for this is [D-Spy](https://apps.gnome.org/Dspy/). Alternatively, you could monitor your inhibit call with [`dbus-monitor`](https://dbus.freedesktop.org/doc/dbus-monitor.1.html).
+- **Requirements**: D-Bus + KDE Plasma >=5.12.90 or other DE which implements this older freedesktop D-Bus interface. Exception: Xfce is not supported.
+- **About unsupported DEs** Older versions of KDE Plasma had a bug which also prevented the screenlock/screesaver activation. The bug was fixed in [D11182](https://phabricator.kde.org/D11182), commit  [152400c1b688](https://phabricator.kde.org/R122:152400c1b6880506ee1395011686c2b191f419a0) and was part of the KDE Plasma to 5.12.90 ( = 5.13 Beta) [release](https://kde.org/announcements/changelogs/plasma/5/5.12.5-5.12.90/). This Method is not supported either on Xfce as it has similar bug which prevents also the automatic screenlock/screensaver (See: [xfce4-power-manager/#65](https://gitlab.xfce.org/xfce/xfce4-power-manager/-/issues/65)), hence, wakepy refuses to use org.freedesktop.PowerManagement as method for keep.running mode on KDE < 5.12.90 and on any version of Xfce.
+- **Tested on**:  openSUSE 15.5 with KDE Plasma 5.27.9 ([Comment in #310](https://github.com/fohrloop/wakepy/issues/310#issuecomment-2140156882) by [fohrloop](https://github.com/fohrloop/)).
+
+
 (keep-running-windows-stes)=
 ### SetThreadExecutionState
 
 ````{admonition} Windows will not lock the screen automatically if Screen Saver settings do not require it
 :class: warning
 
 Since this method prevents sleep, screen can be only locked automatically if a screen saver is enabled and it set to ask for password. See [this](#checking-if-windows-will-lock-screen-automatically) for details.
@@ -124,15 +138,15 @@
 - **Name**: `org.freedesktop.ScreenSaver`
 - **Introduced in**: wakepy 0.6.0
 - **How it works**: Uses the Inhibit method of [org.freedesktop.ScreenSaver](https://people.freedesktop.org/~hadess/idle-inhibition-spec/re01.html) D-Bus service when activating and saves the returned cookie on the Method instance. Uses the org.freedesktop.ScreenSaver.UnInhibit method with the cookie when deactivating. The org.freedesktop.ScreenSaver can only be used to prevent idle; that is why there is no "keep.running" mode counterpart.
 - **Multiprocess safe?**: Yes
 - **What if the process holding the lock dies?**: The lock is automatically removed.
 - **How to check it?**:  The org.freedesktop.ScreenSaver does not expose a method for listing the inhibitors, but you could monitor your inhibit call with [`dbus-monitor`](https://dbus.freedesktop.org/doc/dbus-monitor.1.html).
 - **Requirements**: D-Bus, and a [freedesktop.org compliant desktop environment](https://www.freedesktop.org/wiki/Desktops/), which should implement the org.freedesktop.ScreenSaver.Inhibit method.
-- **Tested on**:  Ubuntu 22.04 with GNOME 42.9 ([PR #171](https://github.com/fohrloop/wakepy/pull/171) by [fohrloop](https://github.com/fohrloop/)).
+- **Tested on**:  Ubuntu 22.04 with GNOME 42.9 ([wakepy/#171](https://github.com/fohrloop/wakepy/pull/171)) and openSUSE 15.5 with KDE Plasma 5.27.9 ([wakepy/#310](https://github.com/fohrloop/wakepy/issues/310#issuecomment-2135512139)) by [fohrloop](https://github.com/fohrloop/).
 
 (keep-presenting-windows-stes)=
 ### SetThreadExecutionState
 
 - **Name**: `SetThreadExecutionState`
 - **Introduced in**: wakepy 0.1.0
 - **How it works**: Exactly the same as the [keep.running](keep-running-windows-stes), but using ES_CONTINUOUS, ES_SYSTEM_REQUIRED *and* ES_DISPLAY_REQUIRED flags when activating.
```

### Comparing `wakepy-0.8.0/docs/source/migration.md` & `wakepy-0.9.0/docs/source/migration.md`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/docs/source/modes.md` & `wakepy-0.9.0/docs/source/modes.md`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/docs/source/test-manually.md` & `wakepy-0.9.0/docs/source/test-manually.md`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/docs/source/tests-and-ci.md` & `wakepy-0.9.0/docs/source/tests-and-ci.md`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/docs/source/user-guide.md` & `wakepy-0.9.0/docs/source/user-guide.md`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/docs/source/wakepy-mode-lifecycle.md` & `wakepy-0.9.0/docs/source/wakepy-mode-lifecycle.md`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/pyproject.toml` & `wakepy-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/requirements/requirements-test.txt` & `wakepy-0.9.0/requirements/requirements-test.txt`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/src/wakepy/__init__.py` & `wakepy-0.9.0/src/wakepy/__init__.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/src/wakepy/__main__.py` & `wakepy-0.9.0/src/wakepy/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -157,18 +157,18 @@
         no_auto_suspend="x",
         presentation_mode="x" if mode == ModeName.KEEP_PRESENTING else " ",
     )
     return "\n".join((wakepy_text, options_txt)) + "\n"
 
 
 def wait_until_keyboardinterrupt() -> None:
-    spinning_chars = ["|", "/", "-", "\\"]
+    spinner_symbols = ["⢎⡰", "⢎⡡", "⢎⡑", "⢎⠱", "⠎⡱", "⢊⡱", "⢌⡱", "⢆⡱"]
     try:
-        for char in itertools.cycle(spinning_chars):  # pragma: no branch
-            print("\r" + char + r" [Press Ctrl+C to exit]", end="")
-            time.sleep(1)
+        for spinner_symbol in itertools.cycle(spinner_symbols):  # pragma: no branch
+            print("\r " + spinner_symbol + r" [Press Ctrl+C to exit] ", end="")
+            time.sleep(0.8)
     except KeyboardInterrupt:
         pass
 
 
 if __name__ == "__main__":
     main()  # pragma: no cover
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `wakepy-0.8.0/src/wakepy/core/__init__.py` & `wakepy-0.9.0/src/wakepy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/src/wakepy/core/activationresult.py` & `wakepy-0.9.0/src/wakepy/core/activationresult.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/src/wakepy/core/constants.py` & `wakepy-0.9.0/src/wakepy/core/constants.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/src/wakepy/core/dbus.py` & `wakepy-0.9.0/src/wakepy/core/dbus.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/src/wakepy/core/heartbeat.py` & `wakepy-0.9.0/src/wakepy/core/heartbeat.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/src/wakepy/core/method.py` & `wakepy-0.9.0/src/wakepy/core/method.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/src/wakepy/core/mode.py` & `wakepy-0.9.0/src/wakepy/core/mode.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/src/wakepy/core/platform.py` & `wakepy-0.9.0/src/wakepy/core/platform.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/src/wakepy/core/prioritization.py` & `wakepy-0.9.0/src/wakepy/core/prioritization.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/src/wakepy/core/registry.py` & `wakepy-0.9.0/src/wakepy/core/registry.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/src/wakepy/core/strenum.py` & `wakepy-0.9.0/src/wakepy/core/strenum.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/src/wakepy/dbus_adapters/jeepney.py` & `wakepy-0.9.0/src/wakepy/dbus_adapters/jeepney.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/src/wakepy/methods/__init__.py` & `wakepy-0.9.0/src/wakepy/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/src/wakepy/methods/_testing.py` & `wakepy-0.9.0/src/wakepy/methods/_testing.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/src/wakepy/methods/gnome.py` & `wakepy-0.9.0/src/wakepy/methods/gnome.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/src/wakepy/methods/macos.py` & `wakepy-0.9.0/src/wakepy/methods/macos.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/src/wakepy/methods/windows.py` & `wakepy-0.9.0/src/wakepy/methods/windows.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/src/wakepy/modes/keep.py` & `wakepy-0.9.0/src/wakepy/modes/keep.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/src/wakepy.egg-info/PKG-INFO` & `wakepy-0.9.0/src/wakepy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wakepy
-Version: 0.8.0
+Version: 0.9.0
 Summary: wakelock / keep-awake / stay-awake
 Author-email: Niko Föhr <fohrloop@gmail.com>
 License: MIT License
         
         Copyright (c) 2021-2024 Niko Föhr
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `wakepy-0.8.0/src/wakepy.egg-info/SOURCES.txt` & `wakepy-0.9.0/src/wakepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/tasks.py` & `wakepy-0.9.0/tasks.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/tests/conftest.py` & `wakepy-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/tests/integration/conftest.py` & `wakepy-0.9.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/tests/integration/dbus_service.py` & `wakepy-0.9.0/tests/integration/dbus_service.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/tests/integration/test_dbus_adapters.py` & `wakepy-0.9.0/tests/integration/test_dbus_adapters.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/tests/tox_build_wakepy.py` & `wakepy-0.9.0/tests/tox_build_wakepy.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/tests/unit/conftest.py` & `wakepy-0.9.0/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/tests/unit/test__init__.py` & `wakepy-0.9.0/tests/unit/test__init__.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/tests/unit/test_core/conftest.py` & `wakepy-0.9.0/tests/unit/test_core/conftest.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/tests/unit/test_core/test_activationresult.py` & `wakepy-0.9.0/tests/unit/test_core/test_activationresult.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/tests/unit/test_core/test_calls.py` & `wakepy-0.9.0/tests/unit/test_core/test_calls.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/tests/unit/test_core/test_dbus.py` & `wakepy-0.9.0/tests/unit/test_core/test_dbus.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/tests/unit/test_core/test_method/test_activation.py` & `wakepy-0.9.0/tests/unit/test_core/test_method/test_activation.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/tests/unit/test_core/test_method/test_method.py` & `wakepy-0.9.0/tests/unit/test_core/test_method/test_method.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/tests/unit/test_core/test_mode.py` & `wakepy-0.9.0/tests/unit/test_core/test_mode.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/tests/unit/test_core/test_platform.py` & `wakepy-0.9.0/tests/unit/test_core/test_platform.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/tests/unit/test_core/test_prioritization.py` & `wakepy-0.9.0/tests/unit/test_core/test_prioritization.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/tests/unit/test_core/test_registry.py` & `wakepy-0.9.0/tests/unit/test_core/test_registry.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/tests/unit/test_core/test_strenum.py` & `wakepy-0.9.0/tests/unit/test_core/test_strenum.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/tests/unit/test_core/testmethods.py` & `wakepy-0.9.0/tests/unit/test_core/testmethods.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/tests/unit/test_main.py` & `wakepy-0.9.0/tests/unit/test_main.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/tests/unit/test_methods/test_gnome.py` & `wakepy-0.9.0/tests/unit/test_methods/test_gnome.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/tests/unit/test_methods/test_macos.py` & `wakepy-0.9.0/tests/unit/test_methods/test_macos.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/tests/unit/test_methods/test_windows.py` & `wakepy-0.9.0/tests/unit/test_methods/test_windows.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/tests/unit/test_modes.py` & `wakepy-0.9.0/tests/unit/test_modes.py`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/tox.ini` & `wakepy-0.9.0/tox.ini`

 * *Files identical despite different names*

### Comparing `wakepy-0.8.0/toxfile.py` & `wakepy-0.9.0/toxfile.py`

 * *Files identical despite different names*

