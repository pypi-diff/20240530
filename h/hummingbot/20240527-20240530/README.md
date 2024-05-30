# Comparing `tmp/hummingbot-20240527.tar.gz` & `tmp/hummingbot-20240530.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hummingbot-20240527.tar", last modified: Thu May 30 17:49:49 2024, max compression
+gzip compressed data, was "hummingbot-20240530.tar", last modified: Thu May 30 19:52:28 2024, max compression
```

## Comparing `hummingbot-20240527.tar` & `hummingbot-20240530.tar`

### file list

```diff
@@ -1,966 +1,966 @@
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.381000 hummingbot-20240527/
--rw-r--r--   0 madcatz    (501) staff       (20)    11352 2024-05-30 17:40:42.000000 hummingbot-20240527/LICENSE
--rw-r--r--   0 madcatz    (501) staff       (20)     1771 2024-05-30 17:49:49.380897 hummingbot-20240527/PKG-INFO
--rw-r--r--   0 madcatz    (501) staff       (20)     9670 2024-05-30 17:40:42.000000 hummingbot-20240527/README.md
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:48.944497 hummingbot-20240527/bin/
--rwxr-xr-x   0 madcatz    (501) staff       (20)     6821 2024-05-30 17:40:42.000000 hummingbot-20240527/bin/hummingbot_quickstart.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:48.946070 hummingbot-20240527/hummingbot/
--rw-r--r--   0 madcatz    (501) staff       (20)        6 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/VERSION
--rw-r--r--   0 madcatz    (501) staff       (20)     5811 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/__init__.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:48.951988 hummingbot-20240527/hummingbot/client/
--rw-r--r--   0 madcatz    (501) staff       (20)      655 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/__init__.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:48.963509 hummingbot-20240527/hummingbot/client/command/
--rw-r--r--   0 madcatz    (501) staff       (20)     1249 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/command/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     9967 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/command/balance_command.py
--rw-r--r--   0 madcatz    (501) staff       (20)    22563 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/command/config_command.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6908 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/command/connect_command.py
--rw-r--r--   0 madcatz    (501) staff       (20)    16234 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/command/create_command.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1458 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/command/exit_command.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4844 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/command/export_command.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6371 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/command/gateway_api_manager.py
--rw-r--r--   0 madcatz    (501) staff       (20)    41186 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/command/gateway_command.py
--rw-r--r--   0 madcatz    (501) staff       (20)      916 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/command/help_command.py
--rw-r--r--   0 madcatz    (501) staff       (20)    12319 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/command/history_command.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3698 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/command/import_command.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4566 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/command/mqtt_command.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3001 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/command/order_book_command.py
--rw-r--r--   0 madcatz    (501) staff       (20)      344 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/command/pmm_script_command.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2571 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/command/previous_strategy_command.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2697 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/command/rate_command.py
--rw-r--r--   0 madcatz    (501) staff       (20)     9686 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/command/silly_commands.py
--rw-r--r--   0 madcatz    (501) staff       (20)    15078 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/command/start_command.py
--rw-r--r--   0 madcatz    (501) staff       (20)    10502 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/command/status_command.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2552 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/command/stop_command.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2996 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/command/ticker_command.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:48.970761 hummingbot-20240527/hummingbot/client/config/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/config/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    41900 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/config/client_config_map.py
--rw-r--r--   0 madcatz    (501) staff       (20)    18418 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/config/conf_migration.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4553 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/config/config_crypt.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2608 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/config/config_data_types.py
--rw-r--r--   0 madcatz    (501) staff       (20)    38116 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/config/config_helpers.py
--rw-r--r--   0 madcatz    (501) staff       (20)      633 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/config/config_methods.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7452 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/config/config_validators.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3189 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/config/config_var.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1404 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/config/fee_overrides_config_map.py
--rw-r--r--   0 madcatz    (501) staff       (20)      364 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/config/gateway_ssl_config_map.py
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/config/global_config_map.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3858 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/config/security.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6288 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/config/strategy_config_data_types.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3003 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/config/trade_fee_schema_loader.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:48.971216 hummingbot-20240527/hummingbot/client/data_type/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/data_type/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      426 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/data_type/currency_amount.py
--rw-r--r--   0 madcatz    (501) staff       (20)    15273 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/hummingbot_application.py
--rw-r--r--   0 madcatz    (501) staff       (20)    13787 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/performance.py
--rw-r--r--   0 madcatz    (501) staff       (20)      516 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/platform.py
--rw-r--r--   0 madcatz    (501) staff       (20)    27252 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/settings.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:48.973225 hummingbot-20240527/hummingbot/client/tab/
--rw-r--r--   0 madcatz    (501) staff       (20)      135 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/tab/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      872 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/tab/data_types.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3140 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/tab/order_book_tab.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1723 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/tab/tab_base.py
--rw-r--r--   0 madcatz    (501) staff       (20)      774 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/tab/tab_example_tab.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:48.978728 hummingbot-20240527/hummingbot/client/ui/
--rw-r--r--   0 madcatz    (501) staff       (20)     8435 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/ui/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    24695 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/ui/completer.py
--rw-r--r--   0 madcatz    (501) staff       (20)     9614 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/ui/custom_widgets.py
--rw-r--r--   0 madcatz    (501) staff       (20)    11623 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/ui/hummingbot_cli.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4952 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/ui/interface_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3593 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/ui/keybindings.py
--rw-r--r--   0 madcatz    (501) staff       (20)    11632 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/ui/layout.py
--rw-r--r--   0 madcatz    (501) staff       (20)    11856 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/ui/parser.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1710 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/ui/scroll_handlers.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2524 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/ui/stdout_redirection.py
--rw-r--r--   0 madcatz    (501) staff       (20)    11314 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/client/ui/style.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:48.994187 hummingbot-20240527/hummingbot/connector/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7400 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/budget_checker.py
--rw-r--r--   0 madcatz    (501) staff       (20)    18938 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/client_order_tracker.py
--rw-r--r--   0 madcatz    (501) staff       (20)  1403631 2024-05-30 17:49:45.000000 hummingbot-20240527/hummingbot/connector/connector_base.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     6375 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/connector_metrics_collector.py
--rw-r--r--   0 madcatz    (501) staff       (20)      215 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/constants.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:48.996133 hummingbot-20240527/hummingbot/connector/derivative/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/__init__.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.004161 hummingbot-20240527/hummingbot/connector/derivative/binance_perpetual/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/binance_perpetual/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     9683 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1944 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6016 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    38371 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_derivative.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6334 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2428 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4013 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_web_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)   341295 2024-05-30 17:49:45.000000 hummingbot-20240527/hummingbot/connector/derivative/binance_perpetual/dummy.cpp
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.008433 hummingbot-20240527/hummingbot/connector/derivative/bit_com_perpetual/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/bit_com_perpetual/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    10413 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3497 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4597 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    35998 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_derivative.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5494 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2420 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2670 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_web_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)   341295 2024-05-30 17:49:45.000000 hummingbot-20240527/hummingbot/connector/derivative/bit_com_perpetual/dummy.cpp
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.012410 hummingbot-20240527/hummingbot/connector/derivative/bitget_perpetual/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/bitget_perpetual/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    12125 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2898 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5025 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    40405 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_derivative.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5830 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2002 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3142 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_web_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.016260 hummingbot-20240527/hummingbot/connector/derivative/bybit_perpetual/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/bybit_perpetual/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    15468 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3238 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5848 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    38897 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_derivative.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6821 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4168 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)    19340 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_web_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)   341067 2024-05-30 17:49:45.000000 hummingbot-20240527/hummingbot/connector/derivative/bybit_perpetual/dummy.cpp
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.019354 hummingbot-20240527/hummingbot/connector/derivative/dydx_perpetual/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/dydx_perpetual/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    12544 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4454 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3774 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    40418 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_derivative.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2566 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2154 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2663 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_web_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.023273 hummingbot-20240527/hummingbot/connector/derivative/gate_io_perpetual/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/gate_io_perpetual/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)   341295 2024-05-30 17:49:45.000000 hummingbot-20240527/hummingbot/connector/derivative/gate_io_perpetual/dummy.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)    10758 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3135 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5254 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    34398 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_derivative.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4492 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1634 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1851 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_web_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.026533 hummingbot-20240527/hummingbot/connector/derivative/hyperliquid_perpetual/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/hyperliquid_perpetual/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)   341751 2024-05-30 17:49:45.000000 hummingbot-20240527/hummingbot/connector/derivative/hyperliquid_perpetual/dummy.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)    10842 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6022 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3695 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    36109 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_derivative.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5656 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4106 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5213 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_web_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.029009 hummingbot-20240527/hummingbot/connector/derivative/injective_v2_perpetual/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/injective_v2_perpetual/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      466 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/injective_v2_perpetual/injective_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4840 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/injective_v2_perpetual/injective_v2_perpetual_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)    48511 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/injective_v2_perpetual/injective_v2_perpetual_derivative.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3981 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/injective_v2_perpetual/injective_v2_perpetual_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)      410 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/injective_v2_perpetual/injective_v2_perpetual_web_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.033014 hummingbot-20240527/hummingbot/connector/derivative/kucoin_perpetual/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/kucoin_perpetual/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)   341181 2024-05-30 17:49:45.000000 hummingbot-20240527/hummingbot/connector/derivative/kucoin_perpetual/dummy.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)    14498 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     8026 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_api_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6301 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6066 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    45173 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_derivative.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2117 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6479 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_web_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.040778 hummingbot-20240527/hummingbot/connector/derivative/okx_perpetual/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/okx_perpetual/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    20796 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5462 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6000 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    39008 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_derivative.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6527 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2707 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)    12961 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_web_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1421 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/perpetual_budget_checker.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.044358 hummingbot-20240527/hummingbot/connector/derivative/phemex_perpetual/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/phemex_perpetual/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    12075 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5017 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_api_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2335 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6113 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    32650 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_derivative.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2679 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3838 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_web_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2238 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/position.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.048712 hummingbot-20240527/hummingbot/connector/derivative/vega_perpetual/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/vega_perpetual/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    14929 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3977 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     9352 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1466 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_data.py
--rw-r--r--   0 madcatz    (501) staff       (20)    66373 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_derivative.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6581 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2481 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6529 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_web_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2528 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/derivative_base.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.049100 hummingbot-20240527/hummingbot/connector/exchange/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/__init__.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.052592 hummingbot-20240527/hummingbot/connector/exchange/ascend_ex/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/ascend_ex/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7240 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/ascend_ex/ascend_ex_api_order_book_data_source.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)     3627 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/ascend_ex/ascend_ex_api_user_stream_data_source.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)     2478 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/ascend_ex/ascend_ex_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5036 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/ascend_ex/ascend_ex_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    26170 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/ascend_ex/ascend_ex_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2084 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/ascend_ex/ascend_ex_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2719 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/ascend_ex/ascend_ex_web_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.056105 hummingbot-20240527/hummingbot/connector/exchange/binance/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/binance/__init__.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)     6402 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/binance/binance_api_order_book_data_source.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)     6081 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/binance/binance_api_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2413 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/binance/binance_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4688 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/binance/binance_constants.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)    25993 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/binance/binance_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3224 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/binance/binance_order_book.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2972 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/binance/binance_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3154 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/binance/binance_web_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)   339765 2024-05-30 17:49:45.000000 hummingbot-20240527/hummingbot/connector/exchange/binance/dummy.cpp
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.067721 hummingbot-20240527/hummingbot/connector/exchange/bitfinex/
--rw-r--r--   0 madcatz    (501) staff       (20)     1257 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/bitfinex/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)   785720 2024-05-30 17:49:45.000000 hummingbot-20240527/hummingbot/connector/exchange/bitfinex/bitfinex_active_order_tracker.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)    22384 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/bitfinex/bitfinex_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2224 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/bitfinex/bitfinex_api_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1580 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/bitfinex/bitfinex_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)  3066713 2024-05-30 17:49:45.000000 hummingbot-20240527/hummingbot/connector/exchange/bitfinex/bitfinex_exchange.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)   554137 2024-05-30 17:49:45.000000 hummingbot-20240527/hummingbot/connector/exchange/bitfinex/bitfinex_in_flight_order.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)   576560 2024-05-30 17:49:45.000000 hummingbot-20240527/hummingbot/connector/exchange/bitfinex/bitfinex_order_book.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     1273 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/bitfinex/bitfinex_order_book_message.py
--rw-r--r--   0 madcatz    (501) staff       (20)    10355 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/bitfinex/bitfinex_order_book_tracker.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1057 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/bitfinex/bitfinex_order_book_tracker_entry.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2052 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/bitfinex/bitfinex_user_stream_tracker.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3928 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/bitfinex/bitfinex_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5028 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/bitfinex/bitfinex_websocket.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.071628 hummingbot-20240527/hummingbot/connector/exchange/bitmart/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/bitmart/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    10154 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/bitmart/bitmart_api_order_book_data_source.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)     4787 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/bitmart/bitmart_api_user_stream_data_source.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)     2913 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/bitmart/bitmart_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2473 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/bitmart/bitmart_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    19821 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/bitmart/bitmart_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2451 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/bitmart/bitmart_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2538 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/bitmart/bitmart_web_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)   339765 2024-05-30 17:49:45.000000 hummingbot-20240527/hummingbot/connector/exchange/bitmart/dummy.cpp
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.076417 hummingbot-20240527/hummingbot/connector/exchange/bitrue/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/bitrue/__init__.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)     8798 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/bitrue/bitrue_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2385 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/bitrue/bitrue_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6008 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/bitrue/bitrue_constants.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)    30434 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/bitrue/bitrue_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3211 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/bitrue/bitrue_order_book.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)     8058 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/bitrue/bitrue_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1604 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/bitrue/bitrue_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3128 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/bitrue/bitrue_web_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.080733 hummingbot-20240527/hummingbot/connector/exchange/btc_markets/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/btc_markets/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     9564 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/btc_markets/btc_markets_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4055 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/btc_markets/btc_markets_api_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4543 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/btc_markets/btc_markets_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3114 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/btc_markets/btc_markets_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    25469 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/btc_markets/btc_markets_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4545 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/btc_markets/btc_markets_order_book.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1662 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/btc_markets/btc_markets_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2831 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/btc_markets/btc_markets_web_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.085084 hummingbot-20240527/hummingbot/connector/exchange/bybit/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/bybit/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    12169 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/bybit/bybit_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5372 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/bybit/bybit_api_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3308 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/bybit/bybit_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4659 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/bybit/bybit_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    21562 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/bybit/bybit_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4246 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/bybit/bybit_order_book.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2581 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/bybit/bybit_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5170 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/bybit/bybit_web_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)   339537 2024-05-30 17:49:45.000000 hummingbot-20240527/hummingbot/connector/exchange/bybit/dummy.cpp
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.090359 hummingbot-20240527/hummingbot/connector/exchange/coinbase_advanced_trade/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/coinbase_advanced_trade/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    11069 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)    13923 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_api_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)    12512 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5500 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    50376 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7810 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_order_book.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2030 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7161 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_web_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)   341676 2024-05-30 17:49:45.000000 hummingbot-20240527/hummingbot/connector/exchange/coinbase_advanced_trade/dummy.cpp
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.105084 hummingbot-20240527/hummingbot/connector/exchange/coinbase_pro/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/coinbase_pro/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)   927886 2024-05-30 17:49:45.000000 hummingbot-20240527/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_active_order_tracker.cpp
--rwxr-xr-x   0 madcatz    (501) staff       (20)    14517 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_api_order_book_data_source.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)     5006 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_api_user_stream_data_source.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)     2753 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)      493 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)  2596602 2024-05-30 17:49:45.000000 hummingbot-20240527/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_exchange.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)   499653 2024-05-30 17:49:45.000000 hummingbot-20240527/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_in_flight_order.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)   535437 2024-05-30 17:49:45.000000 hummingbot-20240527/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_order_book.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     1816 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_order_book_message.py
--rw-r--r--   0 madcatz    (501) staff       (20)     8848 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_order_book_tracker.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1041 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_order_book_tracker_entry.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2361 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_user_stream_tracker.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2530 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.109741 hummingbot-20240527/hummingbot/connector/exchange/cube/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/cube/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    11507 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/cube/cube_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3570 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/cube/cube_api_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3643 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/cube/cube_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3371 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/cube/cube_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    52528 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/cube/cube_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4473 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/cube/cube_order_book.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4547 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/cube/cube_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1660 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/cube/cube_web_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.112127 hummingbot-20240527/hummingbot/connector/exchange/cube/cube_ws_protobufs/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/cube/cube_ws_protobufs/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    10219 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/cube/cube_ws_protobufs/market_data_pb2.py
--rw-r--r--   0 madcatz    (501) staff       (20)    15363 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/cube/cube_ws_protobufs/market_data_pb2.pyi
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/cube/cube_ws_protobufs/py.typed
--rw-r--r--   0 madcatz    (501) staff       (20)    15992 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/cube/cube_ws_protobufs/trade_pb2.py
--rw-r--r--   0 madcatz    (501) staff       (20)    29121 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/cube/cube_ws_protobufs/trade_pb2.pyi
--rw-r--r--   0 madcatz    (501) staff       (20)   339423 2024-05-30 17:49:45.000000 hummingbot-20240527/hummingbot/connector/exchange/cube/dummy.cpp
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.116449 hummingbot-20240527/hummingbot/connector/exchange/foxbit/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/foxbit/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    10078 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/foxbit/foxbit_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5190 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/foxbit/foxbit_api_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3912 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/foxbit/foxbit_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)   345010 2024-05-30 17:49:45.000000 hummingbot-20240527/hummingbot/connector/exchange/foxbit/foxbit_connector.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     5253 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/foxbit/foxbit_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    44815 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/foxbit/foxbit_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7671 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/foxbit/foxbit_order_book.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5090 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/foxbit/foxbit_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4155 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/foxbit/foxbit_web_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.120285 hummingbot-20240527/hummingbot/connector/exchange/gate_io/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/gate_io/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7620 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/gate_io/gate_io_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4310 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/gate_io/gate_io_api_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3166 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/gate_io/gate_io_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3528 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/gate_io/gate_io_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    22712 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/gate_io/gate_io_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1255 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/gate_io/gate_io_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1834 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/gate_io/gate_io_web_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)   341880 2024-05-30 17:49:45.000000 hummingbot-20240527/hummingbot/connector/exchange/gate_io/placeholder.cpp
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.128078 hummingbot-20240527/hummingbot/connector/exchange/hitbtc/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/hitbtc/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)   754445 2024-05-30 17:49:45.000000 hummingbot-20240527/hummingbot/connector/exchange/hitbtc/hitbtc_active_order_tracker.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)    11733 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/hitbtc/hitbtc_api_order_book_data_source.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)     3224 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/hitbtc/hitbtc_api_user_stream_data_source.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)     2451 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/hitbtc/hitbtc_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1847 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/hitbtc/hitbtc_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    42970 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/hitbtc/hitbtc_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3162 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/hitbtc/hitbtc_in_flight_order.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3455 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/hitbtc/hitbtc_order_book.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2397 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/hitbtc/hitbtc_order_book_message.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5637 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/hitbtc/hitbtc_order_book_tracker.py
--rw-r--r--   0 madcatz    (501) staff       (20)      945 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/hitbtc/hitbtc_order_book_tracker_entry.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2346 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/hitbtc/hitbtc_user_stream_tracker.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5706 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/hitbtc/hitbtc_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4686 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/hitbtc/hitbtc_websocket.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.131493 hummingbot-20240527/hummingbot/connector/exchange/htx/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/htx/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     8241 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/htx/htx_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5047 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/htx/htx_api_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3477 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/htx/htx_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2958 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/htx/htx_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    18960 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/htx/htx_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1589 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/htx/htx_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2553 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/htx/htx_web_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.135544 hummingbot-20240527/hummingbot/connector/exchange/injective_v2/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/injective_v2/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4257 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/injective_v2/account_delegation_script.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.140944 hummingbot-20240527/hummingbot/connector/exchange/injective_v2/data_sources/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/injective_v2/data_sources/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    71837 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/injective_v2/data_sources/injective_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)    23529 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/injective_v2/data_sources/injective_grantee_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)    12854 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/injective_v2/data_sources/injective_read_only_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)    24074 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/injective_v2/data_sources/injective_vaults_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5962 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/injective_v2/injective_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)       90 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/injective_v2/injective_events.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4376 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/injective_v2/injective_market.py
--rw-r--r--   0 madcatz    (501) staff       (20)    14999 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/injective_v2/injective_query_executor.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3669 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/injective_v2/injective_v2_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)    42627 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/injective_v2/injective_v2_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)    15808 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/injective_v2/injective_v2_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)      410 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/injective_v2/injective_v2_web_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.146476 hummingbot-20240527/hummingbot/connector/exchange/kraken/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/kraken/__init__.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)     7715 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/kraken/kraken_api_order_book_data_source.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)     3909 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/kraken/kraken_api_user_stream_data_source.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)     2929 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/kraken/kraken_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4146 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/kraken/kraken_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    27389 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/kraken/kraken_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2903 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/kraken/kraken_order_book.py
--rw-r--r--   0 madcatz    (501) staff       (20)     8041 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/kraken/kraken_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1660 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/kraken/kraken_web_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.150532 hummingbot-20240527/hummingbot/connector/exchange/kucoin/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/kucoin/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)   339651 2024-05-30 17:49:45.000000 hummingbot-20240527/hummingbot/connector/exchange/kucoin/dummy.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     8742 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/kucoin/kucoin_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4879 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/kucoin/kucoin_api_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3663 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/kucoin/kucoin_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3297 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/kucoin/kucoin_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    24398 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/kucoin/kucoin_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2132 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/kucoin/kucoin_order_book_message.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3049 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/kucoin/kucoin_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3215 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/kucoin/kucoin_web_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.154520 hummingbot-20240527/hummingbot/connector/exchange/mexc/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/mexc/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)   339423 2024-05-30 17:49:45.000000 hummingbot-20240527/hummingbot/connector/exchange/mexc/dummy.cpp
--rwxr-xr-x   0 madcatz    (501) staff       (20)     6556 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/mexc/mexc_api_order_book_data_source.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)     8131 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/mexc/mexc_api_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2480 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/mexc/mexc_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4344 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/mexc/mexc_constants.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)    26610 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/mexc/mexc_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3481 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/mexc/mexc_order_book.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1705 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/mexc/mexc_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3142 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/mexc/mexc_web_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.160485 hummingbot-20240527/hummingbot/connector/exchange/ndax/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/ndax/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)   339423 2024-05-30 17:49:45.000000 hummingbot-20240527/hummingbot/connector/exchange/ndax/dummy.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)    15461 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/ndax/ndax_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5670 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/ndax/ndax_api_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2103 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/ndax/ndax_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5426 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/ndax/ndax_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    49594 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/ndax/ndax_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2421 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/ndax/ndax_in_flight_order.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3556 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/ndax/ndax_order_book.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3561 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/ndax/ndax_order_book_message.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5934 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/ndax/ndax_order_book_tracker.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2369 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/ndax/ndax_user_stream_tracker.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4179 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/ndax/ndax_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3928 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/ndax/ndax_websocket_adaptor.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.163527 hummingbot-20240527/hummingbot/connector/exchange/okx/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/okx/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     9214 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/okx/okx_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4432 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/okx/okx_api_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3330 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/okx/okx_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2775 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/okx/okx_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    18614 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/okx/okx_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1761 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/okx/okx_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2723 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/okx/okx_web_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.165824 hummingbot-20240527/hummingbot/connector/exchange/paper_trade/
--rw-r--r--   0 madcatz    (501) staff       (20)     1293 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/paper_trade/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      910 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/paper_trade/market_config.py
--rw-r--r--   0 madcatz    (501) staff       (20)  2193488 2024-05-30 17:49:46.000000 hummingbot-20240527/hummingbot/connector/exchange/paper_trade/paper_trade_exchange.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)      126 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/paper_trade/trading_pair.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.172891 hummingbot-20240527/hummingbot/connector/exchange/polkadex/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/polkadex/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4527 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/polkadex/polkadex_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4188 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/polkadex/polkadex_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    26470 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/polkadex/polkadex_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)    18334 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/polkadex/polkadex_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)    19864 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/polkadex/polkadex_query_executor.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2076 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/polkadex/polkadex_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)      405 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/polkadex/polkadex_web_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.179951 hummingbot-20240527/hummingbot/connector/exchange/vertex/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/vertex/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)   343537 2024-05-30 17:49:45.000000 hummingbot-20240527/hummingbot/connector/exchange/vertex/dummy.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     7949 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/vertex/vertex_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5123 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/vertex/vertex_api_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3400 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/vertex/vertex_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)    10086 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/vertex/vertex_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)      959 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/vertex/vertex_eip712_structs.py
--rw-r--r--   0 madcatz    (501) staff       (20)    40072 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/vertex/vertex_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4655 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/vertex/vertex_order_book.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7773 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/vertex/vertex_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1774 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange/vertex/vertex_web_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)  1444488 2024-05-30 17:49:46.000000 hummingbot-20240527/hummingbot/connector/exchange_base.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)    45930 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/exchange_py_base.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.182411 hummingbot-20240527/hummingbot/connector/gateway/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/__init__.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.184668 hummingbot-20240527/hummingbot/connector/gateway/amm/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/amm/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    10973 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/amm/gateway_algorand_amm.py
--rw-r--r--   0 madcatz    (501) staff       (20)    46320 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/amm/gateway_evm_amm.py
--rw-r--r--   0 madcatz    (501) staff       (20)     9794 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/amm/gateway_near_amm.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5794 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/amm/gateway_tezos_amm.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.186219 hummingbot-20240527/hummingbot/connector/gateway/amm_lp/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/amm_lp/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    58500 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/amm_lp/gateway_evm_amm_lp.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4735 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/amm_lp/gateway_in_flight_lp_order.py
--rw-r--r--   0 madcatz    (501) staff       (20)    56750 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/amm_lp/gateway_osmosis_amm_lp.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.186842 hummingbot-20240527/hummingbot/connector/gateway/amm_perpetual/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/amm_perpetual/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    26154 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/amm_perpetual/gateway_evm_amm_perpetual.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.188215 hummingbot-20240527/hummingbot/connector/gateway/clob_perp/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/clob_perp/__init__.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.188776 hummingbot-20240527/hummingbot/connector/gateway/clob_perp/data_sources/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/clob_perp/data_sources/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1425 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/clob_perp/data_sources/clob_perp_api_data_source_base.py
--rw-r--r--   0 madcatz    (501) staff       (20)    21799 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/clob_perp/gateway_clob_perp.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4144 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/clob_perp/gateway_clob_perp_api_order_book_data_source.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.189694 hummingbot-20240527/hummingbot/connector/gateway/clob_spot/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/clob_spot/__init__.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.191176 hummingbot-20240527/hummingbot/connector/gateway/clob_spot/data_sources/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/clob_spot/data_sources/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7967 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/clob_spot/data_sources/clob_api_data_source_base.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.193879 hummingbot-20240527/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    29847 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/dexalot_api_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1779 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/dexalot_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3455 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/dexalot_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1296 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/dexalot_web_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)    18003 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/clob_spot/data_sources/gateway_clob_api_data_source_base.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.195932 hummingbot-20240527/hummingbot/connector/gateway/clob_spot/data_sources/kujira/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/clob_spot/data_sources/kujira/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    40889 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/clob_spot/data_sources/kujira/kujira_api_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)      315 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/clob_spot/data_sources/kujira/kujira_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1952 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/clob_spot/data_sources/kujira/kujira_helpers.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4659 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/clob_spot/data_sources/kujira/kujira_types.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.197077 hummingbot-20240527/hummingbot/connector/gateway/clob_spot/data_sources/xrpl/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/clob_spot/data_sources/xrpl/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    17880 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/clob_spot/data_sources/xrpl/xrpl_api_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2560 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/clob_spot/data_sources/xrpl/xrpl_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3244 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/clob_spot/gateway_clob_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)    31044 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/clob_spot/gateway_clob_spot.py
--rw-r--r--   0 madcatz    (501) staff       (20)      944 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/common_types.py
--rw-r--r--   0 madcatz    (501) staff       (20)    10185 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/gateway_in_flight_order.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2230 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/gateway_order_tracker.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6890 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/gateway/gateway_price_shim.py
--rw-r--r--   0 madcatz    (501) staff       (20)   857765 2024-05-30 17:49:45.000000 hummingbot-20240527/hummingbot/connector/in_flight_order_base.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)    29014 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/markets_recorder.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.197636 hummingbot-20240527/hummingbot/connector/other/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/other/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6037 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/parrot.py
--rw-r--r--   0 madcatz    (501) staff       (20)    17636 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/perpetual_derivative_py_base.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7622 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/perpetual_trading.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.203637 hummingbot-20240527/hummingbot/connector/test_support/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/test_support/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    86233 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/test_support/exchange_connector_test.py
--rw-r--r--   0 madcatz    (501) staff       (20)    42837 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/test_support/gateway_clob_api_data_source_test.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1411 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/test_support/mock_order_tracker.py
--rw-r--r--   0 madcatz    (501) staff       (20)   813971 2024-05-30 17:49:46.000000 hummingbot-20240527/hummingbot/connector/test_support/mock_paper_exchange.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)      227 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/test_support/mock_pure_python_paper_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     8740 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/test_support/network_mocking_assistant.py
--rw-r--r--   0 madcatz    (501) staff       (20)    44545 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/test_support/oms_exchange_connector_test.py
--rw-r--r--   0 madcatz    (501) staff       (20)    33536 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/test_support/perpetual_derivative_test.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3607 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/time_synchronizer.py
--rw-r--r--   0 madcatz    (501) staff       (20)   531657 2024-05-30 17:49:45.000000 hummingbot-20240527/hummingbot/connector/trading_rule.cpp
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.204262 hummingbot-20240527/hummingbot/connector/utilities/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/utilities/__init__.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.206989 hummingbot-20240527/hummingbot/connector/utilities/oms_connector/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/utilities/oms_connector/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     8912 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/utilities/oms_connector/oms_connector_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3929 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/utilities/oms_connector/oms_connector_api_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2849 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/utilities/oms_connector/oms_connector_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5724 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/utilities/oms_connector/oms_connector_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    25851 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/utilities/oms_connector/oms_connector_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)      641 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/utilities/oms_connector/oms_connector_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2789 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/utilities/oms_connector/oms_connector_web_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4992 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/connector/utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.211513 hummingbot-20240527/hummingbot/core/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/__init__.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.213941 hummingbot-20240527/hummingbot/core/api_throttler/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/api_throttler/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3565 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/api_throttler/async_request_context_base.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3888 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/api_throttler/async_throttler.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3875 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/api_throttler/async_throttler_base.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1789 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/api_throttler/data_types.py
--rw-r--r--   0 madcatz    (501) staff       (20)   699724 2024-05-30 17:49:45.000000 hummingbot-20240527/hummingbot/core/clock.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)      104 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/clock_mode.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.218038 hummingbot-20240527/hummingbot/core/cpp/
--rw-r--r--   0 madcatz    (501) staff       (20)     4793 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/cpp/LimitOrder.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     1832 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/cpp/LimitOrder.h
--rw-r--r--   0 madcatz    (501) staff       (20)     3183 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/cpp/OrderBookEntry.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)      991 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/cpp/OrderBookEntry.h
--rw-r--r--   0 madcatz    (501) staff       (20)     1825 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/cpp/OrderExpirationEntry.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)      868 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/cpp/OrderExpirationEntry.h
--rw-r--r--   0 madcatz    (501) staff       (20)      684 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/cpp/PyRef.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)      503 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/cpp/PyRef.h
--rw-r--r--   0 madcatz    (501) staff       (20)     3086 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/cpp/TestOrderBookEntry.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)       19 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/cpp/Utils.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)      246 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/cpp/Utils.h
--rwxr-xr-x   0 madcatz    (501) staff       (20)      139 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/cpp/compile.sh
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.233244 hummingbot-20240527/hummingbot/core/data_type/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/data_type/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      129 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/data_type/cancellation_result.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1067 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/data_type/common.py
--rw-r--r--   0 madcatz    (501) staff       (20)   707148 2024-05-30 17:49:46.000000 hummingbot-20240527/hummingbot/core/data_type/composite_order_book.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     2052 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/data_type/funding_info.py
--rw-r--r--   0 madcatz    (501) staff       (20)    14142 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/data_type/in_flight_order.py
--rw-r--r--   0 madcatz    (501) staff       (20)   664173 2024-05-30 17:49:46.000000 hummingbot-20240527/hummingbot/core/data_type/limit_order.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     1836 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/data_type/market_order.py
--rw-r--r--   0 madcatz    (501) staff       (20)  1140705 2024-05-30 17:49:46.000000 hummingbot-20240527/hummingbot/core/data_type/order_book.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     2989 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/data_type/order_book_message.py
--rw-r--r--   0 madcatz    (501) staff       (20)   390625 2024-05-30 17:49:46.000000 hummingbot-20240527/hummingbot/core/data_type/order_book_query_result.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)      587 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/data_type/order_book_row.py
--rw-r--r--   0 madcatz    (501) staff       (20)    15929 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/data_type/order_book_tracker.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)    11594 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/data_type/order_book_tracker_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)      776 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/data_type/order_book_tracker_entry.py
--rw-r--r--   0 madcatz    (501) staff       (20)    15612 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/data_type/order_candidate.py
--rw-r--r--   0 madcatz    (501) staff       (20)   408361 2024-05-30 17:49:46.000000 hummingbot-20240527/hummingbot/core/data_type/order_expiration_entry.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     1809 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/data_type/perpetual_api_order_book_data_source.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)     5496 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/data_type/remote_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1843 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/data_type/trade.py
--rw-r--r--   0 madcatz    (501) staff       (20)    12881 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/data_type/trade_fee.py
--rw-r--r--   0 madcatz    (501) staff       (20)   371702 2024-05-30 17:49:46.000000 hummingbot-20240527/hummingbot/core/data_type/transaction_tracker.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     1310 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/data_type/user_stream_tracker.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)     3994 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/data_type/user_stream_tracker_data_source.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.235562 hummingbot-20240527/hummingbot/core/event/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/event/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      754 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/event/event_forwarder.py
--rw-r--r--   0 madcatz    (501) staff       (20)   402941 2024-05-30 17:49:46.000000 hummingbot-20240527/hummingbot/core/event/event_listener.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)   604746 2024-05-30 17:49:46.000000 hummingbot-20240527/hummingbot/core/event/event_logger.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)   448102 2024-05-30 17:49:46.000000 hummingbot-20240527/hummingbot/core/event/event_reporter.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     8411 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/event/events.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.241418 hummingbot-20240527/hummingbot/core/gateway/
--rw-r--r--   0 madcatz    (501) staff       (20)     5198 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/gateway/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    42014 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/gateway/gateway_http_client.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5292 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/gateway/gateway_status_monitor.py
--rw-r--r--   0 madcatz    (501) staff       (20)      892 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/gateway/utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.242382 hummingbot-20240527/hummingbot/core/management/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/management/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2632 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/management/console.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1325 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/management/diagnosis.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.243711 hummingbot-20240527/hummingbot/core/mock_api/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/mock_api/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2827 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/mock_api/mock_mqtt_server.py
--rw-r--r--   0 madcatz    (501) staff       (20)     9206 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/mock_api/mock_web_server.py
--rw-r--r--   0 madcatz    (501) staff       (20)     8409 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/mock_api/mock_web_socket_server.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4386 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/network_base.py
--rw-r--r--   0 madcatz    (501) staff       (20)   680641 2024-05-30 17:49:46.000000 hummingbot-20240527/hummingbot/core/network_iterator.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)   498964 2024-05-30 17:49:46.000000 hummingbot-20240527/hummingbot/core/pubsub.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)   331173 2024-05-30 17:49:46.000000 hummingbot-20240527/hummingbot/core/py_time_iterator.cpp
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.244829 hummingbot-20240527/hummingbot/core/rate_oracle/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/rate_oracle/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     8190 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/rate_oracle/rate_oracle.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.248216 hummingbot-20240527/hummingbot/core/rate_oracle/sources/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/rate_oracle/sources/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2207 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/rate_oracle/sources/ascend_ex_rate_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3589 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/rate_oracle/sources/binance_rate_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3624 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/rate_oracle/sources/binance_us_rate_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1386 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/rate_oracle/sources/coin_cap_rate_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7211 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/rate_oracle/sources/coin_gecko_rate_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3578 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/rate_oracle/sources/coinbase_advanced_trade_rate_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3871 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/rate_oracle/sources/cube_rate_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2800 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/rate_oracle/sources/gate_io_rate_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2349 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/rate_oracle/sources/kucoin_rate_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)      605 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/rate_oracle/sources/rate_source_base.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1678 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/rate_oracle/utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)   394085 2024-05-30 17:49:46.000000 hummingbot-20240527/hummingbot/core/time_iterator.cpp
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.252630 hummingbot-20240527/hummingbot/core/utils/
--rw-r--r--   0 madcatz    (501) staff       (20)     1257 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/utils/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4470 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/utils/async_call_scheduler.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2486 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/utils/async_retry.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2031 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/utils/async_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3613 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/utils/estimate_fee.py
--rw-r--r--   0 madcatz    (501) staff       (20)      892 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/utils/fixed_rate_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5970 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/utils/gateway_config_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2821 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/utils/kill_switch.py
--rw-r--r--   0 madcatz    (501) staff       (20)      940 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/utils/market_price.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7907 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/utils/ssl_cert.py
--rw-r--r--   0 madcatz    (501) staff       (20)      675 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/utils/ssl_client_request.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2203 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/utils/tracking_nonce.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4187 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/utils/trading_pair_fetcher.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.255564 hummingbot-20240527/hummingbot/core/web_assistant/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/web_assistant/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      696 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/web_assistant/auth.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.257048 hummingbot-20240527/hummingbot/core/web_assistant/connections/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/web_assistant/connections/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1834 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/web_assistant/connections/connections_factory.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4371 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/web_assistant/connections/data_types.py
--rw-r--r--   0 madcatz    (501) staff       (20)      797 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/web_assistant/connections/rest_connection.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4767 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/web_assistant/connections/ws_connection.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5116 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/web_assistant/rest_assistant.py
--rw-r--r--   0 madcatz    (501) staff       (20)      467 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/web_assistant/rest_post_processors.py
--rw-r--r--   0 madcatz    (501) staff       (20)      460 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/web_assistant/rest_pre_processors.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2883 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/web_assistant/web_assistants_factory.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3740 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/web_assistant/ws_assistant.py
--rw-r--r--   0 madcatz    (501) staff       (20)      457 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/web_assistant/ws_post_processors.py
--rw-r--r--   0 madcatz    (501) staff       (20)      450 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/core/web_assistant/ws_pre_processors.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.258999 hummingbot-20240527/hummingbot/data_feed/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5140 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/amm_gateway_data_feed.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.260510 hummingbot-20240527/hummingbot/data_feed/candles_feed/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/candles_feed/__init__.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.261476 hummingbot-20240527/hummingbot/data_feed/candles_feed/ascend_ex_spot_candles/
--rw-r--r--   0 madcatz    (501) staff       (20)      147 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/candles_feed/ascend_ex_spot_candles/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     8002 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/candles_feed/ascend_ex_spot_candles/ascend_ex_spot_candles.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1086 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/candles_feed/ascend_ex_spot_candles/constants.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.262513 hummingbot-20240527/hummingbot/data_feed/candles_feed/binance_perpetual_candles/
--rw-r--r--   0 madcatz    (501) staff       (20)      170 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/candles_feed/binance_perpetual_candles/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7298 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/candles_feed/binance_perpetual_candles/binance_perpetual_candles.py
--rw-r--r--   0 madcatz    (501) staff       (20)      897 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/candles_feed/binance_perpetual_candles/constants.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.263318 hummingbot-20240527/hummingbot/data_feed/candles_feed/binance_spot_candles/
--rw-r--r--   0 madcatz    (501) staff       (20)      141 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/candles_feed/binance_spot_candles/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7262 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/candles_feed/binance_spot_candles/binance_spot_candles.py
--rw-r--r--   0 madcatz    (501) staff       (20)      900 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/candles_feed/binance_spot_candles/constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)     8895 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/candles_feed/candles_base.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2746 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/candles_feed/candles_factory.py
--rw-r--r--   0 madcatz    (501) staff       (20)      539 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/candles_feed/data_types.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.264282 hummingbot-20240527/hummingbot/data_feed/candles_feed/gate_io_perpetual_candles/
--rw-r--r--   0 madcatz    (501) staff       (20)      159 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/candles_feed/gate_io_perpetual_candles/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1187 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/candles_feed/gate_io_perpetual_candles/constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)     9004 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/candles_feed/gate_io_perpetual_candles/gate_io_perpetual_candles.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.265373 hummingbot-20240527/hummingbot/data_feed/candles_feed/gate_io_spot_candles/
--rw-r--r--   0 madcatz    (501) staff       (20)      139 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/candles_feed/gate_io_spot_candles/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      985 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/candles_feed/gate_io_spot_candles/constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7884 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/candles_feed/gate_io_spot_candles/gate_io_spot_candles.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.266452 hummingbot-20240527/hummingbot/data_feed/candles_feed/kraken_spot_candles/
--rw-r--r--   0 madcatz    (501) staff       (20)      137 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/candles_feed/kraken_spot_candles/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1046 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/candles_feed/kraken_spot_candles/constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    10243 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/candles_feed/kraken_spot_candles/kraken_spot_candles.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.268250 hummingbot-20240527/hummingbot/data_feed/candles_feed/kucoin_spot_candles/
--rw-r--r--   0 madcatz    (501) staff       (20)      137 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/candles_feed/kucoin_spot_candles/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      816 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/candles_feed/kucoin_spot_candles/constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)     9411 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/candles_feed/kucoin_spot_candles/kucoin_spot_candles.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.269278 hummingbot-20240527/hummingbot/data_feed/candles_feed/okx_perpetual_candles/
--rw-r--r--   0 madcatz    (501) staff       (20)      145 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/candles_feed/okx_perpetual_candles/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1387 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/candles_feed/okx_perpetual_candles/constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)     8700 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/candles_feed/okx_perpetual_candles/okx_perpetual_candles.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.270213 hummingbot-20240527/hummingbot/data_feed/candles_feed/okx_spot_candles/
--rw-r--r--   0 madcatz    (501) staff       (20)      125 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/candles_feed/okx_spot_candles/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1387 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/candles_feed/okx_spot_candles/constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)     8670 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/candles_feed/okx_spot_candles/okx_spot_candles.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.271679 hummingbot-20240527/hummingbot/data_feed/coin_cap_data_feed/
--rw-r--r--   0 madcatz    (501) staff       (20)      118 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/coin_cap_data_feed/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1075 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/coin_cap_data_feed/coin_cap_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6923 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/coin_cap_data_feed/coin_cap_data_feed.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.272848 hummingbot-20240527/hummingbot/data_feed/coin_gecko_data_feed/
--rw-r--r--   0 madcatz    (501) staff       (20)      126 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/coin_gecko_data_feed/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      602 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/coin_gecko_data_feed/coin_gecko_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5803 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/coin_gecko_data_feed/coin_gecko_data_feed.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3226 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/custom_api_data_feed.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2466 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/data_feed_base.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.273996 hummingbot-20240527/hummingbot/data_feed/liquidations_feed/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/liquidations_feed/__init__.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.274936 hummingbot-20240527/hummingbot/data_feed/liquidations_feed/binance/
--rw-r--r--   0 madcatz    (501) staff       (20)      153 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/liquidations_feed/binance/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7604 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/liquidations_feed/binance/binance_liquidations.py
--rw-r--r--   0 madcatz    (501) staff       (20)      567 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/liquidations_feed/binance/constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)     8828 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/liquidations_feed/liquidations_base.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2550 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/liquidations_feed/liquidations_factory.py
--rw-r--r--   0 madcatz    (501) staff       (20)     9688 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/market_data_provider.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3909 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/data_feed/wallet_tracker_data_feed.py
--rw-r--r--   0 madcatz    (501) staff       (20)      766 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/exceptions.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.276800 hummingbot-20240527/hummingbot/logger/
--rw-r--r--   0 madcatz    (501) staff       (20)      755 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/logger/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      586 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/logger/application_warning.py
--rw-r--r--   0 madcatz    (501) staff       (20)      668 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/logger/cli_handler.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4260 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/logger/log_server_client.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3785 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/logger/logger.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1234 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/logger/struct_logger.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.281777 hummingbot-20240527/hummingbot/model/
--rw-r--r--   0 madcatz    (501) staff       (20)      566 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/model/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      487 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/model/controllers.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.282798 hummingbot-20240527/hummingbot/model/db_migration/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/model/db_migration/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1877 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/model/db_migration/base_transformation.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2992 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/model/db_migration/migrator.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6482 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/model/db_migration/transformations.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1267 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/model/decimal_type_decorator.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2377 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/model/executors.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2961 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/model/funding_payment.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2005 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/model/inventory_cost.py
--rw-r--r--   0 madcatz    (501) staff       (20)      888 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/model/market_data.py
--rw-r--r--   0 madcatz    (501) staff       (20)      821 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/model/market_state.py
--rw-r--r--   0 madcatz    (501) staff       (20)      365 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/model/metadata.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3109 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/model/order.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1203 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/model/order_status.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1148 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/model/range_position_collected_fees.py
--rw-r--r--   0 madcatz    (501) staff       (20)      967 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/model/range_position_update.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5796 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/model/sql_connection_manager.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7084 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/model/trade_fill.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1100 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/model/transaction_base.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.283529 hummingbot-20240527/hummingbot/notifier/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/notifier/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      262 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/notifier/notifier_base.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7780 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/notifier/telegram_notifier.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.285374 hummingbot-20240527/hummingbot/pmm_script/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/pmm_script/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    10849 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/pmm_script/pmm_script_base.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5675 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/pmm_script/pmm_script_interface.py
--rw-r--r--   0 madcatz    (501) staff       (20)   724923 2024-05-30 17:49:46.000000 hummingbot-20240527/hummingbot/pmm_script/pmm_script_iterator.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     1441 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/pmm_script/pmm_script_process.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.287279 hummingbot-20240527/hummingbot/remote_iface/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/remote_iface/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3855 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/remote_iface/messages.py
--rw-r--r--   0 madcatz    (501) staff       (20)    45513 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/remote_iface/mqtt.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.306478 hummingbot-20240527/hummingbot/strategy/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/__init__.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.307099 hummingbot-20240527/hummingbot/strategy/__utils__/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/__utils__/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)  1261421 2024-05-30 17:49:47.000000 hummingbot-20240527/hummingbot/strategy/__utils__/ring_buffer.cpp
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.309840 hummingbot-20240527/hummingbot/strategy/__utils__/trailing_indicators/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/__utils__/trailing_indicators/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2136 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/__utils__/trailing_indicators/base_trailing_indicator.py
--rw-r--r--   0 madcatz    (501) staff       (20)      717 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/__utils__/trailing_indicators/exponential_moving_average.py
--rw-r--r--   0 madcatz    (501) staff       (20)      734 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/__utils__/trailing_indicators/historical_volatility.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1141 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/__utils__/trailing_indicators/instant_volatility.py
--rw-r--r--   0 madcatz    (501) staff       (20)   816262 2024-05-30 17:49:46.000000 hummingbot-20240527/hummingbot/strategy/__utils__/trailing_indicators/trading_intensity.cpp
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.312904 hummingbot-20240527/hummingbot/strategy/amm_arb/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/amm_arb/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    26897 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/amm_arb/amm_arb.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6279 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/amm_arb/amm_arb_config_map.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7350 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/amm_arb/data_types.py
--rw-r--r--   0 madcatz    (501) staff       (20)   338533 2024-05-30 17:49:46.000000 hummingbot-20240527/hummingbot/strategy/amm_arb/dummy.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     4476 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/amm_arb/start.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2327 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/amm_arb/utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.314078 hummingbot-20240527/hummingbot/strategy/amm_v3_lp/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/amm_v3_lp/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     9882 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/amm_v3_lp/amm_v3_lp.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3293 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/amm_v3_lp/amm_v3_lp_config_map.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1052 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/amm_v3_lp/start.py
--rw-r--r--   0 madcatz    (501) staff       (20)   549973 2024-05-30 17:49:47.000000 hummingbot-20240527/hummingbot/strategy/api_asset_price_delegate.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)   381512 2024-05-30 17:49:46.000000 hummingbot-20240527/hummingbot/strategy/asset_price_delegate.cpp
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.321196 hummingbot-20240527/hummingbot/strategy/avellaneda_market_making/
--rw-r--r--   0 madcatz    (501) staff       (20)      142 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/avellaneda_market_making/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)  2721645 2024-05-30 17:49:47.000000 hummingbot-20240527/hummingbot/strategy/avellaneda_market_making/avellaneda_market_making.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)    17210 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/avellaneda_market_making/avellaneda_market_making_config_map_pydantic.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1767 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/avellaneda_market_making/start.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5368 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/conditional_execution_state.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.328603 hummingbot-20240527/hummingbot/strategy/cross_exchange_market_making/
--rw-r--r--   0 madcatz    (501) staff       (20)      234 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/cross_exchange_market_making/__init__.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)    90840 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/cross_exchange_market_making/cross_exchange_market_making.py
--rw-r--r--   0 madcatz    (501) staff       (20)    20395 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/cross_exchange_market_making/cross_exchange_market_making_config_map_pydantic.py
--rw-r--r--   0 madcatz    (501) staff       (20)   593721 2024-05-30 17:49:47.000000 hummingbot-20240527/hummingbot/strategy/cross_exchange_market_making/order_id_market_pair_tracker.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     3149 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/cross_exchange_market_making/start.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.334084 hummingbot-20240527/hummingbot/strategy/cross_exchange_mining/
--rw-r--r--   0 madcatz    (501) staff       (20)      204 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/cross_exchange_mining/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)  1449409 2024-05-30 17:49:47.000000 hummingbot-20240527/hummingbot/strategy/cross_exchange_mining/cross_exchange_mining.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     5145 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/cross_exchange_mining/cross_exchange_mining_config_map_pydantic.py
--rw-r--r--   0 madcatz    (501) staff       (20)      548 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/cross_exchange_mining/cross_exchange_mining_pair.py
--rw-r--r--   0 madcatz    (501) staff       (20)   528526 2024-05-30 17:49:47.000000 hummingbot-20240527/hummingbot/strategy/cross_exchange_mining/order_id_market_pair_tracker.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     2547 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/cross_exchange_mining/start.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2166 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/data_types.py
--rw-r--r--   0 madcatz    (501) staff       (20)    15084 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/directional_strategy_base.py
--rw-r--r--   0 madcatz    (501) staff       (20)    17966 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/hanging_orders_tracker.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.336442 hummingbot-20240527/hummingbot/strategy/hedge/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/hedge/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    29916 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/hedge/hedge.py
--rw-r--r--   0 madcatz    (501) staff       (20)    10953 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/hedge/hedge_config_map_pydantic.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1772 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/hedge/start.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.339248 hummingbot-20240527/hummingbot/strategy/liquidity_mining/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/liquidity_mining/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      948 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/liquidity_mining/data_types.py
--rw-r--r--   0 madcatz    (501) staff       (20)   339646 2024-05-30 17:49:47.000000 hummingbot-20240527/hummingbot/strategy/liquidity_mining/dummy.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)    28111 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/liquidity_mining/liquidity_mining.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7282 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/liquidity_mining/liquidity_mining_config_map.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2671 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/liquidity_mining/start.py
--rw-r--r--   0 madcatz    (501) staff       (20)      524 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/maker_taker_market_pair.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2033 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/market_trading_pair_tuple.py
--rw-r--r--   0 madcatz    (501) staff       (20)   550837 2024-05-30 17:49:47.000000 hummingbot-20240527/hummingbot/strategy/order_book_asset_price_delegate.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)   846938 2024-05-30 17:49:47.000000 hummingbot-20240527/hummingbot/strategy/order_tracker.cpp
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.343217 hummingbot-20240527/hummingbot/strategy/perpetual_market_making/
--rw-r--r--   0 madcatz    (501) staff       (20)      139 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/perpetual_market_making/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1407 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/perpetual_market_making/data_types.py
--rw-r--r--   0 madcatz    (501) staff       (20)   340444 2024-05-30 17:49:47.000000 hummingbot-20240527/hummingbot/strategy/perpetual_market_making/dummy.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)    48666 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/perpetual_market_making/perpetual_market_making.py
--rw-r--r--   0 madcatz    (501) staff       (20)    15708 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/perpetual_market_making/perpetual_market_making_config_map.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1452 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/perpetual_market_making/perpetual_market_making_order_tracker.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5933 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/perpetual_market_making/start.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.352232 hummingbot-20240527/hummingbot/strategy/pure_market_making/
--rw-r--r--   0 madcatz    (501) staff       (20)      226 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/pure_market_making/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1407 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/pure_market_making/data_types.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3288 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/pure_market_making/inventory_cost_price_delegate.py
--rw-r--r--   0 madcatz    (501) staff       (20)   331772 2024-05-30 17:49:47.000000 hummingbot-20240527/hummingbot/strategy/pure_market_making/inventory_skew_calculator.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     2801 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/pure_market_making/moving_price_band.py
--rw-r--r--   0 madcatz    (501) staff       (20)  2526417 2024-05-30 17:49:48.000000 hummingbot-20240527/hummingbot/strategy/pure_market_making/pure_market_making.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)    22271 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/pure_market_making/pure_market_making_config_map.py
--rw-r--r--   0 madcatz    (501) staff       (20)   414399 2024-05-30 17:49:47.000000 hummingbot-20240527/hummingbot/strategy/pure_market_making/pure_market_making_order_tracker.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     8774 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/pure_market_making/start.py
--rw-r--r--   0 madcatz    (501) staff       (20)    10449 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/script_strategy_base.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.357923 hummingbot-20240527/hummingbot/strategy/spot_perpetual_arbitrage/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/spot_perpetual_arbitrage/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2620 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/spot_perpetual_arbitrage/arb_proposal.py
--rw-r--r--   0 madcatz    (501) staff       (20)   340558 2024-05-30 17:49:47.000000 hummingbot-20240527/hummingbot/strategy/spot_perpetual_arbitrage/dummy.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)    26556 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/spot_perpetual_arbitrage/spot_perpetual_arbitrage.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5762 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/spot_perpetual_arbitrage/spot_perpetual_arbitrage_config_map.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2592 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/spot_perpetual_arbitrage/start.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1942 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/spot_perpetual_arbitrage/utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)  2398768 2024-05-30 17:49:47.000000 hummingbot-20240527/hummingbot/strategy/strategy_base.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)   620855 2024-05-30 17:49:47.000000 hummingbot-20240527/hummingbot/strategy/strategy_py_base.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)    20411 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/strategy_v2_base.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.360477 hummingbot-20240527/hummingbot/strategy/twap/
--rw-r--r--   0 madcatz    (501) staff       (20)       97 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/twap/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)   338167 2024-05-30 17:49:47.000000 hummingbot-20240527/hummingbot/strategy/twap/dummy.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     3468 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/twap/start.py
--rw-r--r--   0 madcatz    (501) staff       (20)    18542 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/twap/twap.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7079 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/twap/twap_config_map.py
--rw-r--r--   0 madcatz    (501) staff       (20)      700 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy/utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.360972 hummingbot-20240527/hummingbot/strategy_v2/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/__init__.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.362869 hummingbot-20240527/hummingbot/strategy_v2/backtesting/
--rw-r--r--   0 madcatz    (501) staff       (20)      474 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/backtesting/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3378 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/backtesting/backtesting_data_provider.py
--rw-r--r--   0 madcatz    (501) staff       (20)    16829 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/backtesting/backtesting_engine_base.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.363684 hummingbot-20240527/hummingbot/strategy_v2/backtesting/controllers_backtesting/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/backtesting/controllers_backtesting/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      294 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/backtesting/controllers_backtesting/directional_trading_backtesting.py
--rw-r--r--   0 madcatz    (501) staff       (20)      440 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/backtesting/controllers_backtesting/market_making_backtesting.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3591 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/backtesting/executor_simulator_base.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.364435 hummingbot-20240527/hummingbot/strategy_v2/backtesting/executors_simulator/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/backtesting/executors_simulator/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7060 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/backtesting/executors_simulator/dca_executor_simulator.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3758 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/backtesting/executors_simulator/position_executor_simulator.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.365790 hummingbot-20240527/hummingbot/strategy_v2/controllers/
--rw-r--r--   0 madcatz    (501) staff       (20)      645 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/controllers/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     8401 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/controllers/controller_base.py
--rw-r--r--   0 madcatz    (501) staff       (20)    10241 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/controllers/directional_trading_controller_base.py
--rw-r--r--   0 madcatz    (501) staff       (20)    15922 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/controllers/market_making_controller_base.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.367151 hummingbot-20240527/hummingbot/strategy_v2/executors/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/executors/__init__.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.368147 hummingbot-20240527/hummingbot/strategy_v2/executors/arbitrage_executor/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/executors/arbitrage_executor/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    12599 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/executors/arbitrage_executor/arbitrage_executor.py
--rw-r--r--   0 madcatz    (501) staff       (20)      492 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/executors/arbitrage_executor/data_types.py
--rw-r--r--   0 madcatz    (501) staff       (20)      834 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/executors/data_types.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.369021 hummingbot-20240527/hummingbot/strategy_v2/executors/dca_executor/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/executors/dca_executor/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      876 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/executors/dca_executor/data_types.py
--rw-r--r--   0 madcatz    (501) staff       (20)    25744 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/executors/dca_executor/dca_executor.py
--rw-r--r--   0 madcatz    (501) staff       (20)    15360 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/executors/executor_base.py
--rw-r--r--   0 madcatz    (501) staff       (20)    10331 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/executors/executor_orchestrator.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.369892 hummingbot-20240527/hummingbot/strategy_v2/executors/position_executor/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/executors/position_executor/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2172 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/executors/position_executor/data_types.py
--rw-r--r--   0 madcatz    (501) staff       (20)    30954 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/executors/position_executor/position_executor.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.370817 hummingbot-20240527/hummingbot/strategy_v2/executors/twap_executor/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/executors/twap_executor/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1460 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/executors/twap_executor/data_types.py
--rw-r--r--   0 madcatz    (501) staff       (20)    13720 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/executors/twap_executor/twap_executor.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.371662 hummingbot-20240527/hummingbot/strategy_v2/executors/xemm_executor/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/executors/xemm_executor/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      464 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/executors/xemm_executor/data_types.py
--rw-r--r--   0 madcatz    (501) staff       (20)    16859 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/executors/xemm_executor/xemm_executor.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.373154 hummingbot-20240527/hummingbot/strategy_v2/models/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/models/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      129 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/models/base.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1113 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/models/executor_actions.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1504 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/models/executors.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2639 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/models/executors_info.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3099 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/runnable_base.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.374668 hummingbot-20240527/hummingbot/strategy_v2/utils/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/utils/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      312 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/utils/common.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1809 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/utils/config_encoder_decoder.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4419 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/utils/distributions.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4738 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/strategy_v2/utils/order_level_builder.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.377671 hummingbot-20240527/hummingbot/templates/
--rw-r--r--   0 madcatz    (501) staff       (20)     1898 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/templates/conf_amm_arb_strategy_TEMPLATE.yml
--rw-r--r--   0 madcatz    (501) staff       (20)      536 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/templates/conf_amm_v3_lp_strategy_TEMPLATE.yml
--rw-r--r--   0 madcatz    (501) staff       (20)     5439 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/templates/conf_fee_overrides_TEMPLATE.yml
--rw-r--r--   0 madcatz    (501) staff       (20)     2001 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/templates/conf_liquidity_mining_strategy_TEMPLATE.yml
--rw-r--r--   0 madcatz    (501) staff       (20)     4032 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/templates/conf_perpetual_market_making_strategy_TEMPLATE.yml
--rw-r--r--   0 madcatz    (501) staff       (20)     5161 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/templates/conf_pure_market_making_strategy_TEMPLATE.yml
--rw-r--r--   0 madcatz    (501) staff       (20)     1569 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/templates/conf_spot_perpetual_arbitrage_strategy_TEMPLATE.yml
--rw-r--r--   0 madcatz    (501) staff       (20)     1344 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/templates/conf_twap_strategy_TEMPLATE.yml
--rwxr-xr-x   0 madcatz    (501) staff       (20)     2159 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/templates/hummingbot_logs_TEMPLATE.yml
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.378184 hummingbot-20240527/hummingbot/user/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/user/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     8061 2024-05-30 17:40:42.000000 hummingbot-20240527/hummingbot/user/user_balances.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.380385 hummingbot-20240527/hummingbot.egg-info/
--rw-r--r--   0 madcatz    (501) staff       (20)     1771 2024-05-30 17:49:48.000000 hummingbot-20240527/hummingbot.egg-info/PKG-INFO
--rw-r--r--   0 madcatz    (501) staff       (20)    48151 2024-05-30 17:49:48.000000 hummingbot-20240527/hummingbot.egg-info/SOURCES.txt
--rw-r--r--   0 madcatz    (501) staff       (20)        1 2024-05-30 17:49:48.000000 hummingbot-20240527/hummingbot.egg-info/dependency_links.txt
--rw-r--r--   0 madcatz    (501) staff       (20)      622 2024-05-30 17:49:48.000000 hummingbot-20240527/hummingbot.egg-info/requires.txt
--rw-r--r--   0 madcatz    (501) staff       (20)       11 2024-05-30 17:49:48.000000 hummingbot-20240527/hummingbot.egg-info/top_level.txt
--rw-r--r--   0 madcatz    (501) staff       (20)      491 2024-05-30 17:40:42.000000 hummingbot-20240527/pyproject.toml
--rw-r--r--   0 madcatz    (501) staff       (20)       85 2024-05-30 17:49:49.381332 hummingbot-20240527/setup.cfg
--rw-r--r--   0 madcatz    (501) staff       (20)     4356 2024-05-30 17:40:42.000000 hummingbot-20240527/setup.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 17:49:49.379891 hummingbot-20240527/test/
--rw-r--r--   0 madcatz    (501) staff       (20)     6190 2024-05-30 17:40:42.000000 hummingbot-20240527/test/test_isolated_asyncio_wrapper_test_case.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3267 2024-05-30 17:40:42.000000 hummingbot-20240527/test/test_local_class_event_loop_wrapper_test_case.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3504 2024-05-30 17:40:42.000000 hummingbot-20240527/test/test_local_test_event_loop_wrapper_test_case.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5466 2024-05-30 17:40:42.000000 hummingbot-20240527/test/test_logger_mixin_for_test.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.714586 hummingbot-20240530/
+-rw-r--r--   0 madcatz    (501) staff       (20)    11352 2024-05-30 19:45:41.000000 hummingbot-20240530/LICENSE
+-rw-r--r--   0 madcatz    (501) staff       (20)     1771 2024-05-30 19:52:28.714500 hummingbot-20240530/PKG-INFO
+-rw-r--r--   0 madcatz    (501) staff       (20)     9670 2024-05-30 19:45:41.000000 hummingbot-20240530/README.md
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.276970 hummingbot-20240530/bin/
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     6821 2024-05-30 19:45:41.000000 hummingbot-20240530/bin/hummingbot_quickstart.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.278671 hummingbot-20240530/hummingbot/
+-rw-r--r--   0 madcatz    (501) staff       (20)        6 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/VERSION
+-rw-r--r--   0 madcatz    (501) staff       (20)     5811 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/__init__.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.284807 hummingbot-20240530/hummingbot/client/
+-rw-r--r--   0 madcatz    (501) staff       (20)      655 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/__init__.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.296338 hummingbot-20240530/hummingbot/client/command/
+-rw-r--r--   0 madcatz    (501) staff       (20)     1249 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/command/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     9967 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/command/balance_command.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    22563 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/command/config_command.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6908 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/command/connect_command.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    16234 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/command/create_command.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1458 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/command/exit_command.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4844 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/command/export_command.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6371 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/command/gateway_api_manager.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    41186 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/command/gateway_command.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      916 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/command/help_command.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    12319 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/command/history_command.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3698 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/command/import_command.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4566 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/command/mqtt_command.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3001 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/command/order_book_command.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      344 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/command/pmm_script_command.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2571 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/command/previous_strategy_command.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2697 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/command/rate_command.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     9686 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/command/silly_commands.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    15078 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/command/start_command.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    10502 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/command/status_command.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2552 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/command/stop_command.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2996 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/command/ticker_command.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.303431 hummingbot-20240530/hummingbot/client/config/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/config/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    42100 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/config/client_config_map.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    18418 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/config/conf_migration.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4553 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/config/config_crypt.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2726 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/config/config_data_types.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    38116 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/config/config_helpers.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      633 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/config/config_methods.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7452 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/config/config_validators.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3189 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/config/config_var.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1404 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/config/fee_overrides_config_map.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      364 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/config/gateway_ssl_config_map.py
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/config/global_config_map.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3858 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/config/security.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6288 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/config/strategy_config_data_types.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3003 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/config/trade_fee_schema_loader.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.303934 hummingbot-20240530/hummingbot/client/data_type/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/data_type/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      426 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/data_type/currency_amount.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    15273 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/hummingbot_application.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    13787 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/performance.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      516 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/platform.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    27252 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/settings.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.307358 hummingbot-20240530/hummingbot/client/tab/
+-rw-r--r--   0 madcatz    (501) staff       (20)      135 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/tab/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      872 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/tab/data_types.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3140 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/tab/order_book_tab.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1723 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/tab/tab_base.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      774 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/tab/tab_example_tab.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.312481 hummingbot-20240530/hummingbot/client/ui/
+-rw-r--r--   0 madcatz    (501) staff       (20)     8435 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/ui/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    24695 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/ui/completer.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     9614 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/ui/custom_widgets.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    11623 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/ui/hummingbot_cli.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4952 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/ui/interface_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3593 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/ui/keybindings.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    11632 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/ui/layout.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    11856 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/ui/parser.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1710 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/ui/scroll_handlers.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2524 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/ui/stdout_redirection.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    11314 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/client/ui/style.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.332349 hummingbot-20240530/hummingbot/connector/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7400 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/budget_checker.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    18938 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/client_order_tracker.py
+-rw-r--r--   0 madcatz    (501) staff       (20)  1403631 2024-05-30 19:52:24.000000 hummingbot-20240530/hummingbot/connector/connector_base.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     6375 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/connector_metrics_collector.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      215 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/constants.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.334388 hummingbot-20240530/hummingbot/connector/derivative/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/__init__.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.339000 hummingbot-20240530/hummingbot/connector/derivative/binance_perpetual/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/binance_perpetual/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     9683 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1944 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6016 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    38371 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_derivative.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6334 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2428 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4013 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_web_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   341295 2024-05-30 19:52:24.000000 hummingbot-20240530/hummingbot/connector/derivative/binance_perpetual/dummy.cpp
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.343475 hummingbot-20240530/hummingbot/connector/derivative/bit_com_perpetual/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/bit_com_perpetual/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    10413 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3497 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4597 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    35998 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_derivative.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5494 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2420 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2670 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_web_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   341295 2024-05-30 19:52:24.000000 hummingbot-20240530/hummingbot/connector/derivative/bit_com_perpetual/dummy.cpp
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.348459 hummingbot-20240530/hummingbot/connector/derivative/bitget_perpetual/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/bitget_perpetual/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    12125 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2898 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5025 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    40405 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_derivative.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5830 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2002 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3142 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_web_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.352595 hummingbot-20240530/hummingbot/connector/derivative/bybit_perpetual/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/bybit_perpetual/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    15468 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3238 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5848 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    38897 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_derivative.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6821 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4168 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    19340 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_web_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   341067 2024-05-30 19:52:24.000000 hummingbot-20240530/hummingbot/connector/derivative/bybit_perpetual/dummy.cpp
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.356329 hummingbot-20240530/hummingbot/connector/derivative/dydx_perpetual/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/dydx_perpetual/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    12544 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4454 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3774 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    40418 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_derivative.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2566 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2154 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2663 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_web_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.365527 hummingbot-20240530/hummingbot/connector/derivative/gate_io_perpetual/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/gate_io_perpetual/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   341295 2024-05-30 19:52:24.000000 hummingbot-20240530/hummingbot/connector/derivative/gate_io_perpetual/dummy.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)    10758 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3135 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5254 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    34398 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_derivative.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4492 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1634 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1851 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_web_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.371410 hummingbot-20240530/hummingbot/connector/derivative/hyperliquid_perpetual/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/hyperliquid_perpetual/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   341751 2024-05-30 19:52:24.000000 hummingbot-20240530/hummingbot/connector/derivative/hyperliquid_perpetual/dummy.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)    10842 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6022 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3695 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    36109 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_derivative.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5656 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4106 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5213 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_web_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.373630 hummingbot-20240530/hummingbot/connector/derivative/injective_v2_perpetual/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/injective_v2_perpetual/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      466 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/injective_v2_perpetual/injective_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4840 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/injective_v2_perpetual/injective_v2_perpetual_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    48511 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/injective_v2_perpetual/injective_v2_perpetual_derivative.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3981 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/injective_v2_perpetual/injective_v2_perpetual_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      410 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/injective_v2_perpetual/injective_v2_perpetual_web_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.378118 hummingbot-20240530/hummingbot/connector/derivative/kucoin_perpetual/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/kucoin_perpetual/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   341181 2024-05-30 19:52:24.000000 hummingbot-20240530/hummingbot/connector/derivative/kucoin_perpetual/dummy.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)    14498 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     8026 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_api_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6301 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6066 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    45173 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_derivative.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2117 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6479 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_web_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.381579 hummingbot-20240530/hummingbot/connector/derivative/okx_perpetual/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/okx_perpetual/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    20796 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5462 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6000 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    39008 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_derivative.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6527 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2707 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    12961 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_web_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1421 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/perpetual_budget_checker.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.384680 hummingbot-20240530/hummingbot/connector/derivative/phemex_perpetual/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/phemex_perpetual/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    12075 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5017 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_api_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2335 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6113 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    32650 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_derivative.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2679 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3838 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_web_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2238 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/position.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.387689 hummingbot-20240530/hummingbot/connector/derivative/vega_perpetual/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/vega_perpetual/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    14929 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3977 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     9352 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1466 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_data.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    66373 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_derivative.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6581 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2481 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6529 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_web_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2528 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/derivative_base.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.387981 hummingbot-20240530/hummingbot/connector/exchange/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/__init__.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.391310 hummingbot-20240530/hummingbot/connector/exchange/ascend_ex/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/ascend_ex/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7240 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/ascend_ex/ascend_ex_api_order_book_data_source.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     3627 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/ascend_ex/ascend_ex_api_user_stream_data_source.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     2478 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/ascend_ex/ascend_ex_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5036 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/ascend_ex/ascend_ex_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    26170 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/ascend_ex/ascend_ex_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2084 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/ascend_ex/ascend_ex_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2719 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/ascend_ex/ascend_ex_web_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.395427 hummingbot-20240530/hummingbot/connector/exchange/binance/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/binance/__init__.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     6402 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/binance/binance_api_order_book_data_source.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     6081 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/binance/binance_api_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2413 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/binance/binance_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4688 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/binance/binance_constants.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)    25993 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/binance/binance_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3224 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/binance/binance_order_book.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2972 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/binance/binance_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3154 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/binance/binance_web_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   339765 2024-05-30 19:52:24.000000 hummingbot-20240530/hummingbot/connector/exchange/binance/dummy.cpp
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.414314 hummingbot-20240530/hummingbot/connector/exchange/bitfinex/
+-rw-r--r--   0 madcatz    (501) staff       (20)     1257 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/bitfinex/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   785720 2024-05-30 19:52:24.000000 hummingbot-20240530/hummingbot/connector/exchange/bitfinex/bitfinex_active_order_tracker.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)    22384 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/bitfinex/bitfinex_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2224 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/bitfinex/bitfinex_api_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1580 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/bitfinex/bitfinex_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)  3066713 2024-05-30 19:52:25.000000 hummingbot-20240530/hummingbot/connector/exchange/bitfinex/bitfinex_exchange.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)   554137 2024-05-30 19:52:24.000000 hummingbot-20240530/hummingbot/connector/exchange/bitfinex/bitfinex_in_flight_order.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)   576560 2024-05-30 19:52:24.000000 hummingbot-20240530/hummingbot/connector/exchange/bitfinex/bitfinex_order_book.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     1273 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/bitfinex/bitfinex_order_book_message.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    10355 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/bitfinex/bitfinex_order_book_tracker.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1057 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/bitfinex/bitfinex_order_book_tracker_entry.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2052 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/bitfinex/bitfinex_user_stream_tracker.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3928 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/bitfinex/bitfinex_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5028 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/bitfinex/bitfinex_websocket.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.418262 hummingbot-20240530/hummingbot/connector/exchange/bitmart/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/bitmart/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    10154 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/bitmart/bitmart_api_order_book_data_source.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     4787 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/bitmart/bitmart_api_user_stream_data_source.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     2913 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/bitmart/bitmart_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2473 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/bitmart/bitmart_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    19821 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/bitmart/bitmart_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2451 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/bitmart/bitmart_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2538 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/bitmart/bitmart_web_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   339765 2024-05-30 19:52:24.000000 hummingbot-20240530/hummingbot/connector/exchange/bitmart/dummy.cpp
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.422524 hummingbot-20240530/hummingbot/connector/exchange/bitrue/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/bitrue/__init__.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     8798 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/bitrue/bitrue_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2385 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/bitrue/bitrue_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6008 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/bitrue/bitrue_constants.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)    30434 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/bitrue/bitrue_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3211 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/bitrue/bitrue_order_book.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     8058 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/bitrue/bitrue_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1604 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/bitrue/bitrue_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3128 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/bitrue/bitrue_web_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.425874 hummingbot-20240530/hummingbot/connector/exchange/btc_markets/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/btc_markets/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     9564 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/btc_markets/btc_markets_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4055 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/btc_markets/btc_markets_api_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4543 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/btc_markets/btc_markets_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3114 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/btc_markets/btc_markets_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    25469 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/btc_markets/btc_markets_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4545 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/btc_markets/btc_markets_order_book.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1662 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/btc_markets/btc_markets_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2831 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/btc_markets/btc_markets_web_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.429596 hummingbot-20240530/hummingbot/connector/exchange/bybit/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/bybit/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    12169 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/bybit/bybit_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5372 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/bybit/bybit_api_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3308 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/bybit/bybit_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4659 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/bybit/bybit_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    21562 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/bybit/bybit_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4246 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/bybit/bybit_order_book.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2581 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/bybit/bybit_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5170 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/bybit/bybit_web_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   339537 2024-05-30 19:52:24.000000 hummingbot-20240530/hummingbot/connector/exchange/bybit/dummy.cpp
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.434419 hummingbot-20240530/hummingbot/connector/exchange/coinbase_advanced_trade/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/coinbase_advanced_trade/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    11069 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    13923 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_api_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    12512 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5500 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    50376 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7810 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_order_book.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2030 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7161 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_web_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   341676 2024-05-30 19:52:24.000000 hummingbot-20240530/hummingbot/connector/exchange/coinbase_advanced_trade/dummy.cpp
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.448128 hummingbot-20240530/hummingbot/connector/exchange/coinbase_pro/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/coinbase_pro/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   927886 2024-05-30 19:52:24.000000 hummingbot-20240530/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_active_order_tracker.cpp
+-rwxr-xr-x   0 madcatz    (501) staff       (20)    14517 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_api_order_book_data_source.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     5006 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_api_user_stream_data_source.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     2753 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      493 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)  2596602 2024-05-30 19:52:25.000000 hummingbot-20240530/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_exchange.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)   499653 2024-05-30 19:52:24.000000 hummingbot-20240530/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_in_flight_order.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)   535437 2024-05-30 19:52:25.000000 hummingbot-20240530/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_order_book.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     1816 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_order_book_message.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     8848 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_order_book_tracker.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1041 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_order_book_tracker_entry.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2361 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_user_stream_tracker.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2530 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.453078 hummingbot-20240530/hummingbot/connector/exchange/cube/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/cube/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    11507 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/cube/cube_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3570 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/cube/cube_api_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3643 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/cube/cube_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3371 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/cube/cube_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    52528 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/cube/cube_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4473 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/cube/cube_order_book.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4547 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/cube/cube_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1660 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/cube/cube_web_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.460185 hummingbot-20240530/hummingbot/connector/exchange/cube/cube_ws_protobufs/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/cube/cube_ws_protobufs/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    10219 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/cube/cube_ws_protobufs/market_data_pb2.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    15363 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/cube/cube_ws_protobufs/market_data_pb2.pyi
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/cube/cube_ws_protobufs/py.typed
+-rw-r--r--   0 madcatz    (501) staff       (20)    15992 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/cube/cube_ws_protobufs/trade_pb2.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    29121 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/cube/cube_ws_protobufs/trade_pb2.pyi
+-rw-r--r--   0 madcatz    (501) staff       (20)   339423 2024-05-30 19:52:24.000000 hummingbot-20240530/hummingbot/connector/exchange/cube/dummy.cpp
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.465100 hummingbot-20240530/hummingbot/connector/exchange/foxbit/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/foxbit/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    10078 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/foxbit/foxbit_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5190 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/foxbit/foxbit_api_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3912 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/foxbit/foxbit_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   345010 2024-05-30 19:52:24.000000 hummingbot-20240530/hummingbot/connector/exchange/foxbit/foxbit_connector.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     5253 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/foxbit/foxbit_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    44815 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/foxbit/foxbit_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7671 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/foxbit/foxbit_order_book.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5090 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/foxbit/foxbit_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4155 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/foxbit/foxbit_web_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.468337 hummingbot-20240530/hummingbot/connector/exchange/gate_io/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/gate_io/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7620 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/gate_io/gate_io_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4310 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/gate_io/gate_io_api_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3166 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/gate_io/gate_io_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3528 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/gate_io/gate_io_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    22712 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/gate_io/gate_io_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1255 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/gate_io/gate_io_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1834 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/gate_io/gate_io_web_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   341880 2024-05-30 19:52:25.000000 hummingbot-20240530/hummingbot/connector/exchange/gate_io/placeholder.cpp
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.476059 hummingbot-20240530/hummingbot/connector/exchange/hitbtc/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/hitbtc/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   754445 2024-05-30 19:52:25.000000 hummingbot-20240530/hummingbot/connector/exchange/hitbtc/hitbtc_active_order_tracker.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)    11733 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/hitbtc/hitbtc_api_order_book_data_source.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     3224 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/hitbtc/hitbtc_api_user_stream_data_source.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     2451 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/hitbtc/hitbtc_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1847 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/hitbtc/hitbtc_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    42970 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/hitbtc/hitbtc_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3162 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/hitbtc/hitbtc_in_flight_order.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3455 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/hitbtc/hitbtc_order_book.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2397 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/hitbtc/hitbtc_order_book_message.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5637 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/hitbtc/hitbtc_order_book_tracker.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      945 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/hitbtc/hitbtc_order_book_tracker_entry.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2346 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/hitbtc/hitbtc_user_stream_tracker.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5706 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/hitbtc/hitbtc_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4686 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/hitbtc/hitbtc_websocket.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.479312 hummingbot-20240530/hummingbot/connector/exchange/htx/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/htx/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     8241 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/htx/htx_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5047 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/htx/htx_api_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3477 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/htx/htx_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2958 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/htx/htx_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    18960 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/htx/htx_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1589 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/htx/htx_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2553 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/htx/htx_web_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.483307 hummingbot-20240530/hummingbot/connector/exchange/injective_v2/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/injective_v2/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4257 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/injective_v2/account_delegation_script.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.486427 hummingbot-20240530/hummingbot/connector/exchange/injective_v2/data_sources/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/injective_v2/data_sources/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    71837 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/injective_v2/data_sources/injective_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    23529 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/injective_v2/data_sources/injective_grantee_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    12854 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/injective_v2/data_sources/injective_read_only_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    24074 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/injective_v2/data_sources/injective_vaults_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5962 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/injective_v2/injective_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)       90 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/injective_v2/injective_events.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4376 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/injective_v2/injective_market.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    14999 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/injective_v2/injective_query_executor.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3669 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/injective_v2/injective_v2_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    42627 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/injective_v2/injective_v2_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    15808 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/injective_v2/injective_v2_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      410 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/injective_v2/injective_v2_web_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.489948 hummingbot-20240530/hummingbot/connector/exchange/kraken/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/kraken/__init__.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     7715 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/kraken/kraken_api_order_book_data_source.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     3909 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/kraken/kraken_api_user_stream_data_source.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     2929 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/kraken/kraken_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4146 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/kraken/kraken_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    27389 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/kraken/kraken_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2903 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/kraken/kraken_order_book.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     8041 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/kraken/kraken_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1660 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/kraken/kraken_web_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.494067 hummingbot-20240530/hummingbot/connector/exchange/kucoin/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/kucoin/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   339651 2024-05-30 19:52:25.000000 hummingbot-20240530/hummingbot/connector/exchange/kucoin/dummy.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     8742 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/kucoin/kucoin_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4879 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/kucoin/kucoin_api_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3663 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/kucoin/kucoin_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3297 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/kucoin/kucoin_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    24398 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/kucoin/kucoin_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2132 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/kucoin/kucoin_order_book_message.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3049 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/kucoin/kucoin_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3215 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/kucoin/kucoin_web_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.497525 hummingbot-20240530/hummingbot/connector/exchange/mexc/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/mexc/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   339423 2024-05-30 19:52:25.000000 hummingbot-20240530/hummingbot/connector/exchange/mexc/dummy.cpp
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     6556 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/mexc/mexc_api_order_book_data_source.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     8131 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/mexc/mexc_api_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2480 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/mexc/mexc_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4344 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/mexc/mexc_constants.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)    26610 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/mexc/mexc_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3481 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/mexc/mexc_order_book.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1705 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/mexc/mexc_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3142 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/mexc/mexc_web_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.503631 hummingbot-20240530/hummingbot/connector/exchange/ndax/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/ndax/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   339423 2024-05-30 19:52:25.000000 hummingbot-20240530/hummingbot/connector/exchange/ndax/dummy.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)    15461 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/ndax/ndax_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5670 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/ndax/ndax_api_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2103 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/ndax/ndax_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5426 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/ndax/ndax_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    49594 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/ndax/ndax_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2421 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/ndax/ndax_in_flight_order.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3556 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/ndax/ndax_order_book.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3561 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/ndax/ndax_order_book_message.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5934 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/ndax/ndax_order_book_tracker.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2369 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/ndax/ndax_user_stream_tracker.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4179 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/ndax/ndax_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3928 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/ndax/ndax_websocket_adaptor.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.506208 hummingbot-20240530/hummingbot/connector/exchange/okx/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/okx/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     9214 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/okx/okx_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4432 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/okx/okx_api_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3330 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/okx/okx_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2775 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/okx/okx_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    18614 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/okx/okx_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1761 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/okx/okx_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2723 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/okx/okx_web_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.508529 hummingbot-20240530/hummingbot/connector/exchange/paper_trade/
+-rw-r--r--   0 madcatz    (501) staff       (20)     1293 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/paper_trade/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      910 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/paper_trade/market_config.py
+-rw-r--r--   0 madcatz    (501) staff       (20)  2193488 2024-05-30 19:52:25.000000 hummingbot-20240530/hummingbot/connector/exchange/paper_trade/paper_trade_exchange.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)      126 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/paper_trade/trading_pair.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.516933 hummingbot-20240530/hummingbot/connector/exchange/polkadex/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/polkadex/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4527 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/polkadex/polkadex_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4188 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/polkadex/polkadex_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    26470 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/polkadex/polkadex_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    18334 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/polkadex/polkadex_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    19864 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/polkadex/polkadex_query_executor.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2076 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/polkadex/polkadex_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      405 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/polkadex/polkadex_web_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.522544 hummingbot-20240530/hummingbot/connector/exchange/vertex/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/vertex/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   343537 2024-05-30 19:52:25.000000 hummingbot-20240530/hummingbot/connector/exchange/vertex/dummy.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     7949 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/vertex/vertex_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5123 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/vertex/vertex_api_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3400 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/vertex/vertex_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    10086 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/vertex/vertex_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      959 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/vertex/vertex_eip712_structs.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    40072 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/vertex/vertex_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4655 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/vertex/vertex_order_book.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7773 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/vertex/vertex_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1774 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange/vertex/vertex_web_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)  1444488 2024-05-30 19:52:25.000000 hummingbot-20240530/hummingbot/connector/exchange_base.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)    45930 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/exchange_py_base.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.524025 hummingbot-20240530/hummingbot/connector/gateway/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/__init__.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.526105 hummingbot-20240530/hummingbot/connector/gateway/amm/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/amm/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    10973 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/amm/gateway_algorand_amm.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    46320 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/amm/gateway_evm_amm.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     9794 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/amm/gateway_near_amm.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5794 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/amm/gateway_tezos_amm.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.527411 hummingbot-20240530/hummingbot/connector/gateway/amm_lp/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/amm_lp/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    58500 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/amm_lp/gateway_evm_amm_lp.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4735 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/amm_lp/gateway_in_flight_lp_order.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    56750 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/amm_lp/gateway_osmosis_amm_lp.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.528021 hummingbot-20240530/hummingbot/connector/gateway/amm_perpetual/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/amm_perpetual/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    26154 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/amm_perpetual/gateway_evm_amm_perpetual.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.528856 hummingbot-20240530/hummingbot/connector/gateway/clob_perp/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/clob_perp/__init__.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.529359 hummingbot-20240530/hummingbot/connector/gateway/clob_perp/data_sources/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/clob_perp/data_sources/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1425 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/clob_perp/data_sources/clob_perp_api_data_source_base.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    21799 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/clob_perp/gateway_clob_perp.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4144 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/clob_perp/gateway_clob_perp_api_order_book_data_source.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.530092 hummingbot-20240530/hummingbot/connector/gateway/clob_spot/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/clob_spot/__init__.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.531073 hummingbot-20240530/hummingbot/connector/gateway/clob_spot/data_sources/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/clob_spot/data_sources/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7967 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/clob_spot/data_sources/clob_api_data_source_base.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.532758 hummingbot-20240530/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    29847 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/dexalot_api_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1779 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/dexalot_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3455 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/dexalot_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1296 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/dexalot_web_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    18003 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/clob_spot/data_sources/gateway_clob_api_data_source_base.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.534416 hummingbot-20240530/hummingbot/connector/gateway/clob_spot/data_sources/kujira/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/clob_spot/data_sources/kujira/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    40889 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/clob_spot/data_sources/kujira/kujira_api_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      315 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/clob_spot/data_sources/kujira/kujira_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1952 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/clob_spot/data_sources/kujira/kujira_helpers.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4659 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/clob_spot/data_sources/kujira/kujira_types.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.535671 hummingbot-20240530/hummingbot/connector/gateway/clob_spot/data_sources/xrpl/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/clob_spot/data_sources/xrpl/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    17880 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/clob_spot/data_sources/xrpl/xrpl_api_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2560 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/clob_spot/data_sources/xrpl/xrpl_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3244 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/clob_spot/gateway_clob_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    31044 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/clob_spot/gateway_clob_spot.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      944 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/common_types.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    10185 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/gateway_in_flight_order.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2230 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/gateway_order_tracker.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6890 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/gateway/gateway_price_shim.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   857765 2024-05-30 19:52:25.000000 hummingbot-20240530/hummingbot/connector/in_flight_order_base.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)    29014 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/markets_recorder.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.536095 hummingbot-20240530/hummingbot/connector/other/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/other/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6037 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/parrot.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    17636 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/perpetual_derivative_py_base.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7622 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/perpetual_trading.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.542085 hummingbot-20240530/hummingbot/connector/test_support/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/test_support/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    86233 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/test_support/exchange_connector_test.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    42837 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/test_support/gateway_clob_api_data_source_test.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1411 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/test_support/mock_order_tracker.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   813971 2024-05-30 19:52:25.000000 hummingbot-20240530/hummingbot/connector/test_support/mock_paper_exchange.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)      227 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/test_support/mock_pure_python_paper_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     8740 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/test_support/network_mocking_assistant.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    44545 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/test_support/oms_exchange_connector_test.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    33536 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/test_support/perpetual_derivative_test.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3607 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/time_synchronizer.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   531657 2024-05-30 19:52:25.000000 hummingbot-20240530/hummingbot/connector/trading_rule.cpp
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.542926 hummingbot-20240530/hummingbot/connector/utilities/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/utilities/__init__.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.545575 hummingbot-20240530/hummingbot/connector/utilities/oms_connector/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/utilities/oms_connector/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     8912 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/utilities/oms_connector/oms_connector_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3929 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/utilities/oms_connector/oms_connector_api_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2849 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/utilities/oms_connector/oms_connector_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5724 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/utilities/oms_connector/oms_connector_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    25851 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/utilities/oms_connector/oms_connector_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      641 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/utilities/oms_connector/oms_connector_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2789 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/utilities/oms_connector/oms_connector_web_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4992 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/connector/utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.548962 hummingbot-20240530/hummingbot/core/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/__init__.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.552388 hummingbot-20240530/hummingbot/core/api_throttler/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/api_throttler/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3565 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/api_throttler/async_request_context_base.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3888 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/api_throttler/async_throttler.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3875 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/api_throttler/async_throttler_base.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1789 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/api_throttler/data_types.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   699724 2024-05-30 19:52:25.000000 hummingbot-20240530/hummingbot/core/clock.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)      104 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/clock_mode.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.555622 hummingbot-20240530/hummingbot/core/cpp/
+-rw-r--r--   0 madcatz    (501) staff       (20)     4793 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/cpp/LimitOrder.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     1832 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/cpp/LimitOrder.h
+-rw-r--r--   0 madcatz    (501) staff       (20)     3183 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/cpp/OrderBookEntry.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)      991 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/cpp/OrderBookEntry.h
+-rw-r--r--   0 madcatz    (501) staff       (20)     1825 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/cpp/OrderExpirationEntry.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)      868 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/cpp/OrderExpirationEntry.h
+-rw-r--r--   0 madcatz    (501) staff       (20)      684 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/cpp/PyRef.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)      503 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/cpp/PyRef.h
+-rw-r--r--   0 madcatz    (501) staff       (20)     3086 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/cpp/TestOrderBookEntry.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)       19 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/cpp/Utils.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)      246 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/cpp/Utils.h
+-rwxr-xr-x   0 madcatz    (501) staff       (20)      139 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/cpp/compile.sh
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.574735 hummingbot-20240530/hummingbot/core/data_type/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/data_type/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      129 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/data_type/cancellation_result.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1067 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/data_type/common.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   707148 2024-05-30 19:52:25.000000 hummingbot-20240530/hummingbot/core/data_type/composite_order_book.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     2052 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/data_type/funding_info.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    14142 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/data_type/in_flight_order.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   664173 2024-05-30 19:52:25.000000 hummingbot-20240530/hummingbot/core/data_type/limit_order.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     1836 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/data_type/market_order.py
+-rw-r--r--   0 madcatz    (501) staff       (20)  1140705 2024-05-30 19:52:25.000000 hummingbot-20240530/hummingbot/core/data_type/order_book.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     2989 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/data_type/order_book_message.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   390625 2024-05-30 19:52:25.000000 hummingbot-20240530/hummingbot/core/data_type/order_book_query_result.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)      587 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/data_type/order_book_row.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    15929 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/data_type/order_book_tracker.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)    11594 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/data_type/order_book_tracker_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      776 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/data_type/order_book_tracker_entry.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    15612 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/data_type/order_candidate.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   408361 2024-05-30 19:52:25.000000 hummingbot-20240530/hummingbot/core/data_type/order_expiration_entry.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     1809 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/data_type/perpetual_api_order_book_data_source.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     5496 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/data_type/remote_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1843 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/data_type/trade.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    12881 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/data_type/trade_fee.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   371702 2024-05-30 19:52:25.000000 hummingbot-20240530/hummingbot/core/data_type/transaction_tracker.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     1310 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/data_type/user_stream_tracker.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     3994 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/data_type/user_stream_tracker_data_source.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.577459 hummingbot-20240530/hummingbot/core/event/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/event/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      754 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/event/event_forwarder.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   402941 2024-05-30 19:52:25.000000 hummingbot-20240530/hummingbot/core/event/event_listener.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)   604746 2024-05-30 19:52:26.000000 hummingbot-20240530/hummingbot/core/event/event_logger.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)   448102 2024-05-30 19:52:26.000000 hummingbot-20240530/hummingbot/core/event/event_reporter.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     8411 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/event/events.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.580863 hummingbot-20240530/hummingbot/core/gateway/
+-rw-r--r--   0 madcatz    (501) staff       (20)     5198 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/gateway/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    42014 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/gateway/gateway_http_client.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5292 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/gateway/gateway_status_monitor.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      892 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/gateway/utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.581756 hummingbot-20240530/hummingbot/core/management/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/management/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2632 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/management/console.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1325 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/management/diagnosis.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.582950 hummingbot-20240530/hummingbot/core/mock_api/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/mock_api/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2827 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/mock_api/mock_mqtt_server.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     9206 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/mock_api/mock_web_server.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     8409 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/mock_api/mock_web_socket_server.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4386 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/network_base.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   680641 2024-05-30 19:52:26.000000 hummingbot-20240530/hummingbot/core/network_iterator.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)   498964 2024-05-30 19:52:26.000000 hummingbot-20240530/hummingbot/core/pubsub.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)   331173 2024-05-30 19:52:26.000000 hummingbot-20240530/hummingbot/core/py_time_iterator.cpp
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.584340 hummingbot-20240530/hummingbot/core/rate_oracle/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/rate_oracle/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     8190 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/rate_oracle/rate_oracle.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.587612 hummingbot-20240530/hummingbot/core/rate_oracle/sources/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/rate_oracle/sources/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2207 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/rate_oracle/sources/ascend_ex_rate_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3589 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/rate_oracle/sources/binance_rate_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3624 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/rate_oracle/sources/binance_us_rate_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1386 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/rate_oracle/sources/coin_cap_rate_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7211 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/rate_oracle/sources/coin_gecko_rate_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3578 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/rate_oracle/sources/coinbase_advanced_trade_rate_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3871 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/rate_oracle/sources/cube_rate_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2800 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/rate_oracle/sources/gate_io_rate_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2349 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/rate_oracle/sources/kucoin_rate_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      605 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/rate_oracle/sources/rate_source_base.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1678 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/rate_oracle/utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   394085 2024-05-30 19:52:26.000000 hummingbot-20240530/hummingbot/core/time_iterator.cpp
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.592113 hummingbot-20240530/hummingbot/core/utils/
+-rw-r--r--   0 madcatz    (501) staff       (20)     1257 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/utils/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4470 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/utils/async_call_scheduler.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2486 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/utils/async_retry.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2031 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/utils/async_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3613 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/utils/estimate_fee.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      892 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/utils/fixed_rate_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5970 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/utils/gateway_config_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2821 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/utils/kill_switch.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      940 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/utils/market_price.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7907 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/utils/ssl_cert.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      675 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/utils/ssl_client_request.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2203 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/utils/tracking_nonce.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4187 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/utils/trading_pair_fetcher.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.594708 hummingbot-20240530/hummingbot/core/web_assistant/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/web_assistant/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      696 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/web_assistant/auth.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.595823 hummingbot-20240530/hummingbot/core/web_assistant/connections/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/web_assistant/connections/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1834 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/web_assistant/connections/connections_factory.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4371 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/web_assistant/connections/data_types.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      797 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/web_assistant/connections/rest_connection.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4767 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/web_assistant/connections/ws_connection.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5116 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/web_assistant/rest_assistant.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      467 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/web_assistant/rest_post_processors.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      460 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/web_assistant/rest_pre_processors.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2883 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/web_assistant/web_assistants_factory.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3740 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/web_assistant/ws_assistant.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      457 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/web_assistant/ws_post_processors.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      450 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/core/web_assistant/ws_pre_processors.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.597715 hummingbot-20240530/hummingbot/data_feed/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5140 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/amm_gateway_data_feed.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.598880 hummingbot-20240530/hummingbot/data_feed/candles_feed/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/candles_feed/__init__.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.599700 hummingbot-20240530/hummingbot/data_feed/candles_feed/ascend_ex_spot_candles/
+-rw-r--r--   0 madcatz    (501) staff       (20)      147 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/candles_feed/ascend_ex_spot_candles/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     8002 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/candles_feed/ascend_ex_spot_candles/ascend_ex_spot_candles.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1086 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/candles_feed/ascend_ex_spot_candles/constants.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.600635 hummingbot-20240530/hummingbot/data_feed/candles_feed/binance_perpetual_candles/
+-rw-r--r--   0 madcatz    (501) staff       (20)      170 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/candles_feed/binance_perpetual_candles/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7298 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/candles_feed/binance_perpetual_candles/binance_perpetual_candles.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      897 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/candles_feed/binance_perpetual_candles/constants.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.601414 hummingbot-20240530/hummingbot/data_feed/candles_feed/binance_spot_candles/
+-rw-r--r--   0 madcatz    (501) staff       (20)      141 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/candles_feed/binance_spot_candles/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7267 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/candles_feed/binance_spot_candles/binance_spot_candles.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      900 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/candles_feed/binance_spot_candles/constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     8894 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/candles_feed/candles_base.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2746 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/candles_feed/candles_factory.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      539 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/candles_feed/data_types.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.602157 hummingbot-20240530/hummingbot/data_feed/candles_feed/gate_io_perpetual_candles/
+-rw-r--r--   0 madcatz    (501) staff       (20)      159 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/candles_feed/gate_io_perpetual_candles/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1187 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/candles_feed/gate_io_perpetual_candles/constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     9004 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/candles_feed/gate_io_perpetual_candles/gate_io_perpetual_candles.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.603404 hummingbot-20240530/hummingbot/data_feed/candles_feed/gate_io_spot_candles/
+-rw-r--r--   0 madcatz    (501) staff       (20)      139 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/candles_feed/gate_io_spot_candles/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      985 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/candles_feed/gate_io_spot_candles/constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7884 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/candles_feed/gate_io_spot_candles/gate_io_spot_candles.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.604255 hummingbot-20240530/hummingbot/data_feed/candles_feed/kraken_spot_candles/
+-rw-r--r--   0 madcatz    (501) staff       (20)      137 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/candles_feed/kraken_spot_candles/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1046 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/candles_feed/kraken_spot_candles/constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    10243 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/candles_feed/kraken_spot_candles/kraken_spot_candles.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.605141 hummingbot-20240530/hummingbot/data_feed/candles_feed/kucoin_spot_candles/
+-rw-r--r--   0 madcatz    (501) staff       (20)      137 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/candles_feed/kucoin_spot_candles/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      816 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/candles_feed/kucoin_spot_candles/constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     9411 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/candles_feed/kucoin_spot_candles/kucoin_spot_candles.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.606769 hummingbot-20240530/hummingbot/data_feed/candles_feed/okx_perpetual_candles/
+-rw-r--r--   0 madcatz    (501) staff       (20)      145 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/candles_feed/okx_perpetual_candles/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1387 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/candles_feed/okx_perpetual_candles/constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     8700 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/candles_feed/okx_perpetual_candles/okx_perpetual_candles.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.608015 hummingbot-20240530/hummingbot/data_feed/candles_feed/okx_spot_candles/
+-rw-r--r--   0 madcatz    (501) staff       (20)      125 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/candles_feed/okx_spot_candles/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1387 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/candles_feed/okx_spot_candles/constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     8670 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/candles_feed/okx_spot_candles/okx_spot_candles.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.608980 hummingbot-20240530/hummingbot/data_feed/coin_cap_data_feed/
+-rw-r--r--   0 madcatz    (501) staff       (20)      118 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/coin_cap_data_feed/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1075 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/coin_cap_data_feed/coin_cap_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6923 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/coin_cap_data_feed/coin_cap_data_feed.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.609876 hummingbot-20240530/hummingbot/data_feed/coin_gecko_data_feed/
+-rw-r--r--   0 madcatz    (501) staff       (20)      126 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/coin_gecko_data_feed/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      602 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/coin_gecko_data_feed/coin_gecko_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5803 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/coin_gecko_data_feed/coin_gecko_data_feed.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3226 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/custom_api_data_feed.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2466 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/data_feed_base.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.611075 hummingbot-20240530/hummingbot/data_feed/liquidations_feed/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/liquidations_feed/__init__.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.611893 hummingbot-20240530/hummingbot/data_feed/liquidations_feed/binance/
+-rw-r--r--   0 madcatz    (501) staff       (20)      153 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/liquidations_feed/binance/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7604 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/liquidations_feed/binance/binance_liquidations.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      567 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/liquidations_feed/binance/constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     8828 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/liquidations_feed/liquidations_base.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2550 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/liquidations_feed/liquidations_factory.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     9688 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/market_data_provider.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3909 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/data_feed/wallet_tracker_data_feed.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      766 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/exceptions.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.614235 hummingbot-20240530/hummingbot/logger/
+-rw-r--r--   0 madcatz    (501) staff       (20)      755 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/logger/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      586 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/logger/application_warning.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      668 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/logger/cli_handler.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4260 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/logger/log_server_client.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3785 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/logger/logger.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1234 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/logger/struct_logger.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.619061 hummingbot-20240530/hummingbot/model/
+-rw-r--r--   0 madcatz    (501) staff       (20)      566 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/model/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      487 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/model/controllers.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.620041 hummingbot-20240530/hummingbot/model/db_migration/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/model/db_migration/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1877 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/model/db_migration/base_transformation.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2992 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/model/db_migration/migrator.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6482 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/model/db_migration/transformations.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1267 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/model/decimal_type_decorator.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2377 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/model/executors.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2961 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/model/funding_payment.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2005 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/model/inventory_cost.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      888 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/model/market_data.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      821 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/model/market_state.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      365 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/model/metadata.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3109 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/model/order.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1203 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/model/order_status.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1148 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/model/range_position_collected_fees.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      967 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/model/range_position_update.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5796 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/model/sql_connection_manager.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7084 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/model/trade_fill.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1100 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/model/transaction_base.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.620779 hummingbot-20240530/hummingbot/notifier/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/notifier/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      262 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/notifier/notifier_base.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7780 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/notifier/telegram_notifier.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.622598 hummingbot-20240530/hummingbot/pmm_script/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/pmm_script/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    10849 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/pmm_script/pmm_script_base.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5675 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/pmm_script/pmm_script_interface.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   724923 2024-05-30 19:52:26.000000 hummingbot-20240530/hummingbot/pmm_script/pmm_script_iterator.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     1441 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/pmm_script/pmm_script_process.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.624237 hummingbot-20240530/hummingbot/remote_iface/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/remote_iface/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3855 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/remote_iface/messages.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    45513 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/remote_iface/mqtt.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.643922 hummingbot-20240530/hummingbot/strategy/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/__init__.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.646067 hummingbot-20240530/hummingbot/strategy/__utils__/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/__utils__/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)  1261421 2024-05-30 19:52:26.000000 hummingbot-20240530/hummingbot/strategy/__utils__/ring_buffer.cpp
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.649758 hummingbot-20240530/hummingbot/strategy/__utils__/trailing_indicators/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/__utils__/trailing_indicators/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2136 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/__utils__/trailing_indicators/base_trailing_indicator.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      717 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/__utils__/trailing_indicators/exponential_moving_average.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      734 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/__utils__/trailing_indicators/historical_volatility.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1141 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/__utils__/trailing_indicators/instant_volatility.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   816262 2024-05-30 19:52:26.000000 hummingbot-20240530/hummingbot/strategy/__utils__/trailing_indicators/trading_intensity.cpp
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.653237 hummingbot-20240530/hummingbot/strategy/amm_arb/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/amm_arb/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    26897 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/amm_arb/amm_arb.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6279 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/amm_arb/amm_arb_config_map.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7350 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/amm_arb/data_types.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   338533 2024-05-30 19:52:26.000000 hummingbot-20240530/hummingbot/strategy/amm_arb/dummy.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     4476 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/amm_arb/start.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2327 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/amm_arb/utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.654519 hummingbot-20240530/hummingbot/strategy/amm_v3_lp/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/amm_v3_lp/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     9882 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/amm_v3_lp/amm_v3_lp.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3293 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/amm_v3_lp/amm_v3_lp_config_map.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1052 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/amm_v3_lp/start.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   549973 2024-05-30 19:52:26.000000 hummingbot-20240530/hummingbot/strategy/api_asset_price_delegate.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)   381512 2024-05-30 19:52:26.000000 hummingbot-20240530/hummingbot/strategy/asset_price_delegate.cpp
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.660944 hummingbot-20240530/hummingbot/strategy/avellaneda_market_making/
+-rw-r--r--   0 madcatz    (501) staff       (20)      142 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/avellaneda_market_making/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)  2721645 2024-05-30 19:52:26.000000 hummingbot-20240530/hummingbot/strategy/avellaneda_market_making/avellaneda_market_making.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)    17210 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/avellaneda_market_making/avellaneda_market_making_config_map_pydantic.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1767 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/avellaneda_market_making/start.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5368 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/conditional_execution_state.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.668091 hummingbot-20240530/hummingbot/strategy/cross_exchange_market_making/
+-rw-r--r--   0 madcatz    (501) staff       (20)      234 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/cross_exchange_market_making/__init__.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)    90840 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/cross_exchange_market_making/cross_exchange_market_making.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    20395 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/cross_exchange_market_making/cross_exchange_market_making_config_map_pydantic.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   593721 2024-05-30 19:52:26.000000 hummingbot-20240530/hummingbot/strategy/cross_exchange_market_making/order_id_market_pair_tracker.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     3149 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/cross_exchange_market_making/start.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.673338 hummingbot-20240530/hummingbot/strategy/cross_exchange_mining/
+-rw-r--r--   0 madcatz    (501) staff       (20)      204 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/cross_exchange_mining/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)  1449409 2024-05-30 19:52:26.000000 hummingbot-20240530/hummingbot/strategy/cross_exchange_mining/cross_exchange_mining.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     5145 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/cross_exchange_mining/cross_exchange_mining_config_map_pydantic.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      548 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/cross_exchange_mining/cross_exchange_mining_pair.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   528526 2024-05-30 19:52:26.000000 hummingbot-20240530/hummingbot/strategy/cross_exchange_mining/order_id_market_pair_tracker.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     2547 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/cross_exchange_mining/start.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2166 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/data_types.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    15084 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/directional_strategy_base.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    17966 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/hanging_orders_tracker.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.675975 hummingbot-20240530/hummingbot/strategy/hedge/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/hedge/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    29916 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/hedge/hedge.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    10953 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/hedge/hedge_config_map_pydantic.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1772 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/hedge/start.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.678992 hummingbot-20240530/hummingbot/strategy/liquidity_mining/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/liquidity_mining/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      948 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/liquidity_mining/data_types.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   339646 2024-05-30 19:52:26.000000 hummingbot-20240530/hummingbot/strategy/liquidity_mining/dummy.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)    28111 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/liquidity_mining/liquidity_mining.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7282 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/liquidity_mining/liquidity_mining_config_map.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2671 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/liquidity_mining/start.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      524 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/maker_taker_market_pair.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2033 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/market_trading_pair_tuple.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   550837 2024-05-30 19:52:26.000000 hummingbot-20240530/hummingbot/strategy/order_book_asset_price_delegate.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)   846938 2024-05-30 19:52:26.000000 hummingbot-20240530/hummingbot/strategy/order_tracker.cpp
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.682165 hummingbot-20240530/hummingbot/strategy/perpetual_market_making/
+-rw-r--r--   0 madcatz    (501) staff       (20)      139 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/perpetual_market_making/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1407 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/perpetual_market_making/data_types.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   340444 2024-05-30 19:52:26.000000 hummingbot-20240530/hummingbot/strategy/perpetual_market_making/dummy.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)    48666 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/perpetual_market_making/perpetual_market_making.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    15708 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/perpetual_market_making/perpetual_market_making_config_map.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1452 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/perpetual_market_making/perpetual_market_making_order_tracker.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5933 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/perpetual_market_making/start.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.687054 hummingbot-20240530/hummingbot/strategy/pure_market_making/
+-rw-r--r--   0 madcatz    (501) staff       (20)      226 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/pure_market_making/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1407 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/pure_market_making/data_types.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3288 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/pure_market_making/inventory_cost_price_delegate.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   331772 2024-05-30 19:52:26.000000 hummingbot-20240530/hummingbot/strategy/pure_market_making/inventory_skew_calculator.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     2801 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/pure_market_making/moving_price_band.py
+-rw-r--r--   0 madcatz    (501) staff       (20)  2526417 2024-05-30 19:52:27.000000 hummingbot-20240530/hummingbot/strategy/pure_market_making/pure_market_making.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)    22271 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/pure_market_making/pure_market_making_config_map.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   414399 2024-05-30 19:52:27.000000 hummingbot-20240530/hummingbot/strategy/pure_market_making/pure_market_making_order_tracker.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     8774 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/pure_market_making/start.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    10449 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/script_strategy_base.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.691446 hummingbot-20240530/hummingbot/strategy/spot_perpetual_arbitrage/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/spot_perpetual_arbitrage/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2620 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/spot_perpetual_arbitrage/arb_proposal.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   340558 2024-05-30 19:52:26.000000 hummingbot-20240530/hummingbot/strategy/spot_perpetual_arbitrage/dummy.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)    26556 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/spot_perpetual_arbitrage/spot_perpetual_arbitrage.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5762 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/spot_perpetual_arbitrage/spot_perpetual_arbitrage_config_map.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2592 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/spot_perpetual_arbitrage/start.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1942 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/spot_perpetual_arbitrage/utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)  2398768 2024-05-30 19:52:27.000000 hummingbot-20240530/hummingbot/strategy/strategy_base.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)   620855 2024-05-30 19:52:27.000000 hummingbot-20240530/hummingbot/strategy/strategy_py_base.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)    20411 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/strategy_v2_base.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.693991 hummingbot-20240530/hummingbot/strategy/twap/
+-rw-r--r--   0 madcatz    (501) staff       (20)       97 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/twap/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   338167 2024-05-30 19:52:27.000000 hummingbot-20240530/hummingbot/strategy/twap/dummy.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     3468 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/twap/start.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    18542 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/twap/twap.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7079 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/twap/twap_config_map.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      700 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy/utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.694600 hummingbot-20240530/hummingbot/strategy_v2/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/__init__.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.695901 hummingbot-20240530/hummingbot/strategy_v2/backtesting/
+-rw-r--r--   0 madcatz    (501) staff       (20)      474 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/backtesting/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3378 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/backtesting/backtesting_data_provider.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    16905 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/backtesting/backtesting_engine_base.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.696586 hummingbot-20240530/hummingbot/strategy_v2/backtesting/controllers_backtesting/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/backtesting/controllers_backtesting/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      294 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/backtesting/controllers_backtesting/directional_trading_backtesting.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      440 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/backtesting/controllers_backtesting/market_making_backtesting.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3591 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/backtesting/executor_simulator_base.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.697412 hummingbot-20240530/hummingbot/strategy_v2/backtesting/executors_simulator/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/backtesting/executors_simulator/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7053 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/backtesting/executors_simulator/dca_executor_simulator.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3751 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/backtesting/executors_simulator/position_executor_simulator.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.698964 hummingbot-20240530/hummingbot/strategy_v2/controllers/
+-rw-r--r--   0 madcatz    (501) staff       (20)      645 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/controllers/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     8401 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/controllers/controller_base.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    10232 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/controllers/directional_trading_controller_base.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    15908 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/controllers/market_making_controller_base.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.700575 hummingbot-20240530/hummingbot/strategy_v2/executors/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/executors/__init__.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.701520 hummingbot-20240530/hummingbot/strategy_v2/executors/arbitrage_executor/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/executors/arbitrage_executor/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    12599 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/executors/arbitrage_executor/arbitrage_executor.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      492 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/executors/arbitrage_executor/data_types.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      834 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/executors/data_types.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.702313 hummingbot-20240530/hummingbot/strategy_v2/executors/dca_executor/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/executors/dca_executor/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      876 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/executors/dca_executor/data_types.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    25744 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/executors/dca_executor/dca_executor.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    15360 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/executors/executor_base.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    11732 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/executors/executor_orchestrator.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.703114 hummingbot-20240530/hummingbot/strategy_v2/executors/position_executor/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/executors/position_executor/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2172 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/executors/position_executor/data_types.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    32056 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/executors/position_executor/position_executor.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.703954 hummingbot-20240530/hummingbot/strategy_v2/executors/twap_executor/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/executors/twap_executor/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1460 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/executors/twap_executor/data_types.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    13720 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/executors/twap_executor/twap_executor.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.704889 hummingbot-20240530/hummingbot/strategy_v2/executors/xemm_executor/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/executors/xemm_executor/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      464 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/executors/xemm_executor/data_types.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    16859 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/executors/xemm_executor/xemm_executor.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.706450 hummingbot-20240530/hummingbot/strategy_v2/models/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/models/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      129 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/models/base.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1113 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/models/executor_actions.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1504 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/models/executors.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2703 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/models/executors_info.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3099 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/runnable_base.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.708100 hummingbot-20240530/hummingbot/strategy_v2/utils/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/utils/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      312 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/utils/common.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1809 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/utils/config_encoder_decoder.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4419 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/utils/distributions.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4738 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/strategy_v2/utils/order_level_builder.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.711598 hummingbot-20240530/hummingbot/templates/
+-rw-r--r--   0 madcatz    (501) staff       (20)     1898 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/templates/conf_amm_arb_strategy_TEMPLATE.yml
+-rw-r--r--   0 madcatz    (501) staff       (20)      536 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/templates/conf_amm_v3_lp_strategy_TEMPLATE.yml
+-rw-r--r--   0 madcatz    (501) staff       (20)     5439 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/templates/conf_fee_overrides_TEMPLATE.yml
+-rw-r--r--   0 madcatz    (501) staff       (20)     2001 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/templates/conf_liquidity_mining_strategy_TEMPLATE.yml
+-rw-r--r--   0 madcatz    (501) staff       (20)     4032 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/templates/conf_perpetual_market_making_strategy_TEMPLATE.yml
+-rw-r--r--   0 madcatz    (501) staff       (20)     5161 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/templates/conf_pure_market_making_strategy_TEMPLATE.yml
+-rw-r--r--   0 madcatz    (501) staff       (20)     1569 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/templates/conf_spot_perpetual_arbitrage_strategy_TEMPLATE.yml
+-rw-r--r--   0 madcatz    (501) staff       (20)     1344 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/templates/conf_twap_strategy_TEMPLATE.yml
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     2159 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/templates/hummingbot_logs_TEMPLATE.yml
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.712055 hummingbot-20240530/hummingbot/user/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/user/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     8061 2024-05-30 19:45:41.000000 hummingbot-20240530/hummingbot/user/user_balances.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.714024 hummingbot-20240530/hummingbot.egg-info/
+-rw-r--r--   0 madcatz    (501) staff       (20)     1771 2024-05-30 19:52:28.000000 hummingbot-20240530/hummingbot.egg-info/PKG-INFO
+-rw-r--r--   0 madcatz    (501) staff       (20)    48151 2024-05-30 19:52:28.000000 hummingbot-20240530/hummingbot.egg-info/SOURCES.txt
+-rw-r--r--   0 madcatz    (501) staff       (20)        1 2024-05-30 19:52:28.000000 hummingbot-20240530/hummingbot.egg-info/dependency_links.txt
+-rw-r--r--   0 madcatz    (501) staff       (20)      622 2024-05-30 19:52:28.000000 hummingbot-20240530/hummingbot.egg-info/requires.txt
+-rw-r--r--   0 madcatz    (501) staff       (20)       11 2024-05-30 19:52:28.000000 hummingbot-20240530/hummingbot.egg-info/top_level.txt
+-rw-r--r--   0 madcatz    (501) staff       (20)      491 2024-05-30 19:45:41.000000 hummingbot-20240530/pyproject.toml
+-rw-r--r--   0 madcatz    (501) staff       (20)       85 2024-05-30 19:52:28.714890 hummingbot-20240530/setup.cfg
+-rw-r--r--   0 madcatz    (501) staff       (20)     4356 2024-05-30 19:52:02.000000 hummingbot-20240530/setup.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-30 19:52:28.713614 hummingbot-20240530/test/
+-rw-r--r--   0 madcatz    (501) staff       (20)     6190 2024-05-30 19:45:41.000000 hummingbot-20240530/test/test_isolated_asyncio_wrapper_test_case.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3267 2024-05-30 19:45:41.000000 hummingbot-20240530/test/test_local_class_event_loop_wrapper_test_case.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3504 2024-05-30 19:45:41.000000 hummingbot-20240530/test/test_local_test_event_loop_wrapper_test_case.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5466 2024-05-30 19:45:41.000000 hummingbot-20240530/test/test_logger_mixin_for_test.py
```

### Comparing `hummingbot-20240527/LICENSE` & `hummingbot-20240530/LICENSE`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/PKG-INFO` & `hummingbot-20240530/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hummingbot
-Version: 20240527
+Version: 20240530
 Summary: Hummingbot
 Home-page: https://github.com/hummingbot/hummingbot
 Author: Hummingbot Foundation
 Author-email: dev@hummingbot.org
 License: Apache 2.0
 License-File: LICENSE
 Requires-Dist: bidict
```

### Comparing `hummingbot-20240527/README.md` & `hummingbot-20240530/README.md`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/bin/hummingbot_quickstart.py` & `hummingbot-20240530/bin/hummingbot_quickstart.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/__init__.py` & `hummingbot-20240530/hummingbot/__init__.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/__init__.py` & `hummingbot-20240530/hummingbot/client/__init__.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/command/__init__.py` & `hummingbot-20240530/hummingbot/client/command/__init__.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/command/balance_command.py` & `hummingbot-20240530/hummingbot/client/command/balance_command.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/command/config_command.py` & `hummingbot-20240530/hummingbot/client/command/config_command.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/command/connect_command.py` & `hummingbot-20240530/hummingbot/client/command/connect_command.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/command/create_command.py` & `hummingbot-20240530/hummingbot/client/command/create_command.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/command/exit_command.py` & `hummingbot-20240530/hummingbot/client/command/exit_command.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/command/export_command.py` & `hummingbot-20240530/hummingbot/client/command/export_command.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/command/gateway_api_manager.py` & `hummingbot-20240530/hummingbot/client/command/gateway_api_manager.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/command/gateway_command.py` & `hummingbot-20240530/hummingbot/client/command/gateway_command.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/command/help_command.py` & `hummingbot-20240530/hummingbot/client/command/help_command.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/command/history_command.py` & `hummingbot-20240530/hummingbot/client/command/history_command.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/command/import_command.py` & `hummingbot-20240530/hummingbot/client/command/import_command.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/command/mqtt_command.py` & `hummingbot-20240530/hummingbot/client/command/mqtt_command.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/command/order_book_command.py` & `hummingbot-20240530/hummingbot/client/command/order_book_command.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/command/previous_strategy_command.py` & `hummingbot-20240530/hummingbot/client/command/previous_strategy_command.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/command/rate_command.py` & `hummingbot-20240530/hummingbot/client/command/rate_command.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/command/silly_commands.py` & `hummingbot-20240530/hummingbot/client/command/silly_commands.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/command/start_command.py` & `hummingbot-20240530/hummingbot/client/command/start_command.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/command/status_command.py` & `hummingbot-20240530/hummingbot/client/command/status_command.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/command/stop_command.py` & `hummingbot-20240530/hummingbot/client/command/stop_command.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/command/ticker_command.py` & `hummingbot-20240530/hummingbot/client/command/ticker_command.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/config/client_config_map.py` & `hummingbot-20240530/hummingbot/client/config/client_config_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -432,14 +432,15 @@
     def get_url(self, db_path: str) -> str:
         ...
 
 
 class DBSqliteMode(DBMode):
     db_engine: str = Field(
         default="sqlite",
+        const=True,
         client_data=ClientFieldData(
             prompt=lambda cm: (
                 "Please enter database engine you want to use (reference: https://docs.sqlalchemy.org/en/13/dialects/)"
             ),
         ),
     )
 
@@ -741,54 +742,59 @@
     def build_rate_source(self) -> RateSourceBase:
         return RATE_ORACLE_SOURCES[self.Config.title]()
 
 
 class AscendExRateSourceMode(ExchangeRateSourceModeBase):
     name: str = Field(
         default="ascend_ex",
+        const=True,
         client_data=None,
     )
 
     class Config:
         title = "ascend_ex"
 
 
 class BinanceRateSourceMode(ExchangeRateSourceModeBase):
     name: str = Field(
         default="binance",
+        const=True,
         client_data=None,
     )
 
     class Config:
         title = "binance"
 
 
 class BinanceUSRateSourceMode(ExchangeRateSourceModeBase):
     name: str = Field(
         default="binance_us",
+        const=True,
         client_data=None,
     )
 
     class Config:
         title = "binance_us"
 
 
 class CubeRateSourceMode(ExchangeRateSourceModeBase):
     name: str = Field(
         default="cube",
+        const=True,
         client_data=None,
     )
 
     class Config:
         title = "cube"
 
 
 class CoinGeckoRateSourceMode(RateSourceModeBase):
     name: str = Field(
         default="coin_gecko",
+        const=True,
         client_data=None,
     )
 
     extra_tokens: List[str] = Field(
         default=[],
         client_data=ClientFieldData(
             prompt=lambda cm: (
@@ -819,14 +825,15 @@
         RateOracle.get_instance().source.extra_token_ids = values["extra_tokens"]
         return values
 
 
 class CoinCapRateSourceMode(RateSourceModeBase):
     name: str = Field(
         default="coin_cap",
+        const=True,
         client_data=None,
     )
     assets_map: Dict[str, str] = Field(
         default=",".join(
             [
                 ":".join(pair) for pair in {
                     "BTC": "bitcoin",
@@ -899,34 +906,37 @@
         )
         return rate_source
 
 
 class KuCoinRateSourceMode(ExchangeRateSourceModeBase):
     name: str = Field(
         default="kucoin",
+        const=True,
         client_data=None,
     )
 
     class Config:
         title = "kucoin"
 
 
 class GateIoRateSourceMode(ExchangeRateSourceModeBase):
     name: str = Field(
         default="gate_io",
+        const=True,
         client_data=None,
     )
 
     class Config:
         title: str = "gate_io"
 
 
 class CoinbaseAdvancedTradeRateSourceMode(ExchangeRateSourceModeBase):
     name: str = Field(
         default="coinbase_advanced_trade",
+        const=True,
         client_data=None,
     )
 
     class Config:
         title: str = "coinbase_advanced_trade"
```

### Comparing `hummingbot-20240527/hummingbot/client/config/conf_migration.py` & `hummingbot-20240530/hummingbot/client/config/conf_migration.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/config/config_crypt.py` & `hummingbot-20240530/hummingbot/client/config/config_crypt.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/config/config_data_types.py` & `hummingbot-20240530/hummingbot/client/config/config_data_types.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from dataclasses import dataclass
 from datetime import datetime
 from decimal import Decimal
 from enum import Enum
 from typing import Any, Callable, Optional
 
 from pydantic import BaseModel, Extra, Field, validator
+from pydantic.schema import default_ref_template
 
 from hummingbot.client.config.config_methods import strategy_config_schema_encoder
 from hummingbot.client.config.config_validators import validate_connector, validate_decimal
 
 
 class ClientConfigEnum(Enum):
     def __str__(self):
@@ -32,19 +33,19 @@
         extra = Extra.forbid
         json_encoders = {
             datetime: lambda dt: dt.strftime("%Y-%m-%d %H:%M:%S"),
         }
 
     @classmethod
     def schema_json(
-        cls, *, by_alias: bool = True, **dumps_kwargs: Any
+        cls, *, by_alias: bool = True, ref_template: str = default_ref_template, **dumps_kwargs: Any
     ) -> str:
         # todo: make it ignore `client_data` all together
         return cls.__config__.json_dumps(
-            cls.schema(by_alias=by_alias),
+            cls.schema(by_alias=by_alias, ref_template=ref_template),
             default=strategy_config_schema_encoder,
             **dumps_kwargs
         )
 
     @classmethod
     def _clear_schema_cache(cls):
         cls.__schema_cache__ = {}
```

### Comparing `hummingbot-20240527/hummingbot/client/config/config_helpers.py` & `hummingbot-20240530/hummingbot/client/config/config_helpers.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/config/config_methods.py` & `hummingbot-20240530/hummingbot/client/config/config_methods.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/config/config_validators.py` & `hummingbot-20240530/hummingbot/client/config/config_validators.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/config/config_var.py` & `hummingbot-20240530/hummingbot/client/config/config_var.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/config/fee_overrides_config_map.py` & `hummingbot-20240530/hummingbot/client/config/fee_overrides_config_map.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/config/security.py` & `hummingbot-20240530/hummingbot/client/config/security.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/config/strategy_config_data_types.py` & `hummingbot-20240530/hummingbot/client/config/strategy_config_data_types.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/config/trade_fee_schema_loader.py` & `hummingbot-20240530/hummingbot/client/config/trade_fee_schema_loader.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/hummingbot_application.py` & `hummingbot-20240530/hummingbot/client/hummingbot_application.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/performance.py` & `hummingbot-20240530/hummingbot/client/performance.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/platform.py` & `hummingbot-20240530/hummingbot/client/platform.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/settings.py` & `hummingbot-20240530/hummingbot/client/settings.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/tab/data_types.py` & `hummingbot-20240530/hummingbot/client/tab/data_types.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/tab/order_book_tab.py` & `hummingbot-20240530/hummingbot/client/tab/order_book_tab.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/tab/tab_base.py` & `hummingbot-20240530/hummingbot/client/tab/tab_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/tab/tab_example_tab.py` & `hummingbot-20240530/hummingbot/client/tab/tab_example_tab.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/ui/__init__.py` & `hummingbot-20240530/hummingbot/client/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/ui/completer.py` & `hummingbot-20240530/hummingbot/client/ui/completer.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/ui/custom_widgets.py` & `hummingbot-20240530/hummingbot/client/ui/custom_widgets.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/ui/hummingbot_cli.py` & `hummingbot-20240530/hummingbot/client/ui/hummingbot_cli.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/ui/interface_utils.py` & `hummingbot-20240530/hummingbot/client/ui/interface_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/ui/keybindings.py` & `hummingbot-20240530/hummingbot/client/ui/keybindings.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/ui/layout.py` & `hummingbot-20240530/hummingbot/client/ui/layout.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/ui/parser.py` & `hummingbot-20240530/hummingbot/client/ui/parser.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/ui/scroll_handlers.py` & `hummingbot-20240530/hummingbot/client/ui/scroll_handlers.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/ui/stdout_redirection.py` & `hummingbot-20240530/hummingbot/client/ui/stdout_redirection.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/client/ui/style.py` & `hummingbot-20240530/hummingbot/client/ui/style.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/budget_checker.py` & `hummingbot-20240530/hummingbot/connector/budget_checker.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/client_order_tracker.py` & `hummingbot-20240530/hummingbot/connector/client_order_tracker.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/connector_base.cpp` & `hummingbot-20240530/hummingbot/connector/connector_base.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/connector_metrics_collector.py` & `hummingbot-20240530/hummingbot/connector/connector_metrics_collector.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_auth.py` & `hummingbot-20240530/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_constants.py` & `hummingbot-20240530/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_derivative.py` & `hummingbot-20240530/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_derivative.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_user_stream_data_source.py` & `hummingbot-20240530/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_utils.py` & `hummingbot-20240530/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_web_utils.py` & `hummingbot-20240530/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/binance_perpetual/dummy.cpp` & `hummingbot-20240530/hummingbot/connector/derivative/binance_perpetual/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_auth.py` & `hummingbot-20240530/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_constants.py` & `hummingbot-20240530/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_derivative.py` & `hummingbot-20240530/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_derivative.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_user_stream_data_source.py` & `hummingbot-20240530/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_utils.py` & `hummingbot-20240530/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_web_utils.py` & `hummingbot-20240530/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/bit_com_perpetual/dummy.cpp` & `hummingbot-20240530/hummingbot/connector/derivative/bit_com_perpetual/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_auth.py` & `hummingbot-20240530/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_constants.py` & `hummingbot-20240530/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_derivative.py` & `hummingbot-20240530/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_derivative.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_user_stream_data_source.py` & `hummingbot-20240530/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_utils.py` & `hummingbot-20240530/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_web_utils.py` & `hummingbot-20240530/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_auth.py` & `hummingbot-20240530/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_constants.py` & `hummingbot-20240530/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_derivative.py` & `hummingbot-20240530/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_derivative.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_user_stream_data_source.py` & `hummingbot-20240530/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_utils.py` & `hummingbot-20240530/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_web_utils.py` & `hummingbot-20240530/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/bybit_perpetual/dummy.cpp` & `hummingbot-20240530/hummingbot/connector/derivative/bybit_perpetual/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_auth.py` & `hummingbot-20240530/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_constants.py` & `hummingbot-20240530/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_derivative.py` & `hummingbot-20240530/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_derivative.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_user_stream_data_source.py` & `hummingbot-20240530/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_utils.py` & `hummingbot-20240530/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_web_utils.py` & `hummingbot-20240530/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/gate_io_perpetual/dummy.cpp` & `hummingbot-20240530/hummingbot/connector/derivative/gate_io_perpetual/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_auth.py` & `hummingbot-20240530/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_constants.py` & `hummingbot-20240530/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_derivative.py` & `hummingbot-20240530/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_derivative.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_user_stream_data_source.py` & `hummingbot-20240530/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_utils.py` & `hummingbot-20240530/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_web_utils.py` & `hummingbot-20240530/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/hyperliquid_perpetual/dummy.cpp` & `hummingbot-20240530/hummingbot/connector/derivative/hyperliquid_perpetual/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_auth.py` & `hummingbot-20240530/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_constants.py` & `hummingbot-20240530/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_derivative.py` & `hummingbot-20240530/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_derivative.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_user_stream_data_source.py` & `hummingbot-20240530/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_utils.py` & `hummingbot-20240530/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_web_utils.py` & `hummingbot-20240530/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/injective_v2_perpetual/injective_v2_perpetual_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/derivative/injective_v2_perpetual/injective_v2_perpetual_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/injective_v2_perpetual/injective_v2_perpetual_derivative.py` & `hummingbot-20240530/hummingbot/connector/derivative/injective_v2_perpetual/injective_v2_perpetual_derivative.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/injective_v2_perpetual/injective_v2_perpetual_utils.py` & `hummingbot-20240530/hummingbot/connector/derivative/injective_v2_perpetual/injective_v2_perpetual_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/kucoin_perpetual/dummy.cpp` & `hummingbot-20240530/hummingbot/connector/derivative/kucoin_perpetual/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_api_user_stream_data_source.py` & `hummingbot-20240530/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_auth.py` & `hummingbot-20240530/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_constants.py` & `hummingbot-20240530/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_derivative.py` & `hummingbot-20240530/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_derivative.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_utils.py` & `hummingbot-20240530/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_web_utils.py` & `hummingbot-20240530/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_auth.py` & `hummingbot-20240530/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_constants.py` & `hummingbot-20240530/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_derivative.py` & `hummingbot-20240530/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_derivative.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_user_stream_data_source.py` & `hummingbot-20240530/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_utils.py` & `hummingbot-20240530/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_web_utils.py` & `hummingbot-20240530/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/perpetual_budget_checker.py` & `hummingbot-20240530/hummingbot/connector/derivative/perpetual_budget_checker.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_api_user_stream_data_source.py` & `hummingbot-20240530/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_auth.py` & `hummingbot-20240530/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_constants.py` & `hummingbot-20240530/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_derivative.py` & `hummingbot-20240530/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_derivative.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_utils.py` & `hummingbot-20240530/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_web_utils.py` & `hummingbot-20240530/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/position.py` & `hummingbot-20240530/hummingbot/connector/derivative/position.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_auth.py` & `hummingbot-20240530/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_constants.py` & `hummingbot-20240530/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_data.py` & `hummingbot-20240530/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_data.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_derivative.py` & `hummingbot-20240530/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_derivative.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_user_stream_data_source.py` & `hummingbot-20240530/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_utils.py` & `hummingbot-20240530/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_web_utils.py` & `hummingbot-20240530/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/derivative_base.py` & `hummingbot-20240530/hummingbot/connector/derivative_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/ascend_ex/ascend_ex_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/ascend_ex/ascend_ex_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/ascend_ex/ascend_ex_api_user_stream_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/ascend_ex/ascend_ex_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/ascend_ex/ascend_ex_auth.py` & `hummingbot-20240530/hummingbot/connector/exchange/ascend_ex/ascend_ex_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/ascend_ex/ascend_ex_constants.py` & `hummingbot-20240530/hummingbot/connector/exchange/ascend_ex/ascend_ex_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/ascend_ex/ascend_ex_exchange.py` & `hummingbot-20240530/hummingbot/connector/exchange/ascend_ex/ascend_ex_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/ascend_ex/ascend_ex_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/ascend_ex/ascend_ex_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/ascend_ex/ascend_ex_web_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/ascend_ex/ascend_ex_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/binance/binance_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/binance/binance_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/binance/binance_api_user_stream_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/binance/binance_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/binance/binance_auth.py` & `hummingbot-20240530/hummingbot/connector/exchange/binance/binance_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/binance/binance_constants.py` & `hummingbot-20240530/hummingbot/connector/exchange/binance/binance_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/binance/binance_exchange.py` & `hummingbot-20240530/hummingbot/connector/exchange/binance/binance_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/binance/binance_order_book.py` & `hummingbot-20240530/hummingbot/connector/exchange/binance/binance_order_book.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/binance/binance_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/binance/binance_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/binance/binance_web_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/binance/binance_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/binance/dummy.cpp` & `hummingbot-20240530/hummingbot/connector/exchange/binance/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bitfinex/__init__.py` & `hummingbot-20240530/hummingbot/connector/exchange/bitfinex/__init__.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bitfinex/bitfinex_active_order_tracker.cpp` & `hummingbot-20240530/hummingbot/connector/exchange/bitfinex/bitfinex_active_order_tracker.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bitfinex/bitfinex_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/bitfinex/bitfinex_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bitfinex/bitfinex_api_user_stream_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/bitfinex/bitfinex_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bitfinex/bitfinex_auth.py` & `hummingbot-20240530/hummingbot/connector/exchange/bitfinex/bitfinex_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bitfinex/bitfinex_exchange.cpp` & `hummingbot-20240530/hummingbot/connector/exchange/bitfinex/bitfinex_exchange.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bitfinex/bitfinex_in_flight_order.cpp` & `hummingbot-20240530/hummingbot/connector/exchange/bitfinex/bitfinex_in_flight_order.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bitfinex/bitfinex_order_book.cpp` & `hummingbot-20240530/hummingbot/connector/exchange/bitfinex/bitfinex_order_book.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bitfinex/bitfinex_order_book_message.py` & `hummingbot-20240530/hummingbot/connector/exchange/bitfinex/bitfinex_order_book_message.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bitfinex/bitfinex_order_book_tracker.py` & `hummingbot-20240530/hummingbot/connector/exchange/bitfinex/bitfinex_order_book_tracker.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bitfinex/bitfinex_order_book_tracker_entry.py` & `hummingbot-20240530/hummingbot/connector/exchange/bitfinex/bitfinex_order_book_tracker_entry.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bitfinex/bitfinex_user_stream_tracker.py` & `hummingbot-20240530/hummingbot/connector/exchange/bitfinex/bitfinex_user_stream_tracker.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bitfinex/bitfinex_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/bitfinex/bitfinex_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bitfinex/bitfinex_websocket.py` & `hummingbot-20240530/hummingbot/connector/exchange/bitfinex/bitfinex_websocket.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bitmart/bitmart_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/bitmart/bitmart_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bitmart/bitmart_api_user_stream_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/bitmart/bitmart_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bitmart/bitmart_auth.py` & `hummingbot-20240530/hummingbot/connector/exchange/bitmart/bitmart_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bitmart/bitmart_constants.py` & `hummingbot-20240530/hummingbot/connector/exchange/bitmart/bitmart_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bitmart/bitmart_exchange.py` & `hummingbot-20240530/hummingbot/connector/exchange/bitmart/bitmart_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bitmart/bitmart_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/bitmart/bitmart_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bitmart/bitmart_web_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/bitmart/bitmart_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bitmart/dummy.cpp` & `hummingbot-20240530/hummingbot/connector/exchange/bitmart/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bitrue/bitrue_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/bitrue/bitrue_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bitrue/bitrue_auth.py` & `hummingbot-20240530/hummingbot/connector/exchange/bitrue/bitrue_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bitrue/bitrue_constants.py` & `hummingbot-20240530/hummingbot/connector/exchange/bitrue/bitrue_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bitrue/bitrue_exchange.py` & `hummingbot-20240530/hummingbot/connector/exchange/bitrue/bitrue_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bitrue/bitrue_order_book.py` & `hummingbot-20240530/hummingbot/connector/exchange/bitrue/bitrue_order_book.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bitrue/bitrue_user_stream_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/bitrue/bitrue_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bitrue/bitrue_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/bitrue/bitrue_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bitrue/bitrue_web_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/bitrue/bitrue_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/btc_markets/btc_markets_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/btc_markets/btc_markets_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/btc_markets/btc_markets_api_user_stream_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/btc_markets/btc_markets_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/btc_markets/btc_markets_auth.py` & `hummingbot-20240530/hummingbot/connector/exchange/btc_markets/btc_markets_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/btc_markets/btc_markets_constants.py` & `hummingbot-20240530/hummingbot/connector/exchange/btc_markets/btc_markets_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/btc_markets/btc_markets_exchange.py` & `hummingbot-20240530/hummingbot/connector/exchange/btc_markets/btc_markets_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/btc_markets/btc_markets_order_book.py` & `hummingbot-20240530/hummingbot/connector/exchange/btc_markets/btc_markets_order_book.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/btc_markets/btc_markets_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/btc_markets/btc_markets_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/btc_markets/btc_markets_web_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/btc_markets/btc_markets_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bybit/bybit_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/bybit/bybit_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bybit/bybit_api_user_stream_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/bybit/bybit_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bybit/bybit_auth.py` & `hummingbot-20240530/hummingbot/connector/exchange/bybit/bybit_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bybit/bybit_constants.py` & `hummingbot-20240530/hummingbot/connector/exchange/bybit/bybit_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bybit/bybit_exchange.py` & `hummingbot-20240530/hummingbot/connector/exchange/bybit/bybit_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bybit/bybit_order_book.py` & `hummingbot-20240530/hummingbot/connector/exchange/bybit/bybit_order_book.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bybit/bybit_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/bybit/bybit_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bybit/bybit_web_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/bybit/bybit_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/bybit/dummy.cpp` & `hummingbot-20240530/hummingbot/connector/exchange/bybit/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_api_user_stream_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_auth.py` & `hummingbot-20240530/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_constants.py` & `hummingbot-20240530/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_exchange.py` & `hummingbot-20240530/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_order_book.py` & `hummingbot-20240530/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_order_book.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_web_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/coinbase_advanced_trade/dummy.cpp` & `hummingbot-20240530/hummingbot/connector/exchange/coinbase_advanced_trade/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_active_order_tracker.cpp` & `hummingbot-20240530/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_active_order_tracker.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_api_user_stream_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_auth.py` & `hummingbot-20240530/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_exchange.cpp` & `hummingbot-20240530/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_exchange.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_in_flight_order.cpp` & `hummingbot-20240530/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_in_flight_order.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_order_book.cpp` & `hummingbot-20240530/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_order_book.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_order_book_message.py` & `hummingbot-20240530/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_order_book_message.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_order_book_tracker.py` & `hummingbot-20240530/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_order_book_tracker.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_order_book_tracker_entry.py` & `hummingbot-20240530/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_order_book_tracker_entry.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_user_stream_tracker.py` & `hummingbot-20240530/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_user_stream_tracker.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/cube/cube_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/cube/cube_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/cube/cube_api_user_stream_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/cube/cube_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/cube/cube_auth.py` & `hummingbot-20240530/hummingbot/connector/exchange/cube/cube_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/cube/cube_constants.py` & `hummingbot-20240530/hummingbot/connector/exchange/cube/cube_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/cube/cube_exchange.py` & `hummingbot-20240530/hummingbot/connector/exchange/cube/cube_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/cube/cube_order_book.py` & `hummingbot-20240530/hummingbot/connector/exchange/cube/cube_order_book.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/cube/cube_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/cube/cube_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/cube/cube_web_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/cube/cube_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/cube/cube_ws_protobufs/market_data_pb2.py` & `hummingbot-20240530/hummingbot/connector/exchange/cube/cube_ws_protobufs/market_data_pb2.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/cube/cube_ws_protobufs/market_data_pb2.pyi` & `hummingbot-20240530/hummingbot/connector/exchange/cube/cube_ws_protobufs/market_data_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/cube/cube_ws_protobufs/trade_pb2.py` & `hummingbot-20240530/hummingbot/connector/exchange/cube/cube_ws_protobufs/trade_pb2.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/cube/cube_ws_protobufs/trade_pb2.pyi` & `hummingbot-20240530/hummingbot/connector/exchange/cube/cube_ws_protobufs/trade_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/cube/dummy.cpp` & `hummingbot-20240530/hummingbot/connector/exchange/cube/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/foxbit/foxbit_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/foxbit/foxbit_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/foxbit/foxbit_api_user_stream_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/foxbit/foxbit_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/foxbit/foxbit_auth.py` & `hummingbot-20240530/hummingbot/connector/exchange/foxbit/foxbit_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/foxbit/foxbit_connector.cpp` & `hummingbot-20240530/hummingbot/connector/exchange/foxbit/foxbit_connector.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/foxbit/foxbit_constants.py` & `hummingbot-20240530/hummingbot/connector/exchange/foxbit/foxbit_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/foxbit/foxbit_exchange.py` & `hummingbot-20240530/hummingbot/connector/exchange/foxbit/foxbit_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/foxbit/foxbit_order_book.py` & `hummingbot-20240530/hummingbot/connector/exchange/foxbit/foxbit_order_book.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/foxbit/foxbit_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/foxbit/foxbit_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/foxbit/foxbit_web_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/foxbit/foxbit_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/gate_io/gate_io_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/gate_io/gate_io_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/gate_io/gate_io_api_user_stream_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/gate_io/gate_io_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/gate_io/gate_io_auth.py` & `hummingbot-20240530/hummingbot/connector/exchange/gate_io/gate_io_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/gate_io/gate_io_constants.py` & `hummingbot-20240530/hummingbot/connector/exchange/gate_io/gate_io_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/gate_io/gate_io_exchange.py` & `hummingbot-20240530/hummingbot/connector/exchange/gate_io/gate_io_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/gate_io/gate_io_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/gate_io/gate_io_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/gate_io/gate_io_web_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/gate_io/gate_io_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/gate_io/placeholder.cpp` & `hummingbot-20240530/hummingbot/connector/exchange/gate_io/placeholder.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/hitbtc/hitbtc_active_order_tracker.cpp` & `hummingbot-20240530/hummingbot/connector/exchange/hitbtc/hitbtc_active_order_tracker.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/hitbtc/hitbtc_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/hitbtc/hitbtc_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/hitbtc/hitbtc_api_user_stream_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/hitbtc/hitbtc_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/hitbtc/hitbtc_auth.py` & `hummingbot-20240530/hummingbot/connector/exchange/hitbtc/hitbtc_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/hitbtc/hitbtc_constants.py` & `hummingbot-20240530/hummingbot/connector/exchange/hitbtc/hitbtc_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/hitbtc/hitbtc_exchange.py` & `hummingbot-20240530/hummingbot/connector/exchange/hitbtc/hitbtc_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/hitbtc/hitbtc_in_flight_order.py` & `hummingbot-20240530/hummingbot/connector/exchange/hitbtc/hitbtc_in_flight_order.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/hitbtc/hitbtc_order_book.py` & `hummingbot-20240530/hummingbot/connector/exchange/hitbtc/hitbtc_order_book.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/hitbtc/hitbtc_order_book_message.py` & `hummingbot-20240530/hummingbot/connector/exchange/hitbtc/hitbtc_order_book_message.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/hitbtc/hitbtc_order_book_tracker.py` & `hummingbot-20240530/hummingbot/connector/exchange/hitbtc/hitbtc_order_book_tracker.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/hitbtc/hitbtc_order_book_tracker_entry.py` & `hummingbot-20240530/hummingbot/connector/exchange/hitbtc/hitbtc_order_book_tracker_entry.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/hitbtc/hitbtc_user_stream_tracker.py` & `hummingbot-20240530/hummingbot/connector/exchange/hitbtc/hitbtc_user_stream_tracker.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/hitbtc/hitbtc_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/hitbtc/hitbtc_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/hitbtc/hitbtc_websocket.py` & `hummingbot-20240530/hummingbot/connector/exchange/hitbtc/hitbtc_websocket.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/htx/htx_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/htx/htx_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/htx/htx_api_user_stream_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/htx/htx_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/htx/htx_auth.py` & `hummingbot-20240530/hummingbot/connector/exchange/htx/htx_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/htx/htx_constants.py` & `hummingbot-20240530/hummingbot/connector/exchange/htx/htx_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/htx/htx_exchange.py` & `hummingbot-20240530/hummingbot/connector/exchange/htx/htx_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/htx/htx_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/htx/htx_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/htx/htx_web_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/htx/htx_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/injective_v2/account_delegation_script.py` & `hummingbot-20240530/hummingbot/connector/exchange/injective_v2/account_delegation_script.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/injective_v2/data_sources/injective_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/injective_v2/data_sources/injective_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/injective_v2/data_sources/injective_grantee_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/injective_v2/data_sources/injective_grantee_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/injective_v2/data_sources/injective_read_only_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/injective_v2/data_sources/injective_read_only_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/injective_v2/data_sources/injective_vaults_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/injective_v2/data_sources/injective_vaults_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/injective_v2/injective_constants.py` & `hummingbot-20240530/hummingbot/connector/exchange/injective_v2/injective_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/injective_v2/injective_market.py` & `hummingbot-20240530/hummingbot/connector/exchange/injective_v2/injective_market.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/injective_v2/injective_query_executor.py` & `hummingbot-20240530/hummingbot/connector/exchange/injective_v2/injective_query_executor.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/injective_v2/injective_v2_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/injective_v2/injective_v2_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/injective_v2/injective_v2_exchange.py` & `hummingbot-20240530/hummingbot/connector/exchange/injective_v2/injective_v2_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/injective_v2/injective_v2_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/injective_v2/injective_v2_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/kraken/kraken_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/kraken/kraken_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/kraken/kraken_api_user_stream_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/kraken/kraken_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/kraken/kraken_auth.py` & `hummingbot-20240530/hummingbot/connector/exchange/kraken/kraken_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/kraken/kraken_constants.py` & `hummingbot-20240530/hummingbot/connector/exchange/kraken/kraken_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/kraken/kraken_exchange.py` & `hummingbot-20240530/hummingbot/connector/exchange/kraken/kraken_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/kraken/kraken_order_book.py` & `hummingbot-20240530/hummingbot/connector/exchange/kraken/kraken_order_book.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/kraken/kraken_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/kraken/kraken_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/kraken/kraken_web_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/kraken/kraken_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/kucoin/dummy.cpp` & `hummingbot-20240530/hummingbot/connector/exchange/kucoin/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/kucoin/kucoin_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/kucoin/kucoin_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/kucoin/kucoin_api_user_stream_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/kucoin/kucoin_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/kucoin/kucoin_auth.py` & `hummingbot-20240530/hummingbot/connector/exchange/kucoin/kucoin_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/kucoin/kucoin_constants.py` & `hummingbot-20240530/hummingbot/connector/exchange/kucoin/kucoin_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/kucoin/kucoin_exchange.py` & `hummingbot-20240530/hummingbot/connector/exchange/kucoin/kucoin_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/kucoin/kucoin_order_book_message.py` & `hummingbot-20240530/hummingbot/connector/exchange/kucoin/kucoin_order_book_message.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/kucoin/kucoin_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/kucoin/kucoin_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/kucoin/kucoin_web_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/kucoin/kucoin_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/mexc/dummy.cpp` & `hummingbot-20240530/hummingbot/connector/exchange/mexc/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/mexc/mexc_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/mexc/mexc_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/mexc/mexc_api_user_stream_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/mexc/mexc_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/mexc/mexc_auth.py` & `hummingbot-20240530/hummingbot/connector/exchange/mexc/mexc_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/mexc/mexc_constants.py` & `hummingbot-20240530/hummingbot/connector/exchange/mexc/mexc_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/mexc/mexc_exchange.py` & `hummingbot-20240530/hummingbot/connector/exchange/mexc/mexc_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/mexc/mexc_order_book.py` & `hummingbot-20240530/hummingbot/connector/exchange/mexc/mexc_order_book.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/mexc/mexc_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/mexc/mexc_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/mexc/mexc_web_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/mexc/mexc_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/ndax/dummy.cpp` & `hummingbot-20240530/hummingbot/connector/exchange/ndax/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/ndax/ndax_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/ndax/ndax_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/ndax/ndax_api_user_stream_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/ndax/ndax_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/ndax/ndax_auth.py` & `hummingbot-20240530/hummingbot/connector/exchange/ndax/ndax_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/ndax/ndax_constants.py` & `hummingbot-20240530/hummingbot/connector/exchange/ndax/ndax_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/ndax/ndax_exchange.py` & `hummingbot-20240530/hummingbot/connector/exchange/ndax/ndax_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/ndax/ndax_in_flight_order.py` & `hummingbot-20240530/hummingbot/connector/exchange/ndax/ndax_in_flight_order.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/ndax/ndax_order_book.py` & `hummingbot-20240530/hummingbot/connector/exchange/ndax/ndax_order_book.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/ndax/ndax_order_book_message.py` & `hummingbot-20240530/hummingbot/connector/exchange/ndax/ndax_order_book_message.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/ndax/ndax_order_book_tracker.py` & `hummingbot-20240530/hummingbot/connector/exchange/ndax/ndax_order_book_tracker.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/ndax/ndax_user_stream_tracker.py` & `hummingbot-20240530/hummingbot/connector/exchange/ndax/ndax_user_stream_tracker.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/ndax/ndax_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/ndax/ndax_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/ndax/ndax_websocket_adaptor.py` & `hummingbot-20240530/hummingbot/connector/exchange/ndax/ndax_websocket_adaptor.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/okx/okx_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/okx/okx_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/okx/okx_api_user_stream_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/okx/okx_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/okx/okx_auth.py` & `hummingbot-20240530/hummingbot/connector/exchange/okx/okx_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/okx/okx_constants.py` & `hummingbot-20240530/hummingbot/connector/exchange/okx/okx_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/okx/okx_exchange.py` & `hummingbot-20240530/hummingbot/connector/exchange/okx/okx_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/okx/okx_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/okx/okx_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/okx/okx_web_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/okx/okx_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/paper_trade/__init__.py` & `hummingbot-20240530/hummingbot/connector/exchange/paper_trade/__init__.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/paper_trade/market_config.py` & `hummingbot-20240530/hummingbot/connector/exchange/paper_trade/market_config.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/paper_trade/paper_trade_exchange.cpp` & `hummingbot-20240530/hummingbot/connector/exchange/paper_trade/paper_trade_exchange.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/polkadex/polkadex_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/polkadex/polkadex_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/polkadex/polkadex_constants.py` & `hummingbot-20240530/hummingbot/connector/exchange/polkadex/polkadex_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/polkadex/polkadex_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/polkadex/polkadex_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/polkadex/polkadex_exchange.py` & `hummingbot-20240530/hummingbot/connector/exchange/polkadex/polkadex_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/polkadex/polkadex_query_executor.py` & `hummingbot-20240530/hummingbot/connector/exchange/polkadex/polkadex_query_executor.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/polkadex/polkadex_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/polkadex/polkadex_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/vertex/dummy.cpp` & `hummingbot-20240530/hummingbot/connector/exchange/vertex/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/vertex/vertex_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/vertex/vertex_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/vertex/vertex_api_user_stream_data_source.py` & `hummingbot-20240530/hummingbot/connector/exchange/vertex/vertex_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/vertex/vertex_auth.py` & `hummingbot-20240530/hummingbot/connector/exchange/vertex/vertex_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/vertex/vertex_constants.py` & `hummingbot-20240530/hummingbot/connector/exchange/vertex/vertex_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/vertex/vertex_eip712_structs.py` & `hummingbot-20240530/hummingbot/connector/exchange/vertex/vertex_eip712_structs.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/vertex/vertex_exchange.py` & `hummingbot-20240530/hummingbot/connector/exchange/vertex/vertex_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/vertex/vertex_order_book.py` & `hummingbot-20240530/hummingbot/connector/exchange/vertex/vertex_order_book.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/vertex/vertex_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/vertex/vertex_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange/vertex/vertex_web_utils.py` & `hummingbot-20240530/hummingbot/connector/exchange/vertex/vertex_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange_base.cpp` & `hummingbot-20240530/hummingbot/connector/exchange_base.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/exchange_py_base.py` & `hummingbot-20240530/hummingbot/connector/exchange_py_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/gateway/amm/gateway_algorand_amm.py` & `hummingbot-20240530/hummingbot/connector/gateway/amm/gateway_algorand_amm.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/gateway/amm/gateway_evm_amm.py` & `hummingbot-20240530/hummingbot/connector/gateway/amm/gateway_evm_amm.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/gateway/amm/gateway_near_amm.py` & `hummingbot-20240530/hummingbot/connector/gateway/amm/gateway_near_amm.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/gateway/amm/gateway_tezos_amm.py` & `hummingbot-20240530/hummingbot/connector/gateway/amm/gateway_tezos_amm.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/gateway/amm_lp/gateway_evm_amm_lp.py` & `hummingbot-20240530/hummingbot/connector/gateway/amm_lp/gateway_evm_amm_lp.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/gateway/amm_lp/gateway_in_flight_lp_order.py` & `hummingbot-20240530/hummingbot/connector/gateway/amm_lp/gateway_in_flight_lp_order.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/gateway/amm_lp/gateway_osmosis_amm_lp.py` & `hummingbot-20240530/hummingbot/connector/gateway/amm_lp/gateway_osmosis_amm_lp.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/gateway/amm_perpetual/gateway_evm_amm_perpetual.py` & `hummingbot-20240530/hummingbot/connector/gateway/amm_perpetual/gateway_evm_amm_perpetual.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/gateway/clob_perp/data_sources/clob_perp_api_data_source_base.py` & `hummingbot-20240530/hummingbot/connector/gateway/clob_perp/data_sources/clob_perp_api_data_source_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/gateway/clob_perp/gateway_clob_perp.py` & `hummingbot-20240530/hummingbot/connector/gateway/clob_perp/gateway_clob_perp.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/gateway/clob_perp/gateway_clob_perp_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/gateway/clob_perp/gateway_clob_perp_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/gateway/clob_spot/data_sources/clob_api_data_source_base.py` & `hummingbot-20240530/hummingbot/connector/gateway/clob_spot/data_sources/clob_api_data_source_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/dexalot_api_data_source.py` & `hummingbot-20240530/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/dexalot_api_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/dexalot_auth.py` & `hummingbot-20240530/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/dexalot_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/dexalot_constants.py` & `hummingbot-20240530/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/dexalot_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/dexalot_web_utils.py` & `hummingbot-20240530/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/dexalot_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/gateway/clob_spot/data_sources/gateway_clob_api_data_source_base.py` & `hummingbot-20240530/hummingbot/connector/gateway/clob_spot/data_sources/gateway_clob_api_data_source_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/gateway/clob_spot/data_sources/kujira/kujira_api_data_source.py` & `hummingbot-20240530/hummingbot/connector/gateway/clob_spot/data_sources/kujira/kujira_api_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/gateway/clob_spot/data_sources/kujira/kujira_helpers.py` & `hummingbot-20240530/hummingbot/connector/gateway/clob_spot/data_sources/kujira/kujira_helpers.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/gateway/clob_spot/data_sources/kujira/kujira_types.py` & `hummingbot-20240530/hummingbot/connector/gateway/clob_spot/data_sources/kujira/kujira_types.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/gateway/clob_spot/data_sources/xrpl/xrpl_api_data_source.py` & `hummingbot-20240530/hummingbot/connector/gateway/clob_spot/data_sources/xrpl/xrpl_api_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/gateway/clob_spot/data_sources/xrpl/xrpl_constants.py` & `hummingbot-20240530/hummingbot/connector/gateway/clob_spot/data_sources/xrpl/xrpl_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/gateway/clob_spot/gateway_clob_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/gateway/clob_spot/gateway_clob_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/gateway/clob_spot/gateway_clob_spot.py` & `hummingbot-20240530/hummingbot/connector/gateway/clob_spot/gateway_clob_spot.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/gateway/common_types.py` & `hummingbot-20240530/hummingbot/connector/gateway/common_types.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/gateway/gateway_in_flight_order.py` & `hummingbot-20240530/hummingbot/connector/gateway/gateway_in_flight_order.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/gateway/gateway_order_tracker.py` & `hummingbot-20240530/hummingbot/connector/gateway/gateway_order_tracker.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/gateway/gateway_price_shim.py` & `hummingbot-20240530/hummingbot/connector/gateway/gateway_price_shim.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/in_flight_order_base.cpp` & `hummingbot-20240530/hummingbot/connector/in_flight_order_base.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/markets_recorder.py` & `hummingbot-20240530/hummingbot/connector/markets_recorder.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/parrot.py` & `hummingbot-20240530/hummingbot/connector/parrot.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/perpetual_derivative_py_base.py` & `hummingbot-20240530/hummingbot/connector/perpetual_derivative_py_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/perpetual_trading.py` & `hummingbot-20240530/hummingbot/connector/perpetual_trading.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/test_support/exchange_connector_test.py` & `hummingbot-20240530/hummingbot/connector/test_support/exchange_connector_test.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/test_support/gateway_clob_api_data_source_test.py` & `hummingbot-20240530/hummingbot/connector/test_support/gateway_clob_api_data_source_test.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/test_support/mock_order_tracker.py` & `hummingbot-20240530/hummingbot/connector/test_support/mock_order_tracker.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/test_support/mock_paper_exchange.cpp` & `hummingbot-20240530/hummingbot/connector/test_support/mock_paper_exchange.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/test_support/network_mocking_assistant.py` & `hummingbot-20240530/hummingbot/connector/test_support/network_mocking_assistant.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/test_support/oms_exchange_connector_test.py` & `hummingbot-20240530/hummingbot/connector/test_support/oms_exchange_connector_test.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/test_support/perpetual_derivative_test.py` & `hummingbot-20240530/hummingbot/connector/test_support/perpetual_derivative_test.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/time_synchronizer.py` & `hummingbot-20240530/hummingbot/connector/time_synchronizer.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/trading_rule.cpp` & `hummingbot-20240530/hummingbot/connector/trading_rule.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/utilities/oms_connector/oms_connector_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/connector/utilities/oms_connector/oms_connector_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/utilities/oms_connector/oms_connector_api_user_stream_data_source.py` & `hummingbot-20240530/hummingbot/connector/utilities/oms_connector/oms_connector_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/utilities/oms_connector/oms_connector_auth.py` & `hummingbot-20240530/hummingbot/connector/utilities/oms_connector/oms_connector_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/utilities/oms_connector/oms_connector_constants.py` & `hummingbot-20240530/hummingbot/connector/utilities/oms_connector/oms_connector_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/utilities/oms_connector/oms_connector_exchange.py` & `hummingbot-20240530/hummingbot/connector/utilities/oms_connector/oms_connector_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/utilities/oms_connector/oms_connector_utils.py` & `hummingbot-20240530/hummingbot/connector/utilities/oms_connector/oms_connector_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/utilities/oms_connector/oms_connector_web_utils.py` & `hummingbot-20240530/hummingbot/connector/utilities/oms_connector/oms_connector_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/connector/utils.py` & `hummingbot-20240530/hummingbot/connector/utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/api_throttler/async_request_context_base.py` & `hummingbot-20240530/hummingbot/core/api_throttler/async_request_context_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/api_throttler/async_throttler.py` & `hummingbot-20240530/hummingbot/core/api_throttler/async_throttler.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/api_throttler/async_throttler_base.py` & `hummingbot-20240530/hummingbot/core/api_throttler/async_throttler_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/api_throttler/data_types.py` & `hummingbot-20240530/hummingbot/core/api_throttler/data_types.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/clock.cpp` & `hummingbot-20240530/hummingbot/core/clock.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/cpp/LimitOrder.cpp` & `hummingbot-20240530/hummingbot/core/cpp/LimitOrder.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/cpp/LimitOrder.h` & `hummingbot-20240530/hummingbot/core/cpp/LimitOrder.h`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/cpp/OrderBookEntry.cpp` & `hummingbot-20240530/hummingbot/core/cpp/OrderBookEntry.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/cpp/OrderBookEntry.h` & `hummingbot-20240530/hummingbot/core/cpp/OrderBookEntry.h`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/cpp/OrderExpirationEntry.cpp` & `hummingbot-20240530/hummingbot/core/cpp/OrderExpirationEntry.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/cpp/OrderExpirationEntry.h` & `hummingbot-20240530/hummingbot/core/cpp/OrderExpirationEntry.h`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/cpp/PyRef.cpp` & `hummingbot-20240530/hummingbot/core/cpp/PyRef.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/cpp/TestOrderBookEntry.cpp` & `hummingbot-20240530/hummingbot/core/cpp/TestOrderBookEntry.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/data_type/common.py` & `hummingbot-20240530/hummingbot/core/data_type/common.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/data_type/composite_order_book.cpp` & `hummingbot-20240530/hummingbot/core/data_type/composite_order_book.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/data_type/funding_info.py` & `hummingbot-20240530/hummingbot/core/data_type/funding_info.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/data_type/in_flight_order.py` & `hummingbot-20240530/hummingbot/core/data_type/in_flight_order.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/data_type/limit_order.cpp` & `hummingbot-20240530/hummingbot/core/data_type/limit_order.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/data_type/market_order.py` & `hummingbot-20240530/hummingbot/core/data_type/market_order.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/data_type/order_book.cpp` & `hummingbot-20240530/hummingbot/core/data_type/order_book.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/data_type/order_book_message.py` & `hummingbot-20240530/hummingbot/core/data_type/order_book_message.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/data_type/order_book_query_result.cpp` & `hummingbot-20240530/hummingbot/core/data_type/order_book_query_result.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/data_type/order_book_row.py` & `hummingbot-20240530/hummingbot/core/data_type/order_book_row.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/data_type/order_book_tracker.py` & `hummingbot-20240530/hummingbot/core/data_type/order_book_tracker.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/data_type/order_book_tracker_data_source.py` & `hummingbot-20240530/hummingbot/core/data_type/order_book_tracker_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/data_type/order_book_tracker_entry.py` & `hummingbot-20240530/hummingbot/core/data_type/order_book_tracker_entry.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/data_type/order_candidate.py` & `hummingbot-20240530/hummingbot/core/data_type/order_candidate.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/data_type/order_expiration_entry.cpp` & `hummingbot-20240530/hummingbot/core/data_type/order_expiration_entry.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/data_type/perpetual_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/core/data_type/perpetual_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/data_type/remote_api_order_book_data_source.py` & `hummingbot-20240530/hummingbot/core/data_type/remote_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/data_type/trade.py` & `hummingbot-20240530/hummingbot/core/data_type/trade.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/data_type/trade_fee.py` & `hummingbot-20240530/hummingbot/core/data_type/trade_fee.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/data_type/transaction_tracker.cpp` & `hummingbot-20240530/hummingbot/core/data_type/transaction_tracker.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/data_type/user_stream_tracker.py` & `hummingbot-20240530/hummingbot/core/data_type/user_stream_tracker.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/data_type/user_stream_tracker_data_source.py` & `hummingbot-20240530/hummingbot/core/data_type/user_stream_tracker_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/event/event_forwarder.py` & `hummingbot-20240530/hummingbot/core/event/event_forwarder.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/event/event_listener.cpp` & `hummingbot-20240530/hummingbot/core/event/event_listener.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/event/event_logger.cpp` & `hummingbot-20240530/hummingbot/core/event/event_logger.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/event/event_reporter.cpp` & `hummingbot-20240530/hummingbot/core/event/event_reporter.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/event/events.py` & `hummingbot-20240530/hummingbot/core/event/events.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/gateway/__init__.py` & `hummingbot-20240530/hummingbot/core/gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/gateway/gateway_http_client.py` & `hummingbot-20240530/hummingbot/core/gateway/gateway_http_client.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/gateway/gateway_status_monitor.py` & `hummingbot-20240530/hummingbot/core/gateway/gateway_status_monitor.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/gateway/utils.py` & `hummingbot-20240530/hummingbot/core/gateway/utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/management/console.py` & `hummingbot-20240530/hummingbot/core/management/console.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/management/diagnosis.py` & `hummingbot-20240530/hummingbot/core/management/diagnosis.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/mock_api/mock_mqtt_server.py` & `hummingbot-20240530/hummingbot/core/mock_api/mock_mqtt_server.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/mock_api/mock_web_server.py` & `hummingbot-20240530/hummingbot/core/mock_api/mock_web_server.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/mock_api/mock_web_socket_server.py` & `hummingbot-20240530/hummingbot/core/mock_api/mock_web_socket_server.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/network_base.py` & `hummingbot-20240530/hummingbot/core/network_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/network_iterator.cpp` & `hummingbot-20240530/hummingbot/core/network_iterator.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/pubsub.cpp` & `hummingbot-20240530/hummingbot/core/pubsub.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/py_time_iterator.cpp` & `hummingbot-20240530/hummingbot/core/py_time_iterator.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/rate_oracle/rate_oracle.py` & `hummingbot-20240530/hummingbot/core/rate_oracle/rate_oracle.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/rate_oracle/sources/ascend_ex_rate_source.py` & `hummingbot-20240530/hummingbot/core/rate_oracle/sources/ascend_ex_rate_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/rate_oracle/sources/binance_rate_source.py` & `hummingbot-20240530/hummingbot/core/rate_oracle/sources/binance_rate_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/rate_oracle/sources/binance_us_rate_source.py` & `hummingbot-20240530/hummingbot/core/rate_oracle/sources/binance_us_rate_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/rate_oracle/sources/coin_cap_rate_source.py` & `hummingbot-20240530/hummingbot/core/rate_oracle/sources/coin_cap_rate_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/rate_oracle/sources/coin_gecko_rate_source.py` & `hummingbot-20240530/hummingbot/core/rate_oracle/sources/coin_gecko_rate_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/rate_oracle/sources/coinbase_advanced_trade_rate_source.py` & `hummingbot-20240530/hummingbot/core/rate_oracle/sources/coinbase_advanced_trade_rate_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/rate_oracle/sources/cube_rate_source.py` & `hummingbot-20240530/hummingbot/core/rate_oracle/sources/cube_rate_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/rate_oracle/sources/gate_io_rate_source.py` & `hummingbot-20240530/hummingbot/core/rate_oracle/sources/gate_io_rate_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/rate_oracle/sources/kucoin_rate_source.py` & `hummingbot-20240530/hummingbot/core/rate_oracle/sources/kucoin_rate_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/rate_oracle/sources/rate_source_base.py` & `hummingbot-20240530/hummingbot/core/rate_oracle/sources/rate_source_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/rate_oracle/utils.py` & `hummingbot-20240530/hummingbot/core/rate_oracle/utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/time_iterator.cpp` & `hummingbot-20240530/hummingbot/core/time_iterator.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/utils/__init__.py` & `hummingbot-20240530/hummingbot/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/utils/async_call_scheduler.py` & `hummingbot-20240530/hummingbot/core/utils/async_call_scheduler.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/utils/async_retry.py` & `hummingbot-20240530/hummingbot/core/utils/async_retry.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/utils/async_utils.py` & `hummingbot-20240530/hummingbot/core/utils/async_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/utils/estimate_fee.py` & `hummingbot-20240530/hummingbot/core/utils/estimate_fee.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/utils/fixed_rate_source.py` & `hummingbot-20240530/hummingbot/core/utils/fixed_rate_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/utils/gateway_config_utils.py` & `hummingbot-20240530/hummingbot/core/utils/gateway_config_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/utils/kill_switch.py` & `hummingbot-20240530/hummingbot/core/utils/kill_switch.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/utils/market_price.py` & `hummingbot-20240530/hummingbot/core/utils/market_price.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/utils/ssl_cert.py` & `hummingbot-20240530/hummingbot/core/utils/ssl_cert.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/utils/ssl_client_request.py` & `hummingbot-20240530/hummingbot/core/utils/ssl_client_request.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/utils/tracking_nonce.py` & `hummingbot-20240530/hummingbot/core/utils/tracking_nonce.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/utils/trading_pair_fetcher.py` & `hummingbot-20240530/hummingbot/core/utils/trading_pair_fetcher.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/web_assistant/auth.py` & `hummingbot-20240530/hummingbot/core/web_assistant/auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/web_assistant/connections/connections_factory.py` & `hummingbot-20240530/hummingbot/core/web_assistant/connections/connections_factory.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/web_assistant/connections/data_types.py` & `hummingbot-20240530/hummingbot/core/web_assistant/connections/data_types.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/web_assistant/connections/rest_connection.py` & `hummingbot-20240530/hummingbot/core/web_assistant/connections/rest_connection.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/web_assistant/connections/ws_connection.py` & `hummingbot-20240530/hummingbot/core/web_assistant/connections/ws_connection.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/web_assistant/rest_assistant.py` & `hummingbot-20240530/hummingbot/core/web_assistant/rest_assistant.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/web_assistant/web_assistants_factory.py` & `hummingbot-20240530/hummingbot/core/web_assistant/web_assistants_factory.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/core/web_assistant/ws_assistant.py` & `hummingbot-20240530/hummingbot/core/web_assistant/ws_assistant.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/data_feed/amm_gateway_data_feed.py` & `hummingbot-20240530/hummingbot/data_feed/amm_gateway_data_feed.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/data_feed/candles_feed/ascend_ex_spot_candles/ascend_ex_spot_candles.py` & `hummingbot-20240530/hummingbot/data_feed/candles_feed/ascend_ex_spot_candles/ascend_ex_spot_candles.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/data_feed/candles_feed/ascend_ex_spot_candles/constants.py` & `hummingbot-20240530/hummingbot/data_feed/candles_feed/ascend_ex_spot_candles/constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/data_feed/candles_feed/binance_perpetual_candles/binance_perpetual_candles.py` & `hummingbot-20240530/hummingbot/data_feed/candles_feed/binance_perpetual_candles/binance_perpetual_candles.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/data_feed/candles_feed/binance_perpetual_candles/constants.py` & `hummingbot-20240530/hummingbot/data_feed/candles_feed/binance_perpetual_candles/constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/data_feed/candles_feed/binance_spot_candles/binance_spot_candles.py` & `hummingbot-20240530/hummingbot/data_feed/candles_feed/binance_spot_candles/binance_spot_candles.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,23 +78,23 @@
         return np.array(candles)[:, [0, 1, 2, 3, 4, 5, 7, 8, 9, 10]].astype(float)
 
     async def fill_historical_candles(self):
         max_request_needed = (self._candles.maxlen // 1000) + 1
         requests_executed = 0
         while not self.ready:
             missing_records = self._candles.maxlen - len(self._candles)
-            end_timestamp = int(self._candles[-1][0])
+            end_timestamp = int(self._candles[0][0])
             try:
                 if requests_executed < max_request_needed:
                     # we have to add one more since, the last row is not going to be included
                     candles = await self.fetch_candles(end_time=end_timestamp, limit=missing_records + 1)
                     # we are computing again the quantity of records again since the websocket process is able to
                     # modify the deque and if we extend it, the new observations are going to be dropped.
                     missing_records = self._candles.maxlen - len(self._candles)
-                    self._candles.extendleft(candles[-(missing_records + 1):-1])
+                    self._candles.extendleft(candles[-(missing_records + 1):-1][::-1])
                     requests_executed += 1
                 else:
                     self.logger().error(f"There is no data available for the quantity of "
                                         f"candles requested for {self.name}.")
                     raise
             except asyncio.CancelledError:
                 raise
```

### Comparing `hummingbot-20240527/hummingbot/data_feed/candles_feed/binance_spot_candles/constants.py` & `hummingbot-20240530/hummingbot/data_feed/candles_feed/binance_spot_candles/constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/data_feed/candles_feed/candles_base.py` & `hummingbot-20240530/hummingbot/data_feed/candles_feed/candles_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,17 +138,16 @@
 
     async def get_historical_candles(self, config: HistoricalCandlesConfig):
         try:
             all_candles = []
             current_start_time = config.start_time
             while current_start_time <= config.end_time:
                 fetched_candles = await self.fetch_candles(start_time=current_start_time)
-                if fetched_candles.size == 0:
+                if fetched_candles.size <= 1:
                     break
-
                 all_candles.append(fetched_candles)
                 last_timestamp = fetched_candles[-1][0]  # Assuming the first column is the timestamp
                 current_start_time = int(last_timestamp)
 
             final_candles = np.concatenate(all_candles, axis=0) if all_candles else np.array([])
             candles_df = pd.DataFrame(final_candles, columns=self.columns)
             candles_df.drop_duplicates(subset=["timestamp"], inplace=True)
```

### Comparing `hummingbot-20240527/hummingbot/data_feed/candles_feed/candles_factory.py` & `hummingbot-20240530/hummingbot/data_feed/candles_feed/candles_factory.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/data_feed/candles_feed/data_types.py` & `hummingbot-20240530/hummingbot/data_feed/candles_feed/data_types.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/data_feed/candles_feed/gate_io_perpetual_candles/constants.py` & `hummingbot-20240530/hummingbot/data_feed/candles_feed/gate_io_perpetual_candles/constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/data_feed/candles_feed/gate_io_perpetual_candles/gate_io_perpetual_candles.py` & `hummingbot-20240530/hummingbot/data_feed/candles_feed/gate_io_perpetual_candles/gate_io_perpetual_candles.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/data_feed/candles_feed/gate_io_spot_candles/constants.py` & `hummingbot-20240530/hummingbot/data_feed/candles_feed/gate_io_spot_candles/constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/data_feed/candles_feed/gate_io_spot_candles/gate_io_spot_candles.py` & `hummingbot-20240530/hummingbot/data_feed/candles_feed/gate_io_spot_candles/gate_io_spot_candles.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/data_feed/candles_feed/kraken_spot_candles/constants.py` & `hummingbot-20240530/hummingbot/data_feed/candles_feed/kraken_spot_candles/constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/data_feed/candles_feed/kraken_spot_candles/kraken_spot_candles.py` & `hummingbot-20240530/hummingbot/data_feed/candles_feed/kraken_spot_candles/kraken_spot_candles.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/data_feed/candles_feed/kucoin_spot_candles/constants.py` & `hummingbot-20240530/hummingbot/data_feed/candles_feed/kucoin_spot_candles/constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/data_feed/candles_feed/kucoin_spot_candles/kucoin_spot_candles.py` & `hummingbot-20240530/hummingbot/data_feed/candles_feed/kucoin_spot_candles/kucoin_spot_candles.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/data_feed/candles_feed/okx_perpetual_candles/constants.py` & `hummingbot-20240530/hummingbot/data_feed/candles_feed/okx_perpetual_candles/constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/data_feed/candles_feed/okx_perpetual_candles/okx_perpetual_candles.py` & `hummingbot-20240530/hummingbot/data_feed/candles_feed/okx_perpetual_candles/okx_perpetual_candles.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/data_feed/candles_feed/okx_spot_candles/constants.py` & `hummingbot-20240530/hummingbot/data_feed/candles_feed/okx_spot_candles/constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/data_feed/candles_feed/okx_spot_candles/okx_spot_candles.py` & `hummingbot-20240530/hummingbot/data_feed/candles_feed/okx_spot_candles/okx_spot_candles.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/data_feed/coin_cap_data_feed/coin_cap_constants.py` & `hummingbot-20240530/hummingbot/data_feed/coin_cap_data_feed/coin_cap_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/data_feed/coin_cap_data_feed/coin_cap_data_feed.py` & `hummingbot-20240530/hummingbot/data_feed/coin_cap_data_feed/coin_cap_data_feed.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/data_feed/coin_gecko_data_feed/coin_gecko_constants.py` & `hummingbot-20240530/hummingbot/data_feed/coin_gecko_data_feed/coin_gecko_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/data_feed/coin_gecko_data_feed/coin_gecko_data_feed.py` & `hummingbot-20240530/hummingbot/data_feed/coin_gecko_data_feed/coin_gecko_data_feed.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/data_feed/custom_api_data_feed.py` & `hummingbot-20240530/hummingbot/data_feed/custom_api_data_feed.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/data_feed/data_feed_base.py` & `hummingbot-20240530/hummingbot/data_feed/data_feed_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/data_feed/liquidations_feed/binance/binance_liquidations.py` & `hummingbot-20240530/hummingbot/data_feed/liquidations_feed/binance/binance_liquidations.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/data_feed/liquidations_feed/binance/constants.py` & `hummingbot-20240530/hummingbot/data_feed/liquidations_feed/binance/constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/data_feed/liquidations_feed/liquidations_base.py` & `hummingbot-20240530/hummingbot/data_feed/liquidations_feed/liquidations_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/data_feed/liquidations_feed/liquidations_factory.py` & `hummingbot-20240530/hummingbot/data_feed/liquidations_feed/liquidations_factory.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/data_feed/market_data_provider.py` & `hummingbot-20240530/hummingbot/data_feed/market_data_provider.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/data_feed/wallet_tracker_data_feed.py` & `hummingbot-20240530/hummingbot/data_feed/wallet_tracker_data_feed.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/exceptions.py` & `hummingbot-20240530/hummingbot/exceptions.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/logger/__init__.py` & `hummingbot-20240530/hummingbot/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/logger/application_warning.py` & `hummingbot-20240530/hummingbot/logger/application_warning.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/logger/cli_handler.py` & `hummingbot-20240530/hummingbot/logger/cli_handler.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/logger/log_server_client.py` & `hummingbot-20240530/hummingbot/logger/log_server_client.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/logger/logger.py` & `hummingbot-20240530/hummingbot/logger/logger.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/logger/struct_logger.py` & `hummingbot-20240530/hummingbot/logger/struct_logger.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/model/__init__.py` & `hummingbot-20240530/hummingbot/model/__init__.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/model/db_migration/base_transformation.py` & `hummingbot-20240530/hummingbot/model/db_migration/base_transformation.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/model/db_migration/migrator.py` & `hummingbot-20240530/hummingbot/model/db_migration/migrator.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/model/db_migration/transformations.py` & `hummingbot-20240530/hummingbot/model/db_migration/transformations.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/model/decimal_type_decorator.py` & `hummingbot-20240530/hummingbot/model/decimal_type_decorator.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/model/executors.py` & `hummingbot-20240530/hummingbot/model/executors.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/model/funding_payment.py` & `hummingbot-20240530/hummingbot/model/funding_payment.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/model/inventory_cost.py` & `hummingbot-20240530/hummingbot/model/inventory_cost.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/model/market_data.py` & `hummingbot-20240530/hummingbot/model/market_data.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/model/market_state.py` & `hummingbot-20240530/hummingbot/model/market_state.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/model/order.py` & `hummingbot-20240530/hummingbot/model/order.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/model/order_status.py` & `hummingbot-20240530/hummingbot/model/order_status.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/model/range_position_collected_fees.py` & `hummingbot-20240530/hummingbot/model/range_position_collected_fees.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/model/range_position_update.py` & `hummingbot-20240530/hummingbot/model/range_position_update.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/model/sql_connection_manager.py` & `hummingbot-20240530/hummingbot/model/sql_connection_manager.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/model/trade_fill.py` & `hummingbot-20240530/hummingbot/model/trade_fill.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/model/transaction_base.py` & `hummingbot-20240530/hummingbot/model/transaction_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/notifier/telegram_notifier.py` & `hummingbot-20240530/hummingbot/notifier/telegram_notifier.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/pmm_script/pmm_script_base.py` & `hummingbot-20240530/hummingbot/pmm_script/pmm_script_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/pmm_script/pmm_script_interface.py` & `hummingbot-20240530/hummingbot/pmm_script/pmm_script_interface.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/pmm_script/pmm_script_iterator.cpp` & `hummingbot-20240530/hummingbot/pmm_script/pmm_script_iterator.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/pmm_script/pmm_script_process.py` & `hummingbot-20240530/hummingbot/pmm_script/pmm_script_process.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/remote_iface/messages.py` & `hummingbot-20240530/hummingbot/remote_iface/messages.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/remote_iface/mqtt.py` & `hummingbot-20240530/hummingbot/remote_iface/mqtt.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/__utils__/ring_buffer.cpp` & `hummingbot-20240530/hummingbot/strategy/__utils__/ring_buffer.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/__utils__/trailing_indicators/base_trailing_indicator.py` & `hummingbot-20240530/hummingbot/strategy/__utils__/trailing_indicators/base_trailing_indicator.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/__utils__/trailing_indicators/exponential_moving_average.py` & `hummingbot-20240530/hummingbot/strategy/__utils__/trailing_indicators/exponential_moving_average.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/__utils__/trailing_indicators/historical_volatility.py` & `hummingbot-20240530/hummingbot/strategy/__utils__/trailing_indicators/historical_volatility.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/__utils__/trailing_indicators/instant_volatility.py` & `hummingbot-20240530/hummingbot/strategy/__utils__/trailing_indicators/instant_volatility.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/__utils__/trailing_indicators/trading_intensity.cpp` & `hummingbot-20240530/hummingbot/strategy/__utils__/trailing_indicators/trading_intensity.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 {
     "distutils": {
         "depends": [
             "hummingbot/core/cpp/OrderBookEntry.h",
             "hummingbot/core/cpp/PyRef.h"
         ],
         "include_dirs": [
-            "hummingbot/core",
-            "hummingbot/core/data_type"
+            "hummingbot/core/data_type",
+            "hummingbot/core"
         ],
         "language": "c++",
         "name": "hummingbot.strategy.__utils__.trailing_indicators.trading_intensity",
         "sources": [
             "hummingbot/strategy/__utils__/trailing_indicators/trading_intensity.pyx",
             "hummingbot/core/cpp/OrderBookEntry.cpp"
         ]
```

### Comparing `hummingbot-20240527/hummingbot/strategy/amm_arb/amm_arb.py` & `hummingbot-20240530/hummingbot/strategy/amm_arb/amm_arb.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/amm_arb/amm_arb_config_map.py` & `hummingbot-20240530/hummingbot/strategy/amm_arb/amm_arb_config_map.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/amm_arb/data_types.py` & `hummingbot-20240530/hummingbot/strategy/amm_arb/data_types.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/amm_arb/dummy.cpp` & `hummingbot-20240530/hummingbot/strategy/amm_arb/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/amm_arb/start.py` & `hummingbot-20240530/hummingbot/strategy/amm_arb/start.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/amm_arb/utils.py` & `hummingbot-20240530/hummingbot/strategy/amm_arb/utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/amm_v3_lp/amm_v3_lp.py` & `hummingbot-20240530/hummingbot/strategy/amm_v3_lp/amm_v3_lp.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/amm_v3_lp/amm_v3_lp_config_map.py` & `hummingbot-20240530/hummingbot/strategy/amm_v3_lp/amm_v3_lp_config_map.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/amm_v3_lp/start.py` & `hummingbot-20240530/hummingbot/strategy/amm_v3_lp/start.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/api_asset_price_delegate.cpp` & `hummingbot-20240530/hummingbot/strategy/api_asset_price_delegate.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/asset_price_delegate.cpp` & `hummingbot-20240530/hummingbot/strategy/asset_price_delegate.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/avellaneda_market_making/avellaneda_market_making.cpp` & `hummingbot-20240530/hummingbot/strategy/avellaneda_market_making/avellaneda_market_making.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/avellaneda_market_making/avellaneda_market_making_config_map_pydantic.py` & `hummingbot-20240530/hummingbot/strategy/avellaneda_market_making/avellaneda_market_making_config_map_pydantic.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/avellaneda_market_making/start.py` & `hummingbot-20240530/hummingbot/strategy/avellaneda_market_making/start.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/conditional_execution_state.py` & `hummingbot-20240530/hummingbot/strategy/conditional_execution_state.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/cross_exchange_market_making/cross_exchange_market_making.py` & `hummingbot-20240530/hummingbot/strategy/cross_exchange_market_making/cross_exchange_market_making.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/cross_exchange_market_making/cross_exchange_market_making_config_map_pydantic.py` & `hummingbot-20240530/hummingbot/strategy/cross_exchange_market_making/cross_exchange_market_making_config_map_pydantic.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/cross_exchange_market_making/order_id_market_pair_tracker.cpp` & `hummingbot-20240530/hummingbot/strategy/cross_exchange_market_making/order_id_market_pair_tracker.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/cross_exchange_market_making/start.py` & `hummingbot-20240530/hummingbot/strategy/cross_exchange_market_making/start.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/cross_exchange_mining/cross_exchange_mining.cpp` & `hummingbot-20240530/hummingbot/strategy/cross_exchange_mining/cross_exchange_mining.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
     "distutils": {
         "depends": [
             "hummingbot/core/cpp/LimitOrder.h",
             "hummingbot/core/cpp/OrderBookEntry.h",
             "hummingbot/core/cpp/PyRef.h"
         ],
         "include_dirs": [
-            "hummingbot/core/data_type",
-            "hummingbot/core"
+            "hummingbot/core",
+            "hummingbot/core/data_type"
         ],
         "language": "c++",
         "name": "hummingbot.strategy.cross_exchange_mining.cross_exchange_mining",
         "sources": [
             "hummingbot/strategy/cross_exchange_mining/cross_exchange_mining.pyx"
         ]
     },
```

### Comparing `hummingbot-20240527/hummingbot/strategy/cross_exchange_mining/cross_exchange_mining_config_map_pydantic.py` & `hummingbot-20240530/hummingbot/strategy/cross_exchange_mining/cross_exchange_mining_config_map_pydantic.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/cross_exchange_mining/cross_exchange_mining_pair.py` & `hummingbot-20240530/hummingbot/strategy/cross_exchange_mining/cross_exchange_mining_pair.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/cross_exchange_mining/order_id_market_pair_tracker.cpp` & `hummingbot-20240530/hummingbot/strategy/cross_exchange_mining/order_id_market_pair_tracker.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/cross_exchange_mining/start.py` & `hummingbot-20240530/hummingbot/strategy/cross_exchange_mining/start.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/data_types.py` & `hummingbot-20240530/hummingbot/strategy/data_types.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/directional_strategy_base.py` & `hummingbot-20240530/hummingbot/strategy/directional_strategy_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/hanging_orders_tracker.py` & `hummingbot-20240530/hummingbot/strategy/hanging_orders_tracker.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/hedge/hedge.py` & `hummingbot-20240530/hummingbot/strategy/hedge/hedge.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/hedge/hedge_config_map_pydantic.py` & `hummingbot-20240530/hummingbot/strategy/hedge/hedge_config_map_pydantic.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/hedge/start.py` & `hummingbot-20240530/hummingbot/strategy/hedge/start.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/liquidity_mining/data_types.py` & `hummingbot-20240530/hummingbot/strategy/liquidity_mining/data_types.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/liquidity_mining/dummy.cpp` & `hummingbot-20240530/hummingbot/strategy/liquidity_mining/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/liquidity_mining/liquidity_mining.py` & `hummingbot-20240530/hummingbot/strategy/liquidity_mining/liquidity_mining.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/liquidity_mining/liquidity_mining_config_map.py` & `hummingbot-20240530/hummingbot/strategy/liquidity_mining/liquidity_mining_config_map.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/liquidity_mining/start.py` & `hummingbot-20240530/hummingbot/strategy/liquidity_mining/start.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/maker_taker_market_pair.py` & `hummingbot-20240530/hummingbot/strategy/maker_taker_market_pair.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/market_trading_pair_tuple.py` & `hummingbot-20240530/hummingbot/strategy/market_trading_pair_tuple.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/order_book_asset_price_delegate.cpp` & `hummingbot-20240530/hummingbot/strategy/order_book_asset_price_delegate.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/order_tracker.cpp` & `hummingbot-20240530/hummingbot/strategy/order_tracker.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 {
     "distutils": {
         "depends": [
             "hummingbot/core/cpp/LimitOrder.h",
             "hummingbot/core/cpp/PyRef.h"
         ],
         "include_dirs": [
-            "hummingbot/core",
-            "hummingbot/core/data_type"
+            "hummingbot/core/data_type",
+            "hummingbot/core"
         ],
         "language": "c++",
         "name": "hummingbot.strategy.order_tracker",
         "sources": [
             "hummingbot/strategy/order_tracker.pyx"
         ]
     },
```

### Comparing `hummingbot-20240527/hummingbot/strategy/perpetual_market_making/data_types.py` & `hummingbot-20240530/hummingbot/strategy/perpetual_market_making/data_types.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/perpetual_market_making/dummy.cpp` & `hummingbot-20240530/hummingbot/strategy/perpetual_market_making/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/perpetual_market_making/perpetual_market_making.py` & `hummingbot-20240530/hummingbot/strategy/perpetual_market_making/perpetual_market_making.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/perpetual_market_making/perpetual_market_making_config_map.py` & `hummingbot-20240530/hummingbot/strategy/perpetual_market_making/perpetual_market_making_config_map.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/perpetual_market_making/perpetual_market_making_order_tracker.py` & `hummingbot-20240530/hummingbot/strategy/perpetual_market_making/perpetual_market_making_order_tracker.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/perpetual_market_making/start.py` & `hummingbot-20240530/hummingbot/strategy/perpetual_market_making/start.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/pure_market_making/data_types.py` & `hummingbot-20240530/hummingbot/strategy/pure_market_making/data_types.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/pure_market_making/inventory_cost_price_delegate.py` & `hummingbot-20240530/hummingbot/strategy/pure_market_making/inventory_cost_price_delegate.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/pure_market_making/inventory_skew_calculator.cpp` & `hummingbot-20240530/hummingbot/strategy/pure_market_making/inventory_skew_calculator.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/pure_market_making/moving_price_band.py` & `hummingbot-20240530/hummingbot/strategy/pure_market_making/moving_price_band.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/pure_market_making/pure_market_making.cpp` & `hummingbot-20240530/hummingbot/strategy/pure_market_making/pure_market_making.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/pure_market_making/pure_market_making_config_map.py` & `hummingbot-20240530/hummingbot/strategy/pure_market_making/pure_market_making_config_map.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/pure_market_making/pure_market_making_order_tracker.cpp` & `hummingbot-20240530/hummingbot/strategy/pure_market_making/pure_market_making_order_tracker.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 {
     "distutils": {
         "depends": [
             "hummingbot/core/cpp/LimitOrder.h",
             "hummingbot/core/cpp/PyRef.h"
         ],
         "include_dirs": [
-            "hummingbot/core",
-            "hummingbot/core/data_type"
+            "hummingbot/core/data_type",
+            "hummingbot/core"
         ],
         "language": "c++",
         "name": "hummingbot.strategy.pure_market_making.pure_market_making_order_tracker",
         "sources": [
             "hummingbot/strategy/pure_market_making/pure_market_making_order_tracker.pyx"
         ]
     },
```

### Comparing `hummingbot-20240527/hummingbot/strategy/pure_market_making/start.py` & `hummingbot-20240530/hummingbot/strategy/pure_market_making/start.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/script_strategy_base.py` & `hummingbot-20240530/hummingbot/strategy/script_strategy_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/spot_perpetual_arbitrage/arb_proposal.py` & `hummingbot-20240530/hummingbot/strategy/spot_perpetual_arbitrage/arb_proposal.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/spot_perpetual_arbitrage/dummy.cpp` & `hummingbot-20240530/hummingbot/strategy/spot_perpetual_arbitrage/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/spot_perpetual_arbitrage/spot_perpetual_arbitrage.py` & `hummingbot-20240530/hummingbot/strategy/spot_perpetual_arbitrage/spot_perpetual_arbitrage.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/spot_perpetual_arbitrage/spot_perpetual_arbitrage_config_map.py` & `hummingbot-20240530/hummingbot/strategy/spot_perpetual_arbitrage/spot_perpetual_arbitrage_config_map.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/spot_perpetual_arbitrage/start.py` & `hummingbot-20240530/hummingbot/strategy/spot_perpetual_arbitrage/start.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/spot_perpetual_arbitrage/utils.py` & `hummingbot-20240530/hummingbot/strategy/spot_perpetual_arbitrage/utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/strategy_base.cpp` & `hummingbot-20240530/hummingbot/strategy/strategy_base.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/strategy_py_base.cpp` & `hummingbot-20240530/hummingbot/strategy/strategy_py_base.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/strategy_v2_base.py` & `hummingbot-20240530/hummingbot/strategy/strategy_v2_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/twap/dummy.cpp` & `hummingbot-20240530/hummingbot/strategy/twap/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/twap/start.py` & `hummingbot-20240530/hummingbot/strategy/twap/start.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/twap/twap.py` & `hummingbot-20240530/hummingbot/strategy/twap/twap.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/twap/twap_config_map.py` & `hummingbot-20240530/hummingbot/strategy/twap/twap_config_map.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy/utils.py` & `hummingbot-20240530/hummingbot/strategy/utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy_v2/backtesting/backtesting_data_provider.py` & `hummingbot-20240530/hummingbot/strategy_v2/backtesting/backtesting_data_provider.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy_v2/backtesting/backtesting_engine_base.py` & `hummingbot-20240530/hummingbot/strategy_v2/backtesting/backtesting_engine_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,14 +173,15 @@
                                                 direction="backward")
         backtesting_candles["timestamp"] = backtesting_candles["timestamp_bt"]
         backtesting_candles["open"] = backtesting_candles["open_bt"]
         backtesting_candles["high"] = backtesting_candles["high_bt"]
         backtesting_candles["low"] = backtesting_candles["low_bt"]
         backtesting_candles["close"] = backtesting_candles["close_bt"]
         backtesting_candles["volume"] = backtesting_candles["volume_bt"]
+        backtesting_candles.dropna(inplace=True)
         self.controller.processed_data["features"] = backtesting_candles
         return backtesting_candles
 
     def update_market_data(self, row: pd.Series):
         """
         Updates market data in the controller with the current price and timestamp.
 
@@ -271,15 +272,15 @@
 
             peak = np.maximum.accumulate(cumulative_returns)
             drawdown = (cumulative_returns - peak)
             max_draw_down = np.min(drawdown)
             max_drawdown_pct = max_draw_down / executors_with_position["inventory"].iloc[0]
             returns = pd.to_numeric(
                 executors_with_position["cumulative_returns"] / executors_with_position["cumulative_volume"])
-            sharpe_ratio = returns.mean() / returns.std()
+            sharpe_ratio = returns.mean() / returns.std() if len(returns) > 1 else 0
             total_won = win_signals.loc[:, "net_pnl_quote"].sum()
             total_loss = - loss_signals.loc[:, "net_pnl_quote"].sum()
             profit_factor = total_won / total_loss if total_loss > 0 else 1
             net_pnl_pct = net_pnl_quote / total_amount_quote
 
             return {
                 "net_pnl": float(net_pnl_pct),
```

### Comparing `hummingbot-20240527/hummingbot/strategy_v2/backtesting/executor_simulator_base.py` & `hummingbot-20240530/hummingbot/strategy_v2/backtesting/executor_simulator_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy_v2/backtesting/executors_simulator/dca_executor_simulator.py` & `hummingbot-20240530/hummingbot/strategy_v2/backtesting/executors_simulator/dca_executor_simulator.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     def simulate(self, df: pd.DataFrame, config: DCAExecutorConfig, trade_cost: float) -> ExecutorSimulation:
         if config.mode == DCAMode.TAKER:
             raise NotImplementedError("Taker mode is not supported in DCAExecutorSimulator")
         potential_dca_stages = []
         side_multiplier = 1 if config.side == TradeType.BUY else -1
         last_timestamp = df['timestamp'].max()
-        tl = config.time_limit * 1000 if config.time_limit else None
+        tl = config.time_limit if config.time_limit else None
         tl_timestamp = config.timestamp + tl if tl else last_timestamp
         # Filter dataframe based on the conditions
         df_filtered = df[df['timestamp'] <= tl_timestamp].copy()
         df_filtered['net_pnl_pct'] = 0.0
         df_filtered['net_pnl_quote'] = 0.0
         df_filtered['cum_fees_quote'] = 0.0
         df_filtered['filled_amount_quote'] = 0.0
```

### Comparing `hummingbot-20240527/hummingbot/strategy_v2/backtesting/executors_simulator/position_executor_simulator.py` & `hummingbot-20240530/hummingbot/strategy_v2/backtesting/executors_simulator/position_executor_simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         else:
             start_timestamp = df['timestamp'].min()
         last_timestamp = df['timestamp'].max()
 
         # Set up barriers
         tp = Decimal(config.triple_barrier_config.take_profit) if config.triple_barrier_config.take_profit else None
         sl = Decimal(config.triple_barrier_config.stop_loss) if config.triple_barrier_config.stop_loss else None
-        tl = config.triple_barrier_config.time_limit * 1000 if config.triple_barrier_config.time_limit else None
+        tl = config.triple_barrier_config.time_limit if config.triple_barrier_config.time_limit else None
         tl_timestamp = config.timestamp + tl if tl else last_timestamp
 
         # Filter dataframe based on the conditions
         df_filtered = df[df['timestamp'] <= tl_timestamp].copy()
         df_filtered['net_pnl_pct'] = 0.0
         df_filtered['net_pnl_quote'] = 0.0
         df_filtered['cum_fees_quote'] = 0.0
```

### Comparing `hummingbot-20240527/hummingbot/strategy_v2/controllers/__init__.py` & `hummingbot-20240530/hummingbot/strategy_v2/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy_v2/controllers/controller_base.py` & `hummingbot-20240530/hummingbot/strategy_v2/controllers/controller_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy_v2/controllers/directional_trading_controller_base.py` & `hummingbot-20240530/hummingbot/strategy_v2/controllers/directional_trading_controller_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,15 @@
         Check if an executor can be created based on the signal, the quantity of active executors and the cooldown time.
         """
         active_executors_by_signal_side = self.filter_executors(
             executors=self.executors_info,
             filter_func=lambda x: x.is_active and (x.side == TradeType.BUY if signal > 0 else TradeType.SELL))
         max_timestamp = max([executor.timestamp for executor in active_executors_by_signal_side], default=0)
         active_executors_condition = len(active_executors_by_signal_side) < self.config.max_executors_per_side
-        cooldown_condition = (self.market_data_provider.time() - max_timestamp) / 1000 > self.config.cooldown_time
+        cooldown_condition = self.market_data_provider.time() - max_timestamp > self.config.cooldown_time
         return active_executors_condition and cooldown_condition
 
     def stop_actions_proposal(self) -> List[ExecutorAction]:
         """
         Stop actions based on the provided executor handler report.
         """
         stop_actions = []
```

### Comparing `hummingbot-20240527/hummingbot/strategy_v2/controllers/market_making_controller_base.py` & `hummingbot-20240530/hummingbot/strategy_v2/controllers/market_making_controller_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,15 +252,15 @@
                     executor_config=executor_config
                 ))
         return create_actions
 
     def get_levels_to_execute(self) -> List[str]:
         working_levels = self.filter_executors(
             executors=self.executors_info,
-            filter_func=lambda x: x.is_active or (x.close_type == CloseType.STOP_LOSS and self.market_data_provider.time() - x.close_timestamp < self.config.cooldown_time * 1000)
+            filter_func=lambda x: x.is_active or (x.close_type == CloseType.STOP_LOSS and self.market_data_provider.time() - x.close_timestamp < self.config.cooldown_time)
         )
         working_levels_ids = [executor.custom_info["level_id"] for executor in working_levels]
         return self.get_not_active_levels_ids(working_levels_ids)
 
     def stop_actions_proposal(self) -> List[ExecutorAction]:
         """
         Create a list of actions to stop the executors based on order refresh and early stop conditions.
@@ -269,15 +269,15 @@
         stop_actions.extend(self.executors_to_refresh())
         stop_actions.extend(self.executors_to_early_stop())
         return stop_actions
 
     def executors_to_refresh(self) -> List[ExecutorAction]:
         executors_to_refresh = self.filter_executors(
             executors=self.executors_info,
-            filter_func=lambda x: not x.is_trading and x.is_active and self.market_data_provider.time() - x.timestamp > self.config.executor_refresh_time * 1000)
+            filter_func=lambda x: not x.is_trading and x.is_active and self.market_data_provider.time() - x.timestamp > self.config.executor_refresh_time)
 
         return [StopExecutorAction(
             controller_id=self.config.id,
             executor_id=executor.id) for executor in executors_to_refresh]
 
     def executors_to_early_stop(self) -> List[ExecutorAction]:
         """
```

### Comparing `hummingbot-20240527/hummingbot/strategy_v2/executors/arbitrage_executor/arbitrage_executor.py` & `hummingbot-20240530/hummingbot/strategy_v2/executors/arbitrage_executor/arbitrage_executor.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy_v2/executors/data_types.py` & `hummingbot-20240530/hummingbot/strategy_v2/executors/data_types.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy_v2/executors/dca_executor/data_types.py` & `hummingbot-20240530/hummingbot/strategy_v2/executors/dca_executor/data_types.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy_v2/executors/dca_executor/dca_executor.py` & `hummingbot-20240530/hummingbot/strategy_v2/executors/dca_executor/dca_executor.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy_v2/executors/executor_base.py` & `hummingbot-20240530/hummingbot/strategy_v2/executors/executor_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy_v2/executors/executor_orchestrator.py` & `hummingbot-20240530/hummingbot/strategy_v2/executors/executor_orchestrator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 from decimal import Decimal
 from typing import Dict, List
 
 from hummingbot.connector.markets_recorder import MarketsRecorder
+from hummingbot.core.data_type.common import TradeType
 from hummingbot.logger import HummingbotLogger
 from hummingbot.strategy.script_strategy_base import ScriptStrategyBase
 from hummingbot.strategy_v2.executors.arbitrage_executor.arbitrage_executor import ArbitrageExecutor
 from hummingbot.strategy_v2.executors.arbitrage_executor.data_types import ArbitrageExecutorConfig
 from hummingbot.strategy_v2.executors.dca_executor.data_types import DCAExecutorConfig
 from hummingbot.strategy_v2.executors.dca_executor.dca_executor import DCAExecutor
 from hummingbot.strategy_v2.executors.position_executor.data_types import PositionExecutorConfig
@@ -17,14 +18,15 @@
 from hummingbot.strategy_v2.executors.xemm_executor.xemm_executor import XEMMExecutor
 from hummingbot.strategy_v2.models.executor_actions import (
     CreateExecutorAction,
     ExecutorAction,
     StopExecutorAction,
     StoreExecutorAction,
 )
+from hummingbot.strategy_v2.models.executors import CloseType
 from hummingbot.strategy_v2.models.executors_info import ExecutorInfo, PerformanceReport
 
 
 class ExecutorOrchestrator:
     """
     Orchestrator for various executors.
     """
@@ -147,32 +149,45 @@
         return report
 
     def generate_performance_report(self, controller_id: str) -> PerformanceReport:
         # Fetch executors from database and active in-memory executors
         db_executors = MarketsRecorder.get_instance().get_executors_by_controller(controller_id)
         active_executor_ids = [executor.executor_info.id for executor in self.executors.get(controller_id, [])]
         filtered_db_executors = [executor for executor in db_executors if executor.id not in active_executor_ids]
-        combined_executors = self.executors.get(controller_id, []) + filtered_db_executors
+        active_executors = [executor.executor_info for executor in self.executors.get(controller_id, [])]
+        combined_executors = active_executors + filtered_db_executors
 
         # Initialize performance metrics
         realized_pnl_quote = Decimal(0)
         unrealized_pnl_quote = Decimal(0)
         volume_traded = Decimal(0)
+        open_order_volume = Decimal(0)
+        inventory_imbalance = Decimal(0)
         close_type_counts = {}
 
         for executor in combined_executors:
-            if executor.is_active:  # For active executors
-                unrealized_pnl_quote += executor.net_pnl_quote
-            else:  # For closed executors
-                realized_pnl_quote += executor.net_pnl_quote
-                close_type = executor.close_type
+            close_type = executor.close_type
+            if close_type == CloseType.FAILED:
+                continue
+            elif close_type is not None:
                 if close_type in close_type_counts:
                     close_type_counts[close_type] += 1
                 else:
                     close_type_counts[close_type] = 1
+            if executor.is_active:  # For active executors
+                unrealized_pnl_quote += executor.net_pnl_quote
+                side = executor.custom_info.get("side", None)
+                if side:
+                    inventory_imbalance += executor.filled_amount_quote if side == TradeType.BUY else -executor.filled_amount_quote
+                if executor.type == "dca_executor":
+                    open_order_volume += sum(executor.config.amounts_quote) - executor.filled_amount_quote
+                elif executor.type == "position_executor":
+                    open_order_volume += (executor.config.amount * executor.config.entry_price) - executor.filled_amount_quote
+            else:  # For closed executors
+                realized_pnl_quote += executor.net_pnl_quote
             volume_traded += executor.filled_amount_quote
 
         # Calculate global PNL values
         global_pnl_quote = unrealized_pnl_quote + realized_pnl_quote
         global_pnl_pct = (global_pnl_quote / volume_traded) * 100 if volume_traded != 0 else Decimal(0)
 
         # Calculate individual PNL percentages
@@ -184,30 +199,36 @@
             realized_pnl_quote=realized_pnl_quote,
             unrealized_pnl_quote=unrealized_pnl_quote,
             unrealized_pnl_pct=unrealized_pnl_pct,
             realized_pnl_pct=realized_pnl_pct,
             global_pnl_quote=global_pnl_quote,
             global_pnl_pct=global_pnl_pct,
             volume_traded=volume_traded,
+            open_order_volume=open_order_volume,
+            inventory_imbalance=inventory_imbalance,
             close_type_counts=close_type_counts
         )
 
         return report
 
     def generate_global_performance_report(self) -> PerformanceReport:
         global_realized_pnl_quote = Decimal(0)
         global_unrealized_pnl_quote = Decimal(0)
         global_volume_traded = Decimal(0)
+        global_open_order_volume = Decimal(0)
+        global_inventory_imbalance = Decimal(0)
         global_close_type_counts = {}
 
         for controller_id in self.executors.keys():
             report = self.generate_performance_report(controller_id)
             global_realized_pnl_quote += report.realized_pnl_quote
             global_unrealized_pnl_quote += report.unrealized_pnl_quote
             global_volume_traded += report.volume_traded
+            global_open_order_volume += report.open_order_volume
+            global_inventory_imbalance += report.inventory_imbalance
 
             for close_type, count in report.close_type_counts.items():
                 global_close_type_counts[close_type] = global_close_type_counts.get(close_type, 0) + count
 
         global_pnl_quote = global_realized_pnl_quote + global_unrealized_pnl_quote
         global_pnl_pct = (global_pnl_quote / global_volume_traded) * 100 if global_volume_traded != 0 else Decimal(0)
 
@@ -215,9 +236,11 @@
             realized_pnl_quote=global_realized_pnl_quote,
             unrealized_pnl_quote=global_unrealized_pnl_quote,
             realized_pnl_pct=(global_realized_pnl_quote / global_volume_traded) * 100 if global_volume_traded != 0 else Decimal(0),
             unrealized_pnl_pct=(global_unrealized_pnl_quote / global_volume_traded) * 100 if global_volume_traded != 0 else Decimal(0),
             global_pnl_quote=global_pnl_quote,
             global_pnl_pct=global_pnl_pct,
             volume_traded=global_volume_traded,
+            open_order_volume=global_open_order_volume,
+            inventory_imbalance=global_inventory_imbalance,
             close_type_counts=global_close_type_counts
         )
```

### Comparing `hummingbot-20240527/hummingbot/strategy_v2/executors/position_executor/data_types.py` & `hummingbot-20240530/hummingbot/strategy_v2/executors/position_executor/data_types.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy_v2/executors/position_executor/position_executor.py` & `hummingbot-20240530/hummingbot/strategy_v2/executors/position_executor/position_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import asyncio
 import logging
 import math
 from decimal import Decimal
 from typing import Dict, List, Optional, Union
 
+from hummingbot.connector.connector_base import ConnectorBase
 from hummingbot.core.data_type.common import OrderType, PositionAction, PriceType, TradeType
 from hummingbot.core.data_type.order_candidate import OrderCandidate, PerpetualOrderCandidate
 from hummingbot.core.event.events import (
     BuyOrderCompletedEvent,
     BuyOrderCreatedEvent,
     MarketOrderFailureEvent,
+    OrderCancelledEvent,
     OrderFilledEvent,
     SellOrderCompletedEvent,
     SellOrderCreatedEvent,
 )
 from hummingbot.logger import HummingbotLogger
 from hummingbot.strategy.script_strategy_base import ScriptStrategyBase
 from hummingbot.strategy_v2.executors.executor_base import ExecutorBase
@@ -281,15 +283,20 @@
         if math.isclose(self.open_filled_amount, self.close_filled_amount):
             if self.open_orders_completed():
                 self.stop()
             else:
                 self.cancel_open_orders()
                 self._current_retries += 1
         elif self._close_order:
-            self.logger().info(f"Waiting for close order to be filled --> Filled amount: {self.close_filled_amount} | Open amount: {self.open_filled_amount}")
+            if self._current_retries < self._max_retries / 2:
+                self.logger().info(f"Waiting for close order to be filled --> Filled amount: {self.close_filled_amount} | Open amount: {self.open_filled_amount}")
+            else:
+                self.logger().info("No fill on close order, will be retried.")
+                self.cancel_close_order()
+                self._current_retries += 1
         else:
             self.logger().info(f"Open amount: {self.open_filled_amount}, Close amount: {self.close_filled_amount}")
             self.place_close_order_and_cancel_open_orders(close_type=self.close_type)
             self._current_retries += 1
         await asyncio.sleep(1.0)
 
     def evaluate_max_retries(self):
@@ -509,14 +516,27 @@
         self._strategy.cancel(
             connector_name=self.config.connector_name,
             trading_pair=self.config.trading_pair,
             order_id=self._open_order.order_id
         )
         self.logger().debug("Removing open order")
 
+    def cancel_close_order(self):
+        """
+        This method is responsible for canceling the close order.
+
+        :return: None
+        """
+        self._strategy.cancel(
+            connector_name=self.config.connector_name,
+            trading_pair=self.config.trading_pair,
+            order_id=self._close_order.order_id
+        )
+        self.logger().debug("Removing close order")
+
     def early_stop(self):
         """
         This method allows strategy to stop the executor early.
 
         :return: None
         """
         self.place_close_order_and_cancel_open_orders(close_type=CloseType.EARLY_STOP)
@@ -562,14 +582,22 @@
         This method is responsible for processing the order filled event. Here we will update the value of
         _total_executed_amount_backup, that can be used if the InFlightOrder
         is not available.
         """
         self._total_executed_amount_backup += event.amount
         self.update_tracked_orders_with_order_id(event.order_id)
 
+    def process_order_canceled_event(self, _, market: ConnectorBase, event: OrderCancelledEvent):
+        """
+        This method is responsible for processing the order canceled event
+        """
+        if self._close_order and event.order_id == self._close_order.order_id:
+            self._failed_orders.append(self._close_order)
+            self._close_order = None
+
     def process_order_failed_event(self, _, market, event: MarketOrderFailureEvent):
         """
         This method is responsible for processing the order failed event. Here we will add the InFlightOrder to the
         failed orders list.
         """
         self._current_retries += 1
         if self._open_order and event.order_id == self._open_order.order_id:
```

### Comparing `hummingbot-20240527/hummingbot/strategy_v2/executors/twap_executor/data_types.py` & `hummingbot-20240530/hummingbot/strategy_v2/executors/twap_executor/data_types.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy_v2/executors/twap_executor/twap_executor.py` & `hummingbot-20240530/hummingbot/strategy_v2/executors/twap_executor/twap_executor.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy_v2/executors/xemm_executor/xemm_executor.py` & `hummingbot-20240530/hummingbot/strategy_v2/executors/xemm_executor/xemm_executor.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy_v2/models/executor_actions.py` & `hummingbot-20240530/hummingbot/strategy_v2/models/executor_actions.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy_v2/models/executors.py` & `hummingbot-20240530/hummingbot/strategy_v2/models/executors.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy_v2/models/executors_info.py` & `hummingbot-20240530/hummingbot/strategy_v2/models/executors_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,8 +69,10 @@
     realized_pnl_quote: Decimal
     unrealized_pnl_quote: Decimal
     unrealized_pnl_pct: Decimal
     realized_pnl_pct: Decimal
     global_pnl_quote: Decimal
     global_pnl_pct: Decimal
     volume_traded: Decimal
+    open_order_volume: Decimal
+    inventory_imbalance: Decimal
     close_type_counts: Dict[CloseType, int]
```

### Comparing `hummingbot-20240527/hummingbot/strategy_v2/runnable_base.py` & `hummingbot-20240530/hummingbot/strategy_v2/runnable_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy_v2/utils/config_encoder_decoder.py` & `hummingbot-20240530/hummingbot/strategy_v2/utils/config_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy_v2/utils/distributions.py` & `hummingbot-20240530/hummingbot/strategy_v2/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/strategy_v2/utils/order_level_builder.py` & `hummingbot-20240530/hummingbot/strategy_v2/utils/order_level_builder.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/templates/conf_amm_arb_strategy_TEMPLATE.yml` & `hummingbot-20240530/hummingbot/templates/conf_amm_arb_strategy_TEMPLATE.yml`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/templates/conf_amm_v3_lp_strategy_TEMPLATE.yml` & `hummingbot-20240530/hummingbot/templates/conf_amm_v3_lp_strategy_TEMPLATE.yml`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/templates/conf_fee_overrides_TEMPLATE.yml` & `hummingbot-20240530/hummingbot/templates/conf_fee_overrides_TEMPLATE.yml`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/templates/conf_liquidity_mining_strategy_TEMPLATE.yml` & `hummingbot-20240530/hummingbot/templates/conf_liquidity_mining_strategy_TEMPLATE.yml`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/templates/conf_perpetual_market_making_strategy_TEMPLATE.yml` & `hummingbot-20240530/hummingbot/templates/conf_perpetual_market_making_strategy_TEMPLATE.yml`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/templates/conf_pure_market_making_strategy_TEMPLATE.yml` & `hummingbot-20240530/hummingbot/templates/conf_pure_market_making_strategy_TEMPLATE.yml`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/templates/conf_spot_perpetual_arbitrage_strategy_TEMPLATE.yml` & `hummingbot-20240530/hummingbot/templates/conf_spot_perpetual_arbitrage_strategy_TEMPLATE.yml`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/templates/conf_twap_strategy_TEMPLATE.yml` & `hummingbot-20240530/hummingbot/templates/conf_twap_strategy_TEMPLATE.yml`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/templates/hummingbot_logs_TEMPLATE.yml` & `hummingbot-20240530/hummingbot/templates/hummingbot_logs_TEMPLATE.yml`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot/user/user_balances.py` & `hummingbot-20240530/hummingbot/user/user_balances.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot.egg-info/PKG-INFO` & `hummingbot-20240530/hummingbot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hummingbot
-Version: 20240527
+Version: 20240530
 Summary: Hummingbot
 Home-page: https://github.com/hummingbot/hummingbot
 Author: Hummingbot Foundation
 Author-email: dev@hummingbot.org
 License: Apache 2.0
 License-File: LICENSE
 Requires-Dist: bidict
```

### Comparing `hummingbot-20240527/hummingbot.egg-info/SOURCES.txt` & `hummingbot-20240530/hummingbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/hummingbot.egg-info/requires.txt` & `hummingbot-20240530/hummingbot.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/setup.py` & `hummingbot-20240530/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         if os.name != "nt" and "-Wstrict-prototypes" in self.compiler.compiler_so:
             self.compiler.compiler_so.remove("-Wstrict-prototypes")
         super().build_extensions()
 
 
 def main():
     cpu_count = os.cpu_count() or 8
-    version = "20240527"
+    version = "20240530"
     all_packages = find_packages(include=["hummingbot", "hummingbot.*"], )
     excluded_paths = [
         "hummingbot.connector.gateway.clob_spot.data_sources.injective",
         "hummingbot.connector.gateway.clob_perp.data_sources.injective_perpetual"
     ]
     packages = [pkg for pkg in all_packages if not any(fnmatch.fnmatch(pkg, pattern) for pattern in excluded_paths)]
     package_data = {
```

### Comparing `hummingbot-20240527/test/test_isolated_asyncio_wrapper_test_case.py` & `hummingbot-20240530/test/test_isolated_asyncio_wrapper_test_case.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/test/test_local_class_event_loop_wrapper_test_case.py` & `hummingbot-20240530/test/test_local_class_event_loop_wrapper_test_case.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/test/test_local_test_event_loop_wrapper_test_case.py` & `hummingbot-20240530/test/test_local_test_event_loop_wrapper_test_case.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240527/test/test_logger_mixin_for_test.py` & `hummingbot-20240530/test/test_logger_mixin_for_test.py`

 * *Files identical despite different names*

