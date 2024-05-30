# Comparing `tmp/appmap-2.0.3.tar.gz` & `tmp/appmap-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appmap-2.0.3.tar", max compression
+gzip compressed data, was "appmap-2.0.4.tar", max compression
```

## Comparing `appmap-2.0.3.tar` & `appmap-2.0.4.tar`

### file list

```diff
@@ -1,163 +1,163 @@
--rw-r--r--   0        0        0     1925 2024-05-28 16:14:09.656141 appmap-2.0.3/LICENSE
--rw-r--r--   0        0        0     4534 2024-05-28 16:14:09.656141 appmap-2.0.3/README.md
--rw-r--r--   0        0        0      529 2024-05-28 16:14:09.656141 appmap-2.0.3/_appmap/__init__.py
--rw-r--r--   0        0        0    15857 2024-05-28 16:14:09.656141 appmap-2.0.3/_appmap/configuration.py
--rw-r--r--   0        0        0     1082 2024-05-28 16:14:09.656141 appmap-2.0.3/_appmap/django.py
--rw-r--r--   0        0        0     6702 2024-05-28 16:14:09.656141 appmap-2.0.3/_appmap/env.py
--rw-r--r--   0        0        0    15677 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/event.py
--rw-r--r--   0        0        0      694 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/fastapi.py
--rw-r--r--   0        0        0      822 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/flask.py
--rw-r--r--   0        0        0     3642 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/generation.py
--rw-r--r--   0        0        0    11495 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/importer.py
--rw-r--r--   0        0        0     4323 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/instrument.py
--rw-r--r--   0        0        0     1786 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/labels.py
--rw-r--r--   0        0        0     3071 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/metadata.py
--rw-r--r--   0        0        0      267 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/noappmap.py
--rw-r--r--   0        0        0      538 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/py_version_check.py
--rw-r--r--   0        0        0     5513 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/recorder.py
--rw-r--r--   0        0        0     2868 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/recording.py
--rw-r--r--   0        0        0      926 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/remote_recording.py
--rw-r--r--   0        0        0      340 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/singleton.py
--rw-r--r--   0        0        0      174 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/__init__.py
--rw-r--r--   0        0        0     3607 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/appmap_test_base.py
--rwxr-xr-x   0        0        0      121 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/bin/server_runner
--rw-r--r--   0        0        0     6048 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/conftest.py
--rw-r--r--   0        0        0      112 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/appmap-all-paths-malformed.yml
--rw-r--r--   0        0        0       50 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/appmap-broken.yml
--rw-r--r--   0        0        0       82 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/appmap-class.yml
--rw-r--r--   0        0        0       59 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/appmap-empty-path.yml
--rw-r--r--   0        0        0      126 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/appmap-exclude-fn.yml
--rw-r--r--   0        0        0       87 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/appmap-func.yml
--rw-r--r--   0        0        0       82 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/appmap-malformed-path.yml
--rw-r--r--   0        0        0      308 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/appmap-no-pyyaml.yml
--rw-r--r--   0        0        0      323 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/appmap.yml
--rw-r--r--   0        0        0        0 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/appmap_testing/__init__.py
--rw-r--r--   0        0        0      237 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/appmap_testing/django_simplelazyobject.py
--rw-r--r--   0        0        0        0 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/config/src/package/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/config/test/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/config/test/foo.py
--rw-r--r--   0        0        0       16 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/config-exclude/.hide/hidden_mod/__init__.py
--rw-r--r--   0        0        0       25 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/config-exclude/node_modules/node_mod/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/config-exclude/src/package/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/config-exclude/test/__init__.py
--rw-r--r--   0        0        0       14 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/config-exclude/venv/venv_mod/__init__.py
--rw-r--r--   0        0        0       20 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/config-up/appmap.yml
--rw-r--r--   0        0        0        0 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/config-up/project/p1/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/config-up/project/p2/sub1/__init__.py
--rw-r--r--   0        0        0       44 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/django/appmap.yml
--rw-r--r--   0        0        0      495 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/django/djangoapp/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/django/djangoapp/djangoapp.py
--rw-r--r--   0        0        0       39 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/django/djangoapp/hello_world.html
--rw-r--r--   0        0        0      154 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/django/djangoapp/middleware.py
--rw-r--r--   0        0        0      426 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/django/djangoapp/settings.py
--rw-r--r--   0        0        0      563 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/django/djangoapp/settings_dev.py
--rw-r--r--   0        0        0     2148 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/django/djangoapp/urls.py
--rw-r--r--   0        0        0       14 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/django/init/sitecustomize.py
--rwxr-xr-x   0        0        0      665 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/django/manage.py
--rw-r--r--   0        0        0       53 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/django/pytest.ini
--rw-r--r--   0        0        0        0 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/django/test/__init__.py
--rw-r--r--   0        0        0      935 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/django/test/test_app.py
--rw-r--r--   0        0        0     2591 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/example_class.py
--rw-r--r--   0        0        0     7942 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/expected.appmap.json
--rw-r--r--   0        0        0       47 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/fastapi/appmap.yml
--rw-r--r--   0        0        0        0 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/fastapi/fastapiapp/__init__.py
--rw-r--r--   0        0        0     1647 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/fastapi/fastapiapp/main.py
--rw-r--r--   0        0        0       14 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/fastapi/init/sitecustomize.py
--rw-r--r--   0        0        0      240 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/fastapi/test_app.py
--rw-r--r--   0        0        0       38 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/flask/appmap.yml
--rw-r--r--   0        0        0     1200 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/flask/flaskapp.py
--rw-r--r--   0        0        0       14 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/flask/init/sitecustomize.py
--rw-r--r--   0        0        0        0 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/flask/templates/test.html
--rw-r--r--   0        0        0      268 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/flask/test_app.py
--rw-r--r--   0        0        0        0 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/package1/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/package1/package2/__init__.py
--rw-r--r--   0        0        0      113 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/package1/package2/__main__.py
--rw-r--r--   0        0        0       69 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/package1/package2/mod1.py
--rw-r--r--   0        0        0      653 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/params.py
--rw-r--r--   0        0        0       38 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/pytest/appmap.yml
--rw-r--r--   0        0        0     2931 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/pytest/expected/pytest.appmap.json
--rw-r--r--   0        0        0      213 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/pytest/expected/status_errored.metadata.json
--rw-r--r--   0        0        0      221 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/pytest/expected/status_failed.metadata.json
--rw-r--r--   0        0        0      221 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/pytest/expected/status_xfailed.metadata.json
--rw-r--r--   0        0        0      186 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/pytest/simple.py
--rw-r--r--   0        0        0      295 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/pytest/test_noappmap.py
--rw-r--r--   0        0        0      393 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/pytest/test_simple.py
--rw-r--r--   0        0        0     1246 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/remote.appmap.json
--rw-r--r--   0        0        0       13 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/trial/.gitignore
--rw-r--r--   0        0        0       38 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/trial/appmap.yml
--rw-r--r--   0        0        0     1897 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/trial/expected/pytest.appmap.json
--rw-r--r--   0        0        0       14 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/trial/init/sitecustomize.py
--rw-r--r--   0        0        0        0 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/trial/test/__init__.py
--rw-r--r--   0        0        0      400 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/trial/test/test_deferred.py
--rw-r--r--   0        0        0       38 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/unittest/appmap.yml
--rw-r--r--   0        0        0     4428 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/unittest/expected/pytest.appmap.json
--rw-r--r--   0        0        0      220 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/unittest/expected/status_errored.metadata.json
--rw-r--r--   0        0        0      238 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/unittest/expected/status_failed.metadata.json
--rw-r--r--   0        0        0      238 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/unittest/expected/status_xfailed.metadata.json
--rw-r--r--   0        0        0       33 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/unittest/expected/status_xsucceeded.metadata.json
--rw-r--r--   0        0        0     4430 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/unittest/expected/unittest.appmap.json
--rw-r--r--   0        0        0       14 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/unittest/init/sitecustomize.py
--rw-r--r--   0        0        0      275 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/unittest/simple/__init__.py
--rw-r--r--   0        0        0      183 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/unittest/simple/test_noappmap.py
--rw-r--r--   0        0        0     1263 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/data/unittest/simple/test_simple.py
--rw-r--r--   0        0        0      734 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/helpers.py
--rw-r--r--   0        0        0     4761 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/normalize.py
--rw-r--r--   0        0        0     4983 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/test_command.py
--rw-r--r--   0        0        0    11609 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/test_configuration.py
--rw-r--r--   0        0        0     3401 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/test_describe_value.py
--rw-r--r--   0        0        0     8341 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/test_django.py
--rw-r--r--   0        0        0      943 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/test_django_simplelazyobject.py
--rw-r--r--   0        0        0      338 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/test_env.py
--rw-r--r--   0        0        0     3198 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/test_events.py
--rw-r--r--   0        0        0     2732 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/test_fastapi.py
--rw-r--r--   0        0        0     5065 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/test_flask.py
--rw-r--r--   0        0        0     1703 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/test_generation.py
--rw-r--r--   0        0        0     1548 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/test_http.py
--rw-r--r--   0        0        0     1533 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/test_importer.py
--rw-r--r--   0        0        0     2931 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/test_labels.py
--rw-r--r--   0        0        0     1470 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/test_metadata.py
--rw-r--r--   0        0        0     9877 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/test_params.py
--rw-r--r--   0        0        0     6706 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/test_recording.py
--rw-r--r--   0        0        0     2006 2024-05-28 16:14:09.660142 appmap-2.0.3/_appmap/test/test_runner.py
--rw-r--r--   0        0        0     3086 2024-05-28 16:14:09.664142 appmap-2.0.3/_appmap/test/test_sqlalchemy.py
--rw-r--r--   0        0        0     7261 2024-05-28 16:14:09.664142 appmap-2.0.3/_appmap/test/test_test_frameworks.py
--rw-r--r--   0        0        0      861 2024-05-28 16:14:09.664142 appmap-2.0.3/_appmap/test/test_util.py
--rw-r--r--   0        0        0    15340 2024-05-28 16:14:09.664142 appmap-2.0.3/_appmap/test/web_framework.py
--rw-r--r--   0        0        0     4828 2024-05-28 16:14:09.664142 appmap-2.0.3/_appmap/testing_framework.py
--rw-r--r--   0        0        0      370 2024-05-28 16:14:09.664142 appmap-2.0.3/_appmap/trace_logger.py
--rw-r--r--   0        0        0     2950 2024-05-28 16:14:09.664142 appmap-2.0.3/_appmap/unittest.py
--rw-r--r--   0        0        0     6652 2024-05-28 16:14:09.664142 appmap-2.0.3/_appmap/utils.py
--rw-r--r--   0        0        0     8622 2024-05-28 16:14:09.664142 appmap-2.0.3/_appmap/web_framework.py
--rw-r--r--   0        0        0     1853 2024-05-28 16:14:09.664142 appmap-2.0.3/appmap/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 16:14:09.664142 appmap-2.0.3/appmap/command/__init__.py
--rw-r--r--   0        0        0      420 2024-05-28 16:14:09.664142 appmap-2.0.3/appmap/command/appmap_agent_init.py
--rw-r--r--   0        0        0     3475 2024-05-28 16:14:09.664142 appmap-2.0.3/appmap/command/appmap_agent_status.py
--rw-r--r--   0        0        0     2096 2024-05-28 16:14:09.664142 appmap-2.0.3/appmap/command/appmap_agent_validate.py
--rw-r--r--   0        0        0     3916 2024-05-28 16:14:09.664142 appmap-2.0.3/appmap/command/runner.py
--rw-r--r--   0        0        0    11401 2024-05-28 16:14:09.664142 appmap-2.0.3/appmap/django.py
--rw-r--r--   0        0        0     6590 2024-05-28 16:14:09.664142 appmap-2.0.3/appmap/fastapi.py
--rw-r--r--   0        0        0     7219 2024-05-28 16:14:09.664142 appmap-2.0.3/appmap/flask.py
--rw-r--r--   0        0        0     2695 2024-05-28 16:14:09.664142 appmap-2.0.3/appmap/http.py
--rw-r--r--   0        0        0      675 2024-05-28 16:14:09.664142 appmap-2.0.3/appmap/labeling/__init__.py
--rw-r--r--   0        0        0     3387 2024-05-28 16:14:09.664142 appmap-2.0.3/appmap/labeling/crypto.yml
--rw-r--r--   0        0        0     2097 2024-05-28 16:14:09.664142 appmap-2.0.3/appmap/labeling/django.yml
--rw-r--r--   0        0        0      630 2024-05-28 16:14:09.664142 appmap-2.0.3/appmap/labeling/flask.yml
--rw-r--r--   0        0        0      831 2024-05-28 16:14:09.664142 appmap-2.0.3/appmap/labeling/formats.yml
--rw-r--r--   0        0        0       50 2024-05-28 16:14:09.664142 appmap-2.0.3/appmap/labeling/http.yml
--rw-r--r--   0        0        0      196 2024-05-28 16:14:09.664142 appmap-2.0.3/appmap/labeling/jobs.yml
--rw-r--r--   0        0        0       55 2024-05-28 16:14:09.664142 appmap-2.0.3/appmap/labeling/jwt.yml
--rw-r--r--   0        0        0      137 2024-05-28 16:14:09.664142 appmap-2.0.3/appmap/labeling/logger.yml
--rw-r--r--   0        0        0      214 2024-05-28 16:14:09.664142 appmap-2.0.3/appmap/labeling/random.yml
--rw-r--r--   0        0        0     3282 2024-05-28 16:14:09.664142 appmap-2.0.3/appmap/pytest.py
--rw-r--r--   0        0        0     2295 2024-05-28 16:14:09.664142 appmap-2.0.3/appmap/sqlalchemy.py
--rw-r--r--   0        0        0      294 2024-05-28 16:14:09.664142 appmap-2.0.3/appmap/unittest.py
--rw-r--r--   0        0        0      818 2024-05-28 16:14:09.664142 appmap-2.0.3/appmap/uvicorn.py
--rw-r--r--   0        0        0       14 2024-05-28 16:14:09.664142 appmap-2.0.3/appmap.pth
--rw-r--r--   0        0        0     3272 2024-05-28 16:17:13.465783 appmap-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     1304 2024-05-28 16:14:09.664142 appmap-2.0.3/vendor/_appmap/wrapt/LICENSE
--rw-r--r--   0        0        0     1200 2024-05-28 16:14:09.664142 appmap-2.0.3/vendor/_appmap/wrapt/__init__.py
--rw-r--r--   0        0        0     1746 2024-05-28 16:14:09.664142 appmap-2.0.3/vendor/_appmap/wrapt/arguments.py
--rw-r--r--   0        0        0    21332 2024-05-28 16:14:09.664142 appmap-2.0.3/vendor/_appmap/wrapt/decorators.py
--rw-r--r--   0        0        0    10782 2024-05-28 16:14:09.664142 appmap-2.0.3/vendor/_appmap/wrapt/importer.py
--rw-r--r--   0        0        0    38753 2024-05-28 16:14:09.664142 appmap-2.0.3/vendor/_appmap/wrapt/wrappers.py
--rw-r--r--   0        0        0     5717 1970-01-01 00:00:00.000000 appmap-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1925 2024-05-29 18:21:05.889437 appmap-2.0.4/LICENSE
+-rw-r--r--   0        0        0     4534 2024-05-29 18:21:05.889437 appmap-2.0.4/README.md
+-rw-r--r--   0        0        0      529 2024-05-29 18:21:05.889437 appmap-2.0.4/_appmap/__init__.py
+-rw-r--r--   0        0        0    15857 2024-05-29 18:21:05.889437 appmap-2.0.4/_appmap/configuration.py
+-rw-r--r--   0        0        0     1082 2024-05-29 18:21:05.889437 appmap-2.0.4/_appmap/django.py
+-rw-r--r--   0        0        0     6702 2024-05-29 18:21:05.889437 appmap-2.0.4/_appmap/env.py
+-rw-r--r--   0        0        0    15677 2024-05-29 18:21:05.889437 appmap-2.0.4/_appmap/event.py
+-rw-r--r--   0        0        0      694 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/fastapi.py
+-rw-r--r--   0        0        0      822 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/flask.py
+-rw-r--r--   0        0        0     3642 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/generation.py
+-rw-r--r--   0        0        0    11495 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/importer.py
+-rw-r--r--   0        0        0     4390 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/instrument.py
+-rw-r--r--   0        0        0     1786 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/labels.py
+-rw-r--r--   0        0        0     3071 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/metadata.py
+-rw-r--r--   0        0        0      267 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/noappmap.py
+-rw-r--r--   0        0        0      538 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/py_version_check.py
+-rw-r--r--   0        0        0     6225 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/recorder.py
+-rw-r--r--   0        0        0     2868 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/recording.py
+-rw-r--r--   0        0        0      926 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/remote_recording.py
+-rw-r--r--   0        0        0      340 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/singleton.py
+-rw-r--r--   0        0        0      174 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/__init__.py
+-rw-r--r--   0        0        0     3607 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/appmap_test_base.py
+-rwxr-xr-x   0        0        0      121 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/bin/server_runner
+-rw-r--r--   0        0        0     6048 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/conftest.py
+-rw-r--r--   0        0        0      112 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/appmap-all-paths-malformed.yml
+-rw-r--r--   0        0        0       50 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/appmap-broken.yml
+-rw-r--r--   0        0        0       82 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/appmap-class.yml
+-rw-r--r--   0        0        0       59 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/appmap-empty-path.yml
+-rw-r--r--   0        0        0      126 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/appmap-exclude-fn.yml
+-rw-r--r--   0        0        0       87 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/appmap-func.yml
+-rw-r--r--   0        0        0       82 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/appmap-malformed-path.yml
+-rw-r--r--   0        0        0      308 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/appmap-no-pyyaml.yml
+-rw-r--r--   0        0        0      323 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/appmap.yml
+-rw-r--r--   0        0        0        0 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/appmap_testing/__init__.py
+-rw-r--r--   0        0        0      237 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/appmap_testing/django_simplelazyobject.py
+-rw-r--r--   0        0        0        0 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/config/src/package/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/config/test/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/config/test/foo.py
+-rw-r--r--   0        0        0       16 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/config-exclude/.hide/hidden_mod/__init__.py
+-rw-r--r--   0        0        0       25 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/config-exclude/node_modules/node_mod/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/config-exclude/src/package/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/config-exclude/test/__init__.py
+-rw-r--r--   0        0        0       14 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/config-exclude/venv/venv_mod/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/config-up/appmap.yml
+-rw-r--r--   0        0        0        0 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/config-up/project/p1/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/config-up/project/p2/sub1/__init__.py
+-rw-r--r--   0        0        0       44 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/django/appmap.yml
+-rw-r--r--   0        0        0      495 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/django/djangoapp/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/django/djangoapp/djangoapp.py
+-rw-r--r--   0        0        0       39 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/django/djangoapp/hello_world.html
+-rw-r--r--   0        0        0      154 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/django/djangoapp/middleware.py
+-rw-r--r--   0        0        0      426 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/django/djangoapp/settings.py
+-rw-r--r--   0        0        0      563 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/django/djangoapp/settings_dev.py
+-rw-r--r--   0        0        0     2148 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/django/djangoapp/urls.py
+-rw-r--r--   0        0        0       14 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/django/init/sitecustomize.py
+-rwxr-xr-x   0        0        0      665 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/django/manage.py
+-rw-r--r--   0        0        0       53 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/django/pytest.ini
+-rw-r--r--   0        0        0        0 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/django/test/__init__.py
+-rw-r--r--   0        0        0      935 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/django/test/test_app.py
+-rw-r--r--   0        0        0     2591 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/example_class.py
+-rw-r--r--   0        0        0     7942 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/expected.appmap.json
+-rw-r--r--   0        0        0       47 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/fastapi/appmap.yml
+-rw-r--r--   0        0        0        0 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/fastapi/fastapiapp/__init__.py
+-rw-r--r--   0        0        0     1647 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/fastapi/fastapiapp/main.py
+-rw-r--r--   0        0        0       14 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/fastapi/init/sitecustomize.py
+-rw-r--r--   0        0        0      240 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/fastapi/test_app.py
+-rw-r--r--   0        0        0       38 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/flask/appmap.yml
+-rw-r--r--   0        0        0     1200 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/flask/flaskapp.py
+-rw-r--r--   0        0        0       14 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/flask/init/sitecustomize.py
+-rw-r--r--   0        0        0        0 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/flask/templates/test.html
+-rw-r--r--   0        0        0      268 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/flask/test_app.py
+-rw-r--r--   0        0        0        0 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/package1/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/package1/package2/__init__.py
+-rw-r--r--   0        0        0      113 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/package1/package2/__main__.py
+-rw-r--r--   0        0        0       69 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/package1/package2/mod1.py
+-rw-r--r--   0        0        0      653 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/params.py
+-rw-r--r--   0        0        0       38 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/pytest/appmap.yml
+-rw-r--r--   0        0        0     3972 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/pytest/expected/pytest.appmap.json
+-rw-r--r--   0        0        0      213 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/pytest/expected/status_errored.metadata.json
+-rw-r--r--   0        0        0      221 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/pytest/expected/status_failed.metadata.json
+-rw-r--r--   0        0        0      221 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/pytest/expected/status_xfailed.metadata.json
+-rw-r--r--   0        0        0      392 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/pytest/simple.py
+-rw-r--r--   0        0        0      295 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/pytest/test_noappmap.py
+-rw-r--r--   0        0        0      393 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/pytest/test_simple.py
+-rw-r--r--   0        0        0     1246 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/remote.appmap.json
+-rw-r--r--   0        0        0       13 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/trial/.gitignore
+-rw-r--r--   0        0        0       38 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/trial/appmap.yml
+-rw-r--r--   0        0        0     1897 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/trial/expected/pytest.appmap.json
+-rw-r--r--   0        0        0       14 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/trial/init/sitecustomize.py
+-rw-r--r--   0        0        0        0 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/trial/test/__init__.py
+-rw-r--r--   0        0        0      400 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/trial/test/test_deferred.py
+-rw-r--r--   0        0        0       38 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/unittest/appmap.yml
+-rw-r--r--   0        0        0     4428 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/unittest/expected/pytest.appmap.json
+-rw-r--r--   0        0        0      220 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/unittest/expected/status_errored.metadata.json
+-rw-r--r--   0        0        0      238 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/unittest/expected/status_failed.metadata.json
+-rw-r--r--   0        0        0      238 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/unittest/expected/status_xfailed.metadata.json
+-rw-r--r--   0        0        0       33 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/unittest/expected/status_xsucceeded.metadata.json
+-rw-r--r--   0        0        0     4430 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/unittest/expected/unittest.appmap.json
+-rw-r--r--   0        0        0       14 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/unittest/init/sitecustomize.py
+-rw-r--r--   0        0        0      275 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/unittest/simple/__init__.py
+-rw-r--r--   0        0        0      183 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/unittest/simple/test_noappmap.py
+-rw-r--r--   0        0        0     1263 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/data/unittest/simple/test_simple.py
+-rw-r--r--   0        0        0      734 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/helpers.py
+-rw-r--r--   0        0        0     4761 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/normalize.py
+-rw-r--r--   0        0        0     4983 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/test_command.py
+-rw-r--r--   0        0        0    11609 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/test_configuration.py
+-rw-r--r--   0        0        0     3401 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/test_describe_value.py
+-rw-r--r--   0        0        0     8341 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/test_django.py
+-rw-r--r--   0        0        0      943 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/test_django_simplelazyobject.py
+-rw-r--r--   0        0        0      338 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/test_env.py
+-rw-r--r--   0        0        0     3198 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/test_events.py
+-rw-r--r--   0        0        0     2732 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/test_fastapi.py
+-rw-r--r--   0        0        0     5065 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/test_flask.py
+-rw-r--r--   0        0        0     2216 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/test_generation.py
+-rw-r--r--   0        0        0     1548 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/test_http.py
+-rw-r--r--   0        0        0     1533 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/test_importer.py
+-rw-r--r--   0        0        0     2931 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/test_labels.py
+-rw-r--r--   0        0        0     1470 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/test_metadata.py
+-rw-r--r--   0        0        0     9877 2024-05-29 18:21:05.893437 appmap-2.0.4/_appmap/test/test_params.py
+-rw-r--r--   0        0        0     6706 2024-05-29 18:21:05.897437 appmap-2.0.4/_appmap/test/test_recording.py
+-rw-r--r--   0        0        0     2006 2024-05-29 18:21:05.897437 appmap-2.0.4/_appmap/test/test_runner.py
+-rw-r--r--   0        0        0     3086 2024-05-29 18:21:05.897437 appmap-2.0.4/_appmap/test/test_sqlalchemy.py
+-rw-r--r--   0        0        0     7261 2024-05-29 18:21:05.897437 appmap-2.0.4/_appmap/test/test_test_frameworks.py
+-rw-r--r--   0        0        0      861 2024-05-29 18:21:05.897437 appmap-2.0.4/_appmap/test/test_util.py
+-rw-r--r--   0        0        0    15340 2024-05-29 18:21:05.897437 appmap-2.0.4/_appmap/test/web_framework.py
+-rw-r--r--   0        0        0     4828 2024-05-29 18:21:05.897437 appmap-2.0.4/_appmap/testing_framework.py
+-rw-r--r--   0        0        0      370 2024-05-29 18:21:05.897437 appmap-2.0.4/_appmap/trace_logger.py
+-rw-r--r--   0        0        0     2950 2024-05-29 18:21:05.897437 appmap-2.0.4/_appmap/unittest.py
+-rw-r--r--   0        0        0     6652 2024-05-29 18:21:05.897437 appmap-2.0.4/_appmap/utils.py
+-rw-r--r--   0        0        0     8622 2024-05-29 18:21:05.897437 appmap-2.0.4/_appmap/web_framework.py
+-rw-r--r--   0        0        0     1853 2024-05-29 18:21:05.897437 appmap-2.0.4/appmap/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 18:21:05.897437 appmap-2.0.4/appmap/command/__init__.py
+-rw-r--r--   0        0        0      420 2024-05-29 18:21:05.897437 appmap-2.0.4/appmap/command/appmap_agent_init.py
+-rw-r--r--   0        0        0     3475 2024-05-29 18:21:05.897437 appmap-2.0.4/appmap/command/appmap_agent_status.py
+-rw-r--r--   0        0        0     2096 2024-05-29 18:21:05.897437 appmap-2.0.4/appmap/command/appmap_agent_validate.py
+-rw-r--r--   0        0        0     3916 2024-05-29 18:21:05.897437 appmap-2.0.4/appmap/command/runner.py
+-rw-r--r--   0        0        0    11401 2024-05-29 18:21:05.897437 appmap-2.0.4/appmap/django.py
+-rw-r--r--   0        0        0     6590 2024-05-29 18:21:05.897437 appmap-2.0.4/appmap/fastapi.py
+-rw-r--r--   0        0        0     7219 2024-05-29 18:21:05.897437 appmap-2.0.4/appmap/flask.py
+-rw-r--r--   0        0        0     2695 2024-05-29 18:21:05.897437 appmap-2.0.4/appmap/http.py
+-rw-r--r--   0        0        0      675 2024-05-29 18:21:05.897437 appmap-2.0.4/appmap/labeling/__init__.py
+-rw-r--r--   0        0        0     3387 2024-05-29 18:21:05.897437 appmap-2.0.4/appmap/labeling/crypto.yml
+-rw-r--r--   0        0        0     2097 2024-05-29 18:21:05.897437 appmap-2.0.4/appmap/labeling/django.yml
+-rw-r--r--   0        0        0      630 2024-05-29 18:21:05.897437 appmap-2.0.4/appmap/labeling/flask.yml
+-rw-r--r--   0        0        0      831 2024-05-29 18:21:05.897437 appmap-2.0.4/appmap/labeling/formats.yml
+-rw-r--r--   0        0        0       50 2024-05-29 18:21:05.897437 appmap-2.0.4/appmap/labeling/http.yml
+-rw-r--r--   0        0        0      196 2024-05-29 18:21:05.897437 appmap-2.0.4/appmap/labeling/jobs.yml
+-rw-r--r--   0        0        0       55 2024-05-29 18:21:05.897437 appmap-2.0.4/appmap/labeling/jwt.yml
+-rw-r--r--   0        0        0      137 2024-05-29 18:21:05.897437 appmap-2.0.4/appmap/labeling/logger.yml
+-rw-r--r--   0        0        0      214 2024-05-29 18:21:05.897437 appmap-2.0.4/appmap/labeling/random.yml
+-rw-r--r--   0        0        0     3282 2024-05-29 18:21:05.897437 appmap-2.0.4/appmap/pytest.py
+-rw-r--r--   0        0        0     2295 2024-05-29 18:21:05.897437 appmap-2.0.4/appmap/sqlalchemy.py
+-rw-r--r--   0        0        0      294 2024-05-29 18:21:05.897437 appmap-2.0.4/appmap/unittest.py
+-rw-r--r--   0        0        0      818 2024-05-29 18:21:05.897437 appmap-2.0.4/appmap/uvicorn.py
+-rw-r--r--   0        0        0       14 2024-05-29 18:21:05.897437 appmap-2.0.4/appmap.pth
+-rw-r--r--   0        0        0     3272 2024-05-29 18:24:14.211422 appmap-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1304 2024-05-29 18:21:05.897437 appmap-2.0.4/vendor/_appmap/wrapt/LICENSE
+-rw-r--r--   0        0        0     1200 2024-05-29 18:21:05.897437 appmap-2.0.4/vendor/_appmap/wrapt/__init__.py
+-rw-r--r--   0        0        0     1746 2024-05-29 18:21:05.897437 appmap-2.0.4/vendor/_appmap/wrapt/arguments.py
+-rw-r--r--   0        0        0    21332 2024-05-29 18:21:05.897437 appmap-2.0.4/vendor/_appmap/wrapt/decorators.py
+-rw-r--r--   0        0        0    10782 2024-05-29 18:21:05.897437 appmap-2.0.4/vendor/_appmap/wrapt/importer.py
+-rw-r--r--   0        0        0    38753 2024-05-29 18:21:05.897437 appmap-2.0.4/vendor/_appmap/wrapt/wrappers.py
+-rw-r--r--   0        0        0     5717 1970-01-01 00:00:00.000000 appmap-2.0.4/PKG-INFO
```

### Comparing `appmap-2.0.3/LICENSE` & `appmap-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/README.md` & `appmap-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/__init__.py` & `appmap-2.0.4/_appmap/__init__.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/configuration.py` & `appmap-2.0.4/_appmap/configuration.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/django.py` & `appmap-2.0.4/_appmap/django.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/env.py` & `appmap-2.0.4/_appmap/env.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/event.py` & `appmap-2.0.4/_appmap/event.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/fastapi.py` & `appmap-2.0.4/_appmap/fastapi.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/flask.py` & `appmap-2.0.4/_appmap/flask.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/generation.py` & `appmap-2.0.4/_appmap/generation.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/importer.py` & `appmap-2.0.4/_appmap/importer.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/instrument.py` & `appmap-2.0.4/_appmap/instrument.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import time
 from collections import namedtuple
 from contextlib import contextmanager
 
 from . import event
 from .env import Env
 from .event import CallEvent
-from .recorder import Recorder
+from .recorder import Recorder, AppMapTooManyEvents
 from .utils import appmap_tls
 
 logger = Env.current.getLogger(__name__)
 
 
 @contextmanager
 def recording_disabled():
@@ -93,14 +93,16 @@
         elapsed_time = time.time() - start_time
 
         return_event = event.FuncReturnEvent(
             return_value=ret, parent_id=call_event_id, elapsed=elapsed_time
         )
         Recorder.add_event(return_event)
         return ret
+    except AppMapTooManyEvents:
+        raise
     except Exception:  # noqa: E722
         elapsed_time = time.time() - start_time
         Recorder.add_event(
             event.ExceptionEvent(
                 parent_id=call_event_id, elapsed=elapsed_time, exc_info=sys.exc_info()
             )
         )
```

### Comparing `appmap-2.0.3/_appmap/labels.py` & `appmap-2.0.4/_appmap/labels.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/metadata.py` & `appmap-2.0.4/_appmap/metadata.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/py_version_check.py` & `appmap-2.0.4/_appmap/py_version_check.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/recorder.py` & `appmap-2.0.4/_appmap/recorder.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,22 +6,35 @@
 from .utils import appmap_tls
 
 logger = Env.current.getLogger(__name__)
 
 # pylint: disable=global-statement
 _default_recorder = None
 
+# Allow the user to suggest a limit on the number of events that should be added to a Recorder.
+# Depending on how exceptions get processed by the framework, there may be some more added, but it
+# shouldn't be an enormous number.
+_MAX_EVENTS = Env.current.get("APPMAP_MAX_EVENTS")
+if _MAX_EVENTS is not None:
+    _MAX_EVENTS = int(_MAX_EVENTS)
+
+
+class AppMapTooManyEvents(RuntimeError):
+    """Thrown when a recorder has more than APPMAP_MAX_EVENTS"""
+
 
 class Recorder(ABC):
     """
     A base class for Recorders.
 
     Note that the abstract methods have implementations for use by subclasses.
     """
 
+    _aborting = False
+
     @property
     @abstractmethod
     def events(self):
         return self._events
 
     _next_event_id = 0
     _next_event_id_lock = threading.Lock()
@@ -100,14 +113,15 @@
     @classmethod
     def _get_current(cls):
         perthread = appmap_tls().get(cls._RECORDER_KEY, None)
 
         return [perthread, _default_recorder]
 
     def clear(self):
+        Recorder._aborting = False
         self._events = []
 
     def __init__(self, enabled=False):
         self._events = []
         self._enabled = enabled
         self.start_tb = None
 
@@ -126,15 +140,21 @@
         logger.debug("AppMap recording stopped")
         self._enabled = False
         self.start_tb = None
         return self._events
 
     @abstractmethod
     def _add_event(self, event):
+        if Recorder._aborting:
+            return
+
         self._events.append(event)
+        if _MAX_EVENTS is not None and len(self._events) > _MAX_EVENTS:
+            Recorder._aborting = True
+            raise AppMapTooManyEvents()
 
     @staticmethod
     def _initialize():
         """Create a new default, shared recorder.
 
         This method is intentionally not thread-safe. It really doesn't make sense have multiple
         threads initializing the default recorder. If you find yourself wanting to do that, you
```

### Comparing `appmap-2.0.3/_appmap/recording.py` & `appmap-2.0.4/_appmap/recording.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/remote_recording.py` & `appmap-2.0.4/_appmap/remote_recording.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/test/appmap_test_base.py` & `appmap-2.0.4/_appmap/test/appmap_test_base.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/test/conftest.py` & `appmap-2.0.4/_appmap/test/conftest.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/test/data/django/djangoapp/settings_dev.py` & `appmap-2.0.4/_appmap/test/data/django/djangoapp/settings_dev.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/test/data/django/djangoapp/urls.py` & `appmap-2.0.4/_appmap/test/data/django/djangoapp/urls.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/test/data/django/manage.py` & `appmap-2.0.4/_appmap/test/data/django/manage.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/test/data/django/test/test_app.py` & `appmap-2.0.4/_appmap/test/data/django/test/test_app.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/test/data/example_class.py` & `appmap-2.0.4/_appmap/test/data/example_class.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/test/data/expected.appmap.json` & `appmap-2.0.4/_appmap/test/data/expected.appmap.json`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/test/data/fastapi/fastapiapp/main.py` & `appmap-2.0.4/_appmap/test/data/fastapi/fastapiapp/main.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/test/data/flask/flaskapp.py` & `appmap-2.0.4/_appmap/test/data/flask/flaskapp.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/test/data/params.py` & `appmap-2.0.4/_appmap/test/data/params.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/test/data/pytest/expected/pytest.appmap.json` & `appmap-2.0.4/_appmap/test/data/unittest/expected/pytest.appmap.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9061631944444444%*

 * *Differences: {"'classMap'": "{0: {'children': {0: {'children': {0: {'location': 'simple/__init__.py:2'}, 1: "*

 * *               "{'location': 'simple/__init__.py:8'}, 2: {'location': 'simple/__init__.py:5'}}}, "*

 * *               "insert: [(1, OrderedDict([('name', 'test_simple'), ('type', 'package'), "*

 * *               "('children', [OrderedDict([('name', 'UnitTestTest'), ('type', 'class'), "*

 * *               "('children', [OrderedDict([('name', 'test_hello_world'), ('type', 'function'), "*

 * *               "('location', 'simple/te […]*

```diff
@@ -1,136 +1,193 @@
 {
     "classMap": [
         {
             "children": [
                 {
                     "children": [
                         {
-                            "location": "simple.py:2",
+                            "location": "simple/__init__.py:2",
                             "name": "hello",
                             "static": false,
                             "type": "function"
                         },
                         {
-                            "location": "simple.py:8",
+                            "location": "simple/__init__.py:8",
                             "name": "hello_world",
                             "static": false,
                             "type": "function"
                         },
                         {
-                            "location": "simple.py:5",
+                            "location": "simple/__init__.py:5",
                             "name": "world",
                             "static": false,
                             "type": "function"
                         }
                     ],
                     "name": "Simple",
                     "type": "class"
+                },
+                {
+                    "children": [
+                        {
+                            "children": [
+                                {
+                                    "location": "simple/test_simple.py:14",
+                                    "name": "test_hello_world",
+                                    "static": false,
+                                    "type": "function"
+                                }
+                            ],
+                            "name": "UnitTestTest",
+                            "type": "class"
+                        }
+                    ],
+                    "name": "test_simple",
+                    "type": "package"
                 }
             ],
             "name": "simple",
             "type": "package"
         }
     ],
     "events": [
         {
-            "defined_class": "simple.Simple",
+            "defined_class": "simple.test_simple.UnitTestTest",
             "event": "call",
             "id": 1,
+            "lineno": 14,
+            "method_id": "test_hello_world",
+            "parameters": [],
+            "path": "simple/test_simple.py",
+            "receiver": {
+                "class": "simple.test_simple.UnitTestTest",
+                "kind": "req",
+                "name": "self",
+                "value": "<simple.test_simple.UnitTestTest testMethod=test_hello_world>"
+            },
+            "static": false,
+            "thread_id": 1
+        },
+        {
+            "defined_class": "simple.Simple",
+            "event": "call",
+            "id": 2,
             "lineno": 8,
             "method_id": "hello_world",
-            "parameters": [],
-            "path": "simple.py",
+            "parameters": [
+                {
+                    "class": "builtins.str",
+                    "kind": "req",
+                    "name": "bang",
+                    "value": "'!'"
+                }
+            ],
+            "path": "simple/__init__.py",
             "receiver": {
                 "class": "simple.Simple",
                 "kind": "req",
                 "name": "self",
                 "value": "<simple.Simple object at 0xabcdef>"
             },
             "static": false,
             "thread_id": 1
         },
         {
             "defined_class": "simple.Simple",
             "event": "call",
-            "id": 2,
+            "id": 3,
             "lineno": 2,
             "method_id": "hello",
             "parameters": [],
-            "path": "simple.py",
+            "path": "simple/__init__.py",
             "receiver": {
                 "class": "simple.Simple",
                 "kind": "req",
                 "name": "self",
                 "value": "<simple.Simple object at 0xabcdef>"
             },
             "static": false,
             "thread_id": 1
         },
         {
             "event": "return",
-            "id": 3,
-            "parent_id": 2,
+            "id": 4,
+            "parent_id": 3,
             "return_value": {
                 "class": "builtins.str",
                 "value": "'Hello'"
             },
             "thread_id": 1
         },
         {
             "defined_class": "simple.Simple",
             "event": "call",
-            "id": 4,
+            "id": 5,
             "lineno": 5,
             "method_id": "world",
             "parameters": [],
-            "path": "simple.py",
+            "path": "simple/__init__.py",
             "receiver": {
                 "class": "simple.Simple",
                 "kind": "req",
                 "name": "self",
                 "value": "<simple.Simple object at 0xabcdef>"
             },
             "static": false,
             "thread_id": 1
         },
         {
             "event": "return",
-            "id": 5,
-            "parent_id": 4,
+            "id": 6,
+            "parent_id": 5,
             "return_value": {
                 "class": "builtins.str",
-                "value": "'world!'"
+                "value": "'world'"
             },
             "thread_id": 1
         },
         {
             "event": "return",
-            "id": 6,
-            "parent_id": 1,
+            "id": 7,
+            "parent_id": 2,
             "return_value": {
                 "class": "builtins.str",
                 "value": "'Hello world!'"
             },
             "thread_id": 1
+        },
+        {
+            "event": "return",
+            "id": 8,
+            "parent_id": 1,
+            "return_value": {
+                "class": "builtins.NoneType",
+                "value": "None"
+            },
+            "thread_id": 1
         }
     ],
     "metadata": {
         "app": "Simple",
         "client": {
             "name": "appmap",
             "url": "https://github.com/applandinc/appmap-python"
         },
         "feature": "Hello world",
+        "feature_group": "Unit test test",
         "language": {
             "name": "python"
         },
-        "name": "hello world",
+        "name": "Unit test test hello world",
         "recorder": {
             "name": "pytest",
             "type": "tests"
         },
-        "source_location": "test_simple.py:5",
+        "recording": {
+            "defined_class": "simple.test_simple.UnitTestTest",
+            "method_id": "test_hello_world"
+        },
+        "source_location": "simple/test_simple.py:13",
         "test_status": "succeeded"
     },
     "version": "1.9"
 }
```

### Comparing `appmap-2.0.3/_appmap/test/data/remote.appmap.json` & `appmap-2.0.4/_appmap/test/data/remote.appmap.json`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/test/data/trial/expected/pytest.appmap.json` & `appmap-2.0.4/_appmap/test/data/trial/expected/pytest.appmap.json`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/test/data/unittest/expected/pytest.appmap.json` & `appmap-2.0.4/_appmap/test/data/unittest/expected/unittest.appmap.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9921875%*

 * *Differences: {"'metadata'": "{'source_location': 'simple/test_simple.py:14', 'recorder': {'name': 'unittest'}}"}*

```diff
@@ -175,19 +175,19 @@
         "feature": "Hello world",
         "feature_group": "Unit test test",
         "language": {
             "name": "python"
         },
         "name": "Unit test test hello world",
         "recorder": {
-            "name": "pytest",
+            "name": "unittest",
             "type": "tests"
         },
         "recording": {
             "defined_class": "simple.test_simple.UnitTestTest",
             "method_id": "test_hello_world"
         },
-        "source_location": "simple/test_simple.py:13",
+        "source_location": "simple/test_simple.py:14",
         "test_status": "succeeded"
     },
     "version": "1.9"
 }
```

### Comparing `appmap-2.0.3/_appmap/test/data/unittest/expected/unittest.appmap.json` & `appmap-2.0.4/_appmap/test/data/pytest/expected/pytest.appmap.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9380099826388888%*

 * *Differences: {"'classMap'": "{0: {'children': {0: {'children': {1: {'location': 'simple.py:7'}, 2: {'location': "*

 * *               "'simple.py:16'}, 3: {'location': 'simple.py:10'}, insert: [(0, "*

 * *               "OrderedDict([('name', 'get_non_json_serializable'), ('type', 'function'), "*

 * *               "('location', 'simple.py:13'), ('static', False)]))]}}, delete: [1]}}}",*

 * * "'events'": "{0: {'defined_class': 'simple.Simple', 'method_id': 'hello_world', 'path': "*

 * *             "'simple.py', 'lineno': 16, 'receiver': {'clas […]*

```diff
@@ -1,108 +1,89 @@
 {
     "classMap": [
         {
             "children": [
                 {
                     "children": [
                         {
-                            "location": "simple/__init__.py:2",
+                            "location": "simple.py:13",
+                            "name": "get_non_json_serializable",
+                            "static": false,
+                            "type": "function"
+                        },
+                        {
+                            "location": "simple.py:7",
                             "name": "hello",
                             "static": false,
                             "type": "function"
                         },
                         {
-                            "location": "simple/__init__.py:8",
+                            "location": "simple.py:16",
                             "name": "hello_world",
                             "static": false,
                             "type": "function"
                         },
                         {
-                            "location": "simple/__init__.py:5",
+                            "location": "simple.py:10",
                             "name": "world",
                             "static": false,
                             "type": "function"
                         }
                     ],
                     "name": "Simple",
                     "type": "class"
-                },
-                {
-                    "children": [
-                        {
-                            "children": [
-                                {
-                                    "location": "simple/test_simple.py:14",
-                                    "name": "test_hello_world",
-                                    "static": false,
-                                    "type": "function"
-                                }
-                            ],
-                            "name": "UnitTestTest",
-                            "type": "class"
-                        }
-                    ],
-                    "name": "test_simple",
-                    "type": "package"
                 }
             ],
             "name": "simple",
             "type": "package"
         }
     ],
     "events": [
         {
-            "defined_class": "simple.test_simple.UnitTestTest",
+            "defined_class": "simple.Simple",
             "event": "call",
             "id": 1,
-            "lineno": 14,
-            "method_id": "test_hello_world",
+            "lineno": 16,
+            "method_id": "hello_world",
             "parameters": [],
-            "path": "simple/test_simple.py",
+            "path": "simple.py",
             "receiver": {
-                "class": "simple.test_simple.UnitTestTest",
+                "class": "simple.Simple",
                 "kind": "req",
                 "name": "self",
-                "value": "<simple.test_simple.UnitTestTest testMethod=test_hello_world>"
+                "value": "<simple.Simple object at 0xabcdef>"
             },
             "static": false,
             "thread_id": 1
         },
         {
             "defined_class": "simple.Simple",
             "event": "call",
             "id": 2,
-            "lineno": 8,
-            "method_id": "hello_world",
-            "parameters": [
-                {
-                    "class": "builtins.str",
-                    "kind": "req",
-                    "name": "bang",
-                    "value": "'!'"
-                }
-            ],
-            "path": "simple/__init__.py",
+            "lineno": 13,
+            "method_id": "get_non_json_serializable",
+            "parameters": [],
+            "path": "simple.py",
             "receiver": {
                 "class": "simple.Simple",
                 "kind": "req",
                 "name": "self",
                 "value": "<simple.Simple object at 0xabcdef>"
             },
             "static": false,
             "thread_id": 1
         },
         {
             "defined_class": "simple.Simple",
             "event": "call",
             "id": 3,
-            "lineno": 2,
+            "lineno": 7,
             "method_id": "hello",
             "parameters": [],
-            "path": "simple/__init__.py",
+            "path": "simple.py",
             "receiver": {
                 "class": "simple.Simple",
                 "kind": "req",
                 "name": "self",
                 "value": "<simple.Simple object at 0xabcdef>"
             },
             "static": false,
@@ -118,18 +99,18 @@
             },
             "thread_id": 1
         },
         {
             "defined_class": "simple.Simple",
             "event": "call",
             "id": 5,
-            "lineno": 5,
+            "lineno": 10,
             "method_id": "world",
             "parameters": [],
-            "path": "simple/__init__.py",
+            "path": "simple.py",
             "receiver": {
                 "class": "simple.Simple",
                 "kind": "req",
                 "name": "self",
                 "value": "<simple.Simple object at 0xabcdef>"
             },
             "static": false,
@@ -137,57 +118,63 @@
         },
         {
             "event": "return",
             "id": 6,
             "parent_id": 5,
             "return_value": {
                 "class": "builtins.str",
-                "value": "'world'"
+                "value": "'world!'"
             },
             "thread_id": 1
         },
         {
             "event": "return",
             "id": 7,
             "parent_id": 2,
             "return_value": {
-                "class": "builtins.str",
-                "value": "'Hello world!'"
+                "class": "builtins.dict",
+                "properties": [
+                    {
+                        "class": "builtins.str",
+                        "name": "0"
+                    },
+                    {
+                        "class": "builtins.str",
+                        "name": "1"
+                    }
+                ],
+                "size": 2,
+                "value": "{0: 'Hello', 1: 'world!'}"
             },
             "thread_id": 1
         },
         {
             "event": "return",
             "id": 8,
             "parent_id": 1,
             "return_value": {
-                "class": "builtins.NoneType",
-                "value": "None"
+                "class": "builtins.str",
+                "value": "'Hello world!'"
             },
             "thread_id": 1
         }
     ],
     "metadata": {
         "app": "Simple",
         "client": {
             "name": "appmap",
             "url": "https://github.com/applandinc/appmap-python"
         },
         "feature": "Hello world",
-        "feature_group": "Unit test test",
         "language": {
             "name": "python"
         },
-        "name": "Unit test test hello world",
+        "name": "hello world",
         "recorder": {
-            "name": "unittest",
+            "name": "pytest",
             "type": "tests"
         },
-        "recording": {
-            "defined_class": "simple.test_simple.UnitTestTest",
-            "method_id": "test_hello_world"
-        },
-        "source_location": "simple/test_simple.py:14",
+        "source_location": "test_simple.py:5",
         "test_status": "succeeded"
     },
     "version": "1.9"
 }
```

### Comparing `appmap-2.0.3/_appmap/test/data/unittest/simple/test_simple.py` & `appmap-2.0.4/_appmap/test/data/unittest/simple/test_simple.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/test/helpers.py` & `appmap-2.0.4/_appmap/test/helpers.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/test/normalize.py` & `appmap-2.0.4/_appmap/test/normalize.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/test/test_command.py` & `appmap-2.0.4/_appmap/test/test_command.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/test/test_configuration.py` & `appmap-2.0.4/_appmap/test/test_configuration.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/test/test_describe_value.py` & `appmap-2.0.4/_appmap/test/test_describe_value.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/test/test_django.py` & `appmap-2.0.4/_appmap/test/test_django.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/test/test_django_simplelazyobject.py` & `appmap-2.0.4/_appmap/test/test_django_simplelazyobject.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/test/test_events.py` & `appmap-2.0.4/_appmap/test/test_events.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/test/test_fastapi.py` & `appmap-2.0.4/_appmap/test/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/test/test_flask.py` & `appmap-2.0.4/_appmap/test/test_flask.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/test/test_http.py` & `appmap-2.0.4/_appmap/test/test_http.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/test/test_importer.py` & `appmap-2.0.4/_appmap/test/test_importer.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/test/test_labels.py` & `appmap-2.0.4/_appmap/test/test_labels.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/test/test_metadata.py` & `appmap-2.0.4/_appmap/test/test_metadata.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/test/test_params.py` & `appmap-2.0.4/_appmap/test/test_params.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/test/test_recording.py` & `appmap-2.0.4/_appmap/test/test_recording.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/test/test_runner.py` & `appmap-2.0.4/_appmap/test/test_runner.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/test/test_sqlalchemy.py` & `appmap-2.0.4/_appmap/test/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/test/test_test_frameworks.py` & `appmap-2.0.4/_appmap/test/test_test_frameworks.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/test/test_util.py` & `appmap-2.0.4/_appmap/test/test_util.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/test/web_framework.py` & `appmap-2.0.4/_appmap/test/web_framework.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/testing_framework.py` & `appmap-2.0.4/_appmap/testing_framework.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/unittest.py` & `appmap-2.0.4/_appmap/unittest.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/utils.py` & `appmap-2.0.4/_appmap/utils.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/_appmap/web_framework.py` & `appmap-2.0.4/_appmap/web_framework.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/appmap/__init__.py` & `appmap-2.0.4/appmap/__init__.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/appmap/command/appmap_agent_status.py` & `appmap-2.0.4/appmap/command/appmap_agent_status.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/appmap/command/appmap_agent_validate.py` & `appmap-2.0.4/appmap/command/appmap_agent_validate.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/appmap/command/runner.py` & `appmap-2.0.4/appmap/command/runner.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/appmap/django.py` & `appmap-2.0.4/appmap/django.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/appmap/fastapi.py` & `appmap-2.0.4/appmap/fastapi.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/appmap/flask.py` & `appmap-2.0.4/appmap/flask.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/appmap/http.py` & `appmap-2.0.4/appmap/http.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/appmap/labeling/__init__.py` & `appmap-2.0.4/appmap/labeling/__init__.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/appmap/labeling/crypto.yml` & `appmap-2.0.4/appmap/labeling/crypto.yml`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/appmap/labeling/django.yml` & `appmap-2.0.4/appmap/labeling/django.yml`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/appmap/labeling/flask.yml` & `appmap-2.0.4/appmap/labeling/flask.yml`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/appmap/labeling/formats.yml` & `appmap-2.0.4/appmap/labeling/formats.yml`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/appmap/pytest.py` & `appmap-2.0.4/appmap/pytest.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/appmap/sqlalchemy.py` & `appmap-2.0.4/appmap/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/appmap/uvicorn.py` & `appmap-2.0.4/appmap/uvicorn.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/pyproject.toml` & `appmap-2.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "appmap"
-version = "2.0.3"
+version = "2.0.4"
 description = "Create AppMap files by recording a Python application."
 readme = "README.md"
 authors = [
   "Alan Potter <alan@app.land>",
   "Viraj Kanwade <viraj.kanwade@forgeahead.io>",
   "Rafał Rzepecki <rafal@app.land>"
 ]
```

### Comparing `appmap-2.0.3/vendor/_appmap/wrapt/LICENSE` & `appmap-2.0.4/vendor/_appmap/wrapt/LICENSE`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/vendor/_appmap/wrapt/__init__.py` & `appmap-2.0.4/vendor/_appmap/wrapt/__init__.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/vendor/_appmap/wrapt/arguments.py` & `appmap-2.0.4/vendor/_appmap/wrapt/arguments.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/vendor/_appmap/wrapt/decorators.py` & `appmap-2.0.4/vendor/_appmap/wrapt/decorators.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/vendor/_appmap/wrapt/importer.py` & `appmap-2.0.4/vendor/_appmap/wrapt/importer.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/vendor/_appmap/wrapt/wrappers.py` & `appmap-2.0.4/vendor/_appmap/wrapt/wrappers.py`

 * *Files identical despite different names*

### Comparing `appmap-2.0.3/PKG-INFO` & `appmap-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appmap
-Version: 2.0.3
+Version: 2.0.4
 Summary: Create AppMap files by recording a Python application.
 Home-page: https://github.com/applandinc/appmap-python
 License: MIT
 Author: Alan Potter
 Author-email: alan@app.land
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

