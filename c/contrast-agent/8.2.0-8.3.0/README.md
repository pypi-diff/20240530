# Comparing `tmp/contrast_agent-8.2.0.tar.gz` & `tmp/contrast_agent-8.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contrast_agent-8.2.0.tar", last modified: Mon May 20 15:41:07 2024, max compression
+gzip compressed data, was "contrast_agent-8.3.0.tar", last modified: Thu May 30 14:05:43 2024, max compression
```

## Comparing `contrast_agent-8.2.0.tar` & `contrast_agent-8.3.0.tar`

### file list

```diff
@@ -1,788 +1,788 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.623546 contrast_agent-8.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-20 15:41:07.623546 contrast_agent-8.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.495546 contrast_agent-8.2.0/hookspy/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/hookspy/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/hookspy/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.495546 contrast_agent-8.2.0/hookspy/ext/
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/hookspy/ext/hookspy.c
--rwxr-xr-x   0 runner    (1001) docker     (127)      952 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/hookspy/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.479546 contrast_agent-8.2.0/hookspy/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.495546 contrast_agent-8.2.0/hookspy/src/hookspy/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/hookspy/src/hookspy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/hookspy/src/hookspy/autogen.py
--rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/hookspy/src/hookspy/body.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/hookspy/src/hookspy/signatures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/hookspy/src/hookspy/spy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 15:41:07.623546 contrast_agent-8.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.491546 contrast_agent-8.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.495546 contrast_agent-8.2.0/src/contrast/
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.499546 contrast_agent-8.2.0/src/contrast/agent/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.503546 contrast_agent-8.2.0/src/contrast/agent/agent_lib/
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/agent_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13355 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/agent_lib/input_tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/agent_lib/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/agent_lib/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    16054 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/agent_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    10536 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/asgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.503546 contrast_agent-8.2.0/src/contrast/agent/assess/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/adjusted_span.py
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/apply_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/assess_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    18900 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/contrast_event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.507546 contrast_agent-8.2.0/src/contrast/agent/assess/policy/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/deadzone_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     6901 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/patches.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/preshift.py
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagation_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagation_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.511546 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/append_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/base_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/center_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/codecs_splat_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/db_write_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/encode_html_splat_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/format_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/join_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/json_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/keep_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/prepend_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/reductive_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/regex_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/replace_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/repr_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator_django.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/slice_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/splat_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/split_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/starlette_safe_path_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/stream_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/tagger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/source_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    14175 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/source_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11245 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/string_propagation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.511546 contrast_agent-8.2.0/src/contrast/agent/assess/policy/trigger_actions/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/trigger_actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/trigger_actions/default_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/trigger_actions/fromstring_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/trigger_actions/openai_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/trigger_actions/redos_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/trigger_actions/ssrf_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/trigger_actions/subprocess_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/trigger_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/preflight.py
--rw-r--r--   0 runner    (1001) docker     (127)    14431 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/properties.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.511546 contrast_agent-8.2.0/src/contrast/agent/assess/rules/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/base_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.515546 contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/base_config_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/base_django_config_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/base_flask_config_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/django_httponly_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/django_secure_flag_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/django_session_age_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/falcon_secure_flag_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/flask_httponly_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/flask_secure_flag_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/flask_session_age_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/httponly_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/secure_flag_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/session_age_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/dataflow_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/non_dataflow_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.515546 contrast_agent-8.2.0/src/contrast/agent/assess/rules/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/providers/code_parser_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/providers/enable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/providers/hardcoded_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/providers/hardcoded_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/providers/hardcoded_value_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.519546 contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/analyze.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/autocomplete_missing_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/base_body_only_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/base_header_only_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/base_response_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/cache_controls_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/clickjacking_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9007 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/csp_header_insecure_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/csp_header_missing_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/hsts_header_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/parameter_pollution_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/x_content_type_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/x_xss_protection_disabled_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/xss.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/static_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/trigger_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.519546 contrast_agent-8.2.0/src/contrast/agent/assess/rules/triggers/
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/triggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/triggers/httponly_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/triggers/secure_flag_missing_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/triggers/session_rewriting_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/triggers/session_timeout_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/triggers/trigger_config_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/string_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/truncate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/disable_reaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/exclusions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/heartbeat_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.523546 contrast_agent-8.2.0/src/contrast/agent/middlewares/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/middlewares/app_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)    14326 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/middlewares/base_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/middlewares/environ_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.523546 contrast_agent-8.2.0/src/contrast/agent/middlewares/response_wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/middlewares/response_wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/middlewares/response_wrappers/aiohttp_response_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/middlewares/response_wrappers/base_response_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.523546 contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/aiohttp_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/bottle_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/django_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/falcon_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/flask_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/pyramid_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/routes_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/starlette_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/patch_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.527546 contrast_agent-8.2.0/src/contrast/agent/policy/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/policy/applicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/policy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/policy/patch_location_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9673 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/policy/patch_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/policy/policy_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/policy/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/policy/rewriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/policy/trigger_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/policy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.527546 contrast_agent-8.2.0/src/contrast/agent/protect/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12667 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/input_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.527546 contrast_agent-8.2.0/src/contrast/agent/protect/policy/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.527546 contrast_agent-8.2.0/src/contrast/agent/protect/rule/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13381 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/base_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/bot_blocker_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/cmdi_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.531546 contrast_agent-8.2.0/src/contrast/agent/protect/rule/deserialization/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/deserialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/deserialization/custom_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/deserialization/pickle_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/deserialization/yaml_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/deserialization_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/http_method_tampering.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/malformed_header.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/mode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.531546 contrast_agent-8.2.0/src/contrast/agent/protect/rule/nosql_injection/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/nosql_injection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12710 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/nosql_injection/mongo_nosql_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/nosqli_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/path_traversal_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/rules_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/sqli_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/ssrf_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/unsafe_file_upload_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/xss_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.531546 contrast_agent-8.2.0/src/contrast/agent/protect/rule/xxe/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/xxe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/xxe/entity_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/xxe_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/reaction_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/request_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/request_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/server_settings_poll.py
--rw-r--r--   0 runner    (1001) docker     (127)    24894 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/sys_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)    12551 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/thread_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.531546 contrast_agent-8.2.0/src/contrast/aiohttp/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/aiohttp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/aiohttp/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/aiohttp/sources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.531546 contrast_agent-8.2.0/src/contrast/api/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/api/architecture_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/api/attack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/api/finding.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/api/library.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/api/route_coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/api/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/api/trace_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/api/type_checked_property.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/api/user_input.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.531546 contrast_agent-8.2.0/src/contrast/applies/
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/applies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.535546 contrast_agent-8.2.0/src/contrast/applies/assess/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/applies/assess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/applies/assess/unsafe_code_execution.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.535546 contrast_agent-8.2.0/src/contrast/applies/common/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/applies/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.535546 contrast_agent-8.2.0/src/contrast/applies/protect/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/applies/protect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/applies/sqli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.535546 contrast_agent-8.2.0/src/contrast/asgi/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/asgi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/asgi/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.535546 contrast_agent-8.2.0/src/contrast/assess_extensions/
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      167 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/build_funchook.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.535546 contrast_agent-8.2.0/src/contrast/assess_extensions/common/
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/common/cast.c
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/common/format.c
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/common/intern.c
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/common/logging.c
--rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/common/patches.c
--rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/common/propagate.c
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/common/repeat.c
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/common/repr.c
--rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/common/scope.c
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/common/streams.c
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/common/subscript.c
--rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/common/trace.c
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/cs_str.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.539546 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/.git
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/.gitmodules
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.539546 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/.travis/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/.travis/Dockerfile-alpine-test
--rwxr-xr-x   0 runner    (1001) docker     (127)      201 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/.travis/run-test.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)    19118 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/appveyor.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)       34 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/autogen.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)    44826 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/config.guess
--rwxr-xr-x   0 runner    (1001) docker     (127)    35454 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/config.sub
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/configure.ac
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.543546 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/.git
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/MANIFEST
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.543546 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/include/
--rw-r--r--   0 runner    (1001) docker     (127)    19536 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/include/distorm.h
--rw-r--r--   0 runner    (1001) docker     (127)    22674 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/include/mnemonics.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.483546 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/make/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.543546 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/make/linux/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/make/linux/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.543546 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/make/mac/
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/make/mac/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.543546 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/make/win32/
--rw-r--r--   0 runner    (1001) docker     (127)    12995 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj.filters
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/make/win32/distorm.sln
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/make/win32/resource.h
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/make/win32/resource.rc
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.547546 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/
--rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/config.h
--rw-r--r--   0 runner    (1001) docker     (127)    25059 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.c
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)    13127 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/distorm.c
--rw-r--r--   0 runner    (1001) docker     (127)    24718 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.c
--rw-r--r--   0 runner    (1001) docker     (127)    17569 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.h
--rw-r--r--   0 runner    (1001) docker     (127)   209309 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/insts.c
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/insts.h
--rw-r--r--   0 runner    (1001) docker     (127)    24295 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/mnemonics.c
--rw-r--r--   0 runner    (1001) docker     (127)    45685 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/operands.c
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/operands.h
--rw-r--r--   0 runner    (1001) docker     (127)    12423 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.c
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.h
--rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.c
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.h
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.c
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.h
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/x86defs.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.547546 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/include/
--rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/include/funchook.h
--rwxr-xr-x   0 runner    (1001) docker     (127)    13998 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/install-sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.551546 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/__strerror.h
--rw-r--r--   0 runner    (1001) docker     (127)    13592 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/funchook.c
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/funchook_internal.h
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/funchook_io.c
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/funchook_io.h
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/funchook_syscall.S
--rw-r--r--   0 runner    (1001) docker     (127)    16239 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/funchook_unix.c
--rw-r--r--   0 runner    (1001) docker     (127)    14804 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/funchook_windows.c
--rw-r--r--   0 runner    (1001) docker     (127)    20159 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/funchook_x86.c
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/os_func.c
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/os_func.h
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/os_func_unix.c
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/os_func_windows.c
--rw-r--r--   0 runner    (1001) docker     (127)    43872 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/printf_base.c
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/printf_base.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.551546 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/test/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/test/libfunchook_test.c
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/test/libfunchook_test2.c
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/test/suffix.list
--rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/test/test_main.c
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/test/x86_64_test.S
--rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/test/x86_test.S
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.555546 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/win32/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/win32/config.h
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/win32/funchook.sln
--rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj.filters
--rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj.filters
--rw-r--r--   0 runner    (1001) docker     (127)     8909 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj.filters
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/win32/funchook_test_exe.def
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.487546 contrast_agent-8.2.0/src/contrast/assess_extensions/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.487546 contrast_agent-8.2.0/src/contrast/assess_extensions/include/contrast/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.555546 contrast_agent-8.2.0/src/contrast/assess_extensions/include/contrast/assess/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/include/contrast/assess/intern.h
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/include/contrast/assess/logging.h
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/include/contrast/assess/patches.h
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/include/contrast/assess/propagate.h
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/include/contrast/assess/scope.h
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/include/contrast/assess/trace.h
--rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/include/contrast/assess/utils.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.555546 contrast_agent-8.2.0/src/contrast/assess_extensions/py3/
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py3/patches.c
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py3/str_concat.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.555546 contrast_agent-8.2.0/src/contrast/assess_extensions/py310/
--rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py310/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py310/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py310/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py310/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py310/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py310/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.559546 contrast_agent-8.2.0/src/contrast/assess_extensions/py311/
--rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py311/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py311/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py311/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py311/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py311/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py311/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.559546 contrast_agent-8.2.0/src/contrast/assess_extensions/py312/
--rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py312/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py312/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py312/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py312/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py312/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py312/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.559546 contrast_agent-8.2.0/src/contrast/assess_extensions/py35/
--rw-r--r--   0 runner    (1001) docker     (127)     8273 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py35/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py35/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py35/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py35/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py35/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py35/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.559546 contrast_agent-8.2.0/src/contrast/assess_extensions/py36/
--rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py36/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py36/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py36/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py36/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py36/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py36/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.563546 contrast_agent-8.2.0/src/contrast/assess_extensions/py37/
--rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py37/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py37/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py37/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py37/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py37/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py37/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.563546 contrast_agent-8.2.0/src/contrast/assess_extensions/py38/
--rw-r--r--   0 runner    (1001) docker     (127)    10485 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py38/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)     9589 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py38/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py38/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py38/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py38/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py38/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.563546 contrast_agent-8.2.0/src/contrast/assess_extensions/py39/
--rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py39/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py39/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py39/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py39/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py39/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py39/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.563546 contrast_agent-8.2.0/src/contrast/bottle/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/bottle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/bottle/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.567546 contrast_agent-8.2.0/src/contrast/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/configuration/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/configuration/agent_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/configuration/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/configuration/application.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/configuration/assess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/configuration/config_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/configuration/config_option.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/configuration/inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/configuration/protect.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/configuration/root.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/configuration/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.567546 contrast_agent-8.2.0/src/contrast/django/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/django/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.567546 contrast_agent-8.2.0/src/contrast/django_asgi/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/django_asgi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/django_asgi/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.567546 contrast_agent-8.2.0/src/contrast/falcon/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/falcon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/falcon/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.567546 contrast_agent-8.2.0/src/contrast/falcon_asgi/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/falcon_asgi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/falcon_asgi/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.567546 contrast_agent-8.2.0/src/contrast/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/fastapi/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.567546 contrast_agent-8.2.0/src/contrast/flask/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/flask/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.567546 contrast_agent-8.2.0/src/contrast/loader/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/loader/sitecustomize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.571546 contrast_agent-8.2.0/src/contrast/patches/
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/cgi_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/concurrent_futures_thread_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/cs_io.py
--rw-r--r--   0 runner    (1001) docker     (127)    10868 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/cs_str.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.575546 contrast_agent-8.2.0/src/contrast/patches/databases/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8638 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/databases/dbapi2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/databases/mysql_connector_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/databases/psycopg2_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/databases/pymysql_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/databases/sqlalchemy_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/databases/sqlite3_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/encodings_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7791 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/exec_and_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.575546 contrast_agent-8.2.0/src/contrast/patches/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/frameworks/bottle_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/frameworks/django_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/frameworks/drf_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/frameworks/falcon_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/frameworks/flask_and_quart_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     6213 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/frameworks/pyramid_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/frameworks/starlette_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/genshi_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     9370 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/import_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/lxml_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.575546 contrast_agent-8.2.0/src/contrast/patches/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/middleware/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/middleware/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6613 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/middleware/django.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/middleware/mod_wsgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/pathlib_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/re_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/str_new.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/sys_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/threading_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/urllib_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.575546 contrast_agent-8.2.0/src/contrast/policy/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/deadzones.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.579546 contrast_agent-8.2.0/src/contrast/policy/propagators/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/propagators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/propagators/codecs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/propagators/encodings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/propagators/frameworks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/propagators/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/propagators/re.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/propagators/serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/propagators/string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.579546 contrast_agent-8.2.0/src/contrast/policy/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/sources/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/sources/cgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/sources/django.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/sources/falcon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/sources/flask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/sources/quart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/sources/webob.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.583546 contrast_agent-8.2.0/src/contrast/policy/triggers/
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/cmd_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/httponly.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/nosql_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/path_traversal.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/prompt_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/redos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/reflected_xss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/secure_flag_missing.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/session_rewriting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/session_timeout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/sql_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/ssrf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/trust_boundary_violation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/unsafe_code_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/untrusted_deserialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/unvalidated_redirect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/xpath_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/xxe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.583546 contrast_agent-8.2.0/src/contrast/pyramid/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/pyramid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/pyramid/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.583546 contrast_agent-8.2.0/src/contrast/quart/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/quart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/quart/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.583546 contrast_agent-8.2.0/src/contrast/reporting/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/activity_masker.py
--rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/reporting_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/request_audit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.587546 contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/_traces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/agent_startup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/application_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/application_inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/application_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/base_ts_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/effective_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/library_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/observed_route.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/preflight.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/server_activity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.587546 contrast_agent-8.2.0/src/contrast/reporting/teamserver_responses/
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_responses/application_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_responses/ng_application_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_responses/ng_server_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_responses/protect_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_responses/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_responses/server_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.591546 contrast_agent-8.2.0/src/contrast/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/scripts/fix_interpreter_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/scripts/propagator_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/scripts/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/scripts/validate_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.595546 contrast_agent-8.2.0/src/contrast/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.595546 contrast_agent-8.2.0/src/contrast/utils/assess/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/assess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/assess/duck_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.595546 contrast_agent-8.2.0/src/contrast/utils/assess/formatting/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/assess/formatting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/assess/formatting/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/assess/formatting/tokenize_cformat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/assess/formatting/tokenize_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     6671 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/assess/stream_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/assess/tag_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/assess/tracking_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/base64_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/configuration_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/context_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/deprecated_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/digest_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/environ.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.595546 contrast_agent-8.2.0/src/contrast/utils/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/exceptions/deprecation_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/exceptions/wrong_django_middleware_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/exceptions/wsgi_compliance_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/ignored_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.595546 contrast_agent-8.2.0/src/contrast/utils/library_reader/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/library_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/library_reader/library_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/library_reader/patched_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/library_reader/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/locale.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.599546 contrast_agent-8.2.0/src/contrast/utils/loggers/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/loggers/structlog.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/module_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/object_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/patch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/pattern_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/safe_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/stack_trace_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/stdlib_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/string_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-20 15:41:07.000000 contrast_agent-8.2.0/src/contrast/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.599546 contrast_agent-8.2.0/src/contrast/wsgi/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/wsgi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/wsgi/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.623546 contrast_agent-8.2.0/src/contrast_agent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    32206 2024-05-20 15:41:07.000000 contrast_agent-8.2.0/src/contrast_agent.egg-info/SOURCES.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.599546 contrast_agent-8.2.0/src/contrast_rewriter/
--rw-r--r--   0 runner    (1001) docker     (127)    15340 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_rewriter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.599546 contrast_agent-8.2.0/src/contrast_vendor/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/.clang-format
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.599546 contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    34323 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/_adapters.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/_functools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/_itertools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/_text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.599546 contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/compat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/compat/py39.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/diagnose.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.599546 contrast_agent-8.2.0/src/contrast_vendor/isort/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/isort/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/isort/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.603546 contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/all.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/py2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/py27.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/py3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/py310.py
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/py311.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/py312.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/py36.py
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/py37.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/py38.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/py39.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.603546 contrast_agent-8.2.0/src/contrast_vendor/ported_cpython_code/
--rw-r--r--   0 runner    (1001) docker     (127)    12769 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ported_cpython_code/PYTHON_SOFTWARE_FOUNDATION_LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ported_cpython_code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ported_cpython_code/import_functionality.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.491546 contrast_agent-8.2.0/src/contrast_vendor/ruamel/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.611546 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/anchor.py
--rw-r--r--   0 runner    (1001) docker     (127)    37673 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/composer.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/configobjwalker.py
--rw-r--r--   0 runner    (1001) docker     (127)    70392 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/constructor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/cyaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/dumper.py
--rw-r--r--   0 runner    (1001) docker     (127)    67960 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/emitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8807 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     7278 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    59457 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    36019 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    44497 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/representer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15209 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/scalarbool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/scalarfloat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/scalarint.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/scalarstring.py
--rw-r--r--   0 runner    (1001) docker     (127)    87945 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     8231 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.615546 contrast_agent-8.2.0/src/contrast_vendor/structlog/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/LICENSE-APACHE
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/LICENSE-MIT
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13882 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/_frames.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/_greenlets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/_log_levels.py
--rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/_native.py
--rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/contextvars.py
--rw-r--r--   0 runner    (1001) docker     (127)    23428 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    27977 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/processors.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    37555 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/stdlib.py
--rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9206 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/threadlocal.py
--rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/tracebacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/twisted.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/vendor-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.619546 contrast_agent-8.2.0/src/contrast_vendor/webob/
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   210210 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/acceptparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/byterange.py
--rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/cachecontrol.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    32879 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/datetime_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/dec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/etag.py
--rw-r--r--   0 runner    (1001) docker     (127)    38268 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/exc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/license.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13961 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/multidict.py
--rw-r--r--   0 runner    (1001) docker     (127)    59159 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/request.py
--rw-r--r--   0 runner    (1001) docker     (127)    55423 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/static.py
--rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.619546 contrast_agent-8.2.0/src/contrast_vendor/wrapt/
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/wrapt/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/wrapt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/wrapt/__wrapt__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/wrapt/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)    21333 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/wrapt/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    10997 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/wrapt/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/wrapt/patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/wrapt/weakrefs.py
--rw-r--r--   0 runner    (1001) docker     (127)    27137 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/wrapt/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.623546 contrast_agent-8.2.0/src/contrast_vendor/zipp/
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/zipp/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/zipp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.623546 contrast_agent-8.2.0/src/contrast_vendor/zipp/compat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/zipp/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/zipp/compat/py310.py
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/zipp/glob.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.742499 contrast_agent-8.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-30 14:05:43.742499 contrast_agent-8.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.606499 contrast_agent-8.3.0/hookspy/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/hookspy/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/hookspy/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.606499 contrast_agent-8.3.0/hookspy/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/hookspy/ext/hookspy.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)      952 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/hookspy/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.594499 contrast_agent-8.3.0/hookspy/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.610499 contrast_agent-8.3.0/hookspy/src/hookspy/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/hookspy/src/hookspy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/hookspy/src/hookspy/autogen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/hookspy/src/hookspy/body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/hookspy/src/hookspy/signatures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/hookspy/src/hookspy/spy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 14:05:43.742499 contrast_agent-8.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.606499 contrast_agent-8.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.610499 contrast_agent-8.3.0/src/contrast/
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.614499 contrast_agent-8.3.0/src/contrast/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.614499 contrast_agent-8.3.0/src/contrast/agent/agent_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/agent_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13355 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/agent_lib/input_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/agent_lib/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/agent_lib/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16054 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/agent_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10536 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/asgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.618499 contrast_agent-8.3.0/src/contrast/agent/assess/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/adjusted_span.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/apply_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/assess_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18920 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/contrast_event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.618499 contrast_agent-8.3.0/src/contrast/agent/assess/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/deadzone_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6901 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/preshift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagation_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagation_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.622499 contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/append_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/base_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/center_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/codecs_splat_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/db_write_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/encode_html_splat_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/format_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/join_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/json_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/keep_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/prepend_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/reductive_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/regex_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/replace_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/repr_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator_django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/slice_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/splat_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/split_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/starlette_safe_path_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/stream_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/tagger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/source_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14175 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/source_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11245 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/string_propagation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.626499 contrast_agent-8.3.0/src/contrast/agent/assess/policy/trigger_actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/trigger_actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/trigger_actions/default_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/trigger_actions/fromstring_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/trigger_actions/openai_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/trigger_actions/redos_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/trigger_actions/ssrf_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/trigger_actions/subprocess_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/policy/trigger_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/preflight.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14431 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/properties.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.626499 contrast_agent-8.3.0/src/contrast/agent/assess/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/base_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.626499 contrast_agent-8.3.0/src/contrast/agent/assess/rules/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/config/base_config_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/config/base_django_config_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/config/base_flask_config_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/config/django_httponly_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/config/django_secure_flag_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/config/django_session_age_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/config/falcon_secure_flag_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/config/flask_httponly_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/config/flask_secure_flag_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/config/flask_session_age_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/config/httponly_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/config/secure_flag_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/config/session_age_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/dataflow_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/non_dataflow_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.630499 contrast_agent-8.3.0/src/contrast/agent/assess/rules/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/providers/code_parser_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/providers/enable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/providers/hardcoded_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/providers/hardcoded_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/providers/hardcoded_value_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.630499 contrast_agent-8.3.0/src/contrast/agent/assess/rules/response/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/response/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/response/autocomplete_missing_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/response/base_body_only_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/response/base_header_only_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/response/base_response_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/response/cache_controls_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/response/clickjacking_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9007 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/response/csp_header_insecure_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/response/csp_header_missing_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/response/hsts_header_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/response/parameter_pollution_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/response/x_content_type_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/response/x_xss_protection_disabled_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/response/xss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/static_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/trigger_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.634499 contrast_agent-8.3.0/src/contrast/agent/assess/rules/triggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/triggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/triggers/httponly_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/triggers/secure_flag_missing_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/triggers/session_rewriting_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/triggers/session_timeout_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/rules/triggers/trigger_config_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/string_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/truncate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/assess/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/disable_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/exclusions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/heartbeat_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.634499 contrast_agent-8.3.0/src/contrast/agent/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/middlewares/app_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14565 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/middlewares/base_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/middlewares/environ_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.634499 contrast_agent-8.3.0/src/contrast/agent/middlewares/response_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/middlewares/response_wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/middlewares/response_wrappers/aiohttp_response_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/middlewares/response_wrappers/base_response_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.634499 contrast_agent-8.3.0/src/contrast/agent/middlewares/route_coverage/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/middlewares/route_coverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/middlewares/route_coverage/aiohttp_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/middlewares/route_coverage/bottle_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/middlewares/route_coverage/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/middlewares/route_coverage/django_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/middlewares/route_coverage/falcon_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/middlewares/route_coverage/flask_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/middlewares/route_coverage/pyramid_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/middlewares/route_coverage/routes_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/middlewares/route_coverage/starlette_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/patch_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.638499 contrast_agent-8.3.0/src/contrast/agent/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/policy/applicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/policy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/policy/patch_location_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9673 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/policy/patch_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/policy/policy_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/policy/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/policy/rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/policy/trigger_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/policy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.638499 contrast_agent-8.3.0/src/contrast/agent/protect/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/protect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12051 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/protect/input_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.638499 contrast_agent-8.3.0/src/contrast/agent/protect/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/protect/policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.642499 contrast_agent-8.3.0/src/contrast/agent/protect/rule/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/protect/rule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11884 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/protect/rule/base_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/protect/rule/bot_blocker_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/protect/rule/cmdi_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.642499 contrast_agent-8.3.0/src/contrast/agent/protect/rule/deserialization/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/protect/rule/deserialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/protect/rule/deserialization/custom_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/protect/rule/deserialization/pickle_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/protect/rule/deserialization/yaml_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/protect/rule/deserialization_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/protect/rule/http_method_tampering.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/protect/rule/malformed_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/protect/rule/mode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.642499 contrast_agent-8.3.0/src/contrast/agent/protect/rule/nosql_injection/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/protect/rule/nosql_injection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12710 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/protect/rule/nosql_injection/mongo_nosql_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/protect/rule/nosqli_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/protect/rule/path_traversal_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/protect/rule/rules_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/protect/rule/sqli_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/protect/rule/ssrf_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/protect/rule/unsafe_file_upload_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/protect/rule/xss_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.642499 contrast_agent-8.3.0/src/contrast/agent/protect/rule/xxe/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/protect/rule/xxe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/protect/rule/xxe/entity_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/protect/rule/xxe_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/reaction_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/request_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/request_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/server_settings_poll.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25210 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/sys_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12551 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/thread_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/agent/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.642499 contrast_agent-8.3.0/src/contrast/aiohttp/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/aiohttp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6008 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/aiohttp/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/aiohttp/sources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.646499 contrast_agent-8.3.0/src/contrast/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/api/architecture_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/api/attack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/api/finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/api/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/api/route_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/api/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/api/trace_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/api/type_checked_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/api/user_input.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.646499 contrast_agent-8.3.0/src/contrast/applies/
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/applies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.646499 contrast_agent-8.3.0/src/contrast/applies/assess/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/applies/assess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/applies/assess/unsafe_code_execution.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.646499 contrast_agent-8.3.0/src/contrast/applies/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/applies/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.646499 contrast_agent-8.3.0/src/contrast/applies/protect/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/applies/protect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/applies/sqli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.646499 contrast_agent-8.3.0/src/contrast/asgi/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/asgi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/asgi/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.646499 contrast_agent-8.3.0/src/contrast/assess_extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      167 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/build_funchook.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.650499 contrast_agent-8.3.0/src/contrast/assess_extensions/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/common/cast.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/common/format.c
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/common/intern.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/common/logging.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/common/patches.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/common/propagate.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/common/repeat.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/common/repr.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/common/scope.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/common/streams.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/common/subscript.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/common/trace.c
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/cs_str.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.650499 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-30 14:05:33.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/.git
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/.gitmodules
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.650499 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/.travis/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/.travis/Dockerfile-alpine-test
+-rwxr-xr-x   0 runner    (1001) docker     (127)      201 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/.travis/run-test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    19118 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/appveyor.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)       34 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/autogen.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)    44826 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/config.guess
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35454 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/config.sub
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/configure.ac
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.654499 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-30 14:05:35.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/.git
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-30 14:05:35.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-30 14:05:35.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/MANIFEST
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-30 14:05:35.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-30 14:05:35.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.654499 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/include/
+-rw-r--r--   0 runner    (1001) docker     (127)    19536 2024-05-30 14:05:35.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/include/distorm.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22674 2024-05-30 14:05:35.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/include/mnemonics.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.598499 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/make/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.654499 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/make/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-30 14:05:35.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/make/linux/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.654499 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/make/mac/
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-30 14:05:35.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/make/mac/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.654499 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/make/win32/
+-rw-r--r--   0 runner    (1001) docker     (127)    12995 2024-05-30 14:05:35.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-30 14:05:35.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj.filters
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-30 14:05:35.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/make/win32/distorm.sln
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-30 14:05:35.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/make/win32/resource.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-30 14:05:35.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/make/win32/resource.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-30 14:05:35.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-30 14:05:35.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.658499 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-05-30 14:05:35.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/config.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25059 2024-05-30 14:05:35.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-30 14:05:35.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13127 2024-05-30 14:05:35.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/distorm.c
+-rw-r--r--   0 runner    (1001) docker     (127)    24718 2024-05-30 14:05:35.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.c
+-rw-r--r--   0 runner    (1001) docker     (127)    17569 2024-05-30 14:05:35.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.h
+-rw-r--r--   0 runner    (1001) docker     (127)   209309 2024-05-30 14:05:35.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/insts.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-30 14:05:35.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/insts.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24295 2024-05-30 14:05:35.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/mnemonics.c
+-rw-r--r--   0 runner    (1001) docker     (127)    45685 2024-05-30 14:05:35.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/operands.c
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-30 14:05:35.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/operands.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12423 2024-05-30 14:05:35.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-30 14:05:35.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-05-30 14:05:35.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-30 14:05:35.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.h
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-30 14:05:35.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-30 14:05:35.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-30 14:05:35.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/x86defs.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.658499 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/include/
+-rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/include/funchook.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13998 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/install-sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.662499 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/src/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/src/__strerror.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13592 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/src/funchook.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/src/funchook_internal.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/src/funchook_io.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/src/funchook_io.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/src/funchook_syscall.S
+-rw-r--r--   0 runner    (1001) docker     (127)    16239 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/src/funchook_unix.c
+-rw-r--r--   0 runner    (1001) docker     (127)    14804 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/src/funchook_windows.c
+-rw-r--r--   0 runner    (1001) docker     (127)    20159 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/src/funchook_x86.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/src/os_func.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/src/os_func.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/src/os_func_unix.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/src/os_func_windows.c
+-rw-r--r--   0 runner    (1001) docker     (127)    43872 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/src/printf_base.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/src/printf_base.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.662499 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/test/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/test/libfunchook_test.c
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/test/libfunchook_test2.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/test/suffix.list
+-rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/test/test_main.c
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/test/x86_64_test.S
+-rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/test/x86_test.S
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.666499 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/win32/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/win32/config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/win32/funchook.sln
+-rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj.filters
+-rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj.filters
+-rw-r--r--   0 runner    (1001) docker     (127)     8909 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj.filters
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-30 14:05:34.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/win32/funchook_test_exe.def
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.598499 contrast_agent-8.3.0/src/contrast/assess_extensions/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.598499 contrast_agent-8.3.0/src/contrast/assess_extensions/include/contrast/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.666499 contrast_agent-8.3.0/src/contrast/assess_extensions/include/contrast/assess/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/include/contrast/assess/intern.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/include/contrast/assess/logging.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/include/contrast/assess/patches.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/include/contrast/assess/propagate.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/include/contrast/assess/scope.h
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/include/contrast/assess/trace.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/include/contrast/assess/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.666499 contrast_agent-8.3.0/src/contrast/assess_extensions/py3/
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py3/patches.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py3/str_concat.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.666499 contrast_agent-8.3.0/src/contrast/assess_extensions/py310/
+-rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py310/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py310/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py310/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py310/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py310/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py310/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.670499 contrast_agent-8.3.0/src/contrast/assess_extensions/py311/
+-rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py311/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py311/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py311/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py311/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py311/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py311/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.670499 contrast_agent-8.3.0/src/contrast/assess_extensions/py312/
+-rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py312/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py312/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py312/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py312/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py312/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py312/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.670499 contrast_agent-8.3.0/src/contrast/assess_extensions/py35/
+-rw-r--r--   0 runner    (1001) docker     (127)     8273 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py35/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py35/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py35/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py35/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py35/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py35/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.674499 contrast_agent-8.3.0/src/contrast/assess_extensions/py36/
+-rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py36/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py36/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py36/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py36/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py36/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py36/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.674499 contrast_agent-8.3.0/src/contrast/assess_extensions/py37/
+-rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py37/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py37/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py37/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py37/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py37/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py37/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.674499 contrast_agent-8.3.0/src/contrast/assess_extensions/py38/
+-rw-r--r--   0 runner    (1001) docker     (127)    10485 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py38/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9589 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py38/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py38/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py38/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py38/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py38/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.674499 contrast_agent-8.3.0/src/contrast/assess_extensions/py39/
+-rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py39/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py39/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py39/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py39/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py39/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/assess_extensions/py39/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.674499 contrast_agent-8.3.0/src/contrast/bottle/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/bottle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/bottle/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.678499 contrast_agent-8.3.0/src/contrast/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/configuration/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/configuration/agent_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/configuration/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/configuration/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/configuration/assess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/configuration/config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/configuration/config_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/configuration/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/configuration/protect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/configuration/root.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/configuration/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.678499 contrast_agent-8.3.0/src/contrast/django/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/django/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.678499 contrast_agent-8.3.0/src/contrast/django_asgi/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/django_asgi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/django_asgi/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.678499 contrast_agent-8.3.0/src/contrast/falcon/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/falcon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/falcon/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.678499 contrast_agent-8.3.0/src/contrast/falcon_asgi/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/falcon_asgi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/falcon_asgi/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.678499 contrast_agent-8.3.0/src/contrast/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/fastapi/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.682499 contrast_agent-8.3.0/src/contrast/flask/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/flask/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.682499 contrast_agent-8.3.0/src/contrast/loader/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/loader/sitecustomize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.682499 contrast_agent-8.3.0/src/contrast/patches/
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/cgi_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/concurrent_futures_thread_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/cs_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10868 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/cs_str.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.686499 contrast_agent-8.3.0/src/contrast/patches/databases/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8638 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/databases/dbapi2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/databases/mysql_connector_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/databases/psycopg2_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/databases/pymysql_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/databases/sqlalchemy_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/databases/sqlite3_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/encodings_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7791 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/exec_and_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.686499 contrast_agent-8.3.0/src/contrast/patches/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/frameworks/bottle_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/frameworks/django_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/frameworks/drf_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/frameworks/falcon_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/frameworks/flask_and_quart_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6213 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/frameworks/pyramid_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/frameworks/starlette_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/genshi_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9370 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/import_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/lxml_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.686499 contrast_agent-8.3.0/src/contrast/patches/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/middleware/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/middleware/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6613 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/middleware/django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/middleware/mod_wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/pathlib_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/re_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/str_new.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/sys_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/threading_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/urllib_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/patches/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.686499 contrast_agent-8.3.0/src/contrast/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/deadzones.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.690499 contrast_agent-8.3.0/src/contrast/policy/propagators/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/propagators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/propagators/codecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/propagators/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/propagators/frameworks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/propagators/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/propagators/re.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/propagators/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/propagators/string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.690499 contrast_agent-8.3.0/src/contrast/policy/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/sources/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/sources/cgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/sources/django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/sources/falcon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/sources/flask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/sources/quart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/sources/webob.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.694499 contrast_agent-8.3.0/src/contrast/policy/triggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/triggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/triggers/cmd_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/triggers/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/triggers/httponly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/triggers/nosql_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/triggers/path_traversal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/triggers/prompt_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/triggers/redos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/triggers/reflected_xss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/triggers/secure_flag_missing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/triggers/session_rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/triggers/session_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/triggers/sql_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/triggers/ssrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/triggers/trust_boundary_violation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/triggers/unsafe_code_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/triggers/untrusted_deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/triggers/unvalidated_redirect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/triggers/xpath_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/policy/triggers/xxe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.694499 contrast_agent-8.3.0/src/contrast/pyramid/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/pyramid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/pyramid/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.694499 contrast_agent-8.3.0/src/contrast/quart/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/quart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/quart/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.694499 contrast_agent-8.3.0/src/contrast/reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/reporting/activity_masker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/reporting/reporting_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/reporting/request_audit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.698499 contrast_agent-8.3.0/src/contrast/reporting/teamserver_messages/
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/reporting/teamserver_messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/reporting/teamserver_messages/_traces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/reporting/teamserver_messages/agent_startup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/reporting/teamserver_messages/application_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/reporting/teamserver_messages/application_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/reporting/teamserver_messages/application_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/reporting/teamserver_messages/base_ts_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/reporting/teamserver_messages/effective_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/reporting/teamserver_messages/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/reporting/teamserver_messages/library_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/reporting/teamserver_messages/observed_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/reporting/teamserver_messages/preflight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/reporting/teamserver_messages/server_activity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.698499 contrast_agent-8.3.0/src/contrast/reporting/teamserver_responses/
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/reporting/teamserver_responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/reporting/teamserver_responses/application_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/reporting/teamserver_responses/ng_application_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/reporting/teamserver_responses/ng_server_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/reporting/teamserver_responses/protect_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/reporting/teamserver_responses/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/reporting/teamserver_responses/server_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.698499 contrast_agent-8.3.0/src/contrast/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/scripts/fix_interpreter_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/scripts/propagator_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/scripts/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/scripts/validate_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.702499 contrast_agent-8.3.0/src/contrast/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.706499 contrast_agent-8.3.0/src/contrast/utils/assess/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/assess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/assess/duck_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.706499 contrast_agent-8.3.0/src/contrast/utils/assess/formatting/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/assess/formatting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/assess/formatting/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/assess/formatting/tokenize_cformat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/assess/formatting/tokenize_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6671 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/assess/stream_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/assess/tag_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/assess/tracking_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/base64_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/configuration_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/context_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/deprecated_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/digest_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/environ.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.706499 contrast_agent-8.3.0/src/contrast/utils/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/exceptions/deprecation_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/exceptions/wrong_django_middleware_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/exceptions/wsgi_compliance_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/ignored_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.706499 contrast_agent-8.3.0/src/contrast/utils/library_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/library_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/library_reader/library_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/library_reader/patched_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/library_reader/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/locale.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.706499 contrast_agent-8.3.0/src/contrast/utils/loggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17667 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/loggers/structlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/module_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/object_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/patch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/pattern_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/safe_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6279 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/stack_trace_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/stdlib_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/string_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-30 14:05:43.000000 contrast_agent-8.3.0/src/contrast/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.706499 contrast_agent-8.3.0/src/contrast/wsgi/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/wsgi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast/wsgi/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.738499 contrast_agent-8.3.0/src/contrast_agent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    32208 2024-05-30 14:05:43.000000 contrast_agent-8.3.0/src/contrast_agent.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.706499 contrast_agent-8.3.0/src/contrast_rewriter/
+-rw-r--r--   0 runner    (1001) docker     (127)    15340 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_rewriter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.710499 contrast_agent-8.3.0/src/contrast_vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.710499 contrast_agent-8.3.0/src/contrast_vendor/importlib_metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/importlib_metadata/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    34323 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/importlib_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/importlib_metadata/_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/importlib_metadata/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/importlib_metadata/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/importlib_metadata/_functools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/importlib_metadata/_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/importlib_metadata/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/importlib_metadata/_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.710499 contrast_agent-8.3.0/src/contrast_vendor/importlib_metadata/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/importlib_metadata/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/importlib_metadata/compat/py39.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/importlib_metadata/diagnose.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/importlib_metadata/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.710499 contrast_agent-8.3.0/src/contrast_vendor/isort/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/isort/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/isort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.714499 contrast_agent-8.3.0/src/contrast_vendor/isort/stdlibs/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/isort/stdlibs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/isort/stdlibs/all.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/isort/stdlibs/py2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/isort/stdlibs/py27.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/isort/stdlibs/py3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/isort/stdlibs/py310.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/isort/stdlibs/py311.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/isort/stdlibs/py312.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/isort/stdlibs/py36.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/isort/stdlibs/py37.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/isort/stdlibs/py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/isort/stdlibs/py39.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.714499 contrast_agent-8.3.0/src/contrast_vendor/ported_cpython_code/
+-rw-r--r--   0 runner    (1001) docker     (127)    12769 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/ported_cpython_code/PYTHON_SOFTWARE_FOUNDATION_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/ported_cpython_code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/ported_cpython_code/import_functionality.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.606499 contrast_agent-8.3.0/src/contrast_vendor/ruamel/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.722499 contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/anchor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37673 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/composer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/configobjwalker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70392 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/cyaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/dumper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67960 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/emitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8807 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7278 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59457 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36019 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44497 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/representer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15209 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/scalarbool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/scalarfloat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/scalarint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/scalarstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87945 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8231 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.734499 contrast_agent-8.3.0/src/contrast_vendor/structlog/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/structlog/LICENSE-APACHE
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/structlog/LICENSE-MIT
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/structlog/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/structlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7279 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/structlog/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13884 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/structlog/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/structlog/_frames.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/structlog/_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/structlog/_greenlets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/structlog/_log_levels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/structlog/_native.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9147 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/structlog/_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/structlog/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/structlog/contextvars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23950 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/structlog/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/structlog/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28645 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/structlog/processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/structlog/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    38091 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/structlog/stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/structlog/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9206 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/structlog/threadlocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7799 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/structlog/tracebacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10123 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/structlog/twisted.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/structlog/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7979 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/structlog/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/vendor-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.738499 contrast_agent-8.3.0/src/contrast_vendor/webob/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/webob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   210210 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/webob/acceptparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/webob/byterange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/webob/cachecontrol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/webob/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/webob/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32879 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/webob/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/webob/datetime_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/webob/dec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/webob/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/webob/etag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38268 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/webob/exc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/webob/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/webob/license.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13961 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/webob/multidict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59159 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/webob/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55423 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/webob/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/webob/static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/webob/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.738499 contrast_agent-8.3.0/src/contrast_vendor/wrapt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/wrapt/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/wrapt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/wrapt/__wrapt__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/wrapt/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21333 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/wrapt/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10997 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/wrapt/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/wrapt/patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/wrapt/weakrefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27532 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/wrapt/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.738499 contrast_agent-8.3.0/src/contrast_vendor/zipp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/zipp/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11431 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/zipp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:43.738499 contrast_agent-8.3.0/src/contrast_vendor/zipp/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/zipp/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/zipp/compat/py310.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-30 14:05:31.000000 contrast_agent-8.3.0/src/contrast_vendor/zipp/glob.py
```

### Comparing `contrast_agent-8.2.0/LICENSE.txt` & `contrast_agent-8.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/MANIFEST.in` & `contrast_agent-8.3.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/PKG-INFO` & `contrast_agent-8.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contrast-agent
-Version: 8.2.0
+Version: 8.3.0
 Summary: Contrast Security's agent for Python web frameworks
 Author-email: "Contrast Security, Inc." <python@contrastsecurity.com>
 License: Copyright: 2024 Contrast Security, Inc
         Contact: support@contrastsecurity.com
         License: Commercial
         
         NOTICE: This Software and the patented inventions embodied within may only be used as
@@ -25,14 +25,16 @@
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Requires-Python: <3.13,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: requests<3,>=2.4.2
 Requires-Dist: contrast-agent-lib~=0.7.0
+Provides-Extra: debug
+Requires-Dist: viztracer~=0.16.3; extra == "debug"
 
 # Contrast Python Agent
 
 
 The Contrast Python Agent provides interactive vulnerability discovery and
 runtime protection for web applications. The agent is a WSGI-, ASGI-, and
 framework-specific middleware that's compatible with the most popular web
```

### Comparing `contrast_agent-8.2.0/hookspy/README.md` & `contrast_agent-8.3.0/hookspy/README.md`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/hookspy/ext/hookspy.c` & `contrast_agent-8.3.0/hookspy/ext/hookspy.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/hookspy/setup.py` & `contrast_agent-8.3.0/hookspy/setup.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/hookspy/src/hookspy/autogen.py` & `contrast_agent-8.3.0/hookspy/src/hookspy/autogen.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/hookspy/src/hookspy/body.py` & `contrast_agent-8.3.0/hookspy/src/hookspy/body.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/hookspy/src/hookspy/signatures.py` & `contrast_agent-8.3.0/hookspy/src/hookspy/signatures.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/hookspy/src/hookspy/spy.py` & `contrast_agent-8.3.0/hookspy/src/hookspy/spy.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/pyproject.toml` & `contrast_agent-8.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,20 +15,27 @@
     "contrast-agent-lib~=0.7.0",
 ]
 description = "Contrast Security's agent for Python web frameworks"
 keywords = ["security development"]
 license = { file = "LICENSE.txt" }
 requires-python = ">=3.8,<3.13"
 readme = "README.md"
+
+[project.optional-dependencies]
+debug = [
+    "viztracer~=0.16.3"
+]
+
 [project.urls]
 "Contrast" = "https://www.contrastsecurity.com"
 "Change Log" = "https://docs.contrastsecurity.com/en/python-agent-release-notes-and-archive.html"
 "Support" = "https://support.contrastsecurity.com"
 "Trouble Shooting" = "https://support.contrastsecurity.com/hc/en-us/search?utf8=%E2%9C%93&query=Python"
 "Wiki" = "https://docs.contrastsecurity.com/"
+
 [project.scripts]
 "contrast-python-run" = "contrast.scripts:runner"
 "contrast-fix-interpreter-permissions" = "contrast.scripts.fix_interpreter_permissions:fix_interpreter_permissions"
 "contrast-validate-config" = "contrast.scripts.validate_config:validate_config"
 "contrast-propagator-check" = "contrast.scripts.propagator_check:propagator_check"
 
 [build-system]
```

### Comparing `contrast_agent-8.2.0/setup.py` & `contrast_agent-8.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/__init__.py` & `contrast_agent-8.3.0/src/contrast/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/agent_lib/__init__.py` & `contrast_agent-8.3.0/src/contrast/agent/agent_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/agent_lib/input_tracing.py` & `contrast_agent-8.3.0/src/contrast/agent/agent_lib/input_tracing.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/agent_lib/main.py` & `contrast_agent-8.3.0/src/contrast/agent/agent_lib/main.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/agent_state.py` & `contrast_agent-8.3.0/src/contrast/agent/agent_state.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/asgi.py` & `contrast_agent-8.3.0/src/contrast/agent/asgi.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/adjusted_span.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/adjusted_span.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/apply_trigger.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/apply_trigger.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/contrast_event.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/contrast_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     TraceEventObject,
     ParentObjectId,
     TraceEventSource,
 )
 from contrast.utils.assess.duck_utils import len_or_zero
 from contrast.utils.base64_utils import B64_NONE_STRING, base64_encode
 from contrast.utils.stack_trace_utils import (
+    StackSummary,
     acceptable_frame,
     build_stack,
     clean_stack,
 )
 from contrast_vendor import structlog as logging
 from contrast_vendor.webob.util import html_escape
 
@@ -165,15 +166,15 @@
         # These are needed only at trigger-time but values must be set at init.
         self.time_ns = time.time_ns()
         self.thread = threading.current_thread().ident
         self.event_id = ContrastEvent._atomic_id()
 
         self.event_action = self.node.build_action()
 
-        self._raw_stack = build_stack() if self._should_get_stack else []
+        self._raw_stack = build_stack() if self._should_get_stack else StackSummary()
 
         # This must happen at init for stream events to work.
         self._update_method_information()
 
     def _init_tagged(self, tagged: Any, possible_key=None, args=None, kwargs=None):
         """
         Initialize properties related to tagging.
@@ -290,15 +291,15 @@
         event.action = self.event_action
         event.timestamp_ms = self.time_ns // 1_000_000
         event.thread = str(self.thread)
         event.tags = self.node.tags
 
         self._build_all_event_objects(event)
 
-        event.stack = clean_stack(self._raw_stack, depth=20)
+        event.stack = clean_stack(self._raw_stack)
 
         safe_source_name = self.source_name if self.source_name is not None else ""
         event.field_name = safe_source_name
 
         if self.source_type:
             event.event_sources.append(self.build_source_event(safe_source_name))
```

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/policy/analysis.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/policy/analysis.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/policy/deadzone_node.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/policy/deadzone_node.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/policy/patches.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/policy/patches.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/policy/preshift.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/policy/preshift.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagation_node.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagation_node.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagation_policy.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagation_policy.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/__init__.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/append_propagator.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/append_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/base_propagator.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/base_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/db_write_propagator.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/db_write_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/encode_html_splat_propagator.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/encode_html_splat_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/format_propagator.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/format_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/join_propagator.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/join_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/json_propagator.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/json_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/prepend_propagator.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/prepend_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/reductive_propagator.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/reductive_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/regex_propagator.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/regex_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/replace_propagator.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/replace_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/repr_propagator.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/repr_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator_django.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator_django.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/splat_propagator.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/splat_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/split_propagator.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/split_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/starlette_safe_path_propagator.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/starlette_safe_path_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/stream_propagator.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/policy/propagators/stream_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/policy/source_node.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/policy/source_node.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/policy/source_policy.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/policy/source_policy.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/policy/string_propagation.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/policy/string_propagation.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/policy/trigger_actions/default_action.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/policy/trigger_actions/default_action.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/policy/trigger_actions/fromstring_action.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/policy/trigger_actions/fromstring_action.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/policy/trigger_actions/openai_action.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/policy/trigger_actions/openai_action.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/policy/trigger_actions/redos_action.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/policy/trigger_actions/redos_action.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/policy/trigger_actions/ssrf_action.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/policy/trigger_actions/ssrf_action.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/policy/trigger_actions/subprocess_action.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/policy/trigger_actions/subprocess_action.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/policy/trigger_policy.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/policy/trigger_policy.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/preflight.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/preflight.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/properties.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/properties.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/rules/base_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/rules/base_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/base_config_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/rules/config/base_config_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/base_django_config_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/rules/config/base_django_config_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/base_flask_config_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/rules/config/base_flask_config_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/falcon_secure_flag_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/rules/config/falcon_secure_flag_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/secure_flag_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/rules/config/secure_flag_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/session_age_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/rules/config/session_age_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/rules/dataflow_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/rules/dataflow_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/rules/non_dataflow_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/rules/non_dataflow_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/rules/providers/code_parser_mixin.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/rules/providers/code_parser_mixin.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/rules/providers/enable.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/rules/providers/enable.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/rules/providers/hardcoded_key.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/rules/providers/hardcoded_key.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/rules/providers/hardcoded_password.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/rules/providers/hardcoded_password.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/rules/providers/hardcoded_value_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/rules/providers/hardcoded_value_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/analyze.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/rules/response/analyze.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/autocomplete_missing_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/rules/response/autocomplete_missing_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/base_body_only_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/rules/response/base_body_only_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/base_header_only_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/rules/response/base_header_only_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/base_response_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/rules/response/base_response_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/cache_controls_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/rules/response/cache_controls_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/clickjacking_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/rules/response/clickjacking_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/csp_header_insecure_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/rules/response/csp_header_insecure_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/csp_header_missing_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/rules/response/csp_header_missing_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/hsts_header_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/rules/response/hsts_header_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/parameter_pollution_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/rules/response/parameter_pollution_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/x_content_type_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/rules/response/x_content_type_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/x_xss_protection_disabled_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/rules/response/x_xss_protection_disabled_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/xss.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/rules/response/xss.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/rules/static_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/rules/static_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/rules/trigger_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/rules/trigger_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/rules/triggers/httponly_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/rules/triggers/httponly_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/rules/triggers/secure_flag_missing_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/rules/triggers/secure_flag_missing_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/rules/triggers/session_rewriting_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/rules/triggers/session_rewriting_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/rules/triggers/session_timeout_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/rules/triggers/session_timeout_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/rules/triggers/trigger_config_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/rules/triggers/trigger_config_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/sampling.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/sampling.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/string_tracker.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/string_tracker.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/tag.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/tag.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/truncate.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/truncate.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/assess/utils.py` & `contrast_agent-8.3.0/src/contrast/agent/assess/utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/disable_reaction.py` & `contrast_agent-8.3.0/src/contrast/agent/disable_reaction.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/events.py` & `contrast_agent-8.3.0/src/contrast/agent/events.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/exceptions.py` & `contrast_agent-8.3.0/src/contrast/agent/exceptions.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/exclusions.py` & `contrast_agent-8.3.0/src/contrast/agent/exclusions.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/framework.py` & `contrast_agent-8.3.0/src/contrast/agent/framework.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/heartbeat_thread.py` & `contrast_agent-8.3.0/src/contrast/agent/heartbeat_thread.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/metrics.py` & `contrast_agent-8.3.0/src/contrast/agent/metrics.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/middlewares/app_finder.py` & `contrast_agent-8.3.0/src/contrast/agent/middlewares/app_finder.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/middlewares/base_middleware.py` & `contrast_agent-8.3.0/src/contrast/agent/middlewares/base_middleware.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,14 +50,17 @@
             request_path=request_path,
         )
         logger.info(
             "request summary",
             request_path=request_path,
             request_method=request_method,
             elapsed_time_ms=timer.now_ms() - start_time,
+            # native thread id is useful for lining up viztracer threads to requests,
+            # but it requires a syscall so we don't want it in every log message
+            native_thread_id=threading.get_native_id(),
         )
 
 
 def _log_response_info(response: BaseResponseWrapper):
     if response is None:
         logger.debug("No response info for this request")
         return
@@ -104,15 +107,14 @@
         Config scanning still happens here since the behavior is framework-specific.
         """
         # id will be different across processes but also for multiple middlewares
         # within the same process
         self.id = id(self)
         self.settings = None
         self.request_start_time = None
-        self.request_path = None
 
         if BaseMiddleware._loaded:
             logger.warning(
                 "Contrast Agent middleware initialized more than once per process."
             )
 
         agent_state.initialize()
@@ -151,42 +153,44 @@
         raise NotImplementedError("Must implement call_with_agent")
 
     def call_without_agent(self, *args):
         """
         The agent does not set context when this function is called so all other patches
         (e.g propagators) that check context shouldn't run.
         """
-        logger.debug("Contrast Agent did not analyze request %s", self.request_path)
+        raise NotImplementedError("Must implement call_without_agent")
 
     def should_analyze_request(self, environ):
         """
         Determine if request should be analyzed based on configured settings.
 
         While returning different types of objects based on logic is not a good
         pattern, in this case it's an optimization that allows us to create
         the request context obj when we need it.
 
         :return: False or RequestContext instance
         """
+        path = environ.get("PATH_INFO")
+
         if not self.is_agent_enabled():
-            logger.debug("Will not analyze request: agent disabled.")
+            logger.debug("Will not analyze request: agent disabled.", path=path)
             return False
 
         context = RequestContext(environ)
 
-        path = environ.get("PATH_INFO")
-
         if self.settings.evaluate_exclusions(context, path):
-            logger.debug("Will not analyze request: request meets exclusions.")
+            logger.debug(
+                "Will not analyze request: request meets exclusions.", path=path
+            )
             return False
 
         from contrast.agent.assess import sampling
 
         if sampling.enabled() and sampling.meets_criteria(context):
-            logger.debug("Will not analyze request: request meets sampling.")
+            logger.debug("Will not analyze request: request meets sampling.", path=path)
             return False
 
         return context  # equivalent to returning True
 
     @fail_loudly("Unable to do handle_ensure")
     def handle_ensure(self, context, request):
         """
```

### Comparing `contrast_agent-8.2.0/src/contrast/agent/middlewares/environ_tracker.py` & `contrast_agent-8.3.0/src/contrast/agent/middlewares/environ_tracker.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/middlewares/response_wrappers/aiohttp_response_wrapper.py` & `contrast_agent-8.3.0/src/contrast/agent/middlewares/response_wrappers/aiohttp_response_wrapper.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/middlewares/response_wrappers/base_response_wrapper.py` & `contrast_agent-8.3.0/src/contrast/agent/middlewares/response_wrappers/base_response_wrapper.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/aiohttp_routes.py` & `contrast_agent-8.3.0/src/contrast/agent/middlewares/route_coverage/aiohttp_routes.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/bottle_routes.py` & `contrast_agent-8.3.0/src/contrast/agent/middlewares/route_coverage/bottle_routes.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/common.py` & `contrast_agent-8.3.0/src/contrast/agent/middlewares/route_coverage/common.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/django_routes.py` & `contrast_agent-8.3.0/src/contrast/agent/middlewares/route_coverage/django_routes.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/falcon_routes.py` & `contrast_agent-8.3.0/src/contrast/agent/middlewares/route_coverage/falcon_routes.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/flask_routes.py` & `contrast_agent-8.3.0/src/contrast/agent/middlewares/route_coverage/flask_routes.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/pyramid_routes.py` & `contrast_agent-8.3.0/src/contrast/agent/middlewares/route_coverage/pyramid_routes.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/routes_mixin.py` & `contrast_agent-8.3.0/src/contrast/agent/middlewares/route_coverage/routes_mixin.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/starlette_routes.py` & `contrast_agent-8.3.0/src/contrast/agent/middlewares/route_coverage/starlette_routes.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/patch_controller.py` & `contrast_agent-8.3.0/src/contrast/agent/patch_controller.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/policy/applicator.py` & `contrast_agent-8.3.0/src/contrast/agent/policy/applicator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/policy/constants.py` & `contrast_agent-8.3.0/src/contrast/agent/policy/constants.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/policy/patch_location_policy.py` & `contrast_agent-8.3.0/src/contrast/agent/policy/patch_location_policy.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/policy/patch_manager.py` & `contrast_agent-8.3.0/src/contrast/agent/policy/patch_manager.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/policy/policy_node.py` & `contrast_agent-8.3.0/src/contrast/agent/policy/policy_node.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/policy/registry.py` & `contrast_agent-8.3.0/src/contrast/agent/policy/registry.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/policy/rewriter.py` & `contrast_agent-8.3.0/src/contrast/agent/policy/rewriter.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/policy/trigger_node.py` & `contrast_agent-8.3.0/src/contrast/agent/policy/trigger_node.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/policy/utils.py` & `contrast_agent-8.3.0/src/contrast/agent/policy/utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/protect/input_analysis.py` & `contrast_agent-8.3.0/src/contrast/agent/protect/input_analysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 import contrast
 
 import xml.etree.ElementTree
-from contrast.utils.loggers.logger import security_log_msg
-from contrast.utils.string_utils import ensure_string
 
 from contrast.api.user_input import DocumentType, InputType
 from contrast.agent.settings import Settings
 from contrast.agent import agent_lib
 from contrast_vendor import structlog as logging
 from contrast.utils.decorators import fail_quietly
 
@@ -325,25 +323,15 @@
                 and rule_name == input_row.rule_id
             ):
                 logger.debug(
                     f"Input analysis found a value '{input_row.value}' "
                     f"that violated {rule_name} rule!"
                 )
 
-                if input_row.rule_id == rule.RULE_NAME and rule.is_blocked():
-                    rule_message = f"{rule_name} - {ensure_string(input_row.value, errors='replace')}"
-
-                    msg = (
-                        f"The {input_row.input_type.name} {input_row.value} "
-                        "had a value that successfully exploited "
-                        f"{ensure_string(rule_message, errors='replace')}"
-                    )
-
-                    security_log_msg(msg, Settings().app_name, rule_name, "EXPLOITED")
-
+                if rule.is_blocked():
                     raise contrast.SecurityException(rule_name=rule_name)
 
 
 def check_url_input_exclusion(exclusions, input_type, param):
     if not exclusions:
         return False
```

### Comparing `contrast_agent-8.2.0/src/contrast/agent/protect/policy/__init__.py` & `contrast_agent-8.3.0/src/contrast/agent/protect/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/protect/rule/base_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/protect/rule/base_rule.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 
+from typing import Optional
 import contrast
 from contrast.agent import scope
 from contrast.agent.settings import Settings
 from contrast.api.attack import Attack, ProtectResponse
 from contrast.api.user_input import UserInput, InputType
 from contrast.api.sample import Sample
 from contrast.agent.protect.rule.mode import Mode
 from contrast.utils.decorators import fail_loudly, fail_quietly
 from contrast.utils.decorators import cached_property
 from contrast.utils.stack_trace_utils import build_and_clean_stack
 from contrast_vendor import structlog as logging
-from contrast.utils.loggers.logger import security_log_msg
+from contrast.utils.loggers.logger import security_log_attack
 from contrast.utils.string_utils import ensure_string
 
 logger = logging.getLogger("contrast")
 
 
 BLOCKING_RULES = frozenset([Mode.BLOCK, Mode.BLOCK_AT_PERIMETER])
 PREFILTER_RULES = frozenset([Mode.BLOCK_AT_PERIMETER])
@@ -237,44 +238,54 @@
                 )
             else:
                 attack = self.build_attack_without_match(evaluation, attack, **kwargs)
 
         return attack
 
     def build_attack_with_match(
-        self, candidate_string, evaluation=None, attack=None, **kwargs
+        self,
+        candidate_string,
+        evaluation=None,
+        attack: Optional[Attack] = None,
+        **kwargs,
     ):
         attack = self.build_or_append_attack(
             evaluation, attack, candidate_string, **kwargs
         )
 
         if evaluation:
             evaluation.attack_count += 1
 
-        attack.set_response(self.response_from_mode(self.mode))
-        self.log_rule_matched(evaluation, attack.response, candidate_string)
+        attack.response = self.response_from_mode(self.mode)
+        security_log_attack(attack, evaluation, Settings().app_name)
         return attack
 
-    def build_attack_without_match(self, evaluation=None, attack=None, **kwargs):
+    def build_attack_without_match(
+        self, evaluation=None, attack: Optional[Attack] = None, **kwargs
+    ):
         if evaluation and evaluation.score < 10:
             return None
         if self.mode == Mode.BLOCK_AT_PERIMETER:
             attack = self.build_or_append_attack(evaluation, attack, **kwargs)
 
-            attack.set_response(self.response_from_mode(self.mode))
-            self.log_rule_matched(evaluation, attack.response)
+            attack.response = self.response_from_mode(self.mode)
+            security_log_attack(attack, evaluation, Settings().app_name)
         elif evaluation is None or evaluation.attack_count == 0:
             attack = self.build_or_append_attack(evaluation, attack, **kwargs)
-            attack.set_response(ProtectResponse.PROBED)
-            self.log_rule_probed(evaluation)
+            attack.response = ProtectResponse.PROBED
+            security_log_attack(attack, evaluation, Settings().app_name)
 
         return attack
 
     def build_or_append_attack(
-        self, evaluation, attack=None, candidate_string=None, **kwargs
+        self,
+        evaluation,
+        attack: Optional[Attack] = None,
+        candidate_string=None,
+        **kwargs,
     ):
         if attack is None:
             attack = self.build_base_attack()
 
         attack.add_sample(self.build_sample(evaluation, candidate_string, **kwargs))
 
         return attack
@@ -305,62 +316,14 @@
             )
 
         stack = prebuilt_stack if prebuilt_stack else build_and_clean_stack()
         sample.set_stack(stack)
 
         return sample
 
-    def log_rule_matched(self, evaluation, response, _=None):
-        """
-        Logs the exploit for the rule to the security logger
-        """
-        outcome = response.name.replace("_", " ")
-
-        if evaluation:
-            key = str(evaluation.key) if evaluation.key else ""
-
-            rule_message = (
-                f"{self.name} - {ensure_string(evaluation.value, errors='replace')}"
-            )
-
-            msg = f"The {evaluation.input_type.name} {key} had a value that successfully exploited {ensure_string(rule_message, errors='replace')}"
-        else:
-            msg = self.effective_attack_message()
-
-        security_log_msg(msg, Settings().app_name, self.name, outcome)
-
-    def log_rule_probed(self, evaluation):
-        """
-        Logs the probed attack for the rule to the security logger
-        """
-        outcome = "INEFFECTIVE"
-
-        if evaluation:
-            key = str(evaluation.key) if evaluation.key else ""
-
-            rule_message = (
-                f"{self.name} - {ensure_string(evaluation.value, errors='replace')}"
-            )
-
-            msg = (
-                f"The {evaluation.input_type.name} {key} had a value that matched a signature for, but did not"
-                f" successfully exploit {ensure_string(rule_message, errors='replace')}"
-            )
-
-        else:
-            msg = self.ineffective_attack_message()
-
-        security_log_msg(msg, Settings().app_name, self.name, outcome)
-
-    def effective_attack_message(self):
-        return f"An effective attack was detected against {self.name}."
-
-    def ineffective_attack_message(self):
-        return f"An ineffective attack was detected against {self.name}."
-
     def _append_to_context(self, attack):
         context = contrast.CS__CONTEXT_TRACKER.current()
         if context is None:
             # do not remove; this case is not yet well-understood
             logger.debug("WARNING: failed to get request context in _append_to_context")
             return
```

### Comparing `contrast_agent-8.2.0/src/contrast/agent/protect/rule/cmdi_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/protect/rule/cmdi_rule.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 import re
 
 from contrast.agent.agent_lib.input_tracing import check_cmd_injection_query
 from contrast.agent.protect.rule.mode import Mode
+from contrast.agent.settings import Settings
+from contrast.utils.loggers.logger import security_log_attack
 from .base_rule import BaseRule
 
 from contrast_vendor import structlog as logging
 
 logger = logging.getLogger("contrast")
 
 
@@ -46,16 +48,16 @@
             kwargs["startIndex"] = match.start()
             kwargs["endIndex"] = match.end()
             attack = self.build_or_append_attack(
                 evaluation, attack, candidate_string, **kwargs
             )
 
         if attack is not None:
-            attack.set_response(self.response_from_mode(self.mode))
-            self.log_rule_matched(evaluation, attack.response, candidate_string)
+            attack.response = self.response_from_mode(self.mode)
+            security_log_attack(attack, evaluation, Settings().app_name)
 
         return attack
 
     def build_attack_without_match(self, evaluation=None, attack=None, **kwargs):
         if self.mode == Mode.BLOCK_AT_PERIMETER:
             return super().build_attack_without_match(evaluation, attack, **kwargs)
         if evaluation.score < 10:
```

### Comparing `contrast_agent-8.2.0/src/contrast/agent/protect/rule/deserialization/custom_searcher.py` & `contrast_agent-8.3.0/src/contrast/agent/protect/rule/deserialization/custom_searcher.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/protect/rule/deserialization/pickle_searcher.py` & `contrast_agent-8.3.0/src/contrast/agent/protect/rule/deserialization/pickle_searcher.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/protect/rule/deserialization/yaml_searcher.py` & `contrast_agent-8.3.0/src/contrast/agent/protect/rule/deserialization/yaml_searcher.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/protect/rule/deserialization_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/protect/rule/deserialization_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/protect/rule/http_method_tampering.py` & `contrast_agent-8.3.0/src/contrast/agent/protect/rule/http_method_tampering.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,20 +36,22 @@
             return
 
         response_code = context.response.status_code
 
         for evaluation in evaluations_for_rule:
             if str(response_code).startswith("4") or str(response_code).startswith("5"):
                 attack = self.build_attack_without_match(
+                    evaluation=evaluation,
                     method=evaluation.value,
                     response_code=response_code,
                 )
             else:
                 attack = self.build_attack_with_match(
                     None,
+                    evaluation=evaluation,
                     method=evaluation.value,
                     response_code=response_code,
                 )
             self._append_to_context(attack)
 
     def build_sample(self, evaluation, candidate_string, **kwargs):
         sample = self.build_base_sample(None)
```

### Comparing `contrast_agent-8.2.0/src/contrast/agent/protect/rule/nosql_injection/mongo_nosql_scanner.py` & `contrast_agent-8.3.0/src/contrast/agent/protect/rule/nosql_injection/mongo_nosql_scanner.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/protect/rule/nosqli_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/protect/rule/nosqli_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/protect/rule/path_traversal_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/protect/rule/path_traversal_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/protect/rule/rules_builder.py` & `contrast_agent-8.3.0/src/contrast/agent/protect/rule/rules_builder.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/protect/rule/sqli_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/protect/rule/sqli_rule.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 import re
 from contrast.agent.protect.rule.base_rule import BaseRule
 from contrast.agent import agent_lib
 from contrast.agent.protect.rule.mode import Mode
+from contrast.agent.settings import Settings
+from contrast.utils.loggers.logger import security_log_attack
 
 
 class SqlInjection(BaseRule):
     """
     SQL Injection Protection rule
     """
 
@@ -36,16 +38,16 @@
             kwargs["boundary_overrun_idx"] = agent_lib_evaluation.boundary_overrun_index
             kwargs["input_boundary_idx"] = agent_lib_evaluation.input_boundary_index
             attack = self.build_or_append_attack(
                 evaluation, attack, candidate_string, **kwargs
             )
 
         if attack is not None:
-            attack.set_response(self.response_from_mode(self.mode))
-            self.log_rule_matched(evaluation, attack.response, candidate_string)
+            attack.response = self.response_from_mode(self.mode)
+            security_log_attack(attack, evaluation, Settings().app_name)
 
         return attack
 
     def build_attack_without_match(self, evaluation=None, attack=None, **kwargs):
         if self.mode == Mode.BLOCK_AT_PERIMETER:
             return super().build_attack_without_match(evaluation, attack, **kwargs)
         if evaluation.score < 10:
```

### Comparing `contrast_agent-8.2.0/src/contrast/agent/protect/rule/ssrf_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/protect/rule/ssrf_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/protect/rule/xss_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/protect/rule/xss_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/protect/rule/xxe/entity_wrapper.py` & `contrast_agent-8.3.0/src/contrast/agent/protect/rule/xxe/entity_wrapper.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/protect/rule/xxe_rule.py` & `contrast_agent-8.3.0/src/contrast/agent/protect/rule/xxe_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/reaction_processor.py` & `contrast_agent-8.3.0/src/contrast/agent/reaction_processor.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/request.py` & `contrast_agent-8.3.0/src/contrast/agent/request.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/request_context.py` & `contrast_agent-8.3.0/src/contrast/agent/request_context.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/request_state.py` & `contrast_agent-8.3.0/src/contrast/agent/request_state.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/runner.py` & `contrast_agent-8.3.0/src/contrast/agent/runner.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/scope.py` & `contrast_agent-8.3.0/src/contrast/agent/scope.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/server_settings_poll.py` & `contrast_agent-8.3.0/src/contrast/agent/server_settings_poll.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/settings.py` & `contrast_agent-8.3.0/src/contrast/agent/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,23 @@
 
     @cached_property
     def is_policy_rewriter_enabled(self):
         return self.config.should_apply_policy_rewrites
 
     @cached_property
     def is_profiler_enabled(self):
-        return self.config.get_value("agent.python.enable_profiler")
+        # TODO: PYT-3337 - we should issue a deprecation warning if
+        # agent.python.enable_profiler is used
+        return self.config.get_value(
+            "agent.python.enable_profiler"
+        ) or self.config.get_value("agent.python.profiler.enable")
+
+    @cached_property
+    def is_tracer_enabled(self):
+        return self.config.get_value("agent.python.tracer.enable")
 
     @cached_property
     def max_sources(self):
         return self.config.get_value("assess.max_context_source_events")
 
     @cached_property
     def max_propagation(self):
```

### Comparing `contrast_agent-8.2.0/src/contrast/agent/sys_monitoring.py` & `contrast_agent-8.3.0/src/contrast/agent/sys_monitoring.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/telemetry.py` & `contrast_agent-8.3.0/src/contrast/agent/telemetry.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/thread_watcher.py` & `contrast_agent-8.3.0/src/contrast/agent/thread_watcher.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/agent/validator.py` & `contrast_agent-8.3.0/src/contrast/agent/validator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/aiohttp/middleware.py` & `contrast_agent-8.3.0/src/contrast/aiohttp/middleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     log_request_start_and_end,
 )
 from contrast.agent.middlewares.response_wrappers.aiohttp_response_wrapper import (
     AioHttpResponseWrapper,
 )
 
 from contrast.utils.decorators import fail_quietly
-from contrast.utils import Profiler
+from contrast.utils.monitoring import Profiler, tracer
 
 logger = logging.getLogger("contrast")
 
 
 class AioHttpMiddleware(BaseMiddleware):
     __middleware_version__ = 1  # Aiohttp new-style middleware
 
@@ -45,20 +45,24 @@
         if request_state.get_request_id() is not None:
             # This can happen if a single app is wrapped by multiple instances of the
             # middleware (usually caused by automatic instrumentation)
             logger.debug("Detected preexisting request_id - passing through")
             return await handler(request)
 
         self.app = request.app
-        self.request_path = request.path
 
         # the request_id context manager must come first!
         with request_state.request_id_context(), Profiler(
-            self.request_path
-        ), log_request_start_and_end(request.method, self.request_path):
+            request.path,
+        ), log_request_start_and_end(
+            request.method,
+            request.path,
+        ), tracer(
+            request.path,
+        ):
             with scope.contrast_scope():
                 environ = await sources.aiohttp_request_to_environ(request)
 
             context = self.should_analyze_request(environ)
             if context:
                 with contrast.CS__CONTEXT_TRACKER.lifespan(context):
                     return await self.call_with_agent(context, request, handler)
@@ -89,15 +93,14 @@
                     self.do_aiohttp_first_request_analysis()
                     self.do_aiohttp_route_observation(context, request)
                 self.handle_ensure(context, request)
                 if self.settings.is_assess_enabled():
                     contrast.STRING_TRACKER.ageoff()
 
     async def call_without_agent_async(self, request, handler) -> StreamResponse:
-        super().call_without_agent()
         with scope.contrast_scope():
             return await handler(request)
 
     @fail_quietly()
     def do_aiohttp_first_request_analysis(self) -> None:
         if not agent_state.is_first_request():
             return
@@ -117,29 +120,29 @@
     @fail_quietly("Unable to get view func")
     def get_aiohttp_view_func(self, request):
         """
         This intentionally does not override get_view_func. We're generally making route
         coverage more framework-specific; this minimizes shared machinery between
         aiohttp middleware and its base classes.
         """
-        if not self.request_path:
+        if not request.path:
             return None
 
         view_func = None
 
         # This approach has at worst O(_resources) performance
         # but it's a first attempt at implementing a sync
         # version of aiohttp.web_urldispatches.UrlDispatcher.resolve
         for app_route in self.app.router._resources:
             _app_route = (
                 app_route._formatter
                 if isinstance(app_route, DynamicResource)
                 else app_route._path
             )
-            if _app_route == self.request_path:
+            if _app_route == request.path:
                 routes = app_route._routes
                 for route in routes:
                     if route.method == request.method:
                         return route.handler
 
         return view_func
```

### Comparing `contrast_agent-8.2.0/src/contrast/aiohttp/sources.py` & `contrast_agent-8.3.0/src/contrast/aiohttp/sources.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/api/architecture_component.py` & `contrast_agent-8.3.0/src/contrast/api/architecture_component.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/api/attack.py` & `contrast_agent-8.3.0/src/contrast/api/attack.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 from enum import Enum, auto
+from typing import Optional
 
 import contrast
 from contrast.agent.request import Request
 from contrast.utils.timer import now_ms
 from contrast_vendor import structlog as logging
 
 logger = logging.getLogger("contrast")
@@ -30,30 +31,30 @@
 
 class Attack:
     """
     Class storing all data necessary to report a protect attack.
     """
 
     def __init__(self, rule_id):
-        self.rule_id = rule_id
+        self.rule_id: str = rule_id
         self.samples = []
-        self.response = None
+        self.response: Optional[ProtectResponse] = None
         self.start_time_ms = contrast.CS__CONTEXT_TRACKER.current().request.timestamp_ms
-        self.response = None
 
     @property
     def blocked(self):
         return self.response == ProtectResponse.BLOCKED
 
+    @property
+    def perimeter_blocked(self):
+        return self.response == ProtectResponse.BLOCKED_AT_PERIMETER
+
     def add_sample(self, sample):
         self.samples.append(sample)
 
-    def set_response(self, response):
-        self.response = response
-
     def _convert_samples(self, request: Request):
         if request is not None:
             reportable_request = request.reportable_format
         else:
             reportable_request = {}
 
         return [
@@ -86,23 +87,23 @@
                     ),  # in ms which is the format TS accepts
                 },
             }
             for sample in self.samples
         ]
 
     def report_result(self):
-        if ProtectResponse.MONITORED == self.response:
-            if self.rule_id in SUSPICIOUS_RULES:
-                return "suspicious"
-            return "exploited"
-        if ProtectResponse.BLOCKED == self.response:
-            return "blocked"
-        if ProtectResponse.PROBED == self.response:
-            return "ineffective"
-        return None
+        response_map = {
+            ProtectResponse.BLOCKED: "blocked",
+            ProtectResponse.BLOCKED_AT_PERIMETER: "blocked",
+            ProtectResponse.PROBED: "ineffective",
+            ProtectResponse.MONITORED: (
+                "suspicious" if self.rule_id in SUSPICIOUS_RULES else "exploited"
+            ),
+        }
+        return response_map[self.response]
 
     def to_json(self, request: Request):
         common_fields = {
             "startTime": 0,
             "total": 0,
         }
         json = {
@@ -110,17 +111,14 @@
             "blocked": common_fields,
             "exploited": common_fields,
             "ineffective": common_fields,
             "suspicious": common_fields,
         }
 
         relevant_mode = self.report_result()
-        if relevant_mode is None:
-            # Don't know what response is so just report default info so we can debug.
-            return json
 
         samples = self._convert_samples(request)
 
         json[relevant_mode] = {
             "total": 1,  # always 1 until batching happens
             "startTime": self.start_time_ms,
             "samples": samples,
```

### Comparing `contrast_agent-8.2.0/src/contrast/api/finding.py` & `contrast_agent-8.3.0/src/contrast/api/finding.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/api/library.py` & `contrast_agent-8.3.0/src/contrast/api/library.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/api/route_coverage.py` & `contrast_agent-8.3.0/src/contrast/api/route_coverage.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/api/trace_event.py` & `contrast_agent-8.3.0/src/contrast/api/trace_event.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/api/type_checked_property.py` & `contrast_agent-8.3.0/src/contrast/api/type_checked_property.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/applies/__init__.py` & `contrast_agent-8.3.0/src/contrast/applies/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/applies/assess/unsafe_code_execution.py` & `contrast_agent-8.3.0/src/contrast/applies/assess/unsafe_code_execution.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/applies/sqli.py` & `contrast_agent-8.3.0/src/contrast/applies/sqli.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/asgi/middleware.py` & `contrast_agent-8.3.0/src/contrast/asgi/middleware.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     ASGIRequest,
     ASGIResponse,
 )
 from contrast.utils.decorators import cached_property
 from contrast.utils.safe_import import safe_import_list
 from contrast.utils.assess.duck_utils import safe_getattr_list
 
-from contrast.utils import Profiler
+from contrast.utils.monitoring import Profiler, tracer
 from contrast_vendor import structlog as logging
 
 
 logger = logging.getLogger("contrast")
 
 DEFAULT_ASGI_NAME = "asgi_app"
 
@@ -75,25 +75,30 @@
         if request_state.get_request_id() is not None:
             # This can happen if a single app is wrapped by multiple instances of the
             # middleware (usually caused by automatic instrumentation)
             logger.debug("Detected preexisting request_id - passing through")
             await self.asgi_app(scope, receive, send)
             return
 
-        self.request_path = scope.get("path", "")
+        request_path = scope.get("path", "")
+
+        if scope.get("type") != "http":
+            logger.debug("Detected non-http request - cannot analyze", scope=scope)
+            await self.call_without_agent_async(scope, receive, send)
+            return
 
         # the request_id context manager must come first!
         with request_state.request_id_context(), Profiler(
-            self.request_path
-        ), log_request_start_and_end(scope.get("method", ""), self.request_path):
-            if scope.get("type") != "http":
-                logger.debug("Detected non-http request - cannot analyze", scope=scope)
-                await self.call_without_agent_async(scope, receive, send)
-                return
-
+            request_path,
+        ), log_request_start_and_end(
+            scope.get("method", ""),
+            request_path,
+        ), tracer(
+            request_path,
+        ):
             request = ASGIRequest(scope, receive)
             environ = await request.to_wsgi_environ()
 
             context = self.should_analyze_request(environ)
             if context:
                 with contrast.CS__CONTEXT_TRACKER.lifespan(context):
                     await self.call_with_agent(context, request, send)
@@ -125,15 +130,14 @@
 
             finally:
                 self.handle_ensure(context, context.request)
                 if self.settings.is_assess_enabled():
                     contrast.STRING_TRACKER.ageoff()
 
     async def call_without_agent_async(self, scope, receive, send) -> None:
-        super().call_without_agent()
         with scope_.contrast_scope():
             await self.asgi_app(scope, receive, send)
 
     @cached_property
     def trigger_node(self):
         """
         trigger node used by reflected xss postfilter rule
```

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/__init__.py` & `contrast_agent-8.3.0/src/contrast/assess_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/common/cast.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/common/cast.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/common/format.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/common/format.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/common/logging.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/common/logging.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/common/patches.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/common/patches.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/common/propagate.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/common/propagate.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/common/repeat.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/common/repeat.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/common/repr.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/common/repr.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/common/scope.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/common/scope.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/common/streams.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/common/streams.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/common/subscript.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/common/subscript.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/common/trace.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/common/trace.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/cs_str.pyi` & `contrast_agent-8.3.0/src/contrast/assess_extensions/cs_str.pyi`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/.travis.yml` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/.travis.yml`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/LICENSE` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/LICENSE`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/Makefile.in` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/Makefile.in`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/README.md` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/README.md`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/appveyor.yml` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/appveyor.yml`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/config.guess` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/config.guess`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/config.sub` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/config.sub`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/configure.ac` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/configure.ac`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/COPYING` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/COPYING`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/README.md` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/README.md`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/include/distorm.h` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/include/distorm.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/include/mnemonics.h` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/include/mnemonics.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/make/linux/Makefile` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/make/linux/Makefile`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/make/mac/Makefile` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/make/mac/Makefile`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj.filters` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/make/win32/distorm.sln` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/make/win32/distorm.sln`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/make/win32/resource.rc` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/make/win32/resource.rc`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/setup.py` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/setup.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/config.h` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/config.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.h` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/distorm.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/distorm.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.h` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/insts.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/insts.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/insts.h` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/insts.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/mnemonics.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/mnemonics.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/operands.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/operands.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/operands.h` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/operands.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.h` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.h` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.h` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/x86defs.h` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/distorm/src/x86defs.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/include/funchook.h` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/include/funchook.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/install-sh` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/install-sh`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/Makefile.in` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/src/Makefile.in`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/__strerror.h` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/src/__strerror.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/funchook.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/src/funchook.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/funchook_internal.h` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/src/funchook_internal.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/funchook_io.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/src/funchook_io.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/funchook_io.h` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/src/funchook_io.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/funchook_syscall.S` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/src/funchook_syscall.S`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/funchook_unix.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/src/funchook_unix.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/funchook_windows.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/src/funchook_windows.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/funchook_x86.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/src/funchook_x86.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/os_func.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/src/os_func.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/os_func.h` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/src/os_func.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/os_func_unix.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/src/os_func_unix.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/os_func_windows.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/src/os_func_windows.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/printf_base.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/src/printf_base.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/printf_base.h` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/src/printf_base.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/test/Makefile.in` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/test/Makefile.in`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/test/suffix.list` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/test/suffix.list`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/test/test_main.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/test/test_main.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/test/x86_test.S` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/test/x86_test.S`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/win32/funchook.sln` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/win32/funchook.sln`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj.filters` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj.filters` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj.filters` & `contrast_agent-8.3.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/include/contrast/assess/logging.h` & `contrast_agent-8.3.0/src/contrast/assess_extensions/include/contrast/assess/logging.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/include/contrast/assess/patches.h` & `contrast_agent-8.3.0/src/contrast/assess_extensions/include/contrast/assess/patches.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/include/contrast/assess/propagate.h` & `contrast_agent-8.3.0/src/contrast/assess_extensions/include/contrast/assess/propagate.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/include/contrast/assess/scope.h` & `contrast_agent-8.3.0/src/contrast/assess_extensions/include/contrast/assess/scope.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/include/contrast/assess/utils.h` & `contrast_agent-8.3.0/src/contrast/assess_extensions/include/contrast/assess/utils.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py3/patches.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py3/patches.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py3/str_concat.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py3/str_concat.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py310/bytearray.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py310/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py310/bytes.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py310/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py310/bytesio.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py310/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py310/iobase.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py310/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py310/stringio.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py310/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py310/unicode.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py310/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py311/bytearray.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py311/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py311/bytes.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py311/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py311/bytesio.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py311/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py311/iobase.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py311/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py311/stringio.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py311/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py311/unicode.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py311/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py312/bytearray.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py312/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py312/bytes.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py312/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py312/bytesio.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py312/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py312/iobase.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py312/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py312/stringio.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py312/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py312/unicode.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py312/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py35/bytearray.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py35/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py35/bytes.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py35/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py35/bytesio.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py35/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py35/iobase.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py35/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py35/stringio.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py35/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py35/unicode.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py35/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py36/bytearray.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py36/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py36/bytes.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py36/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py36/bytesio.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py36/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py36/iobase.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py36/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py36/stringio.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py36/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py36/unicode.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py36/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py37/bytearray.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py37/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py37/bytes.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py37/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py37/bytesio.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py37/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py37/iobase.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py37/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py37/stringio.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py37/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py37/unicode.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py37/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py38/bytearray.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py38/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py38/bytes.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py38/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py38/bytesio.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py38/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py38/iobase.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py38/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py38/stringio.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py38/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py38/unicode.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py38/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py39/bytearray.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py39/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py39/bytes.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py39/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py39/bytesio.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py39/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py39/iobase.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py39/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py39/stringio.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py39/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/assess_extensions/py39/unicode.c` & `contrast_agent-8.3.0/src/contrast/assess_extensions/py39/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/configuration/__init__.py` & `contrast_agent-8.3.0/src/contrast/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/configuration/agent_config.py` & `contrast_agent-8.3.0/src/contrast/configuration/agent_config.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/configuration/api.py` & `contrast_agent-8.3.0/src/contrast/configuration/api.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/configuration/application.py` & `contrast_agent-8.3.0/src/contrast/configuration/application.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/configuration/assess.py` & `contrast_agent-8.3.0/src/contrast/configuration/assess.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/configuration/config_builder.py` & `contrast_agent-8.3.0/src/contrast/configuration/config_builder.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/configuration/config_option.py` & `contrast_agent-8.3.0/src/contrast/configuration/config_option.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/configuration/inventory.py` & `contrast_agent-8.3.0/src/contrast/configuration/inventory.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/configuration/protect.py` & `contrast_agent-8.3.0/src/contrast/configuration/protect.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/configuration/server.py` & `contrast_agent-8.3.0/src/contrast/configuration/server.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/loader/sitecustomize.py` & `contrast_agent-8.3.0/src/contrast/loader/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/patches/__init__.py` & `contrast_agent-8.3.0/src/contrast/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/patches/cgi_patch.py` & `contrast_agent-8.3.0/src/contrast/patches/cgi_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/patches/concurrent_futures_thread_patch.py` & `contrast_agent-8.3.0/src/contrast/patches/concurrent_futures_thread_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/patches/cs_io.py` & `contrast_agent-8.3.0/src/contrast/patches/cs_io.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/patches/cs_str.py` & `contrast_agent-8.3.0/src/contrast/patches/cs_str.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/patches/databases/dbapi2.py` & `contrast_agent-8.3.0/src/contrast/patches/databases/dbapi2.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/patches/databases/mysql_connector_patch.py` & `contrast_agent-8.3.0/src/contrast/patches/databases/mysql_connector_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/patches/databases/psycopg2_patch.py` & `contrast_agent-8.3.0/src/contrast/patches/databases/psycopg2_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/patches/databases/pymysql_patch.py` & `contrast_agent-8.3.0/src/contrast/patches/databases/pymysql_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/patches/databases/sqlalchemy_patch.py` & `contrast_agent-8.3.0/src/contrast/patches/databases/sqlalchemy_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/patches/databases/sqlite3_patch.py` & `contrast_agent-8.3.0/src/contrast/patches/databases/sqlite3_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/patches/encodings_patch.py` & `contrast_agent-8.3.0/src/contrast/patches/encodings_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/patches/exec_and_eval.py` & `contrast_agent-8.3.0/src/contrast/patches/exec_and_eval.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/patches/frameworks/bottle_patches.py` & `contrast_agent-8.3.0/src/contrast/patches/frameworks/bottle_patches.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/patches/frameworks/django_patches.py` & `contrast_agent-8.3.0/src/contrast/patches/frameworks/django_patches.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/patches/frameworks/drf_patches.py` & `contrast_agent-8.3.0/src/contrast/patches/frameworks/drf_patches.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/patches/frameworks/falcon_patches.py` & `contrast_agent-8.3.0/src/contrast/patches/frameworks/falcon_patches.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/patches/frameworks/flask_and_quart_patches.py` & `contrast_agent-8.3.0/src/contrast/patches/frameworks/flask_and_quart_patches.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/patches/frameworks/pyramid_patch.py` & `contrast_agent-8.3.0/src/contrast/patches/frameworks/pyramid_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/patches/frameworks/starlette_patches.py` & `contrast_agent-8.3.0/src/contrast/patches/frameworks/starlette_patches.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/patches/genshi_patch.py` & `contrast_agent-8.3.0/src/contrast/patches/genshi_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/patches/import_patch.py` & `contrast_agent-8.3.0/src/contrast/patches/import_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/patches/lxml_patch.py` & `contrast_agent-8.3.0/src/contrast/patches/lxml_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/patches/middleware/aiohttp.py` & `contrast_agent-8.3.0/src/contrast/patches/middleware/aiohttp.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/patches/middleware/common.py` & `contrast_agent-8.3.0/src/contrast/patches/middleware/common.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/patches/middleware/django.py` & `contrast_agent-8.3.0/src/contrast/patches/middleware/django.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/patches/middleware/mod_wsgi.py` & `contrast_agent-8.3.0/src/contrast/patches/middleware/mod_wsgi.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/patches/operator.py` & `contrast_agent-8.3.0/src/contrast/patches/operator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/patches/pathlib_patch.py` & `contrast_agent-8.3.0/src/contrast/patches/pathlib_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/patches/re_patch.py` & `contrast_agent-8.3.0/src/contrast/patches/re_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/patches/str_new.py` & `contrast_agent-8.3.0/src/contrast/patches/str_new.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/patches/sys_patch.py` & `contrast_agent-8.3.0/src/contrast/patches/sys_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/patches/threading_patch.py` & `contrast_agent-8.3.0/src/contrast/patches/threading_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/patches/urllib_patch.py` & `contrast_agent-8.3.0/src/contrast/patches/urllib_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/patches/utils.py` & `contrast_agent-8.3.0/src/contrast/patches/utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/policy/deadzones.py` & `contrast_agent-8.3.0/src/contrast/policy/deadzones.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/policy/propagators/codecs.py` & `contrast_agent-8.3.0/src/contrast/policy/propagators/codecs.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/policy/propagators/encodings.py` & `contrast_agent-8.3.0/src/contrast/policy/propagators/encodings.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/policy/propagators/frameworks.py` & `contrast_agent-8.3.0/src/contrast/policy/propagators/frameworks.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/policy/propagators/paths.py` & `contrast_agent-8.3.0/src/contrast/policy/propagators/paths.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/policy/propagators/re.py` & `contrast_agent-8.3.0/src/contrast/policy/propagators/re.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/policy/propagators/serialize.py` & `contrast_agent-8.3.0/src/contrast/policy/propagators/serialize.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/policy/propagators/string.py` & `contrast_agent-8.3.0/src/contrast/policy/propagators/string.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/policy/sources/asgi.py` & `contrast_agent-8.3.0/src/contrast/policy/sources/asgi.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/policy/sources/cgi.py` & `contrast_agent-8.3.0/src/contrast/policy/sources/cgi.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/policy/sources/django.py` & `contrast_agent-8.3.0/src/contrast/policy/sources/django.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/policy/sources/falcon.py` & `contrast_agent-8.3.0/src/contrast/policy/sources/falcon.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/policy/sources/flask.py` & `contrast_agent-8.3.0/src/contrast/policy/sources/flask.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/policy/sources/quart.py` & `contrast_agent-8.3.0/src/contrast/policy/sources/quart.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/policy/sources/webob.py` & `contrast_agent-8.3.0/src/contrast/policy/sources/webob.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/policy/triggers/__init__.py` & `contrast_agent-8.3.0/src/contrast/policy/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/policy/triggers/cmd_injection.py` & `contrast_agent-8.3.0/src/contrast/policy/triggers/cmd_injection.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/policy/triggers/crypto.py` & `contrast_agent-8.3.0/src/contrast/policy/triggers/crypto.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/policy/triggers/httponly.py` & `contrast_agent-8.3.0/src/contrast/policy/triggers/httponly.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/policy/triggers/nosql_injection.py` & `contrast_agent-8.3.0/src/contrast/policy/triggers/nosql_injection.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/policy/triggers/path_traversal.py` & `contrast_agent-8.3.0/src/contrast/policy/triggers/path_traversal.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/policy/triggers/prompt_injection.py` & `contrast_agent-8.3.0/src/contrast/policy/triggers/prompt_injection.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/policy/triggers/redos.py` & `contrast_agent-8.3.0/src/contrast/policy/triggers/redos.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/policy/triggers/reflected_xss.py` & `contrast_agent-8.3.0/src/contrast/policy/triggers/reflected_xss.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/policy/triggers/secure_flag_missing.py` & `contrast_agent-8.3.0/src/contrast/policy/triggers/secure_flag_missing.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/policy/triggers/session_rewriting.py` & `contrast_agent-8.3.0/src/contrast/policy/triggers/session_rewriting.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/policy/triggers/session_timeout.py` & `contrast_agent-8.3.0/src/contrast/policy/triggers/session_timeout.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/policy/triggers/sql_injection.py` & `contrast_agent-8.3.0/src/contrast/policy/triggers/sql_injection.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/policy/triggers/ssrf.py` & `contrast_agent-8.3.0/src/contrast/policy/triggers/ssrf.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/policy/triggers/trust_boundary_violation.py` & `contrast_agent-8.3.0/src/contrast/policy/triggers/trust_boundary_violation.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/policy/triggers/unsafe_code_execution.py` & `contrast_agent-8.3.0/src/contrast/policy/triggers/unsafe_code_execution.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/policy/triggers/untrusted_deserialization.py` & `contrast_agent-8.3.0/src/contrast/policy/triggers/untrusted_deserialization.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/policy/triggers/unvalidated_redirect.py` & `contrast_agent-8.3.0/src/contrast/policy/triggers/unvalidated_redirect.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/policy/triggers/xpath_injection.py` & `contrast_agent-8.3.0/src/contrast/policy/triggers/xpath_injection.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/policy/triggers/xxe.py` & `contrast_agent-8.3.0/src/contrast/policy/triggers/xxe.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/reporting/activity_masker.py` & `contrast_agent-8.3.0/src/contrast/reporting/activity_masker.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/reporting/reporting_client.py` & `contrast_agent-8.3.0/src/contrast/reporting/reporting_client.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/reporting/request_audit.py` & `contrast_agent-8.3.0/src/contrast/reporting/request_audit.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/__init__.py` & `contrast_agent-8.3.0/src/contrast/reporting/teamserver_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/_traces.py` & `contrast_agent-8.3.0/src/contrast/reporting/teamserver_messages/_traces.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/agent_startup.py` & `contrast_agent-8.3.0/src/contrast/reporting/teamserver_messages/agent_startup.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/application_activity.py` & `contrast_agent-8.3.0/src/contrast/reporting/teamserver_messages/application_activity.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/application_inventory.py` & `contrast_agent-8.3.0/src/contrast/reporting/teamserver_messages/application_inventory.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/application_update.py` & `contrast_agent-8.3.0/src/contrast/reporting/teamserver_messages/application_update.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/base_ts_message.py` & `contrast_agent-8.3.0/src/contrast/reporting/teamserver_messages/base_ts_message.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/effective_config.py` & `contrast_agent-8.3.0/src/contrast/reporting/teamserver_messages/effective_config.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/heartbeat.py` & `contrast_agent-8.3.0/src/contrast/reporting/teamserver_messages/heartbeat.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/library_usage.py` & `contrast_agent-8.3.0/src/contrast/reporting/teamserver_messages/library_usage.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/observed_route.py` & `contrast_agent-8.3.0/src/contrast/reporting/teamserver_messages/observed_route.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/preflight.py` & `contrast_agent-8.3.0/src/contrast/reporting/teamserver_messages/preflight.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/server_activity.py` & `contrast_agent-8.3.0/src/contrast/reporting/teamserver_messages/server_activity.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/reporting/teamserver_responses/__init__.py` & `contrast_agent-8.3.0/src/contrast/reporting/teamserver_responses/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/reporting/teamserver_responses/application_settings.py` & `contrast_agent-8.3.0/src/contrast/reporting/teamserver_responses/application_settings.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/reporting/teamserver_responses/ng_application_settings.py` & `contrast_agent-8.3.0/src/contrast/reporting/teamserver_responses/ng_application_settings.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/reporting/teamserver_responses/ng_server_settings.py` & `contrast_agent-8.3.0/src/contrast/reporting/teamserver_responses/ng_server_settings.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/reporting/teamserver_responses/protect_rule.py` & `contrast_agent-8.3.0/src/contrast/reporting/teamserver_responses/protect_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/reporting/teamserver_responses/sampling.py` & `contrast_agent-8.3.0/src/contrast/reporting/teamserver_responses/sampling.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/reporting/teamserver_responses/server_settings.py` & `contrast_agent-8.3.0/src/contrast/reporting/teamserver_responses/server_settings.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/scripts/fix_interpreter_permissions.py` & `contrast_agent-8.3.0/src/contrast/scripts/fix_interpreter_permissions.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/scripts/propagator_check.py` & `contrast_agent-8.3.0/src/contrast/scripts/propagator_check.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/scripts/runner.py` & `contrast_agent-8.3.0/src/contrast/scripts/runner.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/scripts/validate_config.py` & `contrast_agent-8.3.0/src/contrast/scripts/validate_config.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/utils/assess/duck_utils.py` & `contrast_agent-8.3.0/src/contrast/utils/assess/duck_utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/utils/assess/formatting/base.py` & `contrast_agent-8.3.0/src/contrast/utils/assess/formatting/base.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/utils/assess/formatting/tokenize_cformat.py` & `contrast_agent-8.3.0/src/contrast/utils/assess/formatting/tokenize_cformat.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/utils/assess/formatting/tokenize_format.py` & `contrast_agent-8.3.0/src/contrast/utils/assess/formatting/tokenize_format.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/utils/assess/stream_utils.py` & `contrast_agent-8.3.0/src/contrast/utils/assess/stream_utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/utils/assess/tag_utils.py` & `contrast_agent-8.3.0/src/contrast/utils/assess/tag_utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/utils/assess/tracking_util.py` & `contrast_agent-8.3.0/src/contrast/utils/assess/tracking_util.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/utils/base64_utils.py` & `contrast_agent-8.3.0/src/contrast/utils/base64_utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/utils/configuration_utils.py` & `contrast_agent-8.3.0/src/contrast/utils/configuration_utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/utils/context_tracker.py` & `contrast_agent-8.3.0/src/contrast/utils/context_tracker.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/utils/decorators.py` & `contrast_agent-8.3.0/src/contrast/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/utils/deprecated_middleware.py` & `contrast_agent-8.3.0/src/contrast/utils/deprecated_middleware.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/utils/environ.py` & `contrast_agent-8.3.0/src/contrast/utils/environ.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/utils/exceptions/wrong_django_middleware_exception.py` & `contrast_agent-8.3.0/src/contrast/utils/exceptions/wrong_django_middleware_exception.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/utils/ignored_modules.py` & `contrast_agent-8.3.0/src/contrast/utils/ignored_modules.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/utils/library_reader/library_reader.py` & `contrast_agent-8.3.0/src/contrast/utils/library_reader/library_reader.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/utils/library_reader/patched_state.py` & `contrast_agent-8.3.0/src/contrast/utils/library_reader/patched_state.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/utils/library_reader/utils.py` & `contrast_agent-8.3.0/src/contrast/utils/library_reader/utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/utils/loggers/structlog.py` & `contrast_agent-8.3.0/src/contrast/utils/loggers/structlog.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,14 +124,15 @@
             structlog.processors.CallsiteParameterAdder(
                 [
                     structlog.processors.CallsiteParameter.PROCESS,
                     structlog.processors.CallsiteParameter.FILENAME,
                     structlog.processors.CallsiteParameter.FUNC_NAME,
                     structlog.processors.CallsiteParameter.LINENO,
                     structlog.processors.CallsiteParameter.THREAD,
+                    structlog.processors.CallsiteParameter.THREAD_NAME,
                 ],
                 additional_ignores=[
                     "contrast_vendor.structlog",
                     "contrast.utils.decorators",
                 ],
             ),
             rename_key_for_bunyan("process", "pid"),
```

### Comparing `contrast_agent-8.2.0/src/contrast/utils/module_parser.py` & `contrast_agent-8.3.0/src/contrast/utils/module_parser.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/utils/namespace.py` & `contrast_agent-8.3.0/src/contrast/utils/namespace.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/utils/object_utils.py` & `contrast_agent-8.3.0/src/contrast/utils/object_utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/utils/patch_utils.py` & `contrast_agent-8.3.0/src/contrast/utils/patch_utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/utils/pattern_builder.py` & `contrast_agent-8.3.0/src/contrast/utils/pattern_builder.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/utils/safe_import.py` & `contrast_agent-8.3.0/src/contrast/utils/safe_import.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/utils/singleton.py` & `contrast_agent-8.3.0/src/contrast/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/utils/stdlib_modules.py` & `contrast_agent-8.3.0/src/contrast/utils/stdlib_modules.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/utils/string_utils.py` & `contrast_agent-8.3.0/src/contrast/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast/wsgi/middleware.py` & `contrast_agent-8.3.0/src/contrast/wsgi/middleware.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 )
 from contrast.agent.middlewares.environ_tracker import track_environ_sources
 from contrast.utils.decorators import cached_property
 from contrast.utils.safe_import import safe_import_list
 from contrast.utils.assess.duck_utils import safe_getattr_list
 
 from contrast_vendor import structlog as logging
-from contrast.utils import Profiler
+from contrast.utils.monitoring import Profiler, tracer
 
 logger = logging.getLogger("contrast")
 DEFAULT_WSGI_NAME = "wsgi_app"
 
 
 @functools.lru_cache(maxsize=1)
 def _get_flask_types():
@@ -68,21 +68,24 @@
     def __call__(self, environ, start_response):
         if request_state.get_request_id() is not None:
             # This can happen if a single app is wrapped by multiple instances of the
             # middleware (usually caused by automatic instrumentation)
             logger.debug("Detected preexisting request_id - passing through")
             return self.wsgi_app(environ, start_response)
 
-        self.request_path = environ.get("PATH_INFO", "")
+        request_path = environ.get("PATH_INFO", "")
 
         # the request_id context manager must come first!
         with request_state.request_id_context(), Profiler(
-            self.request_path
+            request_path,
         ), log_request_start_and_end(
-            environ.get("REQUEST_METHOD", ""), self.request_path
+            environ.get("REQUEST_METHOD", ""),
+            request_path,
+        ), tracer(
+            request_path,
         ):
             context = self.should_analyze_request(environ)
             if context:
                 with contrast.CS__CONTEXT_TRACKER.lifespan(context):
                     return self.call_with_agent(context, environ, start_response)
 
             return self.call_without_agent(environ, start_response)
@@ -98,49 +101,26 @@
             with scope.pop_contrast_scope():
                 response = webob_request.get_response(self.wsgi_app)
 
             context.extract_response_to_context(response)
 
             self.postfilter(context)
             self.check_for_blocked(context)
-            self.swap_environ_path(environ)  # should not be moved to finally
 
             return response(environ, start_response)
 
         finally:
             self.handle_ensure(context, context.request)
             if self.settings.is_assess_enabled():
                 contrast.STRING_TRACKER.ageoff()
 
-    def swap_environ_path(self, environ):
-        """
-        See PYT-1742.
-
-        Special behavior required for bottle+django to account for an unfortunate
-        encoding behavior.
-
-        In bottle, it occurs here:
-        bottle.py:
-        def _handle(self, environ):
-            ...
-            environ['PATH_INFO'] = path.encode('latin1').decode('utf8')
-            ...
-
-        This casing occurs after the application code is called, and will result in a
-        `UnicodeEncodeError` when the agent attempts to access request.path.
-        As a workaround, we store the original PATH_INFO - before bottle changed it
-        during calling app code - and use it for agent purposes.
-        """
-        environ["PATH_INFO"] = self.request_path
-
     def call_without_agent(self, environ, start_response):
         """
         Normal without middleware call
         """
-        super().call_without_agent()
         with scope.contrast_scope():
             return self.wsgi_app(environ, start_response)
 
     @cached_property
     def trigger_node(self):
         """
         WSGI-specific trigger node used by reflected xss postfilter rule
```

### Comparing `contrast_agent-8.2.0/src/contrast_agent.egg-info/SOURCES.txt` & `contrast_agent-8.3.0/src/contrast_agent.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -516,19 +516,19 @@
 src/contrast/utils/decorators.py
 src/contrast/utils/deprecated_middleware.py
 src/contrast/utils/digest_utils.py
 src/contrast/utils/environ.py
 src/contrast/utils/ignored_modules.py
 src/contrast/utils/locale.py
 src/contrast/utils/module_parser.py
+src/contrast/utils/monitoring.py
 src/contrast/utils/namespace.py
 src/contrast/utils/object_utils.py
 src/contrast/utils/patch_utils.py
 src/contrast/utils/pattern_builder.py
-src/contrast/utils/profiler.py
 src/contrast/utils/safe_import.py
 src/contrast/utils/singleton.py
 src/contrast/utils/stack_trace_utils.py
 src/contrast/utils/stdlib_modules.py
 src/contrast/utils/string_utils.py
 src/contrast/utils/timer.py
 src/contrast/utils/assess/__init__.py
```

### Comparing `contrast_agent-8.2.0/src/contrast_rewriter/__init__.py` & `contrast_agent-8.3.0/src/contrast_rewriter/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/__init__.py` & `contrast_agent-8.3.0/src/contrast_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/LICENSE` & `contrast_agent-8.3.0/src/contrast_vendor/importlib_metadata/LICENSE`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/__init__.py` & `contrast_agent-8.3.0/src/contrast_vendor/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/_adapters.py` & `contrast_agent-8.3.0/src/contrast_vendor/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/_collections.py` & `contrast_agent-8.3.0/src/contrast_vendor/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/_compat.py` & `contrast_agent-8.3.0/src/contrast_vendor/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/_functools.py` & `contrast_agent-8.3.0/src/contrast_vendor/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/_itertools.py` & `contrast_agent-8.3.0/src/contrast_vendor/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/_meta.py` & `contrast_agent-8.3.0/src/contrast_vendor/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/_text.py` & `contrast_agent-8.3.0/src/contrast_vendor/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/compat/py39.py` & `contrast_agent-8.3.0/src/contrast_vendor/importlib_metadata/compat/py39.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/isort/LICENSE` & `contrast_agent-8.3.0/src/contrast_vendor/isort/LICENSE`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/py27.py` & `contrast_agent-8.3.0/src/contrast_vendor/isort/stdlibs/py27.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/py310.py` & `contrast_agent-8.3.0/src/contrast_vendor/isort/stdlibs/py310.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/py311.py` & `contrast_agent-8.3.0/src/contrast_vendor/isort/stdlibs/py311.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/py312.py` & `contrast_agent-8.3.0/src/contrast_vendor/isort/stdlibs/py312.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/py36.py` & `contrast_agent-8.3.0/src/contrast_vendor/isort/stdlibs/py36.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/py37.py` & `contrast_agent-8.3.0/src/contrast_vendor/isort/stdlibs/py37.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/py38.py` & `contrast_agent-8.3.0/src/contrast_vendor/isort/stdlibs/py38.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/py39.py` & `contrast_agent-8.3.0/src/contrast_vendor/isort/stdlibs/py39.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/ported_cpython_code/PYTHON_SOFTWARE_FOUNDATION_LICENSE` & `contrast_agent-8.3.0/src/contrast_vendor/ported_cpython_code/PYTHON_SOFTWARE_FOUNDATION_LICENSE`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/ported_cpython_code/import_functionality.py` & `contrast_agent-8.3.0/src/contrast_vendor/ported_cpython_code/import_functionality.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/LICENSE` & `contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/LICENSE`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/__init__.py` & `contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/comments.py` & `contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/comments.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/compat.py` & `contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/compat.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/composer.py` & `contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/constructor.py` & `contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/cyaml.py` & `contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/dumper.py` & `contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/emitter.py` & `contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/error.py` & `contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/error.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/events.py` & `contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/events.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/loader.py` & `contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/main.py` & `contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/main.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/nodes.py` & `contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/parser.py` & `contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/reader.py` & `contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/representer.py` & `contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/resolver.py` & `contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/scalarbool.py` & `contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/scalarbool.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/scalarfloat.py` & `contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/scalarfloat.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/scalarint.py` & `contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/scalarint.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/scalarstring.py` & `contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/scalarstring.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/scanner.py` & `contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/serializer.py` & `contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/tag.py` & `contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/tag.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/timestamp.py` & `contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/timestamp.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/tokens.py` & `contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/util.py` & `contrast_agent-8.3.0/src/contrast_vendor/ruamel/yaml/util.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/structlog/LICENSE-APACHE` & `contrast_agent-8.3.0/src/contrast_vendor/structlog/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/structlog/LICENSE-MIT` & `contrast_agent-8.3.0/src/contrast_vendor/structlog/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/structlog/__init__.py` & `contrast_agent-8.3.0/src/contrast_vendor/structlog/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/structlog/_base.py` & `contrast_agent-8.3.0/src/contrast_vendor/structlog/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,17 +47,15 @@
         context: Context,
     ):
         self._logger = logger
         self._processors = processors
         self._context = context
 
     def __repr__(self) -> str:
-        return "<{}(context={!r}, processors={!r})>".format(
-            self.__class__.__name__, self._context, self._processors
-        )
+        return f"<{self.__class__.__name__}(context={self._context!r}, processors={self._processors!r})>"
 
     def __eq__(self, other: object) -> bool:
         try:
             return self._context == other._context  # type: ignore[attr-defined]
         except AttributeError:
             return False
```

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/structlog/_config.py` & `contrast_agent-8.3.0/src/contrast_vendor/structlog/_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,17 +59,17 @@
     Global defaults.
     """
 
     is_configured: bool = False
     default_processors: Iterable[Processor] = _BUILTIN_DEFAULT_PROCESSORS[:]
     default_context_class: type[Context] = _BUILTIN_DEFAULT_CONTEXT_CLASS
     default_wrapper_class: Any = _BUILTIN_DEFAULT_WRAPPER_CLASS
-    logger_factory: Callable[
-        ..., WrappedLogger
-    ] = _BUILTIN_DEFAULT_LOGGER_FACTORY
+    logger_factory: Callable[..., WrappedLogger] = (
+        _BUILTIN_DEFAULT_LOGGER_FACTORY
+    )
     cache_logger_on_first_use: bool = _BUILTIN_CACHE_LOGGER_ON_FIRST_USE
 
 
 _CONFIG = _Configuration()
 """
 Global defaults used when arguments to `wrap_logger` are omitted.
 """
```

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/structlog/_frames.py` & `contrast_agent-8.3.0/src/contrast_vendor/structlog/_frames.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,18 +51,18 @@
         _getframe:
             Callable to find current frame. Only for testing to avoid
             monkeypatching of sys._getframe.
 
     Returns:
         tuple of (frame, name)
     """
-    ignores = ["structlog"] + (additional_ignores or [])
+    ignores = tuple(["structlog"] + (additional_ignores or []))
     f = _ASYNC_CALLING_STACK.get(_getframe())
     name = f.f_globals.get("__name__") or "?"
-    while any(tuple(name.startswith(i) for i in ignores)):
+    while name.startswith(ignores):
         if f.f_back is None:
             name = "?"
             break
         f = f.f_back
         name = f.f_globals.get("__name__") or "?"
     return f, name
```

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/structlog/_generic.py` & `contrast_agent-8.3.0/src/contrast_vendor/structlog/_generic.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/structlog/_greenlets.py` & `contrast_agent-8.3.0/src/contrast_vendor/structlog/_greenlets.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/structlog/_log_levels.py` & `contrast_agent-8.3.0/src/contrast_vendor/structlog/_log_levels.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/structlog/_native.py` & `contrast_agent-8.3.0/src/contrast_vendor/structlog/_native.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,16 +206,15 @@
     meths["afatal"] = meths["aerror"]
     meths["warn"] = meths["warning"]
     meths["awarn"] = meths["awarning"]
     meths["msg"] = meths["info"]
     meths["amsg"] = meths["ainfo"]
 
     return type(
-        "BoundLoggerFilteringAt%s"
-        % (LEVEL_TO_NAME.get(min_level, "Notset").capitalize()),
+        f"BoundLoggerFilteringAt{LEVEL_TO_NAME.get(min_level, 'Notset').capitalize()}",
         (BoundLoggerBase,),
         meths,
     )
 
 
 # Pre-create all possible filters to make them pickleable.
 BoundLoggerFilteringAtNotset = _make_filtering_bound_logger(NOTSET)
```

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/structlog/_output.py` & `contrast_agent-8.3.0/src/contrast_vendor/structlog/_output.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 import sys
 import threading
 
 from pickle import PicklingError
 from sys import stderr, stdout
 from typing import IO, Any, BinaryIO, TextIO
 
-from contrast_vendor.structlog._utils import until_not_interrupted
-
 
 WRITE_LOCKS: dict[IO[Any], threading.Lock] = {}
 
 
 def _get_lock_for_file(file: IO[Any]) -> threading.Lock:
     lock = WRITE_LOCKS.get(file)
     if lock is None:
@@ -105,15 +103,15 @@
 
     def msg(self, message: str) -> None:
         """
         Print *message*.
         """
         f = self._file if self._file is not stdout else None
         with self._lock:
-            until_not_interrupted(print, message, file=f, flush=True)
+            print(message, file=f, flush=True)
 
     log = debug = info = warn = warning = msg
     fatal = failure = err = error = critical = exception = msg
 
 
 class PrintLoggerFactory:
     r"""
@@ -212,16 +210,16 @@
         return f"<WriteLogger(file={self._file!r})>"
 
     def msg(self, message: str) -> None:
         """
         Write and flush *message*.
         """
         with self._lock:
-            until_not_interrupted(self._write, message + "\n")
-            until_not_interrupted(self._flush)
+            self._write(message + "\n")
+            self._flush()
 
     log = debug = info = warn = warning = msg
     fatal = failure = err = error = critical = exception = msg
 
 
 class WriteLoggerFactory:
     r"""
@@ -253,14 +251,15 @@
 
     Useful if you follow `current logging best practices
     <logging-best-practices>` together with a formatter that returns bytes
     (e.g. `orjson <https://github.com/ijl/orjson>`_).
 
     .. versionadded:: 20.2.0
     """
+
     __slots__ = ("_file", "_write", "_flush", "_lock")
 
     def __init__(self, file: BinaryIO | None = None):
         self._file = file or sys.stdout.buffer
         self._write = self._file.write
         self._flush = self._file.flush
 
@@ -315,16 +314,16 @@
         return f"<BytesLogger(file={self._file!r})>"
 
     def msg(self, message: bytes) -> None:
         """
         Write *message*.
         """
         with self._lock:
-            until_not_interrupted(self._write, message + b"\n")
-            until_not_interrupted(self._flush)
+            self._write(message + b"\n")
+            self._flush()
 
     log = debug = info = warn = warning = msg
     fatal = failure = err = error = critical = exception = msg
 
 
 class BytesLoggerFactory:
     r"""
@@ -335,14 +334,15 @@
     Args:
         file: File to print to. (default: `sys.stdout`\ ``.buffer``)
 
     Positional arguments are silently ignored.
 
     .. versionadded:: 20.2.0
     """
+
     __slots__ = ("_file",)
 
     def __init__(self, file: BinaryIO | None = None):
         self._file = file
 
     def __call__(self, *args: Any) -> BytesLogger:
         return BytesLogger(self._file)
```

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/structlog/contextvars.py` & `contrast_agent-8.3.0/src/contrast_vendor/structlog/contextvars.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 
 from .typing import BindableLogger, EventDict, WrappedLogger
 
 
 STRUCTLOG_KEY_PREFIX = "structlog_"
 STRUCTLOG_KEY_PREFIX_LEN = len(STRUCTLOG_KEY_PREFIX)
 
-_ASYNC_CALLING_STACK: contextvars.ContextVar[
-    FrameType
-] = contextvars.ContextVar("_ASYNC_CALLING_STACK")
+_ASYNC_CALLING_STACK: contextvars.ContextVar[FrameType] = (
+    contextvars.ContextVar("_ASYNC_CALLING_STACK")
+)
 
 # For proper isolation, we have to use a dict of ContextVars instead of a
 # single ContextVar with a dict.
 # See https://github.com/hynek/structlog/pull/302 for details.
 _CONTEXT_VARS: dict[str, contextvars.ContextVar[Any]] = {}
```

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/structlog/dev.py` & `contrast_agent-8.3.0/src/contrast_vendor/structlog/dev.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the MIT License.  See the LICENSE file in the root of this
 # repository for complete details.
 
 """
 Helpers that make development with *structlog* more pleasant.
 
-See also the narrative documentation in `development`.
+See also the narrative documentation in `console-output`.
 """
 
 from __future__ import annotations
 
 import shutil
 import sys
 import warnings
@@ -279,26 +279,37 @@
             A dictionary of level names to styles that are applied to it. If
             None, the level is formatted as a plain ``[level]``.
 
         reset_style:
             What to use to reset the style after the level name. Ignored if
             if *level_styles* is None.
 
+        width:
+            The width to pad the level to. If 0, no padding is done.
+
     .. versionadded:: 23.3.0
+    .. versionadded:: 24.2.0 *width*
     """
 
     level_styles: dict[str, str] | None
     reset_style: str
     width: int
 
-    def __init__(self, level_styles: dict[str, str], reset_style: str) -> None:
+    def __init__(
+        self,
+        level_styles: dict[str, str],
+        reset_style: str,
+        width: int | None = None,
+    ) -> None:
         self.level_styles = level_styles
         if level_styles:
-            self.width = len(
-                max(self.level_styles.keys(), key=lambda e: len(e))
+            self.width = (
+                0
+                if width == 0
+                else len(max(self.level_styles.keys(), key=lambda e: len(e)))
             )
             self.reset_style = reset_style
         else:
             self.width = 0
             self.reset_style = ""
 
     def __call__(self, key: str, value: object) -> str:
@@ -417,15 +428,15 @@
 elif better_exceptions is not None:
     default_exception_formatter = better_traceback
 else:
     default_exception_formatter = plain_traceback
 
 
 class ConsoleRenderer:
-    """
+    r"""
     Render ``event_dict`` nicely aligned, possibly in colors, and ordered.
 
     If ``event_dict`` contains a true-ish ``exc_info`` key, it will be rendered
     *after* the log line. If Rich_ or better-exceptions_ are present, in colors
     and with extra context.
 
     Args:
@@ -450,16 +461,16 @@
         force_colors:
             Force colors even for non-tty destinations. Use this option if your
             logs are stored in a file that is meant to be streamed to the
             console. Only meaningful on Windows. Ignored if *columns* are
             passed.
 
         repr_native_str:
-            When `True`, `repr` is also applied to ``str``s. The ``event`` key
-            is *never* `repr` -ed. Ignored if *columns* are passed.
+            When `True`, `repr` is also applied to ``str``\ s. The ``event``
+            key is *never* `repr` -ed. Ignored if *columns* are passed.
 
         level_styles:
             When present, use these styles for colors. This must be a dict from
             level names (strings) to Colorama styles. The default can be
             obtained by calling `ConsoleRenderer.get_default_level_styles`.
             Ignored when *columns* are passed.
 
@@ -481,14 +492,18 @@
             *columns* are passed.
 
         timestamp_key:
             The key to look for timestamp of the log message. Needed when you
             rename it e.g. using `structlog.processors.EventRenamer`. Ignored
             if *columns* are passed.
 
+        pad_level:
+            Whether to pad log level with blanks to the longest amongst all
+            level label.
+
     Requires the Colorama_ package if *colors* is `True` **on Windows**.
 
     Raises:
         ValueError: If there's not exactly one default column formatter.
 
     .. _Colorama: https://pypi.org/project/colorama/
     .. _better-exceptions: https://pypi.org/project/better-exceptions/
@@ -520,28 +535,30 @@
        The colors keyword now defaults to True on non-Windows systems, and
        either True or False in Windows depending on whether Colorama is
        installed.
     .. versionadded:: 21.3.0 *sort_keys*
     .. versionadded:: 22.1.0 *event_key*
     .. versionadded:: 23.2.0 *timestamp_key*
     .. versionadded:: 23.3.0 *columns*
+    .. versionadded:: 24.2.0 *pad_level*
     """
 
-    def __init__(  # noqa: PLR0912
+    def __init__(  # noqa: PLR0912, PLR0915
         self,
         pad_event: int = _EVENT_WIDTH,
         colors: bool = _has_colors,
         force_colors: bool = False,
         repr_native_str: bool = False,
         level_styles: Styles | None = None,
         exception_formatter: ExceptionRenderer = default_exception_formatter,
         sort_keys: bool = True,
         event_key: str = "event",
         timestamp_key: str = "timestamp",
         columns: list[Column] | None = None,
+        pad_level: bool = True,
     ):
         self._exception_formatter = exception_formatter
         self._sort_keys = sort_keys
 
         if columns is not None:
             to_warn = []
 
@@ -641,28 +658,30 @@
             value_style=styles.bright + styles.logger_name,
             reset_style=styles.reset,
             value_repr=str,
             prefix="[",
             postfix="]",
         )
 
+        level_width = 0 if not pad_level else None
+
         self._columns = [
             Column(
                 timestamp_key,
                 KeyValueColumnFormatter(
                     key_style=None,
                     value_style=styles.timestamp,
                     reset_style=styles.reset,
                     value_repr=str,
                 ),
             ),
             Column(
                 "level",
                 LogLevelColumnFormatter(
-                    level_to_color, reset_style=styles.reset
+                    level_to_color, reset_style=styles.reset, width=level_width
                 ),
             ),
             Column(
                 event_key,
                 KeyValueColumnFormatter(
                     key_style=None,
                     value_style=styles.bright,
```

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/structlog/processors.py` & `contrast_agent-8.3.0/src/contrast_vendor/structlog/processors.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 Processors useful regardless of the logging framework.
 """
 
 from __future__ import annotations
 
 import datetime
 import enum
-import inspect
 import json
 import logging
 import operator
 import os
 import sys
 import threading
 import time
 
+from types import FrameType
 from typing import (
     Any,
     Callable,
     ClassVar,
     Collection,
     NamedTuple,
     Sequence,
@@ -132,15 +132,15 @@
 
         bool_as_flag:
             When ``True``, render ``{"flag": True}`` as ``flag``, instead of
             ``flag=true``. ``{"flag": False}`` is always rendered as
             ``flag=false``.
 
     Raises:
-        ValueError: If a key contains non printable or space characters.
+        ValueError: If a key contains non-printable or whitespace characters.
 
     .. versionadded:: 21.5.0
     """
 
     def __init__(
         self,
         sort_keys: bool = False,
@@ -166,17 +166,24 @@
 
             if isinstance(value, bool):
                 if self.bool_as_flag and value:
                     elements.append(f"{key}")
                     continue
                 value = "true" if value else "false"
 
-            value = f"{value}".replace('"', '\\"')
+            value = str(value)
+            backslashes_need_escaping = (
+                " " in value or "=" in value or '"' in value
+            )
+            if backslashes_need_escaping and "\\" in value:
+                value = value.replace("\\", "\\\\")
+
+            value = value.replace('"', '\\"').replace("\n", "\\n")
 
-            if " " in value or "=" in value:
+            if backslashes_need_escaping:
                 value = f'"{value}"'
 
             elements.append(f"{key}={value}")
 
         return " ".join(elements)
 
 
@@ -713,14 +720,50 @@
     THREAD_NAME = "thread_name"
     #: The ID of the process the callsite was executed in.
     PROCESS = "process"
     #: The name of the process the callsite was executed in.
     PROCESS_NAME = "process_name"
 
 
+def _get_callsite_pathname(module: str, frame: FrameType) -> Any:
+    return frame.f_code.co_filename
+
+
+def _get_callsite_filename(module: str, frame: FrameType) -> Any:
+    return os.path.basename(frame.f_code.co_filename)
+
+
+def _get_callsite_module(module: str, frame: FrameType) -> Any:
+    return os.path.splitext(os.path.basename(frame.f_code.co_filename))[0]
+
+
+def _get_callsite_func_name(module: str, frame: FrameType) -> Any:
+    return frame.f_code.co_name
+
+
+def _get_callsite_lineno(module: str, frame: FrameType) -> Any:
+    return frame.f_lineno
+
+
+def _get_callsite_thread(module: str, frame: FrameType) -> Any:
+    return threading.get_ident()
+
+
+def _get_callsite_thread_name(module: str, frame: FrameType) -> Any:
+    return threading.current_thread().name
+
+
+def _get_callsite_process(module: str, frame: FrameType) -> Any:
+    return os.getpid()
+
+
+def _get_callsite_process_name(module: str, frame: FrameType) -> Any:
+    return get_processname()
+
+
 class CallsiteParameterAdder:
     """
     Adds parameters of the callsite that an event dictionary originated from to
     the event dictionary. This processor can be used to enrich events
     dictionaries with information such as the function name, line number and
     filename that an event dictionary originated from.
 
@@ -754,43 +797,25 @@
         ``processors`` of `structlog.configure` and ``foreign_pre_chain`` of
         `structlog.stdlib.ProcessorFormatter`.
 
     .. versionadded:: 21.5.0
     """
 
     _handlers: ClassVar[
-        dict[CallsiteParameter, Callable[[str, inspect.Traceback], Any]]
+        dict[CallsiteParameter, Callable[[str, FrameType], Any]]
     ] = {
-        CallsiteParameter.PATHNAME: (
-            lambda module, frame_info: frame_info.filename
-        ),
-        CallsiteParameter.FILENAME: (
-            lambda module, frame_info: os.path.basename(frame_info.filename)
-        ),
-        CallsiteParameter.MODULE: (
-            lambda module, frame_info: os.path.splitext(
-                os.path.basename(frame_info.filename)
-            )[0]
-        ),
-        CallsiteParameter.FUNC_NAME: (
-            lambda module, frame_info: frame_info.function
-        ),
-        CallsiteParameter.LINENO: (
-            lambda module, frame_info: frame_info.lineno
-        ),
-        CallsiteParameter.THREAD: (
-            lambda module, frame_info: threading.get_ident()
-        ),
-        CallsiteParameter.THREAD_NAME: (
-            lambda module, frame_info: threading.current_thread().name
-        ),
-        CallsiteParameter.PROCESS: (lambda module, frame_info: os.getpid()),
-        CallsiteParameter.PROCESS_NAME: (
-            lambda module, frame_info: get_processname()
-        ),
+        CallsiteParameter.PATHNAME: _get_callsite_pathname,
+        CallsiteParameter.FILENAME: _get_callsite_filename,
+        CallsiteParameter.MODULE: _get_callsite_module,
+        CallsiteParameter.FUNC_NAME: _get_callsite_func_name,
+        CallsiteParameter.LINENO: _get_callsite_lineno,
+        CallsiteParameter.THREAD: _get_callsite_thread,
+        CallsiteParameter.THREAD_NAME: _get_callsite_thread_name,
+        CallsiteParameter.PROCESS: _get_callsite_process,
+        CallsiteParameter.PROCESS_NAME: _get_callsite_process_name,
     }
     _record_attribute_map: ClassVar[dict[CallsiteParameter, str]] = {
         CallsiteParameter.PATHNAME: "pathname",
         CallsiteParameter.FILENAME: "filename",
         CallsiteParameter.MODULE: "module",
         CallsiteParameter.FUNC_NAME: "funcName",
         CallsiteParameter.LINENO: "lineno",
@@ -816,15 +841,15 @@
         if additional_ignores is None:
             additional_ignores = []
         # Ignore stack frames from the logging module. They will occur if this
         # processor is used in ProcessorFormatter, and additionally the logging
         # module should not be logging using structlog.
         self._additional_ignores = ["logging", *additional_ignores]
         self._active_handlers: list[
-            tuple[CallsiteParameter, Callable[[str, inspect.Traceback], Any]]
+            tuple[CallsiteParameter, Callable[[str, FrameType], Any]]
         ] = []
         self._record_mappings: list[CallsiteParameterAdder._RecordMapping] = []
         for parameter in parameters:
             self._active_handlers.append(
                 (parameter, self._handlers[parameter])
             )
             self._record_mappings.append(
@@ -835,28 +860,27 @@
             )
 
     def __call__(
         self, logger: logging.Logger, name: str, event_dict: EventDict
     ) -> EventDict:
         record: logging.LogRecord | None = event_dict.get("_record")
         from_structlog: bool | None = event_dict.get("_from_structlog")
-        # If the event dictionary has a record, but it comes from contrast_vendor.structlog,
+        # If the event dictionary has a record, but it comes from structlog,
         # then the callsite parameters of the record will not be correct.
         if record is not None and not from_structlog:
             for mapping in self._record_mappings:
                 event_dict[mapping.event_dict_key] = record.__dict__[
                     mapping.record_attribute
                 ]
         else:
             frame, module = _find_first_app_frame_and_name(
                 additional_ignores=self._additional_ignores
             )
-            frame_info = inspect.getframeinfo(frame)
             for parameter, handler in self._active_handlers:
-                event_dict[parameter.value] = handler(module, frame_info)
+                event_dict[parameter.value] = handler(module, frame)
         return event_dict
 
 
 class EventRenamer:
     r"""
     Rename the ``event`` key in event dicts.
```

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/structlog/stdlib.py` & `contrast_agent-8.3.0/src/contrast_vendor/structlog/stdlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,14 +140,18 @@
         )
 
     It also contains a bunch of properties that pass-through to the wrapped
     `logging.Logger` which should make it work as a drop-in replacement.
 
     .. versionadded:: 23.1.0
        Async variants `alog()`, `adebug()`, `ainfo()`, and so forth.
+
+    .. versionchanged:: 24.2.0
+        Callsite parameters are now also collected by
+        `structlog.processors.CallsiteParameterAdder` for async log methods.
     """
 
     _logger: logging.Logger
 
     def bind(self, **new_values: Any) -> BoundLogger:
         """
         Return a new logger with *new_values* added to the existing ones.
@@ -389,20 +393,24 @@
         event: str,
         args: tuple[Any, ...],
         kw: dict[str, Any],
     ) -> None:
         """
         Merge contextvars and log using the sync logger in a thread pool.
         """
+        scs_token = _ASYNC_CALLING_STACK.set(sys._getframe().f_back.f_back)  # type: ignore[union-attr, arg-type, unused-ignore]
         ctx = contextvars.copy_context()
 
-        await asyncio.get_running_loop().run_in_executor(
-            None,
-            lambda: ctx.run(lambda: meth(event, *args, **kw)),
-        )
+        try:
+            await asyncio.get_running_loop().run_in_executor(
+                None,
+                lambda: ctx.run(lambda: meth(event, *args, **kw)),
+            )
+        finally:
+            _ASYNC_CALLING_STACK.reset(scs_token)
 
     async def adebug(self, event: str, *args: Any, **kw: Any) -> None:
         """
         Log using `debug()`, but asynchronously in a separate thread.
 
         .. versionadded:: 23.1.0
         """
@@ -495,14 +503,16 @@
 
     Only available for Python 3.7 and later.
 
     .. versionadded:: 20.2.0
     .. versionchanged:: 20.2.0 fix _dispatch_to_sync contextvars usage
     .. deprecated:: 23.1.0
        Use the regular `BoundLogger` with its a-prefixed methods instead.
+    .. versionchanged:: 23.3.0
+        Callsite parameters are now also collected for async log methods.
     """
 
     __slots__ = ("sync_bl", "_loop")
 
     #: The wrapped synchronous logger. It is useful to be able to log
     #: synchronously occasionally.
     sync_bl: BoundLogger
@@ -590,16 +600,14 @@
         meth: Callable[..., Any],
         event: str,
         args: tuple[Any, ...],
         kw: dict[str, Any],
     ) -> None:
         """
         Merge contextvars and log using the sync logger in a thread pool.
-        .. versionchanged:: 23.3.0
-           Callsite parameters are now also collected under asyncio.
         """
         scs_token = _ASYNC_CALLING_STACK.set(sys._getframe().f_back.f_back)  # type: ignore[union-attr, arg-type, unused-ignore]
         ctx = contextvars.copy_context()
 
         try:
             await asyncio.get_running_loop().run_in_executor(
                 self._executor,
@@ -866,31 +874,34 @@
 
 
 def render_to_log_kwargs(
     _: logging.Logger, __: str, event_dict: EventDict
 ) -> EventDict:
     """
     Render ``event_dict`` into keyword arguments for `logging.log`.
+    See `logging.Logger`'s ``_log`` method for kwargs reference.
 
     The ``event`` field is translated into ``msg`` and the rest of the
     *event_dict* is added as ``extra``.
 
     This allows you to defer formatting to `logging`.
 
     .. versionadded:: 17.1.0
     .. versionchanged:: 22.1.0
-       ``exc_info``, ``stack_info``, and ``stackLevel`` are passed as proper
+       ``exc_info``, ``stack_info``, and ``stacklevel`` are passed as proper
        kwargs and not put into ``extra``.
+    .. versionchanged:: 24.2.0
+       ``stackLevel`` corrected to ``stacklevel``.
     """
     return {
         "msg": event_dict.pop("event"),
         "extra": event_dict,
         **{
             kw: event_dict.pop(kw)
-            for kw in ("exc_info", "stack_info", "stackLevel")
+            for kw in ("exc_info", "stack_info", "stacklevel")
             if kw in event_dict
         },
     }
 
 
 class ProcessorFormatter(logging.Formatter):
     r"""
```

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/structlog/testing.py` & `contrast_agent-8.3.0/src/contrast_vendor/structlog/testing.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,14 +195,15 @@
 
     To be used with `structlog.configure`\ 's *logger_factory*.
 
     Positional arguments are silently ignored.
 
     .. versionadded:: 20.2.0
     """
+
     logger: CapturingLogger
 
     def __init__(self) -> None:
         self.logger = CapturingLogger()
 
     def __call__(self, *args: Any) -> CapturingLogger:
         return self.logger
```

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/structlog/threadlocal.py` & `contrast_agent-8.3.0/src/contrast_vendor/structlog/threadlocal.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/structlog/tracebacks.py` & `contrast_agent-8.3.0/src/contrast_vendor/structlog/tracebacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     Container for a list of stack traces.
     """
 
     stacks: list[Stack]
 
 
 def safe_str(_object: Any) -> str:
-    """Don't allow exceptions from __str__ to propegate."""
+    """Don't allow exceptions from __str__ to propagate."""
     try:
         return str(_object)
     except Exception as error:  # noqa: BLE001
         return f"<str-error {str(error)!r}>"
 
 
 def to_repr(obj: Any, max_string: int | None = None) -> str:
@@ -173,20 +173,22 @@
             filename = frame_summary.f_code.co_filename
             if filename and not filename.startswith("<"):
                 filename = os.path.abspath(filename)
             frame = Frame(
                 filename=filename or "?",
                 lineno=line_no,
                 name=frame_summary.f_code.co_name,
-                locals={
-                    key: to_repr(value, max_string=locals_max_string)
-                    for key, value in frame_summary.f_locals.items()
-                }
-                if show_locals
-                else None,
+                locals=(
+                    {
+                        key: to_repr(value, max_string=locals_max_string)
+                        for key, value in frame_summary.f_locals.items()
+                    }
+                    if show_locals
+                    else None
+                ),
             )
             append(frame)
 
         cause = getattr(exc_value, "__cause__", None)
         if cause and cause.__traceback__:
             exc_type = cause.__class__
             exc_value = cause
```

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/structlog/twisted.py` & `contrast_agent-8.3.0/src/contrast_vendor/structlog/twisted.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from twisted.python import log
 from twisted.python.failure import Failure
 from twisted.python.log import ILogObserver, textFromEventDict
 from zope.interface import implementer
 
 from ._base import BoundLoggerBase
 from ._config import _BUILTIN_DEFAULT_PROCESSORS
-from ._utils import until_not_interrupted
 from .processors import JSONRenderer as GenericJSONRenderer
 from .typing import EventDict, WrappedLogger
 
 
 class BoundLogger(BoundLoggerBase):
     """
     Twisted-specific version of `structlog.BoundLogger`.
@@ -211,20 +210,19 @@
     """
 
     def __init__(self, file: TextIO) -> None:
         self._write = file.write
         self._flush = file.flush
 
     def __call__(self, eventDict: EventDict) -> None:
-        until_not_interrupted(
-            self._write,
+        self._write(
             textFromEventDict(eventDict)  # type: ignore[arg-type, operator]
             + "\n",
         )
-        until_not_interrupted(self._flush)
+        self._flush()
 
 
 @implementer(ILogObserver)
 class JSONLogObserverWrapper:
     """
     Wrap a log *observer* and render non-`JSONRenderer` entries to JSON.
 
@@ -299,16 +297,17 @@
     **Must** be the last processor in the chain and requires a *dictRenderer*
     for the actual formatting as an constructor argument in order to be able to
     fully support the original behaviors of ``log.msg()`` and ``log.err()``.
     """
 
     def __init__(
         self,
-        dictRenderer: Callable[[WrappedLogger, str, EventDict], str]
-        | None = None,
+        dictRenderer: (
+            Callable[[WrappedLogger, str, EventDict], str] | None
+        ) = None,
     ) -> None:
         self._dictRenderer = dictRenderer or _BUILTIN_DEFAULT_PROCESSORS[-1]
 
     def __call__(
         self, logger: WrappedLogger, name: str, eventDict: EventDict
     ) -> Any:
         if name == "err":
```

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/structlog/types.py` & `contrast_agent-8.3.0/src/contrast_vendor/structlog/types.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/structlog/typing.py` & `contrast_agent-8.3.0/src/contrast_vendor/structlog/typing.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,40 +112,35 @@
     Returns:
         Anything that can be rendered by the last processor in your chain, for
         example, a string or a JSON-serializable structure.
 
     .. versionadded:: 22.1.0
     """
 
-    def __call__(self, exc_info: ExcInfo) -> Any:
-        ...
+    def __call__(self, exc_info: ExcInfo) -> Any: ...
 
 
 @runtime_checkable
 class BindableLogger(Protocol):
     """
     **Protocol**: Methods shared among all bound loggers and that are relied on
     by *structlog*.
 
     .. versionadded:: 20.2.0
     """
 
     _context: Context
 
-    def bind(self, **new_values: Any) -> BindableLogger:
-        ...
+    def bind(self, **new_values: Any) -> BindableLogger: ...
 
-    def unbind(self, *keys: str) -> BindableLogger:
-        ...
+    def unbind(self, *keys: str) -> BindableLogger: ...
 
-    def try_unbind(self, *keys: str) -> BindableLogger:
-        ...
+    def try_unbind(self, *keys: str) -> BindableLogger: ...
 
-    def new(self, **new_values: Any) -> BindableLogger:
-        ...
+    def new(self, **new_values: Any) -> BindableLogger: ...
 
 
 class FilteringBoundLogger(BindableLogger, Protocol):
     """
     **Protocol**: A `BindableLogger` that filters by a level.
 
     The only way to instantiate one is using `make_filtering_bound_logger`.
```

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/webob/__init__.py` & `contrast_agent-8.3.0/src/contrast_vendor/webob/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/webob/acceptparse.py` & `contrast_agent-8.3.0/src/contrast_vendor/webob/acceptparse.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/webob/byterange.py` & `contrast_agent-8.3.0/src/contrast_vendor/webob/byterange.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/webob/cachecontrol.py` & `contrast_agent-8.3.0/src/contrast_vendor/webob/cachecontrol.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/webob/client.py` & `contrast_agent-8.3.0/src/contrast_vendor/webob/client.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/webob/compat.py` & `contrast_agent-8.3.0/src/contrast_vendor/webob/compat.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/webob/cookies.py` & `contrast_agent-8.3.0/src/contrast_vendor/webob/cookies.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/webob/datetime_utils.py` & `contrast_agent-8.3.0/src/contrast_vendor/webob/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/webob/dec.py` & `contrast_agent-8.3.0/src/contrast_vendor/webob/dec.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/webob/descriptors.py` & `contrast_agent-8.3.0/src/contrast_vendor/webob/descriptors.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/webob/etag.py` & `contrast_agent-8.3.0/src/contrast_vendor/webob/etag.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/webob/exc.py` & `contrast_agent-8.3.0/src/contrast_vendor/webob/exc.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/webob/headers.py` & `contrast_agent-8.3.0/src/contrast_vendor/webob/headers.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/webob/license.txt` & `contrast_agent-8.3.0/src/contrast_vendor/webob/license.txt`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/webob/multidict.py` & `contrast_agent-8.3.0/src/contrast_vendor/webob/multidict.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/webob/request.py` & `contrast_agent-8.3.0/src/contrast_vendor/webob/request.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/webob/response.py` & `contrast_agent-8.3.0/src/contrast_vendor/webob/response.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/webob/static.py` & `contrast_agent-8.3.0/src/contrast_vendor/webob/static.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/webob/util.py` & `contrast_agent-8.3.0/src/contrast_vendor/webob/util.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/wrapt/LICENSE` & `contrast_agent-8.3.0/src/contrast_vendor/wrapt/LICENSE`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/wrapt/__init__.py` & `contrast_agent-8.3.0/src/contrast_vendor/wrapt/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/wrapt/arguments.py` & `contrast_agent-8.3.0/src/contrast_vendor/wrapt/arguments.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/wrapt/decorators.py` & `contrast_agent-8.3.0/src/contrast_vendor/wrapt/decorators.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/wrapt/importer.py` & `contrast_agent-8.3.0/src/contrast_vendor/wrapt/importer.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/wrapt/patches.py` & `contrast_agent-8.3.0/src/contrast_vendor/wrapt/patches.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/wrapt/weakrefs.py` & `contrast_agent-8.3.0/src/contrast_vendor/wrapt/weakrefs.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/wrapt/wrappers.py` & `contrast_agent-8.3.0/src/contrast_vendor/wrapt/wrappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -527,14 +527,23 @@
         # None and accessing an unbound instance method from a class.
         # This is because we need to be able to later detect that
         # specific case as we will need to extract the instance from the
         # first argument of those passed in.
 
         if self._self_parent is None:
             if not inspect.isclass(self.__wrapped__):
+                ### Contrast Addition Start ###
+
+                # If the wrapped object is a builtin, we can't bind it
+                # because it doesn't have a __get__ descriptor. We also
+                # don't need to bind it, because it's not a method.
+                if inspect.isbuiltin(self.__wrapped__):
+                    return self
+
+                ### Contrast Addition End ###
                 descriptor = self.__wrapped__.__get__(instance, owner)
 
                 return self.__bound_function_wrapper__(descriptor, instance,
                         self._self_wrapper, self._self_enabled,
                         self._self_binding, self)
 
             return self
```

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/zipp/LICENSE` & `contrast_agent-8.3.0/src/contrast_vendor/zipp/LICENSE`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/zipp/__init__.py` & `contrast_agent-8.3.0/src/contrast_vendor/zipp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import io
 import posixpath
 import zipfile
 import itertools
 import contextlib
 import pathlib
 import re
+import stat
 import sys
 
 from .compat.py310 import text_encoding
 from .glob import Translator
 
 
 __all__ = ['Path']
@@ -259,15 +260,15 @@
     >>> path.name
     'abcde.zip'
     >>> path.filename == pathlib.Path('mem/abcde.zip')
     True
     >>> str(path.parent)
     'mem'
 
-    If the zipfile has no filename, such attribtues are not
+    If the zipfile has no filename, such ﻿attributes are not
     valid and accessing them will raise an Exception.
 
     >>> zf.filename = None
     >>> path.name
     Traceback (most recent call last):
     ...
     TypeError: ...
@@ -387,17 +388,19 @@
         return filter(self._is_child, subs)
 
     def match(self, path_pattern):
         return pathlib.PurePosixPath(self.at).match(path_pattern)
 
     def is_symlink(self):
         """
-        Return whether this path is a symlink. Always false (python/cpython#82102).
+        Return whether this path is a symlink.
         """
-        return False
+        info = self.root.getinfo(self.at)
+        mode = info.external_attr >> 16
+        return stat.S_ISLNK(mode)
 
     def glob(self, pattern):
         if not pattern:
             raise ValueError(f"Unacceptable pattern: {pattern!r}")
 
         prefix = re.escape(self.at)
         tr = Translator(seps='/')
```

### Comparing `contrast_agent-8.2.0/src/contrast_vendor/zipp/glob.py` & `contrast_agent-8.3.0/src/contrast_vendor/zipp/glob.py`

 * *Files identical despite different names*

