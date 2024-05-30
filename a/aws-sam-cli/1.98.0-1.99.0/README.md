# Comparing `tmp/aws-sam-cli-1.98.0.tar.gz` & `tmp/aws-sam-cli-1.99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-sam-cli-1.98.0.tar", last modified: Tue Oct  3 18:50:17 2023, max compression
+gzip compressed data, was "aws-sam-cli-1.99.0.tar", last modified: Wed Oct 18 17:43:05 2023, max compression
```

## Comparing `aws-sam-cli-1.98.0.tar` & `aws-sam-cli-1.99.0.tar`

### file list

```diff
@@ -1,928 +1,930 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.798488 aws-sam-cli-1.98.0/
--rw-r--r--   0 root         (0) root         (0)    11387 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      243 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)       89 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)    12195 2023-10-03 18:50:17.798488 aws-sam-cli-1.98.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8219 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/README.md
--rw-r--r--   0 root         (0) root         (0)     9124 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/THIRD-PARTY-LICENSES
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.706488 aws-sam-cli-1.98.0/aws_sam_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12195 2023-10-03 18:50:15.000000 aws-sam-cli-1.98.0/aws_sam_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    37137 2023-10-03 18:50:16.000000 aws-sam-cli-1.98.0/aws_sam_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-03 18:50:15.000000 aws-sam-cli-1.98.0/aws_sam_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-10-03 18:50:15.000000 aws-sam-cli-1.98.0/aws_sam_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     1270 2023-10-03 18:50:15.000000 aws-sam-cli-1.98.0/aws_sam_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-10-03 18:50:15.000000 aws-sam-cli-1.98.0/aws_sam_cli.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      792 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.706488 aws-sam-cli-1.98.0/requirements/
--rw-r--r--   0 root         (0) root         (0)     1087 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/requirements/base.txt
--rw-r--r--   0 root         (0) root         (0)     1251 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/requirements/dev.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/requirements/pre-dev.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.706488 aws-sam-cli-1.98.0/samcli/
--rw-r--r--   0 root         (0) root         (0)       48 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/__init__.py
--rw-r--r--   0 root         (0) root         (0)      358 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.706488 aws-sam-cli-1.98.0/samcli/cli/
--rw-r--r--   0 root         (0) root         (0)       22 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16220 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/cli/cli_config_file.py
--rw-r--r--   0 root         (0) root         (0)    11226 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/cli/command.py
--rw-r--r--   0 root         (0) root         (0)     8505 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/cli/context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.706488 aws-sam-cli-1.98.0/samcli/cli/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/cli/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3052 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/cli/core/command.py
--rw-r--r--   0 root         (0) root         (0)      901 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/cli/core/options.py
--rw-r--r--   0 root         (0) root         (0)     2593 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/cli/formatters.py
--rw-r--r--   0 root         (0) root         (0)    15124 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/cli/global_config.py
--rw-r--r--   0 root         (0) root         (0)     1020 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/cli/hidden_imports.py
--rw-r--r--   0 root         (0) root         (0)     1945 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/cli/import_module_proxy.py
--rw-r--r--   0 root         (0) root         (0)     5650 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/cli/main.py
--rw-r--r--   0 root         (0) root         (0)     2059 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/cli/options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.706488 aws-sam-cli-1.98.0/samcli/cli/root/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/cli/root/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1125 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/cli/root/command_list.py
--rw-r--r--   0 root         (0) root         (0)     1712 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/cli/row_modifiers.py
--rw-r--r--   0 root         (0) root         (0)    16898 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/cli/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.706488 aws-sam-cli-1.98.0/samcli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.710488 aws-sam-cli-1.98.0/samcli/commands/_utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1233 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/_utils/cdk_support_decorators.py
--rw-r--r--   0 root         (0) root         (0)     3894 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/_utils/click_mutex.py
--rw-r--r--   0 root         (0) root         (0)     3479 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/_utils/command_exception_handler.py
--rw-r--r--   0 root         (0) root         (0)      368 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/_utils/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.710488 aws-sam-cli-1.98.0/samcli/commands/_utils/custom_options/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/_utils/custom_options/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6726 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/_utils/custom_options/hook_name_option.py
--rw-r--r--   0 root         (0) root         (0)     1922 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/_utils/custom_options/option_nargs.py
--rw-r--r--   0 root         (0) root         (0)      534 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/_utils/custom_options/replace_help_option.py
--rw-r--r--   0 root         (0) root         (0)     8878 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/_utils/experimental.py
--rw-r--r--   0 root         (0) root         (0)      440 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/_utils/option_validator.py
--rw-r--r--   0 root         (0) root         (0)     2952 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/_utils/option_value_processor.py
--rw-r--r--   0 root         (0) root         (0)    30733 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/_utils/options.py
--rw-r--r--   0 root         (0) root         (0)      983 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/_utils/parameterized_option.py
--rw-r--r--   0 root         (0) root         (0)     5713 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/_utils/table_print.py
--rw-r--r--   0 root         (0) root         (0)    13274 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/_utils/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.710488 aws-sam-cli-1.98.0/samcli/commands/bootstrap/
--rw-r--r--   0 root         (0) root         (0)      103 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/bootstrap/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1042 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/bootstrap/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.710488 aws-sam-cli-1.98.0/samcli/commands/build/
--rw-r--r--   0 root         (0) root         (0)       91 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/build/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29521 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/build/build_context.py
--rw-r--r--   0 root         (0) root         (0)      677 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/build/click_container.py
--rw-r--r--   0 root         (0) root         (0)     8099 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/build/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.710488 aws-sam-cli-1.98.0/samcli/commands/build/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/build/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2811 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/build/core/command.py
--rw-r--r--   0 root         (0) root         (0)      852 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/build/core/formatters.py
--rw-r--r--   0 root         (0) root         (0)     2929 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/build/core/options.py
--rw-r--r--   0 root         (0) root         (0)      333 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/build/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     3562 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/build/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.710488 aws-sam-cli-1.98.0/samcli/commands/delete/
--rw-r--r--   0 root         (0) root         (0)       92 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/delete/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3845 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/delete/command.py
--rw-r--r--   0 root         (0) root         (0)    14668 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/delete/delete_context.py
--rw-r--r--   0 root         (0) root         (0)     2296 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/delete/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.710488 aws-sam-cli-1.98.0/samcli/commands/deploy/
--rw-r--r--   0 root         (0) root         (0)       92 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/deploy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5746 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/deploy/auth_utils.py
--rw-r--r--   0 root         (0) root         (0)     2516 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/deploy/code_signer_utils.py
--rw-r--r--   0 root         (0) root         (0)    12751 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/deploy/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.714488 aws-sam-cli-1.98.0/samcli/commands/deploy/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/deploy/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4552 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/deploy/core/command.py
--rw-r--r--   0 root         (0) root         (0)      882 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/deploy/core/formatters.py
--rw-r--r--   0 root         (0) root         (0)     2916 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/deploy/core/options.py
--rw-r--r--   0 root         (0) root         (0)    12422 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/deploy/deploy_context.py
--rw-r--r--   0 root         (0) root         (0)     2798 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/deploy/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     5316 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/deploy/guided_config.py
--rw-r--r--   0 root         (0) root         (0)    26323 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/deploy/guided_context.py
--rw-r--r--   0 root         (0) root         (0)     4722 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/deploy/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.714488 aws-sam-cli-1.98.0/samcli/commands/docs/
--rw-r--r--   0 root         (0) root         (0)       90 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/docs/__init__.py
--rw-r--r--   0 root         (0) root         (0)      913 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/docs/command.py
--rw-r--r--   0 root         (0) root         (0)     4047 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/docs/command_context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.714488 aws-sam-cli-1.98.0/samcli/commands/docs/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/docs/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5461 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/docs/core/command.py
--rw-r--r--   0 root         (0) root         (0)      566 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/docs/core/formatter.py
--rw-r--r--   0 root         (0) root         (0)      163 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/docs/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     4576 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.714488 aws-sam-cli-1.98.0/samcli/commands/init/
--rw-r--r--   0 root         (0) root         (0)       73 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/init/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13529 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/init/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.718488 aws-sam-cli-1.98.0/samcli/commands/init/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/init/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4681 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/init/core/command.py
--rw-r--r--   0 root         (0) root         (0)      878 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/init/core/formatters.py
--rw-r--r--   0 root         (0) root         (0)     1955 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/init/core/options.py
--rw-r--r--   0 root         (0) root         (0)     4617 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/init/init_flow_helpers.py
--rw-r--r--   0 root         (0) root         (0)      819 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/init/init_generator.py
--rw-r--r--   0 root         (0) root         (0)    15625 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/init/init_templates.py
--rw-r--r--   0 root         (0) root         (0)     8249 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/init/interactive_event_bridge_flow.py
--rw-r--r--   0 root         (0) root         (0)    20316 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/init/interactive_init_flow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.718488 aws-sam-cli-1.98.0/samcli/commands/list/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/list/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.718488 aws-sam-cli-1.98.0/samcli/commands/list/cli_common/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/list/cli_common/__init__.py
--rw-r--r--   0 root         (0) root         (0)      807 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/list/cli_common/list_common_context.py
--rw-r--r--   0 root         (0) root         (0)     1126 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/list/cli_common/options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.718488 aws-sam-cli-1.98.0/samcli/commands/list/endpoints/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/list/endpoints/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2257 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/list/endpoints/command.py
--rw-r--r--   0 root         (0) root         (0)     3163 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/list/endpoints/endpoints_context.py
--rw-r--r--   0 root         (0) root         (0)     1505 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/list/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      319 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/list/json_consumer.py
--rw-r--r--   0 root         (0) root         (0)      556 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/list/list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.718488 aws-sam-cli-1.98.0/samcli/commands/list/resources/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/list/resources/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2211 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/list/resources/command.py
--rw-r--r--   0 root         (0) root         (0)     2018 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/list/resources/resources_context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.718488 aws-sam-cli-1.98.0/samcli/commands/list/stack_outputs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/list/stack_outputs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1636 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/list/stack_outputs/command.py
--rw-r--r--   0 root         (0) root         (0)     1434 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/list/stack_outputs/stack_outputs_context.py
--rw-r--r--   0 root         (0) root         (0)     1290 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/list/table_consumer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.718488 aws-sam-cli-1.98.0/samcli/commands/local/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.718488 aws-sam-cli-1.98.0/samcli/commands/local/cli_common/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/cli_common/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24015 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/cli_common/invoke_context.py
--rw-r--r--   0 root         (0) root         (0)     8386 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/cli_common/options.py
--rw-r--r--   0 root         (0) root         (0)     2055 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/cli_common/user_exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.718488 aws-sam-cli-1.98.0/samcli/commands/local/generate_event/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/generate_event/__init__.py
--rw-r--r--   0 root         (0) root         (0)      730 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/generate_event/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.718488 aws-sam-cli-1.98.0/samcli/commands/local/generate_event/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/generate_event/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3985 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/generate_event/core/command.py
--rw-r--r--   0 root         (0) root         (0)     7043 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/generate_event/event_generation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.718488 aws-sam-cli-1.98.0/samcli/commands/local/invoke/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/invoke/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8069 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/invoke/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.718488 aws-sam-cli-1.98.0/samcli/commands/local/invoke/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/invoke/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3647 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/invoke/core/command.py
--rw-r--r--   0 root         (0) root         (0)      861 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/invoke/core/formatters.py
--rw-r--r--   0 root         (0) root         (0)     2888 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/invoke/core/options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.722488 aws-sam-cli-1.98.0/samcli/commands/local/lib/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/lib/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1165 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/lib/debug_context.py
--rw-r--r--   0 root         (0) root         (0)     1023 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/lib/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     5524 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/lib/local_api_service.py
--rw-r--r--   0 root         (0) root         (0)    15482 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/lib/local_lambda.py
--rw-r--r--   0 root         (0) root         (0)     2207 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/lib/local_lambda_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.722488 aws-sam-cli-1.98.0/samcli/commands/local/lib/swagger/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/lib/swagger/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11346 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/lib/swagger/integration_uri.py
--rw-r--r--   0 root         (0) root         (0)    19348 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/lib/swagger/parser.py
--rw-r--r--   0 root         (0) root         (0)     9397 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/lib/swagger/reader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.722488 aws-sam-cli-1.98.0/samcli/commands/local/lib/validators/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/lib/validators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2034 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/lib/validators/identity_source_validator.py
--rw-r--r--   0 root         (0) root         (0)    10881 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/lib/validators/lambda_auth_props.py
--rw-r--r--   0 root         (0) root         (0)      658 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/local.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.722488 aws-sam-cli-1.98.0/samcli/commands/local/start_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/start_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8283 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/start_api/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.722488 aws-sam-cli-1.98.0/samcli/commands/local/start_api/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/start_api/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1744 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/start_api/core/command.py
--rw-r--r--   0 root         (0) root         (0)      876 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/start_api/core/formatters.py
--rw-r--r--   0 root         (0) root         (0)     2918 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/start_api/core/options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.722488 aws-sam-cli-1.98.0/samcli/commands/local/start_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/start_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7170 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/start_lambda/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.722488 aws-sam-cli-1.98.0/samcli/commands/local/start_lambda/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/start_lambda/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4066 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/start_lambda/core/command.py
--rw-r--r--   0 root         (0) root         (0)      885 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/start_lambda/core/formatters.py
--rw-r--r--   0 root         (0) root         (0)     2903 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/local/start_lambda/core/options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.722488 aws-sam-cli-1.98.0/samcli/commands/logs/
--rw-r--r--   0 root         (0) root         (0)       90 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6903 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/logs/command.py
--rw-r--r--   0 root         (0) root         (0)      848 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/logs/console_consumers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.722488 aws-sam-cli-1.98.0/samcli/commands/logs/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/logs/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5047 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/logs/core/command.py
--rw-r--r--   0 root         (0) root         (0)      878 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/logs/core/formatters.py
--rw-r--r--   0 root         (0) root         (0)     1805 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/logs/core/options.py
--rw-r--r--   0 root         (0) root         (0)     6742 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/logs/logs_context.py
--rw-r--r--   0 root         (0) root         (0)     7048 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/logs/puller_factory.py
--rw-r--r--   0 root         (0) root         (0)     2523 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/logs/validation_and_exception_handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.722488 aws-sam-cli-1.98.0/samcli/commands/package/
--rw-r--r--   0 root         (0) root         (0)       93 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/package/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5539 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/package/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.726488 aws-sam-cli-1.98.0/samcli/commands/package/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/package/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5574 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/package/core/command.py
--rw-r--r--   0 root         (0) root         (0)      884 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/package/core/formatters.py
--rw-r--r--   0 root         (0) root         (0)     2282 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/package/core/options.py
--rw-r--r--   0 root         (0) root         (0)     5081 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/package/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     7526 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/package/package_context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.726488 aws-sam-cli-1.98.0/samcli/commands/pipeline/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/pipeline/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.726488 aws-sam-cli-1.98.0/samcli/commands/pipeline/bootstrap/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/pipeline/bootstrap/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19260 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/pipeline/bootstrap/cli.py
--rw-r--r--   0 root         (0) root         (0)    19150 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/pipeline/bootstrap/guided_context.py
--rw-r--r--   0 root         (0) root         (0)     2801 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/pipeline/bootstrap/oidc_config.py
--rw-r--r--   0 root         (0) root         (0)     7075 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/pipeline/bootstrap/pipeline_oidc_provider.py
--rw-r--r--   0 root         (0) root         (0)      429 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/pipeline/external_links.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.726488 aws-sam-cli-1.98.0/samcli/commands/pipeline/init/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/pipeline/init/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2158 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/pipeline/init/cli.py
--rw-r--r--   0 root         (0) root         (0)    24242 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/pipeline/init/interactive_init_flow.py
--rw-r--r--   0 root         (0) root         (0)     2398 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/pipeline/init/pipeline_templates_manifest.py
--rw-r--r--   0 root         (0) root         (0)      455 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/pipeline/pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.726488 aws-sam-cli-1.98.0/samcli/commands/publish/
--rw-r--r--   0 root         (0) root         (0)       92 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/publish/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6008 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/publish/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.726488 aws-sam-cli-1.98.0/samcli/commands/remote/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/__init__.py
--rw-r--r--   0 root         (0) root         (0)      857 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.726488 aws-sam-cli-1.98.0/samcli/commands/remote/invoke/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/invoke/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6303 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/invoke/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.726488 aws-sam-cli-1.98.0/samcli/commands/remote/invoke/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/invoke/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6836 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/invoke/core/command.py
--rw-r--r--   0 root         (0) root         (0)      865 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/invoke/core/formatters.py
--rw-r--r--   0 root         (0) root         (0)     1979 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/invoke/core/options.py
--rw-r--r--   0 root         (0) root         (0)      538 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/remote.py
--rw-r--r--   0 root         (0) root         (0)    11090 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/remote_invoke_context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.726488 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.726488 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1165 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/core/base_options.py
--rw-r--r--   0 root         (0) root         (0)      872 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/core/formatters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.726488 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/delete/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/delete/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4204 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/delete/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.730488 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/delete/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/delete/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3971 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/delete/core/command.py
--rw-r--r--   0 root         (0) root         (0)      444 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/delete/core/formatters.py
--rw-r--r--   0 root         (0) root         (0)     1127 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/delete/core/options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.730488 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/get/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/get/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4780 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/get/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.730488 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/get/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/get/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4726 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/get/core/command.py
--rw-r--r--   0 root         (0) root         (0)      434 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/get/core/formatters.py
--rw-r--r--   0 root         (0) root         (0)     1139 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/get/core/options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.730488 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/list/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/list/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3868 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/list/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.730488 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/list/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/list/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3844 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/list/core/command.py
--rw-r--r--   0 root         (0) root         (0)      438 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/list/core/formatters.py
--rw-r--r--   0 root         (0) root         (0)      959 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/list/core/options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.730488 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/put/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/put/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5464 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/put/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.730488 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/put/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/put/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5114 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/put/core/command.py
--rw-r--r--   0 root         (0) root         (0)      434 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/put/core/formatters.py
--rw-r--r--   0 root         (0) root         (0)     1141 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/put/core/options.py
--rw-r--r--   0 root         (0) root         (0)      546 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/test_event.py
--rw-r--r--   0 root         (0) root         (0)     1615 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/remote/test_event/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.730488 aws-sam-cli-1.98.0/samcli/commands/sync/
--rw-r--r--   0 root         (0) root         (0)       89 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/sync/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20846 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/sync/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.730488 aws-sam-cli-1.98.0/samcli/commands/sync/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/sync/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3892 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/sync/core/command.py
--rw-r--r--   0 root         (0) root         (0)      927 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/sync/core/formatters.py
--rw-r--r--   0 root         (0) root         (0)     2315 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/sync/core/options.py
--rw-r--r--   0 root         (0) root         (0)    10155 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/sync/sync_context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.734488 aws-sam-cli-1.98.0/samcli/commands/traces/
--rw-r--r--   0 root         (0) root         (0)      106 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/traces/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2920 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/traces/command.py
--rw-r--r--   0 root         (0) root         (0)      578 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/traces/trace_console_consumers.py
--rw-r--r--   0 root         (0) root         (0)     4189 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/traces/traces_puller_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.734488 aws-sam-cli-1.98.0/samcli/commands/validate/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/validate/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.734488 aws-sam-cli-1.98.0/samcli/commands/validate/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/validate/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1845 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/validate/core/command.py
--rw-r--r--   0 root         (0) root         (0)      862 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/validate/core/formatters.py
--rw-r--r--   0 root         (0) root         (0)     1647 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/validate/core/options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.734488 aws-sam-cli-1.98.0/samcli/commands/validate/lib/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/validate/lib/__init__.py
--rw-r--r--   0 root         (0) root         (0)      158 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/validate/lib/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     7069 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/commands/validate/validate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.734488 aws-sam-cli-1.98.0/samcli/hook_packages/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/hook_packages/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.734488 aws-sam-cli-1.98.0/samcli/hook_packages/terraform/
--rw-r--r--   0 root         (0) root         (0)      425 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/hook_packages/terraform/Config.json
--rw-r--r--   0 root         (0) root         (0)       64 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/hook_packages/terraform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12097 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/hook_packages/terraform/copy_terraform_built_artifacts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.734488 aws-sam-cli-1.98.0/samcli/hook_packages/terraform/designs/
--rw-r--r--   0 root         (0) root         (0)     7203 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/hook_packages/terraform/designs/resource_linking_generalized.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.734488 aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.734488 aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1368 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/constants.py
--rw-r--r--   0 root         (0) root         (0)    28896 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/enrich.py
--rw-r--r--   0 root         (0) root         (0)    13548 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    10856 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/hook.py
--rw-r--r--   0 root         (0) root         (0)     9215 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/makefile_generator.py
--rw-r--r--   0 root         (0) root         (0)    18502 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/property_builder.py
--rw-r--r--   0 root         (0) root         (0)   111362 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/resource_linking.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.734488 aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/resources/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/resources/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13702 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/resources/apigw.py
--rw-r--r--   0 root         (0) root         (0)     2375 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/resources/code_resource_utils.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/resources/internal.py
--rw-r--r--   0 root         (0) root         (0)     2451 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/resources/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     1942 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/resources/lambda_layers.py
--rw-r--r--   0 root         (0) root         (0)     6339 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/resources/resource_links.py
--rw-r--r--   0 root         (0) root         (0)     2965 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/resources/resource_properties.py
--rw-r--r--   0 root         (0) root         (0)    24739 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/translate.py
--rw-r--r--   0 root         (0) root         (0)     6057 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/types.py
--rw-r--r--   0 root         (0) root         (0)      495 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.738488 aws-sam-cli-1.98.0/samcli/hook_packages/terraform/lib/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/hook_packages/terraform/lib/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2789 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/hook_packages/terraform/lib/utils.py
--rw-r--r--   0 root         (0) root         (0)      172 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/hook_packages/terraform/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.738488 aws-sam-cli-1.98.0/samcli/lib/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.738488 aws-sam-cli-1.98.0/samcli/lib/bootstrap/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/bootstrap/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6348 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/bootstrap/bootstrap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.738488 aws-sam-cli-1.98.0/samcli/lib/bootstrap/companion_stack/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/bootstrap/companion_stack/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3615 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/bootstrap/companion_stack/companion_stack_builder.py
--rw-r--r--   0 root         (0) root         (0)    12578 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/bootstrap/companion_stack/companion_stack_manager.py
--rw-r--r--   0 root         (0) root         (0)     5213 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/bootstrap/companion_stack/data_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.738488 aws-sam-cli-1.98.0/samcli/lib/bootstrap/nested_stack/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/bootstrap/nested_stack/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3667 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/bootstrap/nested_stack/nested_stack_builder.py
--rw-r--r--   0 root         (0) root         (0)     8669 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/bootstrap/nested_stack/nested_stack_manager.py
--rw-r--r--   0 root         (0) root         (0)     1937 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/bootstrap/stack_builder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.738488 aws-sam-cli-1.98.0/samcli/lib/build/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/build/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44411 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/build/app_builder.py
--rw-r--r--   0 root         (0) root         (0)    28066 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/build/build_graph.py
--rw-r--r--   0 root         (0) root         (0)    27127 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/build/build_strategy.py
--rw-r--r--   0 root         (0) root         (0)    10142 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/build/bundler.py
--rw-r--r--   0 root         (0) root         (0)      304 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/build/constants.py
--rw-r--r--   0 root         (0) root         (0)     2886 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/build/dependency_hash_generator.py
--rw-r--r--   0 root         (0) root         (0)     1476 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/build/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2255 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/build/utils.py
--rw-r--r--   0 root         (0) root         (0)    11865 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/build/workflow_config.py
--rw-r--r--   0 root         (0) root         (0)     3351 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/build/workflows.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.738488 aws-sam-cli-1.98.0/samcli/lib/cli_validation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/cli_validation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6013 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/cli_validation/image_repository_validation.py
--rw-r--r--   0 root         (0) root         (0)     2980 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/cli_validation/remote_invoke_options_validations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.738488 aws-sam-cli-1.98.0/samcli/lib/config/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)      470 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/config/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     9442 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/config/file_manager.py
--rw-r--r--   0 root         (0) root         (0)    10585 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/config/samconfig.py
--rw-r--r--   0 root         (0) root         (0)      122 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/config/version.py
--rw-r--r--   0 root         (0) root         (0)       32 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.738488 aws-sam-cli-1.98.0/samcli/lib/cookiecutter/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/cookiecutter/__init__.py
--rw-r--r--   0 root         (0) root         (0)      873 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/cookiecutter/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     3384 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/cookiecutter/interactive_flow.py
--rw-r--r--   0 root         (0) root         (0)     5654 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/cookiecutter/interactive_flow_creator.py
--rw-r--r--   0 root         (0) root         (0)     1210 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/cookiecutter/plugin.py
--rw-r--r--   0 root         (0) root         (0)      594 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/cookiecutter/processor.py
--rw-r--r--   0 root         (0) root         (0)    11820 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/cookiecutter/question.py
--rw-r--r--   0 root         (0) root         (0)     9214 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/cookiecutter/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.742488 aws-sam-cli-1.98.0/samcli/lib/delete/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/delete/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8383 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/delete/cfn_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.742488 aws-sam-cli-1.98.0/samcli/lib/deploy/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/deploy/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34866 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/deploy/deployer.py
--rw-r--r--   0 root         (0) root         (0)     1359 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/deploy/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.742488 aws-sam-cli-1.98.0/samcli/lib/docker/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/docker/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3319 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/docker/log_streamer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.742488 aws-sam-cli-1.98.0/samcli/lib/docs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/docs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1212 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/docs/browser_configuration.py
--rw-r--r--   0 root         (0) root         (0)     2007 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/docs/documentation.py
--rw-r--r--   0 root         (0) root         (0)     3405 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/docs/documentation_links.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.742488 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28057 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/event-mapping.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.694488 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.742488 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/alb/
--rw-r--r--   0 root         (0) root         (0)     1050 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/alb/ALBRequest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.742488 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/alexa-skills-kit/
--rw-r--r--   0 root         (0) root         (0)      825 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/alexa-skills-kit/AlexaEndSession.json
--rw-r--r--   0 root         (0) root         (0)     1474 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/alexa-skills-kit/AlexaIntentAnswer.json
--rw-r--r--   0 root         (0) root         (0)      925 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/alexa-skills-kit/AlexaIntentGetNewFact.json
--rw-r--r--   0 root         (0) root         (0)     1018 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/alexa-skills-kit/AlexaIntentMyColorIs.json
--rw-r--r--   0 root         (0) root         (0)     1005 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/alexa-skills-kit/AlexaIntentRecipe.json
--rw-r--r--   0 root         (0) root         (0)      851 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/alexa-skills-kit/AlexaStartSession.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.742488 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/alexa-smart-home/
--rw-r--r--   0 root         (0) root         (0)      365 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/alexa-smart-home/AlexaSmartHomeControlTurnOffRequest.json
--rw-r--r--   0 root         (0) root         (0)      364 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/alexa-smart-home/AlexaSmartHomeControlTurnOnRequest.json
--rw-r--r--   0 root         (0) root         (0)      239 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/alexa-smart-home/AlexaSmartHomeDiscoveryRequest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.742488 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/apigateway/
--rw-r--r--   0 root         (0) root         (0)      207 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/apigateway/ApiGatewayAuthorizer.json
--rw-r--r--   0 root         (0) root         (0)     1513 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/apigateway/ApiGatewayRestRequestAuthorizer.json
--rw-r--r--   0 root         (0) root         (0)     3232 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/apigateway/AwsProxy.json
--rw-r--r--   0 root         (0) root         (0)     1657 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/apigateway/HttpApi.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.742488 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/appsync/
--rw-r--r--   0 root         (0) root         (0)     2516 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/appsync/AppSyncDirectResolver.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.742488 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/batch/
--rw-r--r--   0 root         (0) root         (0)       91 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/batch/BatchGetJob.json
--rw-r--r--   0 root         (0) root         (0)       53 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/batch/BatchSubmitJob.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.742488 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/cloudformation/
--rw-r--r--   0 root         (0) root         (0)      442 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/cloudformation/CfnCreateRequest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.746488 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/cloudfront/
--rw-r--r--   0 root         (0) root         (0)      771 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontABTest.json
--rw-r--r--   0 root         (0) root         (0)      876 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontAccessRequestInResponse.json
--rw-r--r--   0 root         (0) root         (0)      592 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontHttpRedirect.json
--rw-r--r--   0 root         (0) root         (0)      790 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontModifyQueryString.json
--rw-r--r--   0 root         (0) root         (0)      719 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontModifyResponseHeader.json
--rw-r--r--   0 root         (0) root         (0)      592 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontMultipleRemoteCallsAggregateResponse.json
--rw-r--r--   0 root         (0) root         (0)      793 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontNormalizeQuerystringToImproveCacheHit.json
--rw-r--r--   0 root         (0) root         (0)      614 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontRedirectOnViewerCountry.json
--rw-r--r--   0 root         (0) root         (0)      432 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontRedirectUnauthenticatedUsers.json
--rw-r--r--   0 root         (0) root         (0)      442 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontResponseGeneration.json
--rw-r--r--   0 root         (0) root         (0)     1161 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontServeObjectOnViewerDevice.json
--rw-r--r--   0 root         (0) root         (0)      744 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontSimpleRemoteCall.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.746488 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/cloudwatch/
--rw-r--r--   0 root         (0) root         (0)      318 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/cloudwatch/CloudwatchLogs.json
--rw-r--r--   0 root         (0) root         (0)      325 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/cloudwatch/ScheduledEvent.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.746488 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/codecommit/
--rw-r--r--   0 root         (0) root         (0)      868 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/codecommit/CodeCommit.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.746488 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/codepipeline/
--rw-r--r--   0 root         (0) root         (0)     1175 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/codepipeline/CodePipeline.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.746488 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/cognito/
--rw-r--r--   0 root         (0) root         (0)      425 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/cognito/CognitoSyncTrigger.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.746488 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/config/
--rw-r--r--   0 root         (0) root         (0)     1345 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/config/ConfigurationItemChangeNotification.json
--rw-r--r--   0 root         (0) root         (0)     1196 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/config/OversizedConfigurationItemChangeNotification.json
--rw-r--r--   0 root         (0) root         (0)      650 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/config/PeriodicRule.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.746488 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/connect/
--rw-r--r--   0 root         (0) root         (0)     1084 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/connect/ConnectContactFlowEvent.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.746488 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/dynamodb/
--rw-r--r--   0 root         (0) root         (0)     2516 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/dynamodb/DynamoDBUpdate.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.746488 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/kinesis/
--rw-r--r--   0 root         (0) root         (0)      596 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/kinesis/Kinesis.json
--rw-r--r--   0 root         (0) root         (0)      397 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/kinesis/KinesisAnalytics.json
--rw-r--r--   0 root         (0) root         (0)     1737 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/kinesis/KinesisAnalyticsKpl.json
--rw-r--r--   0 root         (0) root         (0)      358 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/kinesis/KinesisFirehose.json
--rw-r--r--   0 root         (0) root         (0)      261 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/kinesis/KinesisFirehoseApachelog.json
--rw-r--r--   0 root         (0) root         (0)     2892 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/kinesis/KinesisFirehoseCloudwatchLogsProcessor.json
--rw-r--r--   0 root         (0) root         (0)      677 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/kinesis/KinesisFirehoseStreamsAsSource.json
--rw-r--r--   0 root         (0) root         (0)      428 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/kinesis/KinesisFirehoseSyslog.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.746488 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/lex/
--rw-r--r--   0 root         (0) root         (0)      489 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/lex/LexBookCar.json
--rw-r--r--   0 root         (0) root         (0)      451 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/lex/LexBookHotel.json
--rw-r--r--   0 root         (0) root         (0)      443 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/lex/LexMakeAppointment.json
--rw-r--r--   0 root         (0) root         (0)      441 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/lex/LexOrderFlowers.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.746488 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/lex-v2/
--rw-r--r--   0 root         (0) root         (0)     3671 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/lex-v2/BankingBot.json
--rw-r--r--   0 root         (0) root         (0)     2732 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/lex-v2/LexBookCar.json
--rw-r--r--   0 root         (0) root         (0)     2663 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/lex-v2/LexBookHotel.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.746488 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/rekognition/
--rw-r--r--   0 root         (0) root         (0)     1018 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/rekognition/RekognitionS3Request.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.746488 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/s3/
--rw-r--r--   0 root         (0) root         (0)      341 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/s3/S3BatchInvocation.json
--rw-r--r--   0 root         (0) root         (0)      943 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/s3/S3Delete.json
--rw-r--r--   0 root         (0) root         (0)     1018 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/s3/S3Put.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.746488 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/sagemaker/
--rw-r--r--   0 root         (0) root         (0)      450 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/sagemaker/AnnotationConsolidation.json
--rw-r--r--   0 root         (0) root         (0)      223 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/sagemaker/PreHumanTask.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.746488 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/ses/
--rw-r--r--   0 root         (0) root         (0)     3305 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/ses/SesEmailReceiving.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.746488 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/sns/
--rw-r--r--   0 root         (0) root         (0)      899 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/sns/Sns.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.750488 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/sqs/
--rw-r--r--   0 root         (0) root         (0)      617 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/sqs/Sqs.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.750488 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/stepfunctions/
--rw-r--r--   0 root         (0) root         (0)       58 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/stepfunctions/StepFunctionsError.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.750488 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/workmail/
--rw-r--r--   0 root         (0) root         (0)      577 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/workmail/WorkMail.json
--rw-r--r--   0 root         (0) root         (0)     5791 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.750488 aws-sam-cli-1.98.0/samcli/lib/hook/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/hook/__init__.py
--rw-r--r--   0 root         (0) root         (0)      529 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/hook/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2768 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/hook/hook_config.py
--rw-r--r--   0 root         (0) root         (0)     2551 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/hook/hook_config_schema.json
--rw-r--r--   0 root         (0) root         (0)     7224 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/hook/hook_wrapper.py
--rw-r--r--   0 root         (0) root         (0)      559 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/hook/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.750488 aws-sam-cli-1.98.0/samcli/lib/iac/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/iac/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.750488 aws-sam-cli-1.98.0/samcli/lib/iac/cdk/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/iac/cdk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1147 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/iac/cdk/cdk_iac.py
--rw-r--r--   0 root         (0) root         (0)     1977 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/iac/cdk/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.750488 aws-sam-cli-1.98.0/samcli/lib/iac/cfn/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/iac/cfn/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7336 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/iac/cfn/cfn_iac.py
--rw-r--r--   0 root         (0) root         (0)      132 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/iac/constants.py
--rw-r--r--   0 root         (0) root         (0)      542 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/iac/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2429 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/iac/iac_factory.py
--rw-r--r--   0 root         (0) root         (0)    23459 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/iac/plugins_interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.750488 aws-sam-cli-1.98.0/samcli/lib/init/
--rw-r--r--   0 root         (0) root         (0)     7528 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3605 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/arbitrary_project.py
--rw-r--r--   0 root         (0) root         (0)     3569 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/default_samconfig.py
--rw-r--r--   0 root         (0) root         (0)      606 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     4661 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/local_manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.750488 aws-sam-cli-1.98.0/samcli/lib/init/template_modifiers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/template_modifiers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3347 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/template_modifiers/application_insights_template_modifier.py
--rw-r--r--   0 root         (0) root         (0)     1680 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/template_modifiers/cli_template_modifier.py
--rw-r--r--   0 root         (0) root         (0)     3346 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/template_modifiers/xray_tracing_template_modifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.702488 aws-sam-cli-1.98.0/samcli/lib/init/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.750488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/
--rw-r--r--   0 root         (0) root         (0)     2277 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/.gitignore
--rw-r--r--   0 root         (0) root         (0)      877 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/LICENSE
--rw-r--r--   0 root         (0) root         (0)      165 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/Pipfile
--rw-r--r--   0 root         (0) root         (0)     1668 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/README.md
--rw-r--r--   0 root         (0) root         (0)      151 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/cookiecutter.json
--rw-r--r--   0 root         (0) root         (0)       18 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.750488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/tests/
--rw-r--r--   0 root         (0) root         (0)     1499 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/tests/test_cookiecutter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.750488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/
--rw-r--r--   0 root         (0) root         (0)     7224 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/.gitignore
--rw-r--r--   0 root         (0) root         (0)     8084 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.754488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/events/
--rw-r--r--   0 root         (0) root         (0)     2121 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/events/event.json
--rw-r--r--   0 root         (0) root         (0)      175 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/omnisharp.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.694488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.754488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/src/HelloWorld/
--rw-r--r--   0 root         (0) root         (0)     1602 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/src/HelloWorld/Function.cs
--rw-r--r--   0 root         (0) root         (0)      559 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/src/HelloWorld/HelloWorld.csproj
--rw-r--r--   0 root         (0) root         (0)      692 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/src/HelloWorld/aws-lambda-tools-defaults.json
--rw-r--r--   0 root         (0) root         (0)     2057 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/template.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.694488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.754488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/test/HelloWorld.Test/
--rw-r--r--   0 root         (0) root         (0)     1987 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/test/HelloWorld.Test/FunctionTest.cs
--rw-r--r--   0 root         (0) root         (0)      688 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/test/HelloWorld.Test/HelloWorld.Tests.csproj
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.754488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/
--rw-r--r--   0 root         (0) root         (0)     2612 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/README.md
--rw-r--r--   0 root         (0) root         (0)      125 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/cookiecutter.json
--rw-r--r--   0 root         (0) root         (0)       70 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/requirements-dev.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.754488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/tests/
--rw-r--r--   0 root         (0) root         (0)     2239 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/tests/test_bake_project.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.754488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/{{cookiecutter.project_name}}/
--rw-r--r--   0 root         (0) root         (0)     5168 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/{{cookiecutter.project_name}}/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.754488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/{{cookiecutter.project_name}}/hello-world/
--rw-r--r--   0 root         (0) root         (0)       65 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/{{cookiecutter.project_name}}/hello-world/go.mod
--rw-r--r--   0 root         (0) root         (0)     1096 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/{{cookiecutter.project_name}}/hello-world/main.go
--rw-r--r--   0 root         (0) root         (0)     1557 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/{{cookiecutter.project_name}}/hello-world/main_test.go
--rw-r--r--   0 root         (0) root         (0)     2059 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/{{cookiecutter.project_name}}/template.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.754488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/
--rw-r--r--   0 root         (0) root         (0)      877 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1651 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/README.md
--rw-r--r--   0 root         (0) root         (0)      150 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/cookiecutter.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.754488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/tests/
--rw-r--r--   0 root         (0) root         (0)     1650 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/tests/test_cookiecutter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.754488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.754488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/
--rw-r--r--   0 root         (0) root         (0)      185 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/build.gradle
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.694488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/gradle/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.754488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/gradle/wrapper/
--rw-r--r--   0 root         (0) root         (0)    55190 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/gradle/wrapper/gradle-wrapper.jar
--rw-r--r--   0 root         (0) root         (0)      202 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/gradle/wrapper/gradle-wrapper.properties
--rwxr-xr-x   0 root         (0) root         (0)     5305 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/gradlew
--rw-r--r--   0 root         (0) root         (0)     2269 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/gradlew.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.694488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.694488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/src/main/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.694488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/src/main/java/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.754488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/src/main/java/helloworld/
--rw-r--r--   0 root         (0) root         (0)     1399 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/src/main/java/helloworld/App.java
--rw-r--r--   0 root         (0) root         (0)      760 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/src/main/java/helloworld/GatewayResponse.java
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.694488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/src/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.694488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/src/test/java/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.754488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/src/test/java/helloworld/
--rw-r--r--   0 root         (0) root         (0)      701 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/src/test/java/helloworld/AppTest.java
--rw-r--r--   0 root         (0) root         (0)     8246 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.754488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/events/
--rw-r--r--   0 root         (0) root         (0)     2121 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/events/event.json
--rw-r--r--   0 root         (0) root         (0)     2046 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/template.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.754488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/
--rw-r--r--   0 root         (0) root         (0)      877 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1651 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/README.md
--rw-r--r--   0 root         (0) root         (0)      150 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/cookiecutter.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.758488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/tests/
--rw-r--r--   0 root         (0) root         (0)     1650 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/tests/test_cookiecutter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.758488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.758488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/HelloWorldFunction/
--rw-r--r--   0 root         (0) root         (0)     1511 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/HelloWorldFunction/pom.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.698488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/HelloWorldFunction/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.698488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/HelloWorldFunction/src/main/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.698488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/HelloWorldFunction/src/main/java/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.758488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/HelloWorldFunction/src/main/java/helloworld/
--rw-r--r--   0 root         (0) root         (0)     1399 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/HelloWorldFunction/src/main/java/helloworld/App.java
--rw-r--r--   0 root         (0) root         (0)      760 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/HelloWorldFunction/src/main/java/helloworld/GatewayResponse.java
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.698488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/HelloWorldFunction/src/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.698488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/HelloWorldFunction/src/test/java/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.758488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/HelloWorldFunction/src/test/java/helloworld/
--rw-r--r--   0 root         (0) root         (0)      701 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/HelloWorldFunction/src/test/java/helloworld/AppTest.java
--rw-r--r--   0 root         (0) root         (0)     8303 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.758488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/events/
--rw-r--r--   0 root         (0) root         (0)     2121 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/events/event.json
--rw-r--r--   0 root         (0) root         (0)     2046 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/template.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.758488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/
--rw-r--r--   0 root         (0) root         (0)     2277 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/.gitignore
--rw-r--r--   0 root         (0) root         (0)      931 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/LICENSE
--rw-r--r--   0 root         (0) root         (0)      722 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/README.md
--rw-r--r--   0 root         (0) root         (0)      154 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/cookiecutter.json
--rw-r--r--   0 root         (0) root         (0)       18 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.758488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/
--rw-r--r--   0 root         (0) root         (0)     2011 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/.gitignore
--rw-r--r--   0 root         (0) root         (0)     8266 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.758488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/events/
--rw-r--r--   0 root         (0) root         (0)     1997 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/events/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.758488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/hello-world/
--rw-r--r--   0 root         (0) root         (0)        8 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/hello-world/.npmignore
--rw-r--r--   0 root         (0) root         (0)     1046 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/hello-world/app.js
--rw-r--r--   0 root         (0) root         (0)      468 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/hello-world/package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.698488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/hello-world/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.758488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/hello-world/tests/unit/
--rw-r--r--   0 root         (0) root         (0)      651 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/hello-world/tests/unit/test-handler.js
--rw-r--r--   0 root         (0) root         (0)     1807 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/template.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.758488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/
--rw-r--r--   0 root         (0) root         (0)     2277 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/.gitignore
--rw-r--r--   0 root         (0) root         (0)      877 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/LICENSE
--rw-r--r--   0 root         (0) root         (0)      772 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/README.md
--rw-r--r--   0 root         (0) root         (0)      153 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/cookiecutter.json
--rw-r--r--   0 root         (0) root         (0)       18 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.758488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/
--rw-r--r--   0 root         (0) root         (0)     3730 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/.gitignore
--rw-r--r--   0 root         (0) root         (0)     8203 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.758488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/events/
--rw-r--r--   0 root         (0) root         (0)     1997 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/events/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.762488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/hello_world/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/hello_world/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1185 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/hello_world/app.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/hello_world/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     1806 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/template.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.702488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.762488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/tests/unit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2607 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/tests/unit/test_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.762488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/
--rw-r--r--   0 root         (0) root         (0)     2277 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/.gitignore
--rw-r--r--   0 root         (0) root         (0)      877 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/LICENSE
--rw-r--r--   0 root         (0) root         (0)      666 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/README.md
--rw-r--r--   0 root         (0) root         (0)      151 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/cookiecutter.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.762488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/
--rw-r--r--   0 root         (0) root         (0)     3730 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/.gitignore
--rw-r--r--   0 root         (0) root         (0)       98 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/Gemfile
--rw-r--r--   0 root         (0) root         (0)     8103 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.762488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/events/
--rw-r--r--   0 root         (0) root         (0)     1997 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/events/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.762488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/hello_world/
--rw-r--r--   0 root         (0) root         (0)       46 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/hello_world/Gemfile
--rw-r--r--   0 root         (0) root         (0)     1126 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/hello_world/app.rb
--rw-r--r--   0 root         (0) root         (0)     1806 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/template.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.702488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.762488 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/tests/unit/
--rw-r--r--   0 root         (0) root         (0)     2887 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/tests/unit/test_handler.rb
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.762488 aws-sam-cli-1.98.0/samcli/lib/intrinsic_resolver/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/intrinsic_resolver/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39540 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/intrinsic_resolver/intrinsic_property_resolver.py
--rw-r--r--   0 root         (0) root         (0)    17270 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/intrinsic_resolver/intrinsics_symbol_table.py
--rw-r--r--   0 root         (0) root         (0)      189 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/intrinsic_resolver/invalid_intrinsic_exception.py
--rw-r--r--   0 root         (0) root         (0)     2940 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/intrinsic_resolver/invalid_intrinsic_validation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.762488 aws-sam-cli-1.98.0/samcli/lib/list/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/list/__init__.py
--rw-r--r--   0 root         (0) root         (0)      286 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/list/data_to_json_mapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.762488 aws-sam-cli-1.98.0/samcli/lib/list/endpoints/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/list/endpoints/__init__.py
--rw-r--r--   0 root         (0) root         (0)      293 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/list/endpoints/endpoints_def.py
--rw-r--r--   0 root         (0) root         (0)    19171 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/list/endpoints/endpoints_producer.py
--rw-r--r--   0 root         (0) root         (0)     3215 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/list/endpoints/endpoints_to_table_mapper.py
--rw-r--r--   0 root         (0) root         (0)     1904 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/list/list_interfaces.py
--rw-r--r--   0 root         (0) root         (0)      256 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/list/mapper_consumer_container.py
--rw-r--r--   0 root         (0) root         (0)     2362 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/list/mapper_consumer_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.762488 aws-sam-cli-1.98.0/samcli/lib/list/resources/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/list/resources/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6798 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/list/resources/resource_mapping_producer.py
--rw-r--r--   0 root         (0) root         (0)      158 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/list/resources/resources_def.py
--rw-r--r--   0 root         (0) root         (0)     1425 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/list/resources/resources_to_table_mapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.766488 aws-sam-cli-1.98.0/samcli/lib/list/stack_outputs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/list/stack_outputs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1484 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/list/stack_outputs/stack_output_to_table_mapper.py
--rw-r--r--   0 root         (0) root         (0)      168 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/list/stack_outputs/stack_outputs.py
--rw-r--r--   0 root         (0) root         (0)     2809 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/list/stack_outputs/stack_outputs_producer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.766488 aws-sam-cli-1.98.0/samcli/lib/observability/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/observability/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.766488 aws-sam-cli-1.98.0/samcli/lib/observability/cw_logs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/observability/cw_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1285 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/observability/cw_logs/cw_log_event.py
--rw-r--r--   0 root         (0) root         (0)     4285 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/observability/cw_logs/cw_log_formatters.py
--rw-r--r--   0 root         (0) root         (0)     5997 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/observability/cw_logs/cw_log_group_provider.py
--rw-r--r--   0 root         (0) root         (0)     5900 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/observability/cw_logs/cw_log_puller.py
--rw-r--r--   0 root         (0) root         (0)     8249 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/observability/observability_info_puller.py
--rw-r--r--   0 root         (0) root         (0)      294 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/observability/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.766488 aws-sam-cli-1.98.0/samcli/lib/observability/xray_traces/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/observability/xray_traces/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6704 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/observability/xray_traces/xray_event_mappers.py
--rw-r--r--   0 root         (0) root         (0)     6919 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/observability/xray_traces/xray_event_puller.py
--rw-r--r--   0 root         (0) root         (0)     5981 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/observability/xray_traces/xray_events.py
--rw-r--r--   0 root         (0) root         (0)     3070 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/observability/xray_traces/xray_service_graph_event_puller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.766488 aws-sam-cli-1.98.0/samcli/lib/package/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/package/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15621 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/package/artifact_exporter.py
--rw-r--r--   0 root         (0) root         (0)     5955 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/package/code_signer.py
--rw-r--r--   0 root         (0) root         (0)     7772 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/package/ecr_uploader.py
--rw-r--r--   0 root         (0) root         (0)      633 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/package/ecr_utils.py
--rw-r--r--   0 root         (0) root         (0)     1826 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/package/image_utils.py
--rw-r--r--   0 root         (0) root         (0)     1672 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/package/local_files_utils.py
--rw-r--r--   0 root         (0) root         (0)    27114 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/package/packageable_resources.py
--rw-r--r--   0 root         (0) root         (0)     3971 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/package/permissions.py
--rw-r--r--   0 root         (0) root         (0)    10395 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/package/s3_uploader.py
--rw-r--r--   0 root         (0) root         (0)     1457 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/package/stream_cursor_utils.py
--rw-r--r--   0 root         (0) root         (0)     1077 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/package/uploaders.py
--rw-r--r--   0 root         (0) root         (0)    13217 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/package/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.766488 aws-sam-cli-1.98.0/samcli/lib/pipeline/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/pipeline/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.766488 aws-sam-cli-1.98.0/samcli/lib/pipeline/bootstrap/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/pipeline/bootstrap/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4411 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/pipeline/bootstrap/resource.py
--rw-r--r--   0 root         (0) root         (0)    23118 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/pipeline/bootstrap/stage.py
--rw-r--r--   0 root         (0) root         (0)    13340 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/pipeline/bootstrap/stage_resources.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.770488 aws-sam-cli-1.98.0/samcli/lib/providers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/providers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11569 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/providers/api_collector.py
--rw-r--r--   0 root         (0) root         (0)     3186 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/providers/api_provider.py
--rw-r--r--   0 root         (0) root         (0)    24524 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/providers/cfn_api_provider.py
--rw-r--r--   0 root         (0) root         (0)    12802 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/providers/cfn_base_api_provider.py
--rw-r--r--   0 root         (0) root         (0)     2411 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/providers/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    34235 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/providers/provider.py
--rw-r--r--   0 root         (0) root         (0)    24457 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/providers/sam_api_provider.py
--rw-r--r--   0 root         (0) root         (0)    11124 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/providers/sam_base_provider.py
--rw-r--r--   0 root         (0) root         (0)    41983 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/providers/sam_function_provider.py
--rw-r--r--   0 root         (0) root         (0)     5866 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/providers/sam_layer_provider.py
--rw-r--r--   0 root         (0) root         (0)    17072 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/providers/sam_stack_provider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.770488 aws-sam-cli-1.98.0/samcli/lib/remote_invoke/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/remote_invoke/__init__.py
--rw-r--r--   0 root         (0) root         (0)      445 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/remote_invoke/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    10417 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/remote_invoke/lambda_invoke_executors.py
--rw-r--r--   0 root         (0) root         (0)     8422 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/remote_invoke/remote_invoke_executor_factory.py
--rw-r--r--   0 root         (0) root         (0)    11158 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/remote_invoke/remote_invoke_executors.py
--rw-r--r--   0 root         (0) root         (0)     6536 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/remote_invoke/stepfunctions_invoke_executors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.770488 aws-sam-cli-1.98.0/samcli/lib/samlib/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/samlib/__init__.py
--rw-r--r--   0 root         (0) root         (0)      840 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/samlib/local_uri_plugin.py
--rw-r--r--   0 root         (0) root         (0)    12061 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/samlib/resource_metadata_normalizer.py
--rw-r--r--   0 root         (0) root         (0)     6037 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/samlib/wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.770488 aws-sam-cli-1.98.0/samcli/lib/schemas/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/schemas/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2304 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/schemas/cli_paginator.py
--rw-r--r--   0 root         (0) root         (0)    19848 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/schemas/schemas_api_caller.py
--rw-r--r--   0 root         (0) root         (0)     3372 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/schemas/schemas_aws_config.py
--rw-r--r--   0 root         (0) root         (0)     1353 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/schemas/schemas_cli_message_generator.py
--rw-r--r--   0 root         (0) root         (0)     3213 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/schemas/schemas_code_manager.py
--rw-r--r--   0 root         (0) root         (0)      447 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/schemas/schemas_constants.py
--rw-r--r--   0 root         (0) root         (0)     1027 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/schemas/schemas_directory_hierarchy_builder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.770488 aws-sam-cli-1.98.0/samcli/lib/shared_test_events/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/shared_test_events/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16499 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/shared_test_events/lambda_shared_test_event.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.770488 aws-sam-cli-1.98.0/samcli/lib/sync/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/sync/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4441 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/sync/continuous_sync_flow_executor.py
--rw-r--r--   0 root         (0) root         (0)     5177 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/sync/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.774488 aws-sam-cli-1.98.0/samcli/lib/sync/flows/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/sync/flows/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3748 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/sync/flows/alias_version_sync_flow.py
--rw-r--r--   0 root         (0) root         (0)     5941 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/sync/flows/auto_dependency_layer_sync_flow.py
--rw-r--r--   0 root         (0) root         (0)     6052 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/sync/flows/function_sync_flow.py
--rw-r--r--   0 root         (0) root         (0)     4103 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/sync/flows/generic_api_sync_flow.py
--rw-r--r--   0 root         (0) root         (0)     2849 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/sync/flows/http_api_sync_flow.py
--rw-r--r--   0 root         (0) root         (0)     7208 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/sync/flows/image_function_sync_flow.py
--rw-r--r--   0 root         (0) root         (0)    18993 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/sync/flows/layer_sync_flow.py
--rw-r--r--   0 root         (0) root         (0)     9275 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/sync/flows/rest_api_sync_flow.py
--rw-r--r--   0 root         (0) root         (0)     5404 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/sync/flows/stepfunctions_sync_flow.py
--rw-r--r--   0 root         (0) root         (0)    11197 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/sync/flows/zip_function_sync_flow.py
--rw-r--r--   0 root         (0) root         (0)    22716 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/sync/infra_sync_executor.py
--rw-r--r--   0 root         (0) root         (0)    16224 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/sync/sync_flow.py
--rw-r--r--   0 root         (0) root         (0)    12842 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/sync/sync_flow_executor.py
--rw-r--r--   0 root         (0) root         (0)    14556 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/sync/sync_flow_factory.py
--rw-r--r--   0 root         (0) root         (0)    15399 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/sync/watch_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.774488 aws-sam-cli-1.98.0/samcli/lib/telemetry/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/telemetry/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4665 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/telemetry/cicd.py
--rw-r--r--   0 root         (0) root         (0)    14425 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/telemetry/event.py
--rw-r--r--   0 root         (0) root         (0)    17162 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/telemetry/metric.py
--rw-r--r--   0 root         (0) root         (0)     4073 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/telemetry/project_metadata.py
--rw-r--r--   0 root         (0) root         (0)     2773 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/telemetry/telemetry.py
--rw-r--r--   0 root         (0) root         (0)      682 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/telemetry/user_agent.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.774488 aws-sam-cli-1.98.0/samcli/lib/translate/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/translate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8473 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/translate/sam_template_validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.778488 aws-sam-cli-1.98.0/samcli/lib/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2535 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/architecture.py
--rw-r--r--   0 root         (0) root         (0)     2895 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/arn_utils.py
--rw-r--r--   0 root         (0) root         (0)     4534 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/async_utils.py
--rw-r--r--   0 root         (0) root         (0)     4431 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/boto_utils.py
--rw-r--r--   0 root         (0) root         (0)     8297 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/cloudformation.py
--rw-r--r--   0 root         (0) root         (0)     4460 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/code_trigger_factory.py
--rw-r--r--   0 root         (0) root         (0)     1202 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/codeuri.py
--rw-r--r--   0 root         (0) root         (0)     3913 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/colors.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/configuration.py
--rw-r--r--   0 root         (0) root         (0)      204 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/defaults.py
--rw-r--r--   0 root         (0) root         (0)     2590 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/definition_validator.py
--rw-r--r--   0 root         (0) root         (0)    24108 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/file_observer.py
--rw-r--r--   0 root         (0) root         (0)     9232 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/git_repo.py
--rw-r--r--   0 root         (0) root         (0)     1589 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/graphql_api.py
--rw-r--r--   0 root         (0) root         (0)     4008 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/hash.py
--rw-r--r--   0 root         (0) root         (0)     4416 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/lock_distributor.py
--rw-r--r--   0 root         (0) root         (0)    12533 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/managed_cloudformation_stack.py
--rw-r--r--   0 root         (0) root         (0)     6463 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/osutils.py
--rw-r--r--   0 root         (0) root         (0)       91 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/packagetype.py
--rw-r--r--   0 root         (0) root         (0)     6436 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/path_observer.py
--rw-r--r--   0 root         (0) root         (0)      429 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/path_utils.py
--rw-r--r--   0 root         (0) root         (0)      218 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/preview_runtimes.py
--rw-r--r--   0 root         (0) root         (0)      195 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/profile.py
--rw-r--r--   0 root         (0) root         (0)      396 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/progressbar.py
--rw-r--r--   0 root         (0) root         (0)    13509 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/resource_trigger.py
--rw-r--r--   0 root         (0) root         (0)     2393 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/resource_type_based_factory.py
--rw-r--r--   0 root         (0) root         (0)     6298 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/resources.py
--rw-r--r--   0 root         (0) root         (0)     1405 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/retry.py
--rw-r--r--   0 root         (0) root         (0)     2456 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/s3.py
--rw-r--r--   0 root         (0) root         (0)     2276 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/sam_logging.py
--rw-r--r--   0 root         (0) root         (0)     1351 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/stream_writer.py
--rw-r--r--   0 root         (0) root         (0)     5724 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/subprocess_utils.py
--rw-r--r--   0 root         (0) root         (0)     2785 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/system_info.py
--rw-r--r--   0 root         (0) root         (0)     2691 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/tar.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/time.py
--rw-r--r--   0 root         (0) root         (0)     4082 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/utils/version_checker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.778488 aws-sam-cli-1.98.0/samcli/lib/warnings/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/warnings/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4957 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/lib/warnings/sam_cli_warning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.778488 aws-sam-cli-1.98.0/samcli/local/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.778488 aws-sam-cli-1.98.0/samcli/local/apigw/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/apigw/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.778488 aws-sam-cli-1.98.0/samcli/local/apigw/authorizers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/apigw/authorizers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      170 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/apigw/authorizers/authorizer.py
--rw-r--r--   0 root         (0) root         (0)    18712 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/apigw/authorizers/lambda_authorizer.py
--rw-r--r--   0 root         (0) root         (0)    10332 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/apigw/event_constructor.py
--rw-r--r--   0 root         (0) root         (0)     1306 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/apigw/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    42181 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/apigw/local_apigw_service.py
--rw-r--r--   0 root         (0) root         (0)     2737 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/apigw/path_converter.py
--rw-r--r--   0 root         (0) root         (0)     3427 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/apigw/route.py
--rw-r--r--   0 root         (0) root         (0)     3681 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/apigw/service_error_responses.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.778488 aws-sam-cli-1.98.0/samcli/local/common/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6188 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/common/runtime_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.778488 aws-sam-cli-1.98.0/samcli/local/docker/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/docker/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22405 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/docker/container.py
--rw-r--r--   0 root         (0) root         (0)     1149 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/docker/effective_user.py
--rw-r--r--   0 root         (0) root         (0)      362 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/docker/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    10508 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/docker/lambda_build_container.py
--rw-r--r--   0 root         (0) root         (0)    11302 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/docker/lambda_container.py
--rw-r--r--   0 root         (0) root         (0)     9327 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/docker/lambda_debug_settings.py
--rw-r--r--   0 root         (0) root         (0)    20678 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/docker/lambda_image.py
--rw-r--r--   0 root         (0) root         (0)     7332 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/docker/manager.py
--rw-r--r--   0 root         (0) root         (0)     3839 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/docker/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.782488 aws-sam-cli-1.98.0/samcli/local/events/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/events/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17708 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/events/api_event.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.782488 aws-sam-cli-1.98.0/samcli/local/lambda_service/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/lambda_service/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7812 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/lambda_service/lambda_error_responses.py
--rw-r--r--   0 root         (0) root         (0)     6785 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/lambda_service/local_lambda_invoke_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.782488 aws-sam-cli-1.98.0/samcli/local/lambdafn/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/lambdafn/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3581 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/lambdafn/config.py
--rw-r--r--   0 root         (0) root         (0)     8743 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/lambdafn/env_vars.py
--rw-r--r--   0 root         (0) root         (0)      273 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/lambdafn/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1793 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/lambdafn/remote_files.py
--rw-r--r--   0 root         (0) root         (0)    23914 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/lambdafn/runtime.py
--rw-r--r--   0 root         (0) root         (0)     4247 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/lambdafn/zip.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.782488 aws-sam-cli-1.98.0/samcli/local/layers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/layers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5967 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/layers/layer_downloader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.786488 aws-sam-cli-1.98.0/samcli/local/rapid/
--rwxr-xr-x   0 root         (0) root         (0)  5373952 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/rapid/aws-lambda-rie-arm64
--rwxr-xr-x   0 root         (0) root         (0)  5582848 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/rapid/aws-lambda-rie-x86_64
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.790488 aws-sam-cli-1.98.0/samcli/local/services/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/services/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6283 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/local/services/base_local_service.py
--rw-r--r--   0 root         (0) root         (0)       79 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/runtime_config.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.790488 aws-sam-cli-1.98.0/samcli/settings/
--rw-r--r--   0 root         (0) root         (0)      832 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/settings/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.790488 aws-sam-cli-1.98.0/samcli/vendor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/vendor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 18:50:17.790488 aws-sam-cli-1.98.0/samcli/vendor/serverlessrepo/
--rw-r--r--   0 root         (0) root         (0)      129 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/vendor/serverlessrepo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2799 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/vendor/serverlessrepo/application_metadata.py
--rw-r--r--   0 root         (0) root         (0)     1534 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/vendor/serverlessrepo/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     3165 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/vendor/serverlessrepo/parser.py
--rw-r--r--   0 root         (0) root         (0)     8417 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/vendor/serverlessrepo/publish.py
--rw-r--r--   0 root         (0) root         (0)     5071 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/samcli/yamlhelper.py
--rw-r--r--   0 root         (0) root         (0)       79 2023-10-03 18:50:17.798488 aws-sam-cli-1.98.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2780 2023-10-03 17:27:22.000000 aws-sam-cli-1.98.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.341447 aws-sam-cli-1.99.0/
+-rw-r--r--   0 root         (0) root         (0)    11387 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      243 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)       89 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    12207 2023-10-18 17:43:05.341447 aws-sam-cli-1.99.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8219 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     9124 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/THIRD-PARTY-LICENSES
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.249446 aws-sam-cli-1.99.0/aws_sam_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12207 2023-10-18 17:43:03.000000 aws-sam-cli-1.99.0/aws_sam_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    37239 2023-10-18 17:43:03.000000 aws-sam-cli-1.99.0/aws_sam_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-10-18 17:43:03.000000 aws-sam-cli-1.99.0/aws_sam_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-10-18 17:43:03.000000 aws-sam-cli-1.99.0/aws_sam_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     1282 2023-10-18 17:43:03.000000 aws-sam-cli-1.99.0/aws_sam_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-10-18 17:43:03.000000 aws-sam-cli-1.99.0/aws_sam_cli.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      792 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.249446 aws-sam-cli-1.99.0/requirements/
+-rw-r--r--   0 root         (0) root         (0)     1099 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/requirements/base.txt
+-rw-r--r--   0 root         (0) root         (0)     1251 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/requirements/dev.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/requirements/pre-dev.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.249446 aws-sam-cli-1.99.0/samcli/
+-rw-r--r--   0 root         (0) root         (0)       48 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      358 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.253446 aws-sam-cli-1.99.0/samcli/cli/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16220 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/cli/cli_config_file.py
+-rw-r--r--   0 root         (0) root         (0)    11226 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/cli/command.py
+-rw-r--r--   0 root         (0) root         (0)     8505 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/cli/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.253446 aws-sam-cli-1.99.0/samcli/cli/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/cli/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3052 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/cli/core/command.py
+-rw-r--r--   0 root         (0) root         (0)      901 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/cli/core/options.py
+-rw-r--r--   0 root         (0) root         (0)     2593 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/cli/formatters.py
+-rw-r--r--   0 root         (0) root         (0)    15124 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/cli/global_config.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/cli/hidden_imports.py
+-rw-r--r--   0 root         (0) root         (0)     1945 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/cli/import_module_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     5650 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/cli/main.py
+-rw-r--r--   0 root         (0) root         (0)     2059 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/cli/options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.253446 aws-sam-cli-1.99.0/samcli/cli/root/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/cli/root/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/cli/root/command_list.py
+-rw-r--r--   0 root         (0) root         (0)     1712 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/cli/row_modifiers.py
+-rw-r--r--   0 root         (0) root         (0)    16898 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/cli/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.253446 aws-sam-cli-1.99.0/samcli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.253446 aws-sam-cli-1.99.0/samcli/commands/_utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1233 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/_utils/cdk_support_decorators.py
+-rw-r--r--   0 root         (0) root         (0)     3894 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/_utils/click_mutex.py
+-rw-r--r--   0 root         (0) root         (0)     3479 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/_utils/command_exception_handler.py
+-rw-r--r--   0 root         (0) root         (0)      368 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/_utils/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.253446 aws-sam-cli-1.99.0/samcli/commands/_utils/custom_options/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/_utils/custom_options/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6726 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/_utils/custom_options/hook_name_option.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/_utils/custom_options/option_nargs.py
+-rw-r--r--   0 root         (0) root         (0)      534 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/_utils/custom_options/replace_help_option.py
+-rw-r--r--   0 root         (0) root         (0)     8878 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/_utils/experimental.py
+-rw-r--r--   0 root         (0) root         (0)      440 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/_utils/option_validator.py
+-rw-r--r--   0 root         (0) root         (0)     2952 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/_utils/option_value_processor.py
+-rw-r--r--   0 root         (0) root         (0)    30733 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/_utils/options.py
+-rw-r--r--   0 root         (0) root         (0)      983 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/_utils/parameterized_option.py
+-rw-r--r--   0 root         (0) root         (0)     5713 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/_utils/table_print.py
+-rw-r--r--   0 root         (0) root         (0)    13274 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/_utils/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.253446 aws-sam-cli-1.99.0/samcli/commands/bootstrap/
+-rw-r--r--   0 root         (0) root         (0)      103 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/bootstrap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/bootstrap/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.257446 aws-sam-cli-1.99.0/samcli/commands/build/
+-rw-r--r--   0 root         (0) root         (0)       91 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/build/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29521 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/build/build_context.py
+-rw-r--r--   0 root         (0) root         (0)      677 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/build/click_container.py
+-rw-r--r--   0 root         (0) root         (0)     8099 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/build/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.257446 aws-sam-cli-1.99.0/samcli/commands/build/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/build/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2811 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/build/core/command.py
+-rw-r--r--   0 root         (0) root         (0)      852 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/build/core/formatters.py
+-rw-r--r--   0 root         (0) root         (0)     2929 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/build/core/options.py
+-rw-r--r--   0 root         (0) root         (0)      333 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/build/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     3562 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/build/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.257446 aws-sam-cli-1.99.0/samcli/commands/delete/
+-rw-r--r--   0 root         (0) root         (0)       92 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/delete/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3845 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/delete/command.py
+-rw-r--r--   0 root         (0) root         (0)    14668 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/delete/delete_context.py
+-rw-r--r--   0 root         (0) root         (0)     2296 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/delete/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.257446 aws-sam-cli-1.99.0/samcli/commands/deploy/
+-rw-r--r--   0 root         (0) root         (0)       92 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/deploy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5746 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/deploy/auth_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2516 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/deploy/code_signer_utils.py
+-rw-r--r--   0 root         (0) root         (0)    12751 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/deploy/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.257446 aws-sam-cli-1.99.0/samcli/commands/deploy/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/deploy/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4552 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/deploy/core/command.py
+-rw-r--r--   0 root         (0) root         (0)      882 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/deploy/core/formatters.py
+-rw-r--r--   0 root         (0) root         (0)     2916 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/deploy/core/options.py
+-rw-r--r--   0 root         (0) root         (0)    12422 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/deploy/deploy_context.py
+-rw-r--r--   0 root         (0) root         (0)     2798 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/deploy/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     5316 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/deploy/guided_config.py
+-rw-r--r--   0 root         (0) root         (0)    26323 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/deploy/guided_context.py
+-rw-r--r--   0 root         (0) root         (0)     4722 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/deploy/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.257446 aws-sam-cli-1.99.0/samcli/commands/docs/
+-rw-r--r--   0 root         (0) root         (0)       90 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/docs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      913 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/docs/command.py
+-rw-r--r--   0 root         (0) root         (0)     4047 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/docs/command_context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.257446 aws-sam-cli-1.99.0/samcli/commands/docs/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/docs/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5461 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/docs/core/command.py
+-rw-r--r--   0 root         (0) root         (0)      566 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/docs/core/formatter.py
+-rw-r--r--   0 root         (0) root         (0)      163 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/docs/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     4576 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.257446 aws-sam-cli-1.99.0/samcli/commands/init/
+-rw-r--r--   0 root         (0) root         (0)       73 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/init/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13529 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/init/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.261446 aws-sam-cli-1.99.0/samcli/commands/init/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/init/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4681 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/init/core/command.py
+-rw-r--r--   0 root         (0) root         (0)      878 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/init/core/formatters.py
+-rw-r--r--   0 root         (0) root         (0)     1955 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/init/core/options.py
+-rw-r--r--   0 root         (0) root         (0)     4617 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/init/init_flow_helpers.py
+-rw-r--r--   0 root         (0) root         (0)      819 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/init/init_generator.py
+-rw-r--r--   0 root         (0) root         (0)    15631 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/init/init_templates.py
+-rw-r--r--   0 root         (0) root         (0)     8249 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/init/interactive_event_bridge_flow.py
+-rw-r--r--   0 root         (0) root         (0)    20316 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/init/interactive_init_flow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.261446 aws-sam-cli-1.99.0/samcli/commands/list/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/list/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.261446 aws-sam-cli-1.99.0/samcli/commands/list/cli_common/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/list/cli_common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      807 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/list/cli_common/list_common_context.py
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/list/cli_common/options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.261446 aws-sam-cli-1.99.0/samcli/commands/list/endpoints/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/list/endpoints/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2257 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/list/endpoints/command.py
+-rw-r--r--   0 root         (0) root         (0)     3163 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/list/endpoints/endpoints_context.py
+-rw-r--r--   0 root         (0) root         (0)     1505 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/list/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      319 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/list/json_consumer.py
+-rw-r--r--   0 root         (0) root         (0)      556 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/list/list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.261446 aws-sam-cli-1.99.0/samcli/commands/list/resources/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/list/resources/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2211 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/list/resources/command.py
+-rw-r--r--   0 root         (0) root         (0)     2018 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/list/resources/resources_context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.261446 aws-sam-cli-1.99.0/samcli/commands/list/stack_outputs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/list/stack_outputs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1636 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/list/stack_outputs/command.py
+-rw-r--r--   0 root         (0) root         (0)     1434 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/list/stack_outputs/stack_outputs_context.py
+-rw-r--r--   0 root         (0) root         (0)     1290 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/list/table_consumer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.261446 aws-sam-cli-1.99.0/samcli/commands/local/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.261446 aws-sam-cli-1.99.0/samcli/commands/local/cli_common/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/cli_common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24015 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/cli_common/invoke_context.py
+-rw-r--r--   0 root         (0) root         (0)     8386 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/cli_common/options.py
+-rw-r--r--   0 root         (0) root         (0)     2055 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/cli_common/user_exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.261446 aws-sam-cli-1.99.0/samcli/commands/local/generate_event/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/generate_event/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      730 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/generate_event/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.261446 aws-sam-cli-1.99.0/samcli/commands/local/generate_event/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/generate_event/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3985 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/generate_event/core/command.py
+-rw-r--r--   0 root         (0) root         (0)     7043 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/generate_event/event_generation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.261446 aws-sam-cli-1.99.0/samcli/commands/local/invoke/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/invoke/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8069 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/invoke/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.261446 aws-sam-cli-1.99.0/samcli/commands/local/invoke/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/invoke/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3647 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/invoke/core/command.py
+-rw-r--r--   0 root         (0) root         (0)      861 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/invoke/core/formatters.py
+-rw-r--r--   0 root         (0) root         (0)     2888 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/invoke/core/options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.265446 aws-sam-cli-1.99.0/samcli/commands/local/lib/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/lib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/lib/debug_context.py
+-rw-r--r--   0 root         (0) root         (0)     1023 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/lib/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     5524 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/lib/local_api_service.py
+-rw-r--r--   0 root         (0) root         (0)    15482 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/lib/local_lambda.py
+-rw-r--r--   0 root         (0) root         (0)     2207 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/lib/local_lambda_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.265446 aws-sam-cli-1.99.0/samcli/commands/local/lib/swagger/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/lib/swagger/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11346 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/lib/swagger/integration_uri.py
+-rw-r--r--   0 root         (0) root         (0)    19348 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/lib/swagger/parser.py
+-rw-r--r--   0 root         (0) root         (0)     9397 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/lib/swagger/reader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.265446 aws-sam-cli-1.99.0/samcli/commands/local/lib/validators/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/lib/validators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2034 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/lib/validators/identity_source_validator.py
+-rw-r--r--   0 root         (0) root         (0)    10881 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/lib/validators/lambda_auth_props.py
+-rw-r--r--   0 root         (0) root         (0)      658 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/local.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.265446 aws-sam-cli-1.99.0/samcli/commands/local/start_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/start_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8283 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/start_api/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.265446 aws-sam-cli-1.99.0/samcli/commands/local/start_api/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/start_api/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1744 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/start_api/core/command.py
+-rw-r--r--   0 root         (0) root         (0)      876 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/start_api/core/formatters.py
+-rw-r--r--   0 root         (0) root         (0)     2918 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/start_api/core/options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.265446 aws-sam-cli-1.99.0/samcli/commands/local/start_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/start_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7170 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/start_lambda/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.265446 aws-sam-cli-1.99.0/samcli/commands/local/start_lambda/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/start_lambda/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4066 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/start_lambda/core/command.py
+-rw-r--r--   0 root         (0) root         (0)      885 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/start_lambda/core/formatters.py
+-rw-r--r--   0 root         (0) root         (0)     2903 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/local/start_lambda/core/options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.265446 aws-sam-cli-1.99.0/samcli/commands/logs/
+-rw-r--r--   0 root         (0) root         (0)       90 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6903 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/logs/command.py
+-rw-r--r--   0 root         (0) root         (0)      848 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/logs/console_consumers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.265446 aws-sam-cli-1.99.0/samcli/commands/logs/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/logs/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5047 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/logs/core/command.py
+-rw-r--r--   0 root         (0) root         (0)      878 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/logs/core/formatters.py
+-rw-r--r--   0 root         (0) root         (0)     1805 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/logs/core/options.py
+-rw-r--r--   0 root         (0) root         (0)     6742 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/logs/logs_context.py
+-rw-r--r--   0 root         (0) root         (0)     7048 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/logs/puller_factory.py
+-rw-r--r--   0 root         (0) root         (0)     2523 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/logs/validation_and_exception_handlers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.265446 aws-sam-cli-1.99.0/samcli/commands/package/
+-rw-r--r--   0 root         (0) root         (0)       93 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/package/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5539 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/package/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.269446 aws-sam-cli-1.99.0/samcli/commands/package/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/package/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5574 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/package/core/command.py
+-rw-r--r--   0 root         (0) root         (0)      884 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/package/core/formatters.py
+-rw-r--r--   0 root         (0) root         (0)     2282 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/package/core/options.py
+-rw-r--r--   0 root         (0) root         (0)     5081 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/package/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     7526 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/package/package_context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.269446 aws-sam-cli-1.99.0/samcli/commands/pipeline/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/pipeline/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.269446 aws-sam-cli-1.99.0/samcli/commands/pipeline/bootstrap/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/pipeline/bootstrap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19260 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/pipeline/bootstrap/cli.py
+-rw-r--r--   0 root         (0) root         (0)    19150 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/pipeline/bootstrap/guided_context.py
+-rw-r--r--   0 root         (0) root         (0)     2801 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/pipeline/bootstrap/oidc_config.py
+-rw-r--r--   0 root         (0) root         (0)     7075 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/pipeline/bootstrap/pipeline_oidc_provider.py
+-rw-r--r--   0 root         (0) root         (0)      429 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/pipeline/external_links.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.269446 aws-sam-cli-1.99.0/samcli/commands/pipeline/init/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/pipeline/init/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2158 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/pipeline/init/cli.py
+-rw-r--r--   0 root         (0) root         (0)    24242 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/pipeline/init/interactive_init_flow.py
+-rw-r--r--   0 root         (0) root         (0)     2398 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/pipeline/init/pipeline_templates_manifest.py
+-rw-r--r--   0 root         (0) root         (0)      455 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/pipeline/pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.269446 aws-sam-cli-1.99.0/samcli/commands/publish/
+-rw-r--r--   0 root         (0) root         (0)       92 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/publish/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6008 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/publish/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.269446 aws-sam-cli-1.99.0/samcli/commands/remote/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      857 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.269446 aws-sam-cli-1.99.0/samcli/commands/remote/invoke/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/invoke/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6303 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/invoke/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.269446 aws-sam-cli-1.99.0/samcli/commands/remote/invoke/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/invoke/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6836 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/invoke/core/command.py
+-rw-r--r--   0 root         (0) root         (0)      865 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/invoke/core/formatters.py
+-rw-r--r--   0 root         (0) root         (0)     1979 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/invoke/core/options.py
+-rw-r--r--   0 root         (0) root         (0)      538 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/remote.py
+-rw-r--r--   0 root         (0) root         (0)    12277 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/remote_invoke_context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.269446 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.269446 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/core/base_options.py
+-rw-r--r--   0 root         (0) root         (0)      872 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/core/formatters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.269446 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/delete/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/delete/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4204 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/delete/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.269446 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/delete/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/delete/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3971 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/delete/core/command.py
+-rw-r--r--   0 root         (0) root         (0)      444 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/delete/core/formatters.py
+-rw-r--r--   0 root         (0) root         (0)     1127 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/delete/core/options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.273446 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/get/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/get/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4780 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/get/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.273446 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/get/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/get/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4726 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/get/core/command.py
+-rw-r--r--   0 root         (0) root         (0)      434 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/get/core/formatters.py
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/get/core/options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.273446 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/list/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/list/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3868 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/list/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.273446 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/list/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/list/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3844 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/list/core/command.py
+-rw-r--r--   0 root         (0) root         (0)      438 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/list/core/formatters.py
+-rw-r--r--   0 root         (0) root         (0)      959 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/list/core/options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.273446 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/put/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/put/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5464 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/put/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.273446 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/put/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/put/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5114 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/put/core/command.py
+-rw-r--r--   0 root         (0) root         (0)      434 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/put/core/formatters.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/put/core/options.py
+-rw-r--r--   0 root         (0) root         (0)      546 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/test_event.py
+-rw-r--r--   0 root         (0) root         (0)     1615 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/remote/test_event/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.273446 aws-sam-cli-1.99.0/samcli/commands/sync/
+-rw-r--r--   0 root         (0) root         (0)       89 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/sync/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20846 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/sync/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.273446 aws-sam-cli-1.99.0/samcli/commands/sync/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/sync/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3892 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/sync/core/command.py
+-rw-r--r--   0 root         (0) root         (0)      927 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/sync/core/formatters.py
+-rw-r--r--   0 root         (0) root         (0)     2315 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/sync/core/options.py
+-rw-r--r--   0 root         (0) root         (0)    10155 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/sync/sync_context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.273446 aws-sam-cli-1.99.0/samcli/commands/traces/
+-rw-r--r--   0 root         (0) root         (0)      106 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/traces/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2920 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/traces/command.py
+-rw-r--r--   0 root         (0) root         (0)      578 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/traces/trace_console_consumers.py
+-rw-r--r--   0 root         (0) root         (0)     4189 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/traces/traces_puller_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.273446 aws-sam-cli-1.99.0/samcli/commands/validate/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/validate/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.273446 aws-sam-cli-1.99.0/samcli/commands/validate/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/validate/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1845 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/validate/core/command.py
+-rw-r--r--   0 root         (0) root         (0)      862 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/validate/core/formatters.py
+-rw-r--r--   0 root         (0) root         (0)     1647 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/validate/core/options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.273446 aws-sam-cli-1.99.0/samcli/commands/validate/lib/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/validate/lib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      158 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/validate/lib/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     7069 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/commands/validate/validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.273446 aws-sam-cli-1.99.0/samcli/hook_packages/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/hook_packages/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.277446 aws-sam-cli-1.99.0/samcli/hook_packages/terraform/
+-rw-r--r--   0 root         (0) root         (0)      425 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/hook_packages/terraform/Config.json
+-rw-r--r--   0 root         (0) root         (0)       64 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/hook_packages/terraform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12097 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/hook_packages/terraform/copy_terraform_built_artifacts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.277446 aws-sam-cli-1.99.0/samcli/hook_packages/terraform/designs/
+-rw-r--r--   0 root         (0) root         (0)     7203 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/hook_packages/terraform/designs/resource_linking_generalized.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.277446 aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.277446 aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1368 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/constants.py
+-rw-r--r--   0 root         (0) root         (0)    28896 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/enrich.py
+-rw-r--r--   0 root         (0) root         (0)    13548 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    10856 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/hook.py
+-rw-r--r--   0 root         (0) root         (0)     9215 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/makefile_generator.py
+-rw-r--r--   0 root         (0) root         (0)    18502 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/property_builder.py
+-rw-r--r--   0 root         (0) root         (0)   111362 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/resource_linking.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.277446 aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/resources/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/resources/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13702 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/resources/apigw.py
+-rw-r--r--   0 root         (0) root         (0)     2375 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/resources/code_resource_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/resources/internal.py
+-rw-r--r--   0 root         (0) root         (0)     2451 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/resources/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     1942 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/resources/lambda_layers.py
+-rw-r--r--   0 root         (0) root         (0)     6339 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/resources/resource_links.py
+-rw-r--r--   0 root         (0) root         (0)     2965 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/resources/resource_properties.py
+-rw-r--r--   0 root         (0) root         (0)    24739 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/translate.py
+-rw-r--r--   0 root         (0) root         (0)     6057 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/types.py
+-rw-r--r--   0 root         (0) root         (0)      495 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.277446 aws-sam-cli-1.99.0/samcli/hook_packages/terraform/lib/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/hook_packages/terraform/lib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2789 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/hook_packages/terraform/lib/utils.py
+-rw-r--r--   0 root         (0) root         (0)      172 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/hook_packages/terraform/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.277446 aws-sam-cli-1.99.0/samcli/lib/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.277446 aws-sam-cli-1.99.0/samcli/lib/bootstrap/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/bootstrap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6348 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/bootstrap/bootstrap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.277446 aws-sam-cli-1.99.0/samcli/lib/bootstrap/companion_stack/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/bootstrap/companion_stack/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3615 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/bootstrap/companion_stack/companion_stack_builder.py
+-rw-r--r--   0 root         (0) root         (0)    12586 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/bootstrap/companion_stack/companion_stack_manager.py
+-rw-r--r--   0 root         (0) root         (0)     5213 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/bootstrap/companion_stack/data_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.281446 aws-sam-cli-1.99.0/samcli/lib/bootstrap/nested_stack/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/bootstrap/nested_stack/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3667 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/bootstrap/nested_stack/nested_stack_builder.py
+-rw-r--r--   0 root         (0) root         (0)     8669 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/bootstrap/nested_stack/nested_stack_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1937 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/bootstrap/stack_builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.281446 aws-sam-cli-1.99.0/samcli/lib/build/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/build/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44620 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/build/app_builder.py
+-rw-r--r--   0 root         (0) root         (0)    28066 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/build/build_graph.py
+-rw-r--r--   0 root         (0) root         (0)    27127 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/build/build_strategy.py
+-rw-r--r--   0 root         (0) root         (0)    10142 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/build/bundler.py
+-rw-r--r--   0 root         (0) root         (0)      304 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/build/constants.py
+-rw-r--r--   0 root         (0) root         (0)     2886 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/build/dependency_hash_generator.py
+-rw-r--r--   0 root         (0) root         (0)     1476 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/build/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2255 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/build/utils.py
+-rw-r--r--   0 root         (0) root         (0)    11865 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/build/workflow_config.py
+-rw-r--r--   0 root         (0) root         (0)     3351 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/build/workflows.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.281446 aws-sam-cli-1.99.0/samcli/lib/cli_validation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/cli_validation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6013 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/cli_validation/image_repository_validation.py
+-rw-r--r--   0 root         (0) root         (0)     2980 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/cli_validation/remote_invoke_options_validations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.281446 aws-sam-cli-1.99.0/samcli/lib/config/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      470 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/config/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     9442 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/config/file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    10585 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/config/samconfig.py
+-rw-r--r--   0 root         (0) root         (0)      122 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/config/version.py
+-rw-r--r--   0 root         (0) root         (0)       32 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.281446 aws-sam-cli-1.99.0/samcli/lib/cookiecutter/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/cookiecutter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      873 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/cookiecutter/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     3384 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/cookiecutter/interactive_flow.py
+-rw-r--r--   0 root         (0) root         (0)     5654 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/cookiecutter/interactive_flow_creator.py
+-rw-r--r--   0 root         (0) root         (0)     1210 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/cookiecutter/plugin.py
+-rw-r--r--   0 root         (0) root         (0)      594 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/cookiecutter/processor.py
+-rw-r--r--   0 root         (0) root         (0)    11820 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/cookiecutter/question.py
+-rw-r--r--   0 root         (0) root         (0)     9214 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/cookiecutter/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.281446 aws-sam-cli-1.99.0/samcli/lib/delete/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/delete/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8633 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/delete/cfn_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.281446 aws-sam-cli-1.99.0/samcli/lib/deploy/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/deploy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34866 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/deploy/deployer.py
+-rw-r--r--   0 root         (0) root         (0)     1359 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/deploy/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.281446 aws-sam-cli-1.99.0/samcli/lib/docker/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/docker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3319 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/docker/log_streamer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.285447 aws-sam-cli-1.99.0/samcli/lib/docs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/docs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1212 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/docs/browser_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     2007 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/docs/documentation.py
+-rw-r--r--   0 root         (0) root         (0)     3405 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/docs/documentation_links.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.285447 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28057 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/event-mapping.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.241446 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.285447 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/alb/
+-rw-r--r--   0 root         (0) root         (0)     1050 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/alb/ALBRequest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.285447 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/alexa-skills-kit/
+-rw-r--r--   0 root         (0) root         (0)      825 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/alexa-skills-kit/AlexaEndSession.json
+-rw-r--r--   0 root         (0) root         (0)     1474 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/alexa-skills-kit/AlexaIntentAnswer.json
+-rw-r--r--   0 root         (0) root         (0)      925 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/alexa-skills-kit/AlexaIntentGetNewFact.json
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/alexa-skills-kit/AlexaIntentMyColorIs.json
+-rw-r--r--   0 root         (0) root         (0)     1005 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/alexa-skills-kit/AlexaIntentRecipe.json
+-rw-r--r--   0 root         (0) root         (0)      851 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/alexa-skills-kit/AlexaStartSession.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.285447 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/alexa-smart-home/
+-rw-r--r--   0 root         (0) root         (0)      365 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/alexa-smart-home/AlexaSmartHomeControlTurnOffRequest.json
+-rw-r--r--   0 root         (0) root         (0)      364 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/alexa-smart-home/AlexaSmartHomeControlTurnOnRequest.json
+-rw-r--r--   0 root         (0) root         (0)      239 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/alexa-smart-home/AlexaSmartHomeDiscoveryRequest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.285447 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/apigateway/
+-rw-r--r--   0 root         (0) root         (0)      207 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/apigateway/ApiGatewayAuthorizer.json
+-rw-r--r--   0 root         (0) root         (0)     1513 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/apigateway/ApiGatewayRestRequestAuthorizer.json
+-rw-r--r--   0 root         (0) root         (0)     3232 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/apigateway/AwsProxy.json
+-rw-r--r--   0 root         (0) root         (0)     1657 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/apigateway/HttpApi.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.285447 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/appsync/
+-rw-r--r--   0 root         (0) root         (0)     2516 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/appsync/AppSyncDirectResolver.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.285447 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/batch/
+-rw-r--r--   0 root         (0) root         (0)       91 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/batch/BatchGetJob.json
+-rw-r--r--   0 root         (0) root         (0)       53 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/batch/BatchSubmitJob.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.285447 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/cloudformation/
+-rw-r--r--   0 root         (0) root         (0)      442 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/cloudformation/CfnCreateRequest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.289446 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/cloudfront/
+-rw-r--r--   0 root         (0) root         (0)      771 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontABTest.json
+-rw-r--r--   0 root         (0) root         (0)      876 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontAccessRequestInResponse.json
+-rw-r--r--   0 root         (0) root         (0)      592 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontHttpRedirect.json
+-rw-r--r--   0 root         (0) root         (0)      790 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontModifyQueryString.json
+-rw-r--r--   0 root         (0) root         (0)      719 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontModifyResponseHeader.json
+-rw-r--r--   0 root         (0) root         (0)      592 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontMultipleRemoteCallsAggregateResponse.json
+-rw-r--r--   0 root         (0) root         (0)      793 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontNormalizeQuerystringToImproveCacheHit.json
+-rw-r--r--   0 root         (0) root         (0)      614 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontRedirectOnViewerCountry.json
+-rw-r--r--   0 root         (0) root         (0)      432 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontRedirectUnauthenticatedUsers.json
+-rw-r--r--   0 root         (0) root         (0)      442 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontResponseGeneration.json
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontServeObjectOnViewerDevice.json
+-rw-r--r--   0 root         (0) root         (0)      744 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontSimpleRemoteCall.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.289446 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/cloudwatch/
+-rw-r--r--   0 root         (0) root         (0)      318 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/cloudwatch/CloudwatchLogs.json
+-rw-r--r--   0 root         (0) root         (0)      325 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/cloudwatch/ScheduledEvent.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.289446 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/codecommit/
+-rw-r--r--   0 root         (0) root         (0)      868 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/codecommit/CodeCommit.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.289446 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/codepipeline/
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/codepipeline/CodePipeline.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.289446 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/cognito/
+-rw-r--r--   0 root         (0) root         (0)      425 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/cognito/CognitoSyncTrigger.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.289446 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/config/
+-rw-r--r--   0 root         (0) root         (0)     1345 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/config/ConfigurationItemChangeNotification.json
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/config/OversizedConfigurationItemChangeNotification.json
+-rw-r--r--   0 root         (0) root         (0)      650 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/config/PeriodicRule.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.289446 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/connect/
+-rw-r--r--   0 root         (0) root         (0)     1084 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/connect/ConnectContactFlowEvent.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.289446 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/dynamodb/
+-rw-r--r--   0 root         (0) root         (0)     2516 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/dynamodb/DynamoDBUpdate.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.289446 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/kinesis/
+-rw-r--r--   0 root         (0) root         (0)      596 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/kinesis/Kinesis.json
+-rw-r--r--   0 root         (0) root         (0)      397 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/kinesis/KinesisAnalytics.json
+-rw-r--r--   0 root         (0) root         (0)     1737 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/kinesis/KinesisAnalyticsKpl.json
+-rw-r--r--   0 root         (0) root         (0)      358 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/kinesis/KinesisFirehose.json
+-rw-r--r--   0 root         (0) root         (0)      261 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/kinesis/KinesisFirehoseApachelog.json
+-rw-r--r--   0 root         (0) root         (0)     2892 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/kinesis/KinesisFirehoseCloudwatchLogsProcessor.json
+-rw-r--r--   0 root         (0) root         (0)      677 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/kinesis/KinesisFirehoseStreamsAsSource.json
+-rw-r--r--   0 root         (0) root         (0)      428 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/kinesis/KinesisFirehoseSyslog.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.289446 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/lex/
+-rw-r--r--   0 root         (0) root         (0)      489 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/lex/LexBookCar.json
+-rw-r--r--   0 root         (0) root         (0)      451 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/lex/LexBookHotel.json
+-rw-r--r--   0 root         (0) root         (0)      443 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/lex/LexMakeAppointment.json
+-rw-r--r--   0 root         (0) root         (0)      441 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/lex/LexOrderFlowers.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.289446 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/lex-v2/
+-rw-r--r--   0 root         (0) root         (0)     3671 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/lex-v2/BankingBot.json
+-rw-r--r--   0 root         (0) root         (0)     2732 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/lex-v2/LexBookCar.json
+-rw-r--r--   0 root         (0) root         (0)     2663 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/lex-v2/LexBookHotel.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.289446 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/rekognition/
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/rekognition/RekognitionS3Request.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.289446 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/s3/
+-rw-r--r--   0 root         (0) root         (0)      341 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/s3/S3BatchInvocation.json
+-rw-r--r--   0 root         (0) root         (0)      943 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/s3/S3Delete.json
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/s3/S3Put.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.289446 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/sagemaker/
+-rw-r--r--   0 root         (0) root         (0)      450 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/sagemaker/AnnotationConsolidation.json
+-rw-r--r--   0 root         (0) root         (0)      223 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/sagemaker/PreHumanTask.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.289446 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/ses/
+-rw-r--r--   0 root         (0) root         (0)     3305 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/ses/SesEmailReceiving.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.289446 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/sns/
+-rw-r--r--   0 root         (0) root         (0)      899 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/sns/Sns.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.289446 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/sqs/
+-rw-r--r--   0 root         (0) root         (0)      617 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/sqs/Sqs.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.289446 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/stepfunctions/
+-rw-r--r--   0 root         (0) root         (0)       58 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/stepfunctions/StepFunctionsError.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.289446 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/workmail/
+-rw-r--r--   0 root         (0) root         (0)      577 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/workmail/WorkMail.json
+-rw-r--r--   0 root         (0) root         (0)     5791 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.293446 aws-sam-cli-1.99.0/samcli/lib/hook/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/hook/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      529 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/hook/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2768 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/hook/hook_config.py
+-rw-r--r--   0 root         (0) root         (0)     2551 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/hook/hook_config_schema.json
+-rw-r--r--   0 root         (0) root         (0)     7224 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/hook/hook_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)      559 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/hook/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.293446 aws-sam-cli-1.99.0/samcli/lib/iac/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/iac/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.293446 aws-sam-cli-1.99.0/samcli/lib/iac/cdk/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/iac/cdk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/iac/cdk/cdk_iac.py
+-rw-r--r--   0 root         (0) root         (0)     1977 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/iac/cdk/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.293446 aws-sam-cli-1.99.0/samcli/lib/iac/cfn/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/iac/cfn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7336 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/iac/cfn/cfn_iac.py
+-rw-r--r--   0 root         (0) root         (0)      132 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/iac/constants.py
+-rw-r--r--   0 root         (0) root         (0)      542 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/iac/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2429 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/iac/iac_factory.py
+-rw-r--r--   0 root         (0) root         (0)    23459 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/iac/plugins_interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.293446 aws-sam-cli-1.99.0/samcli/lib/init/
+-rw-r--r--   0 root         (0) root         (0)     7528 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3605 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/arbitrary_project.py
+-rw-r--r--   0 root         (0) root         (0)     3569 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/default_samconfig.py
+-rw-r--r--   0 root         (0) root         (0)      606 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     4661 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/local_manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.293446 aws-sam-cli-1.99.0/samcli/lib/init/template_modifiers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/template_modifiers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3347 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/template_modifiers/application_insights_template_modifier.py
+-rw-r--r--   0 root         (0) root         (0)     1680 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/template_modifiers/cli_template_modifier.py
+-rw-r--r--   0 root         (0) root         (0)     3346 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/template_modifiers/xray_tracing_template_modifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.245446 aws-sam-cli-1.99.0/samcli/lib/init/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.293446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/
+-rw-r--r--   0 root         (0) root         (0)     2277 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      877 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      165 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/Pipfile
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/README.md
+-rw-r--r--   0 root         (0) root         (0)      151 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/cookiecutter.json
+-rw-r--r--   0 root         (0) root         (0)       18 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.293446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/tests/
+-rw-r--r--   0 root         (0) root         (0)     1499 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/tests/test_cookiecutter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.293446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/
+-rw-r--r--   0 root         (0) root         (0)     7224 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     8084 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.293446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/events/
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/events/event.json
+-rw-r--r--   0 root         (0) root         (0)      175 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/omnisharp.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.241446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.297446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/src/HelloWorld/
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/src/HelloWorld/Function.cs
+-rw-r--r--   0 root         (0) root         (0)      559 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/src/HelloWorld/HelloWorld.csproj
+-rw-r--r--   0 root         (0) root         (0)      692 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/src/HelloWorld/aws-lambda-tools-defaults.json
+-rw-r--r--   0 root         (0) root         (0)     2057 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/template.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.241446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.297446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/test/HelloWorld.Test/
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/test/HelloWorld.Test/FunctionTest.cs
+-rw-r--r--   0 root         (0) root         (0)      688 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/test/HelloWorld.Test/HelloWorld.Tests.csproj
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.297446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/
+-rw-r--r--   0 root         (0) root         (0)     2612 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/README.md
+-rw-r--r--   0 root         (0) root         (0)      125 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/cookiecutter.json
+-rw-r--r--   0 root         (0) root         (0)       70 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/requirements-dev.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.297446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/tests/
+-rw-r--r--   0 root         (0) root         (0)     2239 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/tests/test_bake_project.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.297446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/{{cookiecutter.project_name}}/
+-rw-r--r--   0 root         (0) root         (0)     5168 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/{{cookiecutter.project_name}}/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.297446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/{{cookiecutter.project_name}}/hello-world/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/{{cookiecutter.project_name}}/hello-world/go.mod
+-rw-r--r--   0 root         (0) root         (0)     1096 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/{{cookiecutter.project_name}}/hello-world/main.go
+-rw-r--r--   0 root         (0) root         (0)     1557 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/{{cookiecutter.project_name}}/hello-world/main_test.go
+-rw-r--r--   0 root         (0) root         (0)     2059 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/{{cookiecutter.project_name}}/template.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.297446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/
+-rw-r--r--   0 root         (0) root         (0)      877 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1651 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/README.md
+-rw-r--r--   0 root         (0) root         (0)      150 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/cookiecutter.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.297446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/tests/
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/tests/test_cookiecutter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.297446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.297446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/
+-rw-r--r--   0 root         (0) root         (0)      185 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/build.gradle
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.245446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/gradle/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.297446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/gradle/wrapper/
+-rw-r--r--   0 root         (0) root         (0)    55190 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/gradle/wrapper/gradle-wrapper.jar
+-rw-r--r--   0 root         (0) root         (0)      202 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/gradle/wrapper/gradle-wrapper.properties
+-rwxr-xr-x   0 root         (0) root         (0)     5305 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/gradlew
+-rw-r--r--   0 root         (0) root         (0)     2269 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/gradlew.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.245446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.245446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/src/main/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.245446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/src/main/java/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.297446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/src/main/java/helloworld/
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/src/main/java/helloworld/App.java
+-rw-r--r--   0 root         (0) root         (0)      760 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/src/main/java/helloworld/GatewayResponse.java
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.245446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/src/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.245446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/src/test/java/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.297446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/src/test/java/helloworld/
+-rw-r--r--   0 root         (0) root         (0)      701 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/src/test/java/helloworld/AppTest.java
+-rw-r--r--   0 root         (0) root         (0)     8246 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.297446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/events/
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/events/event.json
+-rw-r--r--   0 root         (0) root         (0)     2046 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/template.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.297446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/
+-rw-r--r--   0 root         (0) root         (0)      877 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1651 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/README.md
+-rw-r--r--   0 root         (0) root         (0)      150 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/cookiecutter.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.297446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/tests/
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/tests/test_cookiecutter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.297446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.297446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/HelloWorldFunction/
+-rw-r--r--   0 root         (0) root         (0)     1511 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/HelloWorldFunction/pom.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.245446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/HelloWorldFunction/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.245446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/HelloWorldFunction/src/main/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.245446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/HelloWorldFunction/src/main/java/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.301447 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/HelloWorldFunction/src/main/java/helloworld/
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/HelloWorldFunction/src/main/java/helloworld/App.java
+-rw-r--r--   0 root         (0) root         (0)      760 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/HelloWorldFunction/src/main/java/helloworld/GatewayResponse.java
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.245446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/HelloWorldFunction/src/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.245446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/HelloWorldFunction/src/test/java/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.301447 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/HelloWorldFunction/src/test/java/helloworld/
+-rw-r--r--   0 root         (0) root         (0)      701 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/HelloWorldFunction/src/test/java/helloworld/AppTest.java
+-rw-r--r--   0 root         (0) root         (0)     8303 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.301447 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/events/
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/events/event.json
+-rw-r--r--   0 root         (0) root         (0)     2046 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/template.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.301447 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/
+-rw-r--r--   0 root         (0) root         (0)     2277 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      931 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      722 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/README.md
+-rw-r--r--   0 root         (0) root         (0)      154 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/cookiecutter.json
+-rw-r--r--   0 root         (0) root         (0)       18 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.301447 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/
+-rw-r--r--   0 root         (0) root         (0)     2011 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     8266 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.301447 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/events/
+-rw-r--r--   0 root         (0) root         (0)     1997 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/events/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.301447 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/hello-world/
+-rw-r--r--   0 root         (0) root         (0)        8 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/hello-world/.npmignore
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/hello-world/app.js
+-rw-r--r--   0 root         (0) root         (0)      468 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/hello-world/package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.245446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/hello-world/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.301447 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/hello-world/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)      651 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/hello-world/tests/unit/test-handler.js
+-rw-r--r--   0 root         (0) root         (0)     1807 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/template.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.301447 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/
+-rw-r--r--   0 root         (0) root         (0)     2277 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      877 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      772 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/README.md
+-rw-r--r--   0 root         (0) root         (0)      153 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/cookiecutter.json
+-rw-r--r--   0 root         (0) root         (0)       18 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.301447 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/
+-rw-r--r--   0 root         (0) root         (0)     3730 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     8203 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.301447 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/events/
+-rw-r--r--   0 root         (0) root         (0)     1997 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/events/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.301447 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/hello_world/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/hello_world/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1185 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/hello_world/app.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/hello_world/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     1806 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/template.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.245446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.301447 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/tests/unit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2607 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/tests/unit/test_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.301447 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/
+-rw-r--r--   0 root         (0) root         (0)     2277 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      877 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      666 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/README.md
+-rw-r--r--   0 root         (0) root         (0)      151 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/cookiecutter.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.305446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/
+-rw-r--r--   0 root         (0) root         (0)     3730 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/.gitignore
+-rw-r--r--   0 root         (0) root         (0)       98 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/Gemfile
+-rw-r--r--   0 root         (0) root         (0)     8103 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.305446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/events/
+-rw-r--r--   0 root         (0) root         (0)     1997 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/events/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.305446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/hello_world/
+-rw-r--r--   0 root         (0) root         (0)       46 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/hello_world/Gemfile
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/hello_world/app.rb
+-rw-r--r--   0 root         (0) root         (0)     1806 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/template.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.245446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.305446 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)     2887 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/tests/unit/test_handler.rb
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.305446 aws-sam-cli-1.99.0/samcli/lib/intrinsic_resolver/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/intrinsic_resolver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39540 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/intrinsic_resolver/intrinsic_property_resolver.py
+-rw-r--r--   0 root         (0) root         (0)    17270 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/intrinsic_resolver/intrinsics_symbol_table.py
+-rw-r--r--   0 root         (0) root         (0)      189 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/intrinsic_resolver/invalid_intrinsic_exception.py
+-rw-r--r--   0 root         (0) root         (0)     2940 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/intrinsic_resolver/invalid_intrinsic_validation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.305446 aws-sam-cli-1.99.0/samcli/lib/list/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/list/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      286 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/list/data_to_json_mapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.305446 aws-sam-cli-1.99.0/samcli/lib/list/endpoints/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/list/endpoints/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      293 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/list/endpoints/endpoints_def.py
+-rw-r--r--   0 root         (0) root         (0)    19171 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/list/endpoints/endpoints_producer.py
+-rw-r--r--   0 root         (0) root         (0)     3215 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/list/endpoints/endpoints_to_table_mapper.py
+-rw-r--r--   0 root         (0) root         (0)     1904 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/list/list_interfaces.py
+-rw-r--r--   0 root         (0) root         (0)      256 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/list/mapper_consumer_container.py
+-rw-r--r--   0 root         (0) root         (0)     2362 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/list/mapper_consumer_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.305446 aws-sam-cli-1.99.0/samcli/lib/list/resources/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/list/resources/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6798 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/list/resources/resource_mapping_producer.py
+-rw-r--r--   0 root         (0) root         (0)      158 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/list/resources/resources_def.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/list/resources/resources_to_table_mapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.305446 aws-sam-cli-1.99.0/samcli/lib/list/stack_outputs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/list/stack_outputs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1484 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/list/stack_outputs/stack_output_to_table_mapper.py
+-rw-r--r--   0 root         (0) root         (0)      168 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/list/stack_outputs/stack_outputs.py
+-rw-r--r--   0 root         (0) root         (0)     2809 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/list/stack_outputs/stack_outputs_producer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.305446 aws-sam-cli-1.99.0/samcli/lib/observability/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/observability/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.305446 aws-sam-cli-1.99.0/samcli/lib/observability/cw_logs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/observability/cw_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1285 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/observability/cw_logs/cw_log_event.py
+-rw-r--r--   0 root         (0) root         (0)     4285 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/observability/cw_logs/cw_log_formatters.py
+-rw-r--r--   0 root         (0) root         (0)     5997 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/observability/cw_logs/cw_log_group_provider.py
+-rw-r--r--   0 root         (0) root         (0)     5900 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/observability/cw_logs/cw_log_puller.py
+-rw-r--r--   0 root         (0) root         (0)     8249 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/observability/observability_info_puller.py
+-rw-r--r--   0 root         (0) root         (0)      294 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/observability/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.309446 aws-sam-cli-1.99.0/samcli/lib/observability/xray_traces/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/observability/xray_traces/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6704 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/observability/xray_traces/xray_event_mappers.py
+-rw-r--r--   0 root         (0) root         (0)     6919 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/observability/xray_traces/xray_event_puller.py
+-rw-r--r--   0 root         (0) root         (0)     5981 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/observability/xray_traces/xray_events.py
+-rw-r--r--   0 root         (0) root         (0)     3070 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/observability/xray_traces/xray_service_graph_event_puller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.309446 aws-sam-cli-1.99.0/samcli/lib/package/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/package/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15621 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/package/artifact_exporter.py
+-rw-r--r--   0 root         (0) root         (0)     5955 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/package/code_signer.py
+-rw-r--r--   0 root         (0) root         (0)     7772 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/package/ecr_uploader.py
+-rw-r--r--   0 root         (0) root         (0)      633 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/package/ecr_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1826 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/package/image_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1672 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/package/local_files_utils.py
+-rw-r--r--   0 root         (0) root         (0)    27114 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/package/packageable_resources.py
+-rw-r--r--   0 root         (0) root         (0)     3971 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/package/permissions.py
+-rw-r--r--   0 root         (0) root         (0)    10395 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/package/s3_uploader.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/package/stream_cursor_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1077 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/package/uploaders.py
+-rw-r--r--   0 root         (0) root         (0)    13217 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/package/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.309446 aws-sam-cli-1.99.0/samcli/lib/pipeline/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/pipeline/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.309446 aws-sam-cli-1.99.0/samcli/lib/pipeline/bootstrap/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/pipeline/bootstrap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4411 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/pipeline/bootstrap/resource.py
+-rw-r--r--   0 root         (0) root         (0)    23118 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/pipeline/bootstrap/stage.py
+-rw-r--r--   0 root         (0) root         (0)    13340 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/pipeline/bootstrap/stage_resources.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.309446 aws-sam-cli-1.99.0/samcli/lib/providers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/providers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11569 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/providers/api_collector.py
+-rw-r--r--   0 root         (0) root         (0)     3186 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/providers/api_provider.py
+-rw-r--r--   0 root         (0) root         (0)    24524 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/providers/cfn_api_provider.py
+-rw-r--r--   0 root         (0) root         (0)    12802 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/providers/cfn_base_api_provider.py
+-rw-r--r--   0 root         (0) root         (0)     2411 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/providers/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    34235 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/providers/provider.py
+-rw-r--r--   0 root         (0) root         (0)    24457 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/providers/sam_api_provider.py
+-rw-r--r--   0 root         (0) root         (0)    11124 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/providers/sam_base_provider.py
+-rw-r--r--   0 root         (0) root         (0)    41983 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/providers/sam_function_provider.py
+-rw-r--r--   0 root         (0) root         (0)     5866 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/providers/sam_layer_provider.py
+-rw-r--r--   0 root         (0) root         (0)    17072 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/providers/sam_stack_provider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.313447 aws-sam-cli-1.99.0/samcli/lib/remote_invoke/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/remote_invoke/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      445 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/remote_invoke/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     4833 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/remote_invoke/kinesis_invoke_executors.py
+-rw-r--r--   0 root         (0) root         (0)    10417 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/remote_invoke/lambda_invoke_executors.py
+-rw-r--r--   0 root         (0) root         (0)    12083 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/remote_invoke/remote_invoke_executor_factory.py
+-rw-r--r--   0 root         (0) root         (0)    11158 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/remote_invoke/remote_invoke_executors.py
+-rw-r--r--   0 root         (0) root         (0)     6620 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/remote_invoke/sqs_invoke_executors.py
+-rw-r--r--   0 root         (0) root         (0)     6536 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/remote_invoke/stepfunctions_invoke_executors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.313447 aws-sam-cli-1.99.0/samcli/lib/samlib/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/samlib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      840 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/samlib/local_uri_plugin.py
+-rw-r--r--   0 root         (0) root         (0)    12061 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/samlib/resource_metadata_normalizer.py
+-rw-r--r--   0 root         (0) root         (0)     6037 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/samlib/wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.313447 aws-sam-cli-1.99.0/samcli/lib/schemas/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/schemas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2304 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/schemas/cli_paginator.py
+-rw-r--r--   0 root         (0) root         (0)    19848 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/schemas/schemas_api_caller.py
+-rw-r--r--   0 root         (0) root         (0)     3372 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/schemas/schemas_aws_config.py
+-rw-r--r--   0 root         (0) root         (0)     1353 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/schemas/schemas_cli_message_generator.py
+-rw-r--r--   0 root         (0) root         (0)     3213 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/schemas/schemas_code_manager.py
+-rw-r--r--   0 root         (0) root         (0)      447 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/schemas/schemas_constants.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/schemas/schemas_directory_hierarchy_builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.313447 aws-sam-cli-1.99.0/samcli/lib/shared_test_events/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/shared_test_events/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16499 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/shared_test_events/lambda_shared_test_event.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.313447 aws-sam-cli-1.99.0/samcli/lib/sync/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/sync/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4441 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/sync/continuous_sync_flow_executor.py
+-rw-r--r--   0 root         (0) root         (0)     5177 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/sync/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.313447 aws-sam-cli-1.99.0/samcli/lib/sync/flows/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/sync/flows/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3748 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/sync/flows/alias_version_sync_flow.py
+-rw-r--r--   0 root         (0) root         (0)     5941 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/sync/flows/auto_dependency_layer_sync_flow.py
+-rw-r--r--   0 root         (0) root         (0)     6052 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/sync/flows/function_sync_flow.py
+-rw-r--r--   0 root         (0) root         (0)     4103 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/sync/flows/generic_api_sync_flow.py
+-rw-r--r--   0 root         (0) root         (0)     2849 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/sync/flows/http_api_sync_flow.py
+-rw-r--r--   0 root         (0) root         (0)     7208 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/sync/flows/image_function_sync_flow.py
+-rw-r--r--   0 root         (0) root         (0)    18993 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/sync/flows/layer_sync_flow.py
+-rw-r--r--   0 root         (0) root         (0)     9275 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/sync/flows/rest_api_sync_flow.py
+-rw-r--r--   0 root         (0) root         (0)     5404 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/sync/flows/stepfunctions_sync_flow.py
+-rw-r--r--   0 root         (0) root         (0)    11197 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/sync/flows/zip_function_sync_flow.py
+-rw-r--r--   0 root         (0) root         (0)    22716 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/sync/infra_sync_executor.py
+-rw-r--r--   0 root         (0) root         (0)    16224 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/sync/sync_flow.py
+-rw-r--r--   0 root         (0) root         (0)    12842 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/sync/sync_flow_executor.py
+-rw-r--r--   0 root         (0) root         (0)    14556 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/sync/sync_flow_factory.py
+-rw-r--r--   0 root         (0) root         (0)    15399 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/sync/watch_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.317447 aws-sam-cli-1.99.0/samcli/lib/telemetry/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/telemetry/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4665 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/telemetry/cicd.py
+-rw-r--r--   0 root         (0) root         (0)    14425 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/telemetry/event.py
+-rw-r--r--   0 root         (0) root         (0)    17162 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/telemetry/metric.py
+-rw-r--r--   0 root         (0) root         (0)     4073 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/telemetry/project_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     2773 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/telemetry/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)      682 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/telemetry/user_agent.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.317447 aws-sam-cli-1.99.0/samcli/lib/translate/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/translate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8473 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/translate/sam_template_validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.321447 aws-sam-cli-1.99.0/samcli/lib/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2535 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/architecture.py
+-rw-r--r--   0 root         (0) root         (0)     2895 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/arn_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4534 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/async_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4431 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/boto_utils.py
+-rw-r--r--   0 root         (0) root         (0)     8297 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/cloudformation.py
+-rw-r--r--   0 root         (0) root         (0)     4460 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/code_trigger_factory.py
+-rw-r--r--   0 root         (0) root         (0)     1202 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/codeuri.py
+-rw-r--r--   0 root         (0) root         (0)     3913 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/colors.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/configuration.py
+-rw-r--r--   0 root         (0) root         (0)      204 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/defaults.py
+-rw-r--r--   0 root         (0) root         (0)     2590 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/definition_validator.py
+-rw-r--r--   0 root         (0) root         (0)    24108 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/file_observer.py
+-rw-r--r--   0 root         (0) root         (0)     9232 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/git_repo.py
+-rw-r--r--   0 root         (0) root         (0)     1589 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/graphql_api.py
+-rw-r--r--   0 root         (0) root         (0)     4008 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/hash.py
+-rw-r--r--   0 root         (0) root         (0)     4416 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/lock_distributor.py
+-rw-r--r--   0 root         (0) root         (0)    12549 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/managed_cloudformation_stack.py
+-rw-r--r--   0 root         (0) root         (0)     6463 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/osutils.py
+-rw-r--r--   0 root         (0) root         (0)       91 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/packagetype.py
+-rw-r--r--   0 root         (0) root         (0)     6436 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/path_observer.py
+-rw-r--r--   0 root         (0) root         (0)      429 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/path_utils.py
+-rw-r--r--   0 root         (0) root         (0)      218 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/preview_runtimes.py
+-rw-r--r--   0 root         (0) root         (0)      195 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/profile.py
+-rw-r--r--   0 root         (0) root         (0)      396 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/progressbar.py
+-rw-r--r--   0 root         (0) root         (0)    13509 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/resource_trigger.py
+-rw-r--r--   0 root         (0) root         (0)     2393 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/resource_type_based_factory.py
+-rw-r--r--   0 root         (0) root         (0)     6298 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/resources.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/retry.py
+-rw-r--r--   0 root         (0) root         (0)     2456 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/s3.py
+-rw-r--r--   0 root         (0) root         (0)     2276 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/sam_logging.py
+-rw-r--r--   0 root         (0) root         (0)     1351 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/stream_writer.py
+-rw-r--r--   0 root         (0) root         (0)     5724 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/subprocess_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2785 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/system_info.py
+-rw-r--r--   0 root         (0) root         (0)     2691 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/tar.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/time.py
+-rw-r--r--   0 root         (0) root         (0)     4082 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/utils/version_checker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.321447 aws-sam-cli-1.99.0/samcli/lib/warnings/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/warnings/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4957 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/lib/warnings/sam_cli_warning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.321447 aws-sam-cli-1.99.0/samcli/local/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.321447 aws-sam-cli-1.99.0/samcli/local/apigw/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/apigw/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.321447 aws-sam-cli-1.99.0/samcli/local/apigw/authorizers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/apigw/authorizers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      170 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/apigw/authorizers/authorizer.py
+-rw-r--r--   0 root         (0) root         (0)    18712 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/apigw/authorizers/lambda_authorizer.py
+-rw-r--r--   0 root         (0) root         (0)    10332 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/apigw/event_constructor.py
+-rw-r--r--   0 root         (0) root         (0)     1306 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/apigw/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    42181 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/apigw/local_apigw_service.py
+-rw-r--r--   0 root         (0) root         (0)     2737 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/apigw/path_converter.py
+-rw-r--r--   0 root         (0) root         (0)     3427 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/apigw/route.py
+-rw-r--r--   0 root         (0) root         (0)     3681 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/apigw/service_error_responses.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.321447 aws-sam-cli-1.99.0/samcli/local/common/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6188 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/common/runtime_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.321447 aws-sam-cli-1.99.0/samcli/local/docker/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/docker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22405 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/docker/container.py
+-rw-r--r--   0 root         (0) root         (0)     1149 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/docker/effective_user.py
+-rw-r--r--   0 root         (0) root         (0)      362 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/docker/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    10508 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/docker/lambda_build_container.py
+-rw-r--r--   0 root         (0) root         (0)    11302 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/docker/lambda_container.py
+-rw-r--r--   0 root         (0) root         (0)     9327 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/docker/lambda_debug_settings.py
+-rw-r--r--   0 root         (0) root         (0)    20678 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/docker/lambda_image.py
+-rw-r--r--   0 root         (0) root         (0)     7332 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/docker/manager.py
+-rw-r--r--   0 root         (0) root         (0)     3839 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/docker/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.321447 aws-sam-cli-1.99.0/samcli/local/events/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/events/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17708 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/events/api_event.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.325446 aws-sam-cli-1.99.0/samcli/local/lambda_service/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/lambda_service/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7812 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/lambda_service/lambda_error_responses.py
+-rw-r--r--   0 root         (0) root         (0)     6785 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/lambda_service/local_lambda_invoke_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.325446 aws-sam-cli-1.99.0/samcli/local/lambdafn/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/lambdafn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3581 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/lambdafn/config.py
+-rw-r--r--   0 root         (0) root         (0)     8743 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/lambdafn/env_vars.py
+-rw-r--r--   0 root         (0) root         (0)      273 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/lambdafn/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1793 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/lambdafn/remote_files.py
+-rw-r--r--   0 root         (0) root         (0)    23914 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/lambdafn/runtime.py
+-rw-r--r--   0 root         (0) root         (0)     4247 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/lambdafn/zip.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.325446 aws-sam-cli-1.99.0/samcli/local/layers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/layers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5967 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/layers/layer_downloader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.329447 aws-sam-cli-1.99.0/samcli/local/rapid/
+-rwxr-xr-x   0 root         (0) root         (0)  5373952 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/rapid/aws-lambda-rie-arm64
+-rwxr-xr-x   0 root         (0) root         (0)  5582848 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/rapid/aws-lambda-rie-x86_64
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.333447 aws-sam-cli-1.99.0/samcli/local/services/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/services/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6283 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/local/services/base_local_service.py
+-rw-r--r--   0 root         (0) root         (0)       79 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/runtime_config.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.333447 aws-sam-cli-1.99.0/samcli/settings/
+-rw-r--r--   0 root         (0) root         (0)      832 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/settings/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.333447 aws-sam-cli-1.99.0/samcli/vendor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/vendor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-18 17:43:05.333447 aws-sam-cli-1.99.0/samcli/vendor/serverlessrepo/
+-rw-r--r--   0 root         (0) root         (0)      129 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/vendor/serverlessrepo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2799 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/vendor/serverlessrepo/application_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/vendor/serverlessrepo/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     3165 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/vendor/serverlessrepo/parser.py
+-rw-r--r--   0 root         (0) root         (0)     8417 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/vendor/serverlessrepo/publish.py
+-rw-r--r--   0 root         (0) root         (0)     5071 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/samcli/yamlhelper.py
+-rw-r--r--   0 root         (0) root         (0)       79 2023-10-18 17:43:05.341447 aws-sam-cli-1.99.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2780 2023-10-18 16:20:28.000000 aws-sam-cli-1.99.0/setup.py
```

### Comparing `aws-sam-cli-1.98.0/LICENSE` & `aws-sam-cli-1.99.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/PKG-INFO` & `aws-sam-cli-1.99.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-sam-cli
-Version: 1.98.0
+Version: 1.99.0
 Summary: AWS SAM CLI is a CLI tool for local development and testing of Serverless applications
 Home-page: https://github.com/aws/aws-sam-cli
 Author: Amazon Web Services
 Author-email: aws-sam-developers@amazon.com
 License: Apache License 2.0
 Keywords: AWS SAM CLI
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,32 +27,32 @@
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: chevron~=0.12
 Requires-Dist: click~=8.1
 Requires-Dist: Flask<2.4
 Requires-Dist: boto3<2,>=1.26.109
 Requires-Dist: jmespath~=1.0.1
-Requires-Dist: ruamel_yaml~=0.17.32
+Requires-Dist: ruamel_yaml~=0.17.35
 Requires-Dist: PyYAML>=6.0.1,~=6.0
-Requires-Dist: cookiecutter~=2.3.0
-Requires-Dist: aws-sam-translator==1.75.0
+Requires-Dist: cookiecutter~=2.3.1
+Requires-Dist: aws-sam-translator==1.77.0
 Requires-Dist: docker~=6.1.0
 Requires-Dist: dateparser~=1.1
 Requires-Dist: requests~=2.31.0
-Requires-Dist: aws_lambda_builders==1.38.0
+Requires-Dist: aws_lambda_builders==1.40.0
 Requires-Dist: tomlkit==0.12.1
 Requires-Dist: watchdog==3.0.0
 Requires-Dist: rich~=13.5.3
 Requires-Dist: pyopenssl~=23.2.0
 Requires-Dist: jsonschema<4.20
 Requires-Dist: typing_extensions<5,>=4.4.0
 Requires-Dist: regex!=2021.10.8
 Requires-Dist: tzlocal==5.0.1
-Requires-Dist: cfn-lint~=0.80.3
-Requires-Dist: boto3-stubs[apigateway,cloudformation,ecr,iam,lambda,s3,schemas,secretsmanager,signer,stepfunctions,sts,xray]==1.28.55
+Requires-Dist: cfn-lint~=0.81.0
+Requires-Dist: boto3-stubs[apigateway,cloudformation,ecr,iam,kinesis,lambda,s3,schemas,secretsmanager,signer,sqs,stepfunctions,sts,xray]==1.28.62
 Provides-Extra: pre-dev
 Requires-Dist: ruff==0.0.291; extra == "pre-dev"
 Provides-Extra: dev
 Requires-Dist: ruff==0.0.291; extra == "dev"
 Requires-Dist: coverage==7.2.7; python_version < "3.8" and extra == "dev"
 Requires-Dist: coverage==7.3.1; python_version >= "3.8" and extra == "dev"
 Requires-Dist: pytest-cov==4.1.0; extra == "dev"
@@ -71,15 +71,15 @@
 Requires-Dist: types-pyOpenSSL==23.2.0.2; extra == "dev"
 Requires-Dist: types-requests==2.31.0.2; extra == "dev"
 Requires-Dist: types-urllib3==1.26.25.14; extra == "dev"
 Requires-Dist: pytest~=7.4.2; extra == "dev"
 Requires-Dist: parameterized==0.9.0; extra == "dev"
 Requires-Dist: pytest-xdist==3.3.1; extra == "dev"
 Requires-Dist: pytest-forked==1.6.0; extra == "dev"
-Requires-Dist: pytest-timeout==2.1.0; extra == "dev"
+Requires-Dist: pytest-timeout==2.2.0; extra == "dev"
 Requires-Dist: pytest-rerunfailures==12.0; extra == "dev"
 Requires-Dist: pytest-metadata==2.0.4; extra == "dev"
 Requires-Dist: pytest-json-report==1.5.0; extra == "dev"
 Requires-Dist: filelock==3.12.2; python_version < "3.8" and extra == "dev"
 Requires-Dist: filelock==3.12.4; python_version >= "3.8" and extra == "dev"
 Requires-Dist: black==22.6.0; python_version < "3.8" and extra == "dev"
 Requires-Dist: black==23.9.1; python_version >= "3.8" and extra == "dev"
```

### Comparing `aws-sam-cli-1.98.0/README.md` & `aws-sam-cli-1.99.0/README.md`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/THIRD-PARTY-LICENSES` & `aws-sam-cli-1.99.0/THIRD-PARTY-LICENSES`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/aws_sam_cli.egg-info/PKG-INFO` & `aws-sam-cli-1.99.0/aws_sam_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-sam-cli
-Version: 1.98.0
+Version: 1.99.0
 Summary: AWS SAM CLI is a CLI tool for local development and testing of Serverless applications
 Home-page: https://github.com/aws/aws-sam-cli
 Author: Amazon Web Services
 Author-email: aws-sam-developers@amazon.com
 License: Apache License 2.0
 Keywords: AWS SAM CLI
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,32 +27,32 @@
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: chevron~=0.12
 Requires-Dist: click~=8.1
 Requires-Dist: Flask<2.4
 Requires-Dist: boto3<2,>=1.26.109
 Requires-Dist: jmespath~=1.0.1
-Requires-Dist: ruamel_yaml~=0.17.32
+Requires-Dist: ruamel_yaml~=0.17.35
 Requires-Dist: PyYAML>=6.0.1,~=6.0
-Requires-Dist: cookiecutter~=2.3.0
-Requires-Dist: aws-sam-translator==1.75.0
+Requires-Dist: cookiecutter~=2.3.1
+Requires-Dist: aws-sam-translator==1.77.0
 Requires-Dist: docker~=6.1.0
 Requires-Dist: dateparser~=1.1
 Requires-Dist: requests~=2.31.0
-Requires-Dist: aws_lambda_builders==1.38.0
+Requires-Dist: aws_lambda_builders==1.40.0
 Requires-Dist: tomlkit==0.12.1
 Requires-Dist: watchdog==3.0.0
 Requires-Dist: rich~=13.5.3
 Requires-Dist: pyopenssl~=23.2.0
 Requires-Dist: jsonschema<4.20
 Requires-Dist: typing_extensions<5,>=4.4.0
 Requires-Dist: regex!=2021.10.8
 Requires-Dist: tzlocal==5.0.1
-Requires-Dist: cfn-lint~=0.80.3
-Requires-Dist: boto3-stubs[apigateway,cloudformation,ecr,iam,lambda,s3,schemas,secretsmanager,signer,stepfunctions,sts,xray]==1.28.55
+Requires-Dist: cfn-lint~=0.81.0
+Requires-Dist: boto3-stubs[apigateway,cloudformation,ecr,iam,kinesis,lambda,s3,schemas,secretsmanager,signer,sqs,stepfunctions,sts,xray]==1.28.62
 Provides-Extra: pre-dev
 Requires-Dist: ruff==0.0.291; extra == "pre-dev"
 Provides-Extra: dev
 Requires-Dist: ruff==0.0.291; extra == "dev"
 Requires-Dist: coverage==7.2.7; python_version < "3.8" and extra == "dev"
 Requires-Dist: coverage==7.3.1; python_version >= "3.8" and extra == "dev"
 Requires-Dist: pytest-cov==4.1.0; extra == "dev"
@@ -71,15 +71,15 @@
 Requires-Dist: types-pyOpenSSL==23.2.0.2; extra == "dev"
 Requires-Dist: types-requests==2.31.0.2; extra == "dev"
 Requires-Dist: types-urllib3==1.26.25.14; extra == "dev"
 Requires-Dist: pytest~=7.4.2; extra == "dev"
 Requires-Dist: parameterized==0.9.0; extra == "dev"
 Requires-Dist: pytest-xdist==3.3.1; extra == "dev"
 Requires-Dist: pytest-forked==1.6.0; extra == "dev"
-Requires-Dist: pytest-timeout==2.1.0; extra == "dev"
+Requires-Dist: pytest-timeout==2.2.0; extra == "dev"
 Requires-Dist: pytest-rerunfailures==12.0; extra == "dev"
 Requires-Dist: pytest-metadata==2.0.4; extra == "dev"
 Requires-Dist: pytest-json-report==1.5.0; extra == "dev"
 Requires-Dist: filelock==3.12.2; python_version < "3.8" and extra == "dev"
 Requires-Dist: filelock==3.12.4; python_version >= "3.8" and extra == "dev"
 Requires-Dist: black==22.6.0; python_version < "3.8" and extra == "dev"
 Requires-Dist: black==23.9.1; python_version >= "3.8" and extra == "dev"
```

### Comparing `aws-sam-cli-1.98.0/aws_sam_cli.egg-info/SOURCES.txt` & `aws-sam-cli-1.99.0/aws_sam_cli.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -577,17 +577,19 @@
 samcli/lib/providers/sam_api_provider.py
 samcli/lib/providers/sam_base_provider.py
 samcli/lib/providers/sam_function_provider.py
 samcli/lib/providers/sam_layer_provider.py
 samcli/lib/providers/sam_stack_provider.py
 samcli/lib/remote_invoke/__init__.py
 samcli/lib/remote_invoke/exceptions.py
+samcli/lib/remote_invoke/kinesis_invoke_executors.py
 samcli/lib/remote_invoke/lambda_invoke_executors.py
 samcli/lib/remote_invoke/remote_invoke_executor_factory.py
 samcli/lib/remote_invoke/remote_invoke_executors.py
+samcli/lib/remote_invoke/sqs_invoke_executors.py
 samcli/lib/remote_invoke/stepfunctions_invoke_executors.py
 samcli/lib/samlib/__init__.py
 samcli/lib/samlib/local_uri_plugin.py
 samcli/lib/samlib/resource_metadata_normalizer.py
 samcli/lib/samlib/wrapper.py
 samcli/lib/schemas/__init__.py
 samcli/lib/schemas/cli_paginator.py
```

### Comparing `aws-sam-cli-1.98.0/aws_sam_cli.egg-info/requires.txt` & `aws-sam-cli-1.99.0/aws_sam_cli.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 chevron~=0.12
 click~=8.1
 Flask<2.4
 boto3<2,>=1.26.109
 jmespath~=1.0.1
-ruamel_yaml~=0.17.32
+ruamel_yaml~=0.17.35
 PyYAML>=6.0.1,~=6.0
-cookiecutter~=2.3.0
-aws-sam-translator==1.75.0
+cookiecutter~=2.3.1
+aws-sam-translator==1.77.0
 docker~=6.1.0
 dateparser~=1.1
 requests~=2.31.0
-aws_lambda_builders==1.38.0
+aws_lambda_builders==1.40.0
 tomlkit==0.12.1
 watchdog==3.0.0
 rich~=13.5.3
 pyopenssl~=23.2.0
 jsonschema<4.20
 typing_extensions<5,>=4.4.0
 regex!=2021.10.8
 tzlocal==5.0.1
-cfn-lint~=0.80.3
-boto3-stubs[apigateway,cloudformation,ecr,iam,lambda,s3,schemas,secretsmanager,signer,stepfunctions,sts,xray]==1.28.55
+cfn-lint~=0.81.0
+boto3-stubs[apigateway,cloudformation,ecr,iam,kinesis,lambda,s3,schemas,secretsmanager,signer,sqs,stepfunctions,sts,xray]==1.28.62
 
 [dev]
 ruff==0.0.291
 pytest-cov==4.1.0
 types-pywin32==306.0.0.4
 types-PyYAML==6.0.12.11
 types-chevron==0.14.2.5
@@ -38,15 +38,15 @@
 types-pyOpenSSL==23.2.0.2
 types-requests==2.31.0.2
 types-urllib3==1.26.25.14
 pytest~=7.4.2
 parameterized==0.9.0
 pytest-xdist==3.3.1
 pytest-forked==1.6.0
-pytest-timeout==2.1.0
+pytest-timeout==2.2.0
 pytest-rerunfailures==12.0
 pytest-metadata==2.0.4
 pytest-json-report==1.5.0
 psutil==5.9.5
 
 [dev:python_version < "3.8"]
 coverage==7.2.7
```

### Comparing `aws-sam-cli-1.98.0/pyproject.toml` & `aws-sam-cli-1.99.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/requirements/base.txt` & `aws-sam-cli-1.99.0/requirements/base.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 chevron~=0.12
 click~=8.1
 Flask<2.4
 boto3>=1.26.109,<2
 jmespath~=1.0.1
-ruamel_yaml~=0.17.32
+ruamel_yaml~=0.17.35
 PyYAML~=6.0,>=6.0.1
-cookiecutter~=2.3.0
-aws-sam-translator==1.75.0
+cookiecutter~=2.3.1
+aws-sam-translator==1.77.0
 #docker minor version updates can include breaking changes. Auto update micro version only.
 docker~=6.1.0
 dateparser~=1.1
 requests~=2.31.0
-aws_lambda_builders==1.38.0
+aws_lambda_builders==1.40.0
 tomlkit==0.12.1
 watchdog==3.0.0
 rich~=13.5.3
 pyopenssl~=23.2.0
 # Pin to <4.18 to until SAM-T no longer uses RefResolver
 jsonschema<4.20
 
@@ -24,11 +24,11 @@
 
 # NOTE: regex is not a direct dependency of SAM CLI, exclude version 2021.10.8 due to not working on M1 Mac - https://github.com/mrabarnett/mrab-regex/issues/399
 regex!=2021.10.8
 # NOTE: tzlocal is not a direct dependency of SAM CLI, but pin to 3.0 as 4.0 break appveyor jobs
 tzlocal==5.0.1
 
 #Adding cfn-lint dependency for SAM validate
-cfn-lint~=0.80.3
+cfn-lint~=0.81.0
 
 # Type checking boto3 objects
-boto3-stubs[apigateway,cloudformation,ecr,iam,lambda,s3,schemas,secretsmanager,signer,stepfunctions,sts,xray]==1.28.55
+boto3-stubs[apigateway,cloudformation,ecr,iam,lambda,s3,schemas,secretsmanager,signer,stepfunctions,sts,xray,sqs,kinesis]==1.28.62
```

### Comparing `aws-sam-cli-1.98.0/requirements/dev.txt` & `aws-sam-cli-1.99.0/requirements/dev.txt`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 types-urllib3==1.26.25.14
 
 # Test requirements
 pytest~=7.4.2
 parameterized==0.9.0
 pytest-xdist==3.3.1
 pytest-forked==1.6.0
-pytest-timeout==2.1.0
+pytest-timeout==2.2.0
 pytest-rerunfailures==12.0
 # NOTE (hawflau): DO NOT upgrade pytest-metadata and pytest-json-report unless pytest-json-report addresses https://github.com/numirias/pytest-json-report/issues/89
 pytest-metadata==2.0.4
 pytest-json-report==1.5.0
 filelock==3.12.2; python_version < "3.8"
 filelock==3.12.4; python_version >= "3.8"
```

### Comparing `aws-sam-cli-1.98.0/samcli/cli/cli_config_file.py` & `aws-sam-cli-1.99.0/samcli/cli/cli_config_file.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/cli/command.py` & `aws-sam-cli-1.99.0/samcli/cli/command.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/cli/context.py` & `aws-sam-cli-1.99.0/samcli/cli/context.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/cli/core/command.py` & `aws-sam-cli-1.99.0/samcli/cli/core/command.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/cli/core/options.py` & `aws-sam-cli-1.99.0/samcli/cli/core/options.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/cli/formatters.py` & `aws-sam-cli-1.99.0/samcli/cli/formatters.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/cli/global_config.py` & `aws-sam-cli-1.99.0/samcli/cli/global_config.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/cli/hidden_imports.py` & `aws-sam-cli-1.99.0/samcli/cli/hidden_imports.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/cli/import_module_proxy.py` & `aws-sam-cli-1.99.0/samcli/cli/import_module_proxy.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/cli/main.py` & `aws-sam-cli-1.99.0/samcli/cli/main.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/cli/options.py` & `aws-sam-cli-1.99.0/samcli/cli/options.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/cli/root/command_list.py` & `aws-sam-cli-1.99.0/samcli/cli/root/command_list.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/cli/row_modifiers.py` & `aws-sam-cli-1.99.0/samcli/cli/row_modifiers.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/cli/types.py` & `aws-sam-cli-1.99.0/samcli/cli/types.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/_utils/cdk_support_decorators.py` & `aws-sam-cli-1.99.0/samcli/commands/_utils/cdk_support_decorators.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/_utils/click_mutex.py` & `aws-sam-cli-1.99.0/samcli/commands/_utils/click_mutex.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/_utils/command_exception_handler.py` & `aws-sam-cli-1.99.0/samcli/commands/_utils/command_exception_handler.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/_utils/custom_options/hook_name_option.py` & `aws-sam-cli-1.99.0/samcli/commands/_utils/custom_options/hook_name_option.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/_utils/custom_options/option_nargs.py` & `aws-sam-cli-1.99.0/samcli/commands/_utils/custom_options/option_nargs.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/_utils/custom_options/replace_help_option.py` & `aws-sam-cli-1.99.0/samcli/commands/_utils/custom_options/replace_help_option.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/_utils/experimental.py` & `aws-sam-cli-1.99.0/samcli/commands/_utils/experimental.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/_utils/option_value_processor.py` & `aws-sam-cli-1.99.0/samcli/commands/_utils/option_value_processor.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/_utils/options.py` & `aws-sam-cli-1.99.0/samcli/commands/_utils/options.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/_utils/parameterized_option.py` & `aws-sam-cli-1.99.0/samcli/commands/_utils/parameterized_option.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/_utils/table_print.py` & `aws-sam-cli-1.99.0/samcli/commands/_utils/table_print.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/_utils/template.py` & `aws-sam-cli-1.99.0/samcli/commands/_utils/template.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/bootstrap/command.py` & `aws-sam-cli-1.99.0/samcli/commands/bootstrap/command.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/build/build_context.py` & `aws-sam-cli-1.99.0/samcli/commands/build/build_context.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/build/click_container.py` & `aws-sam-cli-1.99.0/samcli/commands/build/click_container.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/build/command.py` & `aws-sam-cli-1.99.0/samcli/commands/build/command.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/build/core/command.py` & `aws-sam-cli-1.99.0/samcli/commands/build/core/command.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/build/core/formatters.py` & `aws-sam-cli-1.99.0/samcli/commands/build/core/formatters.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/build/core/options.py` & `aws-sam-cli-1.99.0/samcli/commands/build/core/options.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/build/utils.py` & `aws-sam-cli-1.99.0/samcli/commands/build/utils.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/delete/command.py` & `aws-sam-cli-1.99.0/samcli/commands/delete/command.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/delete/delete_context.py` & `aws-sam-cli-1.99.0/samcli/commands/delete/delete_context.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/delete/exceptions.py` & `aws-sam-cli-1.99.0/samcli/commands/delete/exceptions.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/deploy/auth_utils.py` & `aws-sam-cli-1.99.0/samcli/commands/deploy/auth_utils.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/deploy/code_signer_utils.py` & `aws-sam-cli-1.99.0/samcli/commands/deploy/code_signer_utils.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/deploy/command.py` & `aws-sam-cli-1.99.0/samcli/commands/deploy/command.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/deploy/core/command.py` & `aws-sam-cli-1.99.0/samcli/commands/deploy/core/command.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/deploy/core/formatters.py` & `aws-sam-cli-1.99.0/samcli/commands/deploy/core/formatters.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/deploy/core/options.py` & `aws-sam-cli-1.99.0/samcli/commands/deploy/core/options.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/deploy/deploy_context.py` & `aws-sam-cli-1.99.0/samcli/commands/deploy/deploy_context.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/deploy/exceptions.py` & `aws-sam-cli-1.99.0/samcli/commands/deploy/exceptions.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/deploy/guided_config.py` & `aws-sam-cli-1.99.0/samcli/commands/deploy/guided_config.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/deploy/guided_context.py` & `aws-sam-cli-1.99.0/samcli/commands/deploy/guided_context.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/deploy/utils.py` & `aws-sam-cli-1.99.0/samcli/commands/deploy/utils.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/docs/command.py` & `aws-sam-cli-1.99.0/samcli/commands/docs/command.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/docs/command_context.py` & `aws-sam-cli-1.99.0/samcli/commands/docs/command_context.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/docs/core/command.py` & `aws-sam-cli-1.99.0/samcli/commands/docs/core/command.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/docs/core/formatter.py` & `aws-sam-cli-1.99.0/samcli/commands/docs/core/formatter.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/exceptions.py` & `aws-sam-cli-1.99.0/samcli/commands/exceptions.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/init/command.py` & `aws-sam-cli-1.99.0/samcli/commands/init/command.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/init/core/command.py` & `aws-sam-cli-1.99.0/samcli/commands/init/core/command.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/init/core/formatters.py` & `aws-sam-cli-1.99.0/samcli/commands/init/core/formatters.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/init/core/options.py` & `aws-sam-cli-1.99.0/samcli/commands/init/core/options.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/init/init_flow_helpers.py` & `aws-sam-cli-1.99.0/samcli/commands/init/init_flow_helpers.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/init/init_generator.py` & `aws-sam-cli-1.99.0/samcli/commands/init/init_generator.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/init/init_templates.py` & `aws-sam-cli-1.99.0/samcli/commands/init/init_templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -280,15 +280,15 @@
         if the manifest can't be spooled, it attempts to clone the cli template git repo or
         use local cli template
         """
         try:
             response = requests.get(MANIFEST_URL, timeout=10)
             body = response.text
             # if the commit is not exist then MANIFEST_URL will be invalid, fall back to use manifest in latest commit
-            if response.status_code == Status.NOT_FOUND:
+            if response.status_code == Status.NOT_FOUND.value:
                 LOG.warning(
                     "Request to MANIFEST_URL: %s failed, the commit hash in this url maybe invalid, "
                     "Using manifest.json in the latest commit instead.",
                     MANIFEST_URL,
                 )
                 raise ManifestNotFoundException()
```

### Comparing `aws-sam-cli-1.98.0/samcli/commands/init/interactive_event_bridge_flow.py` & `aws-sam-cli-1.99.0/samcli/commands/init/interactive_event_bridge_flow.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/init/interactive_init_flow.py` & `aws-sam-cli-1.99.0/samcli/commands/init/interactive_init_flow.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/list/cli_common/list_common_context.py` & `aws-sam-cli-1.99.0/samcli/commands/list/cli_common/list_common_context.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/list/cli_common/options.py` & `aws-sam-cli-1.99.0/samcli/commands/list/cli_common/options.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/list/endpoints/command.py` & `aws-sam-cli-1.99.0/samcli/commands/list/endpoints/command.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/list/endpoints/endpoints_context.py` & `aws-sam-cli-1.99.0/samcli/commands/list/endpoints/endpoints_context.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/list/exceptions.py` & `aws-sam-cli-1.99.0/samcli/commands/list/exceptions.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/list/list.py` & `aws-sam-cli-1.99.0/samcli/commands/list/list.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/list/resources/command.py` & `aws-sam-cli-1.99.0/samcli/commands/list/resources/command.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/list/resources/resources_context.py` & `aws-sam-cli-1.99.0/samcli/commands/list/resources/resources_context.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/list/stack_outputs/command.py` & `aws-sam-cli-1.99.0/samcli/commands/list/stack_outputs/command.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/list/stack_outputs/stack_outputs_context.py` & `aws-sam-cli-1.99.0/samcli/commands/list/stack_outputs/stack_outputs_context.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/list/table_consumer.py` & `aws-sam-cli-1.99.0/samcli/commands/list/table_consumer.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/local/cli_common/invoke_context.py` & `aws-sam-cli-1.99.0/samcli/commands/local/cli_common/invoke_context.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/local/cli_common/options.py` & `aws-sam-cli-1.99.0/samcli/commands/local/cli_common/options.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/local/cli_common/user_exceptions.py` & `aws-sam-cli-1.99.0/samcli/commands/local/cli_common/user_exceptions.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/local/generate_event/cli.py` & `aws-sam-cli-1.99.0/samcli/commands/local/generate_event/cli.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/local/generate_event/core/command.py` & `aws-sam-cli-1.99.0/samcli/commands/local/generate_event/core/command.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/local/generate_event/event_generation.py` & `aws-sam-cli-1.99.0/samcli/commands/local/generate_event/event_generation.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/local/invoke/cli.py` & `aws-sam-cli-1.99.0/samcli/commands/local/invoke/cli.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/local/invoke/core/command.py` & `aws-sam-cli-1.99.0/samcli/commands/local/invoke/core/command.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/local/invoke/core/formatters.py` & `aws-sam-cli-1.99.0/samcli/commands/local/invoke/core/formatters.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/local/invoke/core/options.py` & `aws-sam-cli-1.99.0/samcli/commands/local/invoke/core/options.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/local/lib/debug_context.py` & `aws-sam-cli-1.99.0/samcli/commands/local/lib/debug_context.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/local/lib/exceptions.py` & `aws-sam-cli-1.99.0/samcli/commands/local/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/local/lib/local_api_service.py` & `aws-sam-cli-1.99.0/samcli/commands/local/lib/local_api_service.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/local/lib/local_lambda.py` & `aws-sam-cli-1.99.0/samcli/commands/local/lib/local_lambda.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/local/lib/local_lambda_service.py` & `aws-sam-cli-1.99.0/samcli/commands/local/lib/local_lambda_service.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/local/lib/swagger/integration_uri.py` & `aws-sam-cli-1.99.0/samcli/commands/local/lib/swagger/integration_uri.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/local/lib/swagger/parser.py` & `aws-sam-cli-1.99.0/samcli/commands/local/lib/swagger/parser.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/local/lib/swagger/reader.py` & `aws-sam-cli-1.99.0/samcli/commands/local/lib/swagger/reader.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/local/lib/validators/identity_source_validator.py` & `aws-sam-cli-1.99.0/samcli/commands/local/lib/validators/identity_source_validator.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/local/lib/validators/lambda_auth_props.py` & `aws-sam-cli-1.99.0/samcli/commands/local/lib/validators/lambda_auth_props.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/local/local.py` & `aws-sam-cli-1.99.0/samcli/commands/local/local.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/local/start_api/cli.py` & `aws-sam-cli-1.99.0/samcli/commands/local/start_api/cli.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/local/start_api/core/command.py` & `aws-sam-cli-1.99.0/samcli/commands/local/start_api/core/command.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/local/start_api/core/formatters.py` & `aws-sam-cli-1.99.0/samcli/commands/local/start_api/core/formatters.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/local/start_api/core/options.py` & `aws-sam-cli-1.99.0/samcli/commands/local/start_api/core/options.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/local/start_lambda/cli.py` & `aws-sam-cli-1.99.0/samcli/commands/local/start_lambda/cli.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/local/start_lambda/core/command.py` & `aws-sam-cli-1.99.0/samcli/commands/local/start_lambda/core/command.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/local/start_lambda/core/formatters.py` & `aws-sam-cli-1.99.0/samcli/commands/local/start_lambda/core/formatters.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/local/start_lambda/core/options.py` & `aws-sam-cli-1.99.0/samcli/commands/local/start_lambda/core/options.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/logs/command.py` & `aws-sam-cli-1.99.0/samcli/commands/logs/command.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/logs/console_consumers.py` & `aws-sam-cli-1.99.0/samcli/commands/logs/console_consumers.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/logs/core/command.py` & `aws-sam-cli-1.99.0/samcli/commands/logs/core/command.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/logs/core/formatters.py` & `aws-sam-cli-1.99.0/samcli/commands/logs/core/formatters.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/logs/core/options.py` & `aws-sam-cli-1.99.0/samcli/commands/logs/core/options.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/logs/logs_context.py` & `aws-sam-cli-1.99.0/samcli/commands/logs/logs_context.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/logs/puller_factory.py` & `aws-sam-cli-1.99.0/samcli/commands/logs/puller_factory.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/logs/validation_and_exception_handlers.py` & `aws-sam-cli-1.99.0/samcli/commands/logs/validation_and_exception_handlers.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/package/command.py` & `aws-sam-cli-1.99.0/samcli/commands/package/command.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/package/core/command.py` & `aws-sam-cli-1.99.0/samcli/commands/package/core/command.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/package/core/formatters.py` & `aws-sam-cli-1.99.0/samcli/commands/package/core/formatters.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/package/core/options.py` & `aws-sam-cli-1.99.0/samcli/commands/package/core/options.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/package/exceptions.py` & `aws-sam-cli-1.99.0/samcli/commands/package/exceptions.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/package/package_context.py` & `aws-sam-cli-1.99.0/samcli/commands/package/package_context.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/pipeline/bootstrap/cli.py` & `aws-sam-cli-1.99.0/samcli/commands/pipeline/bootstrap/cli.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/pipeline/bootstrap/guided_context.py` & `aws-sam-cli-1.99.0/samcli/commands/pipeline/bootstrap/guided_context.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/pipeline/bootstrap/oidc_config.py` & `aws-sam-cli-1.99.0/samcli/commands/pipeline/bootstrap/oidc_config.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/pipeline/bootstrap/pipeline_oidc_provider.py` & `aws-sam-cli-1.99.0/samcli/commands/pipeline/bootstrap/pipeline_oidc_provider.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/pipeline/init/cli.py` & `aws-sam-cli-1.99.0/samcli/commands/pipeline/init/cli.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/pipeline/init/interactive_init_flow.py` & `aws-sam-cli-1.99.0/samcli/commands/pipeline/init/interactive_init_flow.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/pipeline/init/pipeline_templates_manifest.py` & `aws-sam-cli-1.99.0/samcli/commands/pipeline/init/pipeline_templates_manifest.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/publish/command.py` & `aws-sam-cli-1.99.0/samcli/commands/publish/command.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/remote/exceptions.py` & `aws-sam-cli-1.99.0/samcli/commands/remote/exceptions.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/remote/invoke/cli.py` & `aws-sam-cli-1.99.0/samcli/commands/remote/invoke/cli.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/remote/invoke/core/command.py` & `aws-sam-cli-1.99.0/samcli/commands/remote/invoke/core/command.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/remote/invoke/core/formatters.py` & `aws-sam-cli-1.99.0/samcli/commands/remote/invoke/core/formatters.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/remote/invoke/core/options.py` & `aws-sam-cli-1.99.0/samcli/commands/remote/invoke/core/options.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/remote/remote.py` & `aws-sam-cli-1.99.0/samcli/commands/remote/remote.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/remote/remote_invoke_context.py` & `aws-sam-cli-1.99.0/samcli/commands/remote/remote_invoke_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,33 +11,35 @@
     AmbiguousResourceForRemoteInvoke,
     InvalidRemoteInvokeParameters,
     InvalidStackNameProvidedForRemoteInvoke,
     NoResourceFoundForRemoteInvoke,
     ResourceNotSupportedForRemoteInvoke,
     UnsupportedServiceForRemoteInvoke,
 )
+from samcli.lib.remote_invoke.exceptions import ErrorBotoApiCallException
 from samcli.lib.remote_invoke.remote_invoke_executor_factory import RemoteInvokeExecutorFactory
 from samcli.lib.remote_invoke.remote_invoke_executors import (
     RemoteInvokeConsumer,
     RemoteInvokeExecutionInfo,
     RemoteInvokeLogOutput,
     RemoteInvokeResponse,
 )
+from samcli.lib.remote_invoke.sqs_invoke_executors import get_queue_url_from_arn
 from samcli.lib.schemas.schemas_api_caller import SchemasApiCaller
 from samcli.lib.shared_test_events.lambda_shared_test_event import LambdaSharedTestEvent
 from samcli.lib.utils import osutils
 from samcli.lib.utils.arn_utils import ARNParts, InvalidArnValue
 from samcli.lib.utils.boto_utils import BotoProviderType, get_client_error_code
 from samcli.lib.utils.cloudformation import (
     CloudFormationResourceSummary,
     get_resource_summaries,
     get_resource_summary,
     get_resource_summary_from_physical_id,
 )
-from samcli.lib.utils.resources import AWS_LAMBDA_FUNCTION
+from samcli.lib.utils.resources import AWS_KINESIS_STREAM, AWS_LAMBDA_FUNCTION, AWS_SQS_QUEUE
 from samcli.lib.utils.stream_writer import StreamWriter
 
 LOG = logging.getLogger(__name__)
 
 
 SUPPORTED_SERVICES = {"lambda": AWS_LAMBDA_FUNCTION}
 
@@ -203,14 +205,25 @@
 
             if service_from_arn not in SUPPORTED_SERVICES:
                 raise UnsupportedServiceForRemoteInvoke(
                     f"{service_from_arn} is not supported service, "
                     f"please use an ARN for following services, {SUPPORTED_SERVICES}"
                 )
 
+            if SUPPORTED_SERVICES.get(service_from_arn) == AWS_SQS_QUEUE:
+                # SQS queue_url is used for calling boto3 API calls
+                # Note (hnnasit): Add unit test after AWS_SQS_QUEUE is added to SUPPORTED_SERVICES
+                sqs_client = self._boto_client_provider("sqs")
+                resource_id = get_queue_url_from_arn(sqs_client, resource_arn.resource_id)
+
+            if SUPPORTED_SERVICES.get(service_from_arn) == AWS_KINESIS_STREAM:
+                # Note (hnnasit): Add unit test after AWS_KINESIS_STREAM is added to SUPPORTED_SERVICES
+                # StreamName extracted from arn is used as resource_id.
+                resource_id = resource_arn.resource_id
+
             return CloudFormationResourceSummary(
                 cast(str, SUPPORTED_SERVICES.get(service_from_arn)),
                 resource_id,
                 resource_id,
             )
         except InvalidArnValue:
             LOG.debug(
@@ -219,14 +232,19 @@
             resource_summary = get_resource_summary_from_physical_id(self._boto_client_provider, resource_id)
             if not resource_summary:
                 raise AmbiguousResourceForRemoteInvoke(
                     f"Can't find exact resource information with given {self._resource_id}. "
                     f"Please provide full resource ARN or --stack-name to resolve the ambiguity."
                 )
             return resource_summary
+        except ErrorBotoApiCallException:
+            raise AmbiguousResourceForRemoteInvoke(
+                f"Can't find exact resource information with given {self._resource_id}. "
+                f"Please provide the correct ARN or --stack-name to resolve the ambiguity."
+            )
 
     @property
     def stdout(self) -> StreamWriter:
         """
         Returns stream writer for stdout to output Lambda function logs to
 
         Returns
```

### Comparing `aws-sam-cli-1.98.0/samcli/commands/remote/test_event/core/base_options.py` & `aws-sam-cli-1.99.0/samcli/commands/remote/test_event/core/base_options.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/remote/test_event/core/formatters.py` & `aws-sam-cli-1.99.0/samcli/commands/remote/test_event/core/formatters.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/remote/test_event/delete/cli.py` & `aws-sam-cli-1.99.0/samcli/commands/remote/test_event/delete/cli.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/remote/test_event/delete/core/command.py` & `aws-sam-cli-1.99.0/samcli/commands/remote/test_event/delete/core/command.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/remote/test_event/delete/core/options.py` & `aws-sam-cli-1.99.0/samcli/commands/remote/test_event/delete/core/options.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/remote/test_event/get/cli.py` & `aws-sam-cli-1.99.0/samcli/commands/remote/test_event/get/cli.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/remote/test_event/get/core/command.py` & `aws-sam-cli-1.99.0/samcli/commands/remote/test_event/get/core/command.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/remote/test_event/get/core/options.py` & `aws-sam-cli-1.99.0/samcli/commands/remote/test_event/get/core/options.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/remote/test_event/list/cli.py` & `aws-sam-cli-1.99.0/samcli/commands/remote/test_event/list/cli.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/remote/test_event/list/core/command.py` & `aws-sam-cli-1.99.0/samcli/commands/remote/test_event/list/core/command.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/remote/test_event/list/core/options.py` & `aws-sam-cli-1.99.0/samcli/commands/remote/test_event/list/core/options.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/remote/test_event/put/cli.py` & `aws-sam-cli-1.99.0/samcli/commands/remote/test_event/put/cli.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/remote/test_event/put/core/command.py` & `aws-sam-cli-1.99.0/samcli/commands/remote/test_event/put/core/command.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/remote/test_event/put/core/options.py` & `aws-sam-cli-1.99.0/samcli/commands/remote/test_event/put/core/options.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/remote/test_event/test_event.py` & `aws-sam-cli-1.99.0/samcli/commands/remote/test_event/test_event.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/remote/test_event/utils.py` & `aws-sam-cli-1.99.0/samcli/commands/remote/test_event/utils.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/sync/command.py` & `aws-sam-cli-1.99.0/samcli/commands/sync/command.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/sync/core/command.py` & `aws-sam-cli-1.99.0/samcli/commands/sync/core/command.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/sync/core/formatters.py` & `aws-sam-cli-1.99.0/samcli/commands/sync/core/formatters.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/sync/core/options.py` & `aws-sam-cli-1.99.0/samcli/commands/sync/core/options.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/sync/sync_context.py` & `aws-sam-cli-1.99.0/samcli/commands/sync/sync_context.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/traces/command.py` & `aws-sam-cli-1.99.0/samcli/commands/traces/command.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/traces/trace_console_consumers.py` & `aws-sam-cli-1.99.0/samcli/commands/traces/trace_console_consumers.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/traces/traces_puller_factory.py` & `aws-sam-cli-1.99.0/samcli/commands/traces/traces_puller_factory.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/validate/core/command.py` & `aws-sam-cli-1.99.0/samcli/commands/validate/core/command.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/validate/core/formatters.py` & `aws-sam-cli-1.99.0/samcli/commands/validate/core/formatters.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/validate/core/options.py` & `aws-sam-cli-1.99.0/samcli/commands/validate/core/options.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/commands/validate/validate.py` & `aws-sam-cli-1.99.0/samcli/commands/validate/validate.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/hook_packages/terraform/copy_terraform_built_artifacts.py` & `aws-sam-cli-1.99.0/samcli/hook_packages/terraform/copy_terraform_built_artifacts.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/hook_packages/terraform/designs/resource_linking_generalized.md` & `aws-sam-cli-1.99.0/samcli/hook_packages/terraform/designs/resource_linking_generalized.md`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/constants.py` & `aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/constants.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/enrich.py` & `aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/enrich.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/exceptions.py` & `aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/exceptions.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/hook.py` & `aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/hook.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/makefile_generator.py` & `aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/makefile_generator.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/property_builder.py` & `aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/property_builder.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/resource_linking.py` & `aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/resource_linking.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/resources/apigw.py` & `aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/resources/apigw.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/resources/code_resource_utils.py` & `aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/resources/code_resource_utils.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/resources/internal.py` & `aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/resources/internal.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/resources/lambda_function.py` & `aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/resources/lambda_function.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/resources/lambda_layers.py` & `aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/resources/lambda_layers.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/resources/resource_links.py` & `aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/resources/resource_links.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/resources/resource_properties.py` & `aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/resources/resource_properties.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/translate.py` & `aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/translate.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/hook_packages/terraform/hooks/prepare/types.py` & `aws-sam-cli-1.99.0/samcli/hook_packages/terraform/hooks/prepare/types.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/hook_packages/terraform/lib/utils.py` & `aws-sam-cli-1.99.0/samcli/hook_packages/terraform/lib/utils.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/bootstrap/bootstrap.py` & `aws-sam-cli-1.99.0/samcli/lib/bootstrap/bootstrap.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/bootstrap/companion_stack/companion_stack_builder.py` & `aws-sam-cli-1.99.0/samcli/lib/bootstrap/companion_stack/companion_stack_builder.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/bootstrap/companion_stack/companion_stack_manager.py` & `aws-sam-cli-1.99.0/samcli/lib/bootstrap/companion_stack/companion_stack_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                 "credentials for the AWS SDK for Python client. "
                 "Please see their documentation for options to pass in credentials: "
                 "https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html"
             ) from ex
         except NoRegionError as ex:
             raise RegionError(
                 "Error Setting Up Managed Stack Client: Unable to resolve a region. "
-                "Please provide a region via the --region parameter or by the AWS_REGION environment variable."
+                "Please provide a region via the --region parameter or by the AWS_DEFAULT_REGION environment variable."
             ) from ex
 
     def set_functions(
         self, function_logical_ids: List[str], image_repositories: Optional[Dict[str, str]] = None
     ) -> None:
         """
         Sets functions that need to have ECR repos created
```

### Comparing `aws-sam-cli-1.98.0/samcli/lib/bootstrap/companion_stack/data_types.py` & `aws-sam-cli-1.99.0/samcli/lib/bootstrap/companion_stack/data_types.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/bootstrap/nested_stack/nested_stack_builder.py` & `aws-sam-cli-1.99.0/samcli/lib/bootstrap/nested_stack/nested_stack_builder.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/bootstrap/nested_stack/nested_stack_manager.py` & `aws-sam-cli-1.99.0/samcli/lib/bootstrap/nested_stack/nested_stack_manager.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/bootstrap/stack_builder.py` & `aws-sam-cli-1.99.0/samcli/lib/bootstrap/stack_builder.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/build/app_builder.py` & `aws-sam-cli-1.99.0/samcli/lib/build/app_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,17 +36,18 @@
 from samcli.lib.samlib.resource_metadata_normalizer import ResourceMetadataNormalizer
 from samcli.lib.docker.log_streamer import LogStreamer, LogStreamError
 from samcli.lib.providers.provider import ResourcesToBuildCollector, get_full_path, Stack
 from samcli.lib.utils.colors import Colored, Colors
 from samcli.lib.utils import osutils
 from samcli.lib.utils.packagetype import IMAGE, ZIP
 from samcli.lib.utils.stream_writer import StreamWriter
+from samcli.local.docker.exceptions import ContainerNotStartableException
 from samcli.local.docker.lambda_build_container import LambdaBuildContainer
 from samcli.local.docker.utils import is_docker_reachable, get_docker_platform
-from samcli.local.docker.manager import ContainerManager
+from samcli.local.docker.manager import ContainerManager, DockerImagePullFailedException
 from samcli.commands._utils.experimental import get_enabled_experimental_flags
 from samcli.lib.build.exceptions import (
     DockerConnectionError,
     DockerfileOutSideOfContext,
     DockerBuildFailed,
     BuildError,
     BuildInsideContainerError,
@@ -956,14 +957,18 @@
 
             # Request is successful. Now copy the artifacts back to the host
             LOG.debug("Build inside container was successful. Copying artifacts from container to host")
 
             # "/." is a Docker thing that instructions the copy command to download contents of the folder only
             result_dir_in_container = response["result"]["artifacts_dir"] + "/."
             container.copy(result_dir_in_container, artifacts_dir)
+
+        except DockerImagePullFailedException as ex:
+            raise BuildInsideContainerError(ex)
+
         finally:
             self._container_manager.stop(container)
 
         LOG.debug("Build inside container succeeded")
         return artifacts_dir
 
     @staticmethod
```

### Comparing `aws-sam-cli-1.98.0/samcli/lib/build/build_graph.py` & `aws-sam-cli-1.99.0/samcli/lib/build/build_graph.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/build/build_strategy.py` & `aws-sam-cli-1.99.0/samcli/lib/build/build_strategy.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/build/bundler.py` & `aws-sam-cli-1.99.0/samcli/lib/build/bundler.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/build/dependency_hash_generator.py` & `aws-sam-cli-1.99.0/samcli/lib/build/dependency_hash_generator.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/build/exceptions.py` & `aws-sam-cli-1.99.0/samcli/lib/build/exceptions.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/build/utils.py` & `aws-sam-cli-1.99.0/samcli/lib/build/utils.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/build/workflow_config.py` & `aws-sam-cli-1.99.0/samcli/lib/build/workflow_config.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/build/workflows.py` & `aws-sam-cli-1.99.0/samcli/lib/build/workflows.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/cli_validation/image_repository_validation.py` & `aws-sam-cli-1.99.0/samcli/lib/cli_validation/image_repository_validation.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/cli_validation/remote_invoke_options_validations.py` & `aws-sam-cli-1.99.0/samcli/lib/cli_validation/remote_invoke_options_validations.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/config/file_manager.py` & `aws-sam-cli-1.99.0/samcli/lib/config/file_manager.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/config/samconfig.py` & `aws-sam-cli-1.99.0/samcli/lib/config/samconfig.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/cookiecutter/exceptions.py` & `aws-sam-cli-1.99.0/samcli/lib/cookiecutter/exceptions.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/cookiecutter/interactive_flow.py` & `aws-sam-cli-1.99.0/samcli/lib/cookiecutter/interactive_flow.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/cookiecutter/interactive_flow_creator.py` & `aws-sam-cli-1.99.0/samcli/lib/cookiecutter/interactive_flow_creator.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/cookiecutter/plugin.py` & `aws-sam-cli-1.99.0/samcli/lib/cookiecutter/plugin.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/cookiecutter/processor.py` & `aws-sam-cli-1.99.0/samcli/lib/cookiecutter/processor.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/cookiecutter/question.py` & `aws-sam-cli-1.99.0/samcli/lib/cookiecutter/question.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/cookiecutter/template.py` & `aws-sam-cli-1.99.0/samcli/lib/cookiecutter/template.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/delete/cfn_utils.py` & `aws-sam-cli-1.99.0/samcli/lib/delete/cfn_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Delete Cloudformation stacks and s3 files
 """
 
+import json
 import logging
 from typing import List, Optional
 
 from botocore.exceptions import BotoCoreError, ClientError, WaiterError
 
 from samcli.commands.delete.exceptions import (
     CfDeleteFailedStatusError,
@@ -106,14 +107,19 @@
                 if change_set_name:
                     # the stack has a change set, use the template from this
                     resp = self._client.get_template(
                         StackName=stack_name, TemplateStage=stage, ChangeSetName=change_set_name
                     )
                     template = resp.get("TemplateBody", "")
 
+            # template variable can be of type string or of type dict which does not return
+            # nicely as a string, so it is dumped instead
+            if isinstance(template, dict):
+                return json.dumps(template)
+
             return str(template)
 
         except (ClientError, BotoCoreError) as e:
             # If there are credentials, environment errors,
             # catch that and throw a delete failed error.
 
             LOG.error("Failed to fetch template for the stack : %s", str(e))
```

### Comparing `aws-sam-cli-1.98.0/samcli/lib/deploy/deployer.py` & `aws-sam-cli-1.99.0/samcli/lib/deploy/deployer.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/deploy/utils.py` & `aws-sam-cli-1.99.0/samcli/lib/deploy/utils.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/docker/log_streamer.py` & `aws-sam-cli-1.99.0/samcli/lib/docker/log_streamer.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/docs/browser_configuration.py` & `aws-sam-cli-1.99.0/samcli/lib/docs/browser_configuration.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/docs/documentation.py` & `aws-sam-cli-1.99.0/samcli/lib/docs/documentation.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/docs/documentation_links.json` & `aws-sam-cli-1.99.0/samcli/lib/docs/documentation_links.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/event-mapping.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/event-mapping.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/alb/ALBRequest.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/alb/ALBRequest.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/alexa-skills-kit/AlexaEndSession.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/alexa-skills-kit/AlexaEndSession.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/alexa-skills-kit/AlexaIntentAnswer.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/alexa-skills-kit/AlexaIntentAnswer.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/alexa-skills-kit/AlexaIntentGetNewFact.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/alexa-skills-kit/AlexaIntentGetNewFact.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/alexa-skills-kit/AlexaIntentMyColorIs.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/alexa-skills-kit/AlexaIntentMyColorIs.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/alexa-skills-kit/AlexaIntentRecipe.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/alexa-skills-kit/AlexaIntentRecipe.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/alexa-skills-kit/AlexaStartSession.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/alexa-skills-kit/AlexaStartSession.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/apigateway/ApiGatewayRestRequestAuthorizer.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/apigateway/ApiGatewayRestRequestAuthorizer.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/apigateway/AwsProxy.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/apigateway/AwsProxy.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/apigateway/HttpApi.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/apigateway/HttpApi.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/appsync/AppSyncDirectResolver.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/appsync/AppSyncDirectResolver.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontABTest.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontABTest.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontAccessRequestInResponse.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontAccessRequestInResponse.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontHttpRedirect.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontHttpRedirect.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontModifyQueryString.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontModifyQueryString.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontModifyResponseHeader.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontModifyResponseHeader.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontMultipleRemoteCallsAggregateResponse.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontMultipleRemoteCallsAggregateResponse.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontNormalizeQuerystringToImproveCacheHit.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontNormalizeQuerystringToImproveCacheHit.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontRedirectOnViewerCountry.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontRedirectOnViewerCountry.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontServeObjectOnViewerDevice.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontServeObjectOnViewerDevice.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontSimpleRemoteCall.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/cloudfront/CloudFrontSimpleRemoteCall.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/codecommit/CodeCommit.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/codecommit/CodeCommit.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/codepipeline/CodePipeline.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/codepipeline/CodePipeline.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/config/ConfigurationItemChangeNotification.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/config/ConfigurationItemChangeNotification.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/config/OversizedConfigurationItemChangeNotification.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/config/OversizedConfigurationItemChangeNotification.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/config/PeriodicRule.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/config/PeriodicRule.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/connect/ConnectContactFlowEvent.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/connect/ConnectContactFlowEvent.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/dynamodb/DynamoDBUpdate.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/dynamodb/DynamoDBUpdate.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/kinesis/Kinesis.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/kinesis/Kinesis.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/kinesis/KinesisAnalyticsKpl.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/kinesis/KinesisAnalyticsKpl.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/kinesis/KinesisFirehoseCloudwatchLogsProcessor.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/kinesis/KinesisFirehoseCloudwatchLogsProcessor.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/kinesis/KinesisFirehoseStreamsAsSource.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/kinesis/KinesisFirehoseStreamsAsSource.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/lex-v2/BankingBot.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/lex-v2/BankingBot.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/lex-v2/LexBookCar.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/lex-v2/LexBookCar.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/lex-v2/LexBookHotel.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/lex-v2/LexBookHotel.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/rekognition/RekognitionS3Request.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/rekognition/RekognitionS3Request.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/s3/S3Delete.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/s3/S3Delete.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/s3/S3Put.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/s3/S3Put.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/ses/SesEmailReceiving.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/ses/SesEmailReceiving.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/sns/Sns.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/sns/Sns.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/sqs/Sqs.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/sqs/Sqs.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events/workmail/WorkMail.json` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events/workmail/WorkMail.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/generated_sample_events/events.py` & `aws-sam-cli-1.99.0/samcli/lib/generated_sample_events/events.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/hook/exceptions.py` & `aws-sam-cli-1.99.0/samcli/lib/hook/exceptions.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/hook/hook_config.py` & `aws-sam-cli-1.99.0/samcli/lib/hook/hook_config.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/hook/hook_config_schema.json` & `aws-sam-cli-1.99.0/samcli/lib/hook/hook_config_schema.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/hook/hook_wrapper.py` & `aws-sam-cli-1.99.0/samcli/lib/hook/hook_wrapper.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/hook/utils.py` & `aws-sam-cli-1.99.0/samcli/lib/hook/utils.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/iac/cdk/cdk_iac.py` & `aws-sam-cli-1.99.0/samcli/lib/iac/cdk/cdk_iac.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/iac/cdk/utils.py` & `aws-sam-cli-1.99.0/samcli/lib/iac/cdk/utils.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/iac/cfn/cfn_iac.py` & `aws-sam-cli-1.99.0/samcli/lib/iac/cfn/cfn_iac.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/iac/exceptions.py` & `aws-sam-cli-1.99.0/samcli/lib/iac/exceptions.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/iac/iac_factory.py` & `aws-sam-cli-1.99.0/samcli/lib/iac/iac_factory.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/iac/plugins_interfaces.py` & `aws-sam-cli-1.99.0/samcli/lib/iac/plugins_interfaces.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/__init__.py` & `aws-sam-cli-1.99.0/samcli/lib/init/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/arbitrary_project.py` & `aws-sam-cli-1.99.0/samcli/lib/init/arbitrary_project.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/default_samconfig.py` & `aws-sam-cli-1.99.0/samcli/lib/init/default_samconfig.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/exceptions.py` & `aws-sam-cli-1.99.0/samcli/lib/init/exceptions.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/local_manifest.json` & `aws-sam-cli-1.99.0/samcli/lib/init/local_manifest.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/template_modifiers/application_insights_template_modifier.py` & `aws-sam-cli-1.99.0/samcli/lib/init/template_modifiers/application_insights_template_modifier.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/template_modifiers/cli_template_modifier.py` & `aws-sam-cli-1.99.0/samcli/lib/init/template_modifiers/cli_template_modifier.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/template_modifiers/xray_tracing_template_modifier.py` & `aws-sam-cli-1.99.0/samcli/lib/init/template_modifiers/xray_tracing_template_modifier.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/.gitignore` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/.gitignore`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/LICENSE` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/README.md` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/README.md`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/tests/test_cookiecutter.py` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/tests/test_cookiecutter.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/.gitignore` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/.gitignore`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/README.md` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/README.md`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/events/event.json` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/events/event.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/src/HelloWorld/Function.cs` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/src/HelloWorld/Function.cs`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/src/HelloWorld/HelloWorld.csproj` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/src/HelloWorld/HelloWorld.csproj`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/src/HelloWorld/aws-lambda-tools-defaults.json` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/src/HelloWorld/aws-lambda-tools-defaults.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/template.yaml` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/template.yaml`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/test/HelloWorld.Test/FunctionTest.cs` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/test/HelloWorld.Test/FunctionTest.cs`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/test/HelloWorld.Test/HelloWorld.Tests.csproj` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-dotnet/{{cookiecutter.project_name}}/test/HelloWorld.Test/HelloWorld.Tests.csproj`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/README.md` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/README.md`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/tests/test_bake_project.py` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/tests/test_bake_project.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/{{cookiecutter.project_name}}/README.md` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/{{cookiecutter.project_name}}/README.md`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/{{cookiecutter.project_name}}/hello-world/main.go` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/{{cookiecutter.project_name}}/hello-world/main.go`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/{{cookiecutter.project_name}}/hello-world/main_test.go` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/{{cookiecutter.project_name}}/hello-world/main_test.go`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/{{cookiecutter.project_name}}/template.yaml` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-golang/{{cookiecutter.project_name}}/template.yaml`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/LICENSE` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/README.md` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/README.md`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/tests/test_cookiecutter.py` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/tests/test_cookiecutter.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/gradle/wrapper/gradle-wrapper.jar` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/gradle/wrapper/gradle-wrapper.jar`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/gradlew` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/gradlew`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/gradlew.bat` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/gradlew.bat`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/src/main/java/helloworld/App.java` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/src/main/java/helloworld/App.java`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/src/main/java/helloworld/GatewayResponse.java` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/src/main/java/helloworld/GatewayResponse.java`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/src/test/java/helloworld/AppTest.java` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/HelloWorldFunction/src/test/java/helloworld/AppTest.java`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/README.md` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/README.md`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/events/event.json` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/events/event.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/template.yaml` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-gradle/{{cookiecutter.project_name}}/template.yaml`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/LICENSE` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/README.md` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/README.md`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/tests/test_cookiecutter.py` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/tests/test_cookiecutter.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/HelloWorldFunction/pom.xml` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/HelloWorldFunction/pom.xml`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/HelloWorldFunction/src/main/java/helloworld/App.java` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/HelloWorldFunction/src/main/java/helloworld/App.java`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/HelloWorldFunction/src/main/java/helloworld/GatewayResponse.java` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/HelloWorldFunction/src/main/java/helloworld/GatewayResponse.java`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/HelloWorldFunction/src/test/java/helloworld/AppTest.java` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/HelloWorldFunction/src/test/java/helloworld/AppTest.java`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/README.md` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/README.md`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/events/event.json` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/events/event.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/template.yaml` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-java-maven/{{cookiecutter.project_name}}/template.yaml`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/.gitignore` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/.gitignore`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/LICENSE` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/README.md` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/README.md`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/.gitignore` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/.gitignore`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/README.md` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/README.md`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/events/event.json` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/events/event.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/hello-world/app.js` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/hello-world/app.js`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/hello-world/tests/unit/test-handler.js` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/hello-world/tests/unit/test-handler.js`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/template.yaml` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-nodejs/{{cookiecutter.project_name}}/template.yaml`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/.gitignore` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/.gitignore`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/LICENSE` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/README.md` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/README.md`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/.gitignore` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/.gitignore`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/README.md` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/README.md`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/events/event.json` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/events/event.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/hello_world/app.py` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/hello_world/app.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/template.yaml` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/template.yaml`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/tests/unit/test_handler.py` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-python/{{cookiecutter.project_name}}/tests/unit/test_handler.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/.gitignore` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/.gitignore`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/LICENSE` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/README.md` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/README.md`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/.gitignore` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/.gitignore`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/README.md` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/README.md`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/events/event.json` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/events/event.json`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/hello_world/app.rb` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/hello_world/app.rb`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/template.yaml` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/template.yaml`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/tests/unit/test_handler.rb` & `aws-sam-cli-1.99.0/samcli/lib/init/templates/cookiecutter-aws-sam-hello-ruby/{{cookiecutter.project_name}}/tests/unit/test_handler.rb`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/intrinsic_resolver/intrinsic_property_resolver.py` & `aws-sam-cli-1.99.0/samcli/lib/intrinsic_resolver/intrinsic_property_resolver.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/intrinsic_resolver/intrinsics_symbol_table.py` & `aws-sam-cli-1.99.0/samcli/lib/intrinsic_resolver/intrinsics_symbol_table.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/intrinsic_resolver/invalid_intrinsic_validation.py` & `aws-sam-cli-1.99.0/samcli/lib/intrinsic_resolver/invalid_intrinsic_validation.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/list/endpoints/endpoints_producer.py` & `aws-sam-cli-1.99.0/samcli/lib/list/endpoints/endpoints_producer.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/list/endpoints/endpoints_to_table_mapper.py` & `aws-sam-cli-1.99.0/samcli/lib/list/endpoints/endpoints_to_table_mapper.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/list/list_interfaces.py` & `aws-sam-cli-1.99.0/samcli/lib/list/list_interfaces.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/list/mapper_consumer_factory.py` & `aws-sam-cli-1.99.0/samcli/lib/list/mapper_consumer_factory.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/list/resources/resource_mapping_producer.py` & `aws-sam-cli-1.99.0/samcli/lib/list/resources/resource_mapping_producer.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/list/resources/resources_to_table_mapper.py` & `aws-sam-cli-1.99.0/samcli/lib/list/resources/resources_to_table_mapper.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/list/stack_outputs/stack_output_to_table_mapper.py` & `aws-sam-cli-1.99.0/samcli/lib/list/stack_outputs/stack_output_to_table_mapper.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/list/stack_outputs/stack_outputs_producer.py` & `aws-sam-cli-1.99.0/samcli/lib/list/stack_outputs/stack_outputs_producer.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/observability/cw_logs/cw_log_event.py` & `aws-sam-cli-1.99.0/samcli/lib/observability/cw_logs/cw_log_event.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/observability/cw_logs/cw_log_formatters.py` & `aws-sam-cli-1.99.0/samcli/lib/observability/cw_logs/cw_log_formatters.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/observability/cw_logs/cw_log_group_provider.py` & `aws-sam-cli-1.99.0/samcli/lib/observability/cw_logs/cw_log_group_provider.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/observability/cw_logs/cw_log_puller.py` & `aws-sam-cli-1.99.0/samcli/lib/observability/cw_logs/cw_log_puller.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/observability/observability_info_puller.py` & `aws-sam-cli-1.99.0/samcli/lib/observability/observability_info_puller.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/observability/xray_traces/xray_event_mappers.py` & `aws-sam-cli-1.99.0/samcli/lib/observability/xray_traces/xray_event_mappers.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/observability/xray_traces/xray_event_puller.py` & `aws-sam-cli-1.99.0/samcli/lib/observability/xray_traces/xray_event_puller.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/observability/xray_traces/xray_events.py` & `aws-sam-cli-1.99.0/samcli/lib/observability/xray_traces/xray_events.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/observability/xray_traces/xray_service_graph_event_puller.py` & `aws-sam-cli-1.99.0/samcli/lib/observability/xray_traces/xray_service_graph_event_puller.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/package/artifact_exporter.py` & `aws-sam-cli-1.99.0/samcli/lib/package/artifact_exporter.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/package/code_signer.py` & `aws-sam-cli-1.99.0/samcli/lib/package/code_signer.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/package/ecr_uploader.py` & `aws-sam-cli-1.99.0/samcli/lib/package/ecr_uploader.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/package/ecr_utils.py` & `aws-sam-cli-1.99.0/samcli/lib/package/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/package/image_utils.py` & `aws-sam-cli-1.99.0/samcli/lib/package/image_utils.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/package/local_files_utils.py` & `aws-sam-cli-1.99.0/samcli/lib/package/local_files_utils.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/package/packageable_resources.py` & `aws-sam-cli-1.99.0/samcli/lib/package/packageable_resources.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/package/permissions.py` & `aws-sam-cli-1.99.0/samcli/lib/package/permissions.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/package/s3_uploader.py` & `aws-sam-cli-1.99.0/samcli/lib/package/s3_uploader.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/package/stream_cursor_utils.py` & `aws-sam-cli-1.99.0/samcli/lib/package/stream_cursor_utils.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/package/uploaders.py` & `aws-sam-cli-1.99.0/samcli/lib/package/uploaders.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/package/utils.py` & `aws-sam-cli-1.99.0/samcli/lib/package/utils.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/pipeline/bootstrap/resource.py` & `aws-sam-cli-1.99.0/samcli/lib/pipeline/bootstrap/resource.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/pipeline/bootstrap/stage.py` & `aws-sam-cli-1.99.0/samcli/lib/pipeline/bootstrap/stage.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/pipeline/bootstrap/stage_resources.yaml` & `aws-sam-cli-1.99.0/samcli/lib/pipeline/bootstrap/stage_resources.yaml`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/providers/api_collector.py` & `aws-sam-cli-1.99.0/samcli/lib/providers/api_collector.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/providers/api_provider.py` & `aws-sam-cli-1.99.0/samcli/lib/providers/api_provider.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/providers/cfn_api_provider.py` & `aws-sam-cli-1.99.0/samcli/lib/providers/cfn_api_provider.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/providers/cfn_base_api_provider.py` & `aws-sam-cli-1.99.0/samcli/lib/providers/cfn_base_api_provider.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/providers/exceptions.py` & `aws-sam-cli-1.99.0/samcli/lib/providers/exceptions.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/providers/provider.py` & `aws-sam-cli-1.99.0/samcli/lib/providers/provider.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/providers/sam_api_provider.py` & `aws-sam-cli-1.99.0/samcli/lib/providers/sam_api_provider.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/providers/sam_base_provider.py` & `aws-sam-cli-1.99.0/samcli/lib/providers/sam_base_provider.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/providers/sam_function_provider.py` & `aws-sam-cli-1.99.0/samcli/lib/providers/sam_function_provider.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/providers/sam_layer_provider.py` & `aws-sam-cli-1.99.0/samcli/lib/providers/sam_layer_provider.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/providers/sam_stack_provider.py` & `aws-sam-cli-1.99.0/samcli/lib/providers/sam_stack_provider.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/remote_invoke/lambda_invoke_executors.py` & `aws-sam-cli-1.99.0/samcli/lib/remote_invoke/lambda_invoke_executors.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/remote_invoke/remote_invoke_executor_factory.py` & `aws-sam-cli-1.99.0/samcli/lib/remote_invoke/remote_invoke_executor_factory.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Remote Invoke factory to instantiate remote invoker for given resource
 """
 import logging
 from typing import Any, Callable, Dict, Optional
 
+from samcli.lib.remote_invoke.kinesis_invoke_executors import KinesisPutDataExecutor
 from samcli.lib.remote_invoke.lambda_invoke_executors import (
     DefaultConvertToJSON,
     LambdaInvokeExecutor,
     LambdaInvokeWithResponseStreamExecutor,
     LambdaResponseConverter,
     LambdaStreamResponseConverter,
     _is_function_invoke_mode_response_stream,
@@ -16,14 +17,15 @@
     RemoteInvokeConsumer,
     RemoteInvokeExecutor,
     RemoteInvokeLogOutput,
     RemoteInvokeOutputFormat,
     RemoteInvokeResponse,
     ResponseObjectToJsonStringMapper,
 )
+from samcli.lib.remote_invoke.sqs_invoke_executors import SqsSendMessageExecutor
 from samcli.lib.remote_invoke.stepfunctions_invoke_executors import (
     SfnDescribeExecutionResponseConverter,
     StepFunctionsStartExecutionExecutor,
 )
 from samcli.lib.utils.cloudformation import CloudFormationResourceSummary
 from samcli.lib.utils.resources import AWS_LAMBDA_FUNCTION
 
@@ -181,14 +183,90 @@
             boto_action_executor=StepFunctionsStartExecutionExecutor(
                 sfn_client, cfn_resource_summary.physical_resource_id, remote_invoke_output_format
             ),
             response_consumer=response_consumer,
             log_consumer=log_consumer,
         )
 
+    def _create_sqs_boto_executor(
+        self,
+        cfn_resource_summary: CloudFormationResourceSummary,
+        remote_invoke_output_format: RemoteInvokeOutputFormat,
+        response_consumer: RemoteInvokeConsumer[RemoteInvokeResponse],
+        log_consumer: RemoteInvokeConsumer[RemoteInvokeLogOutput],
+    ) -> RemoteInvokeExecutor:
+        """Creates a remote invoke executor for SQS resource type based on
+        the boto action being called.
+
+        Parameters
+        ----------
+        cfn_resource_summary: CloudFormationResourceSummary
+            Information about the SQS resource
+        remote_invoke_output_format: RemoteInvokeOutputFormat
+            Response output format that will be used for remote invoke execution
+        response_consumer: RemoteInvokeConsumer[RemoteInvokeResponse]
+            Consumer instance which can process RemoteInvokeResponse events
+        log_consumer: RemoteInvokeConsumer[RemoteInvokeLogOutput]
+            Consumer instance which can process RemoteInvokeLogOutput events
+
+        Returns
+        -------
+        RemoteInvokeExecutor
+            Returns the Executor created for SQS
+        """
+        LOG.info("Sending message to SQS queue %s", cfn_resource_summary.logical_resource_id)
+        sqs_client = self._boto_client_provider("sqs")
+        return RemoteInvokeExecutor(
+            request_mappers=[],
+            response_mappers=[ResponseObjectToJsonStringMapper()],
+            boto_action_executor=SqsSendMessageExecutor(
+                sqs_client, cfn_resource_summary.physical_resource_id, remote_invoke_output_format
+            ),
+            response_consumer=response_consumer,
+            log_consumer=log_consumer,
+        )
+
+    def _create_kinesis_boto_executor(
+        self,
+        cfn_resource_summary: CloudFormationResourceSummary,
+        remote_invoke_output_format: RemoteInvokeOutputFormat,
+        response_consumer: RemoteInvokeConsumer[RemoteInvokeResponse],
+        log_consumer: RemoteInvokeConsumer[RemoteInvokeLogOutput],
+    ) -> RemoteInvokeExecutor:
+        """Creates a remote invoke executor for Kinesis resource type based on
+        the boto action being called.
+
+        Parameters
+        ----------
+        cfn_resource_summary: CloudFormationResourceSummary
+            Information about the Kinesis stream resource
+        remote_invoke_output_format: RemoteInvokeOutputFormat
+            Response output format that will be used for remote invoke execution
+        response_consumer: RemoteInvokeConsumer[RemoteInvokeResponse]
+            Consumer instance which can process RemoteInvokeResponse events
+        log_consumer: RemoteInvokeConsumer[RemoteInvokeLogOutput]
+            Consumer instance which can process RemoteInvokeLogOutput events
+
+        Returns
+        -------
+        RemoteInvokeExecutor
+            Returns the Executor created for Kinesis stream
+        """
+        LOG.info("Putting record to Kinesis data stream %s", cfn_resource_summary.logical_resource_id)
+        kinesis_client = self._boto_client_provider("kinesis")
+        return RemoteInvokeExecutor(
+            request_mappers=[DefaultConvertToJSON()],
+            response_mappers=[ResponseObjectToJsonStringMapper()],
+            boto_action_executor=KinesisPutDataExecutor(
+                kinesis_client, cfn_resource_summary.physical_resource_id, remote_invoke_output_format
+            ),
+            response_consumer=response_consumer,
+            log_consumer=log_consumer,
+        )
+
     # mapping definition for each supported resource type
     REMOTE_INVOKE_EXECUTOR_MAPPING: Dict[
         str,
         Callable[
             [
                 "RemoteInvokeExecutorFactory",
                 CloudFormationResourceSummary,
```

### Comparing `aws-sam-cli-1.98.0/samcli/lib/remote_invoke/remote_invoke_executors.py` & `aws-sam-cli-1.99.0/samcli/lib/remote_invoke/remote_invoke_executors.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/remote_invoke/stepfunctions_invoke_executors.py` & `aws-sam-cli-1.99.0/samcli/lib/remote_invoke/stepfunctions_invoke_executors.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/samlib/local_uri_plugin.py` & `aws-sam-cli-1.99.0/samcli/lib/samlib/local_uri_plugin.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/samlib/resource_metadata_normalizer.py` & `aws-sam-cli-1.99.0/samcli/lib/samlib/resource_metadata_normalizer.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/samlib/wrapper.py` & `aws-sam-cli-1.99.0/samcli/lib/samlib/wrapper.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/schemas/cli_paginator.py` & `aws-sam-cli-1.99.0/samcli/lib/schemas/cli_paginator.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/schemas/schemas_api_caller.py` & `aws-sam-cli-1.99.0/samcli/lib/schemas/schemas_api_caller.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/schemas/schemas_aws_config.py` & `aws-sam-cli-1.99.0/samcli/lib/schemas/schemas_aws_config.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/schemas/schemas_cli_message_generator.py` & `aws-sam-cli-1.99.0/samcli/lib/schemas/schemas_cli_message_generator.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/schemas/schemas_code_manager.py` & `aws-sam-cli-1.99.0/samcli/lib/schemas/schemas_code_manager.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/schemas/schemas_directory_hierarchy_builder.py` & `aws-sam-cli-1.99.0/samcli/lib/schemas/schemas_directory_hierarchy_builder.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/shared_test_events/lambda_shared_test_event.py` & `aws-sam-cli-1.99.0/samcli/lib/shared_test_events/lambda_shared_test_event.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/sync/continuous_sync_flow_executor.py` & `aws-sam-cli-1.99.0/samcli/lib/sync/continuous_sync_flow_executor.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/sync/exceptions.py` & `aws-sam-cli-1.99.0/samcli/lib/sync/exceptions.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/sync/flows/alias_version_sync_flow.py` & `aws-sam-cli-1.99.0/samcli/lib/sync/flows/alias_version_sync_flow.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/sync/flows/auto_dependency_layer_sync_flow.py` & `aws-sam-cli-1.99.0/samcli/lib/sync/flows/auto_dependency_layer_sync_flow.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/sync/flows/function_sync_flow.py` & `aws-sam-cli-1.99.0/samcli/lib/sync/flows/function_sync_flow.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/sync/flows/generic_api_sync_flow.py` & `aws-sam-cli-1.99.0/samcli/lib/sync/flows/generic_api_sync_flow.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/sync/flows/http_api_sync_flow.py` & `aws-sam-cli-1.99.0/samcli/lib/sync/flows/http_api_sync_flow.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/sync/flows/image_function_sync_flow.py` & `aws-sam-cli-1.99.0/samcli/lib/sync/flows/image_function_sync_flow.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/sync/flows/layer_sync_flow.py` & `aws-sam-cli-1.99.0/samcli/lib/sync/flows/layer_sync_flow.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/sync/flows/rest_api_sync_flow.py` & `aws-sam-cli-1.99.0/samcli/lib/sync/flows/rest_api_sync_flow.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/sync/flows/stepfunctions_sync_flow.py` & `aws-sam-cli-1.99.0/samcli/lib/sync/flows/stepfunctions_sync_flow.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/sync/flows/zip_function_sync_flow.py` & `aws-sam-cli-1.99.0/samcli/lib/sync/flows/zip_function_sync_flow.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/sync/infra_sync_executor.py` & `aws-sam-cli-1.99.0/samcli/lib/sync/infra_sync_executor.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/sync/sync_flow.py` & `aws-sam-cli-1.99.0/samcli/lib/sync/sync_flow.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/sync/sync_flow_executor.py` & `aws-sam-cli-1.99.0/samcli/lib/sync/sync_flow_executor.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/sync/sync_flow_factory.py` & `aws-sam-cli-1.99.0/samcli/lib/sync/sync_flow_factory.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/sync/watch_manager.py` & `aws-sam-cli-1.99.0/samcli/lib/sync/watch_manager.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/telemetry/cicd.py` & `aws-sam-cli-1.99.0/samcli/lib/telemetry/cicd.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/telemetry/event.py` & `aws-sam-cli-1.99.0/samcli/lib/telemetry/event.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/telemetry/metric.py` & `aws-sam-cli-1.99.0/samcli/lib/telemetry/metric.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/telemetry/project_metadata.py` & `aws-sam-cli-1.99.0/samcli/lib/telemetry/project_metadata.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/telemetry/telemetry.py` & `aws-sam-cli-1.99.0/samcli/lib/telemetry/telemetry.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/telemetry/user_agent.py` & `aws-sam-cli-1.99.0/samcli/lib/telemetry/user_agent.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/translate/sam_template_validator.py` & `aws-sam-cli-1.99.0/samcli/lib/translate/sam_template_validator.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/utils/architecture.py` & `aws-sam-cli-1.99.0/samcli/lib/utils/architecture.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/utils/arn_utils.py` & `aws-sam-cli-1.99.0/samcli/lib/utils/arn_utils.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/utils/async_utils.py` & `aws-sam-cli-1.99.0/samcli/lib/utils/async_utils.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/utils/boto_utils.py` & `aws-sam-cli-1.99.0/samcli/lib/utils/boto_utils.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/utils/cloudformation.py` & `aws-sam-cli-1.99.0/samcli/lib/utils/cloudformation.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/utils/code_trigger_factory.py` & `aws-sam-cli-1.99.0/samcli/lib/utils/code_trigger_factory.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/utils/codeuri.py` & `aws-sam-cli-1.99.0/samcli/lib/utils/codeuri.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/utils/colors.py` & `aws-sam-cli-1.99.0/samcli/lib/utils/colors.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/utils/configuration.py` & `aws-sam-cli-1.99.0/samcli/lib/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/utils/definition_validator.py` & `aws-sam-cli-1.99.0/samcli/lib/utils/definition_validator.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/utils/file_observer.py` & `aws-sam-cli-1.99.0/samcli/lib/utils/file_observer.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/utils/git_repo.py` & `aws-sam-cli-1.99.0/samcli/lib/utils/git_repo.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/utils/graphql_api.py` & `aws-sam-cli-1.99.0/samcli/lib/utils/graphql_api.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/utils/hash.py` & `aws-sam-cli-1.99.0/samcli/lib/utils/hash.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/utils/lock_distributor.py` & `aws-sam-cli-1.99.0/samcli/lib/utils/lock_distributor.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/utils/managed_cloudformation_stack.py` & `aws-sam-cli-1.99.0/samcli/lib/utils/managed_cloudformation_stack.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             "Error Setting Up Managed Stack Client: Unable to resolve credentials for the AWS SDK for Python client. "
             "Please see their documentation for options to pass in credentials: "
             "https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html"
         ) from ex
     except NoRegionError as ex:
         raise RegionError(
             "Error Setting Up Managed Stack Client: Unable to resolve a region. "
-            "Please provide a region via the --region parameter or by the AWS_REGION environment variable."
+            "Please provide a region via the --region parameter or by the AWS_DEFAULT_REGION environment variable."
         ) from ex
     return _create_or_update_stack(cloudformation_client, stack_name, template_body, parameter_overrides)
 
 
 def manage_stack(
     region: Optional[str],
     stack_name: str,
@@ -136,15 +136,15 @@
             "Error Setting Up Managed Stack Client: Unable to resolve credentials for the AWS SDK for Python client. "
             "Please see their documentation for options to pass in credentials: "
             "https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html"
         ) from ex
     except NoRegionError as ex:
         raise RegionError(
             "Error Setting Up Managed Stack Client: Unable to resolve a region. "
-            "Please provide a region via the --region parameter or by the AWS_REGION environment variable."
+            "Please provide a region via the --region parameter or by the AWS_DEFAULT_REGION environment variable."
         ) from ex
     return _create_or_get_stack(cloudformation_client, stack_name, template_body, parameter_overrides)
 
 
 # Todo Add _update_stack to handle the case when the values of the stack parameter got changed
 def _create_or_get_stack(
     cloudformation_client,
```

### Comparing `aws-sam-cli-1.98.0/samcli/lib/utils/osutils.py` & `aws-sam-cli-1.99.0/samcli/lib/utils/osutils.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/utils/path_observer.py` & `aws-sam-cli-1.99.0/samcli/lib/utils/path_observer.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/utils/resource_trigger.py` & `aws-sam-cli-1.99.0/samcli/lib/utils/resource_trigger.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/utils/resource_type_based_factory.py` & `aws-sam-cli-1.99.0/samcli/lib/utils/resource_type_based_factory.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/utils/resources.py` & `aws-sam-cli-1.99.0/samcli/lib/utils/resources.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/utils/retry.py` & `aws-sam-cli-1.99.0/samcli/lib/utils/retry.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/utils/s3.py` & `aws-sam-cli-1.99.0/samcli/lib/utils/s3.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/utils/sam_logging.py` & `aws-sam-cli-1.99.0/samcli/lib/utils/sam_logging.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/utils/stream_writer.py` & `aws-sam-cli-1.99.0/samcli/lib/utils/stream_writer.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/utils/subprocess_utils.py` & `aws-sam-cli-1.99.0/samcli/lib/utils/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/utils/system_info.py` & `aws-sam-cli-1.99.0/samcli/lib/utils/system_info.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/utils/tar.py` & `aws-sam-cli-1.99.0/samcli/lib/utils/tar.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/utils/time.py` & `aws-sam-cli-1.99.0/samcli/lib/utils/time.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/utils/version_checker.py` & `aws-sam-cli-1.99.0/samcli/lib/utils/version_checker.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/lib/warnings/sam_cli_warning.py` & `aws-sam-cli-1.99.0/samcli/lib/warnings/sam_cli_warning.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/local/apigw/authorizers/lambda_authorizer.py` & `aws-sam-cli-1.99.0/samcli/local/apigw/authorizers/lambda_authorizer.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/local/apigw/event_constructor.py` & `aws-sam-cli-1.99.0/samcli/local/apigw/event_constructor.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/local/apigw/exceptions.py` & `aws-sam-cli-1.99.0/samcli/local/apigw/exceptions.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/local/apigw/local_apigw_service.py` & `aws-sam-cli-1.99.0/samcli/local/apigw/local_apigw_service.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/local/apigw/path_converter.py` & `aws-sam-cli-1.99.0/samcli/local/apigw/path_converter.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/local/apigw/route.py` & `aws-sam-cli-1.99.0/samcli/local/apigw/route.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/local/apigw/service_error_responses.py` & `aws-sam-cli-1.99.0/samcli/local/apigw/service_error_responses.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/local/common/runtime_template.py` & `aws-sam-cli-1.99.0/samcli/local/common/runtime_template.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/local/docker/container.py` & `aws-sam-cli-1.99.0/samcli/local/docker/container.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/local/docker/effective_user.py` & `aws-sam-cli-1.99.0/samcli/local/docker/effective_user.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/local/docker/lambda_build_container.py` & `aws-sam-cli-1.99.0/samcli/local/docker/lambda_build_container.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/local/docker/lambda_container.py` & `aws-sam-cli-1.99.0/samcli/local/docker/lambda_container.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/local/docker/lambda_debug_settings.py` & `aws-sam-cli-1.99.0/samcli/local/docker/lambda_debug_settings.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/local/docker/lambda_image.py` & `aws-sam-cli-1.99.0/samcli/local/docker/lambda_image.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/local/docker/manager.py` & `aws-sam-cli-1.99.0/samcli/local/docker/manager.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/local/docker/utils.py` & `aws-sam-cli-1.99.0/samcli/local/docker/utils.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/local/events/api_event.py` & `aws-sam-cli-1.99.0/samcli/local/events/api_event.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/local/lambda_service/lambda_error_responses.py` & `aws-sam-cli-1.99.0/samcli/local/lambda_service/lambda_error_responses.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/local/lambda_service/local_lambda_invoke_service.py` & `aws-sam-cli-1.99.0/samcli/local/lambda_service/local_lambda_invoke_service.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/local/lambdafn/config.py` & `aws-sam-cli-1.99.0/samcli/local/lambdafn/config.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/local/lambdafn/env_vars.py` & `aws-sam-cli-1.99.0/samcli/local/lambdafn/env_vars.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/local/lambdafn/remote_files.py` & `aws-sam-cli-1.99.0/samcli/local/lambdafn/remote_files.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/local/lambdafn/runtime.py` & `aws-sam-cli-1.99.0/samcli/local/lambdafn/runtime.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/local/lambdafn/zip.py` & `aws-sam-cli-1.99.0/samcli/local/lambdafn/zip.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/local/layers/layer_downloader.py` & `aws-sam-cli-1.99.0/samcli/local/layers/layer_downloader.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/local/rapid/aws-lambda-rie-arm64` & `aws-sam-cli-1.99.0/samcli/local/rapid/aws-lambda-rie-arm64`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/local/rapid/aws-lambda-rie-x86_64` & `aws-sam-cli-1.99.0/samcli/local/rapid/aws-lambda-rie-x86_64`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/local/services/base_local_service.py` & `aws-sam-cli-1.99.0/samcli/local/services/base_local_service.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/settings/__init__.py` & `aws-sam-cli-1.99.0/samcli/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/vendor/serverlessrepo/application_metadata.py` & `aws-sam-cli-1.99.0/samcli/vendor/serverlessrepo/application_metadata.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/vendor/serverlessrepo/exceptions.py` & `aws-sam-cli-1.99.0/samcli/vendor/serverlessrepo/exceptions.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/vendor/serverlessrepo/parser.py` & `aws-sam-cli-1.99.0/samcli/vendor/serverlessrepo/parser.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/vendor/serverlessrepo/publish.py` & `aws-sam-cli-1.99.0/samcli/vendor/serverlessrepo/publish.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/samcli/yamlhelper.py` & `aws-sam-cli-1.99.0/samcli/yamlhelper.py`

 * *Files identical despite different names*

### Comparing `aws-sam-cli-1.98.0/setup.py` & `aws-sam-cli-1.99.0/setup.py`

 * *Files identical despite different names*

