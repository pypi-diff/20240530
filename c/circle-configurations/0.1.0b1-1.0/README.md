# Comparing `tmp/circle_configurations-0.1.0b1.tar.gz` & `tmp/circle_configurations-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circle_configurations-0.1.0b1.tar", last modified: Fri May 24 20:24:18 2024, max compression
+gzip compressed data, was "circle_configurations-1.0.tar", last modified: Thu May 30 18:20:42 2024, max compression
```

## Comparing `circle_configurations-0.1.0b1.tar` & `circle_configurations-1.0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-24 20:24:18.504130 circle_configurations-0.1.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2024-05-24 20:24:18.504130 circle_configurations-0.1.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2024-05-24 20:21:17.000000 circle_configurations-0.1.0b1/README.md
-drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-24 20:24:18.404130 circle_configurations-0.1.0b1/circle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2024-05-24 20:21:17.000000 circle_configurations-0.1.0b1/circle/__init__.py
-drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-24 20:24:18.408130 circle_configurations-0.1.0b1/circle/web3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2024-05-24 20:21:17.000000 circle_configurations-0.1.0b1/circle/web3/__init__.py
-drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-24 20:24:18.408130 circle_configurations-0.1.0b1/circle/web3/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2024-05-24 20:21:17.000000 circle_configurations-0.1.0b1/circle/web3/configurations/__init__.py
-drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-24 20:24:18.408130 circle_configurations-0.1.0b1/circle/web3/configurations/api/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2024-05-24 20:21:17.000000 circle_configurations-0.1.0b1/circle/web3/configurations/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12342 2024-05-24 20:21:17.000000 circle_configurations-0.1.0b1/circle/web3/configurations/api/developer_account_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8216 2024-05-24 20:21:17.000000 circle_configurations-0.1.0b1/circle/web3/configurations/api/faucet_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    43514 2024-05-24 20:21:17.000000 circle_configurations-0.1.0b1/circle/web3/configurations/api/monitor_tokens_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9085 2024-05-24 20:21:17.000000 circle_configurations-0.1.0b1/circle/web3/configurations/api/webhook_subscriptions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30052 2024-05-24 20:21:18.000000 circle_configurations-0.1.0b1/circle/web3/configurations/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2024-05-24 20:21:18.000000 circle_configurations-0.1.0b1/circle/web3/configurations/api_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    14649 2024-05-24 20:21:17.000000 circle_configurations-0.1.0b1/circle/web3/configurations/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2024-05-24 20:21:17.000000 circle_configurations-0.1.0b1/circle/web3/configurations/exceptions.py
-drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-24 20:24:18.416130 circle_configurations-0.1.0b1/circle/web3/configurations/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2024-05-24 20:21:17.000000 circle_configurations-0.1.0b1/circle/web3/configurations/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2024-05-24 20:21:15.000000 circle_configurations-0.1.0b1/circle/web3/configurations/models/blockchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2024-05-24 20:21:15.000000 circle_configurations-0.1.0b1/circle/web3/configurations/models/create_monitored_tokens200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2024-05-24 20:21:15.000000 circle_configurations-0.1.0b1/circle/web3/configurations/models/delete_monitored_tokens_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2024-05-24 20:21:15.000000 circle_configurations-0.1.0b1/circle/web3/configurations/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2024-05-24 20:21:15.000000 circle_configurations-0.1.0b1/circle/web3/configurations/models/faucet_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/circle/web3/configurations/models/get_entity_config200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/circle/web3/configurations/models/get_entity_config_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/circle/web3/configurations/models/get_monitored_tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/circle/web3/configurations/models/get_notification_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/circle/web3/configurations/models/get_public_key200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/circle/web3/configurations/models/get_public_key_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/circle/web3/configurations/models/list_monitored_tokens200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/circle/web3/configurations/models/list_monitored_tokens200_response_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/circle/web3/configurations/models/notification_signature_public_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/circle/web3/configurations/models/post_monitored_tokens_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/circle/web3/configurations/models/post_monitored_tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/circle/web3/configurations/models/put_monitored_tokens_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/circle/web3/configurations/models/put_monitored_tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/circle/web3/configurations/models/put_monitored_tokens_scope_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/circle/web3/configurations/models/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/circle/web3/configurations/models/testnet_blockchain.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/circle/web3/configurations/models/token_monitor_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/circle/web3/configurations/models/token_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/circle/web3/configurations/models/token_standard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/circle/web3/configurations/models/update_monitored_tokens200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2024-05-24 20:21:17.000000 circle_configurations-0.1.0b1/circle/web3/configurations/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12800 2024-05-24 20:21:18.000000 circle_configurations-0.1.0b1/circle/web3/configurations/rest.py
-drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-24 20:24:18.504130 circle_configurations-0.1.0b1/circle_configurations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2024-05-24 20:24:18.000000 circle_configurations-0.1.0b1/circle_configurations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2024-05-24 20:24:18.000000 circle_configurations-0.1.0b1/circle_configurations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2024-05-24 20:24:18.000000 circle_configurations-0.1.0b1/circle_configurations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2024-05-24 20:24:18.000000 circle_configurations-0.1.0b1/circle_configurations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2024-05-24 20:24:18.000000 circle_configurations-0.1.0b1/circle_configurations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      758 2024-05-24 20:21:17.000000 circle_configurations-0.1.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2024-05-24 20:24:18.504130 circle_configurations-0.1.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2024-05-24 20:21:17.000000 circle_configurations-0.1.0b1/setup.py
-drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-24 20:24:18.504130 circle_configurations-0.1.0b1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      688 2024-05-24 20:21:15.000000 circle_configurations-0.1.0b1/test/test_blockchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2024-05-24 20:21:15.000000 circle_configurations-0.1.0b1/test/test_create_monitored_tokens200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2024-05-24 20:21:15.000000 circle_configurations-0.1.0b1/test/test_delete_monitored_tokens_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2024-05-24 20:21:17.000000 circle_configurations-0.1.0b1/test/test_developer_account_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2024-05-24 20:21:15.000000 circle_configurations-0.1.0b1/test/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2024-05-24 20:21:17.000000 circle_configurations-0.1.0b1/test/test_faucet_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2024-05-24 20:21:15.000000 circle_configurations-0.1.0b1/test/test_faucet_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/test/test_get_entity_config200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/test/test_get_entity_config_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/test/test_get_monitored_tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/test/test_get_notification_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/test/test_get_public_key200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/test/test_get_public_key_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/test/test_list_monitored_tokens200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/test/test_list_monitored_tokens200_response_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2024-05-24 20:21:17.000000 circle_configurations-0.1.0b1/test/test_monitor_tokens_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/test/test_notification_signature_public_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/test/test_post_monitored_tokens_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/test/test_post_monitored_tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/test/test_put_monitored_tokens_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/test/test_put_monitored_tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/test/test_put_monitored_tokens_scope_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/test/test_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/test/test_testnet_blockchain.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/test/test_token_monitor_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/test/test_token_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/test/test_token_standard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2024-05-24 20:21:16.000000 circle_configurations-0.1.0b1/test/test_update_monitored_tokens200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2024-05-24 20:21:17.000000 circle_configurations-0.1.0b1/test/test_webhook_subscriptions_api.py
+drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-30 18:20:42.277056 circle_configurations-1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2024-05-30 18:20:42.277056 circle_configurations-1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2024-05-30 18:17:44.000000 circle_configurations-1.0/README.md
+drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-30 18:20:42.189056 circle_configurations-1.0/circle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2024-05-30 18:17:44.000000 circle_configurations-1.0/circle/__init__.py
+drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-30 18:20:42.189056 circle_configurations-1.0/circle/web3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2024-05-30 18:17:44.000000 circle_configurations-1.0/circle/web3/__init__.py
+drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-30 18:20:42.189056 circle_configurations-1.0/circle/web3/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2024-05-30 18:17:44.000000 circle_configurations-1.0/circle/web3/configurations/__init__.py
+drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-30 18:20:42.193056 circle_configurations-1.0/circle/web3/configurations/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2024-05-30 18:17:44.000000 circle_configurations-1.0/circle/web3/configurations/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12342 2024-05-30 18:17:43.000000 circle_configurations-1.0/circle/web3/configurations/api/developer_account_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8216 2024-05-30 18:17:43.000000 circle_configurations-1.0/circle/web3/configurations/api/faucet_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43514 2024-05-30 18:17:43.000000 circle_configurations-1.0/circle/web3/configurations/api/monitor_tokens_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9085 2024-05-30 18:17:43.000000 circle_configurations-1.0/circle/web3/configurations/api/webhook_subscriptions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30048 2024-05-30 18:17:44.000000 circle_configurations-1.0/circle/web3/configurations/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2024-05-30 18:17:44.000000 circle_configurations-1.0/circle/web3/configurations/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14645 2024-05-30 18:17:44.000000 circle_configurations-1.0/circle/web3/configurations/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2024-05-30 18:17:44.000000 circle_configurations-1.0/circle/web3/configurations/exceptions.py
+drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-30 18:20:42.197056 circle_configurations-1.0/circle/web3/configurations/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2024-05-30 18:17:44.000000 circle_configurations-1.0/circle/web3/configurations/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2024-05-30 18:17:41.000000 circle_configurations-1.0/circle/web3/configurations/models/blockchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2024-05-30 18:17:41.000000 circle_configurations-1.0/circle/web3/configurations/models/create_monitored_tokens200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2024-05-30 18:17:42.000000 circle_configurations-1.0/circle/web3/configurations/models/delete_monitored_tokens_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2024-05-30 18:17:42.000000 circle_configurations-1.0/circle/web3/configurations/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2024-05-30 18:17:42.000000 circle_configurations-1.0/circle/web3/configurations/models/faucet_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2024-05-30 18:17:42.000000 circle_configurations-1.0/circle/web3/configurations/models/get_entity_config200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2024-05-30 18:17:42.000000 circle_configurations-1.0/circle/web3/configurations/models/get_entity_config_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2024-05-30 18:17:42.000000 circle_configurations-1.0/circle/web3/configurations/models/get_monitored_tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2024-05-30 18:17:42.000000 circle_configurations-1.0/circle/web3/configurations/models/get_notification_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2024-05-30 18:17:42.000000 circle_configurations-1.0/circle/web3/configurations/models/get_public_key200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2024-05-30 18:17:42.000000 circle_configurations-1.0/circle/web3/configurations/models/get_public_key_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2024-05-30 18:17:42.000000 circle_configurations-1.0/circle/web3/configurations/models/list_monitored_tokens200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2024-05-30 18:17:42.000000 circle_configurations-1.0/circle/web3/configurations/models/list_monitored_tokens200_response_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2024-05-30 18:17:42.000000 circle_configurations-1.0/circle/web3/configurations/models/notification_signature_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2024-05-30 18:17:42.000000 circle_configurations-1.0/circle/web3/configurations/models/post_monitored_tokens_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2024-05-30 18:17:42.000000 circle_configurations-1.0/circle/web3/configurations/models/post_monitored_tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2024-05-30 18:17:42.000000 circle_configurations-1.0/circle/web3/configurations/models/put_monitored_tokens_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2024-05-30 18:17:42.000000 circle_configurations-1.0/circle/web3/configurations/models/put_monitored_tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2024-05-30 18:17:42.000000 circle_configurations-1.0/circle/web3/configurations/models/put_monitored_tokens_scope_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2024-05-30 18:17:42.000000 circle_configurations-1.0/circle/web3/configurations/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2024-05-30 18:17:42.000000 circle_configurations-1.0/circle/web3/configurations/models/testnet_blockchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2024-05-30 18:17:42.000000 circle_configurations-1.0/circle/web3/configurations/models/token_monitor_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2024-05-30 18:17:43.000000 circle_configurations-1.0/circle/web3/configurations/models/token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2024-05-30 18:17:43.000000 circle_configurations-1.0/circle/web3/configurations/models/token_standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2024-05-30 18:17:43.000000 circle_configurations-1.0/circle/web3/configurations/models/update_monitored_tokens200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2024-05-30 18:17:44.000000 circle_configurations-1.0/circle/web3/configurations/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12800 2024-05-30 18:17:44.000000 circle_configurations-1.0/circle/web3/configurations/rest.py
+drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-30 18:20:42.277056 circle_configurations-1.0/circle_configurations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2024-05-30 18:20:42.000000 circle_configurations-1.0/circle_configurations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2024-05-30 18:20:42.000000 circle_configurations-1.0/circle_configurations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2024-05-30 18:20:42.000000 circle_configurations-1.0/circle_configurations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2024-05-30 18:20:42.000000 circle_configurations-1.0/circle_configurations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2024-05-30 18:20:42.000000 circle_configurations-1.0/circle_configurations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2024-05-30 18:17:44.000000 circle_configurations-1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2024-05-30 18:20:42.277056 circle_configurations-1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2024-05-30 18:17:44.000000 circle_configurations-1.0/setup.py
+drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-30 18:20:42.277056 circle_configurations-1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2024-05-30 18:17:41.000000 circle_configurations-1.0/test/test_blockchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2024-05-30 18:17:41.000000 circle_configurations-1.0/test/test_create_monitored_tokens200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2024-05-30 18:17:42.000000 circle_configurations-1.0/test/test_delete_monitored_tokens_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2024-05-30 18:17:43.000000 circle_configurations-1.0/test/test_developer_account_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2024-05-30 18:17:42.000000 circle_configurations-1.0/test/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2024-05-30 18:17:43.000000 circle_configurations-1.0/test/test_faucet_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2024-05-30 18:17:42.000000 circle_configurations-1.0/test/test_faucet_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2024-05-30 18:17:42.000000 circle_configurations-1.0/test/test_get_entity_config200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2024-05-30 18:17:42.000000 circle_configurations-1.0/test/test_get_entity_config_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2024-05-30 18:17:42.000000 circle_configurations-1.0/test/test_get_monitored_tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2024-05-30 18:17:42.000000 circle_configurations-1.0/test/test_get_notification_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2024-05-30 18:17:42.000000 circle_configurations-1.0/test/test_get_public_key200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2024-05-30 18:17:42.000000 circle_configurations-1.0/test/test_get_public_key_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2024-05-30 18:17:42.000000 circle_configurations-1.0/test/test_list_monitored_tokens200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2024-05-30 18:17:42.000000 circle_configurations-1.0/test/test_list_monitored_tokens200_response_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2024-05-30 18:17:43.000000 circle_configurations-1.0/test/test_monitor_tokens_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2024-05-30 18:17:42.000000 circle_configurations-1.0/test/test_notification_signature_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2024-05-30 18:17:42.000000 circle_configurations-1.0/test/test_post_monitored_tokens_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2024-05-30 18:17:42.000000 circle_configurations-1.0/test/test_post_monitored_tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2024-05-30 18:17:42.000000 circle_configurations-1.0/test/test_put_monitored_tokens_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2024-05-30 18:17:42.000000 circle_configurations-1.0/test/test_put_monitored_tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2024-05-30 18:17:42.000000 circle_configurations-1.0/test/test_put_monitored_tokens_scope_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2024-05-30 18:17:42.000000 circle_configurations-1.0/test/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2024-05-30 18:17:42.000000 circle_configurations-1.0/test/test_testnet_blockchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2024-05-30 18:17:43.000000 circle_configurations-1.0/test/test_token_monitor_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2024-05-30 18:17:43.000000 circle_configurations-1.0/test/test_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2024-05-30 18:17:43.000000 circle_configurations-1.0/test/test_token_standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2024-05-30 18:17:43.000000 circle_configurations-1.0/test/test_update_monitored_tokens200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2024-05-30 18:17:43.000000 circle_configurations-1.0/test/test_webhook_subscriptions_api.py
```

### Comparing `circle_configurations-0.1.0b1/README.md` & `circle_configurations-1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # circle-configurations
 General Configuration APIs for Web3 Service products.
 
 - API version: 1.0
-- Package version: 0.1.0b1
+- Package version: 1.0
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation
 ### pip install
```

### Comparing `circle_configurations-0.1.0b1/circle/web3/configurations/__init__.py` & `circle_configurations-1.0/circle/web3/configurations/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     The version of the OpenAPI document: 1.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "0.1.0b1"
+__version__ = "1.0"
 
 # import apis into sdk package
 from circle.web3.configurations.api.developer_account_api import DeveloperAccountApi
 from circle.web3.configurations.api.faucet_api import FaucetApi
 from circle.web3.configurations.api.monitor_tokens_api import MonitorTokensApi
 from circle.web3.configurations.api.webhook_subscriptions_api import WebhookSubscriptionsApi
```

### Comparing `circle_configurations-0.1.0b1/circle/web3/configurations/api/developer_account_api.py` & `circle_configurations-1.0/circle/web3/configurations/api/developer_account_api.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/circle/web3/configurations/api/faucet_api.py` & `circle_configurations-1.0/circle/web3/configurations/api/faucet_api.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/circle/web3/configurations/api/monitor_tokens_api.py` & `circle_configurations-1.0/circle/web3/configurations/api/monitor_tokens_api.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/circle/web3/configurations/api/webhook_subscriptions_api.py` & `circle_configurations-1.0/circle/web3/configurations/api/webhook_subscriptions_api.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/circle/web3/configurations/api_client.py` & `circle_configurations-1.0/circle/web3/configurations/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = (user_agent + ' / ' if user_agent else '') + 'CircleWeb3PythonSDK / 0.1.0b1'
+        self.user_agent = (user_agent + ' / ' if user_agent else '') + 'CircleWeb3PythonSDK / 1.0'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `circle_configurations-0.1.0b1/circle/web3/configurations/api_response.py` & `circle_configurations-1.0/circle/web3/configurations/api_response.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/circle/web3/configurations/configuration.py` & `circle_configurations-1.0/circle/web3/configurations/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0\n"\
-               "SDK Package Version: 0.1.0b1".\
+               "SDK Package Version: 1.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `circle_configurations-0.1.0b1/circle/web3/configurations/exceptions.py` & `circle_configurations-1.0/circle/web3/configurations/exceptions.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/circle/web3/configurations/models/__init__.py` & `circle_configurations-1.0/circle/web3/configurations/models/__init__.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/circle/web3/configurations/models/blockchain.py` & `circle_configurations-1.0/circle/web3/configurations/models/blockchain.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/circle/web3/configurations/models/create_monitored_tokens200_response.py` & `circle_configurations-1.0/circle/web3/configurations/models/create_monitored_tokens200_response.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/circle/web3/configurations/models/delete_monitored_tokens_request.py` & `circle_configurations-1.0/circle/web3/configurations/models/delete_monitored_tokens_request.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/circle/web3/configurations/models/error.py` & `circle_configurations-1.0/circle/web3/configurations/models/error.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/circle/web3/configurations/models/faucet_request.py` & `circle_configurations-1.0/circle/web3/configurations/models/faucet_request.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/circle/web3/configurations/models/get_entity_config200_response.py` & `circle_configurations-1.0/circle/web3/configurations/models/get_entity_config200_response.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/circle/web3/configurations/models/get_entity_config_response.py` & `circle_configurations-1.0/circle/web3/configurations/models/get_entity_config_response.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/circle/web3/configurations/models/get_monitored_tokens_response.py` & `circle_configurations-1.0/circle/web3/configurations/models/get_monitored_tokens_response.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/circle/web3/configurations/models/get_notification_signature.py` & `circle_configurations-1.0/circle/web3/configurations/models/get_notification_signature.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/circle/web3/configurations/models/get_public_key200_response.py` & `circle_configurations-1.0/circle/web3/configurations/models/get_public_key200_response.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/circle/web3/configurations/models/get_public_key_response.py` & `circle_configurations-1.0/circle/web3/configurations/models/get_public_key_response.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/circle/web3/configurations/models/list_monitored_tokens200_response.py` & `circle_configurations-1.0/circle/web3/configurations/models/list_monitored_tokens200_response.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/circle/web3/configurations/models/list_monitored_tokens200_response_response.py` & `circle_configurations-1.0/circle/web3/configurations/models/list_monitored_tokens200_response_response.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/circle/web3/configurations/models/notification_signature_public_key.py` & `circle_configurations-1.0/circle/web3/configurations/models/notification_signature_public_key.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/circle/web3/configurations/models/post_monitored_tokens_request.py` & `circle_configurations-1.0/circle/web3/configurations/models/post_monitored_tokens_request.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/circle/web3/configurations/models/post_monitored_tokens_response.py` & `circle_configurations-1.0/circle/web3/configurations/models/post_monitored_tokens_response.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/circle/web3/configurations/models/put_monitored_tokens_request.py` & `circle_configurations-1.0/circle/web3/configurations/models/put_monitored_tokens_request.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/circle/web3/configurations/models/put_monitored_tokens_response.py` & `circle_configurations-1.0/circle/web3/configurations/models/put_monitored_tokens_response.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/circle/web3/configurations/models/put_monitored_tokens_scope_request.py` & `circle_configurations-1.0/circle/web3/configurations/models/put_monitored_tokens_scope_request.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/circle/web3/configurations/models/status.py` & `circle_configurations-1.0/circle/web3/configurations/models/status.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/circle/web3/configurations/models/testnet_blockchain.py` & `circle_configurations-1.0/circle/web3/configurations/models/testnet_blockchain.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/circle/web3/configurations/models/token_monitor_scope.py` & `circle_configurations-1.0/circle/web3/configurations/models/token_monitor_scope.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/circle/web3/configurations/models/token_response.py` & `circle_configurations-1.0/circle/web3/configurations/models/token_response.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/circle/web3/configurations/models/token_standard.py` & `circle_configurations-1.0/circle/web3/configurations/models/token_standard.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/circle/web3/configurations/models/update_monitored_tokens200_response.py` & `circle_configurations-1.0/circle/web3/configurations/models/update_monitored_tokens200_response.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/circle/web3/configurations/rest.py` & `circle_configurations-1.0/circle/web3/configurations/rest.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/circle_configurations.egg-info/SOURCES.txt` & `circle_configurations-1.0/circle_configurations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/pyproject.toml` & `circle_configurations-1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "circle.web3.configurations"
-version = "0.1.0b1"
+version = "1.0"
 description = "Configurations"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Configurations"]
 include = ["circle.web3.configurations/py.typed"]
```

### Comparing `circle_configurations-0.1.0b1/setup.py` & `circle_configurations-1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "circle-configurations"
-VERSION = "0.1.0b1"
+VERSION = "1.0"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 1.10.5, < 2",
     "aenum"
 ]
```

### Comparing `circle_configurations-0.1.0b1/test/test_blockchain.py` & `circle_configurations-1.0/test/test_blockchain.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/test/test_create_monitored_tokens200_response.py` & `circle_configurations-1.0/test/test_create_monitored_tokens200_response.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/test/test_delete_monitored_tokens_request.py` & `circle_configurations-1.0/test/test_delete_monitored_tokens_request.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/test/test_developer_account_api.py` & `circle_configurations-1.0/test/test_developer_account_api.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/test/test_error.py` & `circle_configurations-1.0/test/test_error.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/test/test_faucet_api.py` & `circle_configurations-1.0/test/test_faucet_api.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/test/test_faucet_request.py` & `circle_configurations-1.0/test/test_faucet_request.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/test/test_get_entity_config200_response.py` & `circle_configurations-1.0/test/test_get_entity_config200_response.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/test/test_get_entity_config_response.py` & `circle_configurations-1.0/test/test_get_entity_config_response.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/test/test_get_monitored_tokens_response.py` & `circle_configurations-1.0/test/test_get_monitored_tokens_response.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/test/test_get_notification_signature.py` & `circle_configurations-1.0/test/test_get_notification_signature.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/test/test_get_public_key200_response.py` & `circle_configurations-1.0/test/test_get_public_key200_response.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/test/test_get_public_key_response.py` & `circle_configurations-1.0/test/test_get_public_key_response.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/test/test_list_monitored_tokens200_response.py` & `circle_configurations-1.0/test/test_list_monitored_tokens200_response.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/test/test_list_monitored_tokens200_response_response.py` & `circle_configurations-1.0/test/test_list_monitored_tokens200_response_response.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/test/test_monitor_tokens_api.py` & `circle_configurations-1.0/test/test_monitor_tokens_api.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/test/test_notification_signature_public_key.py` & `circle_configurations-1.0/test/test_notification_signature_public_key.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/test/test_post_monitored_tokens_request.py` & `circle_configurations-1.0/test/test_post_monitored_tokens_request.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/test/test_post_monitored_tokens_response.py` & `circle_configurations-1.0/test/test_post_monitored_tokens_response.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/test/test_put_monitored_tokens_request.py` & `circle_configurations-1.0/test/test_put_monitored_tokens_request.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/test/test_put_monitored_tokens_response.py` & `circle_configurations-1.0/test/test_put_monitored_tokens_response.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/test/test_put_monitored_tokens_scope_request.py` & `circle_configurations-1.0/test/test_put_monitored_tokens_scope_request.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/test/test_status.py` & `circle_configurations-1.0/test/test_status.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/test/test_testnet_blockchain.py` & `circle_configurations-1.0/test/test_testnet_blockchain.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/test/test_token_monitor_scope.py` & `circle_configurations-1.0/test/test_token_monitor_scope.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/test/test_token_response.py` & `circle_configurations-1.0/test/test_token_response.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/test/test_token_standard.py` & `circle_configurations-1.0/test/test_token_standard.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/test/test_update_monitored_tokens200_response.py` & `circle_configurations-1.0/test/test_update_monitored_tokens200_response.py`

 * *Files identical despite different names*

### Comparing `circle_configurations-0.1.0b1/test/test_webhook_subscriptions_api.py` & `circle_configurations-1.0/test/test_webhook_subscriptions_api.py`

 * *Files identical despite different names*

