# Comparing `tmp/logfire-0.36.1.tar.gz` & `tmp/logfire-0.37.0.tar.gz`

## Comparing `logfire-0.36.1.tar` & `logfire-0.37.0.tar`

### file list

```diff
@@ -1,130 +1,130 @@
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 logfire-0.36.1/Makefile
--rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/__main__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/cli.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/exceptions.py
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/propagate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/py.typed
--rw-r--r--   0        0        0     9570 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/testing.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/version.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/__init__.py
--rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/ast_utils.py
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/async_.py
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/auth.py
--rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/backfill.py
--rw-r--r--   0        0        0    18512 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/cli.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/collect_system_info.py
--rw-r--r--   0        0        0    56230 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/config.py
--rw-r--r--   0        0        0    11225 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/config_params.py
--rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/constants.py
--rw-r--r--   0        0        0    19127 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/formatter.py
--rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/instrument.py
--rw-r--r--   0        0        0     9035 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/json_encoder.py
--rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/json_formatter.py
--rw-r--r--   0        0        0    13081 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/json_schema.py
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/json_types.py
--rw-r--r--   0        0        0    63477 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/main.py
--rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/metrics.py
--rw-r--r--   0        0        0     8756 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/scrubbing.py
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/stack_info.py
--rw-r--r--   0        0        0    10602 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/tracer.py
--rw-r--r--   0        0        0     6384 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/utils.py
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/auto_trace/__init__.py
--rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/auto_trace/import_hook.py
--rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/auto_trace/rewrite_ast.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/auto_trace/types.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/exporters/__init__.py
--rw-r--r--   0        0        0    18968 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/exporters/console.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/exporters/fallback.py
--rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/exporters/file.py
--rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/exporters/otlp.py
--rw-r--r--   0        0        0     9014 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/exporters/processor_wrapper.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/exporters/remove_pending.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/exporters/wrapper.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/integrations/__init__.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/integrations/asyncpg.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/integrations/django.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/integrations/executors.py
--rw-r--r--   0        0        0    10656 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/integrations/fastapi.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/integrations/httpx.py
--rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/integrations/psycopg.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/integrations/requests.py
--rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/integrations/llm_providers/anthropic.py
--rw-r--r--   0        0        0     7796 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/integrations/llm_providers/llm_provider.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/integrations/llm_providers/openai.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/_internal/integrations/llm_providers/types.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/integrations/__init__.py
--rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/integrations/logging.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/integrations/loguru.py
--rw-r--r--   0        0        0    19169 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/integrations/pydantic.py
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 logfire-0.36.1/logfire/integrations/structlog.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/__init__.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/conftest.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/module_used_for_tests.py
--rw-r--r--   0        0        0    19034 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/test_auto_trace.py
--rw-r--r--   0        0        0     9988 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/test_backfill.py
--rw-r--r--   0        0        0    47077 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/test_cli.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/test_collect_package_resources.py
--rw-r--r--   0        0        0    53700 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/test_configure.py
--rw-r--r--   0        0        0    29388 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/test_console_exporter.py
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/test_formatter.py
--rw-r--r--   0        0        0    45893 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/test_json_args.py
--rw-r--r--   0        0        0    19936 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/test_json_args_formatting.py
--rw-r--r--   0        0        0   105498 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/test_logfire.py
--rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/test_loguru.py
--rw-r--r--   0        0        0    11914 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/test_metrics.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/test_no_production.py
--rw-r--r--   0        0        0    54162 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/test_pydantic_plugin.py
--rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/test_sampling.py
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/test_secret_scrubbing.py
--rw-r--r--   0        0        0     7270 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/test_slow_async_callbacks.py
--rw-r--r--   0        0        0     8126 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/test_source_code_extraction.py
--rw-r--r--   0        0        0    12334 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/test_stdlib_logging.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/test_structlog.py
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/test_testing.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/test_utils.py
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/auto_trace_samples/__init__.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/auto_trace_samples/foo.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/auto_trace_samples/simple_nesting.py
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/exporters/test_fallback_exporter.py
--rw-r--r--   0        0        0     8384 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/exporters/test_file_exporter.py
--rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/exporters/test_otlp_session.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/exporters/test_remove_pending.py
--rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/exporters/test_retry_fewer_spans.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/import_used_for_tests/__init__.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/import_used_for_tests/slow_async_callbacks_example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/import_used_for_tests/a/__init__.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/import_used_for_tests/a/b.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/otel_integrations/__init__.py
--rw-r--r--   0        0        0    24476 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/otel_integrations/test_anthropic.py
--rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/otel_integrations/test_asgi.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/otel_integrations/test_asyncpg.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/otel_integrations/test_django.py
--rw-r--r--   0        0        0    44449 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/otel_integrations/test_fastapi.py
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/otel_integrations/test_flask.py
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/otel_integrations/test_httpx.py
--rw-r--r--   0        0        0    44469 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/otel_integrations/test_openai.py
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/otel_integrations/test_psycopg.py
--rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/otel_integrations/test_requests.py
--rw-r--r--   0        0        0     7890 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/otel_integrations/test_sqlalchemy.py
--rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/otel_integrations/test_starlette.py
--rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/otel_integrations/test_wsgi.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/otel_integrations/django_test_project/__init__.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/otel_integrations/django_test_project/manage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/otel_integrations/django_test_project/django_test_app/__init__.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/otel_integrations/django_test_project/django_test_app/admin.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/otel_integrations/django_test_project/django_test_app/apps.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/otel_integrations/django_test_project/django_test_app/models.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/otel_integrations/django_test_project/django_test_app/urls.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/otel_integrations/django_test_project/django_test_app/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/otel_integrations/django_test_project/django_test_app/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/otel_integrations/django_test_project/django_test_site/__init__.py
--rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/otel_integrations/django_test_project/django_test_site/settings.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/otel_integrations/django_test_project/django_test_site/urls.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 logfire-0.36.1/tests/otel_integrations/django_test_project/django_test_site/wsgi.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 logfire-0.36.1/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 logfire-0.36.1/LICENSE
--rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 logfire-0.36.1/README.md
--rw-r--r--   0        0        0     8521 2020-02-02 00:00:00.000000 logfire-0.36.1/pyproject.toml
--rw-r--r--   0        0        0     7731 2020-02-02 00:00:00.000000 logfire-0.36.1/PKG-INFO
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 logfire-0.37.0/Makefile
+-rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/__main__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/cli.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/exceptions.py
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/propagate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/py.typed
+-rw-r--r--   0        0        0     9570 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/testing.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/version.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/__init__.py
+-rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/ast_utils.py
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/async_.py
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/auth.py
+-rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/backfill.py
+-rw-r--r--   0        0        0    18512 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/cli.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/collect_system_info.py
+-rw-r--r--   0        0        0    56043 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/config.py
+-rw-r--r--   0        0        0    11225 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/config_params.py
+-rw-r--r--   0        0        0     5179 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/constants.py
+-rw-r--r--   0        0        0    19127 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/formatter.py
+-rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/instrument.py
+-rw-r--r--   0        0        0     9035 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/json_encoder.py
+-rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/json_formatter.py
+-rw-r--r--   0        0        0    13081 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/json_schema.py
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/json_types.py
+-rw-r--r--   0        0        0    63477 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/main.py
+-rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/metrics.py
+-rw-r--r--   0        0        0     8756 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/scrubbing.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/stack_info.py
+-rw-r--r--   0        0        0    10602 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/tracer.py
+-rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/utils.py
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/auto_trace/__init__.py
+-rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/auto_trace/import_hook.py
+-rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/auto_trace/rewrite_ast.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/auto_trace/types.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/exporters/__init__.py
+-rw-r--r--   0        0        0    18968 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/exporters/console.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/exporters/fallback.py
+-rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/exporters/file.py
+-rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/exporters/otlp.py
+-rw-r--r--   0        0        0     8977 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/exporters/processor_wrapper.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/exporters/remove_pending.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/exporters/wrapper.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/integrations/__init__.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/integrations/asyncpg.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/integrations/django.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/integrations/executors.py
+-rw-r--r--   0        0        0    10656 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/integrations/fastapi.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/integrations/httpx.py
+-rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/integrations/psycopg.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/integrations/requests.py
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/integrations/llm_providers/anthropic.py
+-rw-r--r--   0        0        0     7683 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/integrations/llm_providers/llm_provider.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/integrations/llm_providers/openai.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/integrations/llm_providers/types.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/integrations/__init__.py
+-rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/integrations/logging.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/integrations/loguru.py
+-rw-r--r--   0        0        0    19169 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/integrations/pydantic.py
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/integrations/structlog.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/__init__.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/conftest.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/module_used_for_tests.py
+-rw-r--r--   0        0        0    19034 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_auto_trace.py
+-rw-r--r--   0        0        0     9988 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_backfill.py
+-rw-r--r--   0        0        0    47077 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_cli.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_collect_package_resources.py
+-rw-r--r--   0        0        0    53700 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_configure.py
+-rw-r--r--   0        0        0    29388 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_console_exporter.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_formatter.py
+-rw-r--r--   0        0        0    45893 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_json_args.py
+-rw-r--r--   0        0        0    19936 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_json_args_formatting.py
+-rw-r--r--   0        0        0   107358 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_logfire.py
+-rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_loguru.py
+-rw-r--r--   0        0        0    11914 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_metrics.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_no_production.py
+-rw-r--r--   0        0        0    54162 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_pydantic_plugin.py
+-rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_sampling.py
+-rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_secret_scrubbing.py
+-rw-r--r--   0        0        0     7270 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_slow_async_callbacks.py
+-rw-r--r--   0        0        0     8126 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_source_code_extraction.py
+-rw-r--r--   0        0        0    12433 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_stdlib_logging.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_structlog.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_testing.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_utils.py
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/auto_trace_samples/__init__.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/auto_trace_samples/foo.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/auto_trace_samples/simple_nesting.py
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/exporters/test_fallback_exporter.py
+-rw-r--r--   0        0        0     8384 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/exporters/test_file_exporter.py
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/exporters/test_otlp_session.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/exporters/test_remove_pending.py
+-rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/exporters/test_retry_fewer_spans.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/import_used_for_tests/__init__.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/import_used_for_tests/slow_async_callbacks_example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/import_used_for_tests/a/__init__.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/import_used_for_tests/a/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/__init__.py
+-rw-r--r--   0        0        0    24476 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/test_anthropic.py
+-rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/test_asgi.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/test_asyncpg.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/test_django.py
+-rw-r--r--   0        0        0    44449 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/test_fastapi.py
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/test_flask.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/test_httpx.py
+-rw-r--r--   0        0        0    44244 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/test_openai.py
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/test_psycopg.py
+-rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/test_requests.py
+-rw-r--r--   0        0        0     7890 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/test_sqlalchemy.py
+-rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/test_starlette.py
+-rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/test_wsgi.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/django_test_project/__init__.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/django_test_project/manage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/django_test_project/django_test_app/__init__.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/django_test_project/django_test_app/admin.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/django_test_project/django_test_app/apps.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/django_test_project/django_test_app/models.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/django_test_project/django_test_app/urls.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/django_test_project/django_test_app/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/django_test_project/django_test_app/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/django_test_project/django_test_site/__init__.py
+-rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/django_test_project/django_test_site/settings.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/django_test_project/django_test_site/urls.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/django_test_project/django_test_site/wsgi.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 logfire-0.37.0/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 logfire-0.37.0/LICENSE
+-rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 logfire-0.37.0/README.md
+-rw-r--r--   0        0        0     8521 2020-02-02 00:00:00.000000 logfire-0.37.0/pyproject.toml
+-rw-r--r--   0        0        0     7731 2020-02-02 00:00:00.000000 logfire-0.37.0/PKG-INFO
```

### Comparing `logfire-0.36.1/Makefile` & `logfire-0.37.0/Makefile`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/__init__.py` & `logfire-0.37.0/logfire/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     PydanticPlugin,
     configure,
 )
 from ._internal.constants import LevelName
 from ._internal.exporters.file import load_file as load_spans_from_file
 from ._internal.main import Logfire, LogfireSpan
 from ._internal.scrubbing import ScrubMatch
+from ._internal.utils import suppress_instrumentation
 from .integrations.logging import LogfireLoggingHandler
 from .integrations.structlog import LogfireProcessor as StructlogProcessor
 from .version import VERSION
 
 DEFAULT_LOGFIRE_INSTANCE = Logfire()
 span = DEFAULT_LOGFIRE_INSTANCE.span
 instrument = DEFAULT_LOGFIRE_INSTANCE.instrument
@@ -97,10 +98,11 @@
     'with_tags',
     # 'with_trace_sample_rate',
     'load_spans_from_file',
     'no_auto_trace',
     'METRICS_PREFERRED_TEMPORALITY',
     'ScrubMatch',
     'VERSION',
+    'suppress_instrumentation',
     'StructlogProcessor',
     'LogfireLoggingHandler',
 )
```

### Comparing `logfire-0.36.1/logfire/propagate.py` & `logfire-0.37.0/logfire/propagate.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/testing.py` & `logfire-0.37.0/logfire/testing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/_internal/ast_utils.py` & `logfire-0.37.0/logfire/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/_internal/async_.py` & `logfire-0.37.0/logfire/_internal/async_.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/_internal/auth.py` & `logfire-0.37.0/logfire/_internal/auth.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/_internal/backfill.py` & `logfire-0.37.0/logfire/_internal/backfill.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/_internal/cli.py` & `logfire-0.37.0/logfire/_internal/cli.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/_internal/config.py` & `logfire-0.37.0/logfire/_internal/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from threading import RLock
 from typing import Any, Callable, Literal, Sequence, cast
 from urllib.parse import urljoin
 from uuid import uuid4
 
 import requests
 from opentelemetry import metrics, trace
-from opentelemetry.context import attach, detach, set_value
 from opentelemetry.environment_variables import OTEL_TRACES_EXPORTER
 from opentelemetry.exporter.otlp.proto.http.metric_exporter import OTLPMetricExporter
 from opentelemetry.exporter.otlp.proto.http.trace_exporter import OTLPSpanExporter
 from opentelemetry.sdk.environment_variables import (
     OTEL_BSP_SCHEDULE_DELAY,
     OTEL_EXPORTER_OTLP_METRICS_ENDPOINT,
     OTEL_EXPORTER_OTLP_TRACES_ENDPOINT,
@@ -53,15 +52,14 @@
 from .auth import DEFAULT_FILE, DefaultFile, is_logged_in
 from .collect_system_info import collect_package_info
 from .config_params import ParamManager, PydanticPluginRecordValues
 from .constants import (
     DEFAULT_FALLBACK_FILE_NAME,
     OTLP_MAX_BODY_SIZE,
     RESOURCE_ATTRIBUTES_PACKAGE_VERSIONS,
-    SUPPRESS_INSTRUMENTATION_CONTEXT_KEY,
     LevelName,
 )
 from .exporters.console import (
     ConsoleColorsValues,
     IndentedConsoleSpanExporter,
     ShowParentsConsoleSpanExporter,
     SimpleConsoleSpanExporter,
@@ -71,15 +69,15 @@
 from .exporters.otlp import OTLPExporterHttpSession, RetryFewerSpansSpanExporter
 from .exporters.processor_wrapper import SpanProcessorWrapper
 from .exporters.remove_pending import RemovePendingSpansExporter
 from .integrations.executors import instrument_executors
 from .metrics import ProxyMeterProvider, configure_metrics
 from .scrubbing import Scrubber, ScrubCallback
 from .tracer import PendingSpanProcessor, ProxyTracerProvider
-from .utils import UnexpectedResponse, ensure_data_dir_exists, get_version, read_toml_file
+from .utils import UnexpectedResponse, ensure_data_dir_exists, get_version, read_toml_file, suppress_instrumentation
 
 CREDENTIALS_FILENAME = 'logfire_credentials.json'
 """Default base URL for the Logfire API."""
 COMMON_REQUEST_HEADERS = {'User-Agent': f'logfire/{VERSION}'}
 """Common request headers for requests to the Logfire API."""
 PROJECT_NAME_PATTERN = r'^[a-z0-9]+(?:-[a-z0-9]+)*$'
 
@@ -547,16 +545,15 @@
         with self._lock:
             return self._initialize()
 
     def _initialize(self) -> ProxyTracerProvider:
         if self._initialized:  # pragma: no cover
             return self._tracer_provider
 
-        backup_context = attach(set_value(SUPPRESS_INSTRUMENTATION_CONTEXT_KEY, True))
-        try:
+        with suppress_instrumentation():
             otel_resource_attributes: dict[str, Any] = {
                 ResourceAttributes.SERVICE_NAME: self.service_name,
                 RESOURCE_ATTRIBUTES_PACKAGE_VERSIONS: json.dumps(collect_package_info(), separators=(',', ':')),
                 ResourceAttributes.PROCESS_PID: os.getpid(),
             }
             if self.service_version:
                 otel_resource_attributes[ResourceAttributes.SERVICE_VERSION] = self.service_version
@@ -699,16 +696,14 @@
                 metrics.set_meter_provider(self._meter_provider)
 
             self._initialized = True
 
             # set up context propagation for ThreadPoolExecutor and ProcessPoolExecutor
             instrument_executors()
             return self._tracer_provider
-        finally:
-            detach(backup_context)
 
     def get_tracer_provider(self) -> ProxyTracerProvider:
         """Get a tracer provider from this `LogfireConfig`.
 
         This is used internally and should not be called by users of the SDK.
 
         Returns:
```

### Comparing `logfire-0.36.1/logfire/_internal/config_params.py` & `logfire-0.37.0/logfire/_internal/config_params.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/_internal/constants.py` & `logfire-0.37.0/logfire/_internal/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -144,18 +144,14 @@
 
 OTLP_MAX_INT_SIZE = 2**63 - 1
 """OTLP only supports signed 64-bit integers, larger integers get sent as strings."""
 
 DEFAULT_FALLBACK_FILE_NAME = 'logfire_spans.bin'
 """The default name of the fallback file, used when the API is unreachable."""
 
-# see https://github.com/open-telemetry/opentelemetry-python/blob/d054dff47d2da663a39b9656d106c3d15f344269/opentelemetry-api/src/opentelemetry/context/__init__.py#L171
-SUPPRESS_INSTRUMENTATION_CONTEXT_KEY = 'suppress_instrumentation'
-"""Key in OTEL context that indicates whether instrumentation should be suppressed."""
-
 ATTRIBUTES_SAMPLE_RATE_KEY = 'logfire.sample_rate'
 """Key in attributes that indicates the sample rate for this span."""
 
 CONTEXT_ATTRIBUTES_KEY = create_key('logfire.attributes')  # note this has a random suffix that OTEL adds
 """Key in the OTEL context that contains the logfire attributes."""
 
 CONTEXT_SAMPLE_RATE_KEY = create_key('logfire.sample-rate')  # note this has a random suffix that OTEL adds
```

### Comparing `logfire-0.36.1/logfire/_internal/formatter.py` & `logfire-0.37.0/logfire/_internal/formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/_internal/instrument.py` & `logfire-0.37.0/logfire/_internal/instrument.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/_internal/json_encoder.py` & `logfire-0.37.0/logfire/_internal/json_encoder.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/_internal/json_formatter.py` & `logfire-0.37.0/logfire/_internal/json_formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/_internal/json_schema.py` & `logfire-0.37.0/logfire/_internal/json_schema.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/_internal/json_types.py` & `logfire-0.37.0/logfire/_internal/json_types.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/_internal/main.py` & `logfire-0.37.0/logfire/_internal/main.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/_internal/metrics.py` & `logfire-0.37.0/logfire/_internal/metrics.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/_internal/scrubbing.py` & `logfire-0.37.0/logfire/_internal/scrubbing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/_internal/stack_info.py` & `logfire-0.37.0/logfire/_internal/stack_info.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/_internal/tracer.py` & `logfire-0.37.0/logfire/_internal/tracer.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/_internal/utils.py` & `logfire-0.37.0/logfire/_internal/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 import json
 import sys
+from contextlib import contextmanager
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, List, Mapping, Sequence, Tuple, TypedDict, TypeVar, Union
 
-from opentelemetry import trace as trace_api
+from opentelemetry import context, trace as trace_api
 from opentelemetry.sdk.resources import Resource
 from opentelemetry.sdk.trace import Event, ReadableSpan
 from opentelemetry.sdk.util.instrumentation import InstrumentationScope
 from opentelemetry.trace.status import Status
 from opentelemetry.util import types as otel_types
 from requests import RequestException, Response
 
@@ -180,7 +181,41 @@
     """
     try:
         from packaging.version import Version
 
     except ImportError:  # pragma: no cover
         from setuptools._vendor.packaging.version import Version
     return Version(version)  # type: ignore
+
+
+# OTEL uses two different keys to supress instrumentation. We need to check both.
+SUPPRESS_INSTRUMENTATION_CONTEXT_KEYS = [
+    # This is still used in some places in OTEL, and probably more in older versions.
+    'suppress_instrumentation',
+]
+
+try:
+    # This is the 'main' key used by OTEL in recent versions
+    SUPPRESS_INSTRUMENTATION_CONTEXT_KEYS.append(context._SUPPRESS_INSTRUMENTATION_KEY)  # type: ignore
+except AttributeError:  # pragma: no cover
+    pass
+
+
+def is_instrumentation_suppressed() -> bool:
+    """Return True if the `suppress_instrumentation` context manager is currently active.
+
+    This means that any logs/spans generated by logfire or OpenTelemetry will not be logged in any way.
+    """
+    return any(context.get_value(key) for key in SUPPRESS_INSTRUMENTATION_CONTEXT_KEYS)
+
+
+@contextmanager
+def suppress_instrumentation():
+    """Context manager to suppress all logs/spans generated by logfire or OpenTelemetry."""
+    new_context = context.get_current()
+    for key in SUPPRESS_INSTRUMENTATION_CONTEXT_KEYS:
+        new_context = context.set_value(key, True, new_context)
+    token = context.attach(new_context)
+    try:
+        yield
+    finally:
+        context.detach(token)
```

### Comparing `logfire-0.36.1/logfire/_internal/auto_trace/__init__.py` & `logfire-0.37.0/logfire/_internal/auto_trace/__init__.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/_internal/auto_trace/import_hook.py` & `logfire-0.37.0/logfire/_internal/auto_trace/import_hook.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/_internal/auto_trace/rewrite_ast.py` & `logfire-0.37.0/logfire/_internal/auto_trace/rewrite_ast.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/_internal/auto_trace/types.py` & `logfire-0.37.0/logfire/_internal/auto_trace/types.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/_internal/exporters/console.py` & `logfire-0.37.0/logfire/_internal/exporters/console.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/_internal/exporters/fallback.py` & `logfire-0.37.0/logfire/_internal/exporters/fallback.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/_internal/exporters/file.py` & `logfire-0.37.0/logfire/_internal/exporters/file.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/_internal/exporters/otlp.py` & `logfire-0.37.0/logfire/_internal/exporters/otlp.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/_internal/exporters/processor_wrapper.py` & `logfire-0.37.0/logfire/_internal/exporters/processor_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     ATTRIBUTES_MESSAGE_KEY,
     ATTRIBUTES_MESSAGE_TEMPLATE_KEY,
     ATTRIBUTES_SPAN_TYPE_KEY,
     PENDING_SPAN_NAME_SUFFIX,
     log_level_attributes,
 )
 from ..scrubbing import Scrubber
-from ..utils import ReadableSpanDict, span_to_dict, truncate_string
+from ..utils import ReadableSpanDict, is_instrumentation_suppressed, span_to_dict, truncate_string
 
 
 class SpanProcessorWrapper(SpanProcessor):
     """Wrapper around other processors to intercept starting and ending spans with our own global logic.
 
     Suppresses starting/ending if the current context has a `suppress_instrumentation` value.
     Tweaks the send/receive span names generated by the ASGI middleware.
@@ -30,21 +30,21 @@
         self.scrubber = scrubber
 
     def on_start(
         self,
         span: Span,
         parent_context: context.Context | None = None,
     ) -> None:
-        if context.get_value('suppress_instrumentation'):  # pragma: no cover
+        if is_instrumentation_suppressed():
             return
         _set_log_level_on_asgi_send_receive_spans(span)
         self.processor.on_start(span, parent_context)
 
     def on_end(self, span: ReadableSpan) -> None:
-        if context.get_value('suppress_instrumentation'):  # pragma: no cover
+        if is_instrumentation_suppressed():
             return
         span_dict = span_to_dict(span)
         _tweak_asgi_send_receive_spans(span_dict)
         _tweak_http_spans(span_dict)
         self.scrubber.scrub_span(span_dict)
         span = ReadableSpan(**span_dict)
         self.processor.on_end(span)
```

### Comparing `logfire-0.36.1/logfire/_internal/exporters/remove_pending.py` & `logfire-0.37.0/logfire/_internal/exporters/remove_pending.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/_internal/exporters/wrapper.py` & `logfire-0.37.0/logfire/_internal/exporters/wrapper.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/_internal/integrations/executors.py` & `logfire-0.37.0/logfire/_internal/integrations/executors.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/_internal/integrations/fastapi.py` & `logfire-0.37.0/logfire/_internal/integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/_internal/integrations/psycopg.py` & `logfire-0.37.0/logfire/_internal/integrations/psycopg.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/_internal/integrations/llm_providers/anthropic.py` & `logfire-0.37.0/logfire/_internal/integrations/llm_providers/anthropic.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/_internal/integrations/llm_providers/llm_provider.py` & `logfire-0.37.0/logfire/_internal/integrations/llm_providers/llm_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from __future__ import annotations
 
 from collections.abc import Iterable
 from contextlib import ExitStack, contextmanager, nullcontext
 from typing import TYPE_CHECKING, Any, AsyncIterator, Callable, ContextManager, Iterator, cast
 
-from opentelemetry import context
-
 from ...constants import ONE_SECOND_IN_NANOSECONDS
+from ...utils import is_instrumentation_suppressed, suppress_instrumentation
 
 if TYPE_CHECKING:
     from ...main import Logfire, LogfireSpan
     from .types import EndpointConfig
 
 
 __all__ = ('instrument_llm_provider',)
@@ -70,15 +69,15 @@
 
     client._is_instrumented_by_logfire = True
     client._original_request_method = original_request_method = client._request
 
     is_async = is_async_client_fn(client if isinstance(client, type) else type(client))
 
     def _instrumentation_setup(**kwargs: Any) -> Any:
-        if context.get_value('suppress_instrumentation'):
+        if is_instrumentation_suppressed():
             return None, None, kwargs
 
         options = kwargs['options']
         try:
             message_template, span_data, content_from_stream = get_endpoint_config_fn(options)
         except ValueError as exc:
             logfire_llm.warn(
@@ -168,20 +167,16 @@
 
     return uninstrument_context()
 
 
 @contextmanager
 def maybe_suppress_instrumentation(suppress: bool) -> Iterator[None]:
     if suppress:
-        new_context = context.set_value('suppress_instrumentation', True)
-        token = context.attach(new_context)
-        try:
+        with suppress_instrumentation():
             yield
-        finally:
-            context.detach(token)
     else:
         yield
 
 
 @contextmanager
 def record_streaming(
     logire_llm: Logfire,
```

### Comparing `logfire-0.36.1/logfire/_internal/integrations/llm_providers/openai.py` & `logfire-0.37.0/logfire/_internal/integrations/llm_providers/openai.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/integrations/logging.py` & `logfire-0.37.0/logfire/integrations/logging.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Integration with the standard library logging module."""
 
 from __future__ import annotations
 
-import inspect
 from logging import NOTSET, Handler as LoggingHandler, LogRecord, StreamHandler
 from typing import Any, ClassVar, Mapping, cast
 
 import logfire
 
 from .._internal.constants import (
     ATTRIBUTES_LOGGING_ARGS_KEY,
     ATTRIBUTES_MESSAGE_KEY,
     ATTRIBUTES_MESSAGE_TEMPLATE_KEY,
     LOGGING_TO_OTEL_LEVEL_NUMBERS,
 )
+from .._internal.utils import is_instrumentation_suppressed
 
 # skip natural LogRecord attributes
 # http://docs.python.org/library/logging.html#logrecord-attributes
 RESERVED_ATTRS: frozenset[str] = frozenset(
     [
         'args',
         'asctime',
@@ -57,28 +57,17 @@
 
     def emit(self, record: LogRecord) -> None:
         """Send the log to Logfire.
 
         Args:
             record: The log record to send.
         """
-        if record.name.startswith('opentelemetry.'):
-            # This method can lead to OTEL calling logging methods which recursively calls this again.
-            # If we detect recursion, use the fallback handler instead.
-            # TODO find a better way to handle this,
-            #  or document the fallback clearly and nudge the user to configure it.
-            frame = inspect.currentframe()
-            assert frame is not None
-            code_here = frame.f_code
-            frame = frame.f_back
-            while frame:
-                if frame.f_code is code_here:
-                    self.fallback.emit(record)
-                    return
-                frame = frame.f_back
+        if is_instrumentation_suppressed():
+            self.fallback.handle(record)
+            return
 
         attributes = self.fill_attributes(record)
 
         logfire.log(
             msg_template=attributes.pop(ATTRIBUTES_MESSAGE_TEMPLATE_KEY, record.msg),
             level=LOGGING_TO_OTEL_LEVEL_NUMBERS.get(record.levelno, record.levelno),
             attributes=attributes,
```

### Comparing `logfire-0.36.1/logfire/integrations/loguru.py` & `logfire-0.37.0/logfire/integrations/loguru.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/integrations/pydantic.py` & `logfire-0.37.0/logfire/integrations/pydantic.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/logfire/integrations/structlog.py` & `logfire-0.37.0/logfire/integrations/structlog.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/conftest.py` & `logfire-0.37.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/test_auto_trace.py` & `logfire-0.37.0/tests/test_auto_trace.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/test_backfill.py` & `logfire-0.37.0/tests/test_backfill.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/test_cli.py` & `logfire-0.37.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/test_collect_package_resources.py` & `logfire-0.37.0/tests/test_collect_package_resources.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/test_configure.py` & `logfire-0.37.0/tests/test_configure.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/test_console_exporter.py` & `logfire-0.37.0/tests/test_console_exporter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/test_formatter.py` & `logfire-0.37.0/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/test_json_args.py` & `logfire-0.37.0/tests/test_json_args.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/test_json_args_formatting.py` & `logfire-0.37.0/tests/test_json_args_formatting.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/test_logfire.py` & `logfire-0.37.0/tests/test_logfire.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,25 +16,26 @@
 from opentelemetry.sdk.metrics.export import InMemoryMetricReader
 from opentelemetry.sdk.trace import ReadableSpan
 from opentelemetry.sdk.trace.export import SimpleSpanProcessor
 from pydantic import BaseModel
 from pydantic_core import ValidationError
 
 import logfire
-from logfire import Logfire
+from logfire import Logfire, suppress_instrumentation
 from logfire._internal.config import LogfireConfig, configure
 from logfire._internal.constants import (
     ATTRIBUTES_MESSAGE_KEY,
     ATTRIBUTES_MESSAGE_TEMPLATE_KEY,
     ATTRIBUTES_SPAN_TYPE_KEY,
     ATTRIBUTES_TAGS_KEY,
     LEVEL_NUMBERS,
     NULL_ARGS_KEY,
 )
 from logfire._internal.formatter import InspectArgumentsFailedWarning
+from logfire._internal.utils import is_instrumentation_suppressed
 from logfire.integrations.logging import LogfireLoggingHandler
 from logfire.testing import IncrementalIdGenerator, TestExporter, TimeGenerator
 
 
 @pytest.mark.parametrize('method', ['trace', 'info', 'debug', 'warn', 'error', 'fatal'])
 def test_log_methods_without_kwargs(method: str):
     with pytest.warns(UserWarning, match="The field 'foo' is not defined.") as warnings:
@@ -2450,7 +2451,55 @@
                     'code.lineno': 123,
                     'name': 'me',
                     'logfire.json_schema': '{"type":"object","properties":{"name":{}}}',
                 },
             }
         ]
     )
+
+
+def test_suppress_instrumentation(exporter: TestExporter):
+    logfire.info('log1')
+    assert not is_instrumentation_suppressed()
+    with suppress_instrumentation():
+        assert is_instrumentation_suppressed()
+        # Not included in the asserted spans below
+        logfire.info('log2')
+    assert not is_instrumentation_suppressed()
+    logfire.info('log3')
+
+    assert exporter.exported_spans_as_dict() == snapshot(
+        [
+            {
+                'name': 'log1',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 1000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': 'log1',
+                    'logfire.msg': 'log1',
+                    'code.filepath': 'test_logfire.py',
+                    'code.function': 'test_suppress_instrumentation',
+                    'code.lineno': 123,
+                },
+            },
+            {
+                'name': 'log3',
+                'context': {'trace_id': 3, 'span_id': 3, 'is_remote': False},
+                'parent': None,
+                'start_time': 3000000000,
+                'end_time': 3000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 9,
+                    'logfire.msg_template': 'log3',
+                    'logfire.msg': 'log3',
+                    'code.filepath': 'test_logfire.py',
+                    'code.function': 'test_suppress_instrumentation',
+                    'code.lineno': 123,
+                },
+            },
+        ]
+    )
```

### Comparing `logfire-0.36.1/tests/test_loguru.py` & `logfire-0.37.0/tests/test_loguru.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/test_metrics.py` & `logfire-0.37.0/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/test_no_production.py` & `logfire-0.37.0/tests/test_no_production.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/test_pydantic_plugin.py` & `logfire-0.37.0/tests/test_pydantic_plugin.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/test_sampling.py` & `logfire-0.37.0/tests/test_sampling.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/test_secret_scrubbing.py` & `logfire-0.37.0/tests/test_secret_scrubbing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/test_slow_async_callbacks.py` & `logfire-0.37.0/tests/test_slow_async_callbacks.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/test_source_code_extraction.py` & `logfire-0.37.0/tests/test_source_code_extraction.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/test_stdlib_logging.py` & `logfire-0.37.0/tests/test_stdlib_logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,17 +208,18 @@
     logger = getLogger()
     test_logging_handler = TestLoggingHandler()
     logfire_logging_handler = LogfireLoggingHandler(fallback=test_logging_handler)
     logger.addHandler(logfire_logging_handler)
 
     try:
         # This calls ExceptionExporter.export which causes OTEL to log an exception.
-        # That log call goes to LogfireLoggingHandler.emit, which tries to emit another logfire log,
+        # That log call goes to LogfireLoggingHandler.emit, which usually tries to emit another logfire log,
         # causing another stdlib log from OTEL, potentially leading to infinite recursion.
-        # This tests that we handle that by using the fallback test_logging_handler when recursion is detected.
+        # Recursion is prevented by OTEL suppressing instrumentation, so the second logfire log isn't emitted.
+        # But when we detect this, we use the fallback handler instead, so this tests that.
         logfire.info('test')
     finally:
         # Don't mess with the root logger longer than needed.
         logger.removeHandler(logfire_logging_handler)
 
     [record] = test_logging_handler.logs
     # This is the message logged by OTEL.
```

### Comparing `logfire-0.36.1/tests/test_structlog.py` & `logfire-0.37.0/tests/test_structlog.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/test_testing.py` & `logfire-0.37.0/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/test_utils.py` & `logfire-0.37.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/utils.py` & `logfire-0.37.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/exporters/test_fallback_exporter.py` & `logfire-0.37.0/tests/exporters/test_fallback_exporter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/exporters/test_file_exporter.py` & `logfire-0.37.0/tests/exporters/test_file_exporter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/exporters/test_otlp_session.py` & `logfire-0.37.0/tests/exporters/test_otlp_session.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/exporters/test_remove_pending.py` & `logfire-0.37.0/tests/exporters/test_remove_pending.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/exporters/test_retry_fewer_spans.py` & `logfire-0.37.0/tests/exporters/test_retry_fewer_spans.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/import_used_for_tests/slow_async_callbacks_example.py` & `logfire-0.37.0/tests/import_used_for_tests/slow_async_callbacks_example.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/otel_integrations/test_anthropic.py` & `logfire-0.37.0/tests/otel_integrations/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/otel_integrations/test_asgi.py` & `logfire-0.37.0/tests/otel_integrations/test_asgi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/otel_integrations/test_asyncpg.py` & `logfire-0.37.0/tests/otel_integrations/test_asyncpg.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/otel_integrations/test_django.py` & `logfire-0.37.0/tests/otel_integrations/test_django.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/otel_integrations/test_fastapi.py` & `logfire-0.37.0/tests/otel_integrations/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/otel_integrations/test_flask.py` & `logfire-0.37.0/tests/otel_integrations/test_flask.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/otel_integrations/test_httpx.py` & `logfire-0.37.0/tests/otel_integrations/test_httpx.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/otel_integrations/test_openai.py` & `logfire-0.37.0/tests/otel_integrations/test_openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,19 +19,19 @@
     create_embedding_response,
     embedding,
     file_object,
     image,
     images_response,
 )
 from openai.types.chat import chat_completion, chat_completion_chunk as cc_chunk, chat_completion_message
-from opentelemetry import context
 from opentelemetry.instrumentation.httpx import HTTPXClientInstrumentor
 
 import logfire
 from logfire._internal.integrations.llm_providers.openai import get_endpoint_config
+from logfire._internal.utils import suppress_instrumentation
 from logfire.testing import TestExporter
 
 
 def request_handler(request: httpx.Request) -> httpx.Response:
     """Used to mock httpx requests
 
     We do this instead of using pytest-httpx since 1) it's nearly as simple 2) pytest-httpx doesn't support Python 3.8.
@@ -841,33 +841,23 @@
                 },
             },
         ]
     )
 
 
 def test_openai_suppressed(instrumented_client: openai.Client, exporter: TestExporter) -> None:
-    new_context = context.set_value('suppress_instrumentation', True)
-    token = context.attach(new_context)
-    try:
+    with suppress_instrumentation():
         response = instrumented_client.completions.create(model='gpt-3.5-turbo-instruct', prompt='xxx')
-    finally:
-        context.detach(token)
-
     assert response.choices[0].text == 'Nine'
     assert exporter.exported_spans_as_dict() == []
 
 
 async def test_async_openai_suppressed(instrumented_async_client: openai.AsyncClient, exporter: TestExporter) -> None:
-    new_context = context.set_value('suppress_instrumentation', True)
-    token = context.attach(new_context)
-    try:
+    with suppress_instrumentation():
         response = await instrumented_async_client.completions.create(model='gpt-3.5-turbo-instruct', prompt='xxx')
-    finally:
-        context.detach(token)
-
     assert response.choices[0].text == 'Nine'
     assert exporter.exported_spans_as_dict() == []
 
 
 def test_unknown_method(instrumented_client: openai.Client, exporter: TestExporter) -> None:
     response = instrumented_client.files.create(file=BytesIO(b'file contents'), purpose='fine-tune')
     assert response.filename == 'test.txt'
```

### Comparing `logfire-0.36.1/tests/otel_integrations/test_psycopg.py` & `logfire-0.37.0/tests/otel_integrations/test_psycopg.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/otel_integrations/test_requests.py` & `logfire-0.37.0/tests/otel_integrations/test_requests.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/otel_integrations/test_sqlalchemy.py` & `logfire-0.37.0/tests/otel_integrations/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/otel_integrations/test_starlette.py` & `logfire-0.37.0/tests/otel_integrations/test_starlette.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/otel_integrations/test_wsgi.py` & `logfire-0.37.0/tests/otel_integrations/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/otel_integrations/django_test_project/manage.py` & `logfire-0.37.0/tests/otel_integrations/django_test_project/manage.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/tests/otel_integrations/django_test_project/django_test_site/settings.py` & `logfire-0.37.0/tests/otel_integrations/django_test_project/django_test_site/settings.py`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/LICENSE` & `logfire-0.37.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/README.md` & `logfire-0.37.0/README.md`

 * *Files identical despite different names*

### Comparing `logfire-0.36.1/pyproject.toml` & `logfire-0.37.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "logfire"
-version = "0.36.1"
+version = "0.37.0"
 description = "The best Python observability tool! 🪵🔥"
 authors = [
     { name = "Pydantic Team", email = "engineering@pydantic.dev" },
     { name = "Samuel Colvin", email = "samuel@pydantic.dev" },
     { name = "Hasan Ramezani", email = "hasan@pydantic.dev" },
     { name = "Adrian Garcia Badaracco", email = "adrian@pydantic.dev" },
     { name = "David Montague", email = "david@pydantic.dev" },
```

### Comparing `logfire-0.36.1/PKG-INFO` & `logfire-0.37.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: logfire
-Version: 0.36.1
+Version: 0.37.0
 Summary: The best Python observability tool! 🪵🔥
 Author-email: Pydantic Team <engineering@pydantic.dev>, Samuel Colvin <samuel@pydantic.dev>, Hasan Ramezani <hasan@pydantic.dev>, Adrian Garcia Badaracco <adrian@pydantic.dev>, David Montague <david@pydantic.dev>, Marcelo Trylesinski <marcelo@pydantic.dev>, David Hewitt <david.hewitt@pydantic.dev>, Alex Hall <alex@pydantic.dev>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
```

