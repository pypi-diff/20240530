# Comparing `tmp/qwak_sdk-0.5.8.tar.gz` & `tmp/qwak_sdk-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_sdk-0.5.8.tar", max compression
+gzip compressed data, was "qwak_sdk-0.5.9.tar", max compression
```

## Comparing `qwak_sdk-0.5.8.tar` & `qwak_sdk-0.5.9.tar`

### file list

```diff
@@ -1,320 +1,320 @@
--rw-r--r--   0        0        0      183 2023-06-29 11:31:41.454942 qwak_sdk-0.5.8/README.md
--rw-r--r--   0        0        0     2609 2023-06-29 11:32:31.051346 qwak_sdk-0.5.8/pyproject.toml
--rw-r--r--   0        0        0      134 2023-06-29 11:32:31.051346 qwak_sdk-0.5.8/qwak_sdk/__init__.py
--rw-r--r--   0        0        0     2176 2023-06-29 11:31:41.454942 qwak_sdk-0.5.8/qwak_sdk/cli.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.454942 qwak_sdk-0.5.8/qwak_sdk/commands/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.454942 qwak_sdk-0.5.8/qwak_sdk/commands/admin/__init__.py
--rw-r--r--   0        0        0      327 2023-06-29 11:31:41.454942 qwak_sdk-0.5.8/qwak_sdk/commands/admin/admin_commands_group.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.454942 qwak_sdk-0.5.8/qwak_sdk/commands/admin/apikeys/__init__.py
--rw-r--r--   0        0        0      467 2023-06-29 11:31:41.454942 qwak_sdk-0.5.8/qwak_sdk/commands/admin/apikeys/api_keys_commands_group.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.454942 qwak_sdk-0.5.8/qwak_sdk/commands/admin/apikeys/generate/__init__.py
--rw-r--r--   0        0        0      677 2023-06-29 11:31:41.454942 qwak_sdk-0.5.8/qwak_sdk/commands/admin/apikeys/generate/_logic.py
--rw-r--r--   0        0        0     1393 2023-06-29 11:31:41.454942 qwak_sdk-0.5.8/qwak_sdk/commands/admin/apikeys/generate/ui.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.454942 qwak_sdk-0.5.8/qwak_sdk/commands/admin/apikeys/revoke/__init__.py
--rw-r--r--   0        0        0      796 2023-06-29 11:31:41.454942 qwak_sdk-0.5.8/qwak_sdk/commands/admin/apikeys/revoke/_logic.py
--rw-r--r--   0        0        0      942 2023-06-29 11:31:41.454942 qwak_sdk-0.5.8/qwak_sdk/commands/admin/apikeys/revoke/ui.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.454942 qwak_sdk-0.5.8/qwak_sdk/commands/audience/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.454942 qwak_sdk-0.5.8/qwak_sdk/commands/audience/_logic/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.454942 qwak_sdk-0.5.8/qwak_sdk/commands/audience/_logic/config/__init__.py
--rw-r--r--   0        0        0      367 2023-06-29 11:31:41.454942 qwak_sdk-0.5.8/qwak_sdk/commands/audience/_logic/config/config_base.py
--rw-r--r--   0        0        0      885 2023-06-29 11:31:41.454942 qwak_sdk-0.5.8/qwak_sdk/commands/audience/_logic/config/parser.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.454942 qwak_sdk-0.5.8/qwak_sdk/commands/audience/_logic/config/v1/__init__.py
--rw-r--r--   0        0        0      886 2023-06-29 11:31:41.454942 qwak_sdk-0.5.8/qwak_sdk/commands/audience/_logic/config/v1/audience_config.py
--rw-r--r--   0        0        0     1626 2023-06-29 11:31:41.454942 qwak_sdk-0.5.8/qwak_sdk/commands/audience/_logic/config/v1/conditions_config.py
--rw-r--r--   0        0        0      817 2023-06-29 11:31:41.454942 qwak_sdk-0.5.8/qwak_sdk/commands/audience/_logic/config/v1/config_v1.py
--rw-r--r--   0        0        0      340 2023-06-29 11:31:41.454942 qwak_sdk-0.5.8/qwak_sdk/commands/audience/_logic/config/v1/route_config.py
--rw-r--r--   0        0        0      277 2023-06-29 11:31:41.454942 qwak_sdk-0.5.8/qwak_sdk/commands/audience/_logic/config/v1/spec.py
--rw-r--r--   0        0        0     2631 2023-06-29 11:31:41.454942 qwak_sdk-0.5.8/qwak_sdk/commands/audience/audience_api_dump.py
--rw-r--r--   0        0        0      952 2023-06-29 11:31:41.454942 qwak_sdk-0.5.8/qwak_sdk/commands/audience/audience_commands_group.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.454942 qwak_sdk-0.5.8/qwak_sdk/commands/audience/create/__init__.py
--rw-r--r--   0        0        0     1203 2023-06-29 11:31:41.454942 qwak_sdk-0.5.8/qwak_sdk/commands/audience/create/logic.py
--rw-r--r--   0        0        0      836 2023-06-29 11:31:41.454942 qwak_sdk-0.5.8/qwak_sdk/commands/audience/create/ui.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.454942 qwak_sdk-0.5.8/qwak_sdk/commands/audience/delete/__init__.py
--rw-r--r--   0        0        0      460 2023-06-29 11:31:41.454942 qwak_sdk-0.5.8/qwak_sdk/commands/audience/delete/logic.py
--rw-r--r--   0        0        0      663 2023-06-29 11:31:41.454942 qwak_sdk-0.5.8/qwak_sdk/commands/audience/delete/ui.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.454942 qwak_sdk-0.5.8/qwak_sdk/commands/audience/get/__init__.py
--rw-r--r--   0        0        0      528 2023-06-29 11:31:41.454942 qwak_sdk-0.5.8/qwak_sdk/commands/audience/get/logic.py
--rw-r--r--   0        0        0      933 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/audience/get/ui.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/audience/list/__init__.py
--rw-r--r--   0        0        0      532 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/audience/list/logic.py
--rw-r--r--   0        0        0      702 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/audience/list/ui.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/audience/update/__init__.py
--rw-r--r--   0        0        0     1327 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/audience/update/logic.py
--rw-r--r--   0        0        0      952 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/audience/update/ui.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/auto_scalling/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/auto_scalling/_logic/__init__.py
--rw-r--r--   0        0        0       49 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/auto_scalling/_logic/config/__init__.py
--rw-r--r--   0        0        0     3326 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/auto_scalling/_logic/config/config.py
--rw-r--r--   0        0        0      646 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/auto_scalling/_logic/config/parser.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/auto_scalling/attach/__init__.py
--rw-r--r--   0        0        0     1359 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/auto_scalling/attach/_logic.py
--rw-r--r--   0        0        0      949 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/auto_scalling/attach/ui.py
--rw-r--r--   0        0        0      277 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/auto_scalling/autoscaling_commands_group.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/automations/__init__.py
--rw-r--r--   0        0        0      857 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/automations/automations_commands_group.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/automations/delete/__init__.py
--rw-r--r--   0        0        0      235 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/automations/delete/_logic.py
--rw-r--r--   0        0        0      604 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/automations/delete/ui.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/automations/executions/__init__.py
--rw-r--r--   0        0        0      346 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/automations/executions/executions_commands_group.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/automations/executions/list/__init__.py
--rw-r--r--   0        0        0      330 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/automations/executions/list/_logic.py
--rw-r--r--   0        0        0      669 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/automations/executions/list/ui.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/automations/list/__init__.py
--rw-r--r--   0        0        0      252 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/automations/list/_logic.py
--rw-r--r--   0        0        0      546 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/automations/list/ui.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/automations/register/__init__.py
--rw-r--r--   0        0        0     1624 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/automations/register/_logic.py
--rw-r--r--   0        0        0     1331 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/automations/register/ui.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/feature_store/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/feature_store/delete/__init__.py
--rw-r--r--   0        0        0     1716 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/feature_store/delete/_logic.py
--rw-r--r--   0        0        0     1039 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/feature_store/delete/ui.py
--rw-r--r--   0        0        0     1002 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/feature_store/feature_store_command_group.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/feature_store/list/__init__.py
--rw-r--r--   0        0        0     4145 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/feature_store/list/ui.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/feature_store/pause/__init__.py
--rw-r--r--   0        0        0      695 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/feature_store/pause/ui.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/feature_store/register/__init__.py
--rw-r--r--   0        0        0    10893 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/feature_store/register/_logic.py
--rw-r--r--   0        0        0     2822 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/feature_store/register/ui.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/feature_store/resume/__init__.py
--rw-r--r--   0        0        0      700 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/feature_store/resume/ui.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/feature_store/trigger/__init__.py
--rw-r--r--   0        0        0     1015 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/feature_store/trigger/ui.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/_logic/__init__.py
--rw-r--r--   0        0        0     1497 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/_logic/instance_template.py
--rw-r--r--   0        0        0     2050 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/_logic/variations.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/__init__.py
--rw-r--r--   0        0        0     2003 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/build_steps.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/client_logs/__init__.py
--rw-r--r--   0        0        0     6185 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/client_logs/build_run_handlers.py
--rw-r--r--   0        0        0     4383 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/client_logs/cli_ui.py
--rw-r--r--   0        0        0     2908 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/client_logs/logger.py
--rw-r--r--   0        0        0     1369 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/client_logs/messages.py
--rw-r--r--   0        0        0     1435 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/client_logs/notifier_impl.py
--rw-r--r--   0        0        0      359 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/client_logs/spinner.py
--rw-r--r--   0        0        0      975 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/client_logs/time_source.py
--rw-r--r--   0        0        0      311 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/client_logs/utils.py
--rw-r--r--   0        0        0    10020 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/config/config_v1.py
--rw-r--r--   0        0        0      131 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/constant/host_resource.py
--rw-r--r--   0        0        0      881 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/constant/step_description.py
--rw-r--r--   0        0        0       73 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/constant/temp_dir.py
--rw-r--r--   0        0        0      189 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/constant/upload_tag.py
--rw-r--r--   0        0        0     1911 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/context.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/interface/__init__.py
--rw-r--r--   0        0        0      568 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/interface/notifier_interface.py
--rw-r--r--   0        0        0      745 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/interface/step_inteface.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/__init__.py
--rw-r--r--   0        0        0      421 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/__init__.py
--rw-r--r--   0        0        0     2012 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_model_step.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/__init__.py
--rw-r--r--   0        0        0      957 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/common.py
--rw-r--r--   0        0        0     2007 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/fetch_strategy_manager.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/folder/__init__.py
--rw-r--r--   0        0        0     3721 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/folder/folder_strategy.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/git/__init__.py
--rw-r--r--   0        0        0     4731 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/git/git_strategy.py
--rw-r--r--   0        0        0     2025 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/strategy.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/zip/__init__.py
--rw-r--r--   0        0        0     2232 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/zip/zip_strategy.py
--rw-r--r--   0        0        0     4807 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/post_fetch_validation_step.py
--rw-r--r--   0        0        0     7241 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/pre_fetch_validation_step.py
--rw-r--r--   0        0        0      274 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/__init__.py
--rw-r--r--   0        0        0      611 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/cleanup_step.py
--rw-r--r--   0        0        0     1605 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/start_remote_build_step.py
--rw-r--r--   0        0        0    12278 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/upload_step.py
--rw-r--r--   0        0        0      182 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/c_deploy/__init__.py
--rw-r--r--   0        0        0     2169 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/c_deploy/build_polling_status.py
--rw-r--r--   0        0        0     2249 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/c_deploy/deploy_build.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/util/__init__.py
--rw-r--r--   0        0        0     1686 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/util/protobuf_factory.py
--rw-r--r--   0        0        0     1181 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/util/step_decorator.py
--rw-r--r--   0        0        0      188 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/util/text.py
--rw-r--r--   0        0        0     6701 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/build/ui.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/builds/__init__.py
--rw-r--r--   0        0        0      491 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/builds/builds_commands_group.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/builds/cancel/__init__.py
--rw-r--r--   0        0        0      181 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/builds/cancel/_logic.py
--rw-r--r--   0        0        0      518 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/builds/cancel/ui.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/builds/logs/__init__.py
--rw-r--r--   0        0        0     1054 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/builds/logs/ui.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/builds/status/__init__.py
--rw-r--r--   0        0        0      256 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/builds/status/_logic.py
--rw-r--r--   0        0        0      973 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/builds/status/ui.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/create/__init__.py
--rw-r--r--   0        0        0     1335 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/create/_logic.py
--rw-r--r--   0        0        0     1016 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/create/ui.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/delete/__init__.py
--rw-r--r--   0        0        0      186 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/delete/_logic.py
--rw-r--r--   0        0        0      638 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/delete/ui.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/_logic/__init__.py
--rw-r--r--   0        0        0     1251 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/_logic/advance_deployment_options_handler.py
--rw-r--r--   0        0        0     2652 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/_logic/base_deploy_executor.py
--rw-r--r--   0        0        0     8355 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/_logic/deploy_config.py
--rw-r--r--   0        0        0    13221 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/_logic/deployment.py
--rw-r--r--   0        0        0     4087 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_message_helpers.py
--rw-r--r--   0        0        0     5799 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_response_handler.py
--rw-r--r--   0        0        0     2167 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_size_mapper.py
--rw-r--r--   0        0        0     1067 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/_logic/get_latest_successful_build.py
--rw-r--r--   0        0        0     3166 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/_logic/variations.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/batch/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/batch/_logic/__init__.py
--rw-r--r--   0        0        0      495 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/batch/_logic/advanced_deployment_mapper.py
--rw-r--r--   0        0        0      946 2023-06-29 11:31:41.458942 qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/batch/_logic/deploy_executor.py
--rw-r--r--   0        0        0     3182 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/batch/ui.py
--rw-r--r--   0        0        0      500 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/deploy_commands_group.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/realtime/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/__init__.py
--rw-r--r--   0        0        0      902 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/advanced_deployment_mapper.py
--rw-r--r--   0        0        0      950 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/deploy_executor.py
--rw-r--r--   0        0        0     3621 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/serving_strategy_mapper.py
--rw-r--r--   0        0        0     4714 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/realtime/ui.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/streaming/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/__init__.py
--rw-r--r--   0        0        0      948 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/deploy_executor.py
--rw-r--r--   0        0        0     1500 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/serving_strategy_mapper.py
--rw-r--r--   0        0        0     5548 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/streaming/ui.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/undeploy/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/undeploy/_logic/__init__.py
--rw-r--r--   0        0        0     5773 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/undeploy/_logic/request_undeploy.py
--rw-r--r--   0        0        0     3036 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/undeploy/_logic/variations.py
--rw-r--r--   0        0        0     2083 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/undeploy/ui.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/executions/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/executions/cancel/__init__.py
--rw-r--r--   0        0        0      409 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/executions/cancel/_logic.py
--rw-r--r--   0        0        0      828 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/executions/cancel/ui.py
--rw-r--r--   0        0        0      789 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/executions/execution_commands_group.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/executions/report/__init__.py
--rw-r--r--   0        0        0      533 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/executions/report/_logic.py
--rw-r--r--   0        0        0     1435 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/executions/report/ui.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/executions/start/__init__.py
--rw-r--r--   0        0        0      926 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/executions/start/_logic.py
--rw-r--r--   0        0        0     5328 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/executions/start/ui.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/executions/status/__init__.py
--rw-r--r--   0        0        0      480 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/executions/status/_logic.py
--rw-r--r--   0        0        0      820 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/executions/status/ui.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/__init__.py
--rw-r--r--   0        0        0     1375 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/initialize_model_structure.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/churn/__init__.py
--rw-r--r--   0        0        0       35 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/churn/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/__init__.py
--rw-r--r--   0        0        0       84 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/__init__.py
--rw-r--r--   0        0        0      164 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/conda.yml
--rw-r--r--   0        0        0   129370 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/data.csv
--rw-r--r--   0        0        0     3640 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/model.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/it/__init__.py
--rw-r--r--   0        0        0     1030 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/it/test_churn.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/credit_risk/__init__.py
--rw-r--r--   0        0        0       41 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/credit_risk/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/__init__.py
--rw-r--r--   0        0        0       74 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/__init__.py
--rw-r--r--   0        0        0      161 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/conda.yml
--rw-r--r--   0        0        0    53393 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/data.csv
--rw-r--r--   0        0        0     3994 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/model.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/general/__init__.py
--rw-r--r--   0        0        0      139 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/general/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/__init__.py
--rw-r--r--   0        0        0      120 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/__init__.py
--rw-r--r--   0        0        0      140 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/conda.yml
--rw-r--r--   0        0        0     2169 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/model.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.test_directory}}/__init__.py
--rw-r--r--   0        0        0      117 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.test_directory}}/test_qwak_model.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/titanic/__init__.py
--rw-r--r--   0        0        0       61 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/titanic/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/__init__.py
--rw-r--r--   0        0        0      104 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/__init__.py
--rw-r--r--   0        0        0      182 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/conda.yml
--rw-r--r--   0        0        0     3353 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/model.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/it/__init__.py
--rw-r--r--   0        0        0      751 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/it/test_titanic.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/__init__.py
--rw-r--r--   0        0        0       68 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/__init__.py
--rw-r--r--   0        0        0      104 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/__init__.py
--rw-r--r--   0        0        0     3353 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/model.py
--rw-r--r--   0        0        0      448 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/it/__init__.py
--rw-r--r--   0        0        0      752 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/it/test_titanic.py
--rw-r--r--   0        0        0     1906 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/init/ui.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/list/__init__.py
--rw-r--r--   0        0        0      166 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/list/_logic.py
--rw-r--r--   0        0        0     1135 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/list/ui.py
--rw-r--r--   0        0        0     1241 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/models_command_group.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/runtime/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/runtime/feedback/__init__.py
--rw-r--r--   0        0        0     2678 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/runtime/feedback/_logic.py
--rw-r--r--   0        0        0     1378 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/runtime/feedback/ui.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/runtime/logs/__init__.py
--rw-r--r--   0        0        0     1577 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/runtime/logs/ui.py
--rw-r--r--   0        0        0      693 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/runtime/runtime_commands_group.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/runtime/traffic_update/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/runtime/traffic_update/_logic/__init__.py
--rw-r--r--   0        0        0     1811 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/runtime/traffic_update/_logic/execute_runtime_update_traffic.py
--rw-r--r--   0        0        0     3160 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/runtime/traffic_update/_logic/variations.py
--rw-r--r--   0        0        0     1212 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/runtime/traffic_update/ui.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/runtime/update/__init__.py
--rw-r--r--   0        0        0      393 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/runtime/update/_logic.py
--rw-r--r--   0        0        0      622 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/models/runtime/update/ui.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/projects/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/projects/create/__init__.py
--rw-r--r--   0        0        0      259 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/projects/create/_logic.py
--rw-r--r--   0        0        0      691 2023-06-29 11:31:41.462942 qwak_sdk-0.5.8/qwak_sdk/commands/projects/create/ui.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/commands/projects/delete/__init__.py
--rw-r--r--   0        0        0      203 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/commands/projects/delete/_logic.py
--rw-r--r--   0        0        0      557 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/commands/projects/delete/ui.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/commands/projects/list/__init__.py
--rw-r--r--   0        0        0      182 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/commands/projects/list/_logic.py
--rw-r--r--   0        0        0     1124 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/commands/projects/list/ui.py
--rw-r--r--   0        0        0      589 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/commands/projects/projects_command_group.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/commands/secrets/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/commands/secrets/delete/__init__.py
--rw-r--r--   0        0        0      141 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/commands/secrets/delete/_logic.py
--rw-r--r--   0        0        0      741 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/commands/secrets/delete/ui.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/commands/secrets/get/__init__.py
--rw-r--r--   0        0        0      142 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/commands/secrets/get/_logic.py
--rw-r--r--   0        0        0      574 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/commands/secrets/get/ui.py
--rw-r--r--   0        0        0      502 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/commands/secrets/secrets_commands_group.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/commands/secrets/set/__init__.py
--rw-r--r--   0        0        0      149 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/commands/secrets/set/_logic.py
--rw-r--r--   0        0        0      615 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/commands/secrets/set/ui.py
--rw-r--r--   0        0        0      430 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/commands/ui_tools.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/common/__init__.py
--rw-r--r--   0        0        0      437 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/common/run_config/__init__.py
--rw-r--r--   0        0        0     3166 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/common/run_config/base.py
--rw-r--r--   0        0        0     6087 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/common/run_config/utils.py
--rw-r--r--   0        0        0      381 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/exceptions/__init__.py
--rw-r--r--   0        0        0       48 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/exceptions/qwak_command_exception.py
--rw-r--r--   0        0        0      133 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/exceptions/qwak_deploy_new_build_failed.py
--rw-r--r--   0        0        0      424 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/exceptions/qwak_general_build_exception.py
--rw-r--r--   0        0        0      130 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/exceptions/qwak_remote_build_failed.py
--rw-r--r--   0        0        0       48 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/exceptions/qwak_resource_not_found.py
--rw-r--r--   0        0        0      746 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/exceptions/qwak_suggestion_exception.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/inner/__init__.py
--rw-r--r--   0        0        0     3164 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/inner/file_registry.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/inner/tools/__init__.py
--rw-r--r--   0        0        0     4541 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/inner/tools/cli_tools.py
--rw-r--r--   0        0        0      763 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/inner/tools/config_handler.py
--rw-r--r--   0        0        0       71 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/inner/tools/logger/__init__.py
--rw-r--r--   0        0        0     8869 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/inner/tools/logger/logger.py
--rw-r--r--   0        0        0     1941 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/inner/tools/logger/logging.yml
--rw-r--r--   0        0        0     1013 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/inner/tools/tracking.py
--rw-r--r--   0        0        0      136 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/main.py
--rw-r--r--   0        0        0        0 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/tools/__init__.py
--rw-r--r--   0        0        0      287 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/tools/colors.py
--rw-r--r--   0        0        0     2257 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/tools/files.py
--rw-r--r--   0        0        0     5616 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/tools/log_handling.py
--rw-r--r--   0        0        0     1168 2023-06-29 11:31:41.466942 qwak_sdk-0.5.8/qwak_sdk/tools/utils.py
--rw-r--r--   0        0        0     8513 1970-01-01 00:00:00.000000 qwak_sdk-0.5.8/setup.py
--rw-r--r--   0        0        0     1912 1970-01-01 00:00:00.000000 qwak_sdk-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0      183 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/README.md
+-rw-r--r--   0        0        0     2610 2023-07-01 07:34:50.417823 qwak_sdk-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0      134 2023-07-01 07:34:50.417823 qwak_sdk-0.5.9/qwak_sdk/__init__.py
+-rw-r--r--   0        0        0     2176 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/cli.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/admin/__init__.py
+-rw-r--r--   0        0        0      327 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/admin/admin_commands_group.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/admin/apikeys/__init__.py
+-rw-r--r--   0        0        0      467 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/admin/apikeys/api_keys_commands_group.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/admin/apikeys/generate/__init__.py
+-rw-r--r--   0        0        0      677 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/admin/apikeys/generate/_logic.py
+-rw-r--r--   0        0        0     1393 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/admin/apikeys/generate/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/admin/apikeys/revoke/__init__.py
+-rw-r--r--   0        0        0      796 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/admin/apikeys/revoke/_logic.py
+-rw-r--r--   0        0        0      942 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/admin/apikeys/revoke/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/audience/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/audience/_logic/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/audience/_logic/config/__init__.py
+-rw-r--r--   0        0        0      367 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/audience/_logic/config/config_base.py
+-rw-r--r--   0        0        0      885 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/audience/_logic/config/parser.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/audience/_logic/config/v1/__init__.py
+-rw-r--r--   0        0        0      886 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/audience/_logic/config/v1/audience_config.py
+-rw-r--r--   0        0        0     1626 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/audience/_logic/config/v1/conditions_config.py
+-rw-r--r--   0        0        0      817 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/audience/_logic/config/v1/config_v1.py
+-rw-r--r--   0        0        0      340 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/audience/_logic/config/v1/route_config.py
+-rw-r--r--   0        0        0      277 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/audience/_logic/config/v1/spec.py
+-rw-r--r--   0        0        0     2631 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/audience/audience_api_dump.py
+-rw-r--r--   0        0        0      952 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/audience/audience_commands_group.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/audience/create/__init__.py
+-rw-r--r--   0        0        0     1203 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/audience/create/logic.py
+-rw-r--r--   0        0        0      836 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/audience/create/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/audience/delete/__init__.py
+-rw-r--r--   0        0        0      460 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/audience/delete/logic.py
+-rw-r--r--   0        0        0      663 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/audience/delete/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/audience/get/__init__.py
+-rw-r--r--   0        0        0      528 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/audience/get/logic.py
+-rw-r--r--   0        0        0      933 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/audience/get/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/audience/list/__init__.py
+-rw-r--r--   0        0        0      532 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/audience/list/logic.py
+-rw-r--r--   0        0        0      702 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/audience/list/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/audience/update/__init__.py
+-rw-r--r--   0        0        0     1327 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/audience/update/logic.py
+-rw-r--r--   0        0        0      952 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/audience/update/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/auto_scalling/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/auto_scalling/_logic/__init__.py
+-rw-r--r--   0        0        0       49 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/auto_scalling/_logic/config/__init__.py
+-rw-r--r--   0        0        0     3326 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/auto_scalling/_logic/config/config.py
+-rw-r--r--   0        0        0      646 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/auto_scalling/_logic/config/parser.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/auto_scalling/attach/__init__.py
+-rw-r--r--   0        0        0     1359 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/auto_scalling/attach/_logic.py
+-rw-r--r--   0        0        0      949 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/auto_scalling/attach/ui.py
+-rw-r--r--   0        0        0      277 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/auto_scalling/autoscaling_commands_group.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/automations/__init__.py
+-rw-r--r--   0        0        0      857 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/automations/automations_commands_group.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/automations/delete/__init__.py
+-rw-r--r--   0        0        0      235 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/automations/delete/_logic.py
+-rw-r--r--   0        0        0      604 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/automations/delete/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/automations/executions/__init__.py
+-rw-r--r--   0        0        0      346 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/automations/executions/executions_commands_group.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/automations/executions/list/__init__.py
+-rw-r--r--   0        0        0      330 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/automations/executions/list/_logic.py
+-rw-r--r--   0        0        0      669 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/automations/executions/list/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/automations/list/__init__.py
+-rw-r--r--   0        0        0      252 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/automations/list/_logic.py
+-rw-r--r--   0        0        0      546 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/automations/list/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/automations/register/__init__.py
+-rw-r--r--   0        0        0     1624 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/automations/register/_logic.py
+-rw-r--r--   0        0        0     1331 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/automations/register/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/feature_store/delete/__init__.py
+-rw-r--r--   0        0        0     1716 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/feature_store/delete/_logic.py
+-rw-r--r--   0        0        0     1039 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/feature_store/delete/ui.py
+-rw-r--r--   0        0        0     1002 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/feature_store/feature_store_command_group.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/feature_store/list/__init__.py
+-rw-r--r--   0        0        0     4145 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/feature_store/list/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/feature_store/pause/__init__.py
+-rw-r--r--   0        0        0      695 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/feature_store/pause/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/feature_store/register/__init__.py
+-rw-r--r--   0        0        0    10893 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/feature_store/register/_logic.py
+-rw-r--r--   0        0        0     2822 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/feature_store/register/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/feature_store/resume/__init__.py
+-rw-r--r--   0        0        0      700 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/feature_store/resume/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/feature_store/trigger/__init__.py
+-rw-r--r--   0        0        0     1015 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/feature_store/trigger/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/models/_logic/__init__.py
+-rw-r--r--   0        0        0     1497 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/models/_logic/instance_template.py
+-rw-r--r--   0        0        0     2050 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/models/_logic/variations.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/__init__.py
+-rw-r--r--   0        0        0     2003 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/build_steps.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/client_logs/__init__.py
+-rw-r--r--   0        0        0     6185 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/client_logs/build_run_handlers.py
+-rw-r--r--   0        0        0     4383 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/client_logs/cli_ui.py
+-rw-r--r--   0        0        0     2908 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/client_logs/logger.py
+-rw-r--r--   0        0        0     1369 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/client_logs/messages.py
+-rw-r--r--   0        0        0     1435 2023-07-01 07:33:58.925433 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/client_logs/notifier_impl.py
+-rw-r--r--   0        0        0      359 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/client_logs/spinner.py
+-rw-r--r--   0        0        0      975 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/client_logs/time_source.py
+-rw-r--r--   0        0        0      311 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/client_logs/utils.py
+-rw-r--r--   0        0        0    10020 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/config/config_v1.py
+-rw-r--r--   0        0        0      131 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/constant/host_resource.py
+-rw-r--r--   0        0        0      881 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/constant/step_description.py
+-rw-r--r--   0        0        0       73 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/constant/temp_dir.py
+-rw-r--r--   0        0        0      189 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/constant/upload_tag.py
+-rw-r--r--   0        0        0     1911 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/context.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/interface/__init__.py
+-rw-r--r--   0        0        0      568 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/interface/notifier_interface.py
+-rw-r--r--   0        0        0      745 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/interface/step_inteface.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/__init__.py
+-rw-r--r--   0        0        0      421 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/__init__.py
+-rw-r--r--   0        0        0     2012 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_model_step.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/__init__.py
+-rw-r--r--   0        0        0      957 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/common.py
+-rw-r--r--   0        0        0     2007 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/fetch_strategy_manager.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/folder/__init__.py
+-rw-r--r--   0        0        0     3721 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/folder/folder_strategy.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/git/__init__.py
+-rw-r--r--   0        0        0     4731 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/git/git_strategy.py
+-rw-r--r--   0        0        0     2025 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/strategy.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/zip/__init__.py
+-rw-r--r--   0        0        0     2232 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/zip/zip_strategy.py
+-rw-r--r--   0        0        0     4807 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/post_fetch_validation_step.py
+-rw-r--r--   0        0        0     7241 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/pre_fetch_validation_step.py
+-rw-r--r--   0        0        0      274 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/__init__.py
+-rw-r--r--   0        0        0      611 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/cleanup_step.py
+-rw-r--r--   0        0        0     1605 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/start_remote_build_step.py
+-rw-r--r--   0        0        0    12278 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/upload_step.py
+-rw-r--r--   0        0        0      182 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/c_deploy/__init__.py
+-rw-r--r--   0        0        0     2169 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/c_deploy/build_polling_status.py
+-rw-r--r--   0        0        0     2249 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/c_deploy/deploy_build.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/util/__init__.py
+-rw-r--r--   0        0        0     1686 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/util/protobuf_factory.py
+-rw-r--r--   0        0        0     1181 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/util/step_decorator.py
+-rw-r--r--   0        0        0      188 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/util/text.py
+-rw-r--r--   0        0        0     6701 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/build/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/builds/__init__.py
+-rw-r--r--   0        0        0      491 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/builds/builds_commands_group.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/builds/cancel/__init__.py
+-rw-r--r--   0        0        0      181 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/builds/cancel/_logic.py
+-rw-r--r--   0        0        0      518 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/builds/cancel/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/builds/logs/__init__.py
+-rw-r--r--   0        0        0     1054 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/builds/logs/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/builds/status/__init__.py
+-rw-r--r--   0        0        0      256 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/builds/status/_logic.py
+-rw-r--r--   0        0        0      973 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/builds/status/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/create/__init__.py
+-rw-r--r--   0        0        0     1335 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/create/_logic.py
+-rw-r--r--   0        0        0     1016 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/create/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/delete/__init__.py
+-rw-r--r--   0        0        0      186 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/delete/_logic.py
+-rw-r--r--   0        0        0      638 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/delete/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/_logic/__init__.py
+-rw-r--r--   0        0        0     1251 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/_logic/advance_deployment_options_handler.py
+-rw-r--r--   0        0        0     2652 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/_logic/base_deploy_executor.py
+-rw-r--r--   0        0        0     8355 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/_logic/deploy_config.py
+-rw-r--r--   0        0        0    13221 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/_logic/deployment.py
+-rw-r--r--   0        0        0     4087 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_message_helpers.py
+-rw-r--r--   0        0        0     5799 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_response_handler.py
+-rw-r--r--   0        0        0     2167 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_size_mapper.py
+-rw-r--r--   0        0        0     1067 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/_logic/get_latest_successful_build.py
+-rw-r--r--   0        0        0     3166 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/_logic/variations.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/batch/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/batch/_logic/__init__.py
+-rw-r--r--   0        0        0      495 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/batch/_logic/advanced_deployment_mapper.py
+-rw-r--r--   0        0        0      946 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/batch/_logic/deploy_executor.py
+-rw-r--r--   0        0        0     3182 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/batch/ui.py
+-rw-r--r--   0        0        0      500 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/deploy_commands_group.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/realtime/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/__init__.py
+-rw-r--r--   0        0        0      902 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/advanced_deployment_mapper.py
+-rw-r--r--   0        0        0      950 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/deploy_executor.py
+-rw-r--r--   0        0        0     3621 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/serving_strategy_mapper.py
+-rw-r--r--   0        0        0     4714 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/realtime/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/streaming/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/__init__.py
+-rw-r--r--   0        0        0      948 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/deploy_executor.py
+-rw-r--r--   0        0        0     1500 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/serving_strategy_mapper.py
+-rw-r--r--   0        0        0     5548 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/streaming/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/undeploy/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/undeploy/_logic/__init__.py
+-rw-r--r--   0        0        0     5773 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/undeploy/_logic/request_undeploy.py
+-rw-r--r--   0        0        0     3036 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/undeploy/_logic/variations.py
+-rw-r--r--   0        0        0     2083 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/undeploy/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/executions/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/executions/cancel/__init__.py
+-rw-r--r--   0        0        0      409 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/executions/cancel/_logic.py
+-rw-r--r--   0        0        0      828 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/executions/cancel/ui.py
+-rw-r--r--   0        0        0      789 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/executions/execution_commands_group.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/executions/report/__init__.py
+-rw-r--r--   0        0        0      533 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/executions/report/_logic.py
+-rw-r--r--   0        0        0     1435 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/executions/report/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/executions/start/__init__.py
+-rw-r--r--   0        0        0      926 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/executions/start/_logic.py
+-rw-r--r--   0        0        0     5328 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/executions/start/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/executions/status/__init__.py
+-rw-r--r--   0        0        0      480 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/executions/status/_logic.py
+-rw-r--r--   0        0        0      820 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/executions/status/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/__init__.py
+-rw-r--r--   0        0        0     1375 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/initialize_model_structure.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/churn/__init__.py
+-rw-r--r--   0        0        0       35 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/churn/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/__init__.py
+-rw-r--r--   0        0        0       84 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/__init__.py
+-rw-r--r--   0        0        0      164 2023-07-01 07:33:58.929432 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/conda.yml
+-rw-r--r--   0        0        0   129370 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/data.csv
+-rw-r--r--   0        0        0     3640 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/model.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/it/__init__.py
+-rw-r--r--   0        0        0     1030 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/it/test_churn.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/credit_risk/__init__.py
+-rw-r--r--   0        0        0       41 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/credit_risk/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/__init__.py
+-rw-r--r--   0        0        0       74 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/__init__.py
+-rw-r--r--   0        0        0      161 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/conda.yml
+-rw-r--r--   0        0        0    53393 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/data.csv
+-rw-r--r--   0        0        0     3994 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/model.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/general/__init__.py
+-rw-r--r--   0        0        0      139 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/general/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/__init__.py
+-rw-r--r--   0        0        0      120 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/__init__.py
+-rw-r--r--   0        0        0      140 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/conda.yml
+-rw-r--r--   0        0        0     2169 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/model.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.test_directory}}/__init__.py
+-rw-r--r--   0        0        0      117 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.test_directory}}/test_qwak_model.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/titanic/__init__.py
+-rw-r--r--   0        0        0       61 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/titanic/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/__init__.py
+-rw-r--r--   0        0        0      104 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/__init__.py
+-rw-r--r--   0        0        0      182 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/conda.yml
+-rw-r--r--   0        0        0     3353 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/model.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/it/__init__.py
+-rw-r--r--   0        0        0      751 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/it/test_titanic.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/__init__.py
+-rw-r--r--   0        0        0       68 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/__init__.py
+-rw-r--r--   0        0        0      104 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/__init__.py
+-rw-r--r--   0        0        0     3353 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/model.py
+-rw-r--r--   0        0        0      448 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/it/__init__.py
+-rw-r--r--   0        0        0      752 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/it/test_titanic.py
+-rw-r--r--   0        0        0     1906 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/init/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/list/__init__.py
+-rw-r--r--   0        0        0      166 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/list/_logic.py
+-rw-r--r--   0        0        0     1135 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/list/ui.py
+-rw-r--r--   0        0        0     1241 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/models_command_group.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/runtime/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/runtime/feedback/__init__.py
+-rw-r--r--   0        0        0     2678 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/runtime/feedback/_logic.py
+-rw-r--r--   0        0        0     1378 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/runtime/feedback/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/runtime/logs/__init__.py
+-rw-r--r--   0        0        0     1577 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/runtime/logs/ui.py
+-rw-r--r--   0        0        0      693 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/runtime/runtime_commands_group.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/runtime/traffic_update/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/runtime/traffic_update/_logic/__init__.py
+-rw-r--r--   0        0        0     1811 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/runtime/traffic_update/_logic/execute_runtime_update_traffic.py
+-rw-r--r--   0        0        0     3160 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/runtime/traffic_update/_logic/variations.py
+-rw-r--r--   0        0        0     1212 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/runtime/traffic_update/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/runtime/update/__init__.py
+-rw-r--r--   0        0        0      393 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/runtime/update/_logic.py
+-rw-r--r--   0        0        0      622 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/models/runtime/update/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/projects/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/projects/create/__init__.py
+-rw-r--r--   0        0        0      259 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/projects/create/_logic.py
+-rw-r--r--   0        0        0      691 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/projects/create/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/projects/delete/__init__.py
+-rw-r--r--   0        0        0      203 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/projects/delete/_logic.py
+-rw-r--r--   0        0        0      557 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/projects/delete/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/projects/list/__init__.py
+-rw-r--r--   0        0        0      182 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/projects/list/_logic.py
+-rw-r--r--   0        0        0     1124 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/projects/list/ui.py
+-rw-r--r--   0        0        0      589 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/projects/projects_command_group.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/secrets/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/secrets/delete/__init__.py
+-rw-r--r--   0        0        0      141 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/secrets/delete/_logic.py
+-rw-r--r--   0        0        0      741 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/secrets/delete/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/secrets/get/__init__.py
+-rw-r--r--   0        0        0      142 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/secrets/get/_logic.py
+-rw-r--r--   0        0        0      574 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/secrets/get/ui.py
+-rw-r--r--   0        0        0      502 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/secrets/secrets_commands_group.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/secrets/set/__init__.py
+-rw-r--r--   0        0        0      149 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/secrets/set/_logic.py
+-rw-r--r--   0        0        0      615 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/secrets/set/ui.py
+-rw-r--r--   0        0        0      430 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/commands/ui_tools.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/common/__init__.py
+-rw-r--r--   0        0        0      437 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/common/run_config/__init__.py
+-rw-r--r--   0        0        0     3166 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/common/run_config/base.py
+-rw-r--r--   0        0        0     6087 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/common/run_config/utils.py
+-rw-r--r--   0        0        0      381 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/exceptions/__init__.py
+-rw-r--r--   0        0        0       48 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/exceptions/qwak_command_exception.py
+-rw-r--r--   0        0        0      133 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/exceptions/qwak_deploy_new_build_failed.py
+-rw-r--r--   0        0        0      424 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/exceptions/qwak_general_build_exception.py
+-rw-r--r--   0        0        0      130 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/exceptions/qwak_remote_build_failed.py
+-rw-r--r--   0        0        0       48 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/exceptions/qwak_resource_not_found.py
+-rw-r--r--   0        0        0      746 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/exceptions/qwak_suggestion_exception.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/inner/__init__.py
+-rw-r--r--   0        0        0     3164 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/inner/file_registry.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/inner/tools/__init__.py
+-rw-r--r--   0        0        0     4541 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/inner/tools/cli_tools.py
+-rw-r--r--   0        0        0      763 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/inner/tools/config_handler.py
+-rw-r--r--   0        0        0       71 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/inner/tools/logger/__init__.py
+-rw-r--r--   0        0        0     8869 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/inner/tools/logger/logger.py
+-rw-r--r--   0        0        0     1941 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/inner/tools/logger/logging.yml
+-rw-r--r--   0        0        0     1013 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/inner/tools/tracking.py
+-rw-r--r--   0        0        0      136 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/main.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/tools/__init__.py
+-rw-r--r--   0        0        0      287 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/tools/colors.py
+-rw-r--r--   0        0        0     2257 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/tools/files.py
+-rw-r--r--   0        0        0     5616 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/tools/log_handling.py
+-rw-r--r--   0        0        0     1168 2023-07-01 07:33:58.933433 qwak_sdk-0.5.9/qwak_sdk/tools/utils.py
+-rw-r--r--   0        0        0     8515 1970-01-01 00:00:00.000000 qwak_sdk-0.5.9/setup.py
+-rw-r--r--   0        0        0     1917 1970-01-01 00:00:00.000000 qwak_sdk-0.5.9/PKG-INFO
```

### Comparing `qwak_sdk-0.5.8/pyproject.toml` & `qwak_sdk-0.5.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-sdk"
-version = "0.5.8"
+version = "0.5.9"
 description = "Qwak SDK and CLI for qwak models"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     {include = "qwak_sdk"},
 ]
@@ -27,15 +27,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.7.1,<3.10"
 qwak-core = "==0.0.113"
 qwak-inference = "==0.1.4"
 tabulate = ">=0.8.0"
 python-json-logger = ">=2.0.2"
-pydantic = "*"
+pydantic = "<2"
 yaspin = ">=2.0.0"
 assertpy = "^1.1"
 cookiecutter = "*"
 gitpython = ">=2.1.0"
 boto3 = { version="^1.24.116", optional=true } # Inference dependencies
 pandas = [ # Inference dependencies
     {version="<1.4", python=">=3.7.1,<3.8", optional=true},
```

### Comparing `qwak_sdk-0.5.8/qwak_sdk/cli.py` & `qwak_sdk-0.5.9/qwak_sdk/cli.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/admin/apikeys/generate/_logic.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/admin/apikeys/generate/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/admin/apikeys/generate/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/admin/apikeys/generate/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/admin/apikeys/revoke/_logic.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/admin/apikeys/revoke/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/admin/apikeys/revoke/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/admin/apikeys/revoke/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/audience/_logic/config/parser.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/audience/_logic/config/parser.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/audience/_logic/config/v1/audience_config.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/audience/_logic/config/v1/audience_config.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/audience/_logic/config/v1/conditions_config.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/audience/_logic/config/v1/conditions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/audience/_logic/config/v1/config_v1.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/audience/_logic/config/v1/config_v1.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/audience/audience_api_dump.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/audience/audience_api_dump.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/audience/audience_commands_group.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/audience/audience_commands_group.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/audience/create/logic.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/audience/create/logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/audience/create/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/audience/create/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/audience/delete/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/audience/delete/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/audience/get/logic.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/audience/get/logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/audience/get/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/audience/get/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/audience/list/logic.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/audience/list/logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/audience/list/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/audience/list/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/audience/update/logic.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/audience/update/logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/audience/update/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/audience/update/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/auto_scalling/_logic/config/config.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/auto_scalling/_logic/config/config.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/auto_scalling/_logic/config/parser.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/auto_scalling/_logic/config/parser.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/auto_scalling/attach/_logic.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/auto_scalling/attach/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/auto_scalling/attach/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/auto_scalling/attach/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/automations/automations_commands_group.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/automations/automations_commands_group.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/automations/delete/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/automations/delete/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/automations/executions/list/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/automations/executions/list/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/automations/list/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/automations/list/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/automations/register/_logic.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/automations/register/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/automations/register/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/automations/register/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/feature_store/delete/_logic.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/feature_store/delete/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/feature_store/delete/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/feature_store/delete/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/feature_store/feature_store_command_group.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/feature_store/feature_store_command_group.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/feature_store/list/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/feature_store/list/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/feature_store/pause/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/feature_store/pause/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/feature_store/register/_logic.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/feature_store/register/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/feature_store/register/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/feature_store/register/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/feature_store/resume/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/feature_store/resume/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/feature_store/trigger/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/feature_store/trigger/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/_logic/instance_template.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/_logic/instance_template.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/_logic/variations.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/_logic/variations.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/build_steps.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/build_steps.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/client_logs/build_run_handlers.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/client_logs/build_run_handlers.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/client_logs/cli_ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/client_logs/cli_ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/client_logs/logger.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/client_logs/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/client_logs/messages.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/client_logs/messages.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/client_logs/notifier_impl.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/client_logs/notifier_impl.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/client_logs/time_source.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/client_logs/time_source.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/config/config_v1.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/config/config_v1.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/constant/step_description.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/constant/step_description.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/context.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/context.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/interface/notifier_interface.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/interface/notifier_interface.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/interface/step_inteface.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/interface/step_inteface.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_model_step.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_model_step.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/common.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/common.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/fetch_strategy_manager.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/fetch_strategy_manager.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/folder/folder_strategy.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/folder/folder_strategy.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/git/git_strategy.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/git/git_strategy.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/strategy.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/zip/zip_strategy.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/zip/zip_strategy.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/post_fetch_validation_step.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/post_fetch_validation_step.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/pre_fetch_validation_step.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/pre_fetch_validation_step.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/cleanup_step.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/cleanup_step.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/start_remote_build_step.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/start_remote_build_step.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/upload_step.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/upload_step.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/c_deploy/build_polling_status.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/c_deploy/build_polling_status.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/phase/c_deploy/deploy_build.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/phase/c_deploy/deploy_build.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/util/protobuf_factory.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/util/protobuf_factory.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/build/_logic/util/step_decorator.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/build/_logic/util/step_decorator.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/build/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/build/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/builds/cancel/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/builds/cancel/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/builds/logs/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/builds/logs/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/builds/status/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/builds/status/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/create/_logic.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/create/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/create/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/create/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/delete/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/delete/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/_logic/advance_deployment_options_handler.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/_logic/advance_deployment_options_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/_logic/base_deploy_executor.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/_logic/base_deploy_executor.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/_logic/deploy_config.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/_logic/deploy_config.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/_logic/deployment.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/_logic/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_message_helpers.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_message_helpers.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_response_handler.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_response_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_size_mapper.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_size_mapper.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/_logic/get_latest_successful_build.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/_logic/get_latest_successful_build.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/_logic/variations.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/_logic/variations.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/batch/_logic/deploy_executor.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/batch/_logic/deploy_executor.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/batch/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/batch/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/advanced_deployment_mapper.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/advanced_deployment_mapper.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/deploy_executor.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/deploy_executor.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/serving_strategy_mapper.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/serving_strategy_mapper.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/realtime/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/realtime/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/deploy_executor.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/deploy_executor.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/serving_strategy_mapper.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/serving_strategy_mapper.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/deploy/streaming/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/deploy/streaming/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/undeploy/_logic/request_undeploy.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/undeploy/_logic/request_undeploy.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/undeploy/_logic/variations.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/undeploy/_logic/variations.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/deployments/undeploy/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/deployments/undeploy/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/executions/cancel/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/executions/cancel/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/executions/execution_commands_group.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/executions/execution_commands_group.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/executions/report/_logic.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/executions/report/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/executions/report/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/executions/report/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/executions/start/_logic.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/executions/start/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/executions/start/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/executions/start/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/executions/status/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/executions/status/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/initialize_model_structure.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/initialize_model_structure.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/data.csv` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/data.csv`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/model.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/model.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/it/test_churn.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/it/test_churn.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/data.csv` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/data.csv`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/model.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/model.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/model.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/model.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/model.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/model.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/it/test_titanic.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/it/test_titanic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/model.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/model.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/it/test_titanic.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/it/test_titanic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/init/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/init/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/list/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/list/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/models_command_group.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/models_command_group.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/runtime/feedback/_logic.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/runtime/feedback/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/runtime/feedback/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/runtime/feedback/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/runtime/logs/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/runtime/logs/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/runtime/runtime_commands_group.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/runtime/runtime_commands_group.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/runtime/traffic_update/_logic/execute_runtime_update_traffic.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/runtime/traffic_update/_logic/execute_runtime_update_traffic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/runtime/traffic_update/_logic/variations.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/runtime/traffic_update/_logic/variations.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/runtime/traffic_update/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/runtime/traffic_update/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/models/runtime/update/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/models/runtime/update/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/projects/create/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/projects/create/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/projects/delete/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/projects/delete/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/projects/list/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/projects/list/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/projects/projects_command_group.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/projects/projects_command_group.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/secrets/delete/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/secrets/delete/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/secrets/get/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/secrets/get/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/commands/secrets/set/ui.py` & `qwak_sdk-0.5.9/qwak_sdk/commands/secrets/set/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/common/run_config/base.py` & `qwak_sdk-0.5.9/qwak_sdk/common/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/common/run_config/utils.py` & `qwak_sdk-0.5.9/qwak_sdk/common/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/exceptions/qwak_suggestion_exception.py` & `qwak_sdk-0.5.9/qwak_sdk/exceptions/qwak_suggestion_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/inner/file_registry.py` & `qwak_sdk-0.5.9/qwak_sdk/inner/file_registry.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/inner/tools/cli_tools.py` & `qwak_sdk-0.5.9/qwak_sdk/inner/tools/cli_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/inner/tools/config_handler.py` & `qwak_sdk-0.5.9/qwak_sdk/inner/tools/config_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/inner/tools/logger/logger.py` & `qwak_sdk-0.5.9/qwak_sdk/inner/tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/inner/tools/logger/logging.yml` & `qwak_sdk-0.5.9/qwak_sdk/inner/tools/logger/logging.yml`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/inner/tools/tracking.py` & `qwak_sdk-0.5.9/qwak_sdk/inner/tools/tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/tools/files.py` & `qwak_sdk-0.5.9/qwak_sdk/tools/files.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/tools/log_handling.py` & `qwak_sdk-0.5.9/qwak_sdk/tools/log_handling.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/qwak_sdk/tools/utils.py` & `qwak_sdk-0.5.9/qwak_sdk/tools/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.8/setup.py` & `qwak_sdk-0.5.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['assertpy>=1.1,<2.0',
  'cookiecutter',
  'gitpython>=2.1.0',
- 'pydantic',
+ 'pydantic<2',
  'python-json-logger>=2.0.2',
  'qwak-core==0.0.113',
  'qwak-inference==0.1.4',
  'tabulate>=0.8.0',
  'yaspin>=2.0.0']
 
 extras_require = \
@@ -152,15 +152,15 @@
                                                                   'pandas>=1.4.3,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['qwak = qwak_sdk.main:qwak_cli']}
 
 setup_kwargs = {
     'name': 'qwak-sdk',
-    'version': '0.5.8',
+    'version': '0.5.9',
     'description': 'Qwak SDK and CLI for qwak models',
     'long_description': '# Qwak SDK\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_sdk-0.5.8/PKG-INFO` & `qwak_sdk-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-sdk
-Version: 0.5.8
+Version: 0.5.9
 Summary: Qwak SDK and CLI for qwak models
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
@@ -23,15 +23,15 @@
 Requires-Dist: boto3 (>=1.24.116,<2.0.0) ; extra == "batch" or extra == "feedback"
 Requires-Dist: cookiecutter
 Requires-Dist: gitpython (>=2.1.0)
 Requires-Dist: joblib (>=1.1.0,<2.0.0) ; extra == "batch" or extra == "feedback"
 Requires-Dist: pandas (<1.4) ; (python_full_version >= "3.7.1" and python_version < "3.8") and (extra == "batch" or extra == "feedback")
 Requires-Dist: pandas (>=1.4.3,<2.0.0) ; (python_version >= "3.8" and python_version < "3.10") and (extra == "batch" or extra == "feedback")
 Requires-Dist: pyarrow (>=6.0.0,<11.0.0) ; extra == "batch"
-Requires-Dist: pydantic
+Requires-Dist: pydantic (<2)
 Requires-Dist: python-json-logger (>=2.0.2)
 Requires-Dist: qwak-core (==0.0.113)
 Requires-Dist: qwak-inference (==0.1.4)
 Requires-Dist: tabulate (>=0.8.0)
 Requires-Dist: yaspin (>=2.0.0)
 Project-URL: Home page, https://www.qwak.com/
 Description-Content-Type: text/markdown
```

