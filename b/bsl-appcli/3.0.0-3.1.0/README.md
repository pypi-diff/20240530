# Comparing `tmp/bsl_appcli-3.0.0.tar.gz` & `tmp/bsl_appcli-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bsl_appcli-3.0.0.tar", last modified: Wed Apr 24 22:39:04 2024, max compression
+gzip compressed data, was "bsl_appcli-3.1.0.tar", last modified: Thu May 30 05:02:49 2024, max compression
```

## Comparing `bsl_appcli-3.0.0.tar` & `bsl_appcli-3.1.0.tar`

### file list

```diff
@@ -1,100 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.974914 bsl_appcli-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    38553 2024-04-24 22:39:04.974914 bsl_appcli-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    37519 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.966914 bsl_appcli-3.0.0/appcli/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.966914 bsl_appcli-3.0.0/appcli/backup_manager/
--rw-r--r--   0 runner    (1001) docker     (127)    22873 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/backup_manager/backup_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/backup_manager/remote_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)    18065 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/cli_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.966914 bsl_appcli-3.0.0/appcli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/commands/appcli_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/commands/backup_manager_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    10479 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/commands/configure_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8018 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/commands/configure_template_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/commands/debug_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/commands/encrypt_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/commands/init_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/commands/install_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/commands/launcher_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/commands/migrate_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    10272 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/commands/service_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/commands/task_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/commands/version_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.966914 bsl_appcli-3.0.0/appcli/common/
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/common/data_class_extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.966914 bsl_appcli-3.0.0/appcli/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)    13880 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/configuration/configuration_dir_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    29934 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/configuration_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.970914 bsl_appcli-3.0.0/appcli/crypto/
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/crypto/cipher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/crypto/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/dev_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.970914 bsl_appcli-3.0.0/appcli/git_repositories/
--rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/git_repositories/git_repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)    11246 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/keycloak_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.970914 bsl_appcli-3.0.0/appcli/models/
--rw-r--r--   0 runner    (1001) docker     (127)     7131 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/models/cli_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     9440 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/models/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    31161 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/orchestrators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/string_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.970914 bsl_appcli-3.0.0/appcli/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/templates/installer.j2
--rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/templates/launcher.j2
--rw-r--r--   0 runner    (1001) docker     (127)    10966 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/appcli/variables_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.974914 bsl_appcli-3.0.0/bsl_appcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    38553 2024-04-24 22:39:04.000000 bsl_appcli-3.0.0/bsl_appcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-24 22:39:04.000000 bsl_appcli-3.0.0/bsl_appcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 22:39:04.000000 bsl_appcli-3.0.0/bsl_appcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-24 22:39:04.000000 bsl_appcli-3.0.0/bsl_appcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 22:39:04.000000 bsl_appcli-3.0.0/bsl_appcli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 22:39:04.974914 bsl_appcli-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.962914 bsl_appcli-3.0.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.970914 bsl_appcli-3.0.0/tests/backup_manager/
--rw-r--r--   0 runner    (1001) docker     (127)    36565 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/tests/backup_manager/test_backup_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.970914 bsl_appcli-3.0.0/tests/cipher/
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/tests/cipher/test_cipher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.970914 bsl_appcli-3.0.0/tests/commands/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.962914 bsl_appcli-3.0.0/tests/commands/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.962914 bsl_appcli-3.0.0/tests/commands/resources/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.962914 bsl_appcli-3.0.0/tests/commands/resources/templates/baseline/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.970914 bsl_appcli-3.0.0/tests/commands/resources/templates/baseline/nesting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/tests/commands/resources/templates/baseline/nesting/nested_baseline_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    17602 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/tests/commands/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/tests/commands/test_install_script.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.970914 bsl_appcli-3.0.0/tests/commands_task/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.962914 bsl_appcli-3.0.0/tests/commands_task/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.962914 bsl_appcli-3.0.0/tests/commands_task/resources/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.962914 bsl_appcli-3.0.0/tests/commands_task/resources/templates/baseline/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.970914 bsl_appcli-3.0.0/tests/commands_task/resources/templates/baseline/nesting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/tests/commands_task/resources/templates/baseline/nesting/nested_baseline_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/tests/commands_task/test_commands_task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.970914 bsl_appcli-3.0.0/tests/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/tests/configuration/test_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.970914 bsl_appcli-3.0.0/tests/configuration_manager/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.962914 bsl_appcli-3.0.0/tests/configuration_manager/expected_generated/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.970914 bsl_appcli-3.0.0/tests/configuration_manager/expected_generated/nesting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/tests/configuration_manager/expected_generated/nesting/nested_baseline_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.962914 bsl_appcli-3.0.0/tests/configuration_manager/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.962914 bsl_appcli-3.0.0/tests/configuration_manager/resources/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.962914 bsl_appcli-3.0.0/tests/configuration_manager/resources/templates/baseline/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.970914 bsl_appcli-3.0.0/tests/configuration_manager/resources/templates/baseline/nesting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/tests/configuration_manager/resources/templates/baseline/nesting/nested_baseline_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    12006 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/tests/configuration_manager/test_configuration_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.970914 bsl_appcli-3.0.0/tests/configuration_state/
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/tests/configuration_state/test_configuration_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.970914 bsl_appcli-3.0.0/tests/crypto/
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/tests/crypto/test_crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.974914 bsl_appcli-3.0.0/tests/git_repositories/
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/tests/git_repositories/test_git_repositories.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.974914 bsl_appcli-3.0.0/tests/string_transformer/
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/tests/string_transformer/test_string_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.974914 bsl_appcli-3.0.0/tests/variables_manager/
--rw-r--r--   0 runner    (1001) docker     (127)    10415 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/tests/variables_manager/test_variables_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:39:04.974914 bsl_appcli-3.0.0/tests/version/
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-24 22:38:24.000000 bsl_appcli-3.0.0/tests/version/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.693319 bsl_appcli-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    42615 2024-05-30 05:02:49.693319 bsl_appcli-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    41560 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.685319 bsl_appcli-3.1.0/appcli/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.685319 bsl_appcli-3.1.0/appcli/backup_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)    22873 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/appcli/backup_manager/backup_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/appcli/backup_manager/remote_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19863 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/appcli/cli_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.689319 bsl_appcli-3.1.0/appcli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/appcli/commands/appcli_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/appcli/commands/backup_manager_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10479 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/appcli/commands/configure_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8018 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/appcli/commands/configure_template_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/appcli/commands/debug_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/appcli/commands/encrypt_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/appcli/commands/init_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/appcli/commands/install_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/appcli/commands/launcher_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/appcli/commands/migrate_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10272 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/appcli/commands/service_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/appcli/commands/task_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/appcli/commands/version_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.689319 bsl_appcli-3.1.0/appcli/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/appcli/common/data_class_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.689319 bsl_appcli-3.1.0/appcli/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)    13880 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/appcli/configuration/configuration_dir_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29934 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/appcli/configuration_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.689319 bsl_appcli-3.1.0/appcli/crypto/
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/appcli/crypto/cipher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/appcli/crypto/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/appcli/dev_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/appcli/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.689319 bsl_appcli-3.1.0/appcli/git_repositories/
+-rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/appcli/git_repositories/git_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11246 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/appcli/keycloak_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/appcli/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.689319 bsl_appcli-3.1.0/appcli/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     7932 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/appcli/models/cli_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9440 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/appcli/models/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41232 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/appcli/orchestrators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/appcli/string_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.689319 bsl_appcli-3.1.0/appcli/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/appcli/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/appcli/templates/installer.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/appcli/templates/launcher.j2
+-rw-r--r--   0 runner    (1001) docker     (127)    10966 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/appcli/variables_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.693319 bsl_appcli-3.1.0/bsl_appcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    42615 2024-05-30 05:02:49.000000 bsl_appcli-3.1.0/bsl_appcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-05-30 05:02:49.000000 bsl_appcli-3.1.0/bsl_appcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 05:02:49.000000 bsl_appcli-3.1.0/bsl_appcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-30 05:02:49.000000 bsl_appcli-3.1.0/bsl_appcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 05:02:49.000000 bsl_appcli-3.1.0/bsl_appcli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 05:02:49.693319 bsl_appcli-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.681319 bsl_appcli-3.1.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.689319 bsl_appcli-3.1.0/tests/backup_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)    36565 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/tests/backup_manager/test_backup_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.689319 bsl_appcli-3.1.0/tests/cipher/
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/tests/cipher/test_cipher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.689319 bsl_appcli-3.1.0/tests/commands/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.681319 bsl_appcli-3.1.0/tests/commands/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.681319 bsl_appcli-3.1.0/tests/commands/resources/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.681319 bsl_appcli-3.1.0/tests/commands/resources/templates/baseline/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.689319 bsl_appcli-3.1.0/tests/commands/resources/templates/baseline/nesting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/tests/commands/resources/templates/baseline/nesting/nested_baseline_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17602 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/tests/commands/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/tests/commands/test_install_script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.689319 bsl_appcli-3.1.0/tests/commands_task/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.681319 bsl_appcli-3.1.0/tests/commands_task/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.681319 bsl_appcli-3.1.0/tests/commands_task/resources/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.681319 bsl_appcli-3.1.0/tests/commands_task/resources/templates/baseline/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.689319 bsl_appcli-3.1.0/tests/commands_task/resources/templates/baseline/nesting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/tests/commands_task/resources/templates/baseline/nesting/nested_baseline_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/tests/commands_task/test_commands_task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.689319 bsl_appcli-3.1.0/tests/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/tests/configuration/test_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.689319 bsl_appcli-3.1.0/tests/configuration_manager/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.681319 bsl_appcli-3.1.0/tests/configuration_manager/expected_generated/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.689319 bsl_appcli-3.1.0/tests/configuration_manager/expected_generated/nesting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/tests/configuration_manager/expected_generated/nesting/nested_baseline_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.681319 bsl_appcli-3.1.0/tests/configuration_manager/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.681319 bsl_appcli-3.1.0/tests/configuration_manager/resources/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.681319 bsl_appcli-3.1.0/tests/configuration_manager/resources/templates/baseline/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.693319 bsl_appcli-3.1.0/tests/configuration_manager/resources/templates/baseline/nesting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/tests/configuration_manager/resources/templates/baseline/nesting/nested_baseline_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12006 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/tests/configuration_manager/test_configuration_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.693319 bsl_appcli-3.1.0/tests/configuration_state/
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/tests/configuration_state/test_configuration_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.693319 bsl_appcli-3.1.0/tests/crypto/
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/tests/crypto/test_crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.693319 bsl_appcli-3.1.0/tests/git_repositories/
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/tests/git_repositories/test_git_repositories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.693319 bsl_appcli-3.1.0/tests/orchestrators/
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/tests/orchestrators/test_helm_orchestrator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.693319 bsl_appcli-3.1.0/tests/string_transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/tests/string_transformer/test_string_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.693319 bsl_appcli-3.1.0/tests/variables_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)    10415 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/tests/variables_manager/test_variables_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:02:49.693319 bsl_appcli-3.1.0/tests/version/
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-30 05:02:11.000000 bsl_appcli-3.1.0/tests/version/test_version.py
```

### Comparing `bsl_appcli-3.0.0/LICENSE` & `bsl_appcli-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/PKG-INFO` & `bsl_appcli-3.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: bsl-appcli
-Version: 3.0.0
+Version: 3.1.0
 Summary: A library for adding CLI interfaces to applications in the brightSPARK Labs style
 Home-page: https://www.brightsparklabs.com
 Author: brightSPARK Labs
 Author-email: enquire@brightsparklabs.com
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: boto3==1.34.91
+Requires-Dist: boto3==1.34.95
 Requires-Dist: click==8.1.7
 Requires-Dist: coloredlogs==15.0.1
 Requires-Dist: cronex==0.1.3.1
 Requires-Dist: dataclasses-json==0.5.7
 Requires-Dist: deepdiff==6.7.1
 Requires-Dist: GitPython==3.1.43
-Requires-Dist: jsonschema==4.21.1
-Requires-Dist: jinja2==3.1.3
+Requires-Dist: jsonschema==4.22.0
+Requires-Dist: jinja2==3.1.4
 Requires-Dist: pycryptodome==3.20.0
 Requires-Dist: pydantic==2.7.1
 Requires-Dist: pyfiglet==1.0.2
 Requires-Dist: python-keycloak==3.12.0
 Requires-Dist: python-slugify==8.0.4
 Requires-Dist: ruamel-yaml==0.18.6
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: wheel==0.43.0
 Provides-Extra: dev
-Requires-Dist: ruff; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
+Requires-Dist: ruff==0.3.7; extra == "dev"
+Requires-Dist: pre-commit==3.7.0; extra == "dev"
+Requires-Dist: pytest==8.1.1; extra == "dev"
 
 # BSL Application CLI Library
 
 [![PyPI version](https://badge.fury.io/py/bsl-appcli.svg)](https://badge.fury.io/py/bsl-appcli)
 ![Test Python](https://github.com/brightsparklabs/appcli/actions/workflows/build_python.yml/badge.svg)
 
 A library for adding CLI interfaces to applications in the brightSPARK Labs style.
@@ -72,14 +72,26 @@
 
 The `docker-compose.yml` can be templated by renaming to `docker-compose.yml.j2`, and setting
 variables within the `settings.yml` file as described in the Installation section.
 
 Stack variables can be set within the `stack-settings.yml` file as described in the
 `Build configuration template directories` section.
 
+### Volume Mounts
+
+The following directories are mounted from the host system into the container:
+
+```bash
+--volume "/opt/brightsparklabs/<my_app>/<environment>/data/cli/home:/root"
+--volume "/opt/brightsparklabs/<my_app>/<environment>/conf:/opt/brightsparklabs/<my_app>/<environment>/conf"
+--volume "/opt/brightsparklabs/<my_app>/<environment>/conf/.generated:/opt/brightsparklabs/<my_app>/<environment>/conf/.generated"
+--volume "/opt/brightsparklabs/<my_app>/<environment>/data:/opt/brightsparklabs/<my_app>/<environment>/data"
+--volume "/opt/brightsparklabs/<my_app>/<environment>/backup:/opt/brightsparklabs/<my_app>/<environment>/backup"
+```
+
 ## Quick Start
 
 Refer to the [quick start guide](quickstart.md) to get a basic application running.
 
 Otherwise refer to the Installation section below to see all options.
 
 ## Installation
@@ -167,14 +179,116 @@
 for appcli applications which consist only of the launcher container containing various additional CLI 
 command groups. The `NullOrchestrator` disables commands related to managing services.
 
 ```python
 orchestrator=NullOrchestrator()
 ```
 
+#### HelmOrchestrator
+
+The project also includes a [helm](https://helm.sh/docs/intro/quickstart/) orchestrator for deploying charts to [kubernetes](https://kubernetes.io/) clusters.
+
+Create a new `resources` directory as follows:
+
+```bash
+resources/
+├── settings.yml
+└── templates/
+   ├── baseline/
+   │  └── cli/
+   │     └── helm/
+   │        ├── set-files/
+   │        │  ├── baz/
+   │        │  │  ├── foo.json
+   │        │  │  └── qux.waldo.txt
+   │        │  └── thud.bang.yml
+   │        ├── set-values/
+   │        │  ├── foo.yml
+   │        │  └── bar.txt
+   │        └── mychart.tgz
+   └── configurable/
+      └── cli/
+         └── home/
+            └── .kube/
+               └── config  # Overwrite this with a cluster specific config file. ie `~/.kube/config`.
+```
+
+You can then define the orchestrator:
+
+```python
+from appcli.orchestrators import HelmOrchestrator
+orchestrator = HelmOrchestrator(
+    # Chart archive path (relative to `conf/templates/`).
+    # [Optional] Default is `cli/helm/chart`
+    chart_location="cli/helm/mychart.tgz",
+
+    # The directory containing all main `values.yaml` files (relative to `conf/templates/`).
+    # [Optional] Default is `cli/helm/set-values`
+    helm_set_values_dir="cli/helm/set-values"
+
+    # The directory containing all key-specific files (relative to `conf/templates/`).
+    # [Optional] Default is `cli/helm/set-files`
+    helm_set_files_dir="cli/helm/set-files"
+)
+```
+
+##### Values
+
+Values can be supplied either:
+
+1. For a set key by placing files in `set-files` directory.
+    * The name of the key to set is derived from the directory structure and the name of the file
+      (up to the first dot encountered in the filename).
+2. Globally for any files dumped in the `set-values` directory.
+
+For example, given the following `cli/helm/` directory structure:
+
+```bash
+cli/helm/
+├── set-files/
+│  ├── baz/
+│  │  ├── foo.json
+│  │  └── qux.waldo.txt
+│  └── thud.bang.yml
+└── set-values/
+   ├── foo.yml
+   └── bar.txt
+```
+
+This would result in the following arguments being passed to helm:
+
+```bash
+--set-file baz.foo=cli/helm/set-files/baz/foo.json
+--set-file baz.qux=cli/helm/set-files/baz/qux.waldo.yml    # NOTE: Key is `qux` not `qux.waldo`.
+--set-file thud=cli/helm/set-files/thud.bang.yml           # NOTE: Key is `thud` not `thud.bang`.
+--values cli/helm/set-values/foo.yml
+--values cli/helm/set-values/bar.yml
+```
+
+##### Dev Mode Chart
+
+During development it would be slow to require packaging up the chart for any changes.
+Appcli provides a way to speed up development by allow for the chart to deployed directly from source.
+This is done by specifying the dev chart as an environment variable.
+
+```bash
+MYAPP_DEV_MODE=true MYAPP_DEV_MODE_HELM_CHART=/path/to/mychart python3 -m myapp service start
+```
+
+##### Kubeconfig
+
+A custom `kubeconfig` file can be used by specifying the `KUBECONFIG` environment variable.
+
+```bash
+KUBECONFIG=/opt/brightsparklabs/myapp/conf/.generated/config ./myapp ...
+```
+
+_NOTE:_ The `KUBECONFIG` file must be at a location which is mounted into the launch container.
+Refer to [Volume Mounts](#volume-mounts) for details on what volumes are mounted into the launch container.
+
 #### Custom Commands
 
 You can specify some custom top-level commands by adding click commands or command groups to the
 configuration object.  Assuming 'web' is the name of the service in the docker-compose.yml file
 which you wish to exec against, we can create three custom commands in the following example:
 
 - `myapp ls-root` which lists the contents of the root directory within the `web` service container
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bsl_appcli-3.0.0/README.md` & `bsl_appcli-3.1.0/bsl_appcli.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: bsl-appcli
+Version: 3.1.0
+Summary: A library for adding CLI interfaces to applications in the brightSPARK Labs style
+Home-page: https://www.brightsparklabs.com
+Author: brightSPARK Labs
+Author-email: enquire@brightsparklabs.com
+License: MIT License
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: boto3==1.34.95
+Requires-Dist: click==8.1.7
+Requires-Dist: coloredlogs==15.0.1
+Requires-Dist: cronex==0.1.3.1
+Requires-Dist: dataclasses-json==0.5.7
+Requires-Dist: deepdiff==6.7.1
+Requires-Dist: GitPython==3.1.43
+Requires-Dist: jsonschema==4.22.0
+Requires-Dist: jinja2==3.1.4
+Requires-Dist: pycryptodome==3.20.0
+Requires-Dist: pydantic==2.7.1
+Requires-Dist: pyfiglet==1.0.2
+Requires-Dist: python-keycloak==3.12.0
+Requires-Dist: python-slugify==8.0.4
+Requires-Dist: ruamel-yaml==0.18.6
+Requires-Dist: tabulate==0.9.0
+Requires-Dist: wheel==0.43.0
+Provides-Extra: dev
+Requires-Dist: ruff==0.3.7; extra == "dev"
+Requires-Dist: pre-commit==3.7.0; extra == "dev"
+Requires-Dist: pytest==8.1.1; extra == "dev"
+
 # BSL Application CLI Library
 
 [![PyPI version](https://badge.fury.io/py/bsl-appcli.svg)](https://badge.fury.io/py/bsl-appcli)
 ![Test Python](https://github.com/brightsparklabs/appcli/actions/workflows/build_python.yml/badge.svg)
 
 A library for adding CLI interfaces to applications in the brightSPARK Labs style.
 
@@ -40,14 +72,26 @@
 
 The `docker-compose.yml` can be templated by renaming to `docker-compose.yml.j2`, and setting
 variables within the `settings.yml` file as described in the Installation section.
 
 Stack variables can be set within the `stack-settings.yml` file as described in the
 `Build configuration template directories` section.
 
+### Volume Mounts
+
+The following directories are mounted from the host system into the container:
+
+```bash
+--volume "/opt/brightsparklabs/<my_app>/<environment>/data/cli/home:/root"
+--volume "/opt/brightsparklabs/<my_app>/<environment>/conf:/opt/brightsparklabs/<my_app>/<environment>/conf"
+--volume "/opt/brightsparklabs/<my_app>/<environment>/conf/.generated:/opt/brightsparklabs/<my_app>/<environment>/conf/.generated"
+--volume "/opt/brightsparklabs/<my_app>/<environment>/data:/opt/brightsparklabs/<my_app>/<environment>/data"
+--volume "/opt/brightsparklabs/<my_app>/<environment>/backup:/opt/brightsparklabs/<my_app>/<environment>/backup"
+```
+
 ## Quick Start
 
 Refer to the [quick start guide](quickstart.md) to get a basic application running.
 
 Otherwise refer to the Installation section below to see all options.
 
 ## Installation
@@ -135,14 +179,116 @@
 for appcli applications which consist only of the launcher container containing various additional CLI 
 command groups. The `NullOrchestrator` disables commands related to managing services.
 
 ```python
 orchestrator=NullOrchestrator()
 ```
 
+#### HelmOrchestrator
+
+The project also includes a [helm](https://helm.sh/docs/intro/quickstart/) orchestrator for deploying charts to [kubernetes](https://kubernetes.io/) clusters.
+
+Create a new `resources` directory as follows:
+
+```bash
+resources/
+├── settings.yml
+└── templates/
+   ├── baseline/
+   │  └── cli/
+   │     └── helm/
+   │        ├── set-files/
+   │        │  ├── baz/
+   │        │  │  ├── foo.json
+   │        │  │  └── qux.waldo.txt
+   │        │  └── thud.bang.yml
+   │        ├── set-values/
+   │        │  ├── foo.yml
+   │        │  └── bar.txt
+   │        └── mychart.tgz
+   └── configurable/
+      └── cli/
+         └── home/
+            └── .kube/
+               └── config  # Overwrite this with a cluster specific config file. ie `~/.kube/config`.
+```
+
+You can then define the orchestrator:
+
+```python
+from appcli.orchestrators import HelmOrchestrator
+orchestrator = HelmOrchestrator(
+    # Chart archive path (relative to `conf/templates/`).
+    # [Optional] Default is `cli/helm/chart`
+    chart_location="cli/helm/mychart.tgz",
+
+    # The directory containing all main `values.yaml` files (relative to `conf/templates/`).
+    # [Optional] Default is `cli/helm/set-values`
+    helm_set_values_dir="cli/helm/set-values"
+
+    # The directory containing all key-specific files (relative to `conf/templates/`).
+    # [Optional] Default is `cli/helm/set-files`
+    helm_set_files_dir="cli/helm/set-files"
+)
+```
+
+##### Values
+
+Values can be supplied either:
+
+1. For a set key by placing files in `set-files` directory.
+    * The name of the key to set is derived from the directory structure and the name of the file
+      (up to the first dot encountered in the filename).
+2. Globally for any files dumped in the `set-values` directory.
+
+For example, given the following `cli/helm/` directory structure:
+
+```bash
+cli/helm/
+├── set-files/
+│  ├── baz/
+│  │  ├── foo.json
+│  │  └── qux.waldo.txt
+│  └── thud.bang.yml
+└── set-values/
+   ├── foo.yml
+   └── bar.txt
+```
+
+This would result in the following arguments being passed to helm:
+
+```bash
+--set-file baz.foo=cli/helm/set-files/baz/foo.json
+--set-file baz.qux=cli/helm/set-files/baz/qux.waldo.yml    # NOTE: Key is `qux` not `qux.waldo`.
+--set-file thud=cli/helm/set-files/thud.bang.yml           # NOTE: Key is `thud` not `thud.bang`.
+--values cli/helm/set-values/foo.yml
+--values cli/helm/set-values/bar.yml
+```
+
+##### Dev Mode Chart
+
+During development it would be slow to require packaging up the chart for any changes.
+Appcli provides a way to speed up development by allow for the chart to deployed directly from source.
+This is done by specifying the dev chart as an environment variable.
+
+```bash
+MYAPP_DEV_MODE=true MYAPP_DEV_MODE_HELM_CHART=/path/to/mychart python3 -m myapp service start
+```
+
+##### Kubeconfig
+
+A custom `kubeconfig` file can be used by specifying the `KUBECONFIG` environment variable.
+
+```bash
+KUBECONFIG=/opt/brightsparklabs/myapp/conf/.generated/config ./myapp ...
+```
+
+_NOTE:_ The `KUBECONFIG` file must be at a location which is mounted into the launch container.
+Refer to [Volume Mounts](#volume-mounts) for details on what volumes are mounted into the launch container.
+
 #### Custom Commands
 
 You can specify some custom top-level commands by adding click commands or command groups to the
 configuration object.  Assuming 'web' is the name of the service in the docker-compose.yml file
 which you wish to exec against, we can create three custom commands in the following example:
 
 - `myapp ls-root` which lists the contents of the root directory within the `web` service container
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bsl_appcli-3.0.0/appcli/backup_manager/backup_manager.py` & `bsl_appcli-3.1.0/appcli/backup_manager/backup_manager.py`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/appcli/backup_manager/remote_strategy.py` & `bsl_appcli-3.1.0/appcli/backup_manager/remote_strategy.py`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/appcli/cli_builder.py` & `bsl_appcli-3.1.0/appcli/cli_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 # standard libraries
 import getpass
 import os
 import sys
 from pathlib import Path
 from typing import Dict, Iterable
+import shutil
 
 # vendor libraries
 import click
 import pyfiglet
 from tabulate import tabulate
 
 # local libraries
@@ -46,14 +47,20 @@
 
 BASE_DIR = Path(__file__).parent
 """ The directory containing this script. """
 
 IS_PLATFORM_WINDOWS = sys.platform == "win32"
 """ True if the system running this Python code is Windows. """
 
+CONTAINER_HOME_DIR = Path("/root")
+""" Home directory of the container user. """
+
+HOME_CONFIG_DIR = Path("cli/home")
+""" Config directory containing home files to copoy to the container. """
+
 # ------------------------------------------------------------------------------
 # PUBLIC METHODS
 # ------------------------------------------------------------------------------
 
 
 def create_cli(configuration: Configuration, desired_environment: Dict[str, str] = {}):
     """Build the CLI to be run
@@ -88,14 +95,15 @@
     # Mandatory environment variables this script will set.
     ENV_VAR_CONFIG_DIR = f"{APP_NAME_SLUG_UPPER}_CONFIG_DIR"
     ENV_VAR_GENERATED_CONFIG_DIR = f"{APP_NAME_SLUG_UPPER}_GENERATED_CONFIG_DIR"
     ENV_VAR_DATA_DIR = f"{APP_NAME_SLUG_UPPER}_DATA_DIR"
     ENV_VAR_BACKUP_DIR = f"{APP_NAME_SLUG_UPPER}_BACKUP_DIR"
     ENV_VAR_ENVIRONMENT = f"{APP_NAME_SLUG_UPPER}_ENVIRONMENT"
 
+    DEV_MODE_VARIABLES = {}
     if IS_DEV_MODE:
         with wrap_dev_mode():
             environment = "local-dev"
             install_dir = Path("/tmp/") / APP_NAME_SLUG.lower() / environment
             install_dir.mkdir(parents=True, exist_ok=True)
 
             overrides = {
@@ -107,14 +115,24 @@
             }
 
             logger.info("Overriding CLI options via environment variables")
             for key, value in overrides.items():
                 logger.info(f"  {key}={value}")
                 os.environ[key] = str(value)
 
+            # Any environment variable beginning with `{APP_NAME}_DEV_MODE_*`
+            # is loaded up as a `DEV_MODE` variable.
+            logger.info("Detecting and setting `DEV_MODE` variables.")
+            for key, value in os.environ.items():
+                if key.startswith(f"{APP_NAME_SLUG_UPPER}_DEV_MODE_"):
+                    logger.info(
+                        f"Found the `[{key}]` dev variable. Setting to `{value}`."
+                    )
+                    DEV_MODE_VARIABLES[key] = value
+
     # --------------------------------------------------------------------------
     # CREATE_CLI: LOGIC
     # --------------------------------------------------------------------------
 
     default_commands = {}
     for cli_class in (
         ConfigureCli,
@@ -229,14 +247,15 @@
             subcommand_args=ctx.obj,
             debug=debug,
             is_dev_mode=IS_DEV_MODE,
             app_name_slug=APP_NAME_SLUG,
             app_version=APP_VERSION,
             commands=default_commands,
             backup_dir=backup_dir,
+            dev_mode_variables=DEV_MODE_VARIABLES,
         )
         ctx.obj = cli_context
 
         if ctx.invoked_subcommand is None:
             click.echo(ctx.get_help())
             sys.exit(1)
 
@@ -251,14 +270,18 @@
         # to work. Explicitly check for it, unless using an orchestrator which
         # does not need it.
         if not isinstance(configuration.orchestrator, NullOrchestrator):
             __check_docker_socket()
 
         __check_environment()
 
+        __copy_config_to_home_dir(
+            cli_context.get_generated_configuration_dir() / HOME_CONFIG_DIR
+        )
+
         # Table of configuration variables to print
         table = [
             ["Application", f"{APP_NAME} (slug: {APP_NAME_SLUG})"],
             ["Version", APP_VERSION],
             ["Environment", f"{cli_context.environment}"],
             ["Configuration directory", f"{cli_context.configuration_dir}"],
             [
@@ -386,14 +409,33 @@
             and additional_data_dir_env_vars_set
         ):
             error_and_exit(
                 "Some mandatory environment variables weren't set. See error messages above."
             )
         logger.info("All required environment variables are set.")
 
+    def __copy_config_to_home_dir(config_src_dir: Path) -> None:
+        """Copies the .generated `cli/home` directory into `/root` in the container.
+
+        The program might generate data in the `/root` directory which we do not want to lose on restart.
+        We therefore have to merge user provided files from `cli/home` into the container.
+
+        Args:
+            config_src_dir (Path): The location of the user provided home dir.
+        """
+        # Do not copy the users data if we are in dev mode as we are probably not in a container.
+        if IS_DEV_MODE:
+            return
+
+        if config_src_dir.exists() and config_src_dir.is_dir():
+            logger.info(
+                f"Copying `{config_src_dir}` to `{CONTAINER_HOME_DIR}` container directory."
+            )
+            shutil.copytree(config_src_dir, CONTAINER_HOME_DIR, dirs_exist_ok=True)
+
     def check_environment_variable_defined(
         env_variables: Iterable[str], error_message_template: str, exit_message: str
     ) -> bool:
         """Check if environment variables are defined
 
         Args:
             env_variables (Iterable[str]): the environment variables to check
```

### Comparing `bsl_appcli-3.0.0/appcli/commands/appcli_command.py` & `bsl_appcli-3.1.0/appcli/commands/appcli_command.py`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/appcli/commands/backup_manager_cli.py` & `bsl_appcli-3.1.0/appcli/commands/backup_manager_cli.py`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/appcli/commands/configure_cli.py` & `bsl_appcli-3.1.0/appcli/commands/configure_cli.py`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/appcli/commands/configure_template_cli.py` & `bsl_appcli-3.1.0/appcli/commands/configure_template_cli.py`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/appcli/commands/debug_cli.py` & `bsl_appcli-3.1.0/appcli/commands/debug_cli.py`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/appcli/commands/encrypt_cli.py` & `bsl_appcli-3.1.0/appcli/commands/encrypt_cli.py`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/appcli/commands/init_cli.py` & `bsl_appcli-3.1.0/appcli/commands/init_cli.py`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/appcli/commands/install_cli.py` & `bsl_appcli-3.1.0/appcli/commands/install_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
         @click.command(
             hidden=True, help="Outputs an appropriate installer bash script to stdout."
         )
         @click.option(
             "--install-dir",
             "-i",
-            help="Directory to install into. Defaults to '{default_install_dir}/<ENVIRONMENT>'.",
+            help=f"Directory to install into. Defaults to '{default_install_dir}/<ENVIRONMENT>'.",
             type=Path,
             default=default_install_dir,
         )
         @click.pass_context
         # NOTE: Hide the CLI command as end users should not run it manually
         def install(ctx, install_dir: Path):
             cli_context: CliContext = ctx.obj
```

### Comparing `bsl_appcli-3.0.0/appcli/commands/launcher_cli.py` & `bsl_appcli-3.1.0/appcli/commands/launcher_cli.py`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/appcli/commands/migrate_cli.py` & `bsl_appcli-3.1.0/appcli/commands/migrate_cli.py`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/appcli/commands/service_cli.py` & `bsl_appcli-3.1.0/appcli/commands/service_cli.py`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/appcli/commands/task_cli.py` & `bsl_appcli-3.1.0/appcli/commands/task_cli.py`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/appcli/commands/version_cli.py` & `bsl_appcli-3.1.0/appcli/commands/version_cli.py`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/appcli/common/data_class_extensions.py` & `bsl_appcli-3.1.0/appcli/common/data_class_extensions.py`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/appcli/configuration/configuration_dir_state.py` & `bsl_appcli-3.1.0/appcli/configuration/configuration_dir_state.py`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/appcli/configuration_manager.py` & `bsl_appcli-3.1.0/appcli/configuration_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from appcli.crypto.crypto import decrypt_values_in_file
 from appcli.functions import error_and_exit, print_header
 from appcli.git_repositories.git_repositories import (
     ConfigurationGitRepository,
     GeneratedConfigurationGitRepository,
 )
 from appcli.logger import logger
-from appcli.models.cli_context import SCHEMA_SUFFIX, IGNORE_INFIX, CliContext
+from appcli.models.cli_context import IGNORE_INFIX, SCHEMA_SUFFIX, CliContext
 from appcli.models.configuration import Configuration
 from appcli.variables_manager import VariablesManager
 
 # ------------------------------------------------------------------------------
 # CONSTANTS
 # ------------------------------------------------------------------------------
```

### Comparing `bsl_appcli-3.0.0/appcli/crypto/cipher.py` & `bsl_appcli-3.1.0/appcli/crypto/cipher.py`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/appcli/crypto/crypto.py` & `bsl_appcli-3.1.0/appcli/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/appcli/dev_mode.py` & `bsl_appcli-3.1.0/appcli/dev_mode.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 # ------------------------------------------------------------------------------
 
 import sys
 from contextlib import contextmanager
 
 import pyfiglet
 
+from appcli.logger import configure_default_logging, enable_dev_mode_logging
+
 # ------------------------------------------------------------------------------
 # CONSTANTS
 # ------------------------------------------------------------------------------
 
 __BANNER = pyfiglet.figlet_format("DEV MODE", font="tinker-toy")
 
 # ------------------------------------------------------------------------------
@@ -24,32 +26,34 @@
     Creates a context which prints DEV MODE markings around all output shown on terminal.
 
     EXAMPLE:
 
       The below code:
 
         if dev_mode_enabled:
-          with wrap_dev_mode:
+          with wrap_dev_mode():
             ...
-            logger.info("DEV MODE operation successfuly")
+            logger.info("DEV MODE operation completed successfully")
 
       Would result in everything printed by code in the `with` block being bookended by DEV MODE
       markings.
     """
 
     print(
         f"""
 {"<" * 70} DEV MODE BEGIN
 
 {__BANNER}
 """,
         file=sys.stderr,
     )
 
+    enable_dev_mode_logging()
     yield
+    configure_default_logging()
 
     print(
         f"""
 {">" * 70} DEV MODE END
 """,
         file=sys.stderr,
     )
```

### Comparing `bsl_appcli-3.0.0/appcli/functions.py` & `bsl_appcli-3.1.0/appcli/functions.py`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/appcli/git_repositories/git_repositories.py` & `bsl_appcli-3.1.0/appcli/git_repositories/git_repositories.py`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/appcli/keycloak_manager.py` & `bsl_appcli-3.1.0/appcli/keycloak_manager.py`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/appcli/logger.py` & `bsl_appcli-3.1.0/appcli/logger.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,18 +27,32 @@
 
 # ------------------------------------------------------------------------------
 # LOGGING
 # ------------------------------------------------------------------------------
 
 logger = logging.getLogger(__name__)
 logger.propagate = False
-coloredlogs.install(logger=logger, fmt=LOGGER_FORMAT, datefmt=LOGGER_DATE_FORMAT)
+
+
+def configure_default_logging():
+    coloredlogs.install(logger=logger, fmt=LOGGER_FORMAT, datefmt=LOGGER_DATE_FORMAT)
 
 
 def enable_debug_logging():
     coloredlogs.install(
         logger=logger,
         fmt=LOGGER_FORMAT,
         level=logging.DEBUG,
         datefmt=LOGGER_DATE_FORMAT,
     )
     logger.debug("Enabled debug mode")
+
+
+def enable_dev_mode_logging():
+    logger_format = "DEV_MODE | %(asctime)s %(levelname)s: %(message)s"
+    coloredlogs.install(
+        logger=logger,
+        fmt=logger_format,
+    )
+
+
+configure_default_logging()
```

### Comparing `bsl_appcli-3.0.0/appcli/models/cli_context.py` & `bsl_appcli-3.1.0/appcli/models/cli_context.py`

 * *Files 12% similar despite different names*

```diff
@@ -87,14 +87,26 @@
     app_version: str
     """ The application's version """
 
     commands: Dict
     """ Internal commands. """
 
     # ---------------------------------
+    # DEV_MODE specific fields.
+    # ---------------------------------
+
+    dev_mode_variables: Dict[str, str] = {}
+    """ A Dict of `DEV_MODE` env variables the user has supplied to the appliction.
+    These are set with:
+        MYAPP_DEV_MODE_FOO=BAR python -m myapp ...
+    Which would result in:
+        dev_mode_variables = {"MYAPP_DEV_MODE_FOO": "BAR"}
+    """
+
+    # ---------------------------------
     # derived data
     # ---------------------------------
 
     def get_configuration_dir_state(self) -> ConfigurationDirState:
         """Gets the state of the configuration, for use in validating whether
         a command can be used or not.
 
@@ -192,22 +204,30 @@
         but that need to be applied separately.
 
         Returns:
             Path: directory of configurable templates
         """
         return self.configuration_dir.joinpath("templates")
 
-    def get_project_name(self) -> str:
+    def get_project_name(self, make_helm_safe: bool = False) -> str:
         """Get a unique name for the application and environment
 
+        Arg:
+            make_helm_safe (bool): Convert the project name to one that is safe for helm.
+                Helm uses `[a-z0-9]([-a-z0-9]*[a-z0-9])?` for validation.
+                See https://github.com/helm/helm/issues/6192
+
         Returns:
             str: the project name
         """
         # NOTE: Must be lowercase, see https://github.com/brightsparklabs/appcli/issues/301
-        return f"{self.app_name_slug}_{self.environment}".lower()
+        project_name = f"{self.app_name_slug}_{self.environment}".lower()
+        if make_helm_safe:
+            project_name = project_name.replace("_", "-")
+        return project_name
 
     def get_variables_manager(self) -> VariablesManager:
         """Get the Variables Manager for the current cli context.
 
         Returns:
             VariablesManager: the variables manager for the current cli context.
         """
```

### Comparing `bsl_appcli-3.0.0/appcli/models/configuration.py` & `bsl_appcli-3.1.0/appcli/models/configuration.py`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/appcli/orchestrators.py` & `bsl_appcli-3.1.0/appcli/orchestrators.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import click
 
 # local libraries
 from appcli.commands.appcli_command import AppcliCommand
 from appcli.crypto import crypto
 from appcli.logger import logger
 from appcli.models.cli_context import CliContext
+from appcli.dev_mode import wrap_dev_mode
 
 # ------------------------------------------------------------------------------
 # CLASSES
 # ------------------------------------------------------------------------------
 
 
 class Orchestrator:
@@ -594,14 +595,294 @@
         )
 
     def __exec_command(self, command: Iterable[str]) -> CompletedProcess:
         logger.debug("Running [%s]", " ".join(command))
         return subprocess.run(command, capture_output=False)
 
 
+class HelmOrchestrator(Orchestrator):
+    """
+    Uses helm to provision a kubernetes backed helm chart.
+    """
+
+    DEV_CHART_VARIABLE_NAME = "DEV_MODE_HELM_CHART"
+    " Name suffix for the DEV_MODE chart location variable. "
+
+    def __init__(
+        self,
+        chart_location: Path = Path("cli/helm/chart"),
+        helm_set_values_dir: Path = Path("cli/helm/set-values"),
+        helm_set_files_dir: Path = Path("cli/helm/set-files"),
+    ):
+        """
+        Creates a new instance of an orchestrator for helm-based applications.
+
+        NOTE: All `Path` objects are relative to the configuration directory.
+
+        Args:
+            chart_location (Path): Path to the helm chart file/directory to deploy.
+            helm_set_values_dir (Path): The directory containing all main `values.yaml` files.
+                Defaults to: `${GENERATED_CONFIGURATION_DIR}/cli/helm/set-values`
+
+                All files in this directory are applied with:
+                    --values <file>
+
+                See below for more details.
+
+            helm_set_files_dir (Path): The directory containing all key-specific files.
+                Defaults to: `${GENERATED_CONFIGURATION_DIR}/cli/helm/set-files`
+
+                Take the following directory:
+
+                ```
+                ./
+                ├── set-files/
+                │  ├── baz/
+                │  │  ├── foo.json
+                │  │  └── qux.waldo.txt
+                │  └── thud.bang.yml
+                └── set-values/
+                   ├── foo.yml
+                   └── bar.txt
+                ```
+
+                This would result in the following arguments being passed to helm:
+
+                ```
+                --set-file baz.foo=cli/helm/set-files/baz/foo.json
+                --set-file baz.qux=cli/helm/set-files/baz/qux.waldo.yml    # NOTE: Key is `qux` not `qux.waldo`.
+                --set-file thud=cli/helm/set-files/thud.bang.yml           # NOTE: Key is `thud` not `thud.bang`.
+                --values cli/helm/set-values/foo.yml
+                --values cli/helm/set-values/bar.yml
+                ```
+        """
+        self.chart_location = chart_location
+        self.helm_set_values_dir = helm_set_values_dir
+        self.helm_set_files_dir = helm_set_files_dir
+
+    def start(
+        self, cli_context: CliContext, service_name: tuple[str, ...] = None
+    ) -> CompletedProcess:
+        """
+        Installs (or upgrades) a helm chart inside the current kubernetes cluster.
+
+        Args:
+            cli_context (CliContext): The current CLI context.
+
+        Returns:
+            CompletedProcess: Result of the orchestrator command.
+        """
+        # Generate the command string.
+        command = [
+            "helm",
+            "upgrade",
+            "--install",
+            "--namespace",
+            cli_context.get_project_name(make_helm_safe=True),
+            "--create-namespace",
+        ]
+        # Set values args.
+        for arg in self.__generate_values_args(
+            cli_context.get_generated_configuration_dir()
+        ):
+            command.append(arg)
+        # Set release name.
+        command.append(cli_context.get_project_name(make_helm_safe=True))
+        # Set chart location.
+        # If we're in `DEV_MODE` and `<APP-NAME>_DEV_MODE_HELM_CHART` is set, use that.
+        if (
+            cli_context.is_dev_mode
+            and f"{cli_context.app_name_slug.upper()}_{HelmOrchestrator.DEV_CHART_VARIABLE_NAME}"
+            in cli_context.dev_mode_variables.keys()
+        ):
+            with wrap_dev_mode():
+                chart_location = cli_context.dev_mode_variables[
+                    f"{cli_context.app_name_slug.upper()}_{HelmOrchestrator.DEV_CHART_VARIABLE_NAME}"
+                ]
+                logger.debug(
+                    f"Found DEV_MODE chart. Ignoring bundled chart from `{self.chart_location}`"
+                )
+                logger.debug(f"Deploying chart from `{chart_location}`")
+        # If not, then generate the absolute path to the `chart_location`.
+        else:
+            chart_location = (
+                cli_context.get_generated_configuration_dir() / self.chart_location
+            )
+        command.append(chart_location)
+
+        # Run the command.
+        return self.__run_command(command)
+
+    def shutdown(
+        self, cli_context: CliContext, service_name: tuple[str, ...] = None
+    ) -> CompletedProcess:
+        """
+        Uninstalls a helm chart from current kubernetes cluster.
+
+        Args:
+            cli_context (CliContext): The current CLI context.
+
+        Returns:
+            CompletedProcess: Result of the orchestrator command.
+        """
+        # Generate the command string.
+        command = [
+            "helm",
+            "uninstall",
+            cli_context.get_project_name(make_helm_safe=True),
+            "-n",
+            cli_context.get_project_name(make_helm_safe=True),
+        ]
+
+        # Run the command.
+        return self.__run_command(command)
+
+    def status(
+        self, cli_context: CliContext, service_name: tuple[str, ...] = None
+    ) -> CompletedProcess:
+        """
+        Get the status of the chart (through `helm status`).
+
+        Args:
+            cli_context (CliContext): The current CLI context.
+
+        Returns:
+            CompletedProcess: Result of the orchestrator command.
+        """
+        # Generate the command string.
+        command = [
+            "helm",
+            "status",
+            cli_context.get_project_name(make_helm_safe=True),
+            "-n",
+            cli_context.get_project_name(make_helm_safe=True),
+        ]
+
+        # Run the command.
+        return self.__run_command(command)
+
+    def task(
+        self,
+        cli_context: CliContext,
+        service_name: str,
+        extra_args: Iterable[str],
+        detached: bool = False,
+    ) -> CompletedProcess:
+        logger.info("HelmOrchestrator has no services to run tasks for.")
+        return None
+
+    def exec(
+        self,
+        cli_context: CliContext,
+        service_name: str,
+        command: Iterable[str],
+        stdin_input: str = None,
+        capture_output: bool = False,
+    ) -> CompletedProcess:
+        logger.info("HelmOrchestrator does not support executing arbitrary commands.")
+        return None
+
+    def get_logs_command(self) -> click.Command:
+        @click.command()
+        def log():
+            logger.info("HelmOrchestrator does not support getting logs.")
+            return None
+
+        return log
+
+    def get_additional_commands(self):
+        # TODO: AF-248: Add `kubectl`, `helm` and possibly `k9s` as commands that can be called.
+        return []
+
+    def get_name(self) -> str:
+        return "helm"
+
+    def verify_service_names(
+        self, cli_context: CliContext, service_names: tuple[str, ...]
+    ) -> bool:
+        if service_names is None or len(service_names) == 0:
+            return True
+        logger.info("HelmOrchestrator has no services.")
+        return False
+
+    def get_disabled_commands(self) -> list[str]:
+        # The `init` command is disabled because it's used to initialise additional services, and this orchestrator
+        # The `task` command is disabled because helm is only used for install/upgrade/uninstall/downgrade operations.
+        # has no services. NOTE: The `init` command will be removed in the future.
+        return ["init", "task"]
+
+    def __run_command(self, command: list[str]) -> CompletedProcess:
+        """Run the given command and return the CompletedProcess.
+
+        Args:
+            command (list[str]): The command to execute.
+
+        Returns:
+            CompletedProcess: The execution result.
+        """
+        logger.debug(f"Executing {str(command)}")
+        result = subprocess.run(command, capture_output=False)
+        if result.returncode != 0:
+            message = f"Unknown error from running: {str(command)}."
+            logger.error(message)
+            raise subprocess.CalledProcessError(
+                result.returncode,
+                command,
+                result.stdout,
+                result.stderr,
+            )
+        return result
+
+    def __generate_values_args(self, generated_configuration_dir: Path) -> list[str]:
+        """Recursively takes all the values files in the directories and generates an args array to
+        pass to helm through either `--values` or `--set-file` (depending on the location).
+        e.g:
+
+            ["--values", "values.yaml", "--set-file", "path.to.foo=path/to/foo.yaml"...
+
+        Args:
+            generated_configuration_dir (Path): Generated configuration directory form the cli object, e.g:
+                `cli_context.get_generated_configuration_dir()`
+
+        Returns:
+            list[str]: The arg list.
+        """
+        arg_list = []
+
+        # Create all `--values` args.
+        values_dir = generated_configuration_dir / self.helm_set_values_dir
+        values = [
+            file
+            for file in list(values_dir.rglob("*"))
+            if file.suffix in [".yml", ".yaml"]
+        ]
+        for file in values:
+            arg_list.append("--values")
+            arg_list.append(str(file))
+
+        # Create all `--set-file` args.
+        values_files_dir = generated_configuration_dir / self.helm_set_files_dir
+        values_files = [
+            file for file in list(values_files_dir.rglob("*")) if file.is_file()
+        ]
+        for file in values_files:
+            # NOTE: Make path relative to `helm_values_files_dir` so we know which helm key to set it as.
+            relative_file = file.relative_to(
+                generated_configuration_dir / self.helm_set_files_dir
+            )
+            # Get the helm key in `dot.notation.to.value`
+            key = ".".join(
+                [*relative_file.parent.parts, relative_file.stem.split(".")[0]]
+            )
+            arg_list.append("--set-file")
+            arg_list.append(f"{key}={file}")
+
+        return arg_list
+
+
 class NullOrchestrator(Orchestrator):
     """
     Orchestrator which has no services to orchestrate. This is useful for appcli applications which
     consist only of the launcher container containing various additional CLI command groups.
     """
 
     def start(
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bsl_appcli-3.0.0/appcli/string_transformer.py` & `bsl_appcli-3.1.0/appcli/string_transformer.py`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/appcli/templates/installer.j2` & `bsl_appcli-3.1.0/appcli/templates/installer.j2`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/appcli/templates/launcher.j2` & `bsl_appcli-3.1.0/appcli/templates/launcher.j2`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 {
 
     docker run \
         --name {{ app_name_slug }}_{{ cli_context.environment }}_launcher_$(date +%s) \
         --rm \
         $( [[ "${NO_INTERACTIVE}" != "true" ]] && echo "--interactive") \
         $( [[ "${NO_TTY}" != "true" ]] && echo "--tty") \
+        $( [[ -n "${KUBECONFIG}" ]] && echo "--env KUBECONFIG=${KUBECONFIG}") \
 {% if cli_context.docker_credentials_file %}
         --volume "{{ cli_context.docker_credentials_file }}:/root/.docker/config.json" \
 {% endif %}
 {% for name, value in cli_context.additional_env_variables %}
         --env {{ name }}="{{ value }}" \
 {% endfor %}
 {% for name, path in cli_context.additional_data_dirs %}
```

### Comparing `bsl_appcli-3.0.0/appcli/variables_manager.py` & `bsl_appcli-3.1.0/appcli/variables_manager.py`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/bsl_appcli.egg-info/PKG-INFO` & `bsl_appcli-3.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: bsl-appcli
-Version: 3.0.0
-Summary: A library for adding CLI interfaces to applications in the brightSPARK Labs style
-Home-page: https://www.brightsparklabs.com
-Author: brightSPARK Labs
-Author-email: enquire@brightsparklabs.com
-License: MIT License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: boto3==1.34.91
-Requires-Dist: click==8.1.7
-Requires-Dist: coloredlogs==15.0.1
-Requires-Dist: cronex==0.1.3.1
-Requires-Dist: dataclasses-json==0.5.7
-Requires-Dist: deepdiff==6.7.1
-Requires-Dist: GitPython==3.1.43
-Requires-Dist: jsonschema==4.21.1
-Requires-Dist: jinja2==3.1.3
-Requires-Dist: pycryptodome==3.20.0
-Requires-Dist: pydantic==2.7.1
-Requires-Dist: pyfiglet==1.0.2
-Requires-Dist: python-keycloak==3.12.0
-Requires-Dist: python-slugify==8.0.4
-Requires-Dist: ruamel-yaml==0.18.6
-Requires-Dist: tabulate==0.9.0
-Requires-Dist: wheel==0.43.0
-Provides-Extra: dev
-Requires-Dist: ruff; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
-
 # BSL Application CLI Library
 
 [![PyPI version](https://badge.fury.io/py/bsl-appcli.svg)](https://badge.fury.io/py/bsl-appcli)
 ![Test Python](https://github.com/brightsparklabs/appcli/actions/workflows/build_python.yml/badge.svg)
 
 A library for adding CLI interfaces to applications in the brightSPARK Labs style.
 
@@ -72,14 +40,26 @@
 
 The `docker-compose.yml` can be templated by renaming to `docker-compose.yml.j2`, and setting
 variables within the `settings.yml` file as described in the Installation section.
 
 Stack variables can be set within the `stack-settings.yml` file as described in the
 `Build configuration template directories` section.
 
+### Volume Mounts
+
+The following directories are mounted from the host system into the container:
+
+```bash
+--volume "/opt/brightsparklabs/<my_app>/<environment>/data/cli/home:/root"
+--volume "/opt/brightsparklabs/<my_app>/<environment>/conf:/opt/brightsparklabs/<my_app>/<environment>/conf"
+--volume "/opt/brightsparklabs/<my_app>/<environment>/conf/.generated:/opt/brightsparklabs/<my_app>/<environment>/conf/.generated"
+--volume "/opt/brightsparklabs/<my_app>/<environment>/data:/opt/brightsparklabs/<my_app>/<environment>/data"
+--volume "/opt/brightsparklabs/<my_app>/<environment>/backup:/opt/brightsparklabs/<my_app>/<environment>/backup"
+```
+
 ## Quick Start
 
 Refer to the [quick start guide](quickstart.md) to get a basic application running.
 
 Otherwise refer to the Installation section below to see all options.
 
 ## Installation
@@ -167,14 +147,116 @@
 for appcli applications which consist only of the launcher container containing various additional CLI 
 command groups. The `NullOrchestrator` disables commands related to managing services.
 
 ```python
 orchestrator=NullOrchestrator()
 ```
 
+#### HelmOrchestrator
+
+The project also includes a [helm](https://helm.sh/docs/intro/quickstart/) orchestrator for deploying charts to [kubernetes](https://kubernetes.io/) clusters.
+
+Create a new `resources` directory as follows:
+
+```bash
+resources/
+├── settings.yml
+└── templates/
+   ├── baseline/
+   │  └── cli/
+   │     └── helm/
+   │        ├── set-files/
+   │        │  ├── baz/
+   │        │  │  ├── foo.json
+   │        │  │  └── qux.waldo.txt
+   │        │  └── thud.bang.yml
+   │        ├── set-values/
+   │        │  ├── foo.yml
+   │        │  └── bar.txt
+   │        └── mychart.tgz
+   └── configurable/
+      └── cli/
+         └── home/
+            └── .kube/
+               └── config  # Overwrite this with a cluster specific config file. ie `~/.kube/config`.
+```
+
+You can then define the orchestrator:
+
+```python
+from appcli.orchestrators import HelmOrchestrator
+orchestrator = HelmOrchestrator(
+    # Chart archive path (relative to `conf/templates/`).
+    # [Optional] Default is `cli/helm/chart`
+    chart_location="cli/helm/mychart.tgz",
+
+    # The directory containing all main `values.yaml` files (relative to `conf/templates/`).
+    # [Optional] Default is `cli/helm/set-values`
+    helm_set_values_dir="cli/helm/set-values"
+
+    # The directory containing all key-specific files (relative to `conf/templates/`).
+    # [Optional] Default is `cli/helm/set-files`
+    helm_set_files_dir="cli/helm/set-files"
+)
+```
+
+##### Values
+
+Values can be supplied either:
+
+1. For a set key by placing files in `set-files` directory.
+    * The name of the key to set is derived from the directory structure and the name of the file
+      (up to the first dot encountered in the filename).
+2. Globally for any files dumped in the `set-values` directory.
+
+For example, given the following `cli/helm/` directory structure:
+
+```bash
+cli/helm/
+├── set-files/
+│  ├── baz/
+│  │  ├── foo.json
+│  │  └── qux.waldo.txt
+│  └── thud.bang.yml
+└── set-values/
+   ├── foo.yml
+   └── bar.txt
+```
+
+This would result in the following arguments being passed to helm:
+
+```bash
+--set-file baz.foo=cli/helm/set-files/baz/foo.json
+--set-file baz.qux=cli/helm/set-files/baz/qux.waldo.yml    # NOTE: Key is `qux` not `qux.waldo`.
+--set-file thud=cli/helm/set-files/thud.bang.yml           # NOTE: Key is `thud` not `thud.bang`.
+--values cli/helm/set-values/foo.yml
+--values cli/helm/set-values/bar.yml
+```
+
+##### Dev Mode Chart
+
+During development it would be slow to require packaging up the chart for any changes.
+Appcli provides a way to speed up development by allow for the chart to deployed directly from source.
+This is done by specifying the dev chart as an environment variable.
+
+```bash
+MYAPP_DEV_MODE=true MYAPP_DEV_MODE_HELM_CHART=/path/to/mychart python3 -m myapp service start
+```
+
+##### Kubeconfig
+
+A custom `kubeconfig` file can be used by specifying the `KUBECONFIG` environment variable.
+
+```bash
+KUBECONFIG=/opt/brightsparklabs/myapp/conf/.generated/config ./myapp ...
+```
+
+_NOTE:_ The `KUBECONFIG` file must be at a location which is mounted into the launch container.
+Refer to [Volume Mounts](#volume-mounts) for details on what volumes are mounted into the launch container.
+
 #### Custom Commands
 
 You can specify some custom top-level commands by adding click commands or command groups to the
 configuration object.  Assuming 'web' is the name of the service in the docker-compose.yml file
 which you wish to exec against, we can create three custom commands in the following example:
 
 - `myapp ls-root` which lists the contents of the root directory within the `web` service container
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bsl_appcli-3.0.0/bsl_appcli.egg-info/SOURCES.txt` & `bsl_appcli-3.1.0/bsl_appcli.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -51,10 +51,11 @@
 tests/configuration/test_configuration.py
 tests/configuration_manager/test_configuration_manager.py
 tests/configuration_manager/expected_generated/nesting/nested_baseline_file.py
 tests/configuration_manager/resources/templates/baseline/nesting/nested_baseline_file.py
 tests/configuration_state/test_configuration_state.py
 tests/crypto/test_crypto.py
 tests/git_repositories/test_git_repositories.py
+tests/orchestrators/test_helm_orchestrator.py
 tests/string_transformer/test_string_transformer.py
 tests/variables_manager/test_variables_manager.py
 tests/version/test_version.py
```

### Comparing `bsl_appcli-3.0.0/setup.py` & `bsl_appcli-3.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,27 +53,27 @@
     license="MIT License",
     author="brightSPARK Labs",
     author_email="enquire@brightsparklabs.com",
     url="https://www.brightsparklabs.com",
     packages=find_namespace_packages(exclude=["contrib", "docs", "tests"]),
     include_package_data=True,
     install_requires=[
-        "boto3==1.34.91",
+        "boto3==1.34.95",
         "click==8.1.7",
         "coloredlogs==15.0.1",
         "cronex==0.1.3.1",
         "dataclasses-json==0.5.7",
         "deepdiff==6.7.1",
         "GitPython==3.1.43",
-        "jsonschema==4.21.1",
-        "jinja2==3.1.3",
+        "jsonschema==4.22.0",
+        "jinja2==3.1.4",
         "pycryptodome==3.20.0",
         "pydantic==2.7.1",
         "pyfiglet==1.0.2",
         "python-keycloak==3.12.0",
         "python-slugify==8.0.4",
         "ruamel-yaml==0.18.6",
         "tabulate==0.9.0",
         "wheel==0.43.0",
     ],
-    extras_require={"dev": ["ruff", "pre-commit", "pytest"]},
+    extras_require={"dev": ["ruff==0.3.7", "pre-commit==3.7.0", "pytest==8.1.1"]},
 )
```

### Comparing `bsl_appcli-3.0.0/tests/backup_manager/test_backup_manager.py` & `bsl_appcli-3.1.0/tests/backup_manager/test_backup_manager.py`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/tests/cipher/test_cipher.py` & `bsl_appcli-3.1.0/tests/cipher/test_cipher.py`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/tests/commands/test_commands.py` & `bsl_appcli-3.1.0/tests/commands/test_commands.py`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/tests/commands/test_install_script.py` & `bsl_appcli-3.1.0/tests/commands/test_install_script.py`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/tests/commands_task/test_commands_task.py` & `bsl_appcli-3.1.0/tests/commands_task/test_commands_task.py`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/tests/configuration/test_configuration.py` & `bsl_appcli-3.1.0/tests/configuration/test_configuration.py`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/tests/configuration_manager/test_configuration_manager.py` & `bsl_appcli-3.1.0/tests/configuration_manager/test_configuration_manager.py`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/tests/configuration_state/test_configuration_state.py` & `bsl_appcli-3.1.0/tests/configuration_state/test_configuration_state.py`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/tests/crypto/test_crypto.py` & `bsl_appcli-3.1.0/tests/crypto/test_crypto.py`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/tests/git_repositories/test_git_repositories.py` & `bsl_appcli-3.1.0/tests/git_repositories/test_git_repositories.py`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/tests/string_transformer/test_string_transformer.py` & `bsl_appcli-3.1.0/tests/string_transformer/test_string_transformer.py`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/tests/variables_manager/test_variables_manager.py` & `bsl_appcli-3.1.0/tests/variables_manager/test_variables_manager.py`

 * *Files identical despite different names*

### Comparing `bsl_appcli-3.0.0/tests/version/test_version.py` & `bsl_appcli-3.1.0/tests/version/test_version.py`

 * *Files identical despite different names*

