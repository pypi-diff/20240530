# Comparing `tmp/dbgpt-0.5.6rc0.tar.gz` & `tmp/dbgpt-0.5.7rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbgpt-0.5.6rc0.tar", last modified: Mon May  6 06:24:51 2024, max compression
+gzip compressed data, was "dbgpt-0.5.7rc0.tar", last modified: Thu May 30 09:29:16 2024, max compression
```

## Comparing `dbgpt-0.5.6rc0.tar` & `dbgpt-0.5.7rc0.tar`

### file list

```diff
@@ -1,485 +1,521 @@
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.134457 dbgpt-0.5.6rc0/
--rw-r--r--   0 staneyffer   (501) staff       (20)     1067 2023-10-24 06:24:09.000000 dbgpt-0.5.6rc0/LICENSE
--rw-r--r--   0 staneyffer   (501) staff       (20)       59 2023-12-16 11:45:45.000000 dbgpt-0.5.6rc0/MANIFEST.in
--rw-r--r--   0 staneyffer   (501) staff       (20)    31466 2024-05-06 06:24:51.133822 dbgpt-0.5.6rc0/PKG-INFO
--rw-r--r--   0 staneyffer   (501) staff       (20)    12437 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/README.md
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.808346 dbgpt-0.5.6rc0/dbgpt/
--rw-r--r--   0 staneyffer   (501) staff       (20)      638 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.813573 dbgpt-0.5.6rc0/dbgpt/_private/
--rw-r--r--   0 staneyffer   (501) staff       (20)       83 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/_private/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    14757 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/_private/config.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1693 2024-04-20 08:03:40.000000 dbgpt-0.5.6rc0/dbgpt/_private/llm_metadata.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2234 2024-04-20 08:03:40.000000 dbgpt-0.5.6rc0/dbgpt/_private/pydantic.py
--rw-r--r--   0 staneyffer   (501) staff       (20)       18 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/_version.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.814326 dbgpt-0.5.6rc0/dbgpt/agent/
--rw-r--r--   0 staneyffer   (501) staff       (20)     1259 2024-05-06 03:59:41.000000 dbgpt-0.5.6rc0/dbgpt/agent/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.821354 dbgpt-0.5.6rc0/dbgpt/agent/core/
--rw-r--r--   0 staneyffer   (501) staff       (20)     1008 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.823886 dbgpt-0.5.6rc0/dbgpt/agent/core/action/
--rw-r--r--   0 staneyffer   (501) staff       (20)      744 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/action/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5892 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/action/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      936 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/action/blank_action.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9734 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/agent.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5336 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/agent_manage.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    37924 2024-05-06 03:36:27.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/base_agent.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6063 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/base_team.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.830006 dbgpt-0.5.6rc0/dbgpt/agent/core/memory/
--rw-r--r--   0 staneyffer   (501) staff       (20)      540 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/memory/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9235 2024-05-06 03:24:52.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/memory/agent_memory.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    24306 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/memory/base.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.832886 dbgpt-0.5.6rc0/dbgpt/agent/core/memory/gpts/
--rw-r--r--   0 staneyffer   (501) staff       (20)      554 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/memory/gpts/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6837 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/memory/gpts/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5799 2024-05-06 03:59:42.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/memory/gpts/default_gpts_memory.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7169 2024-05-06 03:59:42.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/memory/gpts/gpts_memory.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    10793 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/memory/hybrid.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5629 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/memory/llm.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6836 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/memory/long_term.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8549 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/memory/short_term.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.835976 dbgpt-0.5.6rc0/dbgpt/agent/core/plan/
--rw-r--r--   0 staneyffer   (501) staff       (20)      914 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/plan/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.838948 dbgpt-0.5.6rc0/dbgpt/agent/core/plan/awel/
--rw-r--r--   0 staneyffer   (501) staff       (20)       60 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/plan/awel/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    10720 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/plan/awel/agent_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6272 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/plan/awel/agent_operator_resource.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8700 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/plan/awel/team_awel_layout.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4730 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/plan/plan_action.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8730 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/plan/planner_agent.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    13138 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/plan/team_auto_plan.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.840571 dbgpt-0.5.6rc0/dbgpt/agent/core/profile/
--rw-r--r--   0 staneyffer   (501) staff       (20)      951 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/profile/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    12666 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/profile/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7380 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/role.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      456 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/schema.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      560 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/user_proxy_agent.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.847129 dbgpt-0.5.6rc0/dbgpt/agent/expand/
--rw-r--r--   0 staneyffer   (501) staff       (20)     2560 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/expand/Indicator_assistant_agent.py
--rw-r--r--   0 staneyffer   (501) staff       (20)       26 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/agent/expand/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.852273 dbgpt-0.5.6rc0/dbgpt/agent/expand/actions/
--rw-r--r--   0 staneyffer   (501) staff       (20)       32 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/expand/actions/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3761 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/expand/actions/chart_action.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5249 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/expand/actions/code_action.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4476 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/expand/actions/dashboard_action.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5457 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/expand/actions/indicator_action.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5583 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/expand/actions/plugin_action.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8090 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/expand/code_assistant_agent.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3054 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/expand/dashboard_assistant_agent.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6358 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/expand/data_scientist_agent.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3512 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/expand/plugin_assistant_agent.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    22221 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/expand/retrieve_summary_assistant_agent.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2560 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/expand/summary_assistant_agent.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.855671 dbgpt-0.5.6rc0/dbgpt/agent/plugin/
--rw-r--r--   0 staneyffer   (501) staff       (20)      214 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/agent/plugin/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.860058 dbgpt-0.5.6rc0/dbgpt/agent/plugin/commands/
--rw-r--r--   0 staneyffer   (501) staff       (20)       23 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/agent/plugin/commands/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.860861 dbgpt-0.5.6rc0/dbgpt/agent/plugin/commands/built_in/
--rw-r--r--   0 staneyffer   (501) staff       (20)       36 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/agent/plugin/commands/built_in/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.863406 dbgpt-0.5.6rc0/dbgpt/agent/plugin/commands/built_in/display_type/
--rw-r--r--   0 staneyffer   (501) staff       (20)       88 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/agent/plugin/commands/built_in/display_type/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    10775 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_chart_gen.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      687 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_table_gen.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1188 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_text_gen.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5535 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/plugin/commands/command.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    22485 2024-04-20 08:03:40.000000 dbgpt-0.5.6rc0/dbgpt/agent/plugin/commands/command_manage.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1166 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/agent/plugin/commands/exceptions.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6159 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/plugin/generator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1240 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/agent/plugin/loader.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7625 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/agent/plugin/plugins_util.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.867631 dbgpt-0.5.6rc0/dbgpt/agent/resource/
--rw-r--r--   0 staneyffer   (501) staff       (20)      665 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/agent/resource/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3721 2024-04-20 08:03:40.000000 dbgpt-0.5.6rc0/dbgpt/agent/resource/resource_api.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4443 2024-04-11 14:37:18.000000 dbgpt-0.5.6rc0/dbgpt/agent/resource/resource_db_api.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      782 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/agent/resource/resource_knowledge_api.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1350 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/agent/resource/resource_loader.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3225 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/resource/resource_plugin_api.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.868868 dbgpt-0.5.6rc0/dbgpt/agent/util/
--rw-r--r--   0 staneyffer   (501) staff       (20)      114 2024-04-11 14:37:18.000000 dbgpt-0.5.6rc0/dbgpt/agent/util/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      850 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/agent/util/cmp.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.870630 dbgpt-0.5.6rc0/dbgpt/agent/util/llm/
--rw-r--r--   0 staneyffer   (501) staff       (20)       22 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/util/llm/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3473 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/util/llm/llm.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6745 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/util/llm/llm_client.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.872136 dbgpt-0.5.6rc0/dbgpt/agent/util/llm/strategy/
--rw-r--r--   0 staneyffer   (501) staff       (20)       27 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/util/llm/strategy/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1291 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/util/llm/strategy/priority.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.873116 dbgpt-0.5.6rc0/dbgpt/cli/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/cli/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5794 2024-04-09 19:22:18.000000 dbgpt-0.5.6rc0/dbgpt/cli/cli_scripts.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.880221 dbgpt-0.5.6rc0/dbgpt/client/
--rw-r--r--   0 staneyffer   (501) staff       (20)      154 2024-03-22 07:58:46.000000 dbgpt-0.5.6rc0/dbgpt/client/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7280 2024-04-17 10:27:40.000000 dbgpt-0.5.6rc0/dbgpt/client/_cli.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1413 2024-03-22 07:58:46.000000 dbgpt-0.5.6rc0/dbgpt/client/app.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    14335 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/client/client.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3784 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/client/datasource.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3568 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/client/flow.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7003 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/client/knowledge.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9487 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/client/schema.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    10759 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/component.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.881874 dbgpt-0.5.6rc0/dbgpt/configs/
--rw-r--r--   0 staneyffer   (501) staff       (20)      530 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/configs/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    10962 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/configs/model_config.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.882809 dbgpt-0.5.6rc0/dbgpt/core/
--rw-r--r--   0 staneyffer   (501) staff       (20)     2672 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/core/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.884810 dbgpt-0.5.6rc0/dbgpt/core/_private/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/_private/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1225 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/_private/example_base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3753 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/_private/prompt_registry.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.885666 dbgpt-0.5.6rc0/dbgpt/core/awel/
--rw-r--r--   0 staneyffer   (501) staff       (20)     6061 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.889271 dbgpt-0.5.6rc0/dbgpt/core/awel/dag/
--rw-r--r--   0 staneyffer   (501) staff       (20)       26 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/dag/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    29536 2024-03-26 04:37:36.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/dag/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4143 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/dag/dag_manager.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3309 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/dag/loader.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.893395 dbgpt-0.5.6rc0/dbgpt/core/awel/flow/
--rw-r--r--   0 staneyffer   (501) staff       (20)      752 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/flow/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    33942 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/flow/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1506 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/flow/compat.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1577 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/flow/exceptions.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    29039 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/flow/flow_factory.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.896919 dbgpt-0.5.6rc0/dbgpt/core/awel/operators/
--rw-r--r--   0 staneyffer   (501) staff       (20)       30 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/operators/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    11174 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/operators/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    11132 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/operators/common_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4262 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/operators/stream_operator.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.898405 dbgpt-0.5.6rc0/dbgpt/core/awel/resource/
--rw-r--r--   0 staneyffer   (501) staff       (20)       58 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/resource/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      413 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/resource/base.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.900727 dbgpt-0.5.6rc0/dbgpt/core/awel/runner/
--rw-r--r--   0 staneyffer   (501) staff       (20)      118 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/runner/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4203 2024-03-25 14:27:11.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/runner/job_manager.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7648 2024-03-25 14:27:11.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/runner/local_runner.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.903284 dbgpt-0.5.6rc0/dbgpt/core/awel/task/
--rw-r--r--   0 staneyffer   (501) staff       (20)       26 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/task/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    14271 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/task/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    20591 2024-03-25 14:27:11.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/task/task_impl.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.909529 dbgpt-0.5.6rc0/dbgpt/core/awel/trigger/
--rw-r--r--   0 staneyffer   (501) staff       (20)       34 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/trigger/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      519 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/trigger/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6462 2024-04-09 19:22:18.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/trigger/ext_http_trigger.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    37988 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/trigger/http_trigger.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6040 2024-03-27 07:42:00.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/trigger/iterator_trigger.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7886 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/trigger/trigger_manager.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.912683 dbgpt-0.5.6rc0/dbgpt/core/awel/util/
--rw-r--r--   0 staneyffer   (501) staff       (20)       22 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/util/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      228 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/util/_typing_util.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      500 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/util/http_util.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2328 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/util/parameter_util.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.922466 dbgpt-0.5.6rc0/dbgpt/core/interface/
--rw-r--r--   0 staneyffer   (501) staff       (20)      102 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/core/interface/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3546 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/core/interface/cache.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1018 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/core/interface/embeddings.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7410 2024-03-23 08:18:41.000000 dbgpt-0.5.6rc0/dbgpt/core/interface/evaluation.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3818 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/core/interface/knowledge.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    31110 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/core/interface/llm.py
--rwxr-xr-x   0 staneyffer   (501) staff       (20)    42803 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/core/interface/message.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.928278 dbgpt-0.5.6rc0/dbgpt/core/interface/operators/
--rw-r--r--   0 staneyffer   (501) staff       (20)       55 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/core/interface/operators/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4438 2024-03-25 14:27:11.000000 dbgpt-0.5.6rc0/dbgpt/core/interface/operators/composer_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    18962 2024-03-27 07:42:00.000000 dbgpt-0.5.6rc0/dbgpt/core/interface/operators/llm_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    23685 2024-03-25 14:27:11.000000 dbgpt-0.5.6rc0/dbgpt/core/interface/operators/message_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    16465 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/core/interface/operators/prompt_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      767 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/core/interface/operators/retriever.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    10805 2024-04-09 19:22:18.000000 dbgpt-0.5.6rc0/dbgpt/core/interface/output_parser.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    26575 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/core/interface/prompt.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1748 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/core/interface/serialization.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    15126 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/core/interface/storage.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.929232 dbgpt-0.5.6rc0/dbgpt/core/operators/
--rw-r--r--   0 staneyffer   (501) staff       (20)     1509 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/core/operators/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.931647 dbgpt-0.5.6rc0/dbgpt/core/operators/flow/
--rw-r--r--   0 staneyffer   (501) staff       (20)      340 2024-03-25 14:27:11.000000 dbgpt-0.5.6rc0/dbgpt/core/operators/flow/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9546 2024-03-25 14:27:11.000000 dbgpt-0.5.6rc0/dbgpt/core/operators/flow/composer_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2601 2024-03-25 14:27:11.000000 dbgpt-0.5.6rc0/dbgpt/core/operators/flow/dict_operator.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.932886 dbgpt-0.5.6rc0/dbgpt/core/schema/
--rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/schema/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8246 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/core/schema/api.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.937972 dbgpt-0.5.6rc0/dbgpt/datasource/
--rw-r--r--   0 staneyffer   (501) staff       (20)      412 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6802 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/datasource/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3909 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/conn_spark.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4454 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/datasource/conn_tugraph.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      923 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/db_conn_info.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.940091 dbgpt-0.5.6rc0/dbgpt/datasource/manages/
--rw-r--r--   0 staneyffer   (501) staff       (20)      157 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/manages/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9173 2024-03-28 01:32:30.000000 dbgpt-0.5.6rc0/dbgpt/datasource/manages/connect_config_db.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8623 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/datasource/manages/connector_manager.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.940902 dbgpt-0.5.6rc0/dbgpt/datasource/nosql/
--rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/nosql/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.942250 dbgpt-0.5.6rc0/dbgpt/datasource/operators/
--rw-r--r--   0 staneyffer   (501) staff       (20)      128 2024-03-28 01:32:23.000000 dbgpt-0.5.6rc0/dbgpt/datasource/operators/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      770 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/operators/datasource_operator.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.951460 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/
--rw-r--r--   0 staneyffer   (501) staff       (20)       30 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    23230 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    12710 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/conn_clickhouse.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6407 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/conn_doris.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2473 2024-03-25 06:53:38.000000 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/conn_duckdb.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1417 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/conn_hive.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1329 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/conn_mssql.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      295 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/conn_mysql.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8185 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/conn_postgresql.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9677 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/conn_sqlite.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5681 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/conn_starrocks.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.952403 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/dialect/
--rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/dialect/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.953368 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/dialect/starrocks/
--rw-r--r--   0 staneyffer   (501) staff       (20)      648 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/dialect/starrocks/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.955106 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/
--rw-r--r--   0 staneyffer   (501) staff       (20)      820 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3186 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/datatype.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7507 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/dialect.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      116 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/redis.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.958311 dbgpt-0.5.6rc0/dbgpt/model/
--rw-r--r--   0 staneyffer   (501) staff       (20)      320 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.968349 dbgpt-0.5.6rc0/dbgpt/model/adapter/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/adapter/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    19868 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/adapter/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3589 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/model/adapter/embeddings_loader.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8687 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/adapter/fschat_adapter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    11521 2024-04-22 03:12:53.000000 dbgpt-0.5.6rc0/dbgpt/model/adapter/hf_adapter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    15595 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/adapter/loader.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5520 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/adapter/model_adapter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    17037 2024-04-09 19:22:18.000000 dbgpt-0.5.6rc0/dbgpt/model/adapter/old_adapter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    10399 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/model/adapter/proxy_adapter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3587 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/adapter/template.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3495 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/adapter/vllm_adapter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3050 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    13971 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/cli.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.969947 dbgpt-0.5.6rc0/dbgpt/model/operators/
--rw-r--r--   0 staneyffer   (501) staff       (20)      341 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/operators/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4981 2024-03-25 14:27:11.000000 dbgpt-0.5.6rc0/dbgpt/model/operators/llm_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    18176 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/model/parameter.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.971605 dbgpt-0.5.6rc0/dbgpt/model/proxy/
--rw-r--r--   0 staneyffer   (501) staff       (20)     1096 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/model/proxy/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7967 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/proxy/base.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.983222 dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/
--rw-r--r--   0 staneyffer   (501) staff       (20)      306 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3077 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/baichuan.py
--rwxr-xr-x   0 staneyffer   (501) staff       (20)     2325 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/bard.py
--rwxr-xr-x   0 staneyffer   (501) staff       (20)    10636 2024-04-10 19:49:14.000000 dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/chatgpt.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      200 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/claude.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6485 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/gemini.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3336 2024-04-10 19:49:14.000000 dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/moonshot.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3279 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/ollama.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1350 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/proxy_model.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7602 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/spark.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3720 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/tongyi.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7011 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/wenxin.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2859 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/yi.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3796 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/zhipu.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.986533 dbgpt-0.5.6rc0/dbgpt/model/utils/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/utils/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9274 2024-03-27 07:42:00.000000 dbgpt-0.5.6rc0/dbgpt/model/utils/chatgpt_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2365 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/utils/llm_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3101 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/utils/token_utils.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.988231 dbgpt-0.5.6rc0/dbgpt/rag/
--rw-r--r--   0 staneyffer   (501) staff       (20)      200 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.992159 dbgpt-0.5.6rc0/dbgpt/rag/assembler/
--rw-r--r--   0 staneyffer   (501) staff       (20)      431 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/assembler/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2648 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/assembler/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4815 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/assembler/db_schema.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4199 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/assembler/embedding.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4611 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/assembler/summary.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6792 2024-03-25 14:27:11.000000 dbgpt-0.5.6rc0/dbgpt/rag/chunk_manager.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.995761 dbgpt-0.5.6rc0/dbgpt/rag/embedding/
--rw-r--r--   0 staneyffer   (501) staff       (20)      771 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/rag/embedding/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1167 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/embedding/_wrapped.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8826 2024-03-25 14:27:11.000000 dbgpt-0.5.6rc0/dbgpt/rag/embedding/embedding_factory.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    28119 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/rag/embedding/embeddings.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.997994 dbgpt-0.5.6rc0/dbgpt/rag/evaluation/
--rw-r--r--   0 staneyffer   (501) staff       (20)      271 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/evaluation/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8772 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/rag/evaluation/retriever.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.000176 dbgpt-0.5.6rc0/dbgpt/rag/extractor/
--rw-r--r--   0 staneyffer   (501) staff       (20)      152 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/extractor/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1314 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/extractor/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6352 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/extractor/summary.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.000914 dbgpt-0.5.6rc0/dbgpt/rag/graph/
--rw-r--r--   0 staneyffer   (501) staff       (20)       28 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/graph/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.009299 dbgpt-0.5.6rc0/dbgpt/rag/knowledge/
--rw-r--r--   0 staneyffer   (501) staff       (20)     1338 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/knowledge/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5582 2024-04-10 06:34:08.000000 dbgpt-0.5.6rc0/dbgpt/rag/knowledge/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3541 2024-04-10 06:34:08.000000 dbgpt-0.5.6rc0/dbgpt/rag/knowledge/csv.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2389 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/rag/knowledge/datasource.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2580 2024-04-10 06:34:08.000000 dbgpt-0.5.6rc0/dbgpt/rag/knowledge/docx.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6600 2024-04-10 06:34:08.000000 dbgpt-0.5.6rc0/dbgpt/rag/knowledge/factory.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3024 2024-04-10 06:34:08.000000 dbgpt-0.5.6rc0/dbgpt/rag/knowledge/html.py
--rw-r--r--   0 staneyffer   (501) staff       (20)       22 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/knowledge/json.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2600 2024-04-10 06:34:08.000000 dbgpt-0.5.6rc0/dbgpt/rag/knowledge/markdown.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3378 2024-04-10 06:34:08.000000 dbgpt-0.5.6rc0/dbgpt/rag/knowledge/pdf.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2886 2024-04-10 06:34:08.000000 dbgpt-0.5.6rc0/dbgpt/rag/knowledge/pptx.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1807 2024-04-10 06:34:08.000000 dbgpt-0.5.6rc0/dbgpt/rag/knowledge/string.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2504 2024-04-10 06:34:08.000000 dbgpt-0.5.6rc0/dbgpt/rag/knowledge/txt.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2143 2024-04-10 06:34:08.000000 dbgpt-0.5.6rc0/dbgpt/rag/knowledge/url.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.014824 dbgpt-0.5.6rc0/dbgpt/rag/operators/
--rw-r--r--   0 staneyffer   (501) staff       (20)      971 2024-03-25 14:27:11.000000 dbgpt-0.5.6rc0/dbgpt/rag/operators/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      654 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/operators/assembler.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      743 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/operators/datasource.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2956 2024-03-28 01:32:23.000000 dbgpt-0.5.6rc0/dbgpt/rag/operators/db_schema.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6584 2024-03-25 14:27:11.000000 dbgpt-0.5.6rc0/dbgpt/rag/operators/embedding.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2085 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/operators/evaluation.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4534 2024-03-25 14:27:11.000000 dbgpt-0.5.6rc0/dbgpt/rag/operators/knowledge.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1268 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/operators/rerank.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3199 2024-03-25 14:27:11.000000 dbgpt-0.5.6rc0/dbgpt/rag/operators/rewrite.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1466 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/operators/schema_linking.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4156 2024-03-25 14:27:11.000000 dbgpt-0.5.6rc0/dbgpt/rag/operators/summary.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.018875 dbgpt-0.5.6rc0/dbgpt/rag/retriever/
--rw-r--r--   0 staneyffer   (501) staff       (20)      503 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/retriever/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4379 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/rag/retriever/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7270 2024-04-10 06:34:08.000000 dbgpt-0.5.6rc0/dbgpt/rag/retriever/db_schema.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8888 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/rag/retriever/embedding.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7113 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/rag/retriever/rerank.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5223 2024-03-25 14:27:11.000000 dbgpt-0.5.6rc0/dbgpt/rag/retriever/rewrite.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5186 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/rag/retriever/time_weighted.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.020831 dbgpt-0.5.6rc0/dbgpt/rag/schemalinker/
--rw-r--r--   0 staneyffer   (501) staff       (20)       30 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/schemalinker/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1624 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/schemalinker/base_linker.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3392 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/schemalinker/schema_linking.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.023830 dbgpt-0.5.6rc0/dbgpt/rag/summary/
--rw-r--r--   0 staneyffer   (501) staff       (20)      420 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/summary/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1226 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/summary/db_summary.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5210 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/rag/summary/db_summary_client.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4575 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/rag/summary/gdbms_db_summary.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4443 2024-04-13 17:38:21.000000 dbgpt-0.5.6rc0/dbgpt/rag/summary/rdbms_db_summary.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.026406 dbgpt-0.5.6rc0/dbgpt/rag/text_splitter/
--rw-r--r--   0 staneyffer   (501) staff       (20)      539 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/text_splitter/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1497 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/text_splitter/pre_text_splitter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    32461 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/rag/text_splitter/text_splitter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6913 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/rag/text_splitter/token_splitter.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.027754 dbgpt-0.5.6rc0/dbgpt/storage/
--rw-r--r--   0 staneyffer   (501) staff       (20)       67 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/storage/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.031269 dbgpt-0.5.6rc0/dbgpt/storage/cache/
--rw-r--r--   0 staneyffer   (501) staff       (20)      384 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/storage/cache/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)       24 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/storage/cache/embedding_cache.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6185 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/storage/cache/llm_cache.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4472 2024-04-17 10:41:53.000000 dbgpt-0.5.6rc0/dbgpt/storage/cache/manager.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9995 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/storage/cache/operators.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.031896 dbgpt-0.5.6rc0/dbgpt/storage/cache/protocol/
--rw-r--r--   0 staneyffer   (501) staff       (20)       27 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/storage/cache/protocol/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.032930 dbgpt-0.5.6rc0/dbgpt/storage/cache/storage/
--rw-r--r--   0 staneyffer   (501) staff       (20)       47 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/storage/cache/storage/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8913 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/storage/cache/storage/base.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.034108 dbgpt-0.5.6rc0/dbgpt/storage/cache/storage/disk/
--rw-r--r--   0 staneyffer   (501) staff       (20)       41 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/storage/cache/storage/disk/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3254 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/storage/cache/storage/disk/disk_storage.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.035844 dbgpt-0.5.6rc0/dbgpt/storage/chat_history/
--rw-r--r--   0 staneyffer   (501) staff       (20)      438 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/storage/chat_history/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4736 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/storage/chat_history/chat_history_db.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5829 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/storage/chat_history/storage_adapter.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.039514 dbgpt-0.5.6rc0/dbgpt/storage/metadata/
--rw-r--r--   0 staneyffer   (501) staff       (20)      476 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/storage/metadata/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9345 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/storage/metadata/_base_dao.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1041 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/storage/metadata/db_factory.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    18854 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/storage/metadata/db_manager.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5503 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/storage/metadata/db_storage.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1892 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/storage/schema.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.046483 dbgpt-0.5.6rc0/dbgpt/storage/vector_store/
--rw-r--r--   0 staneyffer   (501) staff       (20)     1173 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/storage/vector_store/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7923 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/storage/vector_store/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8233 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/storage/vector_store/chroma_store.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7445 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/storage/vector_store/connector.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1234 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/storage/vector_store/filters.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    21229 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/storage/vector_store/milvus_store.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    29140 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/storage/vector_store/oceanbase_store.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3440 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/storage/vector_store/pgvector_store.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6727 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/storage/vector_store/weaviate_store.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.069856 dbgpt-0.5.6rc0/dbgpt/util/
--rw-r--r--   0 staneyffer   (501) staff       (20)      413 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    14058 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/_db_migration_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3861 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/util/annotations.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4659 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/api_utils.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.070516 dbgpt-0.5.6rc0/dbgpt/util/benchmarks/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/benchmarks/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.071495 dbgpt-0.5.6rc0/dbgpt/util/benchmarks/llm/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/benchmarks/llm/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    10778 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/benchmarks/llm/fastchat_benchmarks_inference.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9317 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/util/benchmarks/llm/llm_benchmarks.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1703 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/chat_util.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    19326 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/util/code_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5840 2024-04-12 06:30:46.000000 dbgpt-0.5.6rc0/dbgpt/util/command_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1791 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/config_utils.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.072630 dbgpt-0.5.6rc0/dbgpt/util/configure/
--rw-r--r--   0 staneyffer   (501) staff       (20)       56 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/util/configure/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4719 2024-05-06 03:51:05.000000 dbgpt-0.5.6rc0/dbgpt/util/configure/base.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.074252 dbgpt-0.5.6rc0/dbgpt/util/console/
--rw-r--r--   0 staneyffer   (501) staff       (20)       70 2024-03-27 07:42:00.000000 dbgpt-0.5.6rc0/dbgpt/util/console/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1827 2024-03-27 07:42:00.000000 dbgpt-0.5.6rc0/dbgpt/util/console/console.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      780 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/custom_data_structure.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      247 2024-04-09 19:22:04.000000 dbgpt-0.5.6rc0/dbgpt/util/date_utils.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.077668 dbgpt-0.5.6rc0/dbgpt/util/dbgpts/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/dbgpts/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1936 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/dbgpts/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5982 2024-03-27 07:42:00.000000 dbgpt-0.5.6rc0/dbgpt/util/dbgpts/cli.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    11198 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/util/dbgpts/loader.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    11883 2024-04-15 03:42:53.000000 dbgpt-0.5.6rc0/dbgpt/util/dbgpts/repo.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    10560 2024-04-15 03:42:53.000000 dbgpt-0.5.6rc0/dbgpt/util/dbgpts/template.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      533 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/error_types.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2886 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/executor_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3929 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/util/fastapi.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1807 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/formatting.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3340 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/function_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    12937 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/global_helper.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1976 2024-03-25 14:27:11.000000 dbgpt-0.5.6rc0/dbgpt/util/i18n_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2612 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/util/id_generator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3673 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/util/json_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      238 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/memory_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2679 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/model_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      893 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/module_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      704 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/net_utils.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.078464 dbgpt-0.5.6rc0/dbgpt/util/network/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-04-09 19:22:18.000000 dbgpt-0.5.6rc0/dbgpt/util/network/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9818 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/util/network/_cli.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3488 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/openai_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      618 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/util/pagination_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    27652 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/parameter_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      105 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/path_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      629 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/pd_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8747 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/util/prompt_util.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1676 2024-04-18 02:11:54.000000 dbgpt-0.5.6rc0/dbgpt/util/retry.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.079322 dbgpt-0.5.6rc0/dbgpt/util/serialization/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/serialization/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1859 2024-04-17 10:39:42.000000 dbgpt-0.5.6rc0/dbgpt/util/serialization/json_serialization.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2399 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/util/similarity_util.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      697 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/singleton.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.083752 dbgpt-0.5.6rc0/dbgpt/util/speech/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/speech/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1119 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/speech/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1180 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/speech/brian.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2985 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/speech/eleven_labs.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      467 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/speech/gtts.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      523 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/speech/macos_tts.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1441 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/speech/say.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2526 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/splitter_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3006 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/util/string_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7537 2024-04-09 19:22:18.000000 dbgpt-0.5.6rc0/dbgpt/util/system_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1019 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/util/time_utils.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.088031 dbgpt-0.5.6rc0/dbgpt/util/tracer/
--rw-r--r--   0 staneyffer   (501) staff       (20)      723 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/tracer/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7264 2024-04-11 14:37:18.000000 dbgpt-0.5.6rc0/dbgpt/util/tracer/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5743 2024-04-11 14:37:18.000000 dbgpt-0.5.6rc0/dbgpt/util/tracer/span_storage.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    18465 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/tracer/tracer_cli.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7846 2024-04-17 04:06:45.000000 dbgpt-0.5.6rc0/dbgpt/util/tracer/tracer_impl.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1504 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/tracer/tracer_middleware.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5246 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/utils.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.089932 dbgpt-0.5.6rc0/dbgpt/vis/
--rw-r--r--   0 staneyffer   (501) staff       (20)      602 2024-04-11 14:37:18.000000 dbgpt-0.5.6rc0/dbgpt/vis/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1050 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/vis/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1220 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/vis/client.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.094192 dbgpt-0.5.6rc0/dbgpt/vis/tags/
--rw-r--r--   0 staneyffer   (501) staff       (20)       16 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/vis/tags/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      284 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/vis/tags/vis_agent_message.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      257 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/vis/tags/vis_agent_plans.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3080 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/vis/tags/vis_chart.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      256 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/vis/tags/vis_code.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1957 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/vis/tags/vis_dashboard.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      258 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/vis/tags/vis_gpts_execution.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      311 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/vis/tags/vis_gpts_result.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      253 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/vis/tags/vis_plugin.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.811025 dbgpt-0.5.6rc0/dbgpt.egg-info/
--rw-r--r--   0 staneyffer   (501) staff       (20)    31466 2024-05-06 06:24:50.000000 dbgpt-0.5.6rc0/dbgpt.egg-info/PKG-INFO
--rw-r--r--   0 staneyffer   (501) staff       (20)    13441 2024-05-06 06:24:50.000000 dbgpt-0.5.6rc0/dbgpt.egg-info/SOURCES.txt
--rw-r--r--   0 staneyffer   (501) staff       (20)        1 2024-05-06 06:24:50.000000 dbgpt-0.5.6rc0/dbgpt.egg-info/dependency_links.txt
--rw-r--r--   0 staneyffer   (501) staff       (20)       53 2024-05-06 06:24:50.000000 dbgpt-0.5.6rc0/dbgpt.egg-info/entry_points.txt
--rw-r--r--   0 staneyffer   (501) staff       (20)     5169 2024-05-06 06:24:50.000000 dbgpt-0.5.6rc0/dbgpt.egg-info/requires.txt
--rw-r--r--   0 staneyffer   (501) staff       (20)        6 2024-05-06 06:24:50.000000 dbgpt-0.5.6rc0/dbgpt.egg-info/top_level.txt
--rw-r--r--   0 staneyffer   (501) staff       (20)       38 2024-05-06 06:24:51.134553 dbgpt-0.5.6rc0/setup.cfg
--rw-r--r--   0 staneyffer   (501) staff       (20)    24345 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/setup.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.766378 dbgpt-0.5.7rc0/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1067 2023-10-24 06:24:09.000000 dbgpt-0.5.7rc0/LICENSE
+-rw-r--r--   0 staneyffer   (501) staff       (20)       59 2023-12-16 11:45:45.000000 dbgpt-0.5.7rc0/MANIFEST.in
+-rw-r--r--   0 staneyffer   (501) staff       (20)    32191 2024-05-30 09:29:16.765847 dbgpt-0.5.7rc0/PKG-INFO
+-rw-r--r--   0 staneyffer   (501) staff       (20)    12790 2024-05-23 01:46:11.000000 dbgpt-0.5.7rc0/README.md
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.394504 dbgpt-0.5.7rc0/dbgpt/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      638 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.399721 dbgpt-0.5.7rc0/dbgpt/_private/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       83 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/_private/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    14647 2024-05-16 08:08:10.000000 dbgpt-0.5.7rc0/dbgpt/_private/config.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1693 2024-04-20 08:03:40.000000 dbgpt-0.5.7rc0/dbgpt/_private/llm_metadata.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2258 2024-05-30 08:16:14.000000 dbgpt-0.5.7rc0/dbgpt/_private/pydantic.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)       18 2024-05-30 08:16:14.000000 dbgpt-0.5.7rc0/dbgpt/_version.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.400374 dbgpt-0.5.7rc0/dbgpt/agent/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1172 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/agent/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.407085 dbgpt-0.5.7rc0/dbgpt/agent/core/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1008 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/agent/core/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.409278 dbgpt-0.5.7rc0/dbgpt/agent/core/action/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      744 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/agent/core/action/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5785 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/agent/core/action/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      928 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/agent/core/action/blank_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9627 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/agent/core/agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5330 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/agent/core/agent_manage.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    36872 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/agent/core/base_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6063 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/agent/core/base_team.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.414840 dbgpt-0.5.7rc0/dbgpt/agent/core/memory/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      540 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/agent/core/memory/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9235 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/agent/core/memory/agent_memory.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    24306 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/agent/core/memory/base.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.417416 dbgpt-0.5.7rc0/dbgpt/agent/core/memory/gpts/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      554 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/agent/core/memory/gpts/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6837 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/agent/core/memory/gpts/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5799 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/agent/core/memory/gpts/default_gpts_memory.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7169 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/agent/core/memory/gpts/gpts_memory.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10793 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/agent/core/memory/hybrid.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5629 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/agent/core/memory/llm.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6836 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/agent/core/memory/long_term.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8549 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/agent/core/memory/short_term.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.420686 dbgpt-0.5.7rc0/dbgpt/agent/core/plan/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      914 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/agent/core/plan/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.423992 dbgpt-0.5.7rc0/dbgpt/agent/core/plan/awel/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       60 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/agent/core/plan/awel/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10736 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/agent/core/plan/awel/agent_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6386 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/agent/core/plan/awel/agent_operator_resource.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8646 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/agent/core/plan/awel/team_awel_layout.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4722 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/agent/core/plan/plan_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9210 2024-05-23 01:23:49.000000 dbgpt-0.5.7rc0/dbgpt/agent/core/plan/planner_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    13090 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/agent/core/plan/team_auto_plan.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.425375 dbgpt-0.5.7rc0/dbgpt/agent/core/profile/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      951 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/agent/core/profile/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    13263 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/agent/core/profile/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7484 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/agent/core/role.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      456 2024-04-10 14:49:01.000000 dbgpt-0.5.7rc0/dbgpt/agent/core/schema.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      560 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/agent/core/user_proxy_agent.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.431269 dbgpt-0.5.7rc0/dbgpt/agent/expand/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2560 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/agent/expand/Indicator_assistant_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)       26 2024-04-10 14:49:01.000000 dbgpt-0.5.7rc0/dbgpt/agent/expand/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.436043 dbgpt-0.5.7rc0/dbgpt/agent/expand/actions/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       32 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/agent/expand/actions/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3321 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/agent/expand/actions/chart_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5241 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/agent/expand/actions/code_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4087 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/agent/expand/actions/dashboard_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5449 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/agent/expand/actions/indicator_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5028 2024-05-16 09:22:35.000000 dbgpt-0.5.7rc0/dbgpt/agent/expand/actions/tool_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8090 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/agent/expand/code_assistant_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2993 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/agent/expand/dashboard_assistant_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5898 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/agent/expand/data_scientist_agent.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.438967 dbgpt-0.5.7rc0/dbgpt/agent/expand/resources/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       45 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/agent/expand/resources/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      789 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/agent/expand/resources/dbgpt_tool.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1350 2024-05-16 08:08:10.000000 dbgpt-0.5.7rc0/dbgpt/agent/expand/resources/host_tool.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1757 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/agent/expand/resources/search_tool.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    22213 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/agent/expand/retrieve_summary_assistant_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2560 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/agent/expand/summary_assistant_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2079 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/agent/expand/tool_assistant_agent.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.442491 dbgpt-0.5.7rc0/dbgpt/agent/resource/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1220 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/agent/resource/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7246 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/agent/resource/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6608 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/agent/resource/database.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2817 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/agent/resource/knowledge.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9358 2024-05-16 09:22:35.000000 dbgpt-0.5.7rc0/dbgpt/agent/resource/manage.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3490 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/agent/resource/pack.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.444439 dbgpt-0.5.7rc0/dbgpt/agent/resource/tool/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      108 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/agent/resource/tool/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.445258 dbgpt-0.5.7rc0/dbgpt/agent/resource/tool/autogpt/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       41 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/agent/resource/tool/autogpt/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6843 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/agent/resource/tool/autogpt/plugins_util.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    12486 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/agent/resource/tool/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1120 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/agent/resource/tool/exceptions.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7298 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/agent/resource/tool/pack.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.447291 dbgpt-0.5.7rc0/dbgpt/agent/util/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      114 2024-04-11 14:37:18.000000 dbgpt-0.5.7rc0/dbgpt/agent/util/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    15695 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/agent/util/api_call.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      850 2024-04-10 14:49:01.000000 dbgpt-0.5.7rc0/dbgpt/agent/util/cmp.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.449367 dbgpt-0.5.7rc0/dbgpt/agent/util/llm/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       22 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/agent/util/llm/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3473 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/agent/util/llm/llm.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6745 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/agent/util/llm/llm_client.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.450660 dbgpt-0.5.7rc0/dbgpt/agent/util/llm/strategy/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       27 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/agent/util/llm/strategy/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1291 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/agent/util/llm/strategy/priority.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.451632 dbgpt-0.5.7rc0/dbgpt/cli/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/cli/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5794 2024-04-09 19:22:18.000000 dbgpt-0.5.7rc0/dbgpt/cli/cli_scripts.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.458418 dbgpt-0.5.7rc0/dbgpt/client/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      154 2024-03-22 07:58:46.000000 dbgpt-0.5.7rc0/dbgpt/client/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7280 2024-04-17 10:27:40.000000 dbgpt-0.5.7rc0/dbgpt/client/_cli.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1413 2024-03-22 07:58:46.000000 dbgpt-0.5.7rc0/dbgpt/client/app.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    14335 2024-04-20 08:03:41.000000 dbgpt-0.5.7rc0/dbgpt/client/client.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3784 2024-04-20 08:03:41.000000 dbgpt-0.5.7rc0/dbgpt/client/datasource.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3568 2024-04-20 08:03:41.000000 dbgpt-0.5.7rc0/dbgpt/client/flow.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7003 2024-04-20 08:03:41.000000 dbgpt-0.5.7rc0/dbgpt/client/knowledge.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9455 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/client/schema.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10808 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/component.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.459854 dbgpt-0.5.7rc0/dbgpt/configs/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      530 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/configs/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    12720 2024-05-30 08:16:14.000000 dbgpt-0.5.7rc0/dbgpt/configs/model_config.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.460597 dbgpt-0.5.7rc0/dbgpt/core/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2714 2024-05-16 08:08:10.000000 dbgpt-0.5.7rc0/dbgpt/core/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.462155 dbgpt-0.5.7rc0/dbgpt/core/_private/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/core/_private/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1225 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/core/_private/example_base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3753 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/core/_private/prompt_registry.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.462732 dbgpt-0.5.7rc0/dbgpt/core/awel/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6103 2024-05-30 08:16:14.000000 dbgpt-0.5.7rc0/dbgpt/core/awel/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.465710 dbgpt-0.5.7rc0/dbgpt/core/awel/dag/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       26 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/core/awel/dag/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    29536 2024-03-26 04:37:36.000000 dbgpt-0.5.7rc0/dbgpt/core/awel/dag/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4143 2024-04-20 08:03:41.000000 dbgpt-0.5.7rc0/dbgpt/core/awel/dag/dag_manager.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3400 2024-05-30 08:16:14.000000 dbgpt-0.5.7rc0/dbgpt/core/awel/dag/loader.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.468914 dbgpt-0.5.7rc0/dbgpt/core/awel/flow/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      752 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/core/awel/flow/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    33942 2024-04-20 08:03:41.000000 dbgpt-0.5.7rc0/dbgpt/core/awel/flow/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1506 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/core/awel/flow/compat.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1577 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/core/awel/flow/exceptions.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    30038 2024-05-30 08:16:14.000000 dbgpt-0.5.7rc0/dbgpt/core/awel/flow/flow_factory.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.471683 dbgpt-0.5.7rc0/dbgpt/core/awel/operators/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       30 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/core/awel/operators/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    11390 2024-05-30 08:16:14.000000 dbgpt-0.5.7rc0/dbgpt/core/awel/operators/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    12071 2024-05-30 08:16:14.000000 dbgpt-0.5.7rc0/dbgpt/core/awel/operators/common_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4262 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/core/awel/operators/stream_operator.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.472936 dbgpt-0.5.7rc0/dbgpt/core/awel/resource/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       58 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/core/awel/resource/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      413 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/core/awel/resource/base.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.474688 dbgpt-0.5.7rc0/dbgpt/core/awel/runner/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      118 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/core/awel/runner/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4203 2024-03-25 14:27:11.000000 dbgpt-0.5.7rc0/dbgpt/core/awel/runner/job_manager.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7648 2024-05-09 08:02:51.000000 dbgpt-0.5.7rc0/dbgpt/core/awel/runner/local_runner.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.476813 dbgpt-0.5.7rc0/dbgpt/core/awel/task/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       26 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/core/awel/task/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    14271 2024-04-20 08:03:41.000000 dbgpt-0.5.7rc0/dbgpt/core/awel/task/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    20591 2024-03-25 14:27:11.000000 dbgpt-0.5.7rc0/dbgpt/core/awel/task/task_impl.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.480951 dbgpt-0.5.7rc0/dbgpt/core/awel/trigger/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       34 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/core/awel/trigger/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      519 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/core/awel/trigger/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6462 2024-04-09 19:22:18.000000 dbgpt-0.5.7rc0/dbgpt/core/awel/trigger/ext_http_trigger.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    37988 2024-04-20 08:03:41.000000 dbgpt-0.5.7rc0/dbgpt/core/awel/trigger/http_trigger.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6040 2024-03-27 07:42:00.000000 dbgpt-0.5.7rc0/dbgpt/core/awel/trigger/iterator_trigger.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7886 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/core/awel/trigger/trigger_manager.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.483170 dbgpt-0.5.7rc0/dbgpt/core/awel/util/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       22 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/core/awel/util/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      228 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/core/awel/util/_typing_util.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      500 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/core/awel/util/http_util.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2328 2024-04-20 08:03:41.000000 dbgpt-0.5.7rc0/dbgpt/core/awel/util/parameter_util.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.491147 dbgpt-0.5.7rc0/dbgpt/core/interface/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      102 2024-03-22 07:58:44.000000 dbgpt-0.5.7rc0/dbgpt/core/interface/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3546 2024-03-22 07:58:44.000000 dbgpt-0.5.7rc0/dbgpt/core/interface/cache.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1508 2024-05-16 08:08:10.000000 dbgpt-0.5.7rc0/dbgpt/core/interface/embeddings.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7410 2024-03-23 08:18:41.000000 dbgpt-0.5.7rc0/dbgpt/core/interface/evaluation.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4294 2024-05-13 11:08:58.000000 dbgpt-0.5.7rc0/dbgpt/core/interface/knowledge.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    31110 2024-04-20 08:03:41.000000 dbgpt-0.5.7rc0/dbgpt/core/interface/llm.py
+-rwxr-xr-x   0 staneyffer   (501) staff       (20)    43156 2024-05-30 08:16:14.000000 dbgpt-0.5.7rc0/dbgpt/core/interface/message.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.496358 dbgpt-0.5.7rc0/dbgpt/core/interface/operators/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       55 2024-03-22 07:58:44.000000 dbgpt-0.5.7rc0/dbgpt/core/interface/operators/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4438 2024-03-25 14:27:11.000000 dbgpt-0.5.7rc0/dbgpt/core/interface/operators/composer_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    18962 2024-05-23 08:15:22.000000 dbgpt-0.5.7rc0/dbgpt/core/interface/operators/llm_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    23685 2024-03-25 14:27:11.000000 dbgpt-0.5.7rc0/dbgpt/core/interface/operators/message_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    16465 2024-04-20 08:03:41.000000 dbgpt-0.5.7rc0/dbgpt/core/interface/operators/prompt_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      767 2024-03-22 07:58:44.000000 dbgpt-0.5.7rc0/dbgpt/core/interface/operators/retriever.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10805 2024-04-09 19:22:18.000000 dbgpt-0.5.7rc0/dbgpt/core/interface/output_parser.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    26624 2024-05-30 08:16:14.000000 dbgpt-0.5.7rc0/dbgpt/core/interface/prompt.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1748 2024-04-20 08:03:41.000000 dbgpt-0.5.7rc0/dbgpt/core/interface/serialization.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    15126 2024-04-20 08:03:41.000000 dbgpt-0.5.7rc0/dbgpt/core/interface/storage.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.496989 dbgpt-0.5.7rc0/dbgpt/core/operators/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1509 2024-03-22 07:58:44.000000 dbgpt-0.5.7rc0/dbgpt/core/operators/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.499429 dbgpt-0.5.7rc0/dbgpt/core/operators/flow/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      340 2024-03-25 14:27:11.000000 dbgpt-0.5.7rc0/dbgpt/core/operators/flow/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9546 2024-03-25 14:27:11.000000 dbgpt-0.5.7rc0/dbgpt/core/operators/flow/composer_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2601 2024-03-25 14:27:11.000000 dbgpt-0.5.7rc0/dbgpt/core/operators/flow/dict_operator.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.500697 dbgpt-0.5.7rc0/dbgpt/core/schema/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/core/schema/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8837 2024-05-16 08:08:10.000000 dbgpt-0.5.7rc0/dbgpt/core/schema/api.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.505352 dbgpt-0.5.7rc0/dbgpt/datasource/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      412 2024-03-22 07:58:44.000000 dbgpt-0.5.7rc0/dbgpt/datasource/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6802 2024-04-30 09:57:48.000000 dbgpt-0.5.7rc0/dbgpt/datasource/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3909 2024-03-22 07:58:44.000000 dbgpt-0.5.7rc0/dbgpt/datasource/conn_spark.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5848 2024-05-16 08:08:10.000000 dbgpt-0.5.7rc0/dbgpt/datasource/conn_tugraph.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      923 2024-03-22 07:58:44.000000 dbgpt-0.5.7rc0/dbgpt/datasource/db_conn_info.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.507167 dbgpt-0.5.7rc0/dbgpt/datasource/manages/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      157 2024-03-22 07:58:44.000000 dbgpt-0.5.7rc0/dbgpt/datasource/manages/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9173 2024-03-28 01:32:30.000000 dbgpt-0.5.7rc0/dbgpt/datasource/manages/connect_config_db.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8710 2024-05-20 15:27:34.000000 dbgpt-0.5.7rc0/dbgpt/datasource/manages/connector_manager.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.507898 dbgpt-0.5.7rc0/dbgpt/datasource/nosql/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-03-22 07:58:44.000000 dbgpt-0.5.7rc0/dbgpt/datasource/nosql/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.508950 dbgpt-0.5.7rc0/dbgpt/datasource/operators/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      128 2024-03-28 01:32:23.000000 dbgpt-0.5.7rc0/dbgpt/datasource/operators/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      770 2024-03-22 07:58:44.000000 dbgpt-0.5.7rc0/dbgpt/datasource/operators/datasource_operator.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.515775 dbgpt-0.5.7rc0/dbgpt/datasource/rdbms/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       30 2024-03-22 07:58:44.000000 dbgpt-0.5.7rc0/dbgpt/datasource/rdbms/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    23230 2024-03-22 07:58:44.000000 dbgpt-0.5.7rc0/dbgpt/datasource/rdbms/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    12710 2024-04-20 08:03:41.000000 dbgpt-0.5.7rc0/dbgpt/datasource/rdbms/conn_clickhouse.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6407 2024-03-22 07:58:44.000000 dbgpt-0.5.7rc0/dbgpt/datasource/rdbms/conn_doris.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2473 2024-03-25 06:53:38.000000 dbgpt-0.5.7rc0/dbgpt/datasource/rdbms/conn_duckdb.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1417 2024-03-22 07:58:44.000000 dbgpt-0.5.7rc0/dbgpt/datasource/rdbms/conn_hive.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1329 2024-03-22 07:58:44.000000 dbgpt-0.5.7rc0/dbgpt/datasource/rdbms/conn_mssql.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      295 2024-03-22 07:58:44.000000 dbgpt-0.5.7rc0/dbgpt/datasource/rdbms/conn_mysql.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8185 2024-03-22 07:58:44.000000 dbgpt-0.5.7rc0/dbgpt/datasource/rdbms/conn_postgresql.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10006 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/datasource/rdbms/conn_sqlite.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5681 2024-03-22 07:58:44.000000 dbgpt-0.5.7rc0/dbgpt/datasource/rdbms/conn_starrocks.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8958 2024-05-20 15:27:34.000000 dbgpt-0.5.7rc0/dbgpt/datasource/rdbms/conn_vertica.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.516606 dbgpt-0.5.7rc0/dbgpt/datasource/rdbms/dialect/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-03-22 07:58:44.000000 dbgpt-0.5.7rc0/dbgpt/datasource/rdbms/dialect/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.517328 dbgpt-0.5.7rc0/dbgpt/datasource/rdbms/dialect/starrocks/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      648 2024-03-22 07:58:44.000000 dbgpt-0.5.7rc0/dbgpt/datasource/rdbms/dialect/starrocks/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.519068 dbgpt-0.5.7rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      820 2024-03-22 07:58:44.000000 dbgpt-0.5.7rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3186 2024-03-22 07:58:44.000000 dbgpt-0.5.7rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/datatype.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7507 2024-03-22 07:58:44.000000 dbgpt-0.5.7rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/dialect.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      116 2024-03-22 07:58:44.000000 dbgpt-0.5.7rc0/dbgpt/datasource/redis.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.520076 dbgpt-0.5.7rc0/dbgpt/experimental/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      127 2024-05-30 08:16:14.000000 dbgpt-0.5.7rc0/dbgpt/experimental/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.521847 dbgpt-0.5.7rc0/dbgpt/experimental/intent/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       31 2024-05-30 08:16:14.000000 dbgpt-0.5.7rc0/dbgpt/experimental/intent/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8151 2024-05-30 08:16:14.000000 dbgpt-0.5.7rc0/dbgpt/experimental/intent/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3343 2024-05-30 08:16:14.000000 dbgpt-0.5.7rc0/dbgpt/experimental/intent/operators.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.524664 dbgpt-0.5.7rc0/dbgpt/model/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      320 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/model/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.531905 dbgpt-0.5.7rc0/dbgpt/model/adapter/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/model/adapter/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    19880 2024-05-13 11:08:58.000000 dbgpt-0.5.7rc0/dbgpt/model/adapter/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5052 2024-05-16 08:08:10.000000 dbgpt-0.5.7rc0/dbgpt/model/adapter/embeddings_loader.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8687 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/model/adapter/fschat_adapter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    16312 2024-05-30 08:16:14.000000 dbgpt-0.5.7rc0/dbgpt/model/adapter/hf_adapter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    15595 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/model/adapter/loader.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5519 2024-05-16 08:08:10.000000 dbgpt-0.5.7rc0/dbgpt/model/adapter/model_adapter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    17037 2024-04-09 19:22:18.000000 dbgpt-0.5.7rc0/dbgpt/model/adapter/old_adapter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    11240 2024-05-07 09:44:51.000000 dbgpt-0.5.7rc0/dbgpt/model/adapter/proxy_adapter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3587 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/model/adapter/template.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3495 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/model/adapter/vllm_adapter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3050 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/model/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    13971 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/model/cli.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.533179 dbgpt-0.5.7rc0/dbgpt/model/operators/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      341 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/model/operators/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4981 2024-03-25 14:27:11.000000 dbgpt-0.5.7rc0/dbgpt/model/operators/llm_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    19197 2024-05-16 08:08:10.000000 dbgpt-0.5.7rc0/dbgpt/model/parameter.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.534320 dbgpt-0.5.7rc0/dbgpt/model/proxy/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1185 2024-05-07 09:44:51.000000 dbgpt-0.5.7rc0/dbgpt/model/proxy/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7967 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/model/proxy/base.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.543149 dbgpt-0.5.7rc0/dbgpt/model/proxy/llms/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      306 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/model/proxy/llms/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3077 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/model/proxy/llms/baichuan.py
+-rwxr-xr-x   0 staneyffer   (501) staff       (20)     2325 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/model/proxy/llms/bard.py
+-rwxr-xr-x   0 staneyffer   (501) staff       (20)    10636 2024-04-10 19:49:14.000000 dbgpt-0.5.7rc0/dbgpt/model/proxy/llms/chatgpt.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      200 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/model/proxy/llms/claude.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3391 2024-05-07 09:44:51.000000 dbgpt-0.5.7rc0/dbgpt/model/proxy/llms/deepseek.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6485 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/model/proxy/llms/gemini.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3336 2024-04-10 19:49:14.000000 dbgpt-0.5.7rc0/dbgpt/model/proxy/llms/moonshot.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3279 2024-04-30 09:57:48.000000 dbgpt-0.5.7rc0/dbgpt/model/proxy/llms/ollama.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1350 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/model/proxy/llms/proxy_model.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7602 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/model/proxy/llms/spark.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3720 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/model/proxy/llms/tongyi.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7011 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/model/proxy/llms/wenxin.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2859 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/model/proxy/llms/yi.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3796 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/model/proxy/llms/zhipu.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.545180 dbgpt-0.5.7rc0/dbgpt/model/utils/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/model/utils/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9274 2024-03-27 07:42:00.000000 dbgpt-0.5.7rc0/dbgpt/model/utils/chatgpt_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2365 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/model/utils/llm_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3101 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/model/utils/token_utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.546417 dbgpt-0.5.7rc0/dbgpt/rag/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      200 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/rag/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.550178 dbgpt-0.5.7rc0/dbgpt/rag/assembler/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      431 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/rag/assembler/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2884 2024-05-16 08:08:10.000000 dbgpt-0.5.7rc0/dbgpt/rag/assembler/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8082 2024-05-30 08:16:14.000000 dbgpt-0.5.7rc0/dbgpt/rag/assembler/bm25.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4815 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/rag/assembler/db_schema.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5829 2024-05-24 07:02:47.000000 dbgpt-0.5.7rc0/dbgpt/rag/assembler/embedding.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4611 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/rag/assembler/summary.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6792 2024-03-25 14:27:11.000000 dbgpt-0.5.7rc0/dbgpt/rag/chunk_manager.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.554133 dbgpt-0.5.7rc0/dbgpt/rag/embedding/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      926 2024-05-16 08:08:10.000000 dbgpt-0.5.7rc0/dbgpt/rag/embedding/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1200 2024-05-13 11:08:58.000000 dbgpt-0.5.7rc0/dbgpt/rag/embedding/_wrapped.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9369 2024-05-16 08:08:10.000000 dbgpt-0.5.7rc0/dbgpt/rag/embedding/embedding_factory.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    28118 2024-05-16 08:08:10.000000 dbgpt-0.5.7rc0/dbgpt/rag/embedding/embeddings.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4737 2024-05-16 08:08:10.000000 dbgpt-0.5.7rc0/dbgpt/rag/embedding/rerank.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.555215 dbgpt-0.5.7rc0/dbgpt/rag/evaluation/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      271 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/rag/evaluation/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8772 2024-04-30 09:57:48.000000 dbgpt-0.5.7rc0/dbgpt/rag/evaluation/retriever.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.557359 dbgpt-0.5.7rc0/dbgpt/rag/extractor/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      152 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/rag/extractor/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1314 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/rag/extractor/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6352 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/rag/extractor/summary.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.557976 dbgpt-0.5.7rc0/dbgpt/rag/graph/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       28 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/rag/graph/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.559068 dbgpt-0.5.7rc0/dbgpt/rag/index/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       24 2024-05-16 08:08:10.000000 dbgpt-0.5.7rc0/dbgpt/rag/index/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6376 2024-05-24 08:06:35.000000 dbgpt-0.5.7rc0/dbgpt/rag/index/base.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.567663 dbgpt-0.5.7rc0/dbgpt/rag/knowledge/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1394 2024-05-16 09:22:35.000000 dbgpt-0.5.7rc0/dbgpt/rag/knowledge/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5601 2024-05-16 09:22:35.000000 dbgpt-0.5.7rc0/dbgpt/rag/knowledge/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3541 2024-04-10 06:34:08.000000 dbgpt-0.5.7rc0/dbgpt/rag/knowledge/csv.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2389 2024-04-30 09:57:48.000000 dbgpt-0.5.7rc0/dbgpt/rag/knowledge/datasource.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2580 2024-04-10 06:34:08.000000 dbgpt-0.5.7rc0/dbgpt/rag/knowledge/docx.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3796 2024-05-16 09:22:35.000000 dbgpt-0.5.7rc0/dbgpt/rag/knowledge/excel.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6675 2024-05-16 09:22:35.000000 dbgpt-0.5.7rc0/dbgpt/rag/knowledge/factory.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3024 2024-04-10 06:34:08.000000 dbgpt-0.5.7rc0/dbgpt/rag/knowledge/html.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)       22 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/rag/knowledge/json.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2600 2024-04-10 06:34:08.000000 dbgpt-0.5.7rc0/dbgpt/rag/knowledge/markdown.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3378 2024-04-10 06:34:08.000000 dbgpt-0.5.7rc0/dbgpt/rag/knowledge/pdf.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2886 2024-04-10 06:34:08.000000 dbgpt-0.5.7rc0/dbgpt/rag/knowledge/pptx.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1807 2024-04-10 06:34:08.000000 dbgpt-0.5.7rc0/dbgpt/rag/knowledge/string.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2504 2024-04-10 06:34:08.000000 dbgpt-0.5.7rc0/dbgpt/rag/knowledge/txt.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2159 2024-05-13 11:08:58.000000 dbgpt-0.5.7rc0/dbgpt/rag/knowledge/url.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.574483 dbgpt-0.5.7rc0/dbgpt/rag/operators/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      971 2024-03-25 14:27:11.000000 dbgpt-0.5.7rc0/dbgpt/rag/operators/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      654 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/rag/operators/assembler.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      743 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/rag/operators/datasource.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2956 2024-03-28 01:32:23.000000 dbgpt-0.5.7rc0/dbgpt/rag/operators/db_schema.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6584 2024-03-25 14:27:11.000000 dbgpt-0.5.7rc0/dbgpt/rag/operators/embedding.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2085 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/rag/operators/evaluation.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4534 2024-03-25 14:27:11.000000 dbgpt-0.5.7rc0/dbgpt/rag/operators/knowledge.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1268 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/rag/operators/rerank.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3199 2024-03-25 14:27:11.000000 dbgpt-0.5.7rc0/dbgpt/rag/operators/rewrite.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1466 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/rag/operators/schema_linking.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4156 2024-03-25 14:27:11.000000 dbgpt-0.5.7rc0/dbgpt/rag/operators/summary.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.579349 dbgpt-0.5.7rc0/dbgpt/rag/retriever/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      503 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/rag/retriever/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4379 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/rag/retriever/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6216 2024-05-30 08:16:14.000000 dbgpt-0.5.7rc0/dbgpt/rag/retriever/bm25.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7270 2024-04-10 06:34:08.000000 dbgpt-0.5.7rc0/dbgpt/rag/retriever/db_schema.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8947 2024-05-16 08:08:10.000000 dbgpt-0.5.7rc0/dbgpt/rag/retriever/embedding.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10218 2024-05-20 15:27:34.000000 dbgpt-0.5.7rc0/dbgpt/rag/retriever/rerank.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5223 2024-03-25 14:27:11.000000 dbgpt-0.5.7rc0/dbgpt/rag/retriever/rewrite.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5186 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/rag/retriever/time_weighted.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.581119 dbgpt-0.5.7rc0/dbgpt/rag/schemalinker/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       30 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/rag/schemalinker/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1624 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/rag/schemalinker/base_linker.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3392 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/rag/schemalinker/schema_linking.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.583551 dbgpt-0.5.7rc0/dbgpt/rag/summary/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      420 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/rag/summary/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1226 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/rag/summary/db_summary.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5210 2024-04-30 09:57:48.000000 dbgpt-0.5.7rc0/dbgpt/rag/summary/db_summary_client.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4575 2024-04-30 09:57:48.000000 dbgpt-0.5.7rc0/dbgpt/rag/summary/gdbms_db_summary.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4443 2024-04-13 17:38:21.000000 dbgpt-0.5.7rc0/dbgpt/rag/summary/rdbms_db_summary.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.586295 dbgpt-0.5.7rc0/dbgpt/rag/text_splitter/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      539 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/rag/text_splitter/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1497 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/rag/text_splitter/pre_text_splitter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    32461 2024-04-30 09:57:48.000000 dbgpt-0.5.7rc0/dbgpt/rag/text_splitter/text_splitter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6913 2024-04-20 08:03:41.000000 dbgpt-0.5.7rc0/dbgpt/rag/text_splitter/token_splitter.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.590442 dbgpt-0.5.7rc0/dbgpt/rag/transformer/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       30 2024-05-16 08:08:10.000000 dbgpt-0.5.7rc0/dbgpt/rag/transformer/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      582 2024-05-16 08:08:10.000000 dbgpt-0.5.7rc0/dbgpt/rag/transformer/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1806 2024-05-16 08:08:10.000000 dbgpt-0.5.7rc0/dbgpt/rag/transformer/keyword_extractor.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1875 2024-05-16 08:08:10.000000 dbgpt-0.5.7rc0/dbgpt/rag/transformer/llm_extractor.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      199 2024-05-16 08:08:10.000000 dbgpt-0.5.7rc0/dbgpt/rag/transformer/text2cypher.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      190 2024-05-16 08:08:10.000000 dbgpt-0.5.7rc0/dbgpt/rag/transformer/text2gql.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      195 2024-05-16 08:08:10.000000 dbgpt-0.5.7rc0/dbgpt/rag/transformer/text2vector.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2604 2024-05-16 08:08:10.000000 dbgpt-0.5.7rc0/dbgpt/rag/transformer/triplet_extractor.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.591629 dbgpt-0.5.7rc0/dbgpt/storage/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       67 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/storage/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.594864 dbgpt-0.5.7rc0/dbgpt/storage/cache/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      384 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/storage/cache/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)       24 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/storage/cache/embedding_cache.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6185 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/storage/cache/llm_cache.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4472 2024-04-17 10:41:53.000000 dbgpt-0.5.7rc0/dbgpt/storage/cache/manager.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9995 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/storage/cache/operators.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.595642 dbgpt-0.5.7rc0/dbgpt/storage/cache/protocol/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       27 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/storage/cache/protocol/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.596383 dbgpt-0.5.7rc0/dbgpt/storage/cache/storage/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       47 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/storage/cache/storage/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8913 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/storage/cache/storage/base.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.597420 dbgpt-0.5.7rc0/dbgpt/storage/cache/storage/disk/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       41 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/storage/cache/storage/disk/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3254 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/storage/cache/storage/disk/disk_storage.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.599273 dbgpt-0.5.7rc0/dbgpt/storage/chat_history/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      438 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/storage/chat_history/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4736 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/storage/chat_history/chat_history_db.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5829 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/storage/chat_history/storage_adapter.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.602955 dbgpt-0.5.7rc0/dbgpt/storage/graph_store/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      965 2024-05-16 08:08:10.000000 dbgpt-0.5.7rc0/dbgpt/storage/graph_store/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1815 2024-05-16 08:08:10.000000 dbgpt-0.5.7rc0/dbgpt/storage/graph_store/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1441 2024-05-16 08:08:10.000000 dbgpt-0.5.7rc0/dbgpt/storage/graph_store/factory.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    14213 2024-05-16 08:08:10.000000 dbgpt-0.5.7rc0/dbgpt/storage/graph_store/graph.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2895 2024-05-16 08:08:10.000000 dbgpt-0.5.7rc0/dbgpt/storage/graph_store/memgraph_store.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1748 2024-05-16 08:08:10.000000 dbgpt-0.5.7rc0/dbgpt/storage/graph_store/neo4j_store.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8922 2024-05-16 08:08:10.000000 dbgpt-0.5.7rc0/dbgpt/storage/graph_store/tugraph_store.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.606316 dbgpt-0.5.7rc0/dbgpt/storage/knowledge_graph/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       21 2024-05-16 08:08:10.000000 dbgpt-0.5.7rc0/dbgpt/storage/knowledge_graph/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      830 2024-05-16 08:08:10.000000 dbgpt-0.5.7rc0/dbgpt/storage/knowledge_graph/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5703 2024-05-24 07:02:47.000000 dbgpt-0.5.7rc0/dbgpt/storage/knowledge_graph/knowledge_graph.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1321 2024-05-16 08:08:10.000000 dbgpt-0.5.7rc0/dbgpt/storage/knowledge_graph/open_spg.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.611283 dbgpt-0.5.7rc0/dbgpt/storage/metadata/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      476 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/storage/metadata/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9345 2024-04-20 08:03:41.000000 dbgpt-0.5.7rc0/dbgpt/storage/metadata/_base_dao.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1041 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/storage/metadata/db_factory.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    18854 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/storage/metadata/db_manager.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5503 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/storage/metadata/db_storage.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1924 2024-05-20 15:27:34.000000 dbgpt-0.5.7rc0/dbgpt/storage/schema.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.621355 dbgpt-0.5.7rc0/dbgpt/storage/vector_store/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2515 2024-05-16 08:08:10.000000 dbgpt-0.5.7rc0/dbgpt/storage/vector_store/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5348 2024-05-24 08:06:41.000000 dbgpt-0.5.7rc0/dbgpt/storage/vector_store/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10905 2024-05-24 07:02:47.000000 dbgpt-0.5.7rc0/dbgpt/storage/vector_store/chroma_store.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10396 2024-05-24 08:06:35.000000 dbgpt-0.5.7rc0/dbgpt/storage/vector_store/connector.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    15069 2024-05-24 07:02:47.000000 dbgpt-0.5.7rc0/dbgpt/storage/vector_store/elastic_store.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1234 2024-04-20 08:03:41.000000 dbgpt-0.5.7rc0/dbgpt/storage/vector_store/filters.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    22510 2024-05-24 07:02:47.000000 dbgpt-0.5.7rc0/dbgpt/storage/vector_store/milvus_store.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    29166 2024-05-24 07:02:47.000000 dbgpt-0.5.7rc0/dbgpt/storage/vector_store/oceanbase_store.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3782 2024-05-24 07:02:47.000000 dbgpt-0.5.7rc0/dbgpt/storage/vector_store/pgvector_store.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6753 2024-05-24 07:02:47.000000 dbgpt-0.5.7rc0/dbgpt/storage/vector_store/weaviate_store.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.654960 dbgpt-0.5.7rc0/dbgpt/util/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      413 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/util/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    14058 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/util/_db_migration_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3861 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/util/annotations.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4659 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/util/api_utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.655763 dbgpt-0.5.7rc0/dbgpt/util/benchmarks/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/util/benchmarks/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.657747 dbgpt-0.5.7rc0/dbgpt/util/benchmarks/llm/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/util/benchmarks/llm/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10778 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/util/benchmarks/llm/fastchat_benchmarks_inference.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9317 2024-04-20 08:03:41.000000 dbgpt-0.5.7rc0/dbgpt/util/benchmarks/llm/llm_benchmarks.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3166 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/util/cache_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1703 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/util/chat_util.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    19326 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/util/code_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5840 2024-04-12 06:30:46.000000 dbgpt-0.5.7rc0/dbgpt/util/command_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1791 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/util/config_utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.659401 dbgpt-0.5.7rc0/dbgpt/util/configure/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       56 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/util/configure/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4719 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/util/configure/base.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.661018 dbgpt-0.5.7rc0/dbgpt/util/console/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       70 2024-03-27 07:42:00.000000 dbgpt-0.5.7rc0/dbgpt/util/console/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1827 2024-03-27 07:42:00.000000 dbgpt-0.5.7rc0/dbgpt/util/console/console.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      780 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/util/custom_data_structure.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      247 2024-04-09 19:22:04.000000 dbgpt-0.5.7rc0/dbgpt/util/date_utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.665863 dbgpt-0.5.7rc0/dbgpt/util/dbgpts/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/util/dbgpts/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1990 2024-05-16 09:22:35.000000 dbgpt-0.5.7rc0/dbgpt/util/dbgpts/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5982 2024-03-27 07:42:00.000000 dbgpt-0.5.7rc0/dbgpt/util/dbgpts/cli.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    15672 2024-05-30 08:16:14.000000 dbgpt-0.5.7rc0/dbgpt/util/dbgpts/loader.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    11883 2024-04-15 03:42:53.000000 dbgpt-0.5.7rc0/dbgpt/util/dbgpts/repo.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    12501 2024-05-30 08:16:14.000000 dbgpt-0.5.7rc0/dbgpt/util/dbgpts/template.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      533 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/util/error_types.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2886 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/util/executor_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3929 2024-04-20 08:03:41.000000 dbgpt-0.5.7rc0/dbgpt/util/fastapi.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1807 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/util/formatting.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5484 2024-05-15 02:02:22.000000 dbgpt-0.5.7rc0/dbgpt/util/function_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    12937 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/util/global_helper.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1976 2024-03-25 14:27:11.000000 dbgpt-0.5.7rc0/dbgpt/util/i18n_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2612 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/util/id_generator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3673 2024-04-10 14:49:01.000000 dbgpt-0.5.7rc0/dbgpt/util/json_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      238 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/util/memory_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2679 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/util/model_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      893 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/util/module_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      704 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/util/net_utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.667315 dbgpt-0.5.7rc0/dbgpt/util/network/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-04-09 19:22:18.000000 dbgpt-0.5.7rc0/dbgpt/util/network/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9818 2024-04-20 08:03:41.000000 dbgpt-0.5.7rc0/dbgpt/util/network/_cli.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3488 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/util/openai_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      618 2024-04-20 08:03:41.000000 dbgpt-0.5.7rc0/dbgpt/util/pagination_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    27722 2024-05-16 08:27:38.000000 dbgpt-0.5.7rc0/dbgpt/util/parameter_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      105 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/util/path_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      629 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/util/pd_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8747 2024-04-20 08:03:41.000000 dbgpt-0.5.7rc0/dbgpt/util/prompt_util.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1676 2024-04-18 02:11:54.000000 dbgpt-0.5.7rc0/dbgpt/util/retry.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.668577 dbgpt-0.5.7rc0/dbgpt/util/serialization/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/util/serialization/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1859 2024-04-17 10:39:42.000000 dbgpt-0.5.7rc0/dbgpt/util/serialization/json_serialization.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2399 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/util/similarity_util.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      697 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/util/singleton.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.673751 dbgpt-0.5.7rc0/dbgpt/util/speech/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/util/speech/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1119 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/util/speech/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1180 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/util/speech/brian.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2985 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/util/speech/eleven_labs.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      467 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/util/speech/gtts.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      523 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/util/speech/macos_tts.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1441 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/util/speech/say.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2526 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/util/splitter_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3006 2024-04-10 14:49:01.000000 dbgpt-0.5.7rc0/dbgpt/util/string_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7537 2024-04-09 19:22:18.000000 dbgpt-0.5.7rc0/dbgpt/util/system_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1019 2024-05-07 02:03:17.000000 dbgpt-0.5.7rc0/dbgpt/util/time_utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.678831 dbgpt-0.5.7rc0/dbgpt/util/tracer/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      723 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/util/tracer/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7264 2024-04-11 14:37:18.000000 dbgpt-0.5.7rc0/dbgpt/util/tracer/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5743 2024-04-11 14:37:18.000000 dbgpt-0.5.7rc0/dbgpt/util/tracer/span_storage.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    18465 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/util/tracer/tracer_cli.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7846 2024-04-17 04:06:45.000000 dbgpt-0.5.7rc0/dbgpt/util/tracer/tracer_impl.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1504 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/util/tracer/tracer_middleware.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5246 2024-03-22 07:58:45.000000 dbgpt-0.5.7rc0/dbgpt/util/utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.681035 dbgpt-0.5.7rc0/dbgpt/vis/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      602 2024-04-11 14:37:18.000000 dbgpt-0.5.7rc0/dbgpt/vis/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1050 2024-04-10 14:49:01.000000 dbgpt-0.5.7rc0/dbgpt/vis/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1220 2024-04-10 14:49:01.000000 dbgpt-0.5.7rc0/dbgpt/vis/client.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.687476 dbgpt-0.5.7rc0/dbgpt/vis/tags/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       16 2024-04-10 14:49:01.000000 dbgpt-0.5.7rc0/dbgpt/vis/tags/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      284 2024-04-10 14:49:01.000000 dbgpt-0.5.7rc0/dbgpt/vis/tags/vis_agent_message.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      257 2024-04-10 14:49:01.000000 dbgpt-0.5.7rc0/dbgpt/vis/tags/vis_agent_plans.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3080 2024-04-10 14:49:01.000000 dbgpt-0.5.7rc0/dbgpt/vis/tags/vis_chart.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      256 2024-04-10 14:49:01.000000 dbgpt-0.5.7rc0/dbgpt/vis/tags/vis_code.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1957 2024-04-10 14:49:01.000000 dbgpt-0.5.7rc0/dbgpt/vis/tags/vis_dashboard.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      258 2024-04-10 14:49:01.000000 dbgpt-0.5.7rc0/dbgpt/vis/tags/vis_gpts_execution.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      311 2024-04-10 14:49:01.000000 dbgpt-0.5.7rc0/dbgpt/vis/tags/vis_gpts_result.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      253 2024-04-10 14:49:01.000000 dbgpt-0.5.7rc0/dbgpt/vis/tags/vis_plugin.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-30 09:29:16.397166 dbgpt-0.5.7rc0/dbgpt.egg-info/
+-rw-r--r--   0 staneyffer   (501) staff       (20)    32191 2024-05-30 09:29:16.000000 dbgpt-0.5.7rc0/dbgpt.egg-info/PKG-INFO
+-rw-r--r--   0 staneyffer   (501) staff       (20)    14411 2024-05-30 09:29:16.000000 dbgpt-0.5.7rc0/dbgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 staneyffer   (501) staff       (20)        1 2024-05-30 09:29:16.000000 dbgpt-0.5.7rc0/dbgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 staneyffer   (501) staff       (20)       53 2024-05-30 09:29:16.000000 dbgpt-0.5.7rc0/dbgpt.egg-info/entry_points.txt
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5273 2024-05-30 09:29:16.000000 dbgpt-0.5.7rc0/dbgpt.egg-info/requires.txt
+-rw-r--r--   0 staneyffer   (501) staff       (20)        6 2024-05-30 09:29:16.000000 dbgpt-0.5.7rc0/dbgpt.egg-info/top_level.txt
+-rw-r--r--   0 staneyffer   (501) staff       (20)       38 2024-05-30 09:29:16.766472 dbgpt-0.5.7rc0/setup.cfg
+-rw-r--r--   0 staneyffer   (501) staff       (20)    24437 2024-05-30 08:16:14.000000 dbgpt-0.5.7rc0/setup.py
```

### Comparing `dbgpt-0.5.6rc0/LICENSE` & `dbgpt-0.5.7rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/PKG-INFO` & `dbgpt-0.5.7rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbgpt
-Version: 0.5.6rc0
+Version: 0.5.7rc0
 Summary: DB-GPT is an experimental open-source project that uses localized GPT large models to interact with your data and environment. With this solution, you can be assured that there is no risk of data leakage, and your data is 100% private and secure.
 Home-page: https://github.com/eosphoros-ai/DB-GPT
 Author: csunny
 Author-email: cfqcsunny@gmail.com
 License: https://opensource.org/license/mit/
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -13,155 +13,162 @@
 Requires-Dist: chardet==5.1.0
 Requires-Dist: importlib-resources==5.12.0
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: cachetools
 Requires-Dist: pydantic>=2.6.0
 Requires-Dist: typeguard
 Requires-Dist: snowflake-id
+Requires-Dist: typing_inspect
 Provides-Extra: core
-Requires-Dist: cachetools; extra == "core"
-Requires-Dist: importlib-resources==5.12.0; extra == "core"
-Requires-Dist: python-dotenv==1.0.0; extra == "core"
-Requires-Dist: aiohttp==3.8.4; extra == "core"
-Requires-Dist: snowflake-id; extra == "core"
 Requires-Dist: chardet==5.1.0; extra == "core"
+Requires-Dist: typing_inspect; extra == "core"
 Requires-Dist: typeguard; extra == "core"
 Requires-Dist: pydantic>=2.6.0; extra == "core"
+Requires-Dist: snowflake-id; extra == "core"
+Requires-Dist: python-dotenv==1.0.0; extra == "core"
+Requires-Dist: importlib-resources==5.12.0; extra == "core"
+Requires-Dist: aiohttp==3.8.4; extra == "core"
+Requires-Dist: cachetools; extra == "core"
 Provides-Extra: client
-Requires-Dist: cachetools; extra == "client"
 Requires-Dist: fastapi>=0.100.0; extra == "client"
-Requires-Dist: httpx; extra == "client"
-Requires-Dist: importlib-resources==5.12.0; extra == "client"
-Requires-Dist: python-dotenv==1.0.0; extra == "client"
-Requires-Dist: aiohttp==3.8.4; extra == "client"
-Requires-Dist: snowflake-id; extra == "client"
 Requires-Dist: chardet==5.1.0; extra == "client"
+Requires-Dist: typing_inspect; extra == "client"
 Requires-Dist: typeguard; extra == "client"
 Requires-Dist: pydantic>=2.6.0; extra == "client"
+Requires-Dist: snowflake-id; extra == "client"
+Requires-Dist: python-dotenv==1.0.0; extra == "client"
+Requires-Dist: importlib-resources==5.12.0; extra == "client"
+Requires-Dist: aiohttp==3.8.4; extra == "client"
+Requires-Dist: cachetools; extra == "client"
+Requires-Dist: httpx; extra == "client"
 Provides-Extra: cli
-Requires-Dist: cachetools; extra == "cli"
 Requires-Dist: fastapi>=0.100.0; extra == "cli"
 Requires-Dist: psutil==5.9.4; extra == "cli"
+Requires-Dist: chardet==5.1.0; extra == "cli"
+Requires-Dist: typing_inspect; extra == "cli"
 Requires-Dist: tomlkit; extra == "cli"
-Requires-Dist: httpx; extra == "cli"
-Requires-Dist: importlib-resources==5.12.0; extra == "cli"
-Requires-Dist: python-dotenv==1.0.0; extra == "cli"
-Requires-Dist: prettytable; extra == "cli"
-Requires-Dist: aiohttp==3.8.4; extra == "cli"
+Requires-Dist: typeguard; extra == "cli"
+Requires-Dist: rich; extra == "cli"
+Requires-Dist: pydantic>=2.6.0; extra == "cli"
 Requires-Dist: snowflake-id; extra == "cli"
 Requires-Dist: colorama==0.4.6; extra == "cli"
-Requires-Dist: rich; extra == "cli"
+Requires-Dist: python-dotenv==1.0.0; extra == "cli"
+Requires-Dist: importlib-resources==5.12.0; extra == "cli"
 Requires-Dist: click; extra == "cli"
-Requires-Dist: chardet==5.1.0; extra == "cli"
-Requires-Dist: typeguard; extra == "cli"
-Requires-Dist: pydantic>=2.6.0; extra == "cli"
+Requires-Dist: prettytable; extra == "cli"
+Requires-Dist: aiohttp==3.8.4; extra == "cli"
+Requires-Dist: cachetools; extra == "cli"
+Requires-Dist: httpx; extra == "cli"
 Provides-Extra: agent
-Requires-Dist: pandas==2.0.3; extra == "agent"
-Requires-Dist: cachetools; extra == "agent"
 Requires-Dist: fastapi>=0.100.0; extra == "agent"
+Requires-Dist: snowflake-id; extra == "agent"
+Requires-Dist: colorama==0.4.6; extra == "agent"
+Requires-Dist: pandas==2.0.3; extra == "agent"
+Requires-Dist: prettytable; extra == "agent"
 Requires-Dist: psutil==5.9.4; extra == "agent"
-Requires-Dist: tomlkit; extra == "agent"
+Requires-Dist: chardet==5.1.0; extra == "agent"
+Requires-Dist: typing_inspect; extra == "agent"
 Requires-Dist: termcolor; extra == "agent"
-Requires-Dist: httpx; extra == "agent"
 Requires-Dist: importlib-resources==5.12.0; extra == "agent"
-Requires-Dist: python-dotenv==1.0.0; extra == "agent"
-Requires-Dist: prettytable; extra == "agent"
-Requires-Dist: aiohttp==3.8.4; extra == "agent"
-Requires-Dist: snowflake-id; extra == "agent"
-Requires-Dist: colorama==0.4.6; extra == "agent"
-Requires-Dist: rich; extra == "agent"
 Requires-Dist: click; extra == "agent"
-Requires-Dist: chardet==5.1.0; extra == "agent"
+Requires-Dist: rich; extra == "agent"
+Requires-Dist: python-dotenv==1.0.0; extra == "agent"
 Requires-Dist: typeguard; extra == "agent"
 Requires-Dist: pydantic>=2.6.0; extra == "agent"
+Requires-Dist: aiohttp==3.8.4; extra == "agent"
+Requires-Dist: tomlkit; extra == "agent"
+Requires-Dist: cachetools; extra == "agent"
+Requires-Dist: httpx; extra == "agent"
 Provides-Extra: simple-framework
-Requires-Dist: schedule; extra == "simple-framework"
+Requires-Dist: fastapi>=0.100.0; extra == "simple-framework"
+Requires-Dist: snowflake-id; extra == "simple-framework"
+Requires-Dist: colorama==0.4.6; extra == "simple-framework"
+Requires-Dist: pandas==2.0.3; extra == "simple-framework"
+Requires-Dist: jinja2; extra == "simple-framework"
 Requires-Dist: sqlparse==0.4.4; extra == "simple-framework"
-Requires-Dist: msgpack; extra == "simple-framework"
+Requires-Dist: prettytable; extra == "simple-framework"
+Requires-Dist: psutil==5.9.4; extra == "simple-framework"
+Requires-Dist: chardet==5.1.0; extra == "simple-framework"
+Requires-Dist: typing_inspect; extra == "simple-framework"
+Requires-Dist: uvicorn; extra == "simple-framework"
 Requires-Dist: termcolor; extra == "simple-framework"
-Requires-Dist: rich; extra == "simple-framework"
+Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "simple-framework"
 Requires-Dist: shortuuid; extra == "simple-framework"
-Requires-Dist: typeguard; extra == "simple-framework"
-Requires-Dist: jinja2; extra == "simple-framework"
-Requires-Dist: cachetools; extra == "simple-framework"
-Requires-Dist: psutil==5.9.4; extra == "simple-framework"
 Requires-Dist: importlib-resources==5.12.0; extra == "simple-framework"
-Requires-Dist: prettytable; extra == "simple-framework"
-Requires-Dist: fschat; extra == "simple-framework"
-Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "simple-framework"
 Requires-Dist: click; extra == "simple-framework"
-Requires-Dist: duckdb-engine; extra == "simple-framework"
-Requires-Dist: pandas==2.0.3; extra == "simple-framework"
-Requires-Dist: fastapi>=0.100.0; extra == "simple-framework"
+Requires-Dist: schedule; extra == "simple-framework"
 Requires-Dist: pympler; extra == "simple-framework"
-Requires-Dist: tomlkit; extra == "simple-framework"
-Requires-Dist: uvicorn; extra == "simple-framework"
-Requires-Dist: httpx; extra == "simple-framework"
-Requires-Dist: python-dotenv==1.0.0; extra == "simple-framework"
-Requires-Dist: colorama==0.4.6; extra == "simple-framework"
-Requires-Dist: snowflake-id; extra == "simple-framework"
-Requires-Dist: chardet==5.1.0; extra == "simple-framework"
 Requires-Dist: duckdb; extra == "simple-framework"
-Requires-Dist: aiohttp==3.8.4; extra == "simple-framework"
+Requires-Dist: rich; extra == "simple-framework"
+Requires-Dist: python-dotenv==1.0.0; extra == "simple-framework"
+Requires-Dist: duckdb-engine; extra == "simple-framework"
+Requires-Dist: typeguard; extra == "simple-framework"
 Requires-Dist: pydantic>=2.6.0; extra == "simple-framework"
+Requires-Dist: aiohttp==3.8.4; extra == "simple-framework"
+Requires-Dist: fschat; extra == "simple-framework"
+Requires-Dist: tomlkit; extra == "simple-framework"
+Requires-Dist: msgpack; extra == "simple-framework"
+Requires-Dist: cachetools; extra == "simple-framework"
+Requires-Dist: httpx; extra == "simple-framework"
 Provides-Extra: framework
-Requires-Dist: schedule; extra == "framework"
-Requires-Dist: sqlparse==0.4.4; extra == "framework"
-Requires-Dist: seaborn; extra == "framework"
-Requires-Dist: msgpack; extra == "framework"
-Requires-Dist: termcolor; extra == "framework"
-Requires-Dist: alembic==1.12.0; extra == "framework"
-Requires-Dist: rich; extra == "framework"
-Requires-Dist: shortuuid; extra == "framework"
-Requires-Dist: typeguard; extra == "framework"
+Requires-Dist: fastapi>=0.100.0; extra == "framework"
+Requires-Dist: transformers>=4.34.0; extra == "framework"
+Requires-Dist: auto-gpt-plugin-template; extra == "framework"
+Requires-Dist: snowflake-id; extra == "framework"
+Requires-Dist: jsonschema; extra == "framework"
+Requires-Dist: colorama==0.4.6; extra == "framework"
+Requires-Dist: pandas==2.0.3; extra == "framework"
 Requires-Dist: jinja2; extra == "framework"
-Requires-Dist: pymysql; extra == "framework"
-Requires-Dist: cachetools; extra == "framework"
-Requires-Dist: psutil==5.9.4; extra == "framework"
-Requires-Dist: importlib-resources==5.12.0; extra == "framework"
+Requires-Dist: sqlparse==0.4.4; extra == "framework"
 Requires-Dist: prettytable; extra == "framework"
-Requires-Dist: fschat; extra == "framework"
+Requires-Dist: openpyxl==3.1.2; extra == "framework"
 Requires-Dist: graphviz; extra == "framework"
+Requires-Dist: psutil==5.9.4; extra == "framework"
+Requires-Dist: chardet==5.1.0; extra == "framework"
+Requires-Dist: typing_inspect; extra == "framework"
+Requires-Dist: uvicorn; extra == "framework"
+Requires-Dist: pymysql; extra == "framework"
+Requires-Dist: termcolor; extra == "framework"
 Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "framework"
+Requires-Dist: shortuuid; extra == "framework"
+Requires-Dist: gTTS==2.3.1; extra == "framework"
+Requires-Dist: importlib-resources==5.12.0; extra == "framework"
 Requires-Dist: click; extra == "framework"
-Requires-Dist: duckdb-engine; extra == "framework"
-Requires-Dist: pandas==2.0.3; extra == "framework"
-Requires-Dist: fastapi>=0.100.0; extra == "framework"
-Requires-Dist: jsonschema; extra == "framework"
-Requires-Dist: pympler; extra == "framework"
-Requires-Dist: tomlkit; extra == "framework"
-Requires-Dist: uvicorn; extra == "framework"
-Requires-Dist: auto-gpt-plugin-template; extra == "framework"
-Requires-Dist: httpx; extra == "framework"
-Requires-Dist: coloredlogs; extra == "framework"
-Requires-Dist: python-dotenv==1.0.0; extra == "framework"
-Requires-Dist: colorama==0.4.6; extra == "framework"
-Requires-Dist: snowflake-id; extra == "framework"
-Requires-Dist: transformers>=4.34.0; extra == "framework"
 Requires-Dist: aiofiles; extra == "framework"
-Requires-Dist: GitPython; extra == "framework"
-Requires-Dist: chardet==5.1.0; extra == "framework"
-Requires-Dist: gTTS==2.3.1; extra == "framework"
-Requires-Dist: duckdb; extra == "framework"
+Requires-Dist: schedule; extra == "framework"
+Requires-Dist: pympler; extra == "framework"
 Requires-Dist: xlrd==2.0.1; extra == "framework"
-Requires-Dist: aiohttp==3.8.4; extra == "framework"
-Requires-Dist: openpyxl==3.1.2; extra == "framework"
+Requires-Dist: duckdb; extra == "framework"
+Requires-Dist: GitPython; extra == "framework"
+Requires-Dist: alembic==1.12.0; extra == "framework"
+Requires-Dist: rich; extra == "framework"
+Requires-Dist: python-dotenv==1.0.0; extra == "framework"
+Requires-Dist: duckdb-engine; extra == "framework"
+Requires-Dist: coloredlogs; extra == "framework"
+Requires-Dist: typeguard; extra == "framework"
 Requires-Dist: pydantic>=2.6.0; extra == "framework"
+Requires-Dist: aiohttp==3.8.4; extra == "framework"
+Requires-Dist: fschat; extra == "framework"
+Requires-Dist: tomlkit; extra == "framework"
+Requires-Dist: seaborn; extra == "framework"
+Requires-Dist: msgpack; extra == "framework"
+Requires-Dist: cachetools; extra == "framework"
+Requires-Dist: httpx; extra == "framework"
 Provides-Extra: torch
-Requires-Dist: torchvision==0.17.1; extra == "torch"
-Requires-Dist: torch==2.2.1; extra == "torch"
 Requires-Dist: torchaudio==2.2.1; extra == "torch"
+Requires-Dist: torch==2.2.1; extra == "torch"
+Requires-Dist: torchvision==0.17.1; extra == "torch"
 Provides-Extra: torch-cpu
-Requires-Dist: torchvision==0.17.1; extra == "torch-cpu"
-Requires-Dist: torch==2.2.1; extra == "torch-cpu"
 Requires-Dist: torchaudio==2.2.1; extra == "torch-cpu"
+Requires-Dist: torch==2.2.1; extra == "torch-cpu"
+Requires-Dist: torchvision==0.17.1; extra == "torch-cpu"
 Provides-Extra: torch-cuda
-Requires-Dist: torchvision==0.17.1; extra == "torch-cuda"
-Requires-Dist: torch==2.2.1; extra == "torch-cuda"
 Requires-Dist: torchaudio==2.2.1; extra == "torch-cuda"
+Requires-Dist: torch==2.2.1; extra == "torch-cuda"
+Requires-Dist: torchvision==0.17.1; extra == "torch-cuda"
 Provides-Extra: llama-cpp
 Requires-Dist: llama-cpp-python; extra == "llama-cpp"
 Provides-Extra: bitsandbytes
 Requires-Dist: bitsandbytes; extra == "bitsandbytes"
 Provides-Extra: quantization
 Requires-Dist: cpm_kernels; extra == "quantization"
 Requires-Dist: bitsandbytes; extra == "quantization"
@@ -176,246 +183,247 @@
 Provides-Extra: vstore-all
 Requires-Dist: pymilvus; extra == "vstore-all"
 Requires-Dist: weaviate-client; extra == "vstore-all"
 Requires-Dist: chromadb>=0.4.22; extra == "vstore-all"
 Provides-Extra: datasource
 Requires-Dist: pymysql; extra == "datasource"
 Provides-Extra: datasource-all
-Requires-Dist: pymysql; extra == "datasource-all"
 Requires-Dist: thrift; extra == "datasource-all"
-Requires-Dist: pymssql; extra == "datasource-all"
-Requires-Dist: clickhouse-connect; extra == "datasource-all"
-Requires-Dist: thrift_sasl; extra == "datasource-all"
-Requires-Dist: pydoris<2.0.0,>=1.0.2; extra == "datasource-all"
 Requires-Dist: neo4j; extra == "datasource-all"
-Requires-Dist: pyhive; extra == "datasource-all"
-Requires-Dist: psycopg2; extra == "datasource-all"
 Requires-Dist: mysqlclient==2.1.0; extra == "datasource-all"
+Requires-Dist: pymysql; extra == "datasource-all"
+Requires-Dist: pymssql; extra == "datasource-all"
+Requires-Dist: psycopg2; extra == "datasource-all"
+Requires-Dist: pydoris<2.0.0,>=1.0.2; extra == "datasource-all"
+Requires-Dist: vertica_python; extra == "datasource-all"
 Requires-Dist: pyspark; extra == "datasource-all"
+Requires-Dist: pyhive; extra == "datasource-all"
+Requires-Dist: thrift_sasl; extra == "datasource-all"
+Requires-Dist: clickhouse-connect; extra == "datasource-all"
 Provides-Extra: rag
-Requires-Dist: bs4; extra == "rag"
-Requires-Dist: markdown; extra == "rag"
-Requires-Dist: spacy>=3.7; extra == "rag"
 Requires-Dist: sentence-transformers; extra == "rag"
-Requires-Dist: python-pptx; extra == "rag"
+Requires-Dist: python-multipart; extra == "rag"
 Requires-Dist: python-docx; extra == "rag"
+Requires-Dist: bs4; extra == "rag"
+Requires-Dist: python-pptx; extra == "rag"
 Requires-Dist: pypdf; extra == "rag"
+Requires-Dist: spacy>=3.7; extra == "rag"
 Requires-Dist: chromadb>=0.4.22; extra == "rag"
-Requires-Dist: langchain>=0.0.286; extra == "rag"
-Requires-Dist: python-multipart; extra == "rag"
+Requires-Dist: markdown; extra == "rag"
 Provides-Extra: openai
-Requires-Dist: schedule; extra == "openai"
-Requires-Dist: sqlparse==0.4.4; extra == "openai"
-Requires-Dist: seaborn; extra == "openai"
-Requires-Dist: markdown; extra == "openai"
-Requires-Dist: msgpack; extra == "openai"
-Requires-Dist: termcolor; extra == "openai"
+Requires-Dist: fastapi>=0.100.0; extra == "openai"
+Requires-Dist: transformers>=4.34.0; extra == "openai"
+Requires-Dist: python-multipart; extra == "openai"
 Requires-Dist: sentence-transformers; extra == "openai"
-Requires-Dist: tiktoken; extra == "openai"
-Requires-Dist: alembic==1.12.0; extra == "openai"
-Requires-Dist: rich; extra == "openai"
-Requires-Dist: shortuuid; extra == "openai"
 Requires-Dist: pypdf; extra == "openai"
+Requires-Dist: auto-gpt-plugin-template; extra == "openai"
+Requires-Dist: snowflake-id; extra == "openai"
+Requires-Dist: jsonschema; extra == "openai"
+Requires-Dist: colorama==0.4.6; extra == "openai"
 Requires-Dist: chromadb>=0.4.22; extra == "openai"
-Requires-Dist: typeguard; extra == "openai"
+Requires-Dist: pandas==2.0.3; extra == "openai"
 Requires-Dist: jinja2; extra == "openai"
-Requires-Dist: python-multipart; extra == "openai"
-Requires-Dist: pymysql; extra == "openai"
-Requires-Dist: cachetools; extra == "openai"
-Requires-Dist: psutil==5.9.4; extra == "openai"
-Requires-Dist: importlib-resources==5.12.0; extra == "openai"
+Requires-Dist: sqlparse==0.4.4; extra == "openai"
 Requires-Dist: prettytable; extra == "openai"
-Requires-Dist: fschat; extra == "openai"
+Requires-Dist: openpyxl==3.1.2; extra == "openai"
 Requires-Dist: graphviz; extra == "openai"
-Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "openai"
-Requires-Dist: click; extra == "openai"
-Requires-Dist: duckdb-engine; extra == "openai"
-Requires-Dist: pandas==2.0.3; extra == "openai"
-Requires-Dist: fastapi>=0.100.0; extra == "openai"
-Requires-Dist: jsonschema; extra == "openai"
-Requires-Dist: spacy>=3.7; extra == "openai"
-Requires-Dist: pympler; extra == "openai"
-Requires-Dist: tomlkit; extra == "openai"
-Requires-Dist: uvicorn; extra == "openai"
-Requires-Dist: auto-gpt-plugin-template; extra == "openai"
-Requires-Dist: httpx; extra == "openai"
-Requires-Dist: coloredlogs; extra == "openai"
-Requires-Dist: python-dotenv==1.0.0; extra == "openai"
-Requires-Dist: colorama==0.4.6; extra == "openai"
-Requires-Dist: snowflake-id; extra == "openai"
-Requires-Dist: transformers>=4.34.0; extra == "openai"
-Requires-Dist: aiofiles; extra == "openai"
+Requires-Dist: psutil==5.9.4; extra == "openai"
+Requires-Dist: openai; extra == "openai"
 Requires-Dist: python-docx; extra == "openai"
-Requires-Dist: GitPython; extra == "openai"
 Requires-Dist: chardet==5.1.0; extra == "openai"
-Requires-Dist: langchain>=0.0.286; extra == "openai"
-Requires-Dist: openai; extra == "openai"
-Requires-Dist: gTTS==2.3.1; extra == "openai"
 Requires-Dist: bs4; extra == "openai"
-Requires-Dist: duckdb; extra == "openai"
-Requires-Dist: python-pptx; extra == "openai"
+Requires-Dist: typing_inspect; extra == "openai"
+Requires-Dist: uvicorn; extra == "openai"
+Requires-Dist: pymysql; extra == "openai"
+Requires-Dist: termcolor; extra == "openai"
+Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "openai"
+Requires-Dist: shortuuid; extra == "openai"
+Requires-Dist: gTTS==2.3.1; extra == "openai"
+Requires-Dist: markdown; extra == "openai"
+Requires-Dist: importlib-resources==5.12.0; extra == "openai"
+Requires-Dist: click; extra == "openai"
+Requires-Dist: aiofiles; extra == "openai"
+Requires-Dist: schedule; extra == "openai"
+Requires-Dist: pympler; extra == "openai"
 Requires-Dist: xlrd==2.0.1; extra == "openai"
-Requires-Dist: aiohttp==3.8.4; extra == "openai"
-Requires-Dist: openpyxl==3.1.2; extra == "openai"
+Requires-Dist: duckdb; extra == "openai"
+Requires-Dist: GitPython; extra == "openai"
+Requires-Dist: alembic==1.12.0; extra == "openai"
+Requires-Dist: rich; extra == "openai"
+Requires-Dist: spacy>=3.7; extra == "openai"
+Requires-Dist: python-dotenv==1.0.0; extra == "openai"
+Requires-Dist: duckdb-engine; extra == "openai"
+Requires-Dist: coloredlogs; extra == "openai"
+Requires-Dist: typeguard; extra == "openai"
 Requires-Dist: pydantic>=2.6.0; extra == "openai"
+Requires-Dist: aiohttp==3.8.4; extra == "openai"
+Requires-Dist: fschat; extra == "openai"
+Requires-Dist: python-pptx; extra == "openai"
+Requires-Dist: tomlkit; extra == "openai"
+Requires-Dist: tiktoken; extra == "openai"
+Requires-Dist: seaborn; extra == "openai"
+Requires-Dist: msgpack; extra == "openai"
+Requires-Dist: cachetools; extra == "openai"
+Requires-Dist: httpx; extra == "openai"
 Provides-Extra: gpt4all
 Requires-Dist: gpt4all; extra == "gpt4all"
 Provides-Extra: vllm
 Requires-Dist: vllm; extra == "vllm"
 Provides-Extra: cache
 Requires-Dist: rocksdict; extra == "cache"
 Provides-Extra: default
-Requires-Dist: schedule; extra == "default"
-Requires-Dist: sqlparse==0.4.4; extra == "default"
-Requires-Dist: seaborn; extra == "default"
-Requires-Dist: markdown; extra == "default"
-Requires-Dist: msgpack; extra == "default"
-Requires-Dist: termcolor; extra == "default"
+Requires-Dist: cpm_kernels; extra == "default"
+Requires-Dist: fastapi>=0.100.0; extra == "default"
+Requires-Dist: transformers>=4.34.0; extra == "default"
+Requires-Dist: python-multipart; extra == "default"
 Requires-Dist: sentence-transformers; extra == "default"
-Requires-Dist: alembic==1.12.0; extra == "default"
-Requires-Dist: rich; extra == "default"
-Requires-Dist: ollama; extra == "default"
-Requires-Dist: shortuuid; extra == "default"
 Requires-Dist: pypdf; extra == "default"
+Requires-Dist: auto-gpt-plugin-template; extra == "default"
+Requires-Dist: snowflake-id; extra == "default"
+Requires-Dist: sentencepiece; extra == "default"
+Requires-Dist: colorama==0.4.6; extra == "default"
+Requires-Dist: jsonschema; extra == "default"
 Requires-Dist: chromadb>=0.4.22; extra == "default"
-Requires-Dist: cpm_kernels; extra == "default"
-Requires-Dist: typeguard; extra == "default"
+Requires-Dist: pandas==2.0.3; extra == "default"
 Requires-Dist: jinja2; extra == "default"
-Requires-Dist: python-multipart; extra == "default"
-Requires-Dist: torchvision==0.17.1; extra == "default"
-Requires-Dist: pymysql; extra == "default"
-Requires-Dist: cachetools; extra == "default"
+Requires-Dist: sqlparse==0.4.4; extra == "default"
+Requires-Dist: prettytable; extra == "default"
+Requires-Dist: openpyxl==3.1.2; extra == "default"
+Requires-Dist: graphviz; extra == "default"
 Requires-Dist: psutil==5.9.4; extra == "default"
-Requires-Dist: torch==2.2.1; extra == "default"
-Requires-Dist: torchaudio==2.2.1; extra == "default"
+Requires-Dist: python-docx; extra == "default"
+Requires-Dist: chardet==5.1.0; extra == "default"
+Requires-Dist: bs4; extra == "default"
+Requires-Dist: typing_inspect; extra == "default"
+Requires-Dist: uvicorn; extra == "default"
+Requires-Dist: pymysql; extra == "default"
+Requires-Dist: termcolor; extra == "default"
 Requires-Dist: dashscope; extra == "default"
+Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "default"
+Requires-Dist: ollama; extra == "default"
+Requires-Dist: shortuuid; extra == "default"
+Requires-Dist: gTTS==2.3.1; extra == "default"
 Requires-Dist: importlib-resources==5.12.0; extra == "default"
-Requires-Dist: prettytable; extra == "default"
-Requires-Dist: accelerate>=0.20.3; extra == "default"
-Requires-Dist: fschat; extra == "default"
+Requires-Dist: markdown; extra == "default"
 Requires-Dist: zhipuai; extra == "default"
-Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "default"
-Requires-Dist: graphviz; extra == "default"
-Requires-Dist: rocksdict; extra == "default"
 Requires-Dist: click; extra == "default"
-Requires-Dist: duckdb-engine; extra == "default"
-Requires-Dist: pandas==2.0.3; extra == "default"
-Requires-Dist: fastapi>=0.100.0; extra == "default"
-Requires-Dist: jsonschema; extra == "default"
-Requires-Dist: spacy>=3.7; extra == "default"
+Requires-Dist: rocksdict; extra == "default"
+Requires-Dist: aiofiles; extra == "default"
+Requires-Dist: schedule; extra == "default"
 Requires-Dist: pympler; extra == "default"
-Requires-Dist: tomlkit; extra == "default"
-Requires-Dist: uvicorn; extra == "default"
-Requires-Dist: auto-gpt-plugin-template; extra == "default"
-Requires-Dist: httpx; extra == "default"
+Requires-Dist: xlrd==2.0.1; extra == "default"
+Requires-Dist: accelerate>=0.20.3; extra == "default"
+Requires-Dist: duckdb; extra == "default"
+Requires-Dist: GitPython; extra == "default"
+Requires-Dist: alembic==1.12.0; extra == "default"
+Requires-Dist: rich; extra == "default"
+Requires-Dist: torchvision==0.17.1; extra == "default"
+Requires-Dist: spacy>=3.7; extra == "default"
+Requires-Dist: python-dotenv==1.0.0; extra == "default"
+Requires-Dist: duckdb-engine; extra == "default"
 Requires-Dist: coloredlogs; extra == "default"
+Requires-Dist: torch==2.2.1; extra == "default"
+Requires-Dist: torchaudio==2.2.1; extra == "default"
+Requires-Dist: typeguard; extra == "default"
+Requires-Dist: pydantic>=2.6.0; extra == "default"
+Requires-Dist: aiohttp==3.8.4; extra == "default"
+Requires-Dist: chardet; extra == "default"
+Requires-Dist: fschat; extra == "default"
 Requires-Dist: tokenizers>=0.14; extra == "default"
-Requires-Dist: python-dotenv==1.0.0; extra == "default"
-Requires-Dist: snowflake-id; extra == "default"
-Requires-Dist: colorama==0.4.6; extra == "default"
-Requires-Dist: transformers>=4.34.0; extra == "default"
-Requires-Dist: sentencepiece; extra == "default"
-Requires-Dist: aiofiles; extra == "default"
-Requires-Dist: python-docx; extra == "default"
-Requires-Dist: GitPython; extra == "default"
-Requires-Dist: chardet==5.1.0; extra == "default"
-Requires-Dist: langchain>=0.0.286; extra == "default"
-Requires-Dist: gTTS==2.3.1; extra == "default"
-Requires-Dist: bs4; extra == "default"
-Requires-Dist: duckdb; extra == "default"
 Requires-Dist: python-pptx; extra == "default"
-Requires-Dist: chardet; extra == "default"
-Requires-Dist: xlrd==2.0.1; extra == "default"
-Requires-Dist: aiohttp==3.8.4; extra == "default"
+Requires-Dist: tomlkit; extra == "default"
 Requires-Dist: bitsandbytes; extra == "default"
-Requires-Dist: openpyxl==3.1.2; extra == "default"
-Requires-Dist: pydantic>=2.6.0; extra == "default"
+Requires-Dist: seaborn; extra == "default"
+Requires-Dist: msgpack; extra == "default"
+Requires-Dist: cachetools; extra == "default"
+Requires-Dist: httpx; extra == "default"
 Provides-Extra: all
+Requires-Dist: cpm_kernels; extra == "all"
+Requires-Dist: transformers>=4.34.0; extra == "all"
+Requires-Dist: chromadb>=0.4.22; extra == "all"
+Requires-Dist: pandas==2.0.3; extra == "all"
 Requires-Dist: sqlparse==0.4.4; extra == "all"
-Requires-Dist: markdown; extra == "all"
-Requires-Dist: sentence-transformers; extra == "all"
-Requires-Dist: msgpack; extra == "all"
-Requires-Dist: alembic==1.12.0; extra == "all"
+Requires-Dist: clickhouse-connect; extra == "all"
+Requires-Dist: graphviz; extra == "all"
+Requires-Dist: python-docx; extra == "all"
+Requires-Dist: typing_inspect; extra == "all"
+Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "all"
+Requires-Dist: shortuuid; extra == "all"
+Requires-Dist: schedule; extra == "all"
+Requires-Dist: pympler; extra == "all"
 Requires-Dist: rich; extra == "all"
+Requires-Dist: python-dotenv==1.0.0; extra == "all"
+Requires-Dist: llama-cpp-python; extra == "all"
+Requires-Dist: fschat; extra == "all"
+Requires-Dist: tiktoken; extra == "all"
+Requires-Dist: seaborn; extra == "all"
+Requires-Dist: vertica_python; extra == "all"
+Requires-Dist: cachetools; extra == "all"
+Requires-Dist: GitPython; extra == "all"
+Requires-Dist: sentence-transformers; extra == "all"
+Requires-Dist: python-multipart; extra == "all"
 Requires-Dist: pypdf; extra == "all"
 Requires-Dist: psycopg2; extra == "all"
-Requires-Dist: python-multipart; extra == "all"
-Requires-Dist: importlib-resources==5.12.0; extra == "all"
-Requires-Dist: prettytable; extra == "all"
-Requires-Dist: thrift_sasl; extra == "all"
 Requires-Dist: auto-gpt-plugin-template; extra == "all"
-Requires-Dist: sentencepiece; extra == "all"
-Requires-Dist: GitPython; extra == "all"
-Requires-Dist: gTTS==2.3.1; extra == "all"
-Requires-Dist: clickhouse-connect; extra == "all"
-Requires-Dist: pydantic>=2.6.0; extra == "all"
-Requires-Dist: seaborn; extra == "all"
-Requires-Dist: psutil==5.9.4; extra == "all"
-Requires-Dist: gpt4all; extra == "all"
-Requires-Dist: zhipuai; extra == "all"
-Requires-Dist: click; extra == "all"
-Requires-Dist: pandas==2.0.3; extra == "all"
-Requires-Dist: jsonschema; extra == "all"
-Requires-Dist: vllm; extra == "all"
-Requires-Dist: httpx; extra == "all"
-Requires-Dist: colorama==0.4.6; extra == "all"
 Requires-Dist: snowflake-id; extra == "all"
-Requires-Dist: pyhive; extra == "all"
+Requires-Dist: jsonschema; extra == "all"
+Requires-Dist: jinja2; extra == "all"
+Requires-Dist: prettytable; extra == "all"
+Requires-Dist: thrift; extra == "all"
+Requires-Dist: openai; extra == "all"
 Requires-Dist: chardet==5.1.0; extra == "all"
-Requires-Dist: weaviate-client; extra == "all"
-Requires-Dist: pyspark; extra == "all"
-Requires-Dist: termcolor; extra == "all"
-Requires-Dist: pymilvus; extra == "all"
-Requires-Dist: shortuuid; extra == "all"
-Requires-Dist: cpm_kernels; extra == "all"
-Requires-Dist: neo4j; extra == "all"
-Requires-Dist: typeguard; extra == "all"
-Requires-Dist: torchaudio==2.2.1; extra == "all"
-Requires-Dist: accelerate>=0.20.3; extra == "all"
-Requires-Dist: rocksdict; extra == "all"
-Requires-Dist: spacy>=3.7; extra == "all"
-Requires-Dist: pympler; extra == "all"
-Requires-Dist: tomlkit; extra == "all"
 Requires-Dist: uvicorn; extra == "all"
-Requires-Dist: coloredlogs; extra == "all"
-Requires-Dist: tokenizers>=0.14; extra == "all"
-Requires-Dist: python-dotenv==1.0.0; extra == "all"
-Requires-Dist: duckdb; extra == "all"
+Requires-Dist: pyhive; extra == "all"
+Requires-Dist: dashscope; extra == "all"
+Requires-Dist: markdown; extra == "all"
+Requires-Dist: weaviate-client; extra == "all"
 Requires-Dist: xlrd==2.0.1; extra == "all"
+Requires-Dist: torchvision==0.17.1; extra == "all"
+Requires-Dist: duckdb-engine; extra == "all"
+Requires-Dist: torchaudio==2.2.1; extra == "all"
 Requires-Dist: aiohttp==3.8.4; extra == "all"
+Requires-Dist: chardet; extra == "all"
+Requires-Dist: tomlkit; extra == "all"
+Requires-Dist: bitsandbytes; extra == "all"
+Requires-Dist: sentencepiece; extra == "all"
 Requires-Dist: openpyxl==3.1.2; extra == "all"
-Requires-Dist: schedule; extra == "all"
-Requires-Dist: tiktoken; extra == "all"
+Requires-Dist: pymilvus; extra == "all"
+Requires-Dist: termcolor; extra == "all"
+Requires-Dist: pyspark; extra == "all"
 Requires-Dist: ollama; extra == "all"
-Requires-Dist: chromadb>=0.4.22; extra == "all"
-Requires-Dist: jinja2; extra == "all"
-Requires-Dist: torchvision==0.17.1; extra == "all"
-Requires-Dist: pymysql; extra == "all"
-Requires-Dist: cachetools; extra == "all"
-Requires-Dist: thrift; extra == "all"
-Requires-Dist: torch==2.2.1; extra == "all"
-Requires-Dist: dashscope; extra == "all"
-Requires-Dist: fschat; extra == "all"
-Requires-Dist: graphviz; extra == "all"
-Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "all"
-Requires-Dist: duckdb-engine; extra == "all"
+Requires-Dist: gTTS==2.3.1; extra == "all"
+Requires-Dist: importlib-resources==5.12.0; extra == "all"
+Requires-Dist: click; extra == "all"
+Requires-Dist: aiofiles; extra == "all"
+Requires-Dist: neo4j; extra == "all"
+Requires-Dist: mysqlclient==2.1.0; extra == "all"
+Requires-Dist: alembic==1.12.0; extra == "all"
+Requires-Dist: thrift_sasl; extra == "all"
+Requires-Dist: vllm; extra == "all"
+Requires-Dist: python-pptx; extra == "all"
+Requires-Dist: msgpack; extra == "all"
+Requires-Dist: httpx; extra == "all"
 Requires-Dist: fastapi>=0.100.0; extra == "all"
-Requires-Dist: python-docx; extra == "all"
 Requires-Dist: pymssql; extra == "all"
-Requires-Dist: llama-cpp-python; extra == "all"
-Requires-Dist: transformers>=4.34.0; extra == "all"
-Requires-Dist: aiofiles; extra == "all"
-Requires-Dist: pydoris<2.0.0,>=1.0.2; extra == "all"
-Requires-Dist: langchain>=0.0.286; extra == "all"
-Requires-Dist: openai; extra == "all"
+Requires-Dist: colorama==0.4.6; extra == "all"
+Requires-Dist: psutil==5.9.4; extra == "all"
 Requires-Dist: bs4; extra == "all"
-Requires-Dist: python-pptx; extra == "all"
-Requires-Dist: chardet; extra == "all"
-Requires-Dist: bitsandbytes; extra == "all"
-Requires-Dist: mysqlclient==2.1.0; extra == "all"
+Requires-Dist: pymysql; extra == "all"
+Requires-Dist: zhipuai; extra == "all"
+Requires-Dist: rocksdict; extra == "all"
+Requires-Dist: accelerate>=0.20.3; extra == "all"
+Requires-Dist: duckdb; extra == "all"
+Requires-Dist: gpt4all; extra == "all"
+Requires-Dist: pydoris<2.0.0,>=1.0.2; extra == "all"
+Requires-Dist: spacy>=3.7; extra == "all"
+Requires-Dist: torch==2.2.1; extra == "all"
+Requires-Dist: typeguard; extra == "all"
+Requires-Dist: pydantic>=2.6.0; extra == "all"
+Requires-Dist: tokenizers>=0.14; extra == "all"
+Requires-Dist: coloredlogs; extra == "all"
 
 # DB-GPT: Revolutionizing Database Interactions with Private LLM Technology
  
 <p align="left">
   <img src="./assets/LOGO.png" width="100%" />
 </p>
 
@@ -569,14 +577,18 @@
   We've also developed an automated fine-tuning lightweight framework centred on large language models (LLMs), Text2SQL datasets, LoRA/QLoRA/Pturning, and other fine-tuning methods. This framework simplifies Text-to-SQL fine-tuning, making it as straightforward as an assembly line process. [DB-GPT-Hub](https://github.com/eosphoros-ai/DB-GPT-Hub)
 
 - **SMMF(Service-oriented Multi-model Management Framework)**
 
   We offer extensive model support, including dozens of large language models (LLMs) from both open-source and API agents, such as LLaMA/LLaMA2, Baichuan, ChatGLM, Wenxin, Tongyi, Zhipu, and many more. 
 
   - News
+    - 🔥🔥🔥  [Phi-3](https://huggingface.co/collections/microsoft/phi-3-6626e15e9585a200d2d761e3)
+    - 🔥🔥🔥  [Yi-1.5-34B-Chat](https://huggingface.co/01-ai/Yi-1.5-34B-Chat)
+    - 🔥🔥🔥  [Yi-1.5-9B-Chat](https://huggingface.co/01-ai/Yi-1.5-9B-Chat)
+    - 🔥🔥🔥  [Yi-1.5-6B-Chat](https://huggingface.co/01-ai/Yi-1.5-6B-Chat)
     - 🔥🔥🔥  [Qwen1.5-110B-Chat](https://huggingface.co/Qwen/Qwen1.5-110B-Chat)
     - 🔥🔥🔥  [Qwen1.5-MoE-A2.7B-Chat](https://huggingface.co/Qwen/Qwen1.5-MoE-A2.7B-Chat)
     - 🔥🔥🔥  [Meta-Llama-3-70B-Instruct](https://huggingface.co/meta-llama/Meta-Llama-3-70B-Instruct)
     - 🔥🔥🔥  [Meta-Llama-3-8B-Instruct](https://huggingface.co/meta-llama/Meta-Llama-3-8B-Instruct)
     - 🔥🔥🔥  [CodeQwen1.5-7B-Chat](https://huggingface.co/Qwen/CodeQwen1.5-7B-Chat)
     - 🔥🔥🔥  [Qwen1.5-32B-Chat](https://huggingface.co/Qwen/Qwen1.5-32B-Chat)
     - 🔥🔥🔥  [Starling-LM-7B-beta](https://huggingface.co/Nexusflow/Starling-LM-7B-beta)
```

### Comparing `dbgpt-0.5.6rc0/README.md` & `dbgpt-0.5.7rc0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -154,14 +154,18 @@
   We've also developed an automated fine-tuning lightweight framework centred on large language models (LLMs), Text2SQL datasets, LoRA/QLoRA/Pturning, and other fine-tuning methods. This framework simplifies Text-to-SQL fine-tuning, making it as straightforward as an assembly line process. [DB-GPT-Hub](https://github.com/eosphoros-ai/DB-GPT-Hub)
 
 - **SMMF(Service-oriented Multi-model Management Framework)**
 
   We offer extensive model support, including dozens of large language models (LLMs) from both open-source and API agents, such as LLaMA/LLaMA2, Baichuan, ChatGLM, Wenxin, Tongyi, Zhipu, and many more. 
 
   - News
+    - 🔥🔥🔥  [Phi-3](https://huggingface.co/collections/microsoft/phi-3-6626e15e9585a200d2d761e3)
+    - 🔥🔥🔥  [Yi-1.5-34B-Chat](https://huggingface.co/01-ai/Yi-1.5-34B-Chat)
+    - 🔥🔥🔥  [Yi-1.5-9B-Chat](https://huggingface.co/01-ai/Yi-1.5-9B-Chat)
+    - 🔥🔥🔥  [Yi-1.5-6B-Chat](https://huggingface.co/01-ai/Yi-1.5-6B-Chat)
     - 🔥🔥🔥  [Qwen1.5-110B-Chat](https://huggingface.co/Qwen/Qwen1.5-110B-Chat)
     - 🔥🔥🔥  [Qwen1.5-MoE-A2.7B-Chat](https://huggingface.co/Qwen/Qwen1.5-MoE-A2.7B-Chat)
     - 🔥🔥🔥  [Meta-Llama-3-70B-Instruct](https://huggingface.co/meta-llama/Meta-Llama-3-70B-Instruct)
     - 🔥🔥🔥  [Meta-Llama-3-8B-Instruct](https://huggingface.co/meta-llama/Meta-Llama-3-8B-Instruct)
     - 🔥🔥🔥  [CodeQwen1.5-7B-Chat](https://huggingface.co/Qwen/CodeQwen1.5-7B-Chat)
     - 🔥🔥🔥  [Qwen1.5-32B-Chat](https://huggingface.co/Qwen/Qwen1.5-32B-Chat)
     - 🔥🔥🔥  [Starling-LM-7B-beta](https://huggingface.co/Nexusflow/Starling-LM-7B-beta)
```

#### html2text {}

```diff
@@ -99,46 +99,51 @@
 tuning lightweight framework centred on large language models (LLMs), Text2SQL
 datasets, LoRA/QLoRA/Pturning, and other fine-tuning methods. This framework
 simplifies Text-to-SQL fine-tuning, making it as straightforward as an assembly
 line process. [DB-GPT-Hub](https://github.com/eosphoros-ai/DB-GPT-Hub) - **SMMF
 (Service-oriented Multi-model Management Framework)** We offer extensive model
 support, including dozens of large language models (LLMs) from both open-source
 and API agents, such as LLaMA/LLaMA2, Baichuan, ChatGLM, Wenxin, Tongyi, Zhipu,
-and many more. - News - ð¥ð¥ð¥ [Qwen1.5-110B-Chat](https://
-huggingface.co/Qwen/Qwen1.5-110B-Chat) - ð¥ð¥ð¥ [Qwen1.5-MoE-A2.7B-Chat]
-(https://huggingface.co/Qwen/Qwen1.5-MoE-A2.7B-Chat) - ð¥ð¥ð¥ [Meta-
-Llama-3-70B-Instruct](https://huggingface.co/meta-llama/Meta-Llama-3-70B-
-Instruct) - ð¥ð¥ð¥ [Meta-Llama-3-8B-Instruct](https://huggingface.co/
-meta-llama/Meta-Llama-3-8B-Instruct) - ð¥ð¥ð¥ [CodeQwen1.5-7B-Chat]
-(https://huggingface.co/Qwen/CodeQwen1.5-7B-Chat) - ð¥ð¥ð¥ [Qwen1.5-32B-
-Chat](https://huggingface.co/Qwen/Qwen1.5-32B-Chat) - ð¥ð¥ð¥ [Starling-
-LM-7B-beta](https://huggingface.co/Nexusflow/Starling-LM-7B-beta) -
-ð¥ð¥ð¥ [gemma-7b-it](https://huggingface.co/google/gemma-7b-it) -
-ð¥ð¥ð¥ [gemma-2b-it](https://huggingface.co/google/gemma-2b-it) -
-ð¥ð¥ð¥ [SOLAR-10.7B](https://huggingface.co/upstage/SOLAR-10.7B-Instruct-
-v1.0) - ð¥ð¥ð¥ [Mixtral-8x7B](https://huggingface.co/mistralai/Mixtral-
-8x7B-Instruct-v0.1) - ð¥ð¥ð¥ [Qwen-72B-Chat](https://huggingface.co/Qwen/
-Qwen-72B-Chat) - ð¥ð¥ð¥ [Yi-34B-Chat](https://huggingface.co/01-ai/Yi-
-34B-Chat) - [More Supported LLMs](http://docs.dbgpt.site/docs/modules/smmf) -
-**Privacy and Security** We ensure the privacy and security of data through the
-implementation of various technologies, including privatized large models and
-proxy desensitization. - Support Datasources - [Datasources](http://
-docs.dbgpt.site/docs/modules/connections) ## Image ð [AutoDL Image](https://
-www.codewithgpu.com/i/eosphoros-ai/DB-GPT/dbgpt) ### Language Switching In the
-.env configuration file, modify the LANGUAGE parameter to switch to different
-languages. The default is English (Chinese: zh, English: en, other languages to
-be added later). ## Contribution - To check detailed guidelines for new
-contributions, please refer [how to contribute](https://github.com/eosphoros-
-ai/DB-GPT/blob/main/CONTRIBUTING.md) ### Contributors Wall _[_h_t_t_p_s_:_/_/
-_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_e_o_s_p_h_o_r_o_s_-_a_i_/_D_B_-_G_P_T_&_m_a_x_=_2_0_0_]## Licence The MIT License
-(MIT) ## Citation If you find `DB-GPT` useful for your research or development,
-please cite the following _p_a_p_e_r: ```bibtex @article{xue2023dbgpt, title={DB-
-GPT: Empowering Database Interactions with Private Large Language Models},
-author={Siqiao Xue and Caigao Jiang and Wenhui Shi and Fangyin Cheng and Keting
-Chen and Hongjun Yang and Zhiping Zhang and Jianshan He and Hongyang Zhang and
+and many more. - News - ð¥ð¥ð¥ [Phi-3](https://huggingface.co/
+collections/microsoft/phi-3-6626e15e9585a200d2d761e3) - ð¥ð¥ð¥ [Yi-1.5-
+34B-Chat](https://huggingface.co/01-ai/Yi-1.5-34B-Chat) - ð¥ð¥ð¥ [Yi-1.5-
+9B-Chat](https://huggingface.co/01-ai/Yi-1.5-9B-Chat) - ð¥ð¥ð¥ [Yi-1.5-
+6B-Chat](https://huggingface.co/01-ai/Yi-1.5-6B-Chat) - ð¥ð¥ð¥ [Qwen1.5-
+110B-Chat](https://huggingface.co/Qwen/Qwen1.5-110B-Chat) - ð¥ð¥ð¥
+[Qwen1.5-MoE-A2.7B-Chat](https://huggingface.co/Qwen/Qwen1.5-MoE-A2.7B-Chat) -
+ð¥ð¥ð¥ [Meta-Llama-3-70B-Instruct](https://huggingface.co/meta-llama/
+Meta-Llama-3-70B-Instruct) - ð¥ð¥ð¥ [Meta-Llama-3-8B-Instruct](https://
+huggingface.co/meta-llama/Meta-Llama-3-8B-Instruct) - ð¥ð¥ð¥
+[CodeQwen1.5-7B-Chat](https://huggingface.co/Qwen/CodeQwen1.5-7B-Chat) -
+ð¥ð¥ð¥ [Qwen1.5-32B-Chat](https://huggingface.co/Qwen/Qwen1.5-32B-Chat) -
+ð¥ð¥ð¥ [Starling-LM-7B-beta](https://huggingface.co/Nexusflow/Starling-
+LM-7B-beta) - ð¥ð¥ð¥ [gemma-7b-it](https://huggingface.co/google/gemma-
+7b-it) - ð¥ð¥ð¥ [gemma-2b-it](https://huggingface.co/google/gemma-2b-it)
+- ð¥ð¥ð¥ [SOLAR-10.7B](https://huggingface.co/upstage/SOLAR-10.7B-
+Instruct-v1.0) - ð¥ð¥ð¥ [Mixtral-8x7B](https://huggingface.co/mistralai/
+Mixtral-8x7B-Instruct-v0.1) - ð¥ð¥ð¥ [Qwen-72B-Chat](https://
+huggingface.co/Qwen/Qwen-72B-Chat) - ð¥ð¥ð¥ [Yi-34B-Chat](https://
+huggingface.co/01-ai/Yi-34B-Chat) - [More Supported LLMs](http://
+docs.dbgpt.site/docs/modules/smmf) - **Privacy and Security** We ensure the
+privacy and security of data through the implementation of various
+technologies, including privatized large models and proxy desensitization. -
+Support Datasources - [Datasources](http://docs.dbgpt.site/docs/modules/
+connections) ## Image ð [AutoDL Image](https://www.codewithgpu.com/i/
+eosphoros-ai/DB-GPT/dbgpt) ### Language Switching In the .env configuration
+file, modify the LANGUAGE parameter to switch to different languages. The
+default is English (Chinese: zh, English: en, other languages to be added
+later). ## Contribution - To check detailed guidelines for new contributions,
+please refer [how to contribute](https://github.com/eosphoros-ai/DB-GPT/blob/
+main/CONTRIBUTING.md) ### Contributors Wall _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/
+_i_m_a_g_e_?_r_e_p_o_=_e_o_s_p_h_o_r_o_s_-_a_i_/_D_B_-_G_P_T_&_m_a_x_=_2_0_0_]## Licence The MIT License (MIT) ##
+Citation If you find `DB-GPT` useful for your research or development, please
+cite the following _p_a_p_e_r: ```bibtex @article{xue2023dbgpt, title={DB-GPT:
+Empowering Database Interactions with Private Large Language Models}, author=
+{Siqiao Xue and Caigao Jiang and Wenhui Shi and Fangyin Cheng and Keting Chen
+and Hongjun Yang and Zhiping Zhang and Jianshan He and Hongyang Zhang and
 Ganglin Wei and Wang Zhao and Fan Zhou and Danrui Qi and Hong Yi and Shaodong
 Liu and Faqiang Chen}, year={2023}, journal={arXiv preprint arXiv:2312.17449},
 url={https://arxiv.org/abs/2312.17449} } ``` ## Contact Information We are
 working on building a community, if you have any ideas for building the
 community, feel free to contact us. [![](https://dcbadge.vercel.app/api/server/
 7uQnPuveTY?compact=true&style=flat)](https://discord.gg/7uQnPuveTY) [![Star
 History Chart](https://api.star-history.com/svg?repos=csunny/DB-GPT&type=Date)]
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/__init__.py` & `dbgpt-0.5.7rc0/dbgpt/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/_private/config.py` & `dbgpt-0.5.7rc0/dbgpt/_private/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import os
-from typing import TYPE_CHECKING, List, Optional
+from typing import TYPE_CHECKING, Optional
 
 from dbgpt.util.singleton import Singleton
 
 if TYPE_CHECKING:
-    from auto_gpt_plugin_template import AutoGPTPluginTemplate
-
-    from dbgpt.agent.plugin import CommandRegistry
     from dbgpt.component import SystemApp
     from dbgpt.datasource.manages import ConnectorManager
 
 
 class Config(metaclass=Singleton):
     """Configuration class to store the state of bools for different scripts access"""
 
@@ -124,14 +121,24 @@
             os.environ["moonshot_proxyllm_proxy_api_key"] = self.moonshot_proxy_api_key
             os.environ["moonshot_proxyllm_proxyllm_backend"] = os.getenv(
                 "MOONSHOT_MODEL_VERSION", "moonshot-v1-8k"
             )
             os.environ["moonshot_proxyllm_api_base"] = os.getenv(
                 "MOONSHOT_API_BASE", "https://api.moonshot.cn/v1"
             )
+        # Deepseek proxy
+        self.deepseek_proxy_api_key = os.getenv("DEEPSEEK_API_KEY")
+        if self.deepseek_proxy_api_key:
+            os.environ["deepseek_proxyllm_proxy_api_key"] = self.deepseek_proxy_api_key
+            os.environ["deepseek_proxyllm_proxyllm_backend"] = os.getenv(
+                "DEEPSEEK_MODEL_VERSION", "deepseek-chat"
+            )
+            os.environ["deepseek_proxyllm_api_base"] = os.getenv(
+                "DEEPSEEK_API_BASE", "https://api.deepseek.com/v1"
+            )
 
         self.proxy_server_url = os.getenv("PROXY_SERVER_URL")
 
         self.elevenlabs_api_key = os.getenv("ELEVENLABS_API_KEY")
         self.elevenlabs_voice_1_id = os.getenv("ELEVENLABS_VOICE_1_ID")
         self.elevenlabs_voice_2_id = os.getenv("ELEVENLABS_VOICE_2_ID")
 
@@ -151,57 +158,30 @@
             "HUGGINGFACE_AUDIO_TO_TEXT_MODEL"
         )
         self.speak_mode = False
 
         from dbgpt.core._private.prompt_registry import PromptTemplateRegistry
 
         self.prompt_template_registry = PromptTemplateRegistry()
-        ### Related configuration of built-in commands
-        self.command_registry: Optional[CommandRegistry] = None
-
-        disabled_command_categories = os.getenv("DISABLED_COMMAND_CATEGORIES")
-        if disabled_command_categories:
-            self.disabled_command_categories = disabled_command_categories.split(",")
-        else:
-            self.disabled_command_categories = []
 
         self.execute_local_commands = (
             os.getenv("EXECUTE_LOCAL_COMMANDS", "False").lower() == "true"
         )
         ### message stor file
         self.message_dir = os.getenv("MESSAGE_HISTORY_DIR", "../../message")
 
-        ### The associated configuration parameters of the plug-in control the loading and use of the plug-in
-
-        self.plugins: List["AutoGPTPluginTemplate"] = []
-        self.plugins_openai = []  # type: ignore
-        self.plugins_auto_load = os.getenv("AUTO_LOAD_PLUGIN", "True").lower() == "true"
-
-        self.plugins_git_branch = os.getenv("PLUGINS_GIT_BRANCH", "plugin_dashboard")
-
-        plugins_allowlist = os.getenv("ALLOWLISTED_PLUGINS")
-        if plugins_allowlist:
-            self.plugins_allowlist = plugins_allowlist.split(",")
-        else:
-            self.plugins_allowlist = []
-
-        plugins_denylist = os.getenv("DENYLISTED_PLUGINS")
-        if plugins_denylist:
-            self.plugins_denylist = plugins_denylist.split(",")
-        else:
-            self.plugins_denylist = []
         ### Native SQL Execution Capability Control Configuration
         self.NATIVE_SQL_CAN_RUN_DDL = (
             os.getenv("NATIVE_SQL_CAN_RUN_DDL", "True").lower() == "true"
         )
         self.NATIVE_SQL_CAN_RUN_WRITE = (
             os.getenv("NATIVE_SQL_CAN_RUN_WRITE", "True").lower() == "true"
         )
 
-        ###dbgpt meta info database connection configuration
+        ### dbgpt meta info database connection configuration
         self.LOCAL_DB_HOST = os.getenv("LOCAL_DB_HOST")
         self.LOCAL_DB_PATH = os.getenv("LOCAL_DB_PATH", "data/default_sqlite.db")
         self.LOCAL_DB_TYPE = os.getenv("LOCAL_DB_TYPE", "sqlite")
         if self.LOCAL_DB_HOST is None and self.LOCAL_DB_PATH == "":
             self.LOCAL_DB_HOST = "127.0.0.1"
 
         self.LOCAL_DB_NAME = os.getenv("LOCAL_DB_NAME", "dbgpt")
@@ -233,14 +213,19 @@
 
         ### Vector Store Configuration
         self.VECTOR_STORE_TYPE = os.getenv("VECTOR_STORE_TYPE", "Chroma")
         self.MILVUS_URL = os.getenv("MILVUS_URL", "127.0.0.1")
         self.MILVUS_PORT = os.getenv("MILVUS_PORT", "19530")
         self.MILVUS_USERNAME = os.getenv("MILVUS_USERNAME", None)
         self.MILVUS_PASSWORD = os.getenv("MILVUS_PASSWORD", None)
+        # Elasticsearch Vector Configuration
+        self.ELASTICSEARCH_URL = os.getenv("ELASTICSEARCH_URL", "127.0.0.1")
+        self.ELASTICSEARCH_PORT = os.getenv("ELASTICSEARCH_PORT", "9200")
+        self.ELASTICSEARCH_USERNAME = os.getenv("ELASTICSEARCH_USERNAME", None)
+        self.ELASTICSEARCH_PASSWORD = os.getenv("ELASTICSEARCH_PASSWORD", None)
 
         ## OceanBase Configuration
         self.OB_HOST = os.getenv("OB_HOST", "127.0.0.1")
         self.OB_PORT = int(os.getenv("OB_PORT", "2881"))
         self.OB_USER = os.getenv("OB_USER", "root")
         self.OB_PASSWORD = os.getenv("OB_PASSWORD", "")
         self.OB_DATABASE = os.getenv("OB_DATABASE", "test")
@@ -258,17 +243,24 @@
             self.IS_LOAD_8BIT = False
         # In order to be compatible with the new and old model parameter design
         os.environ["load_8bit"] = str(self.IS_LOAD_8BIT)
         os.environ["load_4bit"] = str(self.IS_LOAD_4BIT)
 
         ### EMBEDDING Configuration
         self.EMBEDDING_MODEL = os.getenv("EMBEDDING_MODEL", "text2vec")
+        # Rerank model configuration
+        self.RERANK_MODEL = os.getenv("RERANK_MODEL")
+        self.RERANK_MODEL_PATH = os.getenv("RERANK_MODEL_PATH")
+        self.RERANK_TOP_K = int(os.getenv("RERANK_TOP_K", 3))
         self.KNOWLEDGE_CHUNK_SIZE = int(os.getenv("KNOWLEDGE_CHUNK_SIZE", 100))
         self.KNOWLEDGE_CHUNK_OVERLAP = int(os.getenv("KNOWLEDGE_CHUNK_OVERLAP", 50))
         self.KNOWLEDGE_SEARCH_TOP_SIZE = int(os.getenv("KNOWLEDGE_SEARCH_TOP_SIZE", 5))
+        self.KNOWLEDGE_GRAPH_SEARCH_TOP_SIZE = int(
+            os.getenv("KNOWLEDGE_GRAPH_SEARCH_TOP_SIZE", 50)
+        )
         self.KNOWLEDGE_MAX_CHUNKS_ONCE_LOAD = int(
             os.getenv("KNOWLEDGE_MAX_CHUNKS_ONCE_LOAD", 10)
         )
         # default recall similarity score, between 0 and 1
         self.KNOWLEDGE_SEARCH_RECALL_SCORE = float(
             os.getenv("KNOWLEDGE_SEARCH_RECALL_SCORE", 0.3)
         )
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/_private/llm_metadata.py` & `dbgpt-0.5.7rc0/dbgpt/_private/llm_metadata.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/_private/pydantic.py` & `dbgpt-0.5.7rc0/dbgpt/_private/pydantic.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
         Field,
         NonNegativeFloat,
         NonNegativeInt,
         PositiveFloat,
         PositiveInt,
         PrivateAttr,
         ValidationError,
+        WithJsonSchema,
         field_validator,
         model_validator,
         root_validator,
         validator,
     )
 
     EXTRA_FORBID = "forbid"
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/__init__.py` & `dbgpt-0.5.7rc0/dbgpt/agent/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 from .core.base_agent import ConversableAgent  # noqa: F401
 from .core.memory import *  # noqa: F401, F403
 from .core.memory.gpts.gpts_memory import GptsMemory  # noqa: F401
 from .core.plan import *  # noqa: F401, F403
 from .core.profile import *  # noqa: F401, F403
 from .core.schema import PluginStorageType  # noqa: F401
 from .core.user_proxy_agent import UserProxyAgent  # noqa: F401
-from .resource.resource_api import AgentResource, ResourceType  # noqa: F401
-from .resource.resource_loader import ResourceLoader  # noqa: F401
+from .resource.base import AgentResource, Resource, ResourceType  # noqa: F401
 from .util.llm.llm import LLMConfig  # noqa: F401
 
 __ALL__ = [
     "Agent",
     "AgentContext",
     "AgentGenerateContext",
     "AgentMessage",
@@ -34,11 +33,10 @@
     "ConversableAgent",
     "Action",
     "ActionOutput",
     "LLMConfig",
     "GptsMemory",
     "AgentResource",
     "ResourceType",
-    "ResourceLoader",
     "PluginStorageType",
     "UserProxyAgent",
 ]
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/core/__init__.py` & `dbgpt-0.5.7rc0/dbgpt/agent/core/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/core/action/__init__.py` & `dbgpt-0.5.7rc0/dbgpt/agent/core/action/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/core/action/base.py` & `dbgpt-0.5.7rc0/dbgpt/agent/core/action/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,16 +23,15 @@
     model_fields,
     model_to_dict,
     model_validator,
 )
 from dbgpt.util.json_utils import find_json_objects
 from dbgpt.vis.base import Vis
 
-from ...resource.resource_api import AgentResource, ResourceType
-from ...resource.resource_loader import ResourceLoader
+from ...resource.base import AgentResource, Resource, ResourceType
 
 T = TypeVar("T", bound=Union[BaseModel, List[BaseModel], None])
 
 JsonMessageType = Union[Dict[str, Any], List[Dict[str, Any]]]
 
 
 class ActionOutput(BaseModel):
@@ -73,19 +72,19 @@
 
 
 class Action(ABC, Generic[T]):
     """Base Action class for defining agent actions."""
 
     def __init__(self):
         """Create an action."""
-        self.resource_loader: Optional[ResourceLoader] = None
+        self.resource: Optional[Resource] = None
 
-    def init_resource_loader(self, resource_loader: Optional[ResourceLoader]):
-        """Initialize the resource loader."""
-        self.resource_loader = resource_loader
+    def init_resource(self, resource: Optional[Resource]):
+        """Initialize the resource."""
+        self.resource = resource
 
     @property
     def resource_need(self) -> Optional[ResourceType]:
         """Return the resource type needed for the action."""
         return None
 
     @property
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/core/action/blank_action.py` & `dbgpt-0.5.7rc0/dbgpt/agent/core/action/blank_action.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Blank Action for the Agent."""
 
 import logging
 from typing import Optional
 
-from ...resource.resource_api import AgentResource
+from ...resource.base import AgentResource
 from .base import Action, ActionOutput
 
 logger = logging.getLogger(__name__)
 
 
 class BlankAction(Action):
     """Blank action class."""
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/core/agent.py` & `dbgpt-0.5.7rc0/dbgpt/agent/core/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import dataclasses
 from abc import ABC, abstractmethod
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from dbgpt.core import LLMClient
 from dbgpt.util.annotations import PublicAPI
 
-from ..resource.resource_loader import ResourceLoader
 from .action.base import ActionOutput
 from .memory.agent_memory import AgentMemory
 
 
 class Agent(ABC):
     """Agent Interface."""
 
@@ -205,15 +204,14 @@
     silent: Optional[bool] = False
 
     rely_messages: List[AgentMessage] = dataclasses.field(default_factory=list)
     final: Optional[bool] = True
 
     memory: Optional[AgentMemory] = None
     agent_context: Optional[AgentContext] = None
-    resource_loader: Optional[ResourceLoader] = None
     llm_client: Optional[LLMClient] = None
 
     round_index: Optional[int] = None
 
     def to_dict(self) -> Dict:
         """Return a dictionary representation of the AgentGenerateContext."""
         return dataclasses.asdict(self)
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/core/agent_manage.py` & `dbgpt-0.5.7rc0/dbgpt/agent/core/agent_manage.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,23 +64,23 @@
         self.system_app = system_app
 
     def after_start(self):
         """Register all agents."""
         from ..expand.code_assistant_agent import CodeAssistantAgent
         from ..expand.dashboard_assistant_agent import DashboardAssistantAgent
         from ..expand.data_scientist_agent import DataScientistAgent
-        from ..expand.plugin_assistant_agent import PluginAssistantAgent
         from ..expand.summary_assistant_agent import SummaryAssistantAgent
+        from ..expand.tool_assistant_agent import ToolAssistantAgent
 
         core_agents = set()
         core_agents.add(self.register_agent(CodeAssistantAgent))
         core_agents.add(self.register_agent(DashboardAssistantAgent))
         core_agents.add(self.register_agent(DataScientistAgent))
         core_agents.add(self.register_agent(SummaryAssistantAgent))
-        core_agents.add(self.register_agent(PluginAssistantAgent))
+        core_agents.add(self.register_agent(ToolAssistantAgent))
         self._core_agents = core_agents
 
     def register_agent(
         self, cls: Type[ConversableAgent], ignore_duplicate: bool = False
     ) -> str:
         """Register an agent."""
         inst = cls()
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/core/base_agent.py` & `dbgpt-0.5.7rc0/dbgpt/agent/core/base_agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Base agent class for conversable agents."""
 
 import asyncio
 import json
 import logging
-from typing import Any, Dict, List, Optional, Tuple, Type, cast
+from concurrent.futures import Executor, ThreadPoolExecutor
+from typing import Any, Callable, Dict, List, Optional, Tuple, Type, cast
 
 from dbgpt._private.pydantic import ConfigDict, Field
 from dbgpt.core import LLMClient, ModelMessageRoleType
 from dbgpt.util.error_types import LLMChatError
+from dbgpt.util.executor_utils import blocking_func_to_async
 from dbgpt.util.tracer import SpanType, root_tracer
 from dbgpt.util.utils import colored
 
-from ..resource.resource_api import AgentResource, ResourceClient
-from ..resource.resource_loader import ResourceLoader
+from ..resource.base import Resource
 from ..util.llm.llm import LLMConfig, LLMStrategyType
 from ..util.llm.llm_client import AIWrapper
 from .action.base import Action, ActionOutput
 from .agent import Agent, AgentContext, AgentMessage, AgentReviewInfo
 from .memory.agent_memory import AgentMemory
 from .memory.gpts.base import GptsMessage
 from .memory.gpts.gpts_memory import GptsMemory
@@ -28,20 +29,23 @@
 class ConversableAgent(Role, Agent):
     """ConversableAgent is an agent that can communicate with other agents."""
 
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
     agent_context: Optional[AgentContext] = Field(None, description="Agent context")
     actions: List[Action] = Field(default_factory=list)
-    resources: List[AgentResource] = Field(default_factory=list)
+    resource: Optional[Resource] = Field(None, description="Resource")
     llm_config: Optional[LLMConfig] = None
-    resource_loader: Optional[ResourceLoader] = None
     max_retry_count: int = 3
     consecutive_auto_reply_counter: int = 0
     llm_client: Optional[AIWrapper] = None
+    executor: Executor = Field(
+        default_factory=lambda: ThreadPoolExecutor(max_workers=1),
+        description="Executor for running tasks",
+    )
 
     def __init__(self, **kwargs):
         """Create a new agent."""
         Role.__init__(self, **kwargs)
         Agent.__init__(self)
 
     def check_available(self) -> None:
@@ -54,35 +58,20 @@
         # check run context
         if self.agent_context is None:
             raise ValueError(
                 f"{self.name}[{self.role}] Missing context in which agent is "
                 f"running!"
             )
 
-        # resource check
-        for resource in self.resources:
-            if (
-                self.resource_loader is None
-                or self.resource_loader.get_resource_api(
-                    resource.type, check_instance=False
-                )
-                is None
-            ):
-                raise ValueError(
-                    f"Resource {resource.type}:{resource.value} missing resource loader"
-                    f" implementation,unable to read resources!"
-                )
-
         # action check
         if self.actions and len(self.actions) > 0:
-            have_resource_types = [item.type for item in self.resources]
             for action in self.actions:
-                if (
-                    action.resource_need
-                    and action.resource_need not in have_resource_types
+                if action.resource_need and (
+                    not self.resource
+                    or not self.resource.get_resource_by_type(action.resource_need)
                 ):
                     raise ValueError(
                         f"{self.name}[{self.role}] Missing resources required for "
                         "runtime！"
                     )
         else:
             if not self.is_human and not self.is_team:
@@ -109,52 +98,54 @@
             ValueError: If the agent context is not initialized.
         """
         if not self.agent_context:
             raise ValueError("Agent context is not initialized！")
         return self.agent_context
 
     @property
-    def not_null_resource_loader(self) -> ResourceLoader:
-        """Get the resource loader."""
-        if not self.resource_loader:
-            raise ValueError("Resource loader is not initialized！")
-        return self.resource_loader
-
-    @property
     def not_null_llm_config(self) -> LLMConfig:
         """Get the LLM config."""
         if not self.llm_config:
             raise ValueError("LLM config is not initialized！")
         return self.llm_config
 
     @property
     def not_null_llm_client(self) -> LLMClient:
         """Get the LLM client."""
         llm_client = self.not_null_llm_config.llm_client
         if not llm_client:
             raise ValueError("LLM client is not initialized！")
         return llm_client
 
+    async def blocking_func_to_async(
+        self, func: Callable[..., Any], *args, **kwargs
+    ) -> Any:
+        """Run a potentially blocking function within an executor."""
+        if not asyncio.iscoroutinefunction(func):
+            return await blocking_func_to_async(self.executor, func, *args, **kwargs)
+        return await func(*args, **kwargs)
+
     async def preload_resource(self) -> None:
         """Preload resources before agent initialization."""
-        pass
+        if self.resource:
+            await self.blocking_func_to_async(self.resource.preload_resource)
 
     async def build(self) -> "ConversableAgent":
         """Build the agent."""
+        # Preload resources
+        await self.preload_resource()
         # Check if agent is available
         self.check_available()
         _language = self.not_null_agent_context.language
         if _language:
             self.language = _language
 
-        # Preload resources
-        await self.preload_resource()
         # Initialize resource loader
         for action in self.actions:
-            action.init_resource_loader(self.resource_loader)
+            action.init_resource(self.resource)
 
         # Initialize LLM Server
         if not self.is_human:
             if not self.llm_config or not self.llm_config.llm_client:
                 raise ValueError("LLM client is not initialized！")
             self.llm_client = AIWrapper(llm_client=self.llm_config.llm_client)
             self.memory.initialize(
@@ -171,21 +162,16 @@
         """Bind the resources to the agent."""
         if isinstance(target, LLMConfig):
             self.llm_config = target
         elif isinstance(target, GptsMemory):
             raise ValueError("GptsMemory is not supported!")
         elif isinstance(target, AgentContext):
             self.agent_context = target
-        elif isinstance(target, ResourceLoader):
-            self.resource_loader = target
-        elif isinstance(target, list) and target and len(target) > 0:
-            if _is_list_of_type(target, Action):
-                self.actions.extend(target)
-            elif _is_list_of_type(target, AgentResource):
-                self.resources = target
+        elif isinstance(target, Resource):
+            self.resource = target
         elif isinstance(target, AgentMemory):
             self.memory = target
         return self
 
     async def send(
         self,
         message: AgentMessage,
@@ -476,41 +462,41 @@
         reviewer: Optional[Agent] = None,
         **kwargs,
     ) -> Optional[ActionOutput]:
         """Perform actions."""
         last_out: Optional[ActionOutput] = None
         for i, action in enumerate(self.actions):
             # Select the resources required by acton
-            need_resource = None
-            if self.resources and len(self.resources) > 0:
-                for item in self.resources:
-                    if item.type == action.resource_need:
-                        need_resource = item
-                        break
+            if action.resource_need and self.resource:
+                need_resources = self.resource.get_resource_by_type(
+                    action.resource_need
+                )
+            else:
+                need_resources = []
 
             if not message:
                 raise ValueError("The message content is empty!")
 
             with root_tracer.start_span(
                 "agent.act.run",
                 metadata={
                     "message": message,
                     "sender": sender.name if sender else None,
                     "recipient": self.name,
                     "reviewer": reviewer.name if reviewer else None,
-                    "need_resource": need_resource.to_dict() if need_resource else None,
+                    "need_resource": need_resources[0].name if need_resources else None,
                     "rely_action_out": last_out.to_dict() if last_out else None,
                     "conv_uid": self.not_null_agent_context.conv_id,
                     "action_index": i,
                     "total_action": len(self.actions),
                 },
             ) as span:
                 last_out = await action.run(
                     ai_message=message,
-                    resource=need_resource,
+                    resource=None,
                     rely_action_out=last_out,
                     **kwargs,
                 )
                 span.metadata["action_out"] = last_out.to_dict() if last_out else None
         return last_out
 
     async def correctness_check(
@@ -699,31 +685,19 @@
 
         self._print_received_message(message, sender)
 
     async def generate_resource_variables(
         self, question: Optional[str] = None
     ) -> Dict[str, Any]:
         """Generate the resource variables."""
-        resource_prompt_list = []
-        for item in self.resources:
-            resource_client = self.not_null_resource_loader.get_resource_api(
-                item.type, ResourceClient
+        resource_prompt = None
+        if self.resource:
+            resource_prompt = await self.resource.get_prompt(
+                lang=self.language, question=question
             )
-            if not resource_client:
-                raise ValueError(
-                    f"Resource {item.type}:{item.value} missing resource loader"
-                    f" implementation,unable to read resources!"
-                )
-            resource_prompt_list.append(
-                await resource_client.get_resource_prompt(item, question)
-            )
-
-        resource_prompt = ""
-        if len(resource_prompt_list) > 0:
-            resource_prompt = "RESOURCES:" + "\n".join(resource_prompt_list)
 
         out_schema: Optional[str] = ""
         if self.actions and len(self.actions) > 0:
             out_schema = self.actions[0].ai_out_schema
         return {"resource_prompt": resource_prompt, "out_schema": out_schema}
 
     def _excluded_models(
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/core/base_team.py` & `dbgpt-0.5.7rc0/dbgpt/agent/core/base_team.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/core/memory/__init__.py` & `dbgpt-0.5.7rc0/dbgpt/agent/core/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/core/memory/agent_memory.py` & `dbgpt-0.5.7rc0/dbgpt/agent/core/memory/agent_memory.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/core/memory/base.py` & `dbgpt-0.5.7rc0/dbgpt/agent/core/memory/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/core/memory/gpts/__init__.py` & `dbgpt-0.5.7rc0/dbgpt/agent/core/memory/gpts/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/core/memory/gpts/base.py` & `dbgpt-0.5.7rc0/dbgpt/agent/core/memory/gpts/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/core/memory/gpts/default_gpts_memory.py` & `dbgpt-0.5.7rc0/dbgpt/agent/core/memory/gpts/default_gpts_memory.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/core/memory/gpts/gpts_memory.py` & `dbgpt-0.5.7rc0/dbgpt/agent/core/memory/gpts/gpts_memory.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/core/memory/hybrid.py` & `dbgpt-0.5.7rc0/dbgpt/agent/core/memory/hybrid.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/core/memory/llm.py` & `dbgpt-0.5.7rc0/dbgpt/agent/core/memory/llm.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/core/memory/long_term.py` & `dbgpt-0.5.7rc0/dbgpt/agent/core/memory/long_term.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/core/memory/short_term.py` & `dbgpt-0.5.7rc0/dbgpt/agent/core/memory/short_term.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/core/plan/__init__.py` & `dbgpt-0.5.7rc0/dbgpt/agent/core/plan/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/core/plan/awel/agent_operator.py` & `dbgpt-0.5.7rc0/dbgpt/agent/core/plan/awel/agent_operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 )
 from dbgpt.core.awel.trigger.base import Trigger
 from dbgpt.core.interface.message import ModelMessageRoleType
 
 # TODO: Don't dependent on MixinLLMOperator
 from dbgpt.model.operators.llm_operator import MixinLLMOperator
 
+from ....resource.manage import get_resource_manager
 from ....util.llm.llm import LLMConfig
 from ...agent import Agent, AgentGenerateContext, AgentMessage
 from ...agent_manage import get_agent_manager
 from ...base_agent import ConversableAgent
 from .agent_operator_resource import AWELAgent
 
 
@@ -224,15 +225,14 @@
             sender=agent,
             reviewer=input_value.reviewer,
             # Default single step transfer of information
             rely_messages=now_rely_messages,
             silent=input_value.silent,
             memory=input_value.memory.structure_clone() if input_value.memory else None,
             agent_context=input_value.agent_context,
-            resource_loader=input_value.resource_loader,
             llm_client=input_value.llm_client,
             round_index=agent.consecutive_auto_reply_counter,
         )
 
     async def get_agent(
         self,
         input_value: AgentGenerateContext,
@@ -258,21 +258,21 @@
 
         kwargs = {}
         if self.awel_agent.role_name:
             kwargs["name"] = self.awel_agent.role_name
         if self.awel_agent.fixed_subgoal:
             kwargs["fixed_subgoal"] = self.awel_agent.fixed_subgoal
 
+        resource = get_resource_manager().build_resource(self.awel_agent.resources)
         agent = (
             await agent_cls(**kwargs)
             .bind(input_value.memory)
             .bind(llm_config)
             .bind(input_value.agent_context)
-            .bind(self.awel_agent.resources)
-            .bind(input_value.resource_loader)
+            .bind(resource)
             .build()
         )
 
         return agent
 
 
 class AgentDummyTrigger(Trigger):
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/core/plan/awel/agent_operator_resource.py` & `dbgpt-0.5.7rc0/dbgpt/agent/core/plan/awel/agent_operator_resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,35 +8,38 @@
     FunctionDynamicOptions,
     OptionValue,
     Parameter,
     ResourceCategory,
     register_resource,
 )
 
-from ....resource.resource_api import AgentResource, ResourceType
+from ....resource.base import AgentResource
+from ....resource.manage import get_resource_manager
 from ....util.llm.llm import LLMConfig, LLMStrategyType
 from ...agent_manage import get_agent_manager
 
 
+def _load_resource_types():
+    resources = get_resource_manager().get_supported_resources()
+    return [OptionValue(label=item, name=item, value=item) for item in resources.keys()]
+
+
 @register_resource(
     label="AWEL Agent Resource",
     name="agent_operator_resource",
     description="The Agent Resource.",
     category=ResourceCategory.AGENT,
     parameters=[
         Parameter.build_from(
             label="Agent Resource Type",
             name="agent_resource_type",
             type=str,
             optional=True,
             default=None,
-            options=[
-                OptionValue(label=item.name, name=item.value, value=item.value)
-                for item in ResourceType
-            ],
+            options=FunctionDynamicOptions(func=_load_resource_types),
         ),
         Parameter.build_from(
             label="Agent Resource Name",
             name="agent_resource_name",
             type=str,
             optional=True,
             default=None,
@@ -66,15 +69,15 @@
         if not isinstance(values, dict):
             return values
         name = values.pop("agent_resource_name")
         type = values.pop("agent_resource_type")
         value = values.pop("agent_resource_value")
 
         values["name"] = name
-        values["type"] = ResourceType(type)
+        values["type"] = type
         values["value"] = value
 
         return values
 
 
 @register_resource(
     label="AWEL Agent LLM Config",
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/core/plan/awel/team_awel_layout.py` & `dbgpt-0.5.7rc0/dbgpt/agent/core/plan/awel/team_awel_layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,14 @@
 
             start_message_context: AgentGenerateContext = AgentGenerateContext(
                 message=AgentMessage(content=message, current_goal=message),
                 sender=sender,
                 reviewer=reviewer,
                 memory=self.memory.structure_clone(),
                 agent_context=self.agent_context,
-                resource_loader=self.resource_loader,
                 llm_client=self.not_null_llm_config.llm_client,
             )
             final_generate_context: AgentGenerateContext = await last_node.call(
                 call_data=start_message_context
             )
             last_message = final_generate_context.rely_messages[-1]
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/core/plan/plan_action.py` & `dbgpt-0.5.7rc0/dbgpt/agent/core/plan/plan_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 from typing import List, Optional
 
 from dbgpt._private.pydantic import BaseModel, Field
 from dbgpt.vis.tags.vis_agent_plans import Vis, VisAgentPlans
 
-from ...resource.resource_api import AgentResource
+from ...resource.base import AgentResource
 from ..action.base import Action, ActionOutput
 from ..agent import AgentContext
 from ..memory.gpts.base import GptsPlan
 from ..memory.gpts.gpts_memory import GptsPlansMemory
 from ..schema import Status
 
 logger = logging.getLogger(__name__)
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/core/plan/planner_agent.py` & `dbgpt-0.5.7rc0/dbgpt/agent/core/plan/planner_agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Planner Agent."""
 
-from typing import Any, Dict, List
+from typing import Any, Dict, List, Optional
 
 from dbgpt._private.pydantic import Field
 
+from ...resource.pack import ResourcePack
 from ..agent import AgentMessage
 from ..base_agent import ConversableAgent
 from ..plan.plan_action import PlanAction
 from ..profile import DynConfig, ProfileConfig
 
 
 class PlannerAgent(ConversableAgent):
@@ -85,59 +86,61 @@
         ),
         desc=DynConfig(
             "You are a task planning expert! You can coordinate intelligent agents"
             " and allocate resources to achieve complex task goals.",
             category="agent",
             key="dbgpt_agent_plan_planner_agent_profile_desc",
         ),
+        examples=DynConfig(
+            """
+user:help me build a sales report summarizing our key metrics and trends
+assistants:[
+    {{
+        "serial_number": "1",
+        "agent": "DataScientist",
+        "content": "Retrieve total sales, average sales, and number of transactions grouped by "product_category"'.",
+        "rely": ""
+    }},
+    {{
+        "serial_number": "2",
+        "agent": "DataScientist",
+        "content": "Retrieve monthly sales and transaction number trends.",
+        "rely": ""
+    }},
+    {{
+        "serial_number": "3",
+        "agent": "Reporter",
+        "content": "Integrate analytical data into the format required to build sales reports.",
+        "rely": "1,2"
+    }}
+]""",  # noqa: E501
+            category="agent",
+            key="dbgpt_agent_plan_planner_agent_profile_examples",
+        ),
     )
-    goal_zh: str = (
+    _goal_zh: str = (
         "理解下面每个智能体(agent)和他们的能力，使用给出的资源，通过协调智能体来解决"
         "用户问题。 请发挥你LLM的知识和理解能力，理解用户问题的意图和目标，生成一个可以在没有用户帮助"
         "下，由智能体协作完成目标的任务计划。"
     )
-    expand_prompt_zh: str = "可用智能体(agent):\n {{ agents }}"
+    _expand_prompt_zh: str = "可用智能体(agent):\n {{ agents }}"
 
-    constraints_zh: List[str] = [
+    _constraints_zh: List[str] = [
         "任务计划的每个步骤都应该是为了推进解决用户目标而存在，不要生成无意义的任务步骤，确保每个步骤内目标明确内容完整。",
         "关注任务计划每个步骤的依赖关系和逻辑，被依赖步骤要考虑被依赖的数据，是否能基于当前目标得到，如果不能请在目标中提示要生成被依赖数据。",
         "每个步骤都是一个独立可完成的目标，一定要确保逻辑和信息完整，不要出现类似:"
         "'Analyze the retrieved issues data'这样目标不明确，不知道具体要分析啥内容的步骤",
         "请确保只使用上面提到的智能体，并且可以只使用其中需要的部分，严格根据描述能力和限制分配给合适的步骤，每个智能体都可以重复使用。",
         "根据用户目标的实际需要使用提供的资源来协助生成计划步骤，不要使用不需要的资源。",
         "每个步骤最好只使用一种资源完成一个子目标，如果当前目标可以分解为同类型的多个子任务，可以生成相互不依赖的并行任务。",
         "数据资源可以被合适的智能体加载使用，不用考虑数据资源的加载链接问题",
         "尽量合并有顺序依赖的连续相同步骤,如果用户目标无拆分必要，可以生成内容为用户目标的单步任务。",
         "仔细检查计划，确保计划完整的包含了用户问题所涉及的所有信息，并且最终能完成目标，确认每个步骤是否包含了需要用到的资源信息,如URL、资源名等. ",
     ]
-    desc_zh: str = "你是一个任务规划专家！可以协调智能体，分配资源完成复杂的任务目标。"
-
-    examples: str = """
-    user:help me build a sales report summarizing our key metrics and trends
-    assistants:[
-        {{
-            "serial_number": "1",
-            "agent": "DataScientist",
-            "content": "Retrieve total sales, average sales, and number of transactions grouped by "product_category"'.",
-            "rely": ""
-        }},
-        {{
-            "serial_number": "2",
-            "agent": "DataScientist",
-            "content": "Retrieve monthly sales and transaction number trends.",
-            "rely": ""
-        }},
-        {{
-            "serial_number": "3",
-            "agent": "Reporter",
-            "content": "Integrate analytical data into the format required to build sales reports.",
-            "rely": "1,2"
-        }}
-    ]
-    """  # noqa: E501
+    _desc_zh: str = "你是一个任务规划专家！可以协调智能体，分配资源完成复杂的任务目标。"
 
     def __init__(self, **kwargs):
         """Create a new PlannerAgent instance."""
         super().__init__(**kwargs)
         self._init_actions([PlanAction])
 
     def _init_reply_message(self, received_message: AgentMessage):
@@ -146,18 +149,29 @@
             "agents": "\n".join([f"- {item.role}:{item.desc}" for item in self.agents]),
         }
         return reply_message
 
     def bind_agents(self, agents: List[ConversableAgent]) -> ConversableAgent:
         """Bind the agents to the planner agent."""
         self.agents = agents
+        resources = []
         for agent in self.agents:
-            if agent.resources and len(agent.resources) > 0:
-                self.resources.extend(agent.resources)
+            if agent.resource:
+                resources.append(agent.resource)
+        self.resource = ResourcePack(resources)
         return self
 
+    async def generate_resource_variables(
+        self, question: Optional[str] = None
+    ) -> Dict[str, Any]:
+        """Generate the resource variables."""
+        out_schema: Optional[str] = None
+        if self.actions and len(self.actions) > 0:
+            out_schema = self.actions[0].ai_out_schema
+        return {"out_schema": out_schema}
+
     def prepare_act_param(self) -> Dict[str, Any]:
         """Prepare the parameters for the act method."""
         return {
             "context": self.not_null_agent_context,
             "plans_memory": self.memory.plans_memory,
         }
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/core/plan/team_auto_plan.py` & `dbgpt-0.5.7rc0/dbgpt/agent/core/plan/team_auto_plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,14 @@
                         "resources still fails to build a valid plan！",
                     )
                 planner: ConversableAgent = (
                     await PlannerAgent()
                     .bind(self.memory)
                     .bind(self.agent_context)
                     .bind(self.llm_config)
-                    .bind(self.resource_loader)
                     .bind_agents(self.agents)
                     .build()
                 )
 
                 plan_message = await planner.generate_reply(
                     received_message=AgentMessage.from_llm_message(
                         {"content": message}
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/core/profile/__init__.py` & `dbgpt-0.5.7rc0/dbgpt/agent/core/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/core/profile/base.py` & `dbgpt-0.5.7rc0/dbgpt/agent/core/profile/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -95,14 +95,18 @@
         """
         return None
 
     def get_expand_prompt(self) -> Optional[str]:
         """Return the expand prompt of current agent."""
         return None
 
+    def get_examples(self) -> Optional[str]:
+        """Return the examples of current agent."""
+        return None
+
     @abstractmethod
     def get_system_prompt_template(self) -> str:
         """Return the prompt template of current agent."""
 
     @abstractmethod
     def get_user_prompt_template(self) -> str:
         """Return the user prompt template of current agent."""
@@ -126,14 +130,18 @@
         None, description="The description of the agent, not used to generate prompt."
     )
 
     expand_prompt: Optional[str] = Field(
         None, description="The expand prompt of the agent."
     )
 
+    examples: Optional[str] = Field(
+        None, description="The examples of the agent prompt."
+    )
+
     system_prompt_template: str = Field(
         _DEFAULT_SYSTEM_TEMPLATE, description="The system prompt template of the agent."
     )
     user_prompt_template: str = Field(
         _DEFAULT_USER_TEMPLATE, description="The user prompt template of the agent."
     )
 
@@ -165,14 +173,18 @@
         """
         return self.desc
 
     def get_expand_prompt(self) -> Optional[str]:
         """Return the expand prompt of current agent."""
         return self.expand_prompt
 
+    def get_examples(self) -> Optional[str]:
+        """Return the examples of current agent."""
+        return self.examples
+
     def get_system_prompt_template(self) -> str:
         """Return the prompt template of current agent."""
         return self.system_prompt_template
 
     def get_user_prompt_template(self) -> str:
         """Return the user prompt template of current agent."""
         return self.user_prompt_template
@@ -292,14 +304,16 @@
     constraints: List[str] | ConfigInfo | None = DynConfig(None, is_list=True)
     desc: str | ConfigInfo | None = DynConfig(
         None, description="The description of the agent."
     )
     expand_prompt: str | ConfigInfo | None = DynConfig(
         None, description="The expand prompt."
     )
+    examples: str | ConfigInfo | None = DynConfig(None, description="The examples.")
+
     system_prompt_template: str | ConfigInfo | None = DynConfig(
         _DEFAULT_SYSTEM_TEMPLATE, description="The prompt template."
     )
     user_prompt_template: str | ConfigInfo | None = DynConfig(
         _DEFAULT_USER_TEMPLATE, description="The user prompt template."
     )
     save_memory_template: str | ConfigInfo | None = DynConfig(
@@ -339,14 +353,15 @@
         goal = self.goal
         constraints = self.constraints
         desc = self.desc
         expand_prompt = self.expand_prompt
         system_prompt_template = self.system_prompt_template
         user_prompt_template = self.user_prompt_template
         save_memory_template = self.save_memory_template
+        examples = self.examples
         call_args = {
             "prefer_prompt_language": prefer_prompt_language,
             "prefer_model": prefer_model,
         }
         if isinstance(name, ConfigInfo):
             name = name.query(**call_args)
         if isinstance(role, ConfigInfo):
@@ -355,14 +370,16 @@
             goal = goal.query(**call_args)
         if isinstance(constraints, ConfigInfo):
             constraints = constraints.query(**call_args)
         if isinstance(desc, ConfigInfo):
             desc = desc.query(**call_args)
         if isinstance(expand_prompt, ConfigInfo):
             expand_prompt = expand_prompt.query(**call_args)
+        if isinstance(examples, ConfigInfo):
+            examples = examples.query(**call_args)
         if isinstance(system_prompt_template, ConfigInfo):
             system_prompt_template = system_prompt_template.query(**call_args)
         if isinstance(user_prompt_template, ConfigInfo):
             user_prompt_template = user_prompt_template.query(**call_args)
         if isinstance(save_memory_template, ConfigInfo):
             save_memory_template = save_memory_template.query(**call_args)
 
@@ -381,14 +398,15 @@
         return DefaultProfile(
             name=name,
             role=role,
             goal=goal,
             constraints=constraints,
             desc=desc,
             expand_prompt=expand_prompt,
+            examples=examples,
             system_prompt_template=system_prompt_template,
             user_prompt_template=user_prompt_template,
             save_memory_template=save_memory_template,
         )
 
     def __hash__(self):
         """Return the hash value."""
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/core/role.py` & `dbgpt-0.5.7rc0/dbgpt/agent/core/role.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,14 @@
         ...,
         description="The profile of the role.",
     )
     memory: AgentMemory = Field(default_factory=AgentMemory)
 
     fixed_subgoal: Optional[str] = Field(None, description="Fixed subgoal")
 
-    examples: str = ""
     language: str = "en"
     is_human: bool = False
     is_team: bool = False
 
     template_env: SandboxedEnvironment = Field(default_factory=SandboxedEnvironment)
 
     async def build_prompt(
@@ -57,15 +56,15 @@
             "goal": self.goal,
             "expand_prompt": self.expand_prompt,
             "language": self.language,
             "constraints": self.constraints,
             "most_recent_memories": (
                 most_recent_memories if most_recent_memories else None
             ),
-            "examples": self.examples if self.examples else None,
+            "examples": self.examples,
             # "out_schema": out_schema if out_schema else None,
             # "resource_prompt": resource_prompt if resource_prompt else None,
             "question": question,
         }
         resource_vars = await self.generate_resource_variables(question)
         pass_vars.update(resource_vars)
         pass_vars.update(kwargs)
@@ -106,14 +105,19 @@
 
     @property
     def name(self) -> str:
         """Return the name of the role."""
         return self.current_profile.get_name()
 
     @property
+    def examples(self) -> Optional[str]:
+        """Return the examples of the role."""
+        return self.current_profile.get_examples()
+
+    @property
     def role(self) -> str:
         """Return the role of the role."""
         return self.current_profile.get_role()
 
     @property
     def goal(self) -> Optional[str]:
         """Return the goal of the role."""
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/core/user_proxy_agent.py` & `dbgpt-0.5.7rc0/dbgpt/agent/core/user_proxy_agent.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/expand/Indicator_assistant_agent.py` & `dbgpt-0.5.7rc0/dbgpt/agent/expand/Indicator_assistant_agent.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/expand/actions/chart_action.py` & `dbgpt-0.5.7rc0/dbgpt/agent/expand/actions/chart_action.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Chart Action for SQL execution and rendering."""
 
 import json
 import logging
-from typing import Optional
+from typing import List, Optional
 
 from dbgpt._private.pydantic import BaseModel, Field, model_to_json
 from dbgpt.vis.tags.vis_chart import Vis, VisChart
 
 from ...core.action.base import Action, ActionOutput
-from ...resource.resource_api import AgentResource, ResourceType
-from ...resource.resource_db_api import ResourceDbClient
+from ...resource.base import AgentResource, ResourceType
+from ...resource.database import DBResource
 
 logger = logging.getLogger(__name__)
 
 
 class SqlInput(BaseModel):
     """SQL input model."""
 
@@ -65,42 +65,36 @@
         except Exception as e:
             logger.exception(f"{str(e)}! \n {ai_message}")
             return ActionOutput(
                 is_exe_success=False,
                 content="The requested correctly structured answer could not be found.",
             )
         try:
-            if not self.resource_loader:
-                raise ValueError("ResourceLoader is not initialized！")
-            resource_db_client: Optional[
-                ResourceDbClient
-            ] = self.resource_loader.get_resource_api(
-                self.resource_need, ResourceDbClient
-            )
-            if not resource_db_client:
-                raise ValueError(
-                    "There is no implementation class bound to database resource "
-                    "execution！"
-                )
-            if not resource:
-                raise ValueError("The data resource is not found！")
-            data_df = await resource_db_client.query_to_df(resource.value, param.sql)
+            if not self.resource_need:
+                raise ValueError("The resource type is not found！")
+
             if not self.render_protocol:
                 raise ValueError("The rendering protocol is not initialized！")
+
+            db_resources: List[DBResource] = DBResource.from_resource(self.resource)
+            if not db_resources:
+                raise ValueError("The database resource is not found！")
+
+            db = db_resources[0]
+            data_df = await db.query_to_df(param.sql)
             view = await self.render_protocol.display(
                 chart=json.loads(model_to_json(param)), data_df=data_df
             )
-            if not self.resource_need:
-                raise ValueError("The resource type is not found！")
+
             return ActionOutput(
                 is_exe_success=True,
                 content=model_to_json(param),
                 view=view,
                 resource_type=self.resource_need.value,
-                resource_value=resource.value,
+                resource_value=db._db_name,
             )
         except Exception as e:
             logger.exception("Check your answers, the sql run failed！")
             return ActionOutput(
                 is_exe_success=False,
                 content=f"Check your answers, the sql run failed!Reason:{str(e)}",
             )
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/expand/actions/code_action.py` & `dbgpt-0.5.7rc0/dbgpt/agent/expand/actions/code_action.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Optional, Union
 
 from dbgpt.util.code_utils import UNKNOWN, execute_code, extract_code, infer_lang
 from dbgpt.util.utils import colored
 from dbgpt.vis.tags.vis_code import Vis, VisCode
 
 from ...core.action.base import Action, ActionOutput
-from ...resource.resource_api import AgentResource
+from ...resource.base import AgentResource
 
 logger = logging.getLogger(__name__)
 
 
 class CodeAction(Action[None]):
     """Code Action Module."""
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/expand/actions/dashboard_action.py` & `dbgpt-0.5.7rc0/dbgpt/agent/expand/actions/dashboard_action.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import logging
 from typing import List, Optional
 
 from dbgpt._private.pydantic import BaseModel, Field, model_to_dict
 from dbgpt.vis.tags.vis_dashboard import Vis, VisDashboard
 
 from ...core.action.base import Action, ActionOutput
-from ...resource.resource_api import AgentResource, ResourceType
-from ...resource.resource_db_api import ResourceDbClient
+from ...resource.base import AgentResource, ResourceType
+from ...resource.database import DBResource
 
 logger = logging.getLogger(__name__)
 
 
 class ChartItem(BaseModel):
     """Chart item model."""
 
@@ -79,37 +79,28 @@
         if not isinstance(input_param, list):
             return ActionOutput(
                 is_exe_success=False,
                 content="The requested correctly structured answer could not be found.",
             )
         chart_items: List[ChartItem] = input_param
         try:
-            if not self.resource_loader:
-                raise ValueError("Resource loader is not initialized!")
-            resource_db_client: Optional[
-                ResourceDbClient
-            ] = self.resource_loader.get_resource_api(
-                self.resource_need, ResourceDbClient
-            )
-            if not resource_db_client:
-                raise ValueError(
-                    "There is no implementation class bound to database resource "
-                    "execution！"
-                )
+            db_resources: List[DBResource] = DBResource.from_resource(self.resource)
+            if not db_resources:
+                raise ValueError("The database resource is not found！")
+
+            db = db_resources[0]
 
-            if not resource:
-                raise ValueError("Resource is not initialized!")
+            if not db:
+                raise ValueError("The database resource is not found！")
 
             chart_params = []
             for chart_item in chart_items:
                 chart_dict = {}
                 try:
-                    sql_df = await resource_db_client.query_to_df(
-                        resource.value, chart_item.sql
-                    )
+                    sql_df = await db.query_to_df(chart_item.sql)
                     chart_dict = chart_item.to_dict()
 
                     chart_dict["data"] = sql_df
                 except Exception as e:
                     logger.warning(f"Sql execute failed！{str(e)}")
                     chart_dict["err_msg"] = str(e)
                 chart_params.append(chart_dict)
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/expand/actions/indicator_action.py` & `dbgpt-0.5.7rc0/dbgpt/agent/expand/actions/indicator_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Optional
 
 from dbgpt._private.pydantic import BaseModel, Field
 from dbgpt.vis.tags.vis_plugin import Vis, VisPlugin
 
 from ...core.action.base import Action, ActionOutput
 from ...core.schema import Status
-from ...resource.resource_api import AgentResource, ResourceType
+from ...resource.base import AgentResource, ResourceType
 
 logger = logging.getLogger(__name__)
 
 
 class IndicatorInput(BaseModel):
     """Indicator input model."""
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/expand/actions/plugin_action.py` & `dbgpt-0.5.7rc0/dbgpt/agent/expand/actions/tool_action.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,22 +5,21 @@
 from typing import Optional
 
 from dbgpt._private.pydantic import BaseModel, Field
 from dbgpt.vis.tags.vis_plugin import Vis, VisPlugin
 
 from ...core.action.base import Action, ActionOutput
 from ...core.schema import Status
-from ...plugin.generator import PluginPromptGenerator
-from ...resource.resource_api import AgentResource, ResourceType
-from ...resource.resource_plugin_api import ResourcePluginClient
+from ...resource.base import AgentResource, ResourceType
+from ...resource.tool.pack import ToolPack
 
 logger = logging.getLogger(__name__)
 
 
-class PluginInput(BaseModel):
+class ToolInput(BaseModel):
     """Plugin input model."""
 
     tool_name: str = Field(
         ...,
         description="The name of a tool that can be used to answer the current question"
         " or solve the current task.",
     )
@@ -28,48 +27,48 @@
         default={"arg name1": "", "arg name2": ""},
         description="The tool selected for the current target, the parameter "
         "information required for execution",
     )
     thought: str = Field(..., description="Summary of thoughts to the user")
 
 
-class PluginAction(Action[PluginInput]):
-    """Plugin action class."""
+class ToolAction(Action[ToolInput]):
+    """Tool action class."""
 
     def __init__(self):
         """Create a plugin action."""
         super().__init__()
         self._render_protocol = VisPlugin()
 
     @property
     def resource_need(self) -> Optional[ResourceType]:
         """Return the resource type needed for the action."""
-        return ResourceType.Plugin
+        return ResourceType.Tool
 
     @property
     def render_protocol(self) -> Optional[Vis]:
         """Return the render protocol."""
         return self._render_protocol
 
     @property
     def out_model_type(self):
         """Return the output model type."""
-        return PluginInput
+        return ToolInput
 
     @property
     def ai_out_schema(self) -> Optional[str]:
         """Return the AI output schema."""
         out_put_schema = {
+            "thought": "Summary of thoughts to the user",
             "tool_name": "The name of a tool that can be used to answer the current "
             "question or solve the current task.",
             "args": {
                 "arg name1": "arg value1",
                 "arg name2": "arg value2",
             },
-            "thought": "Summary of thoughts to the user",
         }
 
         return f"""Please response in the following json format:
         {json.dumps(out_put_schema, indent=2, ensure_ascii=False)}
         Make sure the response is correct json and can be parsed by Python json.loads.
         """
 
@@ -88,70 +87,60 @@
             resource (Optional[AgentResource], optional): The resource. Defaults to
                 None.
             rely_action_out (Optional[ActionOutput], optional): The rely action output.
                 Defaults to None.
             need_vis_render (bool, optional): Whether need visualization rendering.
                 Defaults to True.
         """
-        plugin_generator: Optional[PluginPromptGenerator] = kwargs.get(
-            "plugin_generator", None
-        )
-        if not plugin_generator:
-            raise ValueError("No plugin generator found!")
         try:
-            param: PluginInput = self._input_convert(ai_message, PluginInput)
+            param: ToolInput = self._input_convert(ai_message, ToolInput)
         except Exception as e:
             logger.exception((str(e)))
             return ActionOutput(
                 is_exe_success=False,
                 content="The requested correctly structured answer could not be found.",
             )
 
         try:
-            if not self.resource_loader:
-                raise ValueError("No resource_loader found!")
-            resource_plugin_client: Optional[
-                ResourcePluginClient
-            ] = self.resource_loader.get_resource_api(
-                self.resource_need, ResourcePluginClient
-            )
-            if not resource_plugin_client:
-                raise ValueError("No implementation of the use of plug-in resources！")
+            tool_packs = ToolPack.from_resource(self.resource)
+            if not tool_packs:
+                raise ValueError("The tool resource is not found！")
+            tool_pack = tool_packs[0]
             response_success = True
             status = Status.RUNNING.value
             err_msg = None
             try:
-                tool_result = await resource_plugin_client.execute_command(
-                    param.tool_name, param.args, plugin_generator
+                tool_result = await tool_pack.async_execute(
+                    resource_name=param.tool_name, **param.args
                 )
                 status = Status.COMPLETE.value
             except Exception as e:
                 response_success = False
                 logger.exception(f"Tool [{param.tool_name}] execute failed!")
                 status = Status.FAILED.value
                 err_msg = f"Tool [{param.tool_name}] execute failed! {str(e)}"
                 tool_result = err_msg
 
             plugin_param = {
                 "name": param.tool_name,
                 "args": param.args,
                 "status": status,
                 "logo": None,
-                "result": tool_result,
+                "result": str(tool_result),
                 "err_msg": err_msg,
             }
             if not self.render_protocol:
                 raise NotImplementedError("The render_protocol should be implemented.")
 
             view = await self.render_protocol.display(content=plugin_param)
 
             return ActionOutput(
                 is_exe_success=response_success,
-                content=tool_result,
+                content=str(tool_result),
                 view=view,
-                observations=tool_result,
+                observations=str(tool_result),
             )
         except Exception as e:
             logger.exception("Tool Action Run Failed！")
             return ActionOutput(
                 is_exe_success=False, content=f"Tool action run failed!{str(e)}"
             )
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/expand/code_assistant_agent.py` & `dbgpt-0.5.7rc0/dbgpt/agent/expand/code_assistant_agent.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/expand/dashboard_assistant_agent.py` & `dbgpt-0.5.7rc0/dbgpt/agent/expand/dashboard_assistant_agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Dashboard Assistant Agent."""
 
+from typing import List
+
 from ..core.agent import AgentMessage
 from ..core.base_agent import ConversableAgent
 from ..core.profile import DynConfig, ProfileConfig
-from ..resource.resource_db_api import ResourceDbClient
+from ..resource.database import DBResource
 from .actions.dashboard_action import DashboardAction
 
 
 class DashboardAssistantAgent(ConversableAgent):
     """Dashboard Assistant Agent."""
 
     profile: ProfileConfig = ProfileConfig(
@@ -54,19 +56,20 @@
     def __init__(self, **kwargs):
         """Create a new instance of DashboardAssistantAgent."""
         super().__init__(**kwargs)
         self._init_actions([DashboardAction])
 
     def _init_reply_message(self, received_message: AgentMessage) -> AgentMessage:
         reply_message = super()._init_reply_message(received_message)
-        client = self.not_null_resource_loader.get_resource_api(
-            self.actions[0].resource_need, ResourceDbClient
-        )
-        if not client:
+
+        dbs: List[DBResource] = DBResource.from_resource(self.resource)
+
+        if not dbs:
             raise ValueError(
                 f"Resource type {self.actions[0].resource_need} is not supported."
             )
+        db = dbs[0]
         reply_message.context = {
             "display_type": self.actions[0].render_prompt(),
-            "dialect": client.get_data_type(self.resources[0]),
+            "dialect": db.dialect,
         }
         return reply_message
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/expand/data_scientist_agent.py` & `dbgpt-0.5.7rc0/dbgpt/agent/expand/data_scientist_agent.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """Data Scientist Agent."""
 
 import json
 import logging
-from typing import Optional, Tuple, cast
+from typing import List, Optional, Tuple, cast
 
 from ..core.action.base import ActionOutput
 from ..core.agent import AgentMessage
 from ..core.base_agent import ConversableAgent
 from ..core.profile import DynConfig, ProfileConfig
-from ..resource.resource_api import ResourceType
-from ..resource.resource_db_api import ResourceDbClient
+from ..resource.database import DBResource
 from .actions.chart_action import ChartAction
 
 logger = logging.getLogger(__name__)
 
 
 class DataScientistAgent(ConversableAgent):
     """Data Scientist Agent."""
@@ -70,27 +69,30 @@
     def __init__(self, **kwargs):
         """Create a new DataScientistAgent instance."""
         super().__init__(**kwargs)
         self._init_actions([ChartAction])
 
     def _init_reply_message(self, received_message: AgentMessage) -> AgentMessage:
         reply_message = super()._init_reply_message(received_message)
-        client = self.not_null_resource_loader.get_resource_api(
-            self.actions[0].resource_need, ResourceDbClient
-        )
-        if not client:
-            raise ValueError(
-                f"Resource type {self.actions[0].resource_need} is not supported."
-            )
         reply_message.context = {
             "display_type": self.actions[0].render_prompt(),
-            "dialect": client.get_data_type(self.resources[0]),
+            "dialect": self.database.dialect,
         }
         return reply_message
 
+    @property
+    def database(self) -> DBResource:
+        """Get the database resource."""
+        dbs: List[DBResource] = DBResource.from_resource(self.resource)
+        if not dbs:
+            raise ValueError(
+                f"Resource type {self.actions[0].resource_need} is not supported."
+            )
+        return dbs[0]
+
     async def correctness_check(
         self, message: AgentMessage
     ) -> Tuple[bool, Optional[str]]:
         """Verify whether the current execution results meet the target expectations."""
         action_reply = message.action_report
         if action_reply is None:
             return (
@@ -108,34 +110,24 @@
         if not sql:
             return (
                 False,
                 "Please check your answer, the sql information that needs to be "
                 "generated is not found.",
             )
         try:
-            resource_db_client: Optional[
-                ResourceDbClient
-            ] = self.not_null_resource_loader.get_resource_api(
-                ResourceType(action_out.resource_type), ResourceDbClient
-            )
-            if not resource_db_client:
-                return (
-                    False,
-                    "Please check your answer, the data resource type is not "
-                    "supported.",
-                )
             if not action_out.resource_value:
                 return (
                     False,
                     "Please check your answer, the data resource information is not "
                     "found.",
                 )
 
-            columns, values = await resource_db_client.query(
-                db=action_out.resource_value, sql=sql
+            columns, values = await self.database.query(
+                sql=sql,
+                db=action_out.resource_value,
             )
             if not values or len(values) <= 0:
                 return (
                     False,
                     "Please check your answer, the current SQL cannot find the data to "
                     "determine whether filtered field values or inappropriate filter "
                     "conditions are used.",
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/expand/retrieve_summary_assistant_agent.py` & `dbgpt-0.5.7rc0/dbgpt/agent/expand/retrieve_summary_assistant_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from dbgpt.configs.model_config import PILOT_PATH
 from dbgpt.core import ModelMessageRoleType
 
 from ..core.action.base import Action, ActionOutput
 from ..core.agent import Agent, AgentMessage, AgentReviewInfo
 from ..core.base_agent import ConversableAgent
 from ..core.profile import ProfileConfig
-from ..resource.resource_api import AgentResource
+from ..resource.base import AgentResource
 from ..util.cmp import cmp_string_equal
 
 try:
     from unstructured.partition.auto import partition
 
     HAS_UNSTRUCTURED = True
 except ImportError:
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/expand/summary_assistant_agent.py` & `dbgpt-0.5.7rc0/dbgpt/agent/expand/summary_assistant_agent.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/plugin/commands/exceptions.py` & `dbgpt-0.5.7rc0/dbgpt/agent/resource/tool/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-"""Exceptions for the commands plugin."""
+"""Exceptions for the tool."""
 
 
-class CommandException(Exception):
-    """Common command error exception."""
+class ToolException(Exception):
+    """Common tool error exception."""
 
     def __init__(self, message: str, error_type: str = "Common Error"):
-        """Create a new CommandException instance."""
+        """Create a new ToolException instance."""
         super().__init__(message)
         self.message = message
         self.error_type = error_type
 
 
-class CreateCommandException(CommandException):
-    """Create command error exception."""
+class CreateToolException(ToolException):
+    """Create tool error exception."""
 
     def __init__(self, message: str, error_type="Create Command Error"):
-        """Create a new CreateCommandException instance."""
+        """Create a new CreateToolException instance."""
         super().__init__(message, error_type)
 
 
-class NotCommandException(CommandException):
-    """Command not found exception."""
+class ToolNotFoundException(ToolException):
+    """Tool not found exception."""
 
     def __init__(self, message: str, error_type="Not Command Error"):
-        """Create a new NotCommandException instance."""
+        """Create a new ToolNotFoundException instance."""
         super().__init__(message, error_type)
 
 
-class ExecutionCommandException(CommandException):
-    """Command execution error exception."""
+class ToolExecutionException(ToolException):
+    """Tool execution error exception."""
 
     def __init__(self, message: str, error_type="Execution Command Error"):
-        """Create a new ExecutionCommandException instance."""
+        """Create a new ToolExecutionException instance."""
         super().__init__(message, error_type)
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/plugin/plugins_util.py` & `dbgpt-0.5.7rc0/dbgpt/agent/resource/tool/autogpt/plugins_util.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-"""Load plugins from a directory or a zip file."""
+"""Load plugins from a directory or a zip file.
+
+This module provides utility functions to load auto_gpt plugins from a directory or a
+zip file.
+"""
 
 import datetime
 import glob
 import json
 import logging
 import os
 from pathlib import Path
 from typing import TYPE_CHECKING, List, Optional
 
-from dbgpt._private.config import Config
-
 if TYPE_CHECKING:
     from auto_gpt_plugin_template import AutoGPTPluginTemplate
 
 logger = logging.getLogger(__name__)
 
 
 def inspect_zip_for_modules(zip_path: str, debug: bool = False) -> list[str]:
@@ -127,38 +129,14 @@
     if loaded_plugins:
         logger.info(f"\nPlugins found: {len(loaded_plugins)}\n" "--------------------")
     for plugin in loaded_plugins:
         logger.info(f"{plugin._name}: {plugin._version} - {plugin._description}")
     return loaded_plugins
 
 
-def denylist_allowlist_check(plugin_name: str, cfg: Config) -> bool:
-    """Check if the plugin is in the allowlist or denylist.
-
-    Args:
-        plugin_name (str): Name of the plugin.
-        cfg (Config): Config object.
-
-    Returns:
-        True or False
-    """
-    logger.debug(f"Checking if plugin {plugin_name} should be loaded")
-    if plugin_name in cfg.plugins_denylist:
-        logger.debug(f"Not loading plugin {plugin_name} as it was in the denylist.")
-        return False
-    if plugin_name in cfg.plugins_allowlist:
-        logger.debug(f"Loading plugin {plugin_name} as it was in the allowlist.")
-        return True
-    ack = input(
-        f"WARNING: Plugin {plugin_name} found. But not in the"
-        f" allowlist... Load? ({cfg.authorise_key}/{cfg.exit_key}): "
-    )
-    return ack.lower() == cfg.authorise_key
-
-
 def update_from_git(
     download_path: str,
     github_repo: str = "",
     branch_name: str = "main",
     authorization: Optional[str] = None,
 ):
     """Update plugins from a git repository."""
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/util/cmp.py` & `dbgpt-0.5.7rc0/dbgpt/agent/util/cmp.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/util/llm/llm.py` & `dbgpt-0.5.7rc0/dbgpt/agent/util/llm/llm.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/util/llm/llm_client.py` & `dbgpt-0.5.7rc0/dbgpt/agent/util/llm/llm_client.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/agent/util/llm/strategy/priority.py` & `dbgpt-0.5.7rc0/dbgpt/agent/util/llm/strategy/priority.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/cli/cli_scripts.py` & `dbgpt-0.5.7rc0/dbgpt/cli/cli_scripts.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/client/_cli.py` & `dbgpt-0.5.7rc0/dbgpt/client/_cli.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/client/app.py` & `dbgpt-0.5.7rc0/dbgpt/client/app.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/client/client.py` & `dbgpt-0.5.7rc0/dbgpt/client/client.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/client/datasource.py` & `dbgpt-0.5.7rc0/dbgpt/client/datasource.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/client/flow.py` & `dbgpt-0.5.7rc0/dbgpt/client/flow.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/client/knowledge.py` & `dbgpt-0.5.7rc0/dbgpt/client/knowledge.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/client/schema.py` & `dbgpt-0.5.7rc0/dbgpt/client/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """this module contains the schemas for the dbgpt client."""
+
 import json
 from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
 from fastapi import File, UploadFile
 
@@ -139,28 +140,28 @@
     ImageFile = "image_file"
     AWELFlow = "awel_flow"
 
 
 class AgentResourceModel(BaseModel):
     """Agent resource model."""
 
-    type: AgentResourceType
+    type: str
     name: str
     value: str
     is_dynamic: bool = (
         False  # Is the current resource predefined or dynamically passed in?
     )
 
     @staticmethod
     def from_dict(d: Dict[str, Any]):
         """From dict."""
         if d is None:
             return None
         return AgentResourceModel(
-            type=AgentResourceType(d.get("type")),
+            type=d.get("type"),
             name=d.get("name"),
             introduce=d.get("introduce"),
             value=d.get("value", None),
             is_dynamic=d.get("is_dynamic", False),
         )
 
     @staticmethod
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/component.py` & `dbgpt-0.5.7rc0/dbgpt/component.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Component module for dbgpt.
 
 Manages the lifecycle and registration of components.
 """
+
 from __future__ import annotations
 
 import asyncio
 import atexit
 import logging
 import sys
 import threading
@@ -83,14 +84,15 @@
     TRACER_SPAN_STORAGE = "dbgpt_tracer_span_storage"
     RAG_GRAPH_DEFAULT = "dbgpt_rag_engine_default"
     AWEL_TRIGGER_MANAGER = "dbgpt_awel_trigger_manager"
     AWEL_DAG_MANAGER = "dbgpt_awel_dag_manager"
     UNIFIED_METADATA_DB_MANAGER_FACTORY = "dbgpt_unified_metadata_db_manager_factory"
     CONNECTOR_MANAGER = "dbgpt_connector_manager"
     AGENT_MANAGER = "dbgpt_agent_manager"
+    RESOURCE_MANAGER = "dbgpt_resource_manager"
 
 
 _EMPTY_DEFAULT_COMPONENT = "_EMPTY_DEFAULT_COMPONENT"
 
 
 @PublicAPI(stability="beta")
 class BaseComponent(LifeCycle, ABC):
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/configs/__init__.py` & `dbgpt-0.5.7rc0/dbgpt/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/configs/model_config.py` & `dbgpt-0.5.7rc0/dbgpt/configs/model_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os
 from functools import cache
 
 ROOT_PATH = os.path.dirname(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 MODEL_PATH = os.path.join(ROOT_PATH, "models")
 PILOT_PATH = os.path.join(ROOT_PATH, "pilot")
 LOGDIR = os.getenv("DBGPT_LOG_DIR", os.path.join(ROOT_PATH, "logs"))
+STATIC_MESSAGE_IMG_PATH = os.path.join(PILOT_PATH, "message/img")
 
 DATASETS_DIR = os.path.join(PILOT_PATH, "datasets")
 DATA_DIR = os.path.join(PILOT_PATH, "data")
 PLUGINS_DIR = os.path.join(ROOT_PATH, "plugins")
 MODEL_DISK_CACHE_DIR = os.path.join(DATA_DIR, "model_cache")
 _DAG_DEFINITION_DIR = os.path.join(ROOT_PATH, "examples/awel")
 # Global language setting
@@ -66,14 +67,16 @@
     "bc_proxyllm": "bc_proxyllm",
     "spark_proxyllm": "spark_proxyllm",
     # https://platform.lingyiwanwu.com/docs/
     "yi_proxyllm": "yi_proxyllm",
     # https://platform.moonshot.cn/docs/
     "moonshot_proxyllm": "moonshot_proxyllm",
     "ollama_proxyllm": "ollama_proxyllm",
+    # https://platform.deepseek.com/api-docs/
+    "deepseek_proxyllm": "deepseek_proxyllm",
     "llama-2-7b": os.path.join(MODEL_PATH, "Llama-2-7b-chat-hf"),
     "llama-2-13b": os.path.join(MODEL_PATH, "Llama-2-13b-chat-hf"),
     "llama-2-70b": os.path.join(MODEL_PATH, "Llama-2-70b-chat-hf"),
     # https://huggingface.co/meta-llama/Meta-Llama-3-8B-Instruct
     "meta-llama-3-8b-instruct": os.path.join(MODEL_PATH, "Meta-Llama-3-8B-Instruct"),
     # https://huggingface.co/meta-llama/Meta-Llama-3-70B-Instruct
     "meta-llama-3-70b-instruct": os.path.join(MODEL_PATH, "Meta-Llama-3-70B-Instruct"),
@@ -137,14 +140,15 @@
     "orca-2-7b": os.path.join(MODEL_PATH, "Orca-2-7b"),
     # https://huggingface.co/microsoft/Orca-2-13b
     "orca-2-13b": os.path.join(MODEL_PATH, "Orca-2-13b"),
     # https://huggingface.co/openchat/openchat_3.5
     "openchat-3.5": os.path.join(MODEL_PATH, "openchat_3.5"),
     # https://huggingface.co/openchat/openchat-3.5-1210
     "openchat-3.5-1210": os.path.join(MODEL_PATH, "openchat-3.5-1210"),
+    "openchat-3.6-8b-20240522": os.path.join(MODEL_PATH, "openchat-3.6-8b-20240522"),
     # https://huggingface.co/hfl/chinese-alpaca-2-7b
     "chinese-alpaca-2-7b": os.path.join(MODEL_PATH, "chinese-alpaca-2-7b"),
     # https://huggingface.co/hfl/chinese-alpaca-2-13b
     "chinese-alpaca-2-13b": os.path.join(MODEL_PATH, "chinese-alpaca-2-13b"),
     # https://huggingface.co/THUDM/codegeex2-6b
     "codegeex2-6b": os.path.join(MODEL_PATH, "codegeex2-6b"),
     # https://huggingface.co/HuggingFaceH4/zephyr-7b-alpha
@@ -168,19 +172,37 @@
     # https://huggingface.co/01-ai/Yi-34B-Chat
     "yi-34b-chat": os.path.join(MODEL_PATH, "Yi-34B-Chat"),
     # https://huggingface.co/01-ai/Yi-34B-Chat-8bits
     "yi-34b-chat-8bits": os.path.join(MODEL_PATH, "Yi-34B-Chat-8bits"),
     # https://huggingface.co/01-ai/Yi-34B-Chat-4bits
     "yi-34b-chat-4bits": os.path.join(MODEL_PATH, "Yi-34B-Chat-4bits"),
     "yi-6b-chat": os.path.join(MODEL_PATH, "Yi-6B-Chat"),
+    # https://huggingface.co/01-ai/Yi-1.5-6B-Chat
+    "yi-1.5-6b-chat": os.path.join(MODEL_PATH, "Yi-1.5-6B-Chat"),
+    "yi-1.5-9b-chat": os.path.join(MODEL_PATH, "Yi-1.5-9B-Chat"),
+    "yi-1.5-9b-chat-16k": os.path.join(MODEL_PATH, "Yi-1.5-9B-Chat-16K"),
+    "yi-1.5-34b-chat": os.path.join(MODEL_PATH, "Yi-1.5-34B-Chat"),
+    "yi-1.5-34b-chat-16k": os.path.join(MODEL_PATH, "Yi-1.5-34B-Chat-16K"),
     # https://huggingface.co/google/gemma-7b-it
     "gemma-7b-it": os.path.join(MODEL_PATH, "gemma-7b-it"),
     # https://huggingface.co/google/gemma-2b-it
     "gemma-2b-it": os.path.join(MODEL_PATH, "gemma-2b-it"),
     "starling-lm-7b-beta": os.path.join(MODEL_PATH, "Starling-LM-7B-beta"),
+    "deepseek-v2-lite-chat": os.path.join(MODEL_PATH, "DeepSeek-V2-Lite-Chat"),
+    "sailor-14b-chat": os.path.join(MODEL_PATH, "Sailor-14B-Chat"),
+    # https://huggingface.co/microsoft/Phi-3-medium-128k-instruct
+    "phi-3-medium-128k-instruct": os.path.join(
+        MODEL_PATH, "Phi-3-medium-128k-instruct"
+    ),
+    "phi-3-medium-4k-instruct": os.path.join(MODEL_PATH, "Phi-3-medium-4k-instruct"),
+    "phi-3-small-128k-instruct": os.path.join(MODEL_PATH, "Phi-3-small-128k-instruct"),
+    "phi-3-small-8k-instruct": os.path.join(MODEL_PATH, "Phi-3-small-8k-instruct"),
+    "phi-3-mini-128k-instruct": os.path.join(MODEL_PATH, "Phi-3-mini-128k-instruct"),
+    "phi-3-mini-4k-instruct": os.path.join(MODEL_PATH, "Phi-3-mini-4k-instruct"),
+    "llama-3-sqlcoder-8b": os.path.join(MODEL_PATH, "llama-3-sqlcoder-8b"),
 }
 
 EMBEDDING_MODEL_CONFIG = {
     "text2vec": os.path.join(MODEL_PATH, "text2vec-large-chinese"),
     "text2vec-base": os.path.join(MODEL_PATH, "text2vec-base-chinese"),
     # https://huggingface.co/moka-ai/m3e-large
     "m3e-base": os.path.join(MODEL_PATH, "m3e-base"),
@@ -198,11 +220,16 @@
     "gte-base-zh": os.path.join(MODEL_PATH, "gte-base-zh"),
     "sentence-transforms": os.path.join(MODEL_PATH, "all-MiniLM-L6-v2"),
     "proxy_openai": "proxy_openai",
     "proxy_azure": "proxy_azure",
     # Common HTTP embedding model
     "proxy_http_openapi": "proxy_http_openapi",
     "proxy_ollama": "proxy_ollama",
+    # Rerank model, rerank mode is a special embedding model
+    "bge-reranker-base": os.path.join(MODEL_PATH, "bge-reranker-base"),
+    "bge-reranker-large": os.path.join(MODEL_PATH, "bge-reranker-large"),
+    # Proxy rerank model
+    "rerank_proxy_http_openapi": "rerank_proxy_http_openapi",
 }
 
 
 KNOWLEDGE_UPLOAD_ROOT_PATH = DATA_DIR
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/__init__.py` & `dbgpt-0.5.7rc0/dbgpt/core/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from dbgpt.core.interface.cache import (  # noqa: F401
     CacheClient,
     CacheConfig,
     CacheKey,
     CachePolicy,
     CacheValue,
 )
-from dbgpt.core.interface.embeddings import Embeddings  # noqa: F401
+from dbgpt.core.interface.embeddings import Embeddings, RerankEmbeddings  # noqa: F401
 from dbgpt.core.interface.knowledge import Chunk, Document  # noqa: F401
 from dbgpt.core.interface.llm import (  # noqa: F401
     DefaultMessageConverter,
     LLMClient,
     MessageConverter,
     ModelExtraMedata,
     ModelInferenceMetrics,
@@ -102,10 +102,11 @@
     "StorageItemAdapter",
     "StorageInterface",
     "InMemoryStorage",
     "DefaultStorageItemAdapter",
     "QuerySpec",
     "StorageError",
     "Embeddings",
+    "RerankEmbeddings",
     "Chunk",
     "Document",
 ]
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/_private/example_base.py` & `dbgpt-0.5.7rc0/dbgpt/core/_private/example_base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/_private/prompt_registry.py` & `dbgpt-0.5.7rc0/dbgpt/core/_private/prompt_registry.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/awel/__init__.py` & `dbgpt-0.5.7rc0/dbgpt/core/awel/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from dbgpt.component import SystemApp
 
 from .dag.base import DAG, DAGContext, DAGVar
 from .operators.base import BaseOperator, WorkflowRunner
 from .operators.common_operator import (
     BranchFunc,
     BranchOperator,
+    BranchTaskType,
     InputOperator,
     JoinOperator,
     MapOperator,
     ReduceStreamOperator,
     TriggerOperator,
 )
 from .operators.stream_operator import (
@@ -76,14 +77,15 @@
     "JoinOperator",
     "ReduceStreamOperator",
     "TriggerOperator",
     "MapOperator",
     "BranchOperator",
     "InputOperator",
     "BranchFunc",
+    "BranchTaskType",
     "WorkflowRunner",
     "TaskState",
     "is_empty_data",
     "TaskOutput",
     "TaskContext",
     "InputContext",
     "InputSource",
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/awel/dag/base.py` & `dbgpt-0.5.7rc0/dbgpt/core/awel/dag/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/awel/dag/dag_manager.py` & `dbgpt-0.5.7rc0/dbgpt/core/awel/dag/dag_manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/awel/dag/loader.py` & `dbgpt-0.5.7rc0/dbgpt/core/awel/dag/loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """DAG loader.
 
 DAGLoader will load DAGs from dag_dirs or other sources.
 Now only support load DAGs from local files.
 """
+
 import hashlib
 import logging
 import os
 import sys
 import traceback
 from abc import ABC, abstractmethod
 from typing import List
@@ -94,21 +95,24 @@
             logger.error(f"Failed to import: {filepath}, error message: {msg}")
             # TODO save error message
             return []
 
     return parse(mod_name, filepath)
 
 
-def _process_modules(mods) -> List[DAG]:
+def _process_modules(mods, show_log: bool = True) -> List[DAG]:
     top_level_dags = (
         (o, m) for m in mods for o in m.__dict__.values() if isinstance(o, DAG)
     )
     found_dags = []
     for dag, mod in top_level_dags:
         try:
             # TODO validate dag params
-            logger.info(f"Found dag {dag} from mod {mod} and model file {mod.__file__}")
+            if show_log:
+                logger.info(
+                    f"Found dag {dag} from mod {mod} and model file {mod.__file__}"
+                )
             found_dags.append(dag)
         except Exception:
             msg = traceback.format_exc()
             logger.error(f"Failed to dag file, error message: {msg}")
     return found_dags
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/awel/flow/__init__.py` & `dbgpt-0.5.7rc0/dbgpt/core/awel/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/awel/flow/base.py` & `dbgpt-0.5.7rc0/dbgpt/core/awel/flow/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/awel/flow/compat.py` & `dbgpt-0.5.7rc0/dbgpt/core/awel/flow/compat.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/awel/flow/exceptions.py` & `dbgpt-0.5.7rc0/dbgpt/core/awel/flow/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/awel/flow/flow_factory.py` & `dbgpt-0.5.7rc0/dbgpt/core/awel/flow/flow_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,21 @@
 
 import logging
 import uuid
 from contextlib import suppress
 from enum import Enum
 from typing import Any, Dict, List, Optional, Tuple, Type, Union, cast
 
+from typing_extensions import Annotated
+
 from dbgpt._private.pydantic import (
     BaseModel,
+    ConfigDict,
     Field,
+    WithJsonSchema,
     field_validator,
     model_to_dict,
     model_validator,
 )
 from dbgpt.core.awel.dag.base import DAG, DAGNode
 
 from .base import (
@@ -251,17 +255,35 @@
             return cls.COMMON
         for category in FlowCategory:
             if category.value == value:
                 return category
         raise ValueError(f"Invalid flow category value: {value}")
 
 
+_DAGModel = Annotated[
+    DAG,
+    WithJsonSchema(
+        {
+            "type": "object",
+            "properties": {
+                "task_name": {"type": "string", "description": "Dummy task name"}
+            },
+            "description": "DAG model, not used in the serialization.",
+        }
+    ),
+]
+
+
 class FlowPanel(BaseModel):
     """Flow panel."""
 
+    model_config = ConfigDict(
+        arbitrary_types_allowed=True, json_encoders={DAG: lambda v: None}
+    )
+
     uid: str = Field(
         default_factory=lambda: str(uuid.uuid4()),
         description="Flow panel uid",
         examples=[
             "5b25ac8a-ba8e-11ee-b96d-3b9bfdeebd1c",
             "6a4752ae-ba8e-11ee-afff-af8fd9bfe727",
         ],
@@ -273,15 +295,16 @@
         ..., description="Flow panel name", examples=["first_awel_flow", "my_llm_flow"]
     )
     flow_category: Optional[FlowCategory] = Field(
         default=FlowCategory.COMMON,
         description="Flow category",
         examples=[FlowCategory.COMMON, FlowCategory.CHAT_AGENT],
     )
-    flow_data: FlowData = Field(..., description="Flow data")
+    flow_data: Optional[FlowData] = Field(None, description="Flow data")
+    flow_dag: Optional[_DAGModel] = Field(None, description="Flow DAG", exclude=True)
     description: Optional[str] = Field(
         None,
         description="Flow panel description",
         examples=["My first AWEL flow"],
     )
     state: State = Field(
         default=State.INITIALIZING, description="Current state of the flow panel"
@@ -301,14 +324,19 @@
         description="Source url of the flow panel",
     )
     version: Optional[str] = Field(
         AWEL_FLOW_VERSION,
         description="Version of the flow panel",
         examples=["0.1.0", "0.2.0"],
     )
+    define_type: Optional[str] = Field(
+        "json",
+        description="Define type of the flow panel",
+        examples=["json", "python"],
+    )
     editable: bool = Field(
         True,
         description="Whether the flow panel is editable",
         examples=[True, False],
     )
     user_name: Optional[str] = Field(None, description="User name")
     sys_code: Optional[str] = Field(None, description="System code")
@@ -340,27 +368,29 @@
             if flow_category:
                 name = str(flow_category) + "_" + name
             values["name"] = name
         return values
 
     def to_dict(self) -> Dict[str, Any]:
         """Convert to dict."""
-        return model_to_dict(self)
+        return model_to_dict(self, exclude={"flow_dag"})
 
 
 class FlowFactory:
     """Flow factory."""
 
     def __init__(self, dag_prefix: str = "flow_dag"):
         """Init the flow factory."""
         self._dag_prefix = dag_prefix
 
     def build(self, flow_panel: FlowPanel) -> DAG:
         """Build the flow."""
-        flow_data = flow_panel.flow_data
+        if not flow_panel.flow_data:
+            raise ValueError("Flow data is required.")
+        flow_data = cast(FlowData, flow_panel.flow_data)
         key_to_operator_nodes: Dict[str, FlowNodeData] = {}
         key_to_resource_nodes: Dict[str, FlowNodeData] = {}
         key_to_resource: Dict[str, ResourceMetadata] = {}
         key_to_downstream: Dict[str, List[Tuple[str, int, int]]] = {}
         key_to_upstream: Dict[str, List[Tuple[str, int, int]]] = {}
         key_to_upstream_node: Dict[str, List[FlowNodeData]] = {}
         for node in flow_data.nodes:
@@ -606,15 +636,18 @@
         """Pre load requirements for the flow panel.
 
         Args:
             flow_panel (FlowPanel): The flow panel
         """
         from dbgpt.util.module_utils import import_from_string
 
-        flow_data = flow_panel.flow_data
+        if not flow_panel.flow_data:
+            return
+
+        flow_data = cast(FlowData, flow_panel.flow_data)
         for node in flow_data.nodes:
             if node.data.is_operator:
                 node_data = cast(ViewMetadata, node.data)
             else:
                 node_data = cast(ResourceMetadata, node.data)
             if not node_data.type_cls:
                 continue
@@ -705,14 +738,16 @@
 
 def fill_flow_panel(flow_panel: FlowPanel):
     """Fill the flow panel with the latest metadata.
 
     Args:
         flow_panel (FlowPanel): The flow panel to fill.
     """
+    if not flow_panel.flow_data:
+        return
     for node in flow_panel.flow_data.nodes:
         try:
             parameters_map = {}
             if node.data.is_operator:
                 data = cast(ViewMetadata, node.data)
                 key = data.get_operator_key()
                 operator_cls: Type[DAGNode] = _get_operator_class(key)
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/awel/operators/base.py` & `dbgpt-0.5.7rc0/dbgpt/core/awel/operators/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Base classes for operators that can be executed within a workflow."""
+
 import asyncio
 import functools
 from abc import ABC, ABCMeta, abstractmethod
 from contextvars import ContextVar
 from types import FunctionType
 from typing import (
     Any,
@@ -261,15 +262,24 @@
             AsyncIterator[OUT]: An asynchronous iterator over the output stream.
         """
         if call_data != EMPTY_DATA:
             call_data = {"data": call_data}
         out_ctx = await self._runner.execute_workflow(
             self, call_data, streaming_call=True, exist_dag_ctx=dag_ctx
         )
-        return out_ctx.current_task_context.task_output.output_stream
+
+        task_output = out_ctx.current_task_context.task_output
+        if task_output.is_stream:
+            return out_ctx.current_task_context.task_output.output_stream
+        else:
+
+            async def _gen():
+                yield task_output.output
+
+            return _gen()
 
     def _blocking_call_stream(
         self,
         call_data: Optional[CALL_DATA] = EMPTY_DATA,
         loop: Optional[asyncio.BaseEventLoop] = None,
     ) -> Iterator[OUT]:
         """Execute the node and return the output as a stream.
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/awel/operators/common_operator.py` & `dbgpt-0.5.7rc0/dbgpt/core/awel/operators/common_operator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Common operators of AWEL."""
+
 import asyncio
 import logging
 from typing import Any, Awaitable, Callable, Dict, Generic, List, Optional, Union
 
 from ..dag.base import DAGContext
 from ..task.base import (
     IN,
@@ -167,14 +168,16 @@
 
     async def map(self, input_value: IN) -> OUT:
         """Map the input data to a new value."""
         raise NotImplementedError
 
 
 BranchFunc = Union[Callable[[IN], bool], Callable[[IN], Awaitable[bool]]]
+# Function that return the task name
+BranchTaskType = Union[str, Callable[[IN], str], Callable[[IN], Awaitable[str]]]
 
 
 class BranchOperator(BaseOperator, Generic[IN, OUT]):
     """Operator node that branches the workflow based on a provided function.
 
     This node filters its input data using a branching function and
     allows for conditional paths in the workflow.
@@ -183,15 +186,15 @@
     otherwise, the corresponding task will be skipped, and the output of
     this skip node will be set to `SKIP_DATA`
 
     """
 
     def __init__(
         self,
-        branches: Optional[Dict[BranchFunc[IN], Union[BaseOperator, str]]] = None,
+        branches: Optional[Dict[BranchFunc[IN], BranchTaskType]] = None,
         **kwargs,
     ):
         """Create a BranchDAGNode with a branching function.
 
         Args:
             branches (Dict[BranchFunc[IN], Union[BaseOperator, str]]):
                 Dict of function that defines the branching condition.
@@ -204,14 +207,18 @@
             for branch_function, value in branches.items():
                 if not callable(branch_function):
                     raise ValueError("branch_function must be callable")
                 if isinstance(value, BaseOperator):
                     if not value.node_name:
                         raise ValueError("branch node name must be set")
                     branches[branch_function] = value.node_name
+                elif callable(value):
+                    raise ValueError(
+                        "BranchTaskType must be str or BaseOperator on init"
+                    )
         self._branches = branches
 
     async def _do_run(self, dag_ctx: DAGContext) -> TaskOutput[OUT]:
         """Run the branching operation on the DAG context's inputs.
 
         This method applies the branching function to the input context to determine
         the path of execution in the workflow.
@@ -230,22 +237,39 @@
             raise ValueError("BranchDAGNode expects single parent")
 
         branches = self._branches
         if not branches:
             branches = await self.branches()
 
         branch_func_tasks = []
-        branch_nodes: List[Union[BaseOperator, str]] = []
+        branch_name_tasks = []
+        # branch_nodes: List[Union[BaseOperator, str]] = []
         for func, node_name in branches.items():
-            branch_nodes.append(node_name)
+            # branch_nodes.append(node_name)
             branch_func_tasks.append(
                 curr_task_ctx.task_input.predicate_map(func, failed_value=None)
             )
+            if callable(node_name):
+
+                async def map_node_name(func) -> str:
+                    input_context = await curr_task_ctx.task_input.map(func)
+                    task_name = input_context.parent_outputs[0].task_output.output
+                    return task_name
+
+                branch_name_tasks.append(map_node_name(node_name))
+
+            else:
+
+                async def _tmp_map_node_name(task_name: str) -> str:
+                    return task_name
+
+                branch_name_tasks.append(_tmp_map_node_name(node_name))
 
         branch_input_ctxs: List[InputContext] = await asyncio.gather(*branch_func_tasks)
+        branch_nodes: List[str] = await asyncio.gather(*branch_name_tasks)
         parent_output = task_input.parent_outputs[0].task_output
         curr_task_ctx.set_task_output(parent_output)
         skip_node_names = []
         for i, ctx in enumerate(branch_input_ctxs):
             node_name = branch_nodes[i]
             branch_out = ctx.parent_outputs[0].task_output
             logger.info(
@@ -254,15 +278,15 @@
             )
             if ctx.parent_outputs[0].task_output.is_none:
                 logger.info(f"Skip node name {node_name}")
                 skip_node_names.append(node_name)
         curr_task_ctx.update_metadata("skip_node_names", skip_node_names)
         return parent_output
 
-    async def branches(self) -> Dict[BranchFunc[IN], Union[BaseOperator, str]]:
+    async def branches(self) -> Dict[BranchFunc[IN], BranchTaskType]:
         """Return branch logic based on input data."""
         raise NotImplementedError
 
 
 class InputOperator(BaseOperator, Generic[OUT]):
     """Operator node that reads data from an input source."""
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/awel/operators/stream_operator.py` & `dbgpt-0.5.7rc0/dbgpt/core/awel/operators/stream_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/awel/runner/job_manager.py` & `dbgpt-0.5.7rc0/dbgpt/core/awel/runner/job_manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/awel/runner/local_runner.py` & `dbgpt-0.5.7rc0/dbgpt/core/awel/runner/local_runner.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/awel/task/base.py` & `dbgpt-0.5.7rc0/dbgpt/core/awel/task/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/awel/task/task_impl.py` & `dbgpt-0.5.7rc0/dbgpt/core/awel/task/task_impl.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/awel/trigger/base.py` & `dbgpt-0.5.7rc0/dbgpt/core/awel/trigger/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/awel/trigger/ext_http_trigger.py` & `dbgpt-0.5.7rc0/dbgpt/core/awel/trigger/ext_http_trigger.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/awel/trigger/http_trigger.py` & `dbgpt-0.5.7rc0/dbgpt/core/awel/trigger/http_trigger.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/awel/trigger/iterator_trigger.py` & `dbgpt-0.5.7rc0/dbgpt/core/awel/trigger/iterator_trigger.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/awel/trigger/trigger_manager.py` & `dbgpt-0.5.7rc0/dbgpt/core/awel/trigger/trigger_manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/awel/util/parameter_util.py` & `dbgpt-0.5.7rc0/dbgpt/core/awel/util/parameter_util.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/interface/cache.py` & `dbgpt-0.5.7rc0/dbgpt/core/interface/cache.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/interface/evaluation.py` & `dbgpt-0.5.7rc0/dbgpt/core/interface/evaluation.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/interface/knowledge.py` & `dbgpt-0.5.7rc0/dbgpt/core/interface/knowledge.py`

 * *Files 22% similar despite different names*

```diff
@@ -107,17 +107,27 @@
         """Transform llama-index to Chunk format."""
         metadata = node.metadata or {}
         return cls(content=node.content, metadata=metadata)
 
     @classmethod
     def chunk2langchain(cls, chunk):
         """Transform Chunk to Langchain format."""
-        from langchain.schema import Document as LCDocument
-
+        try:
+            from langchain.schema import Document as LCDocument  # mypy: ignore
+        except ImportError:
+            raise ValueError(
+                "Could not import python package: langchain "
+                "Please install langchain by command `pip install langchain"
+            )
         return LCDocument(page_content=chunk.content, metadata=chunk.metadata)
 
     @classmethod
     def chunk2llamaindex(cls, chunk):
         """Transform Chunk to llama-index format."""
-        from llama_index.schema import TextNode
-
+        try:
+            from llama_index.schema import TextNode
+        except ImportError:
+            raise ValueError(
+                "Could not import python package: llama_index "
+                "Please install llama_index by command `pip install llama_index"
+            )
         return TextNode(text=chunk.content, metadata=chunk.metadata)
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/interface/llm.py` & `dbgpt-0.5.7rc0/dbgpt/core/interface/llm.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/interface/message.py` & `dbgpt-0.5.7rc0/dbgpt/core/interface/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,24 +294,32 @@
                 f"(Round {message.round_index}) {message.role}: {message.content} "
             )
             str_msg += curr_message.rstrip() + "\n"
 
         return str_msg
 
     @staticmethod
-    def messages_to_string(messages: List["ModelMessage"]) -> str:
+    def messages_to_string(
+        messages: List["ModelMessage"],
+        human_prefix: str = "Human",
+        ai_prefix: str = "AI",
+        system_prefix: str = "System",
+    ) -> str:
         """Convert messages to str.
 
         Args:
             messages (List[ModelMessage]): The messages
+            human_prefix (str): The human prefix
+            ai_prefix (str): The ai prefix
+            system_prefix (str): The system prefix
 
         Returns:
             str: The str messages
         """
-        return _messages_to_str(messages)
+        return _messages_to_str(messages, human_prefix, ai_prefix, system_prefix)
 
 
 _SingleRoundMessage = List[BaseMessage]
 _MultiRoundMessageMapper = Callable[[List[_SingleRoundMessage]], List[BaseMessage]]
 
 
 def _message_to_dict(message: BaseMessage) -> Dict:
@@ -1207,13 +1215,15 @@
             # Already have view message, do nothing
             continue
         if ai_message:
             view_message = ViewMessage(
                 content=ai_message.content,
                 index=ai_message.index,
                 round_index=ai_message.round_index,
-                additional_kwargs=ai_message.additional_kwargs.copy()
-                if ai_message.additional_kwargs
-                else {},
+                additional_kwargs=(
+                    ai_message.additional_kwargs.copy()
+                    if ai_message.additional_kwargs
+                    else {}
+                ),
             )
             current_round.append(view_message)
     return sum(messages_by_round, [])
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/interface/operators/composer_operator.py` & `dbgpt-0.5.7rc0/dbgpt/core/interface/operators/composer_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/interface/operators/llm_operator.py` & `dbgpt-0.5.7rc0/dbgpt/core/interface/operators/llm_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/interface/operators/message_operator.py` & `dbgpt-0.5.7rc0/dbgpt/core/interface/operators/message_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/interface/operators/prompt_operator.py` & `dbgpt-0.5.7rc0/dbgpt/core/interface/operators/prompt_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/interface/operators/retriever.py` & `dbgpt-0.5.7rc0/dbgpt/core/interface/operators/retriever.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/interface/output_parser.py` & `dbgpt-0.5.7rc0/dbgpt/core/interface/output_parser.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/interface/prompt.py` & `dbgpt-0.5.7rc0/dbgpt/core/interface/prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 
 from __future__ import annotations
 
 import dataclasses
 import json
 from abc import ABC, abstractmethod
 from string import Formatter
-from typing import Any, Callable, Dict, List, Optional, Set, Union
+from typing import Any, Callable, Dict, List, Optional, Set, Type, TypeVar, Union
 
 from dbgpt._private.pydantic import BaseModel, ConfigDict, model_validator
 from dbgpt.core.interface.message import BaseMessage, HumanMessage, SystemMessage
 from dbgpt.core.interface.storage import (
     InMemoryStorage,
     QuerySpec,
     ResourceIdentifier,
     StorageInterface,
     StorageItem,
 )
 from dbgpt.util.formatting import formatter, no_strict_formatter
 
+T = TypeVar("T", bound="BasePromptTemplate")
+
 
 def _jinja2_formatter(template: str, **kwargs: Any) -> str:
     """Format a template using jinja2."""
     try:
         from jinja2 import Template
     except ImportError:
         raise ImportError(
@@ -30,17 +32,17 @@
             "Please install it with `pip install jinja2`."
         )
 
     return Template(template).render(**kwargs)
 
 
 _DEFAULT_FORMATTER_MAPPING: Dict[str, Callable] = {
-    "f-string": lambda is_strict: formatter.format
-    if is_strict
-    else no_strict_formatter.format,
+    "f-string": lambda is_strict: (
+        formatter.format if is_strict else no_strict_formatter.format
+    ),
     "jinja2": lambda is_strict: _jinja2_formatter,
 }
 
 
 class BasePromptTemplate(BaseModel):
     """Base class for all prompt templates, returning a prompt."""
 
@@ -84,16 +86,16 @@
             )
         return _DEFAULT_FORMATTER_MAPPING[self.template_format](
             self.template_is_strict
         )(self.template, **kwargs)
 
     @classmethod
     def from_template(
-        cls, template: str, template_format: str = "f-string", **kwargs: Any
-    ) -> BasePromptTemplate:
+        cls: Type[T], template: str, template_format: str = "f-string", **kwargs: Any
+    ) -> T:
         """Create a prompt template from a template string."""
         input_variables = get_template_vars(template, template_format)
         return cls(
             template=template,
             input_variables=input_variables,
             template_format=template_format,
             **kwargs,
@@ -112,22 +114,22 @@
 
     @abstractmethod
     def format_messages(self, **kwargs: Any) -> List[BaseMessage]:
         """Format the prompt with the inputs."""
 
     @classmethod
     def from_template(
-        cls,
+        cls: Type[T],
         template: str,
         template_format: str = "f-string",
         response_format: Optional[str] = None,
         response_key: str = "response",
         template_is_strict: bool = True,
         **kwargs: Any,
-    ) -> BaseChatPromptTemplate:
+    ) -> T:
         """Create a prompt template from a template string."""
         prompt = PromptTemplate.from_template(
             template,
             template_format,
             response_format=response_format,
             response_key=response_key,
             template_is_strict=template_is_strict,
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/interface/serialization.py` & `dbgpt-0.5.7rc0/dbgpt/core/interface/serialization.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/interface/storage.py` & `dbgpt-0.5.7rc0/dbgpt/core/interface/storage.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/operators/__init__.py` & `dbgpt-0.5.7rc0/dbgpt/core/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/operators/flow/composer_operator.py` & `dbgpt-0.5.7rc0/dbgpt/core/operators/flow/composer_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/operators/flow/dict_operator.py` & `dbgpt-0.5.7rc0/dbgpt/core/operators/flow/dict_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/core/schema/api.py` & `dbgpt-0.5.7rc0/dbgpt/core/schema/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,14 +162,31 @@
 
     object: str = Field("list", description="Object type")
     data: List[Dict[str, Any]] = Field(..., description="Data list")
     model: str = Field(..., description="Model name")
     usage: UsageInfo = Field(..., description="Usage info")
 
 
+class RelevanceRequest(BaseModel):
+    """Relevance request entity."""
+
+    model: str = Field(..., description="Rerank model name")
+    query: str = Field(..., description="Query text")
+    documents: List[str] = Field(..., description="Document texts")
+
+
+class RelevanceResponse(BaseModel):
+    """Relevance response entity."""
+
+    object: str = Field("list", description="Object type")
+    model: str = Field(..., description="Rerank model name")
+    data: List[float] = Field(..., description="Data list, relevance scores")
+    usage: UsageInfo = Field(..., description="Usage info")
+
+
 class ModelPermission(BaseModel):
     """Model permission entity."""
 
     id: str = Field(
         default_factory=lambda: f"modelperm-{str(uuid.uuid1())}",
         description="Permission ID",
     )
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/datasource/base.py` & `dbgpt-0.5.7rc0/dbgpt/datasource/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/datasource/conn_spark.py` & `dbgpt-0.5.7rc0/dbgpt/datasource/conn_spark.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/datasource/db_conn_info.py` & `dbgpt-0.5.7rc0/dbgpt/datasource/db_conn_info.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/datasource/manages/connect_config_db.py` & `dbgpt-0.5.7rc0/dbgpt/datasource/manages/connect_config_db.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/datasource/manages/connector_manager.py` & `dbgpt-0.5.7rc0/dbgpt/datasource/manages/connector_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
         from dbgpt.datasource.rdbms.conn_postgresql import (  # noqa: F401
             PostgreSQLConnector,
         )
         from dbgpt.datasource.rdbms.conn_sqlite import SQLiteConnector  # noqa: F401
         from dbgpt.datasource.rdbms.conn_starrocks import (  # noqa: F401
             StarRocksConnector,
         )
+        from dbgpt.datasource.rdbms.conn_vertica import VerticaConnector  # noqa: F401
 
         from .connect_config_db import ConnectConfigEntity  # noqa: F401
 
     def before_start(self):
         """Execute before start."""
         from dbgpt.rag.summary.db_summary_client import DBSummaryClient
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/datasource/operators/datasource_operator.py` & `dbgpt-0.5.7rc0/dbgpt/datasource/operators/datasource_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/base.py` & `dbgpt-0.5.7rc0/dbgpt/datasource/rdbms/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/conn_clickhouse.py` & `dbgpt-0.5.7rc0/dbgpt/datasource/rdbms/conn_clickhouse.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/conn_doris.py` & `dbgpt-0.5.7rc0/dbgpt/datasource/rdbms/conn_doris.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/conn_duckdb.py` & `dbgpt-0.5.7rc0/dbgpt/datasource/rdbms/conn_duckdb.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/conn_hive.py` & `dbgpt-0.5.7rc0/dbgpt/datasource/rdbms/conn_hive.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/conn_mssql.py` & `dbgpt-0.5.7rc0/dbgpt/datasource/rdbms/conn_mssql.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/conn_postgresql.py` & `dbgpt-0.5.7rc0/dbgpt/datasource/rdbms/conn_postgresql.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/conn_sqlite.py` & `dbgpt-0.5.7rc0/dbgpt/datasource/rdbms/conn_sqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """SQLite connector."""
+
 import logging
 import os
 import tempfile
 from typing import Any, Iterable, List, Optional, Tuple
 
 from sqlalchemy import create_engine, text
 
@@ -118,14 +119,26 @@
             )
         )
         table_comments = cursor.fetchall()
         return [
             (table_comment[0], table_comment[1]) for table_comment in table_comments
         ]
 
+    def get_current_db_name(self) -> str:
+        """Get current database name.
+
+        Returns:
+            str: database name
+        """
+        full_path = self._engine.url.database
+        db_name = os.path.basename(full_path)
+        if db_name.endswith(".db"):
+            db_name = db_name[:-3]
+        return db_name
+
     def table_simple_info(self) -> Iterable[str]:
         """Get table simple info."""
         _tables_sql = """
                 SELECT name FROM sqlite_master WHERE type='table'
             """
         cursor = self.session.execute(text(_tables_sql))
         tables_results = cursor.fetchall()
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/conn_starrocks.py` & `dbgpt-0.5.7rc0/dbgpt/datasource/rdbms/conn_starrocks.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/dialect/starrocks/__init__.py` & `dbgpt-0.5.7rc0/dbgpt/datasource/rdbms/dialect/starrocks/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/__init__.py` & `dbgpt-0.5.7rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/datatype.py` & `dbgpt-0.5.7rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/dialect.py` & `dbgpt-0.5.7rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/model/adapter/base.py` & `dbgpt-0.5.7rc0/dbgpt/model/adapter/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -520,19 +520,19 @@
         model_path (str): The path of the model.
         conv_factory (Optional[ConversationAdapterFactory], optional): The conversation factory. Defaults to None.
     Returns:
         Optional[LLMModelAdapter]: The model adapter.
     """
     adapter = None
     # First find adapter by model_name
-    for adapter_entry in model_adapters:
+    for adapter_entry in model_adapters[::-1]:
         if adapter_entry.model_adapter.match(model_type, model_name, None):
             adapter = adapter_entry.model_adapter
             break
-    for adapter_entry in model_adapters:
+    for adapter_entry in model_adapters[::-1]:
         if adapter_entry.model_adapter.match(model_type, None, model_path):
             adapter = adapter_entry.model_adapter
             break
     if adapter:
         new_adapter = adapter.new_adapter()
         new_adapter.model_name = model_name
         new_adapter.model_path = model_path
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/model/adapter/embeddings_loader.py` & `dbgpt-0.5.7rc0/dbgpt/model/adapter/embeddings_loader.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import logging
 from typing import List, Optional, Type, cast
 
 from dbgpt.configs.model_config import get_device
-from dbgpt.core import Embeddings
+from dbgpt.core import Embeddings, RerankEmbeddings
 from dbgpt.model.parameter import (
     BaseEmbeddingModelParameters,
     EmbeddingModelParameters,
     ProxyEmbeddingParameters,
 )
 from dbgpt.util.parameter_utils import EnvArgumentParser, _get_dict_from_obj
 from dbgpt.util.system_utils import get_system_info
@@ -62,14 +62,46 @@
                 return OllamaEmbeddings(**ollama_param)
             else:
                 from dbgpt.rag.embedding import HuggingFaceEmbeddings
 
                 kwargs = param.build_kwargs(model_name=param.model_path)
                 return HuggingFaceEmbeddings(**kwargs)
 
+    def load_rerank_model(
+        self, model_name: str, param: BaseEmbeddingModelParameters
+    ) -> RerankEmbeddings:
+        metadata = {
+            "model_name": model_name,
+            "run_service": SpanTypeRunName.EMBEDDING_MODEL.value,
+            "params": _get_dict_from_obj(param),
+            "sys_infos": _get_dict_from_obj(get_system_info()),
+        }
+        with root_tracer.start_span(
+            "EmbeddingLoader.load_rerank_model",
+            span_type=SpanType.RUN,
+            metadata=metadata,
+        ):
+            if model_name in ["rerank_proxy_http_openapi"]:
+                from dbgpt.rag.embedding.rerank import OpenAPIRerankEmbeddings
+
+                proxy_param = cast(ProxyEmbeddingParameters, param)
+                openapi_param = {}
+                if proxy_param.proxy_server_url:
+                    openapi_param["api_url"] = proxy_param.proxy_server_url
+                if proxy_param.proxy_api_key:
+                    openapi_param["api_key"] = proxy_param.proxy_api_key
+                if proxy_param.proxy_backend:
+                    openapi_param["model_name"] = proxy_param.proxy_backend
+                return OpenAPIRerankEmbeddings(**openapi_param)
+            else:
+                from dbgpt.rag.embedding.rerank import CrossEncoderRerankEmbeddings
+
+                kwargs = param.build_kwargs(model_name=param.model_path)
+                return CrossEncoderRerankEmbeddings(**kwargs)
+
 
 def _parse_embedding_params(
     model_name: Optional[str] = None,
     model_path: Optional[str] = None,
     command_args: List[str] = None,
     param_cls: Optional[Type] = EmbeddingModelParameters,
     **kwargs,
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/model/adapter/fschat_adapter.py` & `dbgpt-0.5.7rc0/dbgpt/model/adapter/fschat_adapter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/model/adapter/hf_adapter.py` & `dbgpt-0.5.7rc0/dbgpt/model/adapter/hf_adapter.py`

 * *Files 23% similar despite different names*

```diff
@@ -131,14 +131,49 @@
         return (
             lower_model_name_or_path
             and "yi-" in lower_model_name_or_path
             and "chat" in lower_model_name_or_path
         )
 
 
+class Yi15Adapter(YiAdapter):
+    """Yi 1.5 model adapter."""
+
+    def do_match(self, lower_model_name_or_path: Optional[str] = None):
+        return (
+            lower_model_name_or_path
+            and "yi-" in lower_model_name_or_path
+            and "1.5" in lower_model_name_or_path
+            and "chat" in lower_model_name_or_path
+        )
+
+    def get_str_prompt(
+        self,
+        params: Dict,
+        messages: List[ModelMessage],
+        tokenizer: Any,
+        prompt_template: str = None,
+        convert_to_compatible_format: bool = False,
+    ) -> Optional[str]:
+        str_prompt = super().get_str_prompt(
+            params,
+            messages,
+            tokenizer,
+            prompt_template,
+            convert_to_compatible_format,
+        )
+        terminators = [
+            tokenizer.eos_token_id,
+        ]
+        exist_token_ids = params.get("stop_token_ids", [])
+        terminators.extend(exist_token_ids)
+        params["stop_token_ids"] = terminators
+        return str_prompt
+
+
 class Mixtral8x7BAdapter(NewHFChatModelAdapter):
     """
     https://huggingface.co/mistralai/Mixtral-8x7B-Instruct-v0.1
     """
 
     support_4bit: bool = True
     support_8bit: bool = True
@@ -331,15 +366,133 @@
         exist_token_ids = params.get("stop_token_ids", [])
         terminators.extend(exist_token_ids)
         # TODO(fangyinc): We should modify the params in the future
         params["stop_token_ids"] = terminators
         return str_prompt
 
 
+class DeepseekV2Adapter(NewHFChatModelAdapter):
+    support_4bit: bool = False
+    support_8bit: bool = False
+
+    def do_match(self, lower_model_name_or_path: Optional[str] = None):
+        return (
+            lower_model_name_or_path
+            and "deepseek" in lower_model_name_or_path
+            and "v2" in lower_model_name_or_path
+            and "chat" in lower_model_name_or_path
+        )
+
+    def load(self, model_path: str, from_pretrained_kwargs: dict):
+        if not from_pretrained_kwargs:
+            from_pretrained_kwargs = {}
+        if "trust_remote_code" not in from_pretrained_kwargs:
+            from_pretrained_kwargs["trust_remote_code"] = True
+        model, tokenizer = super().load(model_path, from_pretrained_kwargs)
+
+        from transformers import GenerationConfig
+
+        model.generation_config = GenerationConfig.from_pretrained(model_path)
+        model.generation_config.pad_token_id = model.generation_config.eos_token_id
+        return model, tokenizer
+
+
+class SailorAdapter(QwenAdapter):
+    """
+    https://huggingface.co/sail/Sailor-14B-Chat
+    """
+
+    def do_match(self, lower_model_name_or_path: Optional[str] = None):
+        return (
+            lower_model_name_or_path
+            and "sailor" in lower_model_name_or_path
+            and "chat" in lower_model_name_or_path
+        )
+
+
+class PhiAdapter(NewHFChatModelAdapter):
+    """
+    https://huggingface.co/microsoft/Phi-3-medium-128k-instruct
+    """
+
+    support_4bit: bool = True
+    support_8bit: bool = True
+    support_system_message: bool = False
+
+    def do_match(self, lower_model_name_or_path: Optional[str] = None):
+        return (
+            lower_model_name_or_path
+            and "phi-3" in lower_model_name_or_path
+            and "instruct" in lower_model_name_or_path
+        )
+
+    def load(self, model_path: str, from_pretrained_kwargs: dict):
+        if not from_pretrained_kwargs:
+            from_pretrained_kwargs = {}
+        if "trust_remote_code" not in from_pretrained_kwargs:
+            from_pretrained_kwargs["trust_remote_code"] = True
+        return super().load(model_path, from_pretrained_kwargs)
+
+    def get_str_prompt(
+        self,
+        params: Dict,
+        messages: List[ModelMessage],
+        tokenizer: Any,
+        prompt_template: str = None,
+        convert_to_compatible_format: bool = False,
+    ) -> Optional[str]:
+        str_prompt = super().get_str_prompt(
+            params,
+            messages,
+            tokenizer,
+            prompt_template,
+            convert_to_compatible_format,
+        )
+        params["custom_stop_words"] = ["<|end|>"]
+        return str_prompt
+
+
+class SQLCoderAdapter(Llama3Adapter):
+    """
+    https://huggingface.co/defog/llama-3-sqlcoder-8b
+    """
+
+    def do_match(self, lower_model_name_or_path: Optional[str] = None):
+        return (
+            lower_model_name_or_path
+            and "llama-3" in lower_model_name_or_path
+            and "sqlcoder" in lower_model_name_or_path
+        )
+
+
+class OpenChatAdapter(Llama3Adapter):
+    """
+    https://huggingface.co/openchat/openchat-3.6-8b-20240522
+    """
+
+    support_4bit: bool = True
+    support_8bit: bool = True
+
+    def do_match(self, lower_model_name_or_path: Optional[str] = None):
+        return (
+            lower_model_name_or_path
+            and "openchat" in lower_model_name_or_path
+            and "3.6" in lower_model_name_or_path
+        )
+
+
+# The following code is used to register the model adapter
+# The last registered model adapter is matched first
 register_model_adapter(YiAdapter)
+register_model_adapter(Yi15Adapter)
 register_model_adapter(Mixtral8x7BAdapter)
 register_model_adapter(SOLARAdapter)
 register_model_adapter(GemmaAdapter)
 register_model_adapter(StarlingLMAdapter)
 register_model_adapter(QwenAdapter)
 register_model_adapter(QwenMoeAdapter)
 register_model_adapter(Llama3Adapter)
+register_model_adapter(DeepseekV2Adapter)
+register_model_adapter(SailorAdapter)
+register_model_adapter(PhiAdapter)
+register_model_adapter(SQLCoderAdapter)
+register_model_adapter(OpenChatAdapter)
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/model/adapter/loader.py` & `dbgpt-0.5.7rc0/dbgpt/model/adapter/loader.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/model/adapter/model_adapter.py` & `dbgpt-0.5.7rc0/dbgpt/model/adapter/model_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,19 +143,18 @@
 
     pre_args = _SimpleArgParser("model_name", "model_path", "worker_type", "model_type")
     pre_args.parse()
     model_name = pre_args.get("model_name")
     model_path = pre_args.get("model_path")
     worker_type = pre_args.get("worker_type")
     model_type = pre_args.get("model_type")
-    if model_name is None and model_type != ModelType.VLLM:
-        return None
     if worker_type == WorkerType.TEXT2VEC:
         return [
             EMBEDDING_NAME_TO_PARAMETER_CLASS_CONFIG.get(
                 model_name, EmbeddingModelParameters
             )
         ]
-
+    if model_name is None and model_type != ModelType.VLLM:
+        return None
     llm_adapter = get_llm_model_adapter(model_name, model_path, model_type=model_type)
     param_class = llm_adapter.model_param_class()
     return [param_class]
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/model/adapter/old_adapter.py` & `dbgpt-0.5.7rc0/dbgpt/model/adapter/old_adapter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/model/adapter/proxy_adapter.py` & `dbgpt-0.5.7rc0/dbgpt/model/adapter/proxy_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -290,18 +290,44 @@
 
     def get_async_generate_stream_function(self, model, model_path: str):
         from dbgpt.model.proxy.llms.moonshot import moonshot_generate_stream
 
         return moonshot_generate_stream
 
 
+class DeepseekProxyLLMModelAdapter(ProxyLLMModelAdapter):
+    """Deepseek proxy LLM model adapter.
+
+    See Also: `Deepseek Documentation <https://platform.deepseek.com/api-docs/>`_
+    """
+
+    def support_async(self) -> bool:
+        return True
+
+    def do_match(self, lower_model_name_or_path: Optional[str] = None):
+        return lower_model_name_or_path == "deepseek_proxyllm"
+
+    def get_llm_client_class(
+        self, params: ProxyModelParameters
+    ) -> Type[ProxyLLMClient]:
+        from dbgpt.model.proxy.llms.deepseek import DeepseekLLMClient
+
+        return DeepseekLLMClient
+
+    def get_async_generate_stream_function(self, model, model_path: str):
+        from dbgpt.model.proxy.llms.deepseek import deepseek_generate_stream
+
+        return deepseek_generate_stream
+
+
 register_model_adapter(OpenAIProxyLLMModelAdapter)
 register_model_adapter(TongyiProxyLLMModelAdapter)
 register_model_adapter(OllamaLLMModelAdapter)
 register_model_adapter(ZhipuProxyLLMModelAdapter)
 register_model_adapter(WenxinProxyLLMModelAdapter)
 register_model_adapter(GeminiProxyLLMModelAdapter)
 register_model_adapter(SparkProxyLLMModelAdapter)
 register_model_adapter(BardProxyLLMModelAdapter)
 register_model_adapter(BaichuanProxyLLMModelAdapter)
 register_model_adapter(YiProxyLLMModelAdapter)
 register_model_adapter(MoonshotProxyLLMModelAdapter)
+register_model_adapter(DeepseekProxyLLMModelAdapter)
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/model/adapter/template.py` & `dbgpt-0.5.7rc0/dbgpt/model/adapter/template.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/model/adapter/vllm_adapter.py` & `dbgpt-0.5.7rc0/dbgpt/model/adapter/vllm_adapter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/model/base.py` & `dbgpt-0.5.7rc0/dbgpt/model/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/model/cli.py` & `dbgpt-0.5.7rc0/dbgpt/model/cli.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/model/operators/llm_operator.py` & `dbgpt-0.5.7rc0/dbgpt/model/operators/llm_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/model/parameter.py` & `dbgpt-0.5.7rc0/dbgpt/model/parameter.py`

 * *Files 2% similar despite different names*

```diff
@@ -251,14 +251,18 @@
 
 
 @dataclass
 class BaseEmbeddingModelParameters(BaseModelParameters):
     def build_kwargs(self, **kwargs) -> Dict:
         pass
 
+    def is_rerank_model(self) -> bool:
+        """Check if the model is a rerank model"""
+        return False
+
 
 @dataclass
 class EmbeddingModelParameters(BaseEmbeddingModelParameters):
     device: Optional[str] = field(
         default=None,
         metadata={
             "help": "Device to run model. If None, the device is automatically determined"
@@ -268,26 +272,45 @@
     normalize_embeddings: Optional[bool] = field(
         default=None,
         metadata={
             "help": "Determines whether the model's embeddings should be normalized."
         },
     )
 
+    rerank: Optional[bool] = field(
+        default=False, metadata={"help": "Whether the model is a rerank model"}
+    )
+
+    max_length: Optional[int] = field(
+        default=None,
+        metadata={
+            "help": "Max length for input sequences. Longer sequences will be "
+            "truncated. If None, max length of the model will be used, just for rerank"
+            " model now."
+        },
+    )
+
     def build_kwargs(self, **kwargs) -> Dict:
         model_kwargs, encode_kwargs = None, None
         if self.device:
             model_kwargs = {"device": self.device}
         if self.normalize_embeddings:
             encode_kwargs = {"normalize_embeddings": self.normalize_embeddings}
         if model_kwargs:
             kwargs["model_kwargs"] = model_kwargs
+        if self.is_rerank_model():
+            kwargs["max_length"] = self.max_length
         if encode_kwargs:
             kwargs["encode_kwargs"] = encode_kwargs
         return kwargs
 
+    def is_rerank_model(self) -> bool:
+        """Check if the model is a rerank model"""
+        return self.rerank
+
 
 @dataclass
 class ModelParameters(BaseModelParameters):
     device: Optional[str] = field(
         default=None,
         metadata={
             "help": "Device to run model. If None, the device is automatically determined"
@@ -533,34 +556,43 @@
     )
 
     proxy_deployment: Optional[str] = field(
         default="text-embedding-ada-002",
         metadata={"help": "Tto support Azure OpenAI Service custom deployment names"},
     )
 
+    rerank: Optional[bool] = field(
+        default=False, metadata={"help": "Whether the model is a rerank model"}
+    )
+
     def build_kwargs(self, **kwargs) -> Dict:
         params = {
             "openai_api_base": self.proxy_server_url,
             "openai_api_key": self.proxy_api_key,
             "openai_api_type": self.proxy_api_type if self.proxy_api_type else None,
-            "openai_api_version": self.proxy_api_version
-            if self.proxy_api_version
-            else None,
+            "openai_api_version": (
+                self.proxy_api_version if self.proxy_api_version else None
+            ),
             "model": self.proxy_backend,
-            "deployment": self.proxy_deployment
-            if self.proxy_deployment
-            else self.proxy_backend,
+            "deployment": (
+                self.proxy_deployment if self.proxy_deployment else self.proxy_backend
+            ),
         }
         for k, v in kwargs:
             params[k] = v
         return params
 
+    def is_rerank_model(self) -> bool:
+        """Check if the model is a rerank model"""
+        return self.rerank
+
 
 _EMBEDDING_PARAMETER_CLASS_TO_NAME_CONFIG = {
-    ProxyEmbeddingParameters: "proxy_openai,proxy_azure,proxy_http_openapi,proxy_ollama",
+    ProxyEmbeddingParameters: "proxy_openai,proxy_azure,proxy_http_openapi,"
+    "proxy_ollama,rerank_proxy_http_openapi",
 }
 
 EMBEDDING_NAME_TO_PARAMETER_CLASS_CONFIG = {}
 
 
 def _update_embedding_config():
     global EMBEDDING_NAME_TO_PARAMETER_CLASS_CONFIG
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/model/proxy/__init__.py` & `dbgpt-0.5.7rc0/dbgpt/model/proxy/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
         "SparkLLMClient": "dbgpt.model.proxy.llms.spark",
         "TongyiLLMClient": "dbgpt.model.proxy.llms.tongyi",
         "WenxinLLMClient": "dbgpt.model.proxy.llms.wenxin",
         "ZhipuLLMClient": "dbgpt.model.proxy.llms.zhipu",
         "YiLLMClient": "dbgpt.model.proxy.llms.yi",
         "MoonshotLLMClient": "dbgpt.model.proxy.llms.moonshot",
         "OllamaLLMClient": "dbgpt.model.proxy.llms.ollama",
+        "DeepseekLLMClient": "dbgpt.model.proxy.llms.deepseek",
     }
 
     if name in module_path:
         module = __import__(module_path[name], fromlist=[name])
         return getattr(module, name)
     else:
         raise AttributeError(f"module {__name__} has no attribute {name}")
@@ -31,8 +32,9 @@
     "TongyiLLMClient",
     "ZhipuLLMClient",
     "WenxinLLMClient",
     "SparkLLMClient",
     "YiLLMClient",
     "MoonshotLLMClient",
     "OllamaLLMClient",
+    "DeepseekLLMClient",
 ]
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/model/proxy/base.py` & `dbgpt-0.5.7rc0/dbgpt/model/proxy/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/baichuan.py` & `dbgpt-0.5.7rc0/dbgpt/model/proxy/llms/baichuan.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/bard.py` & `dbgpt-0.5.7rc0/dbgpt/model/proxy/llms/bard.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/chatgpt.py` & `dbgpt-0.5.7rc0/dbgpt/model/proxy/llms/chatgpt.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/gemini.py` & `dbgpt-0.5.7rc0/dbgpt/model/proxy/llms/gemini.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/moonshot.py` & `dbgpt-0.5.7rc0/dbgpt/model/proxy/llms/moonshot.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/ollama.py` & `dbgpt-0.5.7rc0/dbgpt/model/proxy/llms/ollama.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/proxy_model.py` & `dbgpt-0.5.7rc0/dbgpt/model/proxy/llms/proxy_model.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/spark.py` & `dbgpt-0.5.7rc0/dbgpt/model/proxy/llms/spark.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/tongyi.py` & `dbgpt-0.5.7rc0/dbgpt/model/proxy/llms/tongyi.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/wenxin.py` & `dbgpt-0.5.7rc0/dbgpt/model/proxy/llms/wenxin.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/yi.py` & `dbgpt-0.5.7rc0/dbgpt/model/proxy/llms/yi.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/zhipu.py` & `dbgpt-0.5.7rc0/dbgpt/model/proxy/llms/zhipu.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/model/utils/chatgpt_utils.py` & `dbgpt-0.5.7rc0/dbgpt/model/utils/chatgpt_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/model/utils/llm_utils.py` & `dbgpt-0.5.7rc0/dbgpt/model/utils/llm_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/model/utils/token_utils.py` & `dbgpt-0.5.7rc0/dbgpt/model/utils/token_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/assembler/base.py` & `dbgpt-0.5.7rc0/dbgpt/rag/assembler/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Base Assembler."""
+
 from abc import ABC, abstractmethod
 from typing import Any, List, Optional
 
 from dbgpt.core import Chunk
 from dbgpt.util.tracer import root_tracer
 
 from ..chunk_manager import ChunkManager, ChunkParameters
@@ -33,21 +34,23 @@
         self._chunk_parameters = chunk_parameters or ChunkParameters()
         self._extractor = extractor
         self._chunk_manager = ChunkManager(
             knowledge=self._knowledge, chunk_parameter=self._chunk_parameters
         )
         self._chunks: List[Chunk] = []
         metadata = {
-            "knowledge_cls": self._knowledge.__class__.__name__
-            if self._knowledge
-            else None,
+            "knowledge_cls": (
+                self._knowledge.__class__.__name__ if self._knowledge else None
+            ),
             "knowledge_type": self._knowledge.type().value if self._knowledge else None,
-            "path": self._knowledge._path
-            if self._knowledge and hasattr(self._knowledge, "_path")
-            else None,
+            "path": (
+                self._knowledge._path
+                if self._knowledge and hasattr(self._knowledge, "_path")
+                else None
+            ),
             "chunk_parameters": self._chunk_parameters.dict(),
         }
         with root_tracer.start_span("BaseAssembler.load_knowledge", metadata=metadata):
             self.load_knowledge(self._knowledge)
 
     def load_knowledge(self, knowledge: Optional[Knowledge] = None) -> None:
         """Load knowledge Pipeline."""
@@ -66,10 +69,18 @@
     def persist(self) -> List[str]:
         """Persist chunks.
 
         Returns:
             List[str]: List of persisted chunk ids.
         """
 
+    async def apersist(self) -> List[str]:
+        """Persist chunks.
+
+        Returns:
+            List[str]: List of persisted chunk ids.
+        """
+        raise NotImplementedError
+
     def get_chunks(self) -> List[Chunk]:
         """Return chunks."""
         return self._chunks
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/assembler/db_schema.py` & `dbgpt-0.5.7rc0/dbgpt/rag/assembler/db_schema.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/assembler/embedding.py` & `dbgpt-0.5.7rc0/dbgpt/rag/assembler/embedding.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Embedding Assembler."""
+from concurrent.futures import ThreadPoolExecutor
 from typing import Any, List, Optional
 
 from dbgpt.core import Chunk, Embeddings
 from dbgpt.storage.vector_store.connector import VectorStoreConnector
 
+from ...util.executor_utils import blocking_func_to_async
 from ..assembler.base import BaseAssembler
 from ..chunk_manager import ChunkParameters
 from ..embedding.embedding_factory import DefaultEmbeddingFactory
 from ..knowledge.base import Knowledge
 from ..retriever.embedding import EmbeddingRetriever
 
 
@@ -94,22 +96,65 @@
             knowledge=knowledge,
             vector_store_connector=vector_store_connector,
             chunk_parameters=chunk_parameters,
             embedding_model=embedding_model,
             embeddings=embeddings,
         )
 
+    @classmethod
+    async def aload_from_knowledge(
+        cls,
+        knowledge: Knowledge,
+        vector_store_connector: VectorStoreConnector,
+        chunk_parameters: Optional[ChunkParameters] = None,
+        embedding_model: Optional[str] = None,
+        embeddings: Optional[Embeddings] = None,
+        executor: Optional[ThreadPoolExecutor] = None,
+    ) -> "EmbeddingAssembler":
+        """Load document embedding into vector store from path.
+
+        Args:
+            knowledge: (Knowledge) Knowledge datasource.
+            vector_store_connector: (VectorStoreConnector) VectorStoreConnector to use.
+            chunk_parameters: (Optional[ChunkParameters]) ChunkManager to use for
+                chunking.
+            embedding_model: (Optional[str]) Embedding model to use.
+            embeddings: (Optional[Embeddings]) Embeddings to use.
+            executor: (Optional[ThreadPoolExecutor) ThreadPoolExecutor to use.
+
+        Returns:
+             EmbeddingAssembler
+        """
+        executor = executor or ThreadPoolExecutor()
+        return await blocking_func_to_async(
+            executor,
+            cls,
+            knowledge,
+            vector_store_connector,
+            chunk_parameters,
+            embedding_model,
+            embeddings,
+        )
+
     def persist(self) -> List[str]:
         """Persist chunks into vector store.
 
         Returns:
             List[str]: List of chunk ids.
         """
         return self._vector_store_connector.load_document(self._chunks)
 
+    async def apersist(self) -> List[str]:
+        """Persist chunks into store.
+
+        Returns:
+            List[str]: List of chunk ids.
+        """
+        return await self._vector_store_connector.aload_document(self._chunks)
+
     def _extract_info(self, chunks) -> List[Chunk]:
         """Extract info from chunks."""
         return []
 
     def as_retriever(self, top_k: int = 4, **kwargs) -> EmbeddingRetriever:
         """Create a retriever.
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/assembler/summary.py` & `dbgpt-0.5.7rc0/dbgpt/rag/assembler/summary.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/chunk_manager.py` & `dbgpt-0.5.7rc0/dbgpt/rag/chunk_manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/embedding/_wrapped.py` & `dbgpt-0.5.7rc0/dbgpt/rag/embedding/_wrapped.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Wraps the third-party language model embeddings to the common interface."""
 
 from typing import TYPE_CHECKING, List
 
 from dbgpt.core import Embeddings
 
 if TYPE_CHECKING:
-    from langchain.embeddings.base import Embeddings as LangChainEmbeddings
+    from langchain.embeddings.base import (
+        Embeddings as LangChainEmbeddings,  # mypy: ignore
+    )
 
 
 class WrappedEmbeddings(Embeddings):
     """Wraps the third-party language model embeddings to the common interface."""
 
     def __init__(self, embeddings: "LangChainEmbeddings") -> None:
         """Create a new WrappedEmbeddings."""
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/embedding/embedding_factory.py` & `dbgpt-0.5.7rc0/dbgpt/rag/embedding/embedding_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 import os
 from abc import ABC, abstractmethod
 from typing import Any, List, Optional, Type
 
 from dbgpt.component import BaseComponent, SystemApp
-from dbgpt.core import Embeddings
+from dbgpt.core import Embeddings, RerankEmbeddings
 from dbgpt.core.awel import DAGVar
 from dbgpt.core.awel.flow import ResourceCategory, register_resource
 from dbgpt.util.i18n_utils import _
 
 logger = logging.getLogger(__name__)
 
 
@@ -30,14 +30,34 @@
             embedding_cls (Type): The embedding class.
 
         Returns:
             Embeddings: The embedding instance.
         """
 
 
+class RerankEmbeddingFactory(BaseComponent, ABC):
+    """Class for RerankEmbeddingFactory."""
+
+    name = "rerank_embedding_factory"
+
+    @abstractmethod
+    def create(
+        self, model_name: Optional[str] = None, embedding_cls: Optional[Type] = None
+    ) -> RerankEmbeddings:
+        """Create an embedding instance.
+
+        Args:
+            model_name (str): The model name.
+            embedding_cls (Type): The embedding class.
+
+        Returns:
+            RerankEmbeddings: The embedding instance.
+        """
+
+
 class DefaultEmbeddingFactory(EmbeddingFactory):
     """The default embedding factory."""
 
     def __init__(
         self,
         system_app: Optional[SystemApp] = None,
         default_model_name: Optional[str] = None,
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/embedding/embeddings.py` & `dbgpt-0.5.7rc0/dbgpt/rag/embedding/embeddings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Embedding implementations."""
 
-
 from typing import Any, Dict, List, Optional
 
 import aiohttp
 import requests
 
 from dbgpt._private.pydantic import EXTRA_FORBID, BaseModel, ConfigDict, Field
 from dbgpt.core import Embeddings
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/evaluation/retriever.py` & `dbgpt-0.5.7rc0/dbgpt/rag/evaluation/retriever.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/extractor/base.py` & `dbgpt-0.5.7rc0/dbgpt/rag/extractor/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/extractor/summary.py` & `dbgpt-0.5.7rc0/dbgpt/rag/extractor/summary.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/knowledge/__init__.py` & `dbgpt-0.5.7rc0/dbgpt/rag/knowledge/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         "HTMLKnowledge": "html",
         "MarkdownKnowledge": "markdown",
         "PDFKnowledge": "pdf",
         "PPTXKnowledge": "pptx",
         "StringKnowledge": "string",
         "TXTKnowledge": "txt",
         "URLKnowledge": "url",
+        "ExcelKnowledge": "xlsx",
     }
 
     if name in _LIBS:
         module_path = "." + _LIBS[name]
         module = importlib.import_module(module_path, __name__)
         attr = getattr(module, name)
         _MODULE_CACHE[name] = attr
@@ -49,8 +50,9 @@
     "HTMLKnowledge",
     "MarkdownKnowledge",
     "PDFKnowledge",
     "PPTXKnowledge",
     "StringKnowledge",
     "TXTKnowledge",
     "URLKnowledge",
+    "ExcelKnowledge",
 ]
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/knowledge/base.py` & `dbgpt-0.5.7rc0/dbgpt/rag/knowledge/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     CSV = "csv"
     MARKDOWN = "md"
     PPTX = "pptx"
     DOCX = "docx"
     TXT = "txt"
     HTML = "html"
     DATASOURCE = "datasource"
+    EXCEL = "xlsx"
 
 
 class KnowledgeType(Enum):
     """Knowledge Type Enum."""
 
     DOCUMENT = "DOCUMENT"
     URL = "URL"
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/knowledge/csv.py` & `dbgpt-0.5.7rc0/dbgpt/rag/knowledge/csv.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/knowledge/datasource.py` & `dbgpt-0.5.7rc0/dbgpt/rag/knowledge/datasource.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/knowledge/docx.py` & `dbgpt-0.5.7rc0/dbgpt/rag/knowledge/docx.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/knowledge/factory.py` & `dbgpt-0.5.7rc0/dbgpt/rag/knowledge/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,14 +166,15 @@
     @staticmethod
     def _get_knowledge_subclasses() -> List["Type[Knowledge]"]:
         """Get all knowledge subclasses."""
         from dbgpt.rag.knowledge.base import Knowledge  # noqa: F401
         from dbgpt.rag.knowledge.csv import CSVKnowledge  # noqa: F401
         from dbgpt.rag.knowledge.datasource import DatasourceKnowledge  # noqa: F401
         from dbgpt.rag.knowledge.docx import DocxKnowledge  # noqa: F401
+        from dbgpt.rag.knowledge.excel import ExcelKnowledge  # noqa: F401
         from dbgpt.rag.knowledge.html import HTMLKnowledge  # noqa: F401
         from dbgpt.rag.knowledge.markdown import MarkdownKnowledge  # noqa: F401
         from dbgpt.rag.knowledge.pdf import PDFKnowledge  # noqa: F401
         from dbgpt.rag.knowledge.pptx import PPTXKnowledge  # noqa: F401
         from dbgpt.rag.knowledge.string import StringKnowledge  # noqa: F401
         from dbgpt.rag.knowledge.txt import TXTKnowledge  # noqa: F401
         from dbgpt.rag.knowledge.url import URLKnowledge  # noqa: F401
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/knowledge/html.py` & `dbgpt-0.5.7rc0/dbgpt/rag/knowledge/html.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/knowledge/markdown.py` & `dbgpt-0.5.7rc0/dbgpt/rag/knowledge/markdown.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/knowledge/pdf.py` & `dbgpt-0.5.7rc0/dbgpt/rag/knowledge/pdf.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/knowledge/pptx.py` & `dbgpt-0.5.7rc0/dbgpt/rag/knowledge/pptx.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/knowledge/string.py` & `dbgpt-0.5.7rc0/dbgpt/rag/knowledge/string.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/knowledge/txt.py` & `dbgpt-0.5.7rc0/dbgpt/rag/knowledge/txt.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/knowledge/url.py` & `dbgpt-0.5.7rc0/dbgpt/rag/knowledge/url.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         self._source_column = source_column
 
     def _load(self) -> List[Document]:
         """Fetch URL document from loader."""
         if self._loader:
             documents = self._loader.load()
         else:
-            from langchain.document_loaders import WebBaseLoader
+            from langchain.document_loaders import WebBaseLoader  # mypy: ignore
 
             if self._path is not None:
                 web_reader = WebBaseLoader(web_path=self._path)
                 documents = web_reader.load()
             else:
                 # Handle the case where self._path is None
                 raise ValueError("web_path cannot be None")
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/operators/__init__.py` & `dbgpt-0.5.7rc0/dbgpt/rag/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/operators/assembler.py` & `dbgpt-0.5.7rc0/dbgpt/rag/operators/assembler.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/operators/datasource.py` & `dbgpt-0.5.7rc0/dbgpt/rag/operators/datasource.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/operators/db_schema.py` & `dbgpt-0.5.7rc0/dbgpt/rag/operators/db_schema.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/operators/embedding.py` & `dbgpt-0.5.7rc0/dbgpt/rag/operators/embedding.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/operators/evaluation.py` & `dbgpt-0.5.7rc0/dbgpt/rag/operators/evaluation.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/operators/knowledge.py` & `dbgpt-0.5.7rc0/dbgpt/rag/operators/knowledge.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/operators/rerank.py` & `dbgpt-0.5.7rc0/dbgpt/rag/operators/rerank.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/operators/rewrite.py` & `dbgpt-0.5.7rc0/dbgpt/rag/operators/rewrite.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/operators/schema_linking.py` & `dbgpt-0.5.7rc0/dbgpt/rag/operators/schema_linking.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/operators/summary.py` & `dbgpt-0.5.7rc0/dbgpt/rag/operators/summary.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/retriever/base.py` & `dbgpt-0.5.7rc0/dbgpt/rag/retriever/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/retriever/db_schema.py` & `dbgpt-0.5.7rc0/dbgpt/rag/retriever/db_schema.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/retriever/embedding.py` & `dbgpt-0.5.7rc0/dbgpt/rag/retriever/embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Embedding retriever."""
+
 from functools import reduce
 from typing import Any, Dict, List, Optional, cast
 
 from dbgpt.core import Chunk
 from dbgpt.rag.retriever.base import BaseRetriever
 from dbgpt.rag.retriever.rerank import DefaultRanker, Ranker
 from dbgpt.rag.retriever.rewrite import QueryRewrite
@@ -116,15 +117,15 @@
                 query, self._top_k, score_threshold, filters
             )
             for query in queries
         ]
         new_candidates_with_score = cast(
             List[Chunk], reduce(lambda x, y: x + y, candidates_with_score)
         )
-        new_candidates_with_score = self._rerank.rank(new_candidates_with_score)
+        new_candidates_with_score = self._rerank.rank(new_candidates_with_score, query)
         return new_candidates_with_score
 
     async def _aretrieve(
         self, query: str, filters: Optional[MetadataFilters] = None
     ) -> List[Chunk]:
         """Retrieve knowledge chunks.
 
@@ -203,15 +204,17 @@
             "EmbeddingRetriever.rerank",
             metadata={
                 "query": query,
                 "score_threshold": score_threshold,
                 "rerank_cls": self._rerank.__class__.__name__,
             },
         ):
-            new_candidates_with_score = self._rerank.rank(new_candidates_with_score)
+            new_candidates_with_score = await self._rerank.arank(
+                new_candidates_with_score, query
+            )
             return new_candidates_with_score
 
     async def _similarity_search(
         self, query, filters: Optional[MetadataFilters] = None
     ) -> List[Chunk]:
         """Similar search."""
         return self._vector_store_connector.similar_search(query, self._top_k, filters)
@@ -222,10 +225,10 @@
         candidates = reduce(lambda x, y: x + y, candidates)
         return cast(List[Chunk], candidates)
 
     async def _similarity_search_with_score(
         self, query, score_threshold, filters: Optional[MetadataFilters] = None
     ) -> List[Chunk]:
         """Similar search with score."""
-        return self._vector_store_connector.similar_search_with_scores(
+        return await self._vector_store_connector.asimilar_search_with_scores(
             query, self._top_k, score_threshold, filters
         )
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/retriever/rewrite.py` & `dbgpt-0.5.7rc0/dbgpt/rag/retriever/rewrite.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/retriever/time_weighted.py` & `dbgpt-0.5.7rc0/dbgpt/rag/retriever/time_weighted.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/schemalinker/base_linker.py` & `dbgpt-0.5.7rc0/dbgpt/rag/schemalinker/base_linker.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/schemalinker/schema_linking.py` & `dbgpt-0.5.7rc0/dbgpt/rag/schemalinker/schema_linking.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/summary/db_summary.py` & `dbgpt-0.5.7rc0/dbgpt/rag/summary/db_summary.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/summary/db_summary_client.py` & `dbgpt-0.5.7rc0/dbgpt/rag/summary/db_summary_client.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/summary/gdbms_db_summary.py` & `dbgpt-0.5.7rc0/dbgpt/rag/summary/gdbms_db_summary.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/summary/rdbms_db_summary.py` & `dbgpt-0.5.7rc0/dbgpt/rag/summary/rdbms_db_summary.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/text_splitter/__init__.py` & `dbgpt-0.5.7rc0/dbgpt/rag/text_splitter/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/text_splitter/pre_text_splitter.py` & `dbgpt-0.5.7rc0/dbgpt/rag/text_splitter/pre_text_splitter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/text_splitter/text_splitter.py` & `dbgpt-0.5.7rc0/dbgpt/rag/text_splitter/text_splitter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/rag/text_splitter/token_splitter.py` & `dbgpt-0.5.7rc0/dbgpt/rag/text_splitter/token_splitter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/storage/cache/llm_cache.py` & `dbgpt-0.5.7rc0/dbgpt/storage/cache/llm_cache.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/storage/cache/manager.py` & `dbgpt-0.5.7rc0/dbgpt/storage/cache/manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/storage/cache/operators.py` & `dbgpt-0.5.7rc0/dbgpt/storage/cache/operators.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/storage/cache/storage/base.py` & `dbgpt-0.5.7rc0/dbgpt/storage/cache/storage/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/storage/cache/storage/disk/disk_storage.py` & `dbgpt-0.5.7rc0/dbgpt/storage/cache/storage/disk/disk_storage.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/storage/chat_history/chat_history_db.py` & `dbgpt-0.5.7rc0/dbgpt/storage/chat_history/chat_history_db.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/storage/chat_history/storage_adapter.py` & `dbgpt-0.5.7rc0/dbgpt/storage/chat_history/storage_adapter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/storage/metadata/_base_dao.py` & `dbgpt-0.5.7rc0/dbgpt/storage/metadata/_base_dao.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/storage/metadata/db_factory.py` & `dbgpt-0.5.7rc0/dbgpt/storage/metadata/db_factory.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/storage/metadata/db_manager.py` & `dbgpt-0.5.7rc0/dbgpt/storage/metadata/db_manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/storage/metadata/db_storage.py` & `dbgpt-0.5.7rc0/dbgpt/storage/metadata/db_storage.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/storage/schema.py` & `dbgpt-0.5.7rc0/dbgpt/storage/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     Mysql = DbInfo("mysql")
     OCeanBase = DbInfo("oceanbase")
     DuckDb = DbInfo("duckdb", True)
     SQLite = DbInfo("sqlite", True)
     Oracle = DbInfo("oracle")
     MSSQL = DbInfo("mssql")
     Postgresql = DbInfo("postgresql")
+    Vertica = DbInfo("vertica")
     Clickhouse = DbInfo("clickhouse")
     StarRocks = DbInfo("starrocks")
     Spark = DbInfo("spark", True)
     Doris = DbInfo("doris")
     Hive = DbInfo("hive")
     TuGraph = DbInfo("tugraph")
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/storage/vector_store/base.py` & `dbgpt-0.5.7rc0/dbgpt/storage/vector_store/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """Vector store base class."""
 import logging
 import math
-import time
 from abc import ABC, abstractmethod
 from concurrent.futures import ThreadPoolExecutor
-from typing import Any, Dict, List, Optional
+from typing import Any, List, Optional
 
-from dbgpt._private.pydantic import BaseModel, ConfigDict, Field, model_to_dict
+from dbgpt._private.pydantic import ConfigDict, Field
 from dbgpt.core import Chunk, Embeddings
 from dbgpt.core.awel.flow import Parameter
+from dbgpt.rag.index.base import IndexStoreBase, IndexStoreConfig
 from dbgpt.storage.vector_store.filters import MetadataFilters
+from dbgpt.util.executor_utils import blocking_func_to_async
 from dbgpt.util.i18n_utils import _
 
 logger = logging.getLogger(__name__)
 
-
 _COMMON_PARAMETERS = [
     Parameter.build_from(
         _("Collection Name"),
         "name",
         str,
         description=_(
-            "The name of vector store, if not set, will use the default " "name."
+            "The name of vector store, if not set, will use the default name."
         ),
         optional=True,
         default="dbgpt_collection",
     ),
     Parameter.build_from(
         _("User"),
         "user",
         str,
         description=_(
-            "The user of vector store, if not set, will use the default " "user."
+            "The user of vector store, if not set, will use the default user."
         ),
         optional=True,
         default=None,
     ),
     Parameter.build_from(
         _("Password"),
         "password",
@@ -80,164 +80,73 @@
         ),
         optional=True,
         default=1,
     ),
 ]
 
 
-class VectorStoreConfig(BaseModel):
+class VectorStoreConfig(IndexStoreConfig):
     """Vector store config."""
 
-    model_config = ConfigDict(arbitrary_types_allowed=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, extra="allow")
 
-    name: str = Field(
-        default="dbgpt_collection",
-        description="The name of vector store, if not set, will use the default name.",
-    )
     user: Optional[str] = Field(
         default=None,
         description="The user of vector store, if not set, will use the default user.",
     )
     password: Optional[str] = Field(
         default=None,
-        description="The password of vector store, if not set, will use the default "
-        "password.",
-    )
-    embedding_fn: Optional[Embeddings] = Field(
-        default=None,
-        description="The embedding function of vector store, if not set, will use the "
-        "default embedding function.",
-    )
-    max_chunks_once_load: int = Field(
-        default=10,
-        description="The max number of chunks to load at once. If your document is "
-        "large, you can set this value to a larger number to speed up the loading "
-        "process. Default is 10.",
-    )
-    max_threads: int = Field(
-        default=1,
-        description="The max number of threads to use. Default is 1. If you set this "
-        "bigger than 1, please make sure your vector store is thread-safe.",
+        description=(
+            "The password of vector store, if not set, will use the default password."
+        ),
     )
 
-    def to_dict(self, **kwargs) -> Dict[str, Any]:
-        """Convert to dict."""
-        return model_to_dict(self, **kwargs)
 
-
-class VectorStoreBase(ABC):
+class VectorStoreBase(IndexStoreBase, ABC):
     """Vector store base class."""
 
-    @abstractmethod
-    def load_document(self, chunks: List[Chunk]) -> List[str]:
-        """Load document in vector database.
-
-        Args:
-            chunks(List[Chunk]): document chunks.
-
-        Return:
-            List[str]: chunk ids.
-        """
-
-    def load_document_with_limit(
-        self, chunks: List[Chunk], max_chunks_once_load: int = 10, max_threads: int = 1
-    ) -> List[str]:
-        """Load document in vector database with specified limit.
+    def __init__(self, executor: Optional[ThreadPoolExecutor] = None):
+        """Initialize vector store."""
+        super().__init__(executor)
 
-        Args:
-            chunks(List[Chunk]): Document chunks.
-            max_chunks_once_load(int): Max number of chunks to load at once.
-            max_threads(int): Max number of threads to use.
-
-        Return:
-            List[str]: Chunk ids.
-        """
-        # Group the chunks into chunks of size max_chunks
-        chunk_groups = [
-            chunks[i : i + max_chunks_once_load]
-            for i in range(0, len(chunks), max_chunks_once_load)
-        ]
-        logger.info(
-            f"Loading {len(chunks)} chunks in {len(chunk_groups)} groups with "
-            f"{max_threads} threads."
-        )
-        ids = []
-        loaded_cnt = 0
-        start_time = time.time()
-        with ThreadPoolExecutor(max_workers=max_threads) as executor:
-            tasks = []
-            for chunk_group in chunk_groups:
-                tasks.append(executor.submit(self.load_document, chunk_group))
-            for future in tasks:
-                success_ids = future.result()
-                ids.extend(success_ids)
-                loaded_cnt += len(success_ids)
-                logger.info(f"Loaded {loaded_cnt} chunks, total {len(chunks)} chunks.")
-        logger.info(
-            f"Loaded {len(chunks)} chunks in {time.time() - start_time} seconds"
-        )
-        return ids
-
-    @abstractmethod
-    def similar_search(
-        self, text: str, topk: int, filters: Optional[MetadataFilters] = None
+    def filter_by_score_threshold(
+        self, chunks: List[Chunk], score_threshold: float
     ) -> List[Chunk]:
-        """Similar search in vector database.
+        """Filter chunks by score threshold.
 
         Args:
-            text(str): The query text.
-            topk(int): The number of similar documents to return.
-            filters(Optional[MetadataFilters]): metadata filters.
+            chunks(List[Chunks]): The chunks to filter.
+            score_threshold(float): The score threshold.
         Return:
-            List[Chunk]: The similar documents.
-        """
-        pass
-
-    @abstractmethod
-    def similar_search_with_scores(
-        self,
-        text,
-        topk,
-        score_threshold: float,
-        filters: Optional[MetadataFilters] = None,
-    ) -> List[Chunk]:
-        """Similar search with scores in vector database.
-
-        Args:
-            text(str): The query text.
-            topk(int): The number of similar documents to return.
-            score_threshold(int): score_threshold: Optional, a floating point value
-                between 0 to 1
-            filters(Optional[MetadataFilters]): metadata filters.
-        Return:
-            List[Chunk]: The similar documents.
+            List[Chunks]: The filtered chunks.
         """
+        candidates_chunks = chunks
+        if score_threshold is not None:
+            candidates_chunks = [
+                Chunk(
+                    metadata=chunk.metadata,
+                    content=chunk.content,
+                    score=chunk.score,
+                    chunk_id=str(id),
+                )
+                for chunk in chunks
+                if chunk.score >= score_threshold
+            ]
+            if len(candidates_chunks) == 0:
+                logger.warning(
+                    "No relevant docs were retrieved using the relevance score"
+                    f" threshold {score_threshold}"
+                )
+        return candidates_chunks
 
     @abstractmethod
     def vector_name_exists(self) -> bool:
         """Whether vector name exists."""
         return False
 
-    @abstractmethod
-    def delete_by_ids(self, ids: str):
-        """Delete vectors by ids.
-
-        Args:
-            ids(str): The ids of vectors to delete, separated by comma.
-        """
-
-    @abstractmethod
-    def delete_vector_name(self, vector_name: str):
-        """Delete vector by name.
-
-        Args:
-            vector_name(str): The name of vector to delete.
-        """
-        pass
-
     def convert_metadata_filters(self, filters: MetadataFilters) -> Any:
         """Convert metadata filters to vector store filters.
 
         Args:
             filters: (Optional[MetadataFilters]) metadata filters.
         """
         raise NotImplementedError
@@ -251,7 +160,18 @@
 
         norm = np.linalg.norm(vectors)
         return vectors / norm
 
     def _default_relevance_score_fn(self, distance: float) -> float:
         """Return a similarity score on a scale [0, 1]."""
         return 1.0 - distance / math.sqrt(2)
+
+    async def aload_document(self, chunks: List[Chunk]) -> List[str]:  # type: ignore
+        """Async load document in index database.
+
+        Args:
+            chunks(List[Chunk]): document chunks.
+
+        Return:
+            List[str]: chunk ids.
+        """
+        return await blocking_func_to_async(self._executor, self.load_document, chunks)
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/storage/vector_store/chroma_store.py` & `dbgpt-0.5.7rc0/dbgpt/storage/vector_store/chroma_store.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Chroma vector store."""
 import logging
 import os
-from typing import List, Optional
+from typing import Any, Dict, Iterable, List, Mapping, Optional, Union
 
 from chromadb import PersistentClient
 from chromadb.config import Settings
 
 from dbgpt._private.pydantic import ConfigDict, Field
 from dbgpt.configs.model_config import PILOT_PATH
 from dbgpt.core import Chunk
@@ -13,14 +13,16 @@
 from dbgpt.util.i18n_utils import _
 
 from .base import _COMMON_PARAMETERS, VectorStoreBase, VectorStoreConfig
 from .filters import FilterOperator, MetadataFilters
 
 logger = logging.getLogger(__name__)
 
+CHROMA_COLLECTION_NAME = "langchain"
+
 
 @register_resource(
     _("Chroma Vector Store"),
     "chroma_vector_store",
     category=ResourceCategory.VECTOR_STORE,
     description=_("Chroma vector store."),
     parameters=[
@@ -51,55 +53,62 @@
     )
 
 
 class ChromaStore(VectorStoreBase):
     """Chroma vector store."""
 
     def __init__(self, vector_store_config: ChromaVectorConfig) -> None:
-        """Create a ChromaStore instance."""
-        from langchain.vectorstores import Chroma
+        """Create a ChromaStore instance.
 
+        Args:
+            vector_store_config(ChromaVectorConfig): vector store config.
+        """
+        super().__init__()
         chroma_vector_config = vector_store_config.to_dict(exclude_none=True)
         chroma_path = chroma_vector_config.get(
             "persist_path", os.path.join(PILOT_PATH, "data")
         )
         self.persist_dir = os.path.join(
             chroma_path, vector_store_config.name + ".vectordb"
         )
         self.embeddings = vector_store_config.embedding_fn
         chroma_settings = Settings(
             # chroma_db_impl="duckdb+parquet", => deprecated configuration of Chroma
             persist_directory=self.persist_dir,
             anonymized_telemetry=False,
         )
-        client = PersistentClient(path=self.persist_dir, settings=chroma_settings)
+        self._chroma_client = PersistentClient(
+            path=self.persist_dir, settings=chroma_settings
+        )
 
         collection_metadata = chroma_vector_config.get("collection_metadata") or {
             "hnsw:space": "cosine"
         }
-        self.vector_store_client = Chroma(
-            persist_directory=self.persist_dir,
-            embedding_function=self.embeddings,
-            # client_settings=chroma_settings,
-            client=client,
-            collection_metadata=collection_metadata,
+        self._collection = self._chroma_client.get_or_create_collection(
+            name=CHROMA_COLLECTION_NAME,
+            embedding_function=None,
+            metadata=collection_metadata,
         )
 
     def similar_search(
         self, text, topk, filters: Optional[MetadataFilters] = None
     ) -> List[Chunk]:
         """Search similar documents."""
         logger.info("ChromaStore similar search")
-        where_filters = self.convert_metadata_filters(filters) if filters else None
-        lc_documents = self.vector_store_client.similarity_search(
-            text, topk, filter=where_filters
+        chroma_results = self._query(
+            text=text,
+            topk=topk,
+            filters=filters,
         )
         return [
-            Chunk(content=doc.page_content, metadata=doc.metadata)
-            for doc in lc_documents
+            Chunk(content=chroma_result[0], metadata=chroma_result[1] or {}, score=0.0)
+            for chroma_result in zip(
+                chroma_results["documents"][0],
+                chroma_results["metadatas"][0],
+            )
         ]
 
     def similar_search_with_scores(
         self, text, topk, score_threshold, filters: Optional[MetadataFilters] = None
     ) -> List[Chunk]:
         """Search similar documents with scores.
 
@@ -110,27 +119,34 @@
             topk(int): return docs nums. Defaults to 4.
             score_threshold(float): score_threshold: Optional, a floating point value
                 between 0 to 1 to filter the resulting set of retrieved docs,0 is
                 dissimilar, 1 is most similar.
             filters(MetadataFilters): metadata filters, defaults to None
         """
         logger.info("ChromaStore similar search with scores")
-        where_filters = self.convert_metadata_filters(filters) if filters else None
-        docs_and_scores = (
-            self.vector_store_client.similarity_search_with_relevance_scores(
-                query=text,
-                k=topk,
-                score_threshold=score_threshold,
-                filter=where_filters,
-            )
+        chroma_results = self._query(
+            text=text,
+            topk=topk,
+            filters=filters,
         )
-        return [
-            Chunk(content=doc.page_content, metadata=doc.metadata, score=score)
-            for doc, score in docs_and_scores
+        chunks = [
+            (
+                Chunk(
+                    content=chroma_result[0],
+                    metadata=chroma_result[1] or {},
+                    score=chroma_result[2],
+                )
+            )
+            for chroma_result in zip(
+                chroma_results["documents"][0],
+                chroma_results["metadatas"][0],
+                chroma_results["distances"][0],
+            )
         ]
+        return self.filter_by_score_threshold(chunks, score_threshold)
 
     def vector_name_exists(self) -> bool:
         """Whether vector name exists."""
         logger.info(f"Check persist_dir: {self.persist_dir}")
         if not os.path.exists(self.persist_dir):
             return False
         files = os.listdir(self.persist_dir)
@@ -140,31 +156,34 @@
 
     def load_document(self, chunks: List[Chunk]) -> List[str]:
         """Load document to vector store."""
         logger.info("ChromaStore load document")
         texts = [chunk.content for chunk in chunks]
         metadatas = [chunk.metadata for chunk in chunks]
         ids = [chunk.chunk_id for chunk in chunks]
-        self.vector_store_client.add_texts(texts=texts, metadatas=metadatas, ids=ids)
+        chroma_metadatas = [
+            _transform_chroma_metadata(metadata) for metadata in metadatas
+        ]
+        self._add_texts(texts=texts, metadatas=chroma_metadatas, ids=ids)
         return ids
 
     def delete_vector_name(self, vector_name: str):
         """Delete vector name."""
         logger.info(f"chroma vector_name:{vector_name} begin delete...")
-        self.vector_store_client.delete_collection()
+        # self.vector_store_client.delete_collection()
+        self._chroma_client.delete_collection(self._collection.name)
         self._clean_persist_folder()
         return True
 
     def delete_by_ids(self, ids):
         """Delete vector by ids."""
         logger.info(f"begin delete chroma ids: {ids}")
         ids = ids.split(",")
         if len(ids) > 0:
-            collection = self.vector_store_client._collection
-            collection.delete(ids=ids)
+            self._collection.delete(ids=ids)
 
     def convert_metadata_filters(
         self,
         filters: MetadataFilters,
     ) -> dict:
         """Convert metadata filters to Chroma filters.
 
@@ -194,14 +213,73 @@
 
         if len(filters_list) == 1:
             return filters_list[0]
         elif len(filters_list) > 1:
             where_filters[chroma_condition] = filters_list
         return where_filters
 
+    def _add_texts(
+        self,
+        texts: Iterable[str],
+        ids: List[str],
+        metadatas: Optional[List[Mapping[str, Union[str, int, float, bool]]]] = None,
+    ) -> List[str]:
+        """Add texts to Chroma collection.
+
+        Args:
+            texts(Iterable[str]): texts.
+            metadatas(Optional[List[dict]]): metadatas.
+            ids(Optional[List[str]]): ids.
+        Returns:
+            List[str]: ids.
+        """
+        embeddings = None
+        texts = list(texts)
+        if self.embeddings is not None:
+            embeddings = self.embeddings.embed_documents(texts)
+        if metadatas:
+            try:
+                self._collection.upsert(
+                    metadatas=metadatas,
+                    embeddings=embeddings,  # type: ignore
+                    documents=texts,
+                    ids=ids,
+                )
+            except ValueError as e:
+                logger.error(f"Error upsert chromadb with metadata: {e}")
+        else:
+            self._collection.upsert(
+                embeddings=embeddings,  # type: ignore
+                documents=texts,
+                ids=ids,
+            )
+        return ids
+
+    def _query(self, text: str, topk: int, filters: Optional[MetadataFilters] = None):
+        """Query Chroma collection.
+
+        Args:
+            text(str): query text.
+            topk(int): topk.
+            filters(MetadataFilters): metadata filters.
+        Returns:
+            dict: query result.
+        """
+        if not text:
+            return {}
+        where_filters = self.convert_metadata_filters(filters) if filters else None
+        if self.embeddings is None:
+            raise ValueError("Chroma Embeddings is None")
+        query_embedding = self.embeddings.embed_query(text)
+        return self._collection.query(
+            query_embeddings=query_embedding,
+            n_results=topk,
+            where=where_filters,
+        )
+
     def _clean_persist_folder(self):
         """Clean persist folder."""
         for root, dirs, files in os.walk(self.persist_dir, topdown=False):
             for name in files:
                 os.remove(os.path.join(root, name))
             for name in dirs:
                 os.rmdir(os.path.join(root, name))
@@ -226,7 +304,18 @@
         return "$lt"
     elif operator == FilterOperator.GTE:
         return "$gte"
     elif operator == FilterOperator.LTE:
         return "$lte"
     else:
         raise ValueError(f"Chroma Where operator {operator} not supported")
+
+
+def _transform_chroma_metadata(
+    metadata: Dict[str, Any]
+) -> Mapping[str, str | int | float | bool]:
+    """Transform metadata to Chroma metadata."""
+    transformed = {}
+    for key, value in metadata.items():
+        if isinstance(value, (str, int, float, bool)):
+            transformed[key] = value
+    return transformed
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/storage/vector_store/filters.py` & `dbgpt-0.5.7rc0/dbgpt/storage/vector_store/filters.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/storage/vector_store/milvus_store.py` & `dbgpt-0.5.7rc0/dbgpt/storage/vector_store/milvus_store.py`

 * *Files 5% similar despite different names*

```diff
@@ -145,16 +145,22 @@
     def __init__(self, vector_store_config: MilvusVectorConfig) -> None:
         """Create a MilvusStore instance.
 
         Args:
             vector_store_config (MilvusVectorConfig): MilvusStore config.
             refer to https://milvus.io/docs/v2.0.x/manage_connection.md
         """
-        from pymilvus import connections
-
+        super().__init__()
+        try:
+            from pymilvus import connections
+        except ImportError:
+            raise ValueError(
+                "Could not import pymilvus python package. "
+                "Please install it with `pip install pymilvus`."
+            )
         connect_kwargs = {}
         milvus_vector_config = vector_store_config.to_dict()
         self.uri = milvus_vector_config.get("uri") or os.getenv(
             "MILVUS_URL", "localhost"
         )
         self.port = milvus_vector_config.get("post") or os.getenv(
             "MILVUS_PORT", "19530"
@@ -369,16 +375,21 @@
         doc_ids = [str(doc_id) for doc_id in doc_ids]
         return doc_ids
 
     def similar_search(
         self, text, topk, filters: Optional[MetadataFilters] = None
     ) -> List[Chunk]:
         """Perform a search on a query string and return results."""
-        from pymilvus import Collection, DataType
-
+        try:
+            from pymilvus import Collection, DataType
+        except ImportError:
+            raise ValueError(
+                "Could not import pymilvus python package. "
+                "Please install it with `pip install pymilvus`."
+            )
         """similar_search in vector database."""
         self.col = Collection(self.collection_name)
         schema = self.col.schema
         for x in schema.fields:
             self.fields.append(x.name)
             if x.auto_id:
                 self.fields.remove(x.name)
@@ -415,25 +426,30 @@
             text (str): The query text.
             topk (int): The number of similar documents to return.
             score_threshold (float): Optional, a floating point value between 0 to 1.
             filters (Optional[MetadataFilters]): Optional, metadata filters.
         Returns:
             List[Tuple[Document, float]]: Result doc and score.
         """
-        from pymilvus import Collection
+        try:
+            from pymilvus import Collection, DataType
+        except ImportError:
+            raise ValueError(
+                "Could not import pymilvus python package. "
+                "Please install it with `pip install pymilvus`."
+            )
 
         self.col = Collection(self.collection_name)
         schema = self.col.schema
         for x in schema.fields:
             self.fields.append(x.name)
             if x.auto_id:
                 self.fields.remove(x.name)
             if x.is_primary:
                 self.primary_field = x.name
-            from pymilvus import DataType
 
             if x.dtype == DataType.FLOAT_VECTOR or x.dtype == DataType.BINARY_VECTOR:
                 self.vector_field = x.name
         # convert to milvus expr filter.
         milvus_filter_expr = self.convert_metadata_filters(filters) if filters else None
         _, docs_and_scores = self._search(
             query=text, topk=topk, expr=milvus_filter_expr
@@ -522,32 +538,48 @@
         if len(ret) == 0:
             logger.warning("No relevant docs were retrieved.")
             return None, []
         return ret[0], ret
 
     def vector_name_exists(self):
         """Whether vector name exists."""
-        from pymilvus import utility
+        try:
+            from pymilvus import utility
+        except ImportError:
+            raise ValueError(
+                "Could not import pymilvus python package. "
+                "Please install it with `pip install pymilvus`."
+            )
 
         """is vector store name exist."""
         return utility.has_collection(self.collection_name)
 
     def delete_vector_name(self, vector_name: str):
         """Delete vector name."""
-        from pymilvus import utility
-
+        try:
+            from pymilvus import utility
+        except ImportError:
+            raise ValueError(
+                "Could not import pymilvus python package. "
+                "Please install it with `pip install pymilvus`."
+            )
         """milvus delete collection name"""
         logger.info(f"milvus vector_name:{vector_name} begin delete...")
         utility.drop_collection(self.collection_name)
         return True
 
     def delete_by_ids(self, ids):
         """Delete vector by ids."""
-        from pymilvus import Collection
-
+        try:
+            from pymilvus import Collection
+        except ImportError:
+            raise ValueError(
+                "Could not import pymilvus python package. "
+                "Please install it with `pip install pymilvus`."
+            )
         self.col = Collection(self.collection_name)
         # milvus delete vectors by ids
         logger.info(f"begin delete milvus ids: {ids}")
         delete_ids = ids.split(",")
         doc_ids = [int(doc_id) for doc_id in delete_ids]
         delete_expr = f"{self.primary_field} in {doc_ids}"
         self.col.delete(delete_expr)
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/storage/vector_store/oceanbase_store.py` & `dbgpt-0.5.7rc0/dbgpt/storage/vector_store/oceanbase_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -713,15 +713,15 @@
 class OceanBaseStore(VectorStoreBase):
     """OceanBase vector store."""
 
     def __init__(self, vector_store_config: OceanBaseConfig) -> None:
         """Create a OceanBaseStore instance."""
         if vector_store_config.embedding_fn is None:
             raise ValueError("embedding_fn is required for OceanBaseStore")
-
+        super().__init__()
         self.embeddings = vector_store_config.embedding_fn
         self.collection_name = vector_store_config.name
         vector_store_config = vector_store_config.dict()
         self.OB_HOST = str(
             vector_store_config.get("ob_host") or os.getenv("OB_HOST", "127.0.0.1")
         )
         self.OB_PORT = int(
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/storage/vector_store/pgvector_store.py` & `dbgpt-0.5.7rc0/dbgpt/storage/vector_store/pgvector_store.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Postgres vector store."""
+
 import logging
 from typing import List, Optional
 
 from dbgpt._private.pydantic import ConfigDict, Field
 from dbgpt.core import Chunk
 from dbgpt.core.awel.flow import Parameter, ResourceCategory, register_resource
 from dbgpt.storage.vector_store.base import (
@@ -52,22 +53,27 @@
     """PG vector store.
 
     To use this, you should have the ``pgvector`` python package installed.
     """
 
     def __init__(self, vector_store_config: PGVectorConfig) -> None:
         """Create a PGVectorStore instance."""
-        from langchain.vectorstores import PGVector
-
+        try:
+            from langchain.vectorstores import PGVector  # mypy: ignore
+        except ImportError:
+            raise ImportError(
+                "Please install the `langchain` package to use the PGVector."
+            )
+        super().__init__()
         self.connection_string = vector_store_config.connection_string
         self.embeddings = vector_store_config.embedding_fn
         self.collection_name = vector_store_config.name
 
         self.vector_store_client = PGVector(
-            embedding_function=self.embeddings,
+            embedding_function=self.embeddings,  # type: ignore
             collection_name=self.collection_name,
             connection_string=self.connection_string,
         )
 
     def similar_search(
         self, text: str, topk: int, filters: Optional[MetadataFilters] = None
     ) -> List[Chunk]:
@@ -89,15 +95,16 @@
         Args:
             chunks(List[Chunk]): document chunks.
 
         Return:
             List[str]: chunk ids.
         """
         lc_documents = [Chunk.chunk2langchain(chunk) for chunk in chunks]
-        return self.vector_store_client.from_documents(lc_documents)
+        self.vector_store_client.from_documents(lc_documents)  # type: ignore
+        return [str(chunk.chunk_id) for chunk in lc_documents]
 
     def delete_vector_name(self, vector_name: str):
         """Delete vector by name.
 
         Args:
             vector_name(str): vector name.
         """
@@ -105,8 +112,9 @@
 
     def delete_by_ids(self, ids: str):
         """Delete vector by ids.
 
         Args:
             ids(str): vector ids, separated by comma.
         """
-        return self.vector_store_client.delete(ids)
+        delete_ids = ids.split(",")
+        return self.vector_store_client.delete(delete_ids)
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/storage/vector_store/weaviate_store.py` & `dbgpt-0.5.7rc0/dbgpt/storage/vector_store/weaviate_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         try:
             import weaviate
         except ImportError:
             raise ValueError(
                 "Could not import weaviate python package. "
                 "Please install it with `pip install weaviate-client`."
             )
-
+        super().__init__()
         self.weaviate_url = vector_store_config.weaviate_url
         self.embedding = vector_store_config.embedding_fn
         self.vector_name = vector_store_config.name
         self.persist_dir = os.path.join(
             vector_store_config.persist_path, vector_store_config.name + ".vectordb"
         )
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/_db_migration_utils.py` & `dbgpt-0.5.7rc0/dbgpt/util/_db_migration_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/annotations.py` & `dbgpt-0.5.7rc0/dbgpt/util/annotations.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/api_utils.py` & `dbgpt-0.5.7rc0/dbgpt/util/api_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/benchmarks/llm/fastchat_benchmarks_inference.py` & `dbgpt-0.5.7rc0/dbgpt/util/benchmarks/llm/fastchat_benchmarks_inference.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/benchmarks/llm/llm_benchmarks.py` & `dbgpt-0.5.7rc0/dbgpt/util/benchmarks/llm/llm_benchmarks.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/chat_util.py` & `dbgpt-0.5.7rc0/dbgpt/util/chat_util.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/code_utils.py` & `dbgpt-0.5.7rc0/dbgpt/util/code_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/command_utils.py` & `dbgpt-0.5.7rc0/dbgpt/util/command_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/config_utils.py` & `dbgpt-0.5.7rc0/dbgpt/util/config_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/configure/base.py` & `dbgpt-0.5.7rc0/dbgpt/util/configure/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/console/console.py` & `dbgpt-0.5.7rc0/dbgpt/util/console/console.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/custom_data_structure.py` & `dbgpt-0.5.7rc0/dbgpt/util/custom_data_structure.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/dbgpts/base.py` & `dbgpt-0.5.7rc0/dbgpt/util/dbgpts/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,24 +14,25 @@
 DBGPTS_REPO_HOME = os.getenv("DBGPTS_REPO_HOME", str(DEFAULT_DBGPTS_DIR / "repos"))
 
 DEFAULT_REPO_MAP = {
     "eosphoros/dbgpts": "https://github.com/eosphoros-ai/dbgpts.git",
     "fangyinc/dbgpts": "https://github.com/fangyinc/dbgpts.git",
 }
 
-DEFAULT_PACKAGES = ["agents", "apps", "operators", "workflow"]
-DEFAULT_PACKAGE_TYPES = ["agent", "app", "operator", "flow"]
+DEFAULT_PACKAGES = ["agents", "apps", "operators", "workflow", "resources"]
+DEFAULT_PACKAGE_TYPES = ["agent", "app", "operator", "flow", "resource"]
 INSTALL_METADATA_FILE = "install_metadata.toml"
 DBGPTS_METADATA_FILE = "dbgpts.toml"
 
 TYPE_TO_PACKAGE = {
     "agent": "agents",
     "app": "apps",
     "operator": "operators",
     "flow": "workflow",
+    "resource": "resources",
 }
 
 
 def _get_env_sig() -> str:
     """Get a unique signature for the current Python environment."""
     py_path = os.path.join(os.path.dirname(sys.executable), "python")
     env_path = f"{_ABS_ROOT_PATH}_{py_path}"
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/dbgpts/cli.py` & `dbgpt-0.5.7rc0/dbgpt/util/dbgpts/cli.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/dbgpts/loader.py` & `dbgpt-0.5.7rc0/dbgpt/util/dbgpts/loader.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import inspect
 import logging
 import os
 import sys
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Type, TypeVar, cast
+from typing import Any, Callable, Dict, List, Optional, Tuple, Type, TypeVar, cast
 
 import schedule
 import tomlkit
 
 from dbgpt._private.pydantic import BaseModel, ConfigDict, Field, model_validator
 from dbgpt.component import BaseComponent, SystemApp
+from dbgpt.core.awel import DAG
 from dbgpt.core.awel.flow.flow_factory import FlowPanel
 from dbgpt.util.dbgpts.base import (
     DBGPTS_METADATA_FILE,
     INSTALL_DIR,
     INSTALL_METADATA_FILE,
 )
 
@@ -69,16 +70,19 @@
         return values
 
     def abs_definition_file(self) -> str:
         return str(Path(self.path) / self.definition_file)
 
     @classmethod
     def load_module_class(
-        cls, values: Dict[str, Any], expected_cls: Type[T]
-    ) -> List[Type[T]]:
+        cls,
+        values: Dict[str, Any],
+        expected_cls: Type[T],
+        predicates: Optional[List[Callable[..., bool]]] = None,
+    ) -> Tuple[List[Type[T]], List[Any], List[Any]]:
         import importlib.resources as pkg_resources
 
         from dbgpt.core.awel.dag.loader import _load_modules_from_file
 
         name = values.get("name")
         root = values.get("root")
         if not name:
@@ -86,31 +90,52 @@
         if not root:
             raise ValueError("The root is required")
         if root not in sys.path:
             sys.path.append(root)
         with pkg_resources.path(name, "__init__.py") as path:
             mods = _load_modules_from_file(str(path), name, show_log=False)
             all_cls = [_get_classes_from_module(m) for m in mods]
+            all_predicate_results = []
+            for m in mods:
+                all_predicate_results.extend(_get_from_module(m, predicates))
             module_cls = []
             for list_cls in all_cls:
                 for c in list_cls:
                     if issubclass(c, expected_cls):
                         module_cls.append(c)
-            return module_cls
+            return module_cls, all_predicate_results, mods
 
 
 class FlowPackage(BasePackage):
     package_type: str = "flow"
 
     @classmethod
     def build_from(
         cls, values: Dict[str, Any], ext_dict: Dict[str, Any]
     ) -> "FlowPackage":
         if values["definition_type"] == "json":
             return FlowJsonPackage.build_from(values, ext_dict)
+        return FlowPythonPackage.build_from(values, ext_dict)
+
+
+class FlowPythonPackage(FlowPackage):
+    dag: DAG = Field(..., description="The DAG of the package")
+
+    @classmethod
+    def build_from(cls, values: Dict[str, Any], ext_dict: Dict[str, Any]):
+        from dbgpt.core.awel.dag.loader import _process_modules
+
+        _, _, mods = cls.load_module_class(values, DAG)
+
+        dags = _process_modules(mods, show_log=False)
+        if not dags:
+            raise ValueError("No DAGs found in the package")
+        if len(dags) > 1:
+            raise ValueError("Only support one DAG in the package")
+        values["dag"] = dags[0]
         return cls(**values)
 
 
 class FlowJsonPackage(FlowPackage):
     @classmethod
     def build_from(cls, values: Dict[str, Any], ext_dict: Dict[str, Any]):
         if "json_config" not in ext_dict:
@@ -134,30 +159,70 @@
         default_factory=list, description="The operators of the package"
     )
 
     @classmethod
     def build_from(cls, values: Dict[str, Any], ext_dict: Dict[str, Any]):
         from dbgpt.core.awel import BaseOperator
 
-        values["operators"] = cls.load_module_class(values, BaseOperator)
+        values["operators"], _, _ = cls.load_module_class(values, BaseOperator)
         return cls(**values)
 
 
 class AgentPackage(BasePackage):
     package_type: str = "agent"
 
     agents: List[type] = Field(
         default_factory=list, description="The agents of the package"
     )
 
     @classmethod
     def build_from(cls, values: Dict[str, Any], ext_dict: Dict[str, Any]):
         from dbgpt.agent import ConversableAgent
 
-        values["agents"] = cls.load_module_class(values, ConversableAgent)
+        values["agents"], _, _ = cls.load_module_class(values, ConversableAgent)
+        return cls(**values)
+
+
+class ResourcePackage(BasePackage):
+    package_type: str = "resource"
+
+    resources: List[type] = Field(
+        default_factory=list, description="The resources of the package"
+    )
+    resource_instances: List[Any] = Field(
+        default_factory=list, description="The resource instances of the package"
+    )
+
+    @classmethod
+    def build_from(cls, values: Dict[str, Any], ext_dict: Dict[str, Any]):
+        from dbgpt.agent.resource import Resource
+        from dbgpt.agent.resource.tool.pack import _is_function_tool
+
+        def _predicate(obj):
+            if not obj:
+                return False
+            elif _is_function_tool(obj):
+                return True
+            elif isinstance(obj, Resource):
+                return True
+            elif isinstance(obj, type) and issubclass(obj, Resource):
+                return True
+            else:
+                return False
+
+        _, predicted_cls, _ = cls.load_module_class(values, Resource, [_predicate])
+        resource_instances = []
+        resources = []
+        for o in predicted_cls:
+            if _is_function_tool(o) or isinstance(o, Resource):
+                resource_instances.append(o)
+            elif isinstance(o, type) and issubclass(o, Resource):
+                resources.append(o)
+        values["resource_instances"] = resource_instances
+        values["resources"] = resources
         return cls(**values)
 
 
 class InstalledPackage(BaseModel):
     name: str = Field(..., description="The name of the package")
     repo: str = Field(..., description="The repository of the package")
     root: str = Field(..., description="The root of the package")
@@ -169,14 +234,25 @@
         obj
         for name, obj in inspect.getmembers(module, inspect.isclass)
         if obj.__module__ == module.__name__
     ]
     return classes
 
 
+def _get_from_module(module, predicates: Optional[List[str]] = None):
+    if not predicates:
+        return []
+    results = []
+    for predicate in predicates:
+        for name, obj in inspect.getmembers(module, predicate):
+            if obj.__module__ == module.__name__:
+                results.append(obj)
+    return results
+
+
 def _parse_package_metadata(package: InstalledPackage) -> BasePackage:
     with open(
         Path(package.root) / DBGPTS_METADATA_FILE, mode="r+", encoding="utf-8"
     ) as f:
         metadata = tomlkit.loads(f.read())
     ext_metadata = {}
     pkg_dict = {}
@@ -186,25 +262,30 @@
             pkg_dict["package_type"] = "flow"
         elif key == "operator":
             pkg_dict = {k: v for k, v in value.items()}
             pkg_dict["package_type"] = "operator"
         elif key == "agent":
             pkg_dict = {k: v for k, v in value.items()}
             pkg_dict["package_type"] = "agent"
+        elif key == "resource":
+            pkg_dict = {k: v for k, v in value.items()}
+            pkg_dict["package_type"] = "resource"
         else:
             ext_metadata[key] = value
     pkg_dict["root"] = package.root
     pkg_dict["repo"] = package.repo
     pkg_dict["package"] = package.package
     if pkg_dict["package_type"] == "flow":
         return FlowPackage.build_from(pkg_dict, ext_metadata)
     elif pkg_dict["package_type"] == "operator":
         return OperatorPackage.build_from(pkg_dict, ext_metadata)
     elif pkg_dict["package_type"] == "agent":
         return AgentPackage.build_from(pkg_dict, ext_metadata)
+    elif pkg_dict["package_type"] == "resource":
+        return ResourcePackage.build_from(pkg_dict, ext_metadata)
     else:
         raise ValueError(
             f"Unsupported package package_type: {pkg_dict['package_type']}"
         )
 
 
 def _load_installed_package(path: str) -> List[InstalledPackage]:
@@ -287,24 +368,40 @@
         Returns:
             List[FlowPanel]: The list of the flows
         """
         panels = []
         for package in self._packages.values():
             if package.package_type != "flow":
                 continue
-            package = cast(FlowJsonPackage, package)
+            package = cast(FlowPackage, package)
             dict_value = {
                 "name": package.name,
                 "label": package.label,
                 "version": package.version,
                 "editable": False,
                 "description": package.description,
                 "source": package.repo,
-                "flow_data": package.read_definition_json(),
+                "define_type": "json",
             }
+            if isinstance(package, FlowJsonPackage):
+                dict_value["flow_data"] = package.read_definition_json()
+            elif isinstance(package, FlowPythonPackage):
+                dict_value["flow_data"] = {
+                    "nodes": [],
+                    "edges": [],
+                    "viewport": {
+                        "x": 213,
+                        "y": 269,
+                        "zoom": 0,
+                    },
+                }
+                dict_value["flow_dag"] = package.dag
+                dict_value["define_type"] = "python"
+            else:
+                raise ValueError(f"Unsupported package type: {package}")
             panels.append(FlowPanel(**dict_value))
         return panels
 
     def _register_packages(self, package: BasePackage):
         if package.package_type == "agent":
             from dbgpt.agent import ConversableAgent, get_agent_manager
 
@@ -312,7 +409,24 @@
             pkg = cast(AgentPackage, package)
             for agent_cls in pkg.agents:
                 if issubclass(agent_cls, ConversableAgent):
                     try:
                         agent_manager.register_agent(agent_cls, ignore_duplicate=True)
                     except ValueError as e:
                         logger.warning(f"Register agent {agent_cls} error: {e}")
+        elif package.package_type == "resource":
+            from dbgpt.agent.resource import Resource
+            from dbgpt.agent.resource.manage import get_resource_manager
+
+            pkg = cast(ResourcePackage, package)
+            rm = get_resource_manager(self._system_app)
+            for inst in pkg.resource_instances:
+                try:
+                    rm.register_resource(resource_instance=inst, ignore_duplicate=True)
+                except ValueError as e:
+                    logger.warning(f"Register resource {inst} error: {e}")
+            for res in pkg.resources:
+                try:
+                    if issubclass(res, Resource):
+                        rm.register_resource(res, ignore_duplicate=True)
+                except ValueError as e:
+                    logger.warning(f"Register resource {res} error: {e}")
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/dbgpts/repo.py` & `dbgpt-0.5.7rc0/dbgpt/util/dbgpts/repo.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/dbgpts/template.py` & `dbgpt-0.5.7rc0/dbgpt/util/dbgpts/template.py`

 * *Files 16% similar despite different names*

```diff
@@ -55,14 +55,23 @@
             name,
             mod_name,
             dbgpts_type,
             base_metadata,
             definition_type,
             working_directory,
         )
+    elif dbgpts_type == "resource":
+        _create_resource_template(
+            name,
+            mod_name,
+            dbgpts_type,
+            base_metadata,
+            definition_type,
+            working_directory,
+        )
     else:
         raise ValueError(f"Invalid dbgpts type: {dbgpts_type}")
 
 
 def _create_flow_template(
     name: str,
     mod_name: str,
@@ -84,17 +93,15 @@
     _create_poetry_project(working_directory, name)
     _write_dbgpts_toml(working_directory, name, json_dict)
     _write_manifest_file(working_directory, name, mod_name)
 
     if definition_type == "json":
         _write_flow_define_json_file(working_directory, name, mod_name)
     else:
-        raise click.ClickException(
-            f"Unsupported definition type: {definition_type} for dbgpts type: {dbgpts_type}"
-        )
+        _write_flow_define_python_file(working_directory, name, mod_name)
 
 
 def _create_operator_template(
     name: str,
     mod_name: str,
     dbgpts_type: str,
     base_metadata: dict,
@@ -141,14 +148,39 @@
 
     _create_poetry_project(working_directory, name)
     _write_dbgpts_toml(working_directory, name, json_dict)
     _write_agent_init_file(working_directory, name, mod_name)
     _write_manifest_file(working_directory, name, mod_name)
 
 
+def _create_resource_template(
+    name: str,
+    mod_name: str,
+    dbgpts_type: str,
+    base_metadata: dict,
+    definition_type: str,
+    working_directory: str,
+):
+    json_dict = {
+        "resource": base_metadata,
+        "python_config": {},
+        "json_config": {},
+    }
+    if definition_type != "python":
+        raise click.ClickException(
+            f"Unsupported definition type: {definition_type} for dbgpts type: "
+            f"{dbgpts_type}"
+        )
+
+    _create_poetry_project(working_directory, name)
+    _write_dbgpts_toml(working_directory, name, json_dict)
+    _write_resource_init_file(working_directory, name, mod_name)
+    _write_manifest_file(working_directory, name, mod_name)
+
+
 def _create_poetry_project(working_directory: str, name: str):
     """Create a new poetry project"""
 
     os.chdir(working_directory)
     subprocess.run(["poetry", "new", name, "-n"], check=True)
 
 
@@ -184,14 +216,24 @@
     if not def_file.parent.exists():
         def_file.parent.mkdir(parents=True)
     with open(def_file, "w") as f:
         f.write("")
         print("Please write your flow json to the file: ", def_file)
 
 
+def _write_flow_define_python_file(working_directory: str, name: str, mod_name: str):
+    """Write the flow define python file"""
+
+    init_file = Path(working_directory) / name / mod_name / "__init__.py"
+    content = ""
+
+    with open(init_file, "w") as f:
+        f.write(f'"""{name} flow package"""\n{content}')
+
+
 def _write_operator_init_file(working_directory: str, name: str, mod_name: str):
     """Write the operator __init__.py file"""
 
     init_file = Path(working_directory) / name / mod_name / "__init__.py"
     content = """
 from dbgpt.core.awel import MapOperator
 from dbgpt.core.awel.flow import ViewMetadata, OperatorCategory, IOField, Parameter
@@ -248,41 +290,46 @@
 
     init_file = Path(working_directory) / name / mod_name / "__init__.py"
     content = """
 import asyncio
 from typing import Optional, Tuple
 
 from dbgpt.agent import (
-    AgentMessage,
     Action,
     ActionOutput,
+    AgentMessage,
     AgentResource,
     ConversableAgent,
+    ProfileConfig,
 )
 from dbgpt.agent.util import cmp_string_equal
 
 _HELLO_WORLD = "Hello world"
 
 
 class HelloWorldSpeakerAgent(ConversableAgent):
-    name: str = "Hodor"
-    profile: str = "HelloWorldSpeaker"
-    goal: str = f"answer any question from user with '{_HELLO_WORLD}'"
-    desc: str = f"You can answer any question from user with '{_HELLO_WORLD}'"
-    constraints: list[str] = [
-        "You can only answer with '{fix_message}'",
-        "You can't use any other words",
-    ]
-    examples: str = (
-        f"user: What's your name?\\nassistant: {_HELLO_WORLD}\\n\\n",
-        f"user: What's the weather today?\\nassistant: {_HELLO_WORLD}\\n\\n",
-        f"user: Can you help me?\\nassistant: {_HELLO_WORLD}\\n\\n",
-        f"user: Please tell me a joke.\\nassistant: {_HELLO_WORLD}\\n\\n",
-        f"user: Please answer me without '{_HELLO_WORLD}'.\\nassistant: {_HELLO_WORLD}"
-        "\\n\\n",
+
+    profile: ProfileConfig = ProfileConfig(
+        name="Hodor",
+        role="HelloWorldSpeaker",
+        goal=f"answer any question from user with '{_HELLO_WORLD}'",
+        desc=f"You can answer any question from user with '{_HELLO_WORLD}'",
+        constraints=[
+            "You can only answer with '{{ fix_message }}'",
+            f"You can't use any other words",
+        ],
+        examples=(
+            f"user: What's your name?\\nassistant: {_HELLO_WORLD}\\n\\n"
+            f"user: What's the weather today?\\nassistant: {_HELLO_WORLD}\\n\\n"
+            f"user: Can you help me?\\nassistant: {_HELLO_WORLD}\\n\\n"
+            f"user: Please tell me a joke.\\nassistant: {_HELLO_WORLD}\\n\\n"
+            f"user: Please answer me without '{_HELLO_WORLD}'.\\nassistant: "
+            f"{_HELLO_WORLD}"
+            "\\n\\n"
+        ),
     )
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self._init_actions([HelloWorldAction])
 
     def _init_reply_message(self, received_message: AgentMessage) -> AgentMessage:
@@ -326,37 +373,59 @@
 
 async def _test_agent():
     \"\"\"Test the agent.
 
     It will not run in the production environment.
     \"\"\"
     from dbgpt.model.proxy import OpenAILLMClient
-    from dbgpt.agent import AgentContext, GptsMemory, UserProxyAgent, LLMConfig
+    from dbgpt.agent import AgentContext, AgentMemory, UserProxyAgent, LLMConfig
 
     llm_client = OpenAILLMClient(model_alias="gpt-3.5-turbo")
     context: AgentContext = AgentContext(conv_id="summarize")
 
-    default_memory: GptsMemory = GptsMemory()
+    agent_memory: AgentMemory = AgentMemory()
 
     speaker = (
         await HelloWorldSpeakerAgent()
         .bind(context)
         .bind(LLMConfig(llm_client=llm_client))
-        .bind(default_memory)
+        .bind(agent_memory)
         .build()
     )
 
-    user_proxy = await UserProxyAgent().bind(default_memory).bind(context).build()
+    user_proxy = await UserProxyAgent().bind(agent_memory).bind(context).build()
     await user_proxy.initiate_chat(
         recipient=speaker,
         reviewer=user_proxy,
         message="What's your name?",
     )
-    print(await default_memory.one_chat_completions("summarize"))
+    print(await agent_memory.gpts_memory.one_chat_completions("summarize"))
 
 
 if __name__ == "__main__":
     asyncio.run(_test_agent())
 
 """
     with open(init_file, "w") as f:
         f.write(f'"""{name} agent package."""\n{content}')
+
+
+def _write_resource_init_file(working_directory: str, name: str, mod_name: str):
+    """Write the resource __init__.py file"""
+
+    init_file = Path(working_directory) / name / mod_name / "__init__.py"
+    content = """\"\"\"A custom resource module that provides a simple tool to send GET requests.\"\"\"
+
+from dbgpt.agent.resource import tool
+
+
+@tool
+def simple_send_requests_get(url: str):
+    \"\"\"Send a GET request to the specified URL and return the text content.\"\"\"
+    import requests
+
+    response = requests.get(url)
+    return response.text
+    
+"""
+    with open(init_file, "w") as f:
+        f.write(content)
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/error_types.py` & `dbgpt-0.5.7rc0/dbgpt/util/error_types.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/executor_utils.py` & `dbgpt-0.5.7rc0/dbgpt/util/executor_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/fastapi.py` & `dbgpt-0.5.7rc0/dbgpt/util/fastapi.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/formatting.py` & `dbgpt-0.5.7rc0/dbgpt/util/formatting.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/function_utils.py` & `dbgpt-0.5.7rc0/dbgpt/util/function_utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 import asyncio
 import inspect
 from functools import wraps
-from typing import Any, get_args, get_origin, get_type_hints
+from typing import (
+    Any,
+    Dict,
+    List,
+    Optional,
+    Union,
+    _UnionGenericAlias,
+    get_args,
+    get_origin,
+    get_type_hints,
+)
 
 from typeguard import check_type
+from typing_extensions import Annotated, Doc, _AnnotatedAlias
 
 
 def _is_typing(obj):
     from typing import _Final  # type: ignore
 
     return isinstance(obj, _Final)
 
@@ -115,7 +126,65 @@
 
     @wraps(func)
     async def async_wrapper(*args, **kwargs):
         sorted_args, sorted_kwargs = _sort_args(func, args, kwargs)
         return await func(*sorted_args, **sorted_kwargs)
 
     return async_wrapper if asyncio.iscoroutinefunction(func) else sync_wrapper
+
+
+def type_to_string(obj: Any, default_type: str = "unknown") -> str:
+    """Convert a type to a string representation."""
+    type_map = {
+        int: "integer",
+        str: "string",
+        float: "float",
+        bool: "boolean",
+        Any: "any",
+        List: "array",
+        dict: "object",
+    }
+    # Check NoneType
+    if obj is type(None):
+        return "null"
+
+    # Get the origin of the type
+    origin = getattr(obj, "__origin__", None)
+    if origin:
+        if _is_typing(origin) and not isinstance(obj, _UnionGenericAlias):
+            obj = origin
+            origin = origin.__origin__
+        # Handle special cases like List[int]
+        if origin is Union and hasattr(obj, "__args__"):
+            subtypes = ", ".join(
+                type_to_string(t) for t in obj.__args__ if t is not type(None)
+            )
+            # return f"Optional[{subtypes}]"
+            return subtypes
+        elif origin is list or origin is List:
+            subtypes = ", ".join(type_to_string(t) for t in obj.__args__)
+            # return f"List[{subtypes}]"
+            return "array"
+        elif origin in [dict, Dict]:
+            key_type, value_type = (type_to_string(t) for t in obj.__args__)
+            # return f"Dict[{key_type}, {value_type}]"
+            return "object"
+        return type_map.get(origin, default_type)
+    else:
+        if hasattr(obj, "__args__"):
+            subtypes = ", ".join(
+                type_to_string(t) for t in obj.__args__ if t is not type(None)
+            )
+            return subtypes
+
+    return type_map.get(obj, default_type)
+
+
+def parse_param_description(name: str, obj: Any) -> str:
+    default_type_title = name.replace("_", " ").title()
+    if isinstance(obj, _AnnotatedAlias):
+        metadata = obj.__metadata__
+        docs = [arg for arg in metadata if isinstance(arg, Doc)]
+        doc_str = docs[0].documentation if docs else default_type_title
+    else:
+        doc_str = default_type_title
+    return doc_str
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/global_helper.py` & `dbgpt-0.5.7rc0/dbgpt/util/global_helper.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/i18n_utils.py` & `dbgpt-0.5.7rc0/dbgpt/util/i18n_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/id_generator.py` & `dbgpt-0.5.7rc0/dbgpt/util/id_generator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/json_utils.py` & `dbgpt-0.5.7rc0/dbgpt/util/json_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/model_utils.py` & `dbgpt-0.5.7rc0/dbgpt/util/model_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/module_utils.py` & `dbgpt-0.5.7rc0/dbgpt/util/module_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/net_utils.py` & `dbgpt-0.5.7rc0/dbgpt/util/net_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/network/_cli.py` & `dbgpt-0.5.7rc0/dbgpt/util/network/_cli.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/openai_utils.py` & `dbgpt-0.5.7rc0/dbgpt/util/openai_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/pagination_utils.py` & `dbgpt-0.5.7rc0/dbgpt/util/pagination_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/parameter_utils.py` & `dbgpt-0.5.7rc0/dbgpt/util/parameter_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,14 +100,17 @@
             args_prefix: args prefix
         Returns:
             A list of strings where each field is represented by two items:
             one for the field name prefixed by args_prefix, and one for its value.
         """
         return _dict_to_command_args(asdict(self), args_prefix=args_prefix)
 
+    def to_dict(self) -> Dict[str, Any]:
+        return asdict(self)
+
 
 def _get_dataclass_print_str(obj):
     class_name = obj.__class__.__name__
     parameters = [
         f"\n\n=========================== {class_name} ===========================\n"
     ]
     for field_info in fields(obj):
```

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/pd_utils.py` & `dbgpt-0.5.7rc0/dbgpt/util/pd_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/prompt_util.py` & `dbgpt-0.5.7rc0/dbgpt/util/prompt_util.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/retry.py` & `dbgpt-0.5.7rc0/dbgpt/util/retry.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/serialization/json_serialization.py` & `dbgpt-0.5.7rc0/dbgpt/util/serialization/json_serialization.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/similarity_util.py` & `dbgpt-0.5.7rc0/dbgpt/util/similarity_util.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/singleton.py` & `dbgpt-0.5.7rc0/dbgpt/util/singleton.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/speech/base.py` & `dbgpt-0.5.7rc0/dbgpt/util/speech/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/speech/brian.py` & `dbgpt-0.5.7rc0/dbgpt/util/speech/brian.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/speech/eleven_labs.py` & `dbgpt-0.5.7rc0/dbgpt/util/speech/eleven_labs.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/speech/macos_tts.py` & `dbgpt-0.5.7rc0/dbgpt/util/speech/macos_tts.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/speech/say.py` & `dbgpt-0.5.7rc0/dbgpt/util/speech/say.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/splitter_utils.py` & `dbgpt-0.5.7rc0/dbgpt/util/splitter_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/string_utils.py` & `dbgpt-0.5.7rc0/dbgpt/util/string_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/system_utils.py` & `dbgpt-0.5.7rc0/dbgpt/util/system_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/time_utils.py` & `dbgpt-0.5.7rc0/dbgpt/util/time_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/tracer/__init__.py` & `dbgpt-0.5.7rc0/dbgpt/util/tracer/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/tracer/base.py` & `dbgpt-0.5.7rc0/dbgpt/util/tracer/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/tracer/span_storage.py` & `dbgpt-0.5.7rc0/dbgpt/util/tracer/span_storage.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/tracer/tracer_cli.py` & `dbgpt-0.5.7rc0/dbgpt/util/tracer/tracer_cli.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/tracer/tracer_impl.py` & `dbgpt-0.5.7rc0/dbgpt/util/tracer/tracer_impl.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/tracer/tracer_middleware.py` & `dbgpt-0.5.7rc0/dbgpt/util/tracer/tracer_middleware.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/util/utils.py` & `dbgpt-0.5.7rc0/dbgpt/util/utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/vis/__init__.py` & `dbgpt-0.5.7rc0/dbgpt/vis/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/vis/base.py` & `dbgpt-0.5.7rc0/dbgpt/vis/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/vis/client.py` & `dbgpt-0.5.7rc0/dbgpt/vis/client.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/vis/tags/vis_chart.py` & `dbgpt-0.5.7rc0/dbgpt/vis/tags/vis_chart.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt/vis/tags/vis_dashboard.py` & `dbgpt-0.5.7rc0/dbgpt/vis/tags/vis_dashboard.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.6rc0/dbgpt.egg-info/PKG-INFO` & `dbgpt-0.5.7rc0/dbgpt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbgpt
-Version: 0.5.6rc0
+Version: 0.5.7rc0
 Summary: DB-GPT is an experimental open-source project that uses localized GPT large models to interact with your data and environment. With this solution, you can be assured that there is no risk of data leakage, and your data is 100% private and secure.
 Home-page: https://github.com/eosphoros-ai/DB-GPT
 Author: csunny
 Author-email: cfqcsunny@gmail.com
 License: https://opensource.org/license/mit/
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -13,155 +13,162 @@
 Requires-Dist: chardet==5.1.0
 Requires-Dist: importlib-resources==5.12.0
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: cachetools
 Requires-Dist: pydantic>=2.6.0
 Requires-Dist: typeguard
 Requires-Dist: snowflake-id
+Requires-Dist: typing_inspect
 Provides-Extra: core
-Requires-Dist: cachetools; extra == "core"
-Requires-Dist: importlib-resources==5.12.0; extra == "core"
-Requires-Dist: python-dotenv==1.0.0; extra == "core"
-Requires-Dist: aiohttp==3.8.4; extra == "core"
-Requires-Dist: snowflake-id; extra == "core"
 Requires-Dist: chardet==5.1.0; extra == "core"
+Requires-Dist: typing_inspect; extra == "core"
 Requires-Dist: typeguard; extra == "core"
 Requires-Dist: pydantic>=2.6.0; extra == "core"
+Requires-Dist: snowflake-id; extra == "core"
+Requires-Dist: python-dotenv==1.0.0; extra == "core"
+Requires-Dist: importlib-resources==5.12.0; extra == "core"
+Requires-Dist: aiohttp==3.8.4; extra == "core"
+Requires-Dist: cachetools; extra == "core"
 Provides-Extra: client
-Requires-Dist: cachetools; extra == "client"
 Requires-Dist: fastapi>=0.100.0; extra == "client"
-Requires-Dist: httpx; extra == "client"
-Requires-Dist: importlib-resources==5.12.0; extra == "client"
-Requires-Dist: python-dotenv==1.0.0; extra == "client"
-Requires-Dist: aiohttp==3.8.4; extra == "client"
-Requires-Dist: snowflake-id; extra == "client"
 Requires-Dist: chardet==5.1.0; extra == "client"
+Requires-Dist: typing_inspect; extra == "client"
 Requires-Dist: typeguard; extra == "client"
 Requires-Dist: pydantic>=2.6.0; extra == "client"
+Requires-Dist: snowflake-id; extra == "client"
+Requires-Dist: python-dotenv==1.0.0; extra == "client"
+Requires-Dist: importlib-resources==5.12.0; extra == "client"
+Requires-Dist: aiohttp==3.8.4; extra == "client"
+Requires-Dist: cachetools; extra == "client"
+Requires-Dist: httpx; extra == "client"
 Provides-Extra: cli
-Requires-Dist: cachetools; extra == "cli"
 Requires-Dist: fastapi>=0.100.0; extra == "cli"
 Requires-Dist: psutil==5.9.4; extra == "cli"
+Requires-Dist: chardet==5.1.0; extra == "cli"
+Requires-Dist: typing_inspect; extra == "cli"
 Requires-Dist: tomlkit; extra == "cli"
-Requires-Dist: httpx; extra == "cli"
-Requires-Dist: importlib-resources==5.12.0; extra == "cli"
-Requires-Dist: python-dotenv==1.0.0; extra == "cli"
-Requires-Dist: prettytable; extra == "cli"
-Requires-Dist: aiohttp==3.8.4; extra == "cli"
+Requires-Dist: typeguard; extra == "cli"
+Requires-Dist: rich; extra == "cli"
+Requires-Dist: pydantic>=2.6.0; extra == "cli"
 Requires-Dist: snowflake-id; extra == "cli"
 Requires-Dist: colorama==0.4.6; extra == "cli"
-Requires-Dist: rich; extra == "cli"
+Requires-Dist: python-dotenv==1.0.0; extra == "cli"
+Requires-Dist: importlib-resources==5.12.0; extra == "cli"
 Requires-Dist: click; extra == "cli"
-Requires-Dist: chardet==5.1.0; extra == "cli"
-Requires-Dist: typeguard; extra == "cli"
-Requires-Dist: pydantic>=2.6.0; extra == "cli"
+Requires-Dist: prettytable; extra == "cli"
+Requires-Dist: aiohttp==3.8.4; extra == "cli"
+Requires-Dist: cachetools; extra == "cli"
+Requires-Dist: httpx; extra == "cli"
 Provides-Extra: agent
-Requires-Dist: pandas==2.0.3; extra == "agent"
-Requires-Dist: cachetools; extra == "agent"
 Requires-Dist: fastapi>=0.100.0; extra == "agent"
+Requires-Dist: snowflake-id; extra == "agent"
+Requires-Dist: colorama==0.4.6; extra == "agent"
+Requires-Dist: pandas==2.0.3; extra == "agent"
+Requires-Dist: prettytable; extra == "agent"
 Requires-Dist: psutil==5.9.4; extra == "agent"
-Requires-Dist: tomlkit; extra == "agent"
+Requires-Dist: chardet==5.1.0; extra == "agent"
+Requires-Dist: typing_inspect; extra == "agent"
 Requires-Dist: termcolor; extra == "agent"
-Requires-Dist: httpx; extra == "agent"
 Requires-Dist: importlib-resources==5.12.0; extra == "agent"
-Requires-Dist: python-dotenv==1.0.0; extra == "agent"
-Requires-Dist: prettytable; extra == "agent"
-Requires-Dist: aiohttp==3.8.4; extra == "agent"
-Requires-Dist: snowflake-id; extra == "agent"
-Requires-Dist: colorama==0.4.6; extra == "agent"
-Requires-Dist: rich; extra == "agent"
 Requires-Dist: click; extra == "agent"
-Requires-Dist: chardet==5.1.0; extra == "agent"
+Requires-Dist: rich; extra == "agent"
+Requires-Dist: python-dotenv==1.0.0; extra == "agent"
 Requires-Dist: typeguard; extra == "agent"
 Requires-Dist: pydantic>=2.6.0; extra == "agent"
+Requires-Dist: aiohttp==3.8.4; extra == "agent"
+Requires-Dist: tomlkit; extra == "agent"
+Requires-Dist: cachetools; extra == "agent"
+Requires-Dist: httpx; extra == "agent"
 Provides-Extra: simple-framework
-Requires-Dist: schedule; extra == "simple-framework"
+Requires-Dist: fastapi>=0.100.0; extra == "simple-framework"
+Requires-Dist: snowflake-id; extra == "simple-framework"
+Requires-Dist: colorama==0.4.6; extra == "simple-framework"
+Requires-Dist: pandas==2.0.3; extra == "simple-framework"
+Requires-Dist: jinja2; extra == "simple-framework"
 Requires-Dist: sqlparse==0.4.4; extra == "simple-framework"
-Requires-Dist: msgpack; extra == "simple-framework"
+Requires-Dist: prettytable; extra == "simple-framework"
+Requires-Dist: psutil==5.9.4; extra == "simple-framework"
+Requires-Dist: chardet==5.1.0; extra == "simple-framework"
+Requires-Dist: typing_inspect; extra == "simple-framework"
+Requires-Dist: uvicorn; extra == "simple-framework"
 Requires-Dist: termcolor; extra == "simple-framework"
-Requires-Dist: rich; extra == "simple-framework"
+Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "simple-framework"
 Requires-Dist: shortuuid; extra == "simple-framework"
-Requires-Dist: typeguard; extra == "simple-framework"
-Requires-Dist: jinja2; extra == "simple-framework"
-Requires-Dist: cachetools; extra == "simple-framework"
-Requires-Dist: psutil==5.9.4; extra == "simple-framework"
 Requires-Dist: importlib-resources==5.12.0; extra == "simple-framework"
-Requires-Dist: prettytable; extra == "simple-framework"
-Requires-Dist: fschat; extra == "simple-framework"
-Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "simple-framework"
 Requires-Dist: click; extra == "simple-framework"
-Requires-Dist: duckdb-engine; extra == "simple-framework"
-Requires-Dist: pandas==2.0.3; extra == "simple-framework"
-Requires-Dist: fastapi>=0.100.0; extra == "simple-framework"
+Requires-Dist: schedule; extra == "simple-framework"
 Requires-Dist: pympler; extra == "simple-framework"
-Requires-Dist: tomlkit; extra == "simple-framework"
-Requires-Dist: uvicorn; extra == "simple-framework"
-Requires-Dist: httpx; extra == "simple-framework"
-Requires-Dist: python-dotenv==1.0.0; extra == "simple-framework"
-Requires-Dist: colorama==0.4.6; extra == "simple-framework"
-Requires-Dist: snowflake-id; extra == "simple-framework"
-Requires-Dist: chardet==5.1.0; extra == "simple-framework"
 Requires-Dist: duckdb; extra == "simple-framework"
-Requires-Dist: aiohttp==3.8.4; extra == "simple-framework"
+Requires-Dist: rich; extra == "simple-framework"
+Requires-Dist: python-dotenv==1.0.0; extra == "simple-framework"
+Requires-Dist: duckdb-engine; extra == "simple-framework"
+Requires-Dist: typeguard; extra == "simple-framework"
 Requires-Dist: pydantic>=2.6.0; extra == "simple-framework"
+Requires-Dist: aiohttp==3.8.4; extra == "simple-framework"
+Requires-Dist: fschat; extra == "simple-framework"
+Requires-Dist: tomlkit; extra == "simple-framework"
+Requires-Dist: msgpack; extra == "simple-framework"
+Requires-Dist: cachetools; extra == "simple-framework"
+Requires-Dist: httpx; extra == "simple-framework"
 Provides-Extra: framework
-Requires-Dist: schedule; extra == "framework"
-Requires-Dist: sqlparse==0.4.4; extra == "framework"
-Requires-Dist: seaborn; extra == "framework"
-Requires-Dist: msgpack; extra == "framework"
-Requires-Dist: termcolor; extra == "framework"
-Requires-Dist: alembic==1.12.0; extra == "framework"
-Requires-Dist: rich; extra == "framework"
-Requires-Dist: shortuuid; extra == "framework"
-Requires-Dist: typeguard; extra == "framework"
+Requires-Dist: fastapi>=0.100.0; extra == "framework"
+Requires-Dist: transformers>=4.34.0; extra == "framework"
+Requires-Dist: auto-gpt-plugin-template; extra == "framework"
+Requires-Dist: snowflake-id; extra == "framework"
+Requires-Dist: jsonschema; extra == "framework"
+Requires-Dist: colorama==0.4.6; extra == "framework"
+Requires-Dist: pandas==2.0.3; extra == "framework"
 Requires-Dist: jinja2; extra == "framework"
-Requires-Dist: pymysql; extra == "framework"
-Requires-Dist: cachetools; extra == "framework"
-Requires-Dist: psutil==5.9.4; extra == "framework"
-Requires-Dist: importlib-resources==5.12.0; extra == "framework"
+Requires-Dist: sqlparse==0.4.4; extra == "framework"
 Requires-Dist: prettytable; extra == "framework"
-Requires-Dist: fschat; extra == "framework"
+Requires-Dist: openpyxl==3.1.2; extra == "framework"
 Requires-Dist: graphviz; extra == "framework"
+Requires-Dist: psutil==5.9.4; extra == "framework"
+Requires-Dist: chardet==5.1.0; extra == "framework"
+Requires-Dist: typing_inspect; extra == "framework"
+Requires-Dist: uvicorn; extra == "framework"
+Requires-Dist: pymysql; extra == "framework"
+Requires-Dist: termcolor; extra == "framework"
 Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "framework"
+Requires-Dist: shortuuid; extra == "framework"
+Requires-Dist: gTTS==2.3.1; extra == "framework"
+Requires-Dist: importlib-resources==5.12.0; extra == "framework"
 Requires-Dist: click; extra == "framework"
-Requires-Dist: duckdb-engine; extra == "framework"
-Requires-Dist: pandas==2.0.3; extra == "framework"
-Requires-Dist: fastapi>=0.100.0; extra == "framework"
-Requires-Dist: jsonschema; extra == "framework"
-Requires-Dist: pympler; extra == "framework"
-Requires-Dist: tomlkit; extra == "framework"
-Requires-Dist: uvicorn; extra == "framework"
-Requires-Dist: auto-gpt-plugin-template; extra == "framework"
-Requires-Dist: httpx; extra == "framework"
-Requires-Dist: coloredlogs; extra == "framework"
-Requires-Dist: python-dotenv==1.0.0; extra == "framework"
-Requires-Dist: colorama==0.4.6; extra == "framework"
-Requires-Dist: snowflake-id; extra == "framework"
-Requires-Dist: transformers>=4.34.0; extra == "framework"
 Requires-Dist: aiofiles; extra == "framework"
-Requires-Dist: GitPython; extra == "framework"
-Requires-Dist: chardet==5.1.0; extra == "framework"
-Requires-Dist: gTTS==2.3.1; extra == "framework"
-Requires-Dist: duckdb; extra == "framework"
+Requires-Dist: schedule; extra == "framework"
+Requires-Dist: pympler; extra == "framework"
 Requires-Dist: xlrd==2.0.1; extra == "framework"
-Requires-Dist: aiohttp==3.8.4; extra == "framework"
-Requires-Dist: openpyxl==3.1.2; extra == "framework"
+Requires-Dist: duckdb; extra == "framework"
+Requires-Dist: GitPython; extra == "framework"
+Requires-Dist: alembic==1.12.0; extra == "framework"
+Requires-Dist: rich; extra == "framework"
+Requires-Dist: python-dotenv==1.0.0; extra == "framework"
+Requires-Dist: duckdb-engine; extra == "framework"
+Requires-Dist: coloredlogs; extra == "framework"
+Requires-Dist: typeguard; extra == "framework"
 Requires-Dist: pydantic>=2.6.0; extra == "framework"
+Requires-Dist: aiohttp==3.8.4; extra == "framework"
+Requires-Dist: fschat; extra == "framework"
+Requires-Dist: tomlkit; extra == "framework"
+Requires-Dist: seaborn; extra == "framework"
+Requires-Dist: msgpack; extra == "framework"
+Requires-Dist: cachetools; extra == "framework"
+Requires-Dist: httpx; extra == "framework"
 Provides-Extra: torch
-Requires-Dist: torchvision==0.17.1; extra == "torch"
-Requires-Dist: torch==2.2.1; extra == "torch"
 Requires-Dist: torchaudio==2.2.1; extra == "torch"
+Requires-Dist: torch==2.2.1; extra == "torch"
+Requires-Dist: torchvision==0.17.1; extra == "torch"
 Provides-Extra: torch-cpu
-Requires-Dist: torchvision==0.17.1; extra == "torch-cpu"
-Requires-Dist: torch==2.2.1; extra == "torch-cpu"
 Requires-Dist: torchaudio==2.2.1; extra == "torch-cpu"
+Requires-Dist: torch==2.2.1; extra == "torch-cpu"
+Requires-Dist: torchvision==0.17.1; extra == "torch-cpu"
 Provides-Extra: torch-cuda
-Requires-Dist: torchvision==0.17.1; extra == "torch-cuda"
-Requires-Dist: torch==2.2.1; extra == "torch-cuda"
 Requires-Dist: torchaudio==2.2.1; extra == "torch-cuda"
+Requires-Dist: torch==2.2.1; extra == "torch-cuda"
+Requires-Dist: torchvision==0.17.1; extra == "torch-cuda"
 Provides-Extra: llama-cpp
 Requires-Dist: llama-cpp-python; extra == "llama-cpp"
 Provides-Extra: bitsandbytes
 Requires-Dist: bitsandbytes; extra == "bitsandbytes"
 Provides-Extra: quantization
 Requires-Dist: cpm_kernels; extra == "quantization"
 Requires-Dist: bitsandbytes; extra == "quantization"
@@ -176,246 +183,247 @@
 Provides-Extra: vstore-all
 Requires-Dist: pymilvus; extra == "vstore-all"
 Requires-Dist: weaviate-client; extra == "vstore-all"
 Requires-Dist: chromadb>=0.4.22; extra == "vstore-all"
 Provides-Extra: datasource
 Requires-Dist: pymysql; extra == "datasource"
 Provides-Extra: datasource-all
-Requires-Dist: pymysql; extra == "datasource-all"
 Requires-Dist: thrift; extra == "datasource-all"
-Requires-Dist: pymssql; extra == "datasource-all"
-Requires-Dist: clickhouse-connect; extra == "datasource-all"
-Requires-Dist: thrift_sasl; extra == "datasource-all"
-Requires-Dist: pydoris<2.0.0,>=1.0.2; extra == "datasource-all"
 Requires-Dist: neo4j; extra == "datasource-all"
-Requires-Dist: pyhive; extra == "datasource-all"
-Requires-Dist: psycopg2; extra == "datasource-all"
 Requires-Dist: mysqlclient==2.1.0; extra == "datasource-all"
+Requires-Dist: pymysql; extra == "datasource-all"
+Requires-Dist: pymssql; extra == "datasource-all"
+Requires-Dist: psycopg2; extra == "datasource-all"
+Requires-Dist: pydoris<2.0.0,>=1.0.2; extra == "datasource-all"
+Requires-Dist: vertica_python; extra == "datasource-all"
 Requires-Dist: pyspark; extra == "datasource-all"
+Requires-Dist: pyhive; extra == "datasource-all"
+Requires-Dist: thrift_sasl; extra == "datasource-all"
+Requires-Dist: clickhouse-connect; extra == "datasource-all"
 Provides-Extra: rag
-Requires-Dist: bs4; extra == "rag"
-Requires-Dist: markdown; extra == "rag"
-Requires-Dist: spacy>=3.7; extra == "rag"
 Requires-Dist: sentence-transformers; extra == "rag"
-Requires-Dist: python-pptx; extra == "rag"
+Requires-Dist: python-multipart; extra == "rag"
 Requires-Dist: python-docx; extra == "rag"
+Requires-Dist: bs4; extra == "rag"
+Requires-Dist: python-pptx; extra == "rag"
 Requires-Dist: pypdf; extra == "rag"
+Requires-Dist: spacy>=3.7; extra == "rag"
 Requires-Dist: chromadb>=0.4.22; extra == "rag"
-Requires-Dist: langchain>=0.0.286; extra == "rag"
-Requires-Dist: python-multipart; extra == "rag"
+Requires-Dist: markdown; extra == "rag"
 Provides-Extra: openai
-Requires-Dist: schedule; extra == "openai"
-Requires-Dist: sqlparse==0.4.4; extra == "openai"
-Requires-Dist: seaborn; extra == "openai"
-Requires-Dist: markdown; extra == "openai"
-Requires-Dist: msgpack; extra == "openai"
-Requires-Dist: termcolor; extra == "openai"
+Requires-Dist: fastapi>=0.100.0; extra == "openai"
+Requires-Dist: transformers>=4.34.0; extra == "openai"
+Requires-Dist: python-multipart; extra == "openai"
 Requires-Dist: sentence-transformers; extra == "openai"
-Requires-Dist: tiktoken; extra == "openai"
-Requires-Dist: alembic==1.12.0; extra == "openai"
-Requires-Dist: rich; extra == "openai"
-Requires-Dist: shortuuid; extra == "openai"
 Requires-Dist: pypdf; extra == "openai"
+Requires-Dist: auto-gpt-plugin-template; extra == "openai"
+Requires-Dist: snowflake-id; extra == "openai"
+Requires-Dist: jsonschema; extra == "openai"
+Requires-Dist: colorama==0.4.6; extra == "openai"
 Requires-Dist: chromadb>=0.4.22; extra == "openai"
-Requires-Dist: typeguard; extra == "openai"
+Requires-Dist: pandas==2.0.3; extra == "openai"
 Requires-Dist: jinja2; extra == "openai"
-Requires-Dist: python-multipart; extra == "openai"
-Requires-Dist: pymysql; extra == "openai"
-Requires-Dist: cachetools; extra == "openai"
-Requires-Dist: psutil==5.9.4; extra == "openai"
-Requires-Dist: importlib-resources==5.12.0; extra == "openai"
+Requires-Dist: sqlparse==0.4.4; extra == "openai"
 Requires-Dist: prettytable; extra == "openai"
-Requires-Dist: fschat; extra == "openai"
+Requires-Dist: openpyxl==3.1.2; extra == "openai"
 Requires-Dist: graphviz; extra == "openai"
-Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "openai"
-Requires-Dist: click; extra == "openai"
-Requires-Dist: duckdb-engine; extra == "openai"
-Requires-Dist: pandas==2.0.3; extra == "openai"
-Requires-Dist: fastapi>=0.100.0; extra == "openai"
-Requires-Dist: jsonschema; extra == "openai"
-Requires-Dist: spacy>=3.7; extra == "openai"
-Requires-Dist: pympler; extra == "openai"
-Requires-Dist: tomlkit; extra == "openai"
-Requires-Dist: uvicorn; extra == "openai"
-Requires-Dist: auto-gpt-plugin-template; extra == "openai"
-Requires-Dist: httpx; extra == "openai"
-Requires-Dist: coloredlogs; extra == "openai"
-Requires-Dist: python-dotenv==1.0.0; extra == "openai"
-Requires-Dist: colorama==0.4.6; extra == "openai"
-Requires-Dist: snowflake-id; extra == "openai"
-Requires-Dist: transformers>=4.34.0; extra == "openai"
-Requires-Dist: aiofiles; extra == "openai"
+Requires-Dist: psutil==5.9.4; extra == "openai"
+Requires-Dist: openai; extra == "openai"
 Requires-Dist: python-docx; extra == "openai"
-Requires-Dist: GitPython; extra == "openai"
 Requires-Dist: chardet==5.1.0; extra == "openai"
-Requires-Dist: langchain>=0.0.286; extra == "openai"
-Requires-Dist: openai; extra == "openai"
-Requires-Dist: gTTS==2.3.1; extra == "openai"
 Requires-Dist: bs4; extra == "openai"
-Requires-Dist: duckdb; extra == "openai"
-Requires-Dist: python-pptx; extra == "openai"
+Requires-Dist: typing_inspect; extra == "openai"
+Requires-Dist: uvicorn; extra == "openai"
+Requires-Dist: pymysql; extra == "openai"
+Requires-Dist: termcolor; extra == "openai"
+Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "openai"
+Requires-Dist: shortuuid; extra == "openai"
+Requires-Dist: gTTS==2.3.1; extra == "openai"
+Requires-Dist: markdown; extra == "openai"
+Requires-Dist: importlib-resources==5.12.0; extra == "openai"
+Requires-Dist: click; extra == "openai"
+Requires-Dist: aiofiles; extra == "openai"
+Requires-Dist: schedule; extra == "openai"
+Requires-Dist: pympler; extra == "openai"
 Requires-Dist: xlrd==2.0.1; extra == "openai"
-Requires-Dist: aiohttp==3.8.4; extra == "openai"
-Requires-Dist: openpyxl==3.1.2; extra == "openai"
+Requires-Dist: duckdb; extra == "openai"
+Requires-Dist: GitPython; extra == "openai"
+Requires-Dist: alembic==1.12.0; extra == "openai"
+Requires-Dist: rich; extra == "openai"
+Requires-Dist: spacy>=3.7; extra == "openai"
+Requires-Dist: python-dotenv==1.0.0; extra == "openai"
+Requires-Dist: duckdb-engine; extra == "openai"
+Requires-Dist: coloredlogs; extra == "openai"
+Requires-Dist: typeguard; extra == "openai"
 Requires-Dist: pydantic>=2.6.0; extra == "openai"
+Requires-Dist: aiohttp==3.8.4; extra == "openai"
+Requires-Dist: fschat; extra == "openai"
+Requires-Dist: python-pptx; extra == "openai"
+Requires-Dist: tomlkit; extra == "openai"
+Requires-Dist: tiktoken; extra == "openai"
+Requires-Dist: seaborn; extra == "openai"
+Requires-Dist: msgpack; extra == "openai"
+Requires-Dist: cachetools; extra == "openai"
+Requires-Dist: httpx; extra == "openai"
 Provides-Extra: gpt4all
 Requires-Dist: gpt4all; extra == "gpt4all"
 Provides-Extra: vllm
 Requires-Dist: vllm; extra == "vllm"
 Provides-Extra: cache
 Requires-Dist: rocksdict; extra == "cache"
 Provides-Extra: default
-Requires-Dist: schedule; extra == "default"
-Requires-Dist: sqlparse==0.4.4; extra == "default"
-Requires-Dist: seaborn; extra == "default"
-Requires-Dist: markdown; extra == "default"
-Requires-Dist: msgpack; extra == "default"
-Requires-Dist: termcolor; extra == "default"
+Requires-Dist: cpm_kernels; extra == "default"
+Requires-Dist: fastapi>=0.100.0; extra == "default"
+Requires-Dist: transformers>=4.34.0; extra == "default"
+Requires-Dist: python-multipart; extra == "default"
 Requires-Dist: sentence-transformers; extra == "default"
-Requires-Dist: alembic==1.12.0; extra == "default"
-Requires-Dist: rich; extra == "default"
-Requires-Dist: ollama; extra == "default"
-Requires-Dist: shortuuid; extra == "default"
 Requires-Dist: pypdf; extra == "default"
+Requires-Dist: auto-gpt-plugin-template; extra == "default"
+Requires-Dist: snowflake-id; extra == "default"
+Requires-Dist: sentencepiece; extra == "default"
+Requires-Dist: colorama==0.4.6; extra == "default"
+Requires-Dist: jsonschema; extra == "default"
 Requires-Dist: chromadb>=0.4.22; extra == "default"
-Requires-Dist: cpm_kernels; extra == "default"
-Requires-Dist: typeguard; extra == "default"
+Requires-Dist: pandas==2.0.3; extra == "default"
 Requires-Dist: jinja2; extra == "default"
-Requires-Dist: python-multipart; extra == "default"
-Requires-Dist: torchvision==0.17.1; extra == "default"
-Requires-Dist: pymysql; extra == "default"
-Requires-Dist: cachetools; extra == "default"
+Requires-Dist: sqlparse==0.4.4; extra == "default"
+Requires-Dist: prettytable; extra == "default"
+Requires-Dist: openpyxl==3.1.2; extra == "default"
+Requires-Dist: graphviz; extra == "default"
 Requires-Dist: psutil==5.9.4; extra == "default"
-Requires-Dist: torch==2.2.1; extra == "default"
-Requires-Dist: torchaudio==2.2.1; extra == "default"
+Requires-Dist: python-docx; extra == "default"
+Requires-Dist: chardet==5.1.0; extra == "default"
+Requires-Dist: bs4; extra == "default"
+Requires-Dist: typing_inspect; extra == "default"
+Requires-Dist: uvicorn; extra == "default"
+Requires-Dist: pymysql; extra == "default"
+Requires-Dist: termcolor; extra == "default"
 Requires-Dist: dashscope; extra == "default"
+Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "default"
+Requires-Dist: ollama; extra == "default"
+Requires-Dist: shortuuid; extra == "default"
+Requires-Dist: gTTS==2.3.1; extra == "default"
 Requires-Dist: importlib-resources==5.12.0; extra == "default"
-Requires-Dist: prettytable; extra == "default"
-Requires-Dist: accelerate>=0.20.3; extra == "default"
-Requires-Dist: fschat; extra == "default"
+Requires-Dist: markdown; extra == "default"
 Requires-Dist: zhipuai; extra == "default"
-Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "default"
-Requires-Dist: graphviz; extra == "default"
-Requires-Dist: rocksdict; extra == "default"
 Requires-Dist: click; extra == "default"
-Requires-Dist: duckdb-engine; extra == "default"
-Requires-Dist: pandas==2.0.3; extra == "default"
-Requires-Dist: fastapi>=0.100.0; extra == "default"
-Requires-Dist: jsonschema; extra == "default"
-Requires-Dist: spacy>=3.7; extra == "default"
+Requires-Dist: rocksdict; extra == "default"
+Requires-Dist: aiofiles; extra == "default"
+Requires-Dist: schedule; extra == "default"
 Requires-Dist: pympler; extra == "default"
-Requires-Dist: tomlkit; extra == "default"
-Requires-Dist: uvicorn; extra == "default"
-Requires-Dist: auto-gpt-plugin-template; extra == "default"
-Requires-Dist: httpx; extra == "default"
+Requires-Dist: xlrd==2.0.1; extra == "default"
+Requires-Dist: accelerate>=0.20.3; extra == "default"
+Requires-Dist: duckdb; extra == "default"
+Requires-Dist: GitPython; extra == "default"
+Requires-Dist: alembic==1.12.0; extra == "default"
+Requires-Dist: rich; extra == "default"
+Requires-Dist: torchvision==0.17.1; extra == "default"
+Requires-Dist: spacy>=3.7; extra == "default"
+Requires-Dist: python-dotenv==1.0.0; extra == "default"
+Requires-Dist: duckdb-engine; extra == "default"
 Requires-Dist: coloredlogs; extra == "default"
+Requires-Dist: torch==2.2.1; extra == "default"
+Requires-Dist: torchaudio==2.2.1; extra == "default"
+Requires-Dist: typeguard; extra == "default"
+Requires-Dist: pydantic>=2.6.0; extra == "default"
+Requires-Dist: aiohttp==3.8.4; extra == "default"
+Requires-Dist: chardet; extra == "default"
+Requires-Dist: fschat; extra == "default"
 Requires-Dist: tokenizers>=0.14; extra == "default"
-Requires-Dist: python-dotenv==1.0.0; extra == "default"
-Requires-Dist: snowflake-id; extra == "default"
-Requires-Dist: colorama==0.4.6; extra == "default"
-Requires-Dist: transformers>=4.34.0; extra == "default"
-Requires-Dist: sentencepiece; extra == "default"
-Requires-Dist: aiofiles; extra == "default"
-Requires-Dist: python-docx; extra == "default"
-Requires-Dist: GitPython; extra == "default"
-Requires-Dist: chardet==5.1.0; extra == "default"
-Requires-Dist: langchain>=0.0.286; extra == "default"
-Requires-Dist: gTTS==2.3.1; extra == "default"
-Requires-Dist: bs4; extra == "default"
-Requires-Dist: duckdb; extra == "default"
 Requires-Dist: python-pptx; extra == "default"
-Requires-Dist: chardet; extra == "default"
-Requires-Dist: xlrd==2.0.1; extra == "default"
-Requires-Dist: aiohttp==3.8.4; extra == "default"
+Requires-Dist: tomlkit; extra == "default"
 Requires-Dist: bitsandbytes; extra == "default"
-Requires-Dist: openpyxl==3.1.2; extra == "default"
-Requires-Dist: pydantic>=2.6.0; extra == "default"
+Requires-Dist: seaborn; extra == "default"
+Requires-Dist: msgpack; extra == "default"
+Requires-Dist: cachetools; extra == "default"
+Requires-Dist: httpx; extra == "default"
 Provides-Extra: all
+Requires-Dist: cpm_kernels; extra == "all"
+Requires-Dist: transformers>=4.34.0; extra == "all"
+Requires-Dist: chromadb>=0.4.22; extra == "all"
+Requires-Dist: pandas==2.0.3; extra == "all"
 Requires-Dist: sqlparse==0.4.4; extra == "all"
-Requires-Dist: markdown; extra == "all"
-Requires-Dist: sentence-transformers; extra == "all"
-Requires-Dist: msgpack; extra == "all"
-Requires-Dist: alembic==1.12.0; extra == "all"
+Requires-Dist: clickhouse-connect; extra == "all"
+Requires-Dist: graphviz; extra == "all"
+Requires-Dist: python-docx; extra == "all"
+Requires-Dist: typing_inspect; extra == "all"
+Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "all"
+Requires-Dist: shortuuid; extra == "all"
+Requires-Dist: schedule; extra == "all"
+Requires-Dist: pympler; extra == "all"
 Requires-Dist: rich; extra == "all"
+Requires-Dist: python-dotenv==1.0.0; extra == "all"
+Requires-Dist: llama-cpp-python; extra == "all"
+Requires-Dist: fschat; extra == "all"
+Requires-Dist: tiktoken; extra == "all"
+Requires-Dist: seaborn; extra == "all"
+Requires-Dist: vertica_python; extra == "all"
+Requires-Dist: cachetools; extra == "all"
+Requires-Dist: GitPython; extra == "all"
+Requires-Dist: sentence-transformers; extra == "all"
+Requires-Dist: python-multipart; extra == "all"
 Requires-Dist: pypdf; extra == "all"
 Requires-Dist: psycopg2; extra == "all"
-Requires-Dist: python-multipart; extra == "all"
-Requires-Dist: importlib-resources==5.12.0; extra == "all"
-Requires-Dist: prettytable; extra == "all"
-Requires-Dist: thrift_sasl; extra == "all"
 Requires-Dist: auto-gpt-plugin-template; extra == "all"
-Requires-Dist: sentencepiece; extra == "all"
-Requires-Dist: GitPython; extra == "all"
-Requires-Dist: gTTS==2.3.1; extra == "all"
-Requires-Dist: clickhouse-connect; extra == "all"
-Requires-Dist: pydantic>=2.6.0; extra == "all"
-Requires-Dist: seaborn; extra == "all"
-Requires-Dist: psutil==5.9.4; extra == "all"
-Requires-Dist: gpt4all; extra == "all"
-Requires-Dist: zhipuai; extra == "all"
-Requires-Dist: click; extra == "all"
-Requires-Dist: pandas==2.0.3; extra == "all"
-Requires-Dist: jsonschema; extra == "all"
-Requires-Dist: vllm; extra == "all"
-Requires-Dist: httpx; extra == "all"
-Requires-Dist: colorama==0.4.6; extra == "all"
 Requires-Dist: snowflake-id; extra == "all"
-Requires-Dist: pyhive; extra == "all"
+Requires-Dist: jsonschema; extra == "all"
+Requires-Dist: jinja2; extra == "all"
+Requires-Dist: prettytable; extra == "all"
+Requires-Dist: thrift; extra == "all"
+Requires-Dist: openai; extra == "all"
 Requires-Dist: chardet==5.1.0; extra == "all"
-Requires-Dist: weaviate-client; extra == "all"
-Requires-Dist: pyspark; extra == "all"
-Requires-Dist: termcolor; extra == "all"
-Requires-Dist: pymilvus; extra == "all"
-Requires-Dist: shortuuid; extra == "all"
-Requires-Dist: cpm_kernels; extra == "all"
-Requires-Dist: neo4j; extra == "all"
-Requires-Dist: typeguard; extra == "all"
-Requires-Dist: torchaudio==2.2.1; extra == "all"
-Requires-Dist: accelerate>=0.20.3; extra == "all"
-Requires-Dist: rocksdict; extra == "all"
-Requires-Dist: spacy>=3.7; extra == "all"
-Requires-Dist: pympler; extra == "all"
-Requires-Dist: tomlkit; extra == "all"
 Requires-Dist: uvicorn; extra == "all"
-Requires-Dist: coloredlogs; extra == "all"
-Requires-Dist: tokenizers>=0.14; extra == "all"
-Requires-Dist: python-dotenv==1.0.0; extra == "all"
-Requires-Dist: duckdb; extra == "all"
+Requires-Dist: pyhive; extra == "all"
+Requires-Dist: dashscope; extra == "all"
+Requires-Dist: markdown; extra == "all"
+Requires-Dist: weaviate-client; extra == "all"
 Requires-Dist: xlrd==2.0.1; extra == "all"
+Requires-Dist: torchvision==0.17.1; extra == "all"
+Requires-Dist: duckdb-engine; extra == "all"
+Requires-Dist: torchaudio==2.2.1; extra == "all"
 Requires-Dist: aiohttp==3.8.4; extra == "all"
+Requires-Dist: chardet; extra == "all"
+Requires-Dist: tomlkit; extra == "all"
+Requires-Dist: bitsandbytes; extra == "all"
+Requires-Dist: sentencepiece; extra == "all"
 Requires-Dist: openpyxl==3.1.2; extra == "all"
-Requires-Dist: schedule; extra == "all"
-Requires-Dist: tiktoken; extra == "all"
+Requires-Dist: pymilvus; extra == "all"
+Requires-Dist: termcolor; extra == "all"
+Requires-Dist: pyspark; extra == "all"
 Requires-Dist: ollama; extra == "all"
-Requires-Dist: chromadb>=0.4.22; extra == "all"
-Requires-Dist: jinja2; extra == "all"
-Requires-Dist: torchvision==0.17.1; extra == "all"
-Requires-Dist: pymysql; extra == "all"
-Requires-Dist: cachetools; extra == "all"
-Requires-Dist: thrift; extra == "all"
-Requires-Dist: torch==2.2.1; extra == "all"
-Requires-Dist: dashscope; extra == "all"
-Requires-Dist: fschat; extra == "all"
-Requires-Dist: graphviz; extra == "all"
-Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "all"
-Requires-Dist: duckdb-engine; extra == "all"
+Requires-Dist: gTTS==2.3.1; extra == "all"
+Requires-Dist: importlib-resources==5.12.0; extra == "all"
+Requires-Dist: click; extra == "all"
+Requires-Dist: aiofiles; extra == "all"
+Requires-Dist: neo4j; extra == "all"
+Requires-Dist: mysqlclient==2.1.0; extra == "all"
+Requires-Dist: alembic==1.12.0; extra == "all"
+Requires-Dist: thrift_sasl; extra == "all"
+Requires-Dist: vllm; extra == "all"
+Requires-Dist: python-pptx; extra == "all"
+Requires-Dist: msgpack; extra == "all"
+Requires-Dist: httpx; extra == "all"
 Requires-Dist: fastapi>=0.100.0; extra == "all"
-Requires-Dist: python-docx; extra == "all"
 Requires-Dist: pymssql; extra == "all"
-Requires-Dist: llama-cpp-python; extra == "all"
-Requires-Dist: transformers>=4.34.0; extra == "all"
-Requires-Dist: aiofiles; extra == "all"
-Requires-Dist: pydoris<2.0.0,>=1.0.2; extra == "all"
-Requires-Dist: langchain>=0.0.286; extra == "all"
-Requires-Dist: openai; extra == "all"
+Requires-Dist: colorama==0.4.6; extra == "all"
+Requires-Dist: psutil==5.9.4; extra == "all"
 Requires-Dist: bs4; extra == "all"
-Requires-Dist: python-pptx; extra == "all"
-Requires-Dist: chardet; extra == "all"
-Requires-Dist: bitsandbytes; extra == "all"
-Requires-Dist: mysqlclient==2.1.0; extra == "all"
+Requires-Dist: pymysql; extra == "all"
+Requires-Dist: zhipuai; extra == "all"
+Requires-Dist: rocksdict; extra == "all"
+Requires-Dist: accelerate>=0.20.3; extra == "all"
+Requires-Dist: duckdb; extra == "all"
+Requires-Dist: gpt4all; extra == "all"
+Requires-Dist: pydoris<2.0.0,>=1.0.2; extra == "all"
+Requires-Dist: spacy>=3.7; extra == "all"
+Requires-Dist: torch==2.2.1; extra == "all"
+Requires-Dist: typeguard; extra == "all"
+Requires-Dist: pydantic>=2.6.0; extra == "all"
+Requires-Dist: tokenizers>=0.14; extra == "all"
+Requires-Dist: coloredlogs; extra == "all"
 
 # DB-GPT: Revolutionizing Database Interactions with Private LLM Technology
  
 <p align="left">
   <img src="./assets/LOGO.png" width="100%" />
 </p>
 
@@ -569,14 +577,18 @@
   We've also developed an automated fine-tuning lightweight framework centred on large language models (LLMs), Text2SQL datasets, LoRA/QLoRA/Pturning, and other fine-tuning methods. This framework simplifies Text-to-SQL fine-tuning, making it as straightforward as an assembly line process. [DB-GPT-Hub](https://github.com/eosphoros-ai/DB-GPT-Hub)
 
 - **SMMF(Service-oriented Multi-model Management Framework)**
 
   We offer extensive model support, including dozens of large language models (LLMs) from both open-source and API agents, such as LLaMA/LLaMA2, Baichuan, ChatGLM, Wenxin, Tongyi, Zhipu, and many more. 
 
   - News
+    - 🔥🔥🔥  [Phi-3](https://huggingface.co/collections/microsoft/phi-3-6626e15e9585a200d2d761e3)
+    - 🔥🔥🔥  [Yi-1.5-34B-Chat](https://huggingface.co/01-ai/Yi-1.5-34B-Chat)
+    - 🔥🔥🔥  [Yi-1.5-9B-Chat](https://huggingface.co/01-ai/Yi-1.5-9B-Chat)
+    - 🔥🔥🔥  [Yi-1.5-6B-Chat](https://huggingface.co/01-ai/Yi-1.5-6B-Chat)
     - 🔥🔥🔥  [Qwen1.5-110B-Chat](https://huggingface.co/Qwen/Qwen1.5-110B-Chat)
     - 🔥🔥🔥  [Qwen1.5-MoE-A2.7B-Chat](https://huggingface.co/Qwen/Qwen1.5-MoE-A2.7B-Chat)
     - 🔥🔥🔥  [Meta-Llama-3-70B-Instruct](https://huggingface.co/meta-llama/Meta-Llama-3-70B-Instruct)
     - 🔥🔥🔥  [Meta-Llama-3-8B-Instruct](https://huggingface.co/meta-llama/Meta-Llama-3-8B-Instruct)
     - 🔥🔥🔥  [CodeQwen1.5-7B-Chat](https://huggingface.co/Qwen/CodeQwen1.5-7B-Chat)
     - 🔥🔥🔥  [Qwen1.5-32B-Chat](https://huggingface.co/Qwen/Qwen1.5-32B-Chat)
     - 🔥🔥🔥  [Starling-LM-7B-beta](https://huggingface.co/Nexusflow/Starling-LM-7B-beta)
```

### Comparing `dbgpt-0.5.6rc0/dbgpt.egg-info/SOURCES.txt` & `dbgpt-0.5.7rc0/dbgpt.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -49,43 +49,41 @@
 dbgpt/agent/core/profile/__init__.py
 dbgpt/agent/core/profile/base.py
 dbgpt/agent/expand/Indicator_assistant_agent.py
 dbgpt/agent/expand/__init__.py
 dbgpt/agent/expand/code_assistant_agent.py
 dbgpt/agent/expand/dashboard_assistant_agent.py
 dbgpt/agent/expand/data_scientist_agent.py
-dbgpt/agent/expand/plugin_assistant_agent.py
 dbgpt/agent/expand/retrieve_summary_assistant_agent.py
 dbgpt/agent/expand/summary_assistant_agent.py
+dbgpt/agent/expand/tool_assistant_agent.py
 dbgpt/agent/expand/actions/__init__.py
 dbgpt/agent/expand/actions/chart_action.py
 dbgpt/agent/expand/actions/code_action.py
 dbgpt/agent/expand/actions/dashboard_action.py
 dbgpt/agent/expand/actions/indicator_action.py
-dbgpt/agent/expand/actions/plugin_action.py
-dbgpt/agent/plugin/__init__.py
-dbgpt/agent/plugin/generator.py
-dbgpt/agent/plugin/loader.py
-dbgpt/agent/plugin/plugins_util.py
-dbgpt/agent/plugin/commands/__init__.py
-dbgpt/agent/plugin/commands/command.py
-dbgpt/agent/plugin/commands/command_manage.py
-dbgpt/agent/plugin/commands/exceptions.py
-dbgpt/agent/plugin/commands/built_in/__init__.py
-dbgpt/agent/plugin/commands/built_in/display_type/__init__.py
-dbgpt/agent/plugin/commands/built_in/display_type/show_chart_gen.py
-dbgpt/agent/plugin/commands/built_in/display_type/show_table_gen.py
-dbgpt/agent/plugin/commands/built_in/display_type/show_text_gen.py
+dbgpt/agent/expand/actions/tool_action.py
+dbgpt/agent/expand/resources/__init__.py
+dbgpt/agent/expand/resources/dbgpt_tool.py
+dbgpt/agent/expand/resources/host_tool.py
+dbgpt/agent/expand/resources/search_tool.py
 dbgpt/agent/resource/__init__.py
-dbgpt/agent/resource/resource_api.py
-dbgpt/agent/resource/resource_db_api.py
-dbgpt/agent/resource/resource_knowledge_api.py
-dbgpt/agent/resource/resource_loader.py
-dbgpt/agent/resource/resource_plugin_api.py
+dbgpt/agent/resource/base.py
+dbgpt/agent/resource/database.py
+dbgpt/agent/resource/knowledge.py
+dbgpt/agent/resource/manage.py
+dbgpt/agent/resource/pack.py
+dbgpt/agent/resource/tool/__init__.py
+dbgpt/agent/resource/tool/base.py
+dbgpt/agent/resource/tool/exceptions.py
+dbgpt/agent/resource/tool/pack.py
+dbgpt/agent/resource/tool/autogpt/__init__.py
+dbgpt/agent/resource/tool/autogpt/plugins_util.py
 dbgpt/agent/util/__init__.py
+dbgpt/agent/util/api_call.py
 dbgpt/agent/util/cmp.py
 dbgpt/agent/util/llm/__init__.py
 dbgpt/agent/util/llm/llm.py
 dbgpt/agent/util/llm/llm_client.py
 dbgpt/agent/util/llm/strategy/__init__.py
 dbgpt/agent/util/llm/strategy/priority.py
 dbgpt/cli/__init__.py
@@ -178,19 +176,24 @@
 dbgpt/datasource/rdbms/conn_duckdb.py
 dbgpt/datasource/rdbms/conn_hive.py
 dbgpt/datasource/rdbms/conn_mssql.py
 dbgpt/datasource/rdbms/conn_mysql.py
 dbgpt/datasource/rdbms/conn_postgresql.py
 dbgpt/datasource/rdbms/conn_sqlite.py
 dbgpt/datasource/rdbms/conn_starrocks.py
+dbgpt/datasource/rdbms/conn_vertica.py
 dbgpt/datasource/rdbms/dialect/__init__.py
 dbgpt/datasource/rdbms/dialect/starrocks/__init__.py
 dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/__init__.py
 dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/datatype.py
 dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/dialect.py
+dbgpt/experimental/__init__.py
+dbgpt/experimental/intent/__init__.py
+dbgpt/experimental/intent/base.py
+dbgpt/experimental/intent/operators.py
 dbgpt/model/__init__.py
 dbgpt/model/base.py
 dbgpt/model/cli.py
 dbgpt/model/parameter.py
 dbgpt/model/adapter/__init__.py
 dbgpt/model/adapter/base.py
 dbgpt/model/adapter/embeddings_loader.py
@@ -207,14 +210,15 @@
 dbgpt/model/proxy/__init__.py
 dbgpt/model/proxy/base.py
 dbgpt/model/proxy/llms/__init__.py
 dbgpt/model/proxy/llms/baichuan.py
 dbgpt/model/proxy/llms/bard.py
 dbgpt/model/proxy/llms/chatgpt.py
 dbgpt/model/proxy/llms/claude.py
+dbgpt/model/proxy/llms/deepseek.py
 dbgpt/model/proxy/llms/gemini.py
 dbgpt/model/proxy/llms/moonshot.py
 dbgpt/model/proxy/llms/ollama.py
 dbgpt/model/proxy/llms/proxy_model.py
 dbgpt/model/proxy/llms/spark.py
 dbgpt/model/proxy/llms/tongyi.py
 dbgpt/model/proxy/llms/wenxin.py
@@ -224,32 +228,37 @@
 dbgpt/model/utils/chatgpt_utils.py
 dbgpt/model/utils/llm_utils.py
 dbgpt/model/utils/token_utils.py
 dbgpt/rag/__init__.py
 dbgpt/rag/chunk_manager.py
 dbgpt/rag/assembler/__init__.py
 dbgpt/rag/assembler/base.py
+dbgpt/rag/assembler/bm25.py
 dbgpt/rag/assembler/db_schema.py
 dbgpt/rag/assembler/embedding.py
 dbgpt/rag/assembler/summary.py
 dbgpt/rag/embedding/__init__.py
 dbgpt/rag/embedding/_wrapped.py
 dbgpt/rag/embedding/embedding_factory.py
 dbgpt/rag/embedding/embeddings.py
+dbgpt/rag/embedding/rerank.py
 dbgpt/rag/evaluation/__init__.py
 dbgpt/rag/evaluation/retriever.py
 dbgpt/rag/extractor/__init__.py
 dbgpt/rag/extractor/base.py
 dbgpt/rag/extractor/summary.py
 dbgpt/rag/graph/__init__.py
+dbgpt/rag/index/__init__.py
+dbgpt/rag/index/base.py
 dbgpt/rag/knowledge/__init__.py
 dbgpt/rag/knowledge/base.py
 dbgpt/rag/knowledge/csv.py
 dbgpt/rag/knowledge/datasource.py
 dbgpt/rag/knowledge/docx.py
+dbgpt/rag/knowledge/excel.py
 dbgpt/rag/knowledge/factory.py
 dbgpt/rag/knowledge/html.py
 dbgpt/rag/knowledge/json.py
 dbgpt/rag/knowledge/markdown.py
 dbgpt/rag/knowledge/pdf.py
 dbgpt/rag/knowledge/pptx.py
 dbgpt/rag/knowledge/string.py
@@ -264,14 +273,15 @@
 dbgpt/rag/operators/knowledge.py
 dbgpt/rag/operators/rerank.py
 dbgpt/rag/operators/rewrite.py
 dbgpt/rag/operators/schema_linking.py
 dbgpt/rag/operators/summary.py
 dbgpt/rag/retriever/__init__.py
 dbgpt/rag/retriever/base.py
+dbgpt/rag/retriever/bm25.py
 dbgpt/rag/retriever/db_schema.py
 dbgpt/rag/retriever/embedding.py
 dbgpt/rag/retriever/rerank.py
 dbgpt/rag/retriever/rewrite.py
 dbgpt/rag/retriever/time_weighted.py
 dbgpt/rag/schemalinker/__init__.py
 dbgpt/rag/schemalinker/base_linker.py
@@ -281,14 +291,22 @@
 dbgpt/rag/summary/db_summary_client.py
 dbgpt/rag/summary/gdbms_db_summary.py
 dbgpt/rag/summary/rdbms_db_summary.py
 dbgpt/rag/text_splitter/__init__.py
 dbgpt/rag/text_splitter/pre_text_splitter.py
 dbgpt/rag/text_splitter/text_splitter.py
 dbgpt/rag/text_splitter/token_splitter.py
+dbgpt/rag/transformer/__init__.py
+dbgpt/rag/transformer/base.py
+dbgpt/rag/transformer/keyword_extractor.py
+dbgpt/rag/transformer/llm_extractor.py
+dbgpt/rag/transformer/text2cypher.py
+dbgpt/rag/transformer/text2gql.py
+dbgpt/rag/transformer/text2vector.py
+dbgpt/rag/transformer/triplet_extractor.py
 dbgpt/storage/__init__.py
 dbgpt/storage/schema.py
 dbgpt/storage/cache/__init__.py
 dbgpt/storage/cache/embedding_cache.py
 dbgpt/storage/cache/llm_cache.py
 dbgpt/storage/cache/manager.py
 dbgpt/storage/cache/operators.py
@@ -296,32 +314,45 @@
 dbgpt/storage/cache/storage/__init__.py
 dbgpt/storage/cache/storage/base.py
 dbgpt/storage/cache/storage/disk/__init__.py
 dbgpt/storage/cache/storage/disk/disk_storage.py
 dbgpt/storage/chat_history/__init__.py
 dbgpt/storage/chat_history/chat_history_db.py
 dbgpt/storage/chat_history/storage_adapter.py
+dbgpt/storage/graph_store/__init__.py
+dbgpt/storage/graph_store/base.py
+dbgpt/storage/graph_store/factory.py
+dbgpt/storage/graph_store/graph.py
+dbgpt/storage/graph_store/memgraph_store.py
+dbgpt/storage/graph_store/neo4j_store.py
+dbgpt/storage/graph_store/tugraph_store.py
+dbgpt/storage/knowledge_graph/__init__.py
+dbgpt/storage/knowledge_graph/base.py
+dbgpt/storage/knowledge_graph/knowledge_graph.py
+dbgpt/storage/knowledge_graph/open_spg.py
 dbgpt/storage/metadata/__init__.py
 dbgpt/storage/metadata/_base_dao.py
 dbgpt/storage/metadata/db_factory.py
 dbgpt/storage/metadata/db_manager.py
 dbgpt/storage/metadata/db_storage.py
 dbgpt/storage/vector_store/__init__.py
 dbgpt/storage/vector_store/base.py
 dbgpt/storage/vector_store/chroma_store.py
 dbgpt/storage/vector_store/connector.py
+dbgpt/storage/vector_store/elastic_store.py
 dbgpt/storage/vector_store/filters.py
 dbgpt/storage/vector_store/milvus_store.py
 dbgpt/storage/vector_store/oceanbase_store.py
 dbgpt/storage/vector_store/pgvector_store.py
 dbgpt/storage/vector_store/weaviate_store.py
 dbgpt/util/__init__.py
 dbgpt/util/_db_migration_utils.py
 dbgpt/util/annotations.py
 dbgpt/util/api_utils.py
+dbgpt/util/cache_utils.py
 dbgpt/util/chat_util.py
 dbgpt/util/code_utils.py
 dbgpt/util/command_utils.py
 dbgpt/util/config_utils.py
 dbgpt/util/custom_data_structure.py
 dbgpt/util/date_utils.py
 dbgpt/util/error_types.py
```

### Comparing `dbgpt-0.5.6rc0/dbgpt.egg-info/requires.txt` & `dbgpt-0.5.7rc0/dbgpt.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -2,415 +2,423 @@
 chardet==5.1.0
 importlib-resources==5.12.0
 python-dotenv==1.0.0
 cachetools
 pydantic>=2.6.0
 typeguard
 snowflake-id
+typing_inspect
 
 [agent]
-pandas==2.0.3
-cachetools
 fastapi>=0.100.0
+snowflake-id
+colorama==0.4.6
+pandas==2.0.3
+prettytable
 psutil==5.9.4
-tomlkit
+chardet==5.1.0
+typing_inspect
 termcolor
-httpx
 importlib-resources==5.12.0
-python-dotenv==1.0.0
-prettytable
-aiohttp==3.8.4
-snowflake-id
-colorama==0.4.6
-rich
 click
-chardet==5.1.0
+rich
+python-dotenv==1.0.0
 typeguard
 pydantic>=2.6.0
+aiohttp==3.8.4
+tomlkit
+cachetools
+httpx
 
 [all]
+cpm_kernels
+transformers>=4.34.0
+chromadb>=0.4.22
+pandas==2.0.3
 sqlparse==0.4.4
-markdown
-sentence-transformers
-msgpack
-alembic==1.12.0
+clickhouse-connect
+graphviz
+python-docx
+typing_inspect
+SQLAlchemy<2.0.29,>=2.0.25
+shortuuid
+schedule
+pympler
 rich
+python-dotenv==1.0.0
+llama-cpp-python
+fschat
+tiktoken
+seaborn
+vertica_python
+cachetools
+GitPython
+sentence-transformers
+python-multipart
 pypdf
 psycopg2
-python-multipart
-importlib-resources==5.12.0
-prettytable
-thrift_sasl
 auto-gpt-plugin-template
-sentencepiece
-GitPython
-gTTS==2.3.1
-clickhouse-connect
-pydantic>=2.6.0
-seaborn
-psutil==5.9.4
-gpt4all
-zhipuai
-click
-pandas==2.0.3
-jsonschema
-vllm
-httpx
-colorama==0.4.6
 snowflake-id
-pyhive
+jsonschema
+jinja2
+prettytable
+thrift
+openai
 chardet==5.1.0
-weaviate-client
-pyspark
-termcolor
-pymilvus
-shortuuid
-cpm_kernels
-neo4j
-typeguard
-torchaudio==2.2.1
-accelerate>=0.20.3
-rocksdict
-spacy>=3.7
-pympler
-tomlkit
 uvicorn
-coloredlogs
-tokenizers>=0.14
-python-dotenv==1.0.0
-duckdb
+pyhive
+dashscope
+markdown
+weaviate-client
 xlrd==2.0.1
+torchvision==0.17.1
+duckdb-engine
+torchaudio==2.2.1
 aiohttp==3.8.4
+chardet
+tomlkit
+bitsandbytes
+sentencepiece
 openpyxl==3.1.2
-schedule
-tiktoken
+pymilvus
+termcolor
+pyspark
 ollama
-chromadb>=0.4.22
-jinja2
-torchvision==0.17.1
-pymysql
-cachetools
-thrift
-torch==2.2.1
-dashscope
-fschat
-graphviz
-SQLAlchemy<2.0.29,>=2.0.25
-duckdb-engine
+gTTS==2.3.1
+importlib-resources==5.12.0
+click
+aiofiles
+neo4j
+mysqlclient==2.1.0
+alembic==1.12.0
+thrift_sasl
+vllm
+python-pptx
+msgpack
+httpx
 fastapi>=0.100.0
-python-docx
 pymssql
-llama-cpp-python
-transformers>=4.34.0
-aiofiles
-pydoris<2.0.0,>=1.0.2
-langchain>=0.0.286
-openai
+colorama==0.4.6
+psutil==5.9.4
 bs4
-python-pptx
-chardet
-bitsandbytes
-mysqlclient==2.1.0
+pymysql
+zhipuai
+rocksdict
+accelerate>=0.20.3
+duckdb
+gpt4all
+pydoris<2.0.0,>=1.0.2
+spacy>=3.7
+torch==2.2.1
+typeguard
+pydantic>=2.6.0
+tokenizers>=0.14
+coloredlogs
 
 [bitsandbytes]
 bitsandbytes
 
 [cache]
 rocksdict
 
 [cli]
-cachetools
 fastapi>=0.100.0
 psutil==5.9.4
+chardet==5.1.0
+typing_inspect
 tomlkit
-httpx
-importlib-resources==5.12.0
-python-dotenv==1.0.0
-prettytable
-aiohttp==3.8.4
+typeguard
+rich
+pydantic>=2.6.0
 snowflake-id
 colorama==0.4.6
-rich
+python-dotenv==1.0.0
+importlib-resources==5.12.0
 click
-chardet==5.1.0
-typeguard
-pydantic>=2.6.0
+prettytable
+aiohttp==3.8.4
+cachetools
+httpx
 
 [client]
-cachetools
 fastapi>=0.100.0
-httpx
-importlib-resources==5.12.0
-python-dotenv==1.0.0
-aiohttp==3.8.4
-snowflake-id
 chardet==5.1.0
+typing_inspect
 typeguard
 pydantic>=2.6.0
-
-[core]
-cachetools
-importlib-resources==5.12.0
+snowflake-id
 python-dotenv==1.0.0
+importlib-resources==5.12.0
 aiohttp==3.8.4
-snowflake-id
+cachetools
+httpx
+
+[core]
 chardet==5.1.0
+typing_inspect
 typeguard
 pydantic>=2.6.0
+snowflake-id
+python-dotenv==1.0.0
+importlib-resources==5.12.0
+aiohttp==3.8.4
+cachetools
 
 [datasource]
 pymysql
 
 [datasource_all]
-pymysql
 thrift
-pymssql
-clickhouse-connect
-thrift_sasl
-pydoris<2.0.0,>=1.0.2
 neo4j
-pyhive
-psycopg2
 mysqlclient==2.1.0
+pymysql
+pymssql
+psycopg2
+pydoris<2.0.0,>=1.0.2
+vertica_python
 pyspark
+pyhive
+thrift_sasl
+clickhouse-connect
 
 [default]
-schedule
-sqlparse==0.4.4
-seaborn
-markdown
-msgpack
-termcolor
+cpm_kernels
+fastapi>=0.100.0
+transformers>=4.34.0
+python-multipart
 sentence-transformers
-alembic==1.12.0
-rich
-ollama
-shortuuid
 pypdf
+auto-gpt-plugin-template
+snowflake-id
+sentencepiece
+colorama==0.4.6
+jsonschema
 chromadb>=0.4.22
-cpm_kernels
-typeguard
+pandas==2.0.3
 jinja2
-python-multipart
-torchvision==0.17.1
-pymysql
-cachetools
+sqlparse==0.4.4
+prettytable
+openpyxl==3.1.2
+graphviz
 psutil==5.9.4
-torch==2.2.1
-torchaudio==2.2.1
+python-docx
+chardet==5.1.0
+bs4
+typing_inspect
+uvicorn
+pymysql
+termcolor
 dashscope
+SQLAlchemy<2.0.29,>=2.0.25
+ollama
+shortuuid
+gTTS==2.3.1
 importlib-resources==5.12.0
-prettytable
-accelerate>=0.20.3
-fschat
+markdown
 zhipuai
-SQLAlchemy<2.0.29,>=2.0.25
-graphviz
-rocksdict
 click
-duckdb-engine
-pandas==2.0.3
-fastapi>=0.100.0
-jsonschema
-spacy>=3.7
+rocksdict
+aiofiles
+schedule
 pympler
-tomlkit
-uvicorn
-auto-gpt-plugin-template
-httpx
+xlrd==2.0.1
+accelerate>=0.20.3
+duckdb
+GitPython
+alembic==1.12.0
+rich
+torchvision==0.17.1
+spacy>=3.7
+python-dotenv==1.0.0
+duckdb-engine
 coloredlogs
+torch==2.2.1
+torchaudio==2.2.1
+typeguard
+pydantic>=2.6.0
+aiohttp==3.8.4
+chardet
+fschat
 tokenizers>=0.14
-python-dotenv==1.0.0
-snowflake-id
-colorama==0.4.6
-transformers>=4.34.0
-sentencepiece
-aiofiles
-python-docx
-GitPython
-chardet==5.1.0
-langchain>=0.0.286
-gTTS==2.3.1
-bs4
-duckdb
 python-pptx
-chardet
-xlrd==2.0.1
-aiohttp==3.8.4
+tomlkit
 bitsandbytes
-openpyxl==3.1.2
-pydantic>=2.6.0
-
-[framework]
-schedule
-sqlparse==0.4.4
 seaborn
 msgpack
-termcolor
-alembic==1.12.0
-rich
-shortuuid
-typeguard
-jinja2
-pymysql
 cachetools
-psutil==5.9.4
-importlib-resources==5.12.0
-prettytable
-fschat
-graphviz
-SQLAlchemy<2.0.29,>=2.0.25
-click
-duckdb-engine
-pandas==2.0.3
+httpx
+
+[framework]
 fastapi>=0.100.0
-jsonschema
-pympler
-tomlkit
-uvicorn
+transformers>=4.34.0
 auto-gpt-plugin-template
-httpx
-coloredlogs
-python-dotenv==1.0.0
-colorama==0.4.6
 snowflake-id
-transformers>=4.34.0
-aiofiles
-GitPython
+jsonschema
+colorama==0.4.6
+pandas==2.0.3
+jinja2
+sqlparse==0.4.4
+prettytable
+openpyxl==3.1.2
+graphviz
+psutil==5.9.4
 chardet==5.1.0
+typing_inspect
+uvicorn
+pymysql
+termcolor
+SQLAlchemy<2.0.29,>=2.0.25
+shortuuid
 gTTS==2.3.1
-duckdb
+importlib-resources==5.12.0
+click
+aiofiles
+schedule
+pympler
 xlrd==2.0.1
-aiohttp==3.8.4
-openpyxl==3.1.2
+duckdb
+GitPython
+alembic==1.12.0
+rich
+python-dotenv==1.0.0
+duckdb-engine
+coloredlogs
+typeguard
 pydantic>=2.6.0
+aiohttp==3.8.4
+fschat
+tomlkit
+seaborn
+msgpack
+cachetools
+httpx
 
 [gpt4all]
 gpt4all
 
 [llama_cpp]
 llama-cpp-python
 
 [openai]
-schedule
-sqlparse==0.4.4
-seaborn
-markdown
-msgpack
-termcolor
+fastapi>=0.100.0
+transformers>=4.34.0
+python-multipart
 sentence-transformers
-tiktoken
-alembic==1.12.0
-rich
-shortuuid
 pypdf
+auto-gpt-plugin-template
+snowflake-id
+jsonschema
+colorama==0.4.6
 chromadb>=0.4.22
-typeguard
+pandas==2.0.3
 jinja2
-python-multipart
-pymysql
-cachetools
-psutil==5.9.4
-importlib-resources==5.12.0
+sqlparse==0.4.4
 prettytable
-fschat
+openpyxl==3.1.2
 graphviz
-SQLAlchemy<2.0.29,>=2.0.25
-click
-duckdb-engine
-pandas==2.0.3
-fastapi>=0.100.0
-jsonschema
-spacy>=3.7
-pympler
-tomlkit
-uvicorn
-auto-gpt-plugin-template
-httpx
-coloredlogs
-python-dotenv==1.0.0
-colorama==0.4.6
-snowflake-id
-transformers>=4.34.0
-aiofiles
+psutil==5.9.4
+openai
 python-docx
-GitPython
 chardet==5.1.0
-langchain>=0.0.286
-openai
-gTTS==2.3.1
 bs4
-duckdb
-python-pptx
+typing_inspect
+uvicorn
+pymysql
+termcolor
+SQLAlchemy<2.0.29,>=2.0.25
+shortuuid
+gTTS==2.3.1
+markdown
+importlib-resources==5.12.0
+click
+aiofiles
+schedule
+pympler
 xlrd==2.0.1
-aiohttp==3.8.4
-openpyxl==3.1.2
+duckdb
+GitPython
+alembic==1.12.0
+rich
+spacy>=3.7
+python-dotenv==1.0.0
+duckdb-engine
+coloredlogs
+typeguard
 pydantic>=2.6.0
+aiohttp==3.8.4
+fschat
+python-pptx
+tomlkit
+tiktoken
+seaborn
+msgpack
+cachetools
+httpx
 
 [quantization]
 cpm_kernels
 bitsandbytes
 
 [rag]
-bs4
-markdown
-spacy>=3.7
 sentence-transformers
-python-pptx
+python-multipart
 python-docx
+bs4
+python-pptx
 pypdf
+spacy>=3.7
 chromadb>=0.4.22
-langchain>=0.0.286
-python-multipart
+markdown
 
 [simple_framework]
-schedule
+fastapi>=0.100.0
+snowflake-id
+colorama==0.4.6
+pandas==2.0.3
+jinja2
 sqlparse==0.4.4
-msgpack
+prettytable
+psutil==5.9.4
+chardet==5.1.0
+typing_inspect
+uvicorn
 termcolor
-rich
+SQLAlchemy<2.0.29,>=2.0.25
 shortuuid
-typeguard
-jinja2
-cachetools
-psutil==5.9.4
 importlib-resources==5.12.0
-prettytable
-fschat
-SQLAlchemy<2.0.29,>=2.0.25
 click
-duckdb-engine
-pandas==2.0.3
-fastapi>=0.100.0
+schedule
 pympler
-tomlkit
-uvicorn
-httpx
-python-dotenv==1.0.0
-colorama==0.4.6
-snowflake-id
-chardet==5.1.0
 duckdb
-aiohttp==3.8.4
+rich
+python-dotenv==1.0.0
+duckdb-engine
+typeguard
 pydantic>=2.6.0
+aiohttp==3.8.4
+fschat
+tomlkit
+msgpack
+cachetools
+httpx
 
 [torch]
-torchvision==0.17.1
-torch==2.2.1
 torchaudio==2.2.1
+torch==2.2.1
+torchvision==0.17.1
 
 [torch_cpu]
-torchvision==0.17.1
-torch==2.2.1
 torchaudio==2.2.1
+torch==2.2.1
+torchvision==0.17.1
 
 [torch_cuda]
-torchvision==0.17.1
-torch==2.2.1
 torchaudio==2.2.1
+torch==2.2.1
+torchvision==0.17.1
 
 [vllm]
 vllm
 
 [vstore]
 chromadb>=0.4.22
```

### Comparing `dbgpt-0.5.6rc0/setup.py` & `dbgpt-0.5.7rc0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 with open("README.md", mode="r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 IS_DEV_MODE = os.getenv("IS_DEV_MODE", "true").lower() == "true"
 # If you modify the version, please modify the version in the following files:
 # dbgpt/_version.py
-DB_GPT_VERSION = os.getenv("DB_GPT_VERSION", "0.5.5")
+DB_GPT_VERSION = os.getenv("DB_GPT_VERSION", "0.5.7")
 
 BUILD_NO_CACHE = os.getenv("BUILD_NO_CACHE", "true").lower() == "true"
 LLAMA_CPP_GPU_ACCELERATION = (
     os.getenv("LLAMA_CPP_GPU_ACCELERATION", "true").lower() == "true"
 )
 BUILD_FROM_SOURCE = os.getenv("BUILD_FROM_SOURCE", "false").lower() == "true"
 BUILD_FROM_SOURCE_URL_FAST_CHAT = os.getenv(
@@ -414,14 +414,15 @@
         "python-dotenv==1.0.0",
         "cachetools",
         "pydantic>=2.6.0",
         # For AWEL type checking
         "typeguard",
         # Snowflake no additional dependencies.
         "snowflake-id",
+        "typing_inspect",
     ]
     # For DB-GPT python client SDK
     setup_spec.extras["client"] = setup_spec.extras["core"] + [
         "httpx",
         "fastapi>=0.100.0",
     ]
     # Simple command line dependencies
@@ -495,15 +496,14 @@
 
 
 def knowledge_requires():
     """
     pip install "dbgpt[rag]"
     """
     setup_spec.extras["rag"] = setup_spec.extras["vstore"] + [
-        "langchain>=0.0.286",
         "spacy>=3.7",
         "markdown",
         "bs4",
         "python-pptx",
         "python-docx",
         "pypdf",
         "python-multipart",
@@ -605,14 +605,15 @@
         # pydoris is too old, we should find a new package to replace it.
         "pydoris>=1.0.2,<2.0.0",
         "clickhouse-connect",
         "pyhive",
         "thrift",
         "thrift_sasl",
         "neo4j",
+        "vertica_python",
     ]
 
 
 def openai_requires():
     """
     pip install "dbgpt[openai]"
     """
@@ -723,14 +724,16 @@
             "dbgpt.client.*",
             "dbgpt.configs",
             "dbgpt.configs.*",
             "dbgpt.core",
             "dbgpt.core.*",
             "dbgpt.datasource",
             "dbgpt.datasource.*",
+            "dbgpt.experimental",
+            "dbgpt.experimental.*",
             "dbgpt.model",
             "dbgpt.model.proxy",
             "dbgpt.model.proxy.*",
             "dbgpt.model.operators",
             "dbgpt.model.operators.*",
             "dbgpt.model.utils",
             "dbgpt.model.utils.*",
```

