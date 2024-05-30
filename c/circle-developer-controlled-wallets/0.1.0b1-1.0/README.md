# Comparing `tmp/circle_developer_controlled_wallets-0.1.0b1.tar.gz` & `tmp/circle_developer_controlled_wallets-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circle_developer_controlled_wallets-0.1.0b1.tar", last modified: Fri May 24 20:24:37 2024, max compression
+gzip compressed data, was "circle_developer_controlled_wallets-1.0.tar", last modified: Thu May 30 18:20:59 2024, max compression
```

## Comparing `circle_developer_controlled_wallets-0.1.0b1.tar` & `circle_developer_controlled_wallets-1.0.tar`

### file list

```diff
@@ -1,189 +1,189 @@
-drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-24 20:24:37.208175 circle_developer_controlled_wallets-0.1.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2024-05-24 20:24:37.208175 circle_developer_controlled_wallets-0.1.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2024-05-24 20:22:01.000000 circle_developer_controlled_wallets-0.1.0b1/README.md
-drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-24 20:24:36.912175 circle_developer_controlled_wallets-0.1.0b1/circle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2024-05-24 20:22:02.000000 circle_developer_controlled_wallets-0.1.0b1/circle/__init__.py
-drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-24 20:24:36.912175 circle_developer_controlled_wallets-0.1.0b1/circle/web3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2024-05-24 20:22:02.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/__init__.py
-drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-24 20:24:36.912175 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/
--rw-r--r--   0 runner    (1001) docker     (123)    10222 2024-05-24 20:22:01.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/__init__.py
-drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-24 20:24:36.916175 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/api/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2024-05-24 20:22:02.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17281 2024-05-24 20:22:01.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/api/signing_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7840 2024-05-24 20:22:01.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/api/token_lookup_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    81988 2024-05-24 20:22:01.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/api/transactions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    35760 2024-05-24 20:22:01.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/api/wallet_sets_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    67317 2024-05-24 20:22:01.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/api/wallets_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    31614 2024-05-24 20:22:02.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2024-05-24 20:22:02.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/api_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    15117 2024-05-24 20:22:01.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2024-05-24 20:22:02.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/exceptions.py
-drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-24 20:24:37.020175 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/
--rw-r--r--   0 runner    (1001) docker     (123)     9016 2024-05-24 20:22:02.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6093 2024-05-24 20:21:57.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/abi_parameters_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2024-05-24 20:21:57.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/accelerate_transaction_for_developer_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2024-05-24 20:21:57.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/accelerate_transaction_for_developer_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2024-05-24 20:21:57.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/account_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2024-05-24 20:21:57.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/balance.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2024-05-24 20:21:57.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/blockchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2024-05-24 20:21:57.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/cancel_transaction_for_developer_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2024-05-24 20:21:57.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/cancel_transaction_for_developer_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8594 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/create_contract_execution_transaction_for_developer_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/create_contract_execution_transaction_for_developer_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/create_developer_transaction_accelerate200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/create_developer_transaction_cancel200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/create_developer_transaction_contract_execution200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/create_developer_transaction_transfer200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/create_developer_wallet200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/create_developer_wallet_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/create_developer_wallet_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/create_developer_wallet_set_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/create_developer_wallet_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/create_transfer_estimate_fee200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7735 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/create_transfer_transaction_for_developer_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/create_transfer_transaction_for_developer_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/create_validate_address200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/create_wallet_set200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/custody_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/estimate_contract_execution_transaction_fee_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/estimate_transaction_fee_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/estimate_transfer_transaction_fee_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/estimated_transaction_fee.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/ext_get_all_wallets_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/ext_get_wallet_by_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/ext_update_wallet_metadata_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/ext_wallet_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5277 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/ext_wallet_response_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/fee_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/get_balances_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/get_nfts_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/get_token_by_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/get_token_id200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/get_transaction200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/get_transaction_by_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/get_transactions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/get_wallet200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/get_wallet_set200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/get_wallet_set_by_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/get_wallet_sets_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/list_transactions200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/list_wallet_ballance200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/list_wallet_nfts200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/list_wallet_sets200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/list_wallets200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/nft.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/sign_developer_message200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/sign_developer_typed_data200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/sign_message_for_developer_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/sign_message_for_developer_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/sign_typed_data_for_developer_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/sign_typed_data_for_developer_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/token_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/token_standard.py
--rw-r--r--   0 runner    (1001) docker     (123)    10517 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/transaction_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/transaction_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/update_wallet200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/update_wallet_set200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/update_wallet_set_metadata_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/update_wallet_set_metadata_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/validate_address_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/validate_address_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/wallet_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5120 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/wallet_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/wallet_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/wallet_state.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2024-05-24 20:22:01.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12814 2024-05-24 20:22:02.000000 circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/rest.py
-drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-24 20:24:37.208175 circle_developer_controlled_wallets-0.1.0b1/circle_developer_controlled_wallets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2024-05-24 20:24:36.000000 circle_developer_controlled_wallets-0.1.0b1/circle_developer_controlled_wallets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10617 2024-05-24 20:24:36.000000 circle_developer_controlled_wallets-0.1.0b1/circle_developer_controlled_wallets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2024-05-24 20:24:36.000000 circle_developer_controlled_wallets-0.1.0b1/circle_developer_controlled_wallets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2024-05-24 20:24:36.000000 circle_developer_controlled_wallets-0.1.0b1/circle_developer_controlled_wallets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2024-05-24 20:24:36.000000 circle_developer_controlled_wallets-0.1.0b1/circle_developer_controlled_wallets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      814 2024-05-24 20:22:01.000000 circle_developer_controlled_wallets-0.1.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2024-05-24 20:24:37.208175 circle_developer_controlled_wallets-0.1.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2024-05-24 20:22:01.000000 circle_developer_controlled_wallets-0.1.0b1/setup.py
-drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-24 20:24:37.208175 circle_developer_controlled_wallets-0.1.0b1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2024-05-24 20:21:57.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_abi_parameters_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2024-05-24 20:21:57.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_accelerate_transaction_for_developer_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2024-05-24 20:21:57.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_accelerate_transaction_for_developer_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2024-05-24 20:21:57.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_account_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2024-05-24 20:21:57.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2024-05-24 20:21:57.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_blockchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2024-05-24 20:21:57.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_cancel_transaction_for_developer_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2024-05-24 20:21:57.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_cancel_transaction_for_developer_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_create_contract_execution_transaction_for_developer_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_create_contract_execution_transaction_for_developer_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_create_developer_transaction_accelerate200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_create_developer_transaction_cancel200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_create_developer_transaction_contract_execution200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_create_developer_transaction_transfer200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_create_developer_wallet200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_create_developer_wallet_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_create_developer_wallet_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_create_developer_wallet_set_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_create_developer_wallet_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_create_transfer_estimate_fee200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_create_transfer_transaction_for_developer_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_create_transfer_transaction_for_developer_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_create_validate_address200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_create_wallet_set200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_custody_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2024-05-24 20:21:58.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_estimate_contract_execution_transaction_fee_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_estimate_transaction_fee_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_estimate_transfer_transaction_fee_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_estimated_transaction_fee.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_ext_get_all_wallets_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_ext_get_wallet_by_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_ext_update_wallet_metadata_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_ext_wallet_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_ext_wallet_response_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_fee_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_get_balances_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_get_nfts_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_get_token_by_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_get_token_id200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_get_transaction200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_get_transaction_by_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_get_transactions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_get_wallet200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_get_wallet_set200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_get_wallet_set_by_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_get_wallet_sets_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_list_transactions200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_list_wallet_ballance200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_list_wallet_nfts200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_list_wallet_sets200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_list_wallets200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_nft.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2024-05-24 20:21:59.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_sign_developer_message200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_sign_developer_typed_data200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_sign_message_for_developer_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_sign_message_for_developer_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_sign_typed_data_for_developer_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_sign_typed_data_for_developer_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2024-05-24 20:22:01.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_signing_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2024-05-24 20:22:01.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_token_lookup_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_token_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_token_standard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_transaction_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_transaction_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2024-05-24 20:22:01.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_transactions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_update_wallet200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_update_wallet_set200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_update_wallet_set_metadata_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_update_wallet_set_metadata_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_validate_address_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_validate_address_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_wallet_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_wallet_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_wallet_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2024-05-24 20:22:01.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_wallet_sets_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2024-05-24 20:22:00.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_wallet_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2024-05-24 20:22:01.000000 circle_developer_controlled_wallets-0.1.0b1/test/test_wallets_api.py
+drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-30 18:20:59.981054 circle_developer_controlled_wallets-1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2024-05-30 18:20:59.981054 circle_developer_controlled_wallets-1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2024-05-30 18:18:27.000000 circle_developer_controlled_wallets-1.0/README.md
+drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-30 18:20:59.709054 circle_developer_controlled_wallets-1.0/circle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2024-05-30 18:18:27.000000 circle_developer_controlled_wallets-1.0/circle/__init__.py
+drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-30 18:20:59.709054 circle_developer_controlled_wallets-1.0/circle/web3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2024-05-30 18:18:27.000000 circle_developer_controlled_wallets-1.0/circle/web3/__init__.py
+drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-30 18:20:59.709054 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/
+-rw-r--r--   0 runner    (1001) docker     (123)    10218 2024-05-30 18:18:27.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/__init__.py
+drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-30 18:20:59.773054 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2024-05-30 18:18:27.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17281 2024-05-30 18:18:27.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/api/signing_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7840 2024-05-30 18:18:27.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/api/token_lookup_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81988 2024-05-30 18:18:27.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/api/transactions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35760 2024-05-30 18:18:27.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/api/wallet_sets_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67317 2024-05-30 18:18:27.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/api/wallets_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31610 2024-05-30 18:18:27.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2024-05-30 18:18:27.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15113 2024-05-30 18:18:27.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2024-05-30 18:18:27.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/exceptions.py
+drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-30 18:20:59.873054 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     9016 2024-05-30 18:18:27.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6093 2024-05-30 18:18:23.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/abi_parameters_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2024-05-30 18:18:23.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/accelerate_transaction_for_developer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2024-05-30 18:18:23.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/accelerate_transaction_for_developer_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2024-05-30 18:18:23.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/account_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2024-05-30 18:18:23.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2024-05-30 18:18:23.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/blockchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2024-05-30 18:18:23.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/cancel_transaction_for_developer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2024-05-30 18:18:23.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/cancel_transaction_for_developer_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8594 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/create_contract_execution_transaction_for_developer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/create_contract_execution_transaction_for_developer_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/create_developer_transaction_accelerate200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/create_developer_transaction_cancel200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/create_developer_transaction_contract_execution200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/create_developer_transaction_transfer200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/create_developer_wallet200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/create_developer_wallet_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/create_developer_wallet_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/create_developer_wallet_set_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/create_developer_wallet_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/create_transfer_estimate_fee200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7735 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/create_transfer_transaction_for_developer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/create_transfer_transaction_for_developer_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/create_validate_address200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/create_wallet_set200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/custody_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/estimate_contract_execution_transaction_fee_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/estimate_transaction_fee_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/estimate_transfer_transaction_fee_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/estimated_transaction_fee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/ext_get_all_wallets_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/ext_get_wallet_by_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/ext_update_wallet_metadata_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/ext_wallet_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5277 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/ext_wallet_response_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/fee_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/get_balances_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/get_nfts_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/get_token_by_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/get_token_id200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/get_transaction200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/get_transaction_by_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/get_transactions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/get_wallet200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/get_wallet_set200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/get_wallet_set_by_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/get_wallet_sets_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/list_transactions200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/list_wallet_ballance200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/list_wallet_nfts200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/list_wallet_sets200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/list_wallets200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/nft.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/sign_developer_message200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/sign_developer_typed_data200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/sign_message_for_developer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/sign_message_for_developer_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/sign_typed_data_for_developer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/sign_typed_data_for_developer_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/token_standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10517 2024-05-30 18:18:26.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2024-05-30 18:18:26.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/transaction_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2024-05-30 18:18:26.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/transaction_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2024-05-30 18:18:26.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/update_wallet200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2024-05-30 18:18:26.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/update_wallet_set200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2024-05-30 18:18:26.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/update_wallet_set_metadata_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2024-05-30 18:18:26.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/update_wallet_set_metadata_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2024-05-30 18:18:26.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/validate_address_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2024-05-30 18:18:26.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/validate_address_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2024-05-30 18:18:26.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/wallet_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2024-05-30 18:18:26.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/wallet_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2024-05-30 18:18:26.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/wallet_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2024-05-30 18:18:26.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/wallet_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2024-05-30 18:18:27.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12814 2024-05-30 18:18:27.000000 circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/rest.py
+drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-30 18:20:59.981054 circle_developer_controlled_wallets-1.0/circle_developer_controlled_wallets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2024-05-30 18:20:59.000000 circle_developer_controlled_wallets-1.0/circle_developer_controlled_wallets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10617 2024-05-30 18:20:59.000000 circle_developer_controlled_wallets-1.0/circle_developer_controlled_wallets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2024-05-30 18:20:59.000000 circle_developer_controlled_wallets-1.0/circle_developer_controlled_wallets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2024-05-30 18:20:59.000000 circle_developer_controlled_wallets-1.0/circle_developer_controlled_wallets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2024-05-30 18:20:59.000000 circle_developer_controlled_wallets-1.0/circle_developer_controlled_wallets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2024-05-30 18:18:27.000000 circle_developer_controlled_wallets-1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2024-05-30 18:20:59.981054 circle_developer_controlled_wallets-1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2024-05-30 18:18:27.000000 circle_developer_controlled_wallets-1.0/setup.py
+drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-30 18:20:59.981054 circle_developer_controlled_wallets-1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2024-05-30 18:18:23.000000 circle_developer_controlled_wallets-1.0/test/test_abi_parameters_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2024-05-30 18:18:23.000000 circle_developer_controlled_wallets-1.0/test/test_accelerate_transaction_for_developer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2024-05-30 18:18:23.000000 circle_developer_controlled_wallets-1.0/test/test_accelerate_transaction_for_developer_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2024-05-30 18:18:23.000000 circle_developer_controlled_wallets-1.0/test/test_account_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2024-05-30 18:18:23.000000 circle_developer_controlled_wallets-1.0/test/test_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2024-05-30 18:18:23.000000 circle_developer_controlled_wallets-1.0/test/test_blockchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2024-05-30 18:18:23.000000 circle_developer_controlled_wallets-1.0/test/test_cancel_transaction_for_developer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2024-05-30 18:18:23.000000 circle_developer_controlled_wallets-1.0/test/test_cancel_transaction_for_developer_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/test/test_create_contract_execution_transaction_for_developer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/test/test_create_contract_execution_transaction_for_developer_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/test/test_create_developer_transaction_accelerate200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/test/test_create_developer_transaction_cancel200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/test/test_create_developer_transaction_contract_execution200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/test/test_create_developer_transaction_transfer200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/test/test_create_developer_wallet200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/test/test_create_developer_wallet_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/test/test_create_developer_wallet_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/test/test_create_developer_wallet_set_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/test/test_create_developer_wallet_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/test/test_create_transfer_estimate_fee200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/test/test_create_transfer_transaction_for_developer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/test/test_create_transfer_transaction_for_developer_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/test/test_create_validate_address200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/test/test_create_wallet_set200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/test/test_custody_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/test/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/test/test_estimate_contract_execution_transaction_fee_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/test/test_estimate_transaction_fee_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/test/test_estimate_transfer_transaction_fee_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/test/test_estimated_transaction_fee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/test/test_ext_get_all_wallets_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2024-05-30 18:18:24.000000 circle_developer_controlled_wallets-1.0/test/test_ext_get_wallet_by_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/test/test_ext_update_wallet_metadata_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/test/test_ext_wallet_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/test/test_ext_wallet_response_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/test/test_fee_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/test/test_get_balances_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/test/test_get_nfts_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/test/test_get_token_by_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/test/test_get_token_id200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/test/test_get_transaction200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/test/test_get_transaction_by_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/test/test_get_transactions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/test/test_get_wallet200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/test/test_get_wallet_set200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/test/test_get_wallet_set_by_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/test/test_get_wallet_sets_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/test/test_list_transactions200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/test/test_list_wallet_ballance200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/test/test_list_wallet_nfts200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/test/test_list_wallet_sets200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/test/test_list_wallets200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/test/test_nft.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/test/test_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/test/test_sign_developer_message200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/test/test_sign_developer_typed_data200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/test/test_sign_message_for_developer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/test/test_sign_message_for_developer_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/test/test_sign_typed_data_for_developer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/test/test_sign_typed_data_for_developer_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2024-05-30 18:18:27.000000 circle_developer_controlled_wallets-1.0/test/test_signing_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2024-05-30 18:18:27.000000 circle_developer_controlled_wallets-1.0/test/test_token_lookup_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/test/test_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2024-05-30 18:18:25.000000 circle_developer_controlled_wallets-1.0/test/test_token_standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2024-05-30 18:18:26.000000 circle_developer_controlled_wallets-1.0/test/test_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2024-05-30 18:18:26.000000 circle_developer_controlled_wallets-1.0/test/test_transaction_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2024-05-30 18:18:26.000000 circle_developer_controlled_wallets-1.0/test/test_transaction_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2024-05-30 18:18:27.000000 circle_developer_controlled_wallets-1.0/test/test_transactions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2024-05-30 18:18:26.000000 circle_developer_controlled_wallets-1.0/test/test_update_wallet200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2024-05-30 18:18:26.000000 circle_developer_controlled_wallets-1.0/test/test_update_wallet_set200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2024-05-30 18:18:26.000000 circle_developer_controlled_wallets-1.0/test/test_update_wallet_set_metadata_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2024-05-30 18:18:26.000000 circle_developer_controlled_wallets-1.0/test/test_update_wallet_set_metadata_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2024-05-30 18:18:26.000000 circle_developer_controlled_wallets-1.0/test/test_validate_address_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2024-05-30 18:18:26.000000 circle_developer_controlled_wallets-1.0/test/test_validate_address_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2024-05-30 18:18:26.000000 circle_developer_controlled_wallets-1.0/test/test_wallet_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2024-05-30 18:18:26.000000 circle_developer_controlled_wallets-1.0/test/test_wallet_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2024-05-30 18:18:26.000000 circle_developer_controlled_wallets-1.0/test/test_wallet_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2024-05-30 18:18:27.000000 circle_developer_controlled_wallets-1.0/test/test_wallet_sets_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2024-05-30 18:18:26.000000 circle_developer_controlled_wallets-1.0/test/test_wallet_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2024-05-30 18:18:27.000000 circle_developer_controlled_wallets-1.0/test/test_wallets_api.py
```

### Comparing `circle_developer_controlled_wallets-0.1.0b1/PKG-INFO` & `circle_developer_controlled_wallets-1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: circle-developer-controlled-wallets
-Version: 0.1.0b1
+Version: 1.0
 Summary: Developer-Controlled Wallets
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: team@openapitools.org
 Keywords: OpenAPI,OpenAPI-Generator,Developer-Controlled Wallets
 Description-Content-Type: text/markdown
 Requires-Dist: urllib3<2.1.0,>=1.25.3
 Requires-Dist: python-dateutil
 Requires-Dist: pydantic<2,>=1.10.5
 Requires-Dist: aenum
 Requires-Dist: pycryptodome>=3.20.0
-Requires-Dist: circle-configurations==0.1.0b1
-Requires-Dist: circle-web3-sdk-util==0.1.0b1
+Requires-Dist: circle-configurations==1.0
+Requires-Dist: circle-web3-sdk-util==1.0
 
 # circle-developer-controlled-wallets
 Developer-Controlled Wallets API documentation.
 
 - API version: 1.0
-- Package version: 0.1.0b1
+- Package version: 1.0
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation
 ### pip install
```

### Comparing `circle_developer_controlled_wallets-0.1.0b1/README.md` & `circle_developer_controlled_wallets-1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # circle-developer-controlled-wallets
 Developer-Controlled Wallets API documentation.
 
 - API version: 1.0
-- Package version: 0.1.0b1
+- Package version: 1.0
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation
 ### pip install
```

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/__init__.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     The version of the OpenAPI document: 1.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "0.1.0b1"
+__version__ = "1.0"
 
 # import apis into sdk package
 from circle.web3.developer_controlled_wallets.api.signing_api import SigningApi
 from circle.web3.developer_controlled_wallets.api.token_lookup_api import TokenLookupApi
 from circle.web3.developer_controlled_wallets.api.transactions_api import TransactionsApi
 from circle.web3.developer_controlled_wallets.api.wallet_sets_api import WalletSetsApi
 from circle.web3.developer_controlled_wallets.api.wallets_api import WalletsApi
```

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/api/signing_api.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/api/signing_api.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/api/token_lookup_api.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/api/token_lookup_api.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/api/transactions_api.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/api/transactions_api.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/api/wallet_sets_api.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/api/wallet_sets_api.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/api/wallets_api.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/api/wallets_api.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/api_client.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = (user_agent + ' / ' if user_agent else '') + 'CircleWeb3PythonSDK / DeveloperControlledWallets / 0.1.0b1'
+        self.user_agent = (user_agent + ' / ' if user_agent else '') + 'CircleWeb3PythonSDK / DeveloperControlledWallets / 1.0'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/api_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/api_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/configuration.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -379,15 +379,15 @@
 
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

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/exceptions.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/exceptions.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/__init__.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/__init__.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/abi_parameters_inner.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/abi_parameters_inner.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/accelerate_transaction_for_developer_request.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/accelerate_transaction_for_developer_request.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/accelerate_transaction_for_developer_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/accelerate_transaction_for_developer_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/account_type.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/account_type.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/balance.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/balance.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/blockchain.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/blockchain.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/cancel_transaction_for_developer_request.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/cancel_transaction_for_developer_request.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/cancel_transaction_for_developer_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/cancel_transaction_for_developer_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/create_contract_execution_transaction_for_developer_request.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/create_contract_execution_transaction_for_developer_request.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/create_contract_execution_transaction_for_developer_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/create_contract_execution_transaction_for_developer_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/create_developer_transaction_accelerate200_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/create_developer_transaction_accelerate200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/create_developer_transaction_cancel200_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/create_developer_transaction_cancel200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/create_developer_transaction_contract_execution200_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/create_developer_transaction_contract_execution200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/create_developer_transaction_transfer200_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/create_developer_transaction_transfer200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/create_developer_wallet200_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/create_developer_wallet200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/create_developer_wallet_request.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/create_developer_wallet_request.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/create_developer_wallet_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/create_developer_wallet_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/create_developer_wallet_set_request.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/create_developer_wallet_set_request.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/create_developer_wallet_set_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/create_developer_wallet_set_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/create_transfer_estimate_fee200_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/create_transfer_estimate_fee200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/create_transfer_transaction_for_developer_request.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/create_transfer_transaction_for_developer_request.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/create_transfer_transaction_for_developer_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/create_transfer_transaction_for_developer_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/create_validate_address200_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/create_validate_address200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/create_wallet_set200_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/create_wallet_set200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/custody_type.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/custody_type.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/error.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/error.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/estimate_contract_execution_transaction_fee_request.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/estimate_contract_execution_transaction_fee_request.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/estimate_transaction_fee_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/estimate_transaction_fee_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/estimate_transfer_transaction_fee_request.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/estimate_transfer_transaction_fee_request.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/estimated_transaction_fee.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/estimated_transaction_fee.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/ext_get_all_wallets_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/ext_get_all_wallets_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/ext_get_wallet_by_id_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/ext_get_wallet_by_id_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/ext_update_wallet_metadata_request.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/ext_update_wallet_metadata_request.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/ext_wallet_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/ext_wallet_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/ext_wallet_response_wallet.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/ext_wallet_response_wallet.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/fee_level.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/fee_level.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/get_balances_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/get_balances_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/get_nfts_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/get_nfts_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/get_token_by_id_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/get_token_by_id_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/get_token_id200_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/get_token_id200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/get_transaction200_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/get_transaction200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/get_transaction_by_id_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/get_transaction_by_id_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/get_transactions_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/get_transactions_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/get_wallet200_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/get_wallet200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/get_wallet_set200_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/get_wallet_set200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/get_wallet_set_by_id_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/get_wallet_set_by_id_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/get_wallet_sets_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/get_wallet_sets_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/list_transactions200_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/list_transactions200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/list_wallet_ballance200_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/list_wallet_ballance200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/list_wallet_nfts200_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/list_wallet_nfts200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/list_wallet_sets200_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/list_wallet_sets200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/list_wallets200_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/list_wallets200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/nft.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/nft.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/operation.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/operation.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/sign_developer_message200_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/sign_developer_message200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/sign_developer_typed_data200_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/sign_developer_typed_data200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/sign_message_for_developer_request.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/sign_message_for_developer_request.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/sign_message_for_developer_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/sign_message_for_developer_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/sign_typed_data_for_developer_request.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/sign_typed_data_for_developer_request.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/sign_typed_data_for_developer_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/sign_typed_data_for_developer_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/token_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/token_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/token_standard.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/token_standard.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/transaction.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/transaction.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/transaction_state.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/transaction_state.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/transaction_type.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/transaction_type.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/update_wallet200_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/update_wallet200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/update_wallet_set200_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/update_wallet_set200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/update_wallet_set_metadata_request.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/update_wallet_set_metadata_request.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/update_wallet_set_metadata_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/update_wallet_set_metadata_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/validate_address_request.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/validate_address_request.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/validate_address_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/validate_address_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/wallet_metadata.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/wallet_metadata.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/wallet_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/wallet_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/wallet_set_response.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/wallet_set_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/models/wallet_state.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/models/wallet_state.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle/web3/developer_controlled_wallets/rest.py` & `circle_developer_controlled_wallets-1.0/circle/web3/developer_controlled_wallets/rest.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle_developer_controlled_wallets.egg-info/PKG-INFO` & `circle_developer_controlled_wallets-1.0/circle_developer_controlled_wallets.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: circle-developer-controlled-wallets
-Version: 0.1.0b1
+Version: 1.0
 Summary: Developer-Controlled Wallets
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: team@openapitools.org
 Keywords: OpenAPI,OpenAPI-Generator,Developer-Controlled Wallets
 Description-Content-Type: text/markdown
 Requires-Dist: urllib3<2.1.0,>=1.25.3
 Requires-Dist: python-dateutil
 Requires-Dist: pydantic<2,>=1.10.5
 Requires-Dist: aenum
 Requires-Dist: pycryptodome>=3.20.0
-Requires-Dist: circle-configurations==0.1.0b1
-Requires-Dist: circle-web3-sdk-util==0.1.0b1
+Requires-Dist: circle-configurations==1.0
+Requires-Dist: circle-web3-sdk-util==1.0
 
 # circle-developer-controlled-wallets
 Developer-Controlled Wallets API documentation.
 
 - API version: 1.0
-- Package version: 0.1.0b1
+- Package version: 1.0
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation
 ### pip install
```

### Comparing `circle_developer_controlled_wallets-0.1.0b1/circle_developer_controlled_wallets.egg-info/SOURCES.txt` & `circle_developer_controlled_wallets-1.0/circle_developer_controlled_wallets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/pyproject.toml` & `circle_developer_controlled_wallets-1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "circle.web3.developer_controlled_wallets"
-version = "0.1.0b1"
+version = "1.0"
 description = "Developer-Controlled Wallets"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Developer-Controlled Wallets"]
 include = ["circle.web3.developer_controlled_wallets/py.typed"]
```

### Comparing `circle_developer_controlled_wallets-0.1.0b1/setup.py` & `circle_developer_controlled_wallets-1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "circle-developer-controlled-wallets"
-VERSION = "0.1.0b1"
+VERSION = "1.0"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 1.10.5, < 2",
     "aenum",
     "pycryptodome >= 3.20.0",
-    "circle-configurations == 0.1.0b1",
-    "circle-web3-sdk-util == 0.1.0b1"
+    "circle-configurations == 1.0",
+    "circle-web3-sdk-util == 1.0"
 ]
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name=NAME,
```

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_abi_parameters_inner.py` & `circle_developer_controlled_wallets-1.0/test/test_abi_parameters_inner.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_accelerate_transaction_for_developer_request.py` & `circle_developer_controlled_wallets-1.0/test/test_accelerate_transaction_for_developer_request.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_accelerate_transaction_for_developer_response.py` & `circle_developer_controlled_wallets-1.0/test/test_accelerate_transaction_for_developer_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_account_type.py` & `circle_developer_controlled_wallets-1.0/test/test_account_type.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_balance.py` & `circle_developer_controlled_wallets-1.0/test/test_balance.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_blockchain.py` & `circle_developer_controlled_wallets-1.0/test/test_blockchain.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_cancel_transaction_for_developer_request.py` & `circle_developer_controlled_wallets-1.0/test/test_cancel_transaction_for_developer_request.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_cancel_transaction_for_developer_response.py` & `circle_developer_controlled_wallets-1.0/test/test_cancel_transaction_for_developer_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_create_contract_execution_transaction_for_developer_request.py` & `circle_developer_controlled_wallets-1.0/test/test_create_contract_execution_transaction_for_developer_request.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_create_contract_execution_transaction_for_developer_response.py` & `circle_developer_controlled_wallets-1.0/test/test_create_contract_execution_transaction_for_developer_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_create_developer_transaction_accelerate200_response.py` & `circle_developer_controlled_wallets-1.0/test/test_create_developer_transaction_accelerate200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_create_developer_transaction_cancel200_response.py` & `circle_developer_controlled_wallets-1.0/test/test_create_developer_transaction_cancel200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_create_developer_transaction_contract_execution200_response.py` & `circle_developer_controlled_wallets-1.0/test/test_create_developer_transaction_contract_execution200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_create_developer_transaction_transfer200_response.py` & `circle_developer_controlled_wallets-1.0/test/test_create_developer_transaction_transfer200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_create_developer_wallet200_response.py` & `circle_developer_controlled_wallets-1.0/test/test_create_developer_wallet200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_create_developer_wallet_request.py` & `circle_developer_controlled_wallets-1.0/test/test_create_developer_wallet_request.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_create_developer_wallet_response.py` & `circle_developer_controlled_wallets-1.0/test/test_create_developer_wallet_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_create_developer_wallet_set_request.py` & `circle_developer_controlled_wallets-1.0/test/test_create_developer_wallet_set_request.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_create_developer_wallet_set_response.py` & `circle_developer_controlled_wallets-1.0/test/test_create_developer_wallet_set_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_create_transfer_estimate_fee200_response.py` & `circle_developer_controlled_wallets-1.0/test/test_create_transfer_estimate_fee200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_create_transfer_transaction_for_developer_request.py` & `circle_developer_controlled_wallets-1.0/test/test_create_transfer_transaction_for_developer_request.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_create_transfer_transaction_for_developer_response.py` & `circle_developer_controlled_wallets-1.0/test/test_create_transfer_transaction_for_developer_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_create_validate_address200_response.py` & `circle_developer_controlled_wallets-1.0/test/test_create_validate_address200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_create_wallet_set200_response.py` & `circle_developer_controlled_wallets-1.0/test/test_create_wallet_set200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_custody_type.py` & `circle_developer_controlled_wallets-1.0/test/test_custody_type.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_error.py` & `circle_developer_controlled_wallets-1.0/test/test_error.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_estimate_contract_execution_transaction_fee_request.py` & `circle_developer_controlled_wallets-1.0/test/test_estimate_contract_execution_transaction_fee_request.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_estimate_transaction_fee_response.py` & `circle_developer_controlled_wallets-1.0/test/test_estimate_transaction_fee_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_estimate_transfer_transaction_fee_request.py` & `circle_developer_controlled_wallets-1.0/test/test_estimate_transfer_transaction_fee_request.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_estimated_transaction_fee.py` & `circle_developer_controlled_wallets-1.0/test/test_estimated_transaction_fee.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_ext_get_all_wallets_response.py` & `circle_developer_controlled_wallets-1.0/test/test_ext_get_all_wallets_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_ext_get_wallet_by_id_response.py` & `circle_developer_controlled_wallets-1.0/test/test_ext_get_wallet_by_id_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_ext_update_wallet_metadata_request.py` & `circle_developer_controlled_wallets-1.0/test/test_ext_update_wallet_metadata_request.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_ext_wallet_response.py` & `circle_developer_controlled_wallets-1.0/test/test_ext_wallet_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_ext_wallet_response_wallet.py` & `circle_developer_controlled_wallets-1.0/test/test_ext_wallet_response_wallet.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_fee_level.py` & `circle_developer_controlled_wallets-1.0/test/test_fee_level.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_get_balances_response.py` & `circle_developer_controlled_wallets-1.0/test/test_get_balances_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_get_nfts_response.py` & `circle_developer_controlled_wallets-1.0/test/test_get_nfts_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_get_token_by_id_response.py` & `circle_developer_controlled_wallets-1.0/test/test_get_token_by_id_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_get_token_id200_response.py` & `circle_developer_controlled_wallets-1.0/test/test_get_token_id200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_get_transaction200_response.py` & `circle_developer_controlled_wallets-1.0/test/test_get_transaction200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_get_transaction_by_id_response.py` & `circle_developer_controlled_wallets-1.0/test/test_get_transaction_by_id_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_get_transactions_response.py` & `circle_developer_controlled_wallets-1.0/test/test_get_transactions_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_get_wallet200_response.py` & `circle_developer_controlled_wallets-1.0/test/test_get_wallet200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_get_wallet_set200_response.py` & `circle_developer_controlled_wallets-1.0/test/test_get_wallet_set200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_get_wallet_set_by_id_response.py` & `circle_developer_controlled_wallets-1.0/test/test_get_wallet_set_by_id_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_get_wallet_sets_response.py` & `circle_developer_controlled_wallets-1.0/test/test_get_wallet_sets_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_list_transactions200_response.py` & `circle_developer_controlled_wallets-1.0/test/test_list_transactions200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_list_wallet_ballance200_response.py` & `circle_developer_controlled_wallets-1.0/test/test_list_wallet_ballance200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_list_wallet_nfts200_response.py` & `circle_developer_controlled_wallets-1.0/test/test_list_wallet_nfts200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_list_wallet_sets200_response.py` & `circle_developer_controlled_wallets-1.0/test/test_list_wallet_sets200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_list_wallets200_response.py` & `circle_developer_controlled_wallets-1.0/test/test_list_wallets200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_nft.py` & `circle_developer_controlled_wallets-1.0/test/test_nft.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_operation.py` & `circle_developer_controlled_wallets-1.0/test/test_operation.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_sign_developer_message200_response.py` & `circle_developer_controlled_wallets-1.0/test/test_sign_developer_message200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_sign_developer_typed_data200_response.py` & `circle_developer_controlled_wallets-1.0/test/test_sign_developer_typed_data200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_sign_message_for_developer_request.py` & `circle_developer_controlled_wallets-1.0/test/test_sign_message_for_developer_request.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_sign_message_for_developer_response.py` & `circle_developer_controlled_wallets-1.0/test/test_sign_message_for_developer_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_sign_typed_data_for_developer_request.py` & `circle_developer_controlled_wallets-1.0/test/test_sign_typed_data_for_developer_request.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_sign_typed_data_for_developer_response.py` & `circle_developer_controlled_wallets-1.0/test/test_sign_typed_data_for_developer_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_signing_api.py` & `circle_developer_controlled_wallets-1.0/test/test_signing_api.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_token_lookup_api.py` & `circle_developer_controlled_wallets-1.0/test/test_token_lookup_api.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_token_response.py` & `circle_developer_controlled_wallets-1.0/test/test_token_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_token_standard.py` & `circle_developer_controlled_wallets-1.0/test/test_token_standard.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_transaction.py` & `circle_developer_controlled_wallets-1.0/test/test_transaction.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_transaction_state.py` & `circle_developer_controlled_wallets-1.0/test/test_transaction_state.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_transaction_type.py` & `circle_developer_controlled_wallets-1.0/test/test_transaction_type.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_transactions_api.py` & `circle_developer_controlled_wallets-1.0/test/test_transactions_api.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_update_wallet200_response.py` & `circle_developer_controlled_wallets-1.0/test/test_update_wallet200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_update_wallet_set200_response.py` & `circle_developer_controlled_wallets-1.0/test/test_update_wallet_set200_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_update_wallet_set_metadata_request.py` & `circle_developer_controlled_wallets-1.0/test/test_update_wallet_set_metadata_request.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_update_wallet_set_metadata_response.py` & `circle_developer_controlled_wallets-1.0/test/test_update_wallet_set_metadata_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_validate_address_request.py` & `circle_developer_controlled_wallets-1.0/test/test_validate_address_request.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_validate_address_response.py` & `circle_developer_controlled_wallets-1.0/test/test_validate_address_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_wallet_metadata.py` & `circle_developer_controlled_wallets-1.0/test/test_wallet_metadata.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_wallet_response.py` & `circle_developer_controlled_wallets-1.0/test/test_wallet_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_wallet_set_response.py` & `circle_developer_controlled_wallets-1.0/test/test_wallet_set_response.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_wallet_sets_api.py` & `circle_developer_controlled_wallets-1.0/test/test_wallet_sets_api.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_wallet_state.py` & `circle_developer_controlled_wallets-1.0/test/test_wallet_state.py`

 * *Files identical despite different names*

### Comparing `circle_developer_controlled_wallets-0.1.0b1/test/test_wallets_api.py` & `circle_developer_controlled_wallets-1.0/test/test_wallets_api.py`

 * *Files identical despite different names*

