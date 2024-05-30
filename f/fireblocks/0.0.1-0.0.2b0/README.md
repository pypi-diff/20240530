# Comparing `tmp/fireblocks-0.0.1.tar.gz` & `tmp/fireblocks-0.0.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fireblocks-0.0.1.tar", last modified: Fri Dec  1 21:50:22 2023, max compression
+gzip compressed data, was "fireblocks-0.0.2b0.tar", last modified: Thu May 30 14:05:02 2024, max compression
```

## Comparing `fireblocks-0.0.1.tar` & `fireblocks-0.0.2b0.tar`

### file list

```diff
@@ -1,1541 +1,967 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.678919 fireblocks-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    43534 2023-12-01 21:50:22.678919 fireblocks-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    42570 2023-12-01 21:50:09.000000 fireblocks-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.678919 fireblocks-0.0.1/fireblocks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    43534 2023-12-01 21:50:22.000000 fireblocks-0.0.1/fireblocks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    76475 2023-12-01 21:50:22.000000 fireblocks-0.0.1/fireblocks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-01 21:50:22.000000 fireblocks-0.0.1/fireblocks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      227 2023-12-01 21:50:22.000000 fireblocks-0.0.1/fireblocks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-01 21:50:22.000000 fireblocks-0.0.1/fireblocks.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.466916 fireblocks-0.0.1/fireblocks_client/
--rw-r--r--   0 runner    (1001) docker     (127)      849 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    58723 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.466916 fireblocks-0.0.1/fireblocks_client/apis/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27379 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/path_to_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.482916 fireblocks-0.0.1/fireblocks_client/apis/paths/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/audits.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/connections_wc.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/connections_wc_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/contracts.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/contracts_contract_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/contracts_contract_id_asset_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/estimate_network_fee.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/exchange_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/exchange_accounts_exchange_account_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/exchange_accounts_exchange_account_id_asset_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/exchange_accounts_exchange_account_id_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/exchange_accounts_exchange_account_id_internal_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/external_wallets.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/external_wallets_wallet_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/external_wallets_wallet_id_asset_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/external_wallets_wallet_id_set_customer_ref_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      113 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/fiat_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/fiat_accounts_account_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/fiat_accounts_account_id_deposit_from_linked_dda.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/fiat_accounts_account_id_redeem_to_linked_dda.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/gas_station.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/gas_station_asset_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/gas_station_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/gas_station_configuration_asset_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/internal_wallets.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/internal_wallets_wallet_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/internal_wallets_wallet_id_asset_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/internal_wallets_wallet_id_set_customer_ref_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/management_ota.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/network_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/network_connections_connection_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/network_connections_connection_id_is_third_party_routing_asset_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/network_connections_connection_id_set_routing_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/network_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/network_ids_network_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/network_ids_network_id_set_discoverability.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/network_ids_network_id_set_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/network_ids_network_id_set_routing_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/nfts_ownership_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/nfts_ownership_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/nfts_ownership_tokens_id_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/nfts_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/nfts_tokens_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/off_exchange_add.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/off_exchange_collateral_accounts_main_exchange_account_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/off_exchange_remove.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/off_exchange_settlements_trader.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/off_exchange_settlements_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/payments_payout.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/payments_payout_payout_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/payments_payout_payout_id_actions_execute.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/payments_xb_settlements_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/payments_xb_settlements_configs_config_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/payments_xb_settlements_flows.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/payments_xb_settlements_flows_flow_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/payments_xb_settlements_flows_flow_id_actions_execute.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/screeening_travel_rule_vasp_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/screening_travel_rule_transaction_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/screening_travel_rule_transaction_validate_full.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/screening_travel_rule_vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/screening_travel_rule_vasp_did.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/supported_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/tap_active_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/tap_draft.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/tap_publish.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/transactions_estimate_fee.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/transactions_external_tx_id_external_tx_id_.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/transactions_tx_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/transactions_tx_id_cancel.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/transactions_tx_id_drop.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/transactions_tx_id_freeze.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/transactions_tx_id_set_confirmation_threshold.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/transactions_tx_id_unfreeze.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/transactions_validate_address_asset_id_address.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/tx_hash_tx_hash_set_confirmation_threshold.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/users.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/users_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/users_groups_group_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/vault_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/vault_accounts_paged.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/vault_accounts_vault_account_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/vault_accounts_vault_account_id_asset_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/vault_accounts_vault_account_id_asset_id_activate.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/vault_accounts_vault_account_id_asset_id_addresses.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/vault_accounts_vault_account_id_asset_id_addresses_address_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/vault_accounts_vault_account_id_asset_id_addresses_address_id_create_legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/vault_accounts_vault_account_id_asset_id_addresses_address_id_set_customer_ref_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/vault_accounts_vault_account_id_asset_id_balance.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/vault_accounts_vault_account_id_asset_id_change_address_index_public_key_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/vault_accounts_vault_account_id_asset_id_max_spendable_amount.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/vault_accounts_vault_account_id_asset_id_unspent_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/vault_accounts_vault_account_id_hide.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/vault_accounts_vault_account_id_set_auto_fuel.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/vault_accounts_vault_account_id_set_customer_ref_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/vault_accounts_vault_account_id_unhide.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/vault_asset_wallets.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/vault_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/vault_assets_asset_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/vault_public_key_info_.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/webhooks_resend.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/paths/webhooks_resend_tx_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/tag_to_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.486916 fireblocks-0.0.1/fireblocks_client/apis/tags/
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/tags/audit_logs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/tags/blockchains_assets_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/tags/contracts_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/tags/exchange_accounts_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/tags/external_wallets_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/tags/fiat_accounts_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/tags/gas_stations_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/tags/internal_wallets_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/tags/network_connections_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/tags/nfts_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/tags/nfts_beta_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/tags/off_exchanges_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/tags/ota_beta_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/tags/payments_cross_border_settlement_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/tags/payments_payout_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/tags/policy_editor_beta_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/tags/transactions_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/tags/travel_rule_beta_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/tags/users_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/tags/users_groups_beta_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/tags/vaults_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/tags/web3_connections_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/apis/tags/webhooks_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    15852 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4528 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.546917 fireblocks-0.0.1/fireblocks_client/model/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/add_collateral_request_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/add_collateral_request_body.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/aml_screening_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/aml_screening_result.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/amount_aggregation_time_period_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/amount_aggregation_time_period_method.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4243 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/amount_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4243 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/amount_info.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7205 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/asset_type_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6604 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/asset_type_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7921 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/asset_wallet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7921 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/asset_wallet.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5333 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/authorization_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/authorization_groups.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5435 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/authorization_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/authorization_info.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/block_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/block_info.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/cancel_transaction_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/cancel_transaction_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/collection_ownership_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6001 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/collection_ownership_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/config_change_request_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/config_change_request_status.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/create_address_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/create_address_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/create_connection_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/create_connection_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5058 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/create_connection_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5058 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/create_connection_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/create_internal_transfer_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/create_internal_transfer_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4354 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/create_payout_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4354 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/create_payout_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/create_transaction_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/create_transaction_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/create_users_group_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/create_users_group_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/create_vault_asset_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/create_vault_asset_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/custom_crypto_routing_dest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4144 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/custom_crypto_routing_dest.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4366 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/custom_fiat_routing_dest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/custom_fiat_routing_dest.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/default_network_routing_dest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/default_network_routing_dest.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/destination_transfer_peer_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/destination_transfer_peer_path.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6006 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/destination_transfer_peer_path_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6006 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/destination_transfer_peer_path_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/dispatch_payout_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/dispatch_payout_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/draft_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/draft_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/draft_review_and_validation_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/draft_review_and_validation_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/drop_transaction_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/drop_transaction_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/drop_transaction_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/drop_transaction_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7649 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6992 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/error_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/estimated_network_fee_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/estimated_network_fee_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/estimated_transaction_fee_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/estimated_transaction_fee_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8299 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/exchange_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     8299 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/exchange_account.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4570 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/exchange_asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4570 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/exchange_asset.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4412 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/exchange_trading_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     4412 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/exchange_trading_account.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/exchange_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/exchange_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7502 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/external_wallet_asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7502 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/external_wallet_asset.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/fee_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/fee_info.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5472 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/fiat_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     5472 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/fiat_account.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/fiat_account_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/fiat_account_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/fiat_asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/fiat_asset.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/freeze_transaction_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/freeze_transaction_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/gas_station_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/gas_station_configuration.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/gas_station_properties_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/gas_station_properties_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/get_connections_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/get_connections_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      680 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/get_settlement_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/get_settlement_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5221 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/get_transaction_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4688 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/get_transaction_operation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/get_users_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/get_users_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/instruction_amount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/instruction_amount.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4857 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/media_entity_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/media_entity_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/ncw.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/ncw.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/network_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/network_channel.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/network_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/network_connection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10231 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/network_connection_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10231 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/network_connection_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14734 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/network_connection_routing_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    14734 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/network_connection_routing_policy.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/network_fee.py
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/network_fee.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/network_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/network_id.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5252 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/network_id_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5252 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/network_id_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14352 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/network_id_routing_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    14352 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/network_id_routing_policy.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9667 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/network_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     9667 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/network_record.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/none_network_routing_dest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/none_network_routing_dest.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/one_time_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/one_time_address.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6919 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/paginated_asset_wallet_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6919 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/paginated_asset_wallet_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/paging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/paging.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/payee_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/payee_account.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/payee_account_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/payee_account_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/payee_account_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/payee_account_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/payment_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/payment_account.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/payment_account_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/payment_account_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/payment_account_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/payment_account_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/payout_init_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/payout_init_method.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/payout_instruction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/payout_instruction.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6058 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/payout_instruction_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6058 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/payout_instruction_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/payout_instruction_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/payout_instruction_state.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8602 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/payout_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     8602 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/payout_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/payout_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/payout_state.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/payout_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/payout_status.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3346 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/policy_and_validation_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3346 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/policy_and_validation_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/policy_check_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/policy_check_result.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4213 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/policy_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4213 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/policy_metadata.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/policy_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/policy_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    90219 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/policy_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    87753 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/policy_rule.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5120 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/policy_rule_check_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4915 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/policy_rule_check_result.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6440 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/policy_rule_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     5810 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/policy_rule_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      679 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/policy_src_or_dest_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/policy_src_or_dest_id.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/policy_src_or_dest_sub_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/policy_src_or_dest_sub_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/policy_src_or_dest_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/policy_src_or_dest_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/policy_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/policy_status.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/policy_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/policy_validation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4555 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/public_key_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     4555 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/public_key_information.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/publish_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/publish_result.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/remove_collateral_request_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/remove_collateral_request_body.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/request_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/request_options.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/resend_webhooks_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/resend_webhooks_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/respond_to_connection_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/respond_to_connection_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3322 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/reward_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3322 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/reward_info.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/rewards_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/rewards_info.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11726 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/session_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)    11086 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/session_dto.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/session_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/session_metadata.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/set_confirmations_threshold_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/set_confirmations_threshold_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/set_confirmations_threshold_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/set_confirmations_threshold_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/settlement_request_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/settlement_request_body.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5251 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/settlement_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5251 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/settlement_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10296 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/signed_message.py
--rw-r--r--   0 runner    (1001) docker     (127)    10045 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/signed_message.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5996 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/source_transfer_peer_path_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5996 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/source_transfer_peer_path_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/system_message_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/system_message_info.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5189 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/term.py
--rw-r--r--   0 runner    (1001) docker     (127)     5189 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/term.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4525 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/to_collateral_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4525 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/to_collateral_transaction.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/to_exchange_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/to_exchange_transaction.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/token_collection_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/token_collection_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14206 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/token_ownership_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    13879 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/token_ownership_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11494 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11167 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/token_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/trading_account_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/trading_account_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8132 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/transaction.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/transaction_fee.py
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/transaction_fee.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/transaction_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/transaction_operation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    33572 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/transaction_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    33327 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/transaction_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/transaction_request_destination.py
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/transaction_request_destination.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    38298 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/transaction_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    38073 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/transaction_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7201 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/transaction_response_destination.py
--rw-r--r--   0 runner    (1001) docker     (127)     7201 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/transaction_response_destination.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12927 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/transfer_peer_path.py
--rw-r--r--   0 runner    (1001) docker     (127)    10531 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/transfer_peer_path.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4072 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/travel_rule_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     4072 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/travel_rule_address.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/travel_rule_get_all_vasps_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/travel_rule_get_all_vasps_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/travel_rule_issuer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/travel_rule_issuer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10605 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/travel_rule_issuers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10605 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/travel_rule_issuers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/travel_rule_ownership_proof.py
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/travel_rule_ownership_proof.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7716 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/travel_rule_pii_ivms.py
--rw-r--r--   0 runner    (1001) docker     (127)     7716 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/travel_rule_pii_ivms.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/travel_rule_transaction_blockchain_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/travel_rule_transaction_blockchain_info.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/travel_rule_update_vasp_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/travel_rule_update_vasp_details.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    25325 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/travel_rule_validate_full_transaction_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    25325 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/travel_rule_validate_full_transaction_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11732 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/travel_rule_validate_transaction_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11732 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/travel_rule_validate_transaction_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7213 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/travel_rule_validate_transaction_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     7213 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/travel_rule_validate_transaction_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    29687 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/travel_rule_vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)    29687 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/travel_rule_vasp.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/unfreeze_transaction_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/unfreeze_transaction_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5268 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/unmanaged_wallet.py
--rw-r--r--   0 runner    (1001) docker     (127)     5268 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/unmanaged_wallet.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5279 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/unsigned_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     5279 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/unsigned_message.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/unspent_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/unspent_input.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/unspent_inputs_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/unspent_inputs_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/update_token_ownership_status_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/update_token_ownership_status_dto.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3894 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/user_group_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3894 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/user_group_create_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4789 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/user_group_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4789 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/user_group_create_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3894 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/user_group_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3894 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/user_group_update_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/user_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/user_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4779 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/users_group_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4779 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/users_group_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/users_groups_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/users_groups_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/validate_address_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/validate_address_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6033 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/vault_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     6033 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/vault_account.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7954 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/vault_accounts_paged_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     7954 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/vault_accounts_paged_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11729 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/vault_asset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11729 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/vault_asset.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8781 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/vault_wallet_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     8570 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/vault_wallet_address.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5833 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/wallet_asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5833 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/wallet_asset.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12047 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/wallet_asset_additional_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    12047 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/wallet_asset_additional_info.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_asset.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_asset_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_asset_id.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_config_creation_request_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_config_creation_request_body.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      693 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_config_creation_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_config_creation_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      693 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_config_deletion_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_config_deletion_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_config_edit_request_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_config_edit_request_body.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      689 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_config_edit_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_config_edit_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      683 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_config_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_config_id.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6190 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_config_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6190 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_config_model.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_config_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_config_step.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6460 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_config_steps_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     6460 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_config_steps_record.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_conversion_slippage_basis_points.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_conversion_slippage_basis_points.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_corridor_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_corridor_id.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_create_flow_request_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_create_flow_request_body.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      689 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_create_flow_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_create_flow_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_crypto_asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_crypto_asset.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_fiat_asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_fiat_asset.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_flow_execution_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_flow_execution_model.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_flow_execution_request_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_flow_execution_request_body.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      692 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_flow_execution_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_flow_execution_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_flow_execution_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_flow_execution_status.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7512 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_flow_execution_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     7512 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_flow_execution_step.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_flow_execution_step_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_flow_execution_step_status.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7292 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_flow_preview_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7292 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_flow_preview_model.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_flow_selected_conversion_slippage_reason.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_flow_selected_conversion_slippage_reason.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_flow_setup_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_flow_setup_step.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_flow_steps_execution_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_flow_steps_execution_record.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_flow_steps_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_flow_steps_record.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_get_all_configs_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_get_all_configs_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      688 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_get_config_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_get_config_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_get_flow_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_get_flow_response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_step_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/model/xb_settlement_step_type.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.546917 fireblocks-0.0.1/fireblocks_client/models/
--rw-r--r--   0 runner    (1001) docker     (127)    15755 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.546917 fireblocks-0.0.1/fireblocks_client/paths/
--rw-r--r--   0 runner    (1001) docker     (127)     7894 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.550917 fireblocks-0.0.1/fireblocks_client/paths/audits/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/audits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6219 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/audits/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/audits/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.550917 fireblocks-0.0.1/fireblocks_client/paths/connections/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14120 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/connections/get.py
--rw-r--r--   0 runner    (1001) docker     (127)    13045 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/connections/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.550917 fireblocks-0.0.1/fireblocks_client/paths/connections_wc/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/connections_wc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5767 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/connections_wc/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     5167 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/connections_wc/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.550917 fireblocks-0.0.1/fireblocks_client/paths/connections_wc_id/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/connections_wc_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/connections_wc_id/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/connections_wc_id/delete.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7443 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/connections_wc_id/put.py
--rw-r--r--   0 runner    (1001) docker     (127)     6660 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/connections_wc_id/put.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.550917 fireblocks-0.0.1/fireblocks_client/paths/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5164 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/contracts/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     4739 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/contracts/get.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7196 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/contracts/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     6771 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/contracts/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.550917 fireblocks-0.0.1/fireblocks_client/paths/contracts_contract_id/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/contracts_contract_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5861 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/contracts_contract_id/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     5436 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/contracts_contract_id/delete.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6123 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/contracts_contract_id/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     5698 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/contracts_contract_id/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.554917 fireblocks-0.0.1/fireblocks_client/paths/contracts_contract_id_asset_id/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/contracts_contract_id_asset_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6240 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/contracts_contract_id_asset_id/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     5815 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/contracts_contract_id_asset_id/delete.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6468 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/contracts_contract_id_asset_id/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     6043 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/contracts_contract_id_asset_id/get.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9537 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/contracts_contract_id_asset_id/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     9112 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/contracts_contract_id_asset_id/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.554917 fireblocks-0.0.1/fireblocks_client/paths/estimate_network_fee/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/estimate_network_fee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6244 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/estimate_network_fee/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     5819 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/estimate_network_fee/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.554917 fireblocks-0.0.1/fireblocks_client/paths/exchange_accounts/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/exchange_accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/exchange_accounts/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/exchange_accounts/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.554917 fireblocks-0.0.1/fireblocks_client/paths/exchange_accounts_exchange_account_id/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/exchange_accounts_exchange_account_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6229 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/exchange_accounts_exchange_account_id/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     5804 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/exchange_accounts_exchange_account_id/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.554917 fireblocks-0.0.1/fireblocks_client/paths/exchange_accounts_exchange_account_id_asset_id/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/exchange_accounts_exchange_account_id_asset_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6549 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/exchange_accounts_exchange_account_id_asset_id/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     6124 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/exchange_accounts_exchange_account_id_asset_id/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.554917 fireblocks-0.0.1/fireblocks_client/paths/exchange_accounts_exchange_account_id_convert/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/exchange_accounts_exchange_account_id_convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9758 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/exchange_accounts_exchange_account_id_convert/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     9333 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/exchange_accounts_exchange_account_id_convert/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.558917 fireblocks-0.0.1/fireblocks_client/paths/exchange_accounts_exchange_account_id_internal_transfer/
--rw-r--r--   0 runner    (1001) docker     (127)      403 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/exchange_accounts_exchange_account_id_internal_transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6833 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/exchange_accounts_exchange_account_id_internal_transfer/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     6408 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/exchange_accounts_exchange_account_id_internal_transfer/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.558917 fireblocks-0.0.1/fireblocks_client/paths/external_wallets/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/external_wallets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/external_wallets/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     4780 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/external_wallets/get.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7834 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/external_wallets/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     7409 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/external_wallets/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.558917 fireblocks-0.0.1/fireblocks_client/paths/external_wallets_wallet_id/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/external_wallets_wallet_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5887 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/external_wallets_wallet_id/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     5462 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/external_wallets_wallet_id/delete.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/external_wallets_wallet_id/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     5715 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/external_wallets_wallet_id/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.558917 fireblocks-0.0.1/fireblocks_client/paths/external_wallets_wallet_id_asset_id/
--rw-r--r--   0 runner    (1001) docker     (127)      363 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/external_wallets_wallet_id_asset_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/external_wallets_wallet_id_asset_id/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/external_wallets_wallet_id_asset_id/delete.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6501 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/external_wallets_wallet_id_asset_id/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     6076 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/external_wallets_wallet_id_asset_id/get.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    47470 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/external_wallets_wallet_id_asset_id/post.py
--rw-r--r--   0 runner    (1001) docker     (127)    47045 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/external_wallets_wallet_id_asset_id/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.558917 fireblocks-0.0.1/fireblocks_client/paths/external_wallets_wallet_id_set_customer_ref_id/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/external_wallets_wallet_id_set_customer_ref_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8642 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/external_wallets_wallet_id_set_customer_ref_id/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     8217 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/external_wallets_wallet_id_set_customer_ref_id/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.558917 fireblocks-0.0.1/fireblocks_client/paths/fiat_accounts/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/fiat_accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5159 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/fiat_accounts/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/fiat_accounts/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.562917 fireblocks-0.0.1/fireblocks_client/paths/fiat_accounts_account_id/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/fiat_accounts_account_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/fiat_accounts_account_id/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/fiat_accounts_account_id/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.562917 fireblocks-0.0.1/fireblocks_client/paths/fiat_accounts_account_id_deposit_from_linked_dda/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/fiat_accounts_account_id_deposit_from_linked_dda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8486 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/fiat_accounts_account_id_deposit_from_linked_dda/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     8061 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/fiat_accounts_account_id_deposit_from_linked_dda/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.562917 fireblocks-0.0.1/fireblocks_client/paths/fiat_accounts_account_id_redeem_to_linked_dda/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/fiat_accounts_account_id_redeem_to_linked_dda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8468 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/fiat_accounts_account_id_redeem_to_linked_dda/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     8043 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/fiat_accounts_account_id_redeem_to_linked_dda/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.562917 fireblocks-0.0.1/fireblocks_client/paths/gas_station/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/gas_station/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/gas_station/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/gas_station/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.562917 fireblocks-0.0.1/fireblocks_client/paths/gas_station_asset_id/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/gas_station_asset_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6192 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/gas_station_asset_id/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     5767 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/gas_station_asset_id/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.562917 fireblocks-0.0.1/fireblocks_client/paths/gas_station_configuration/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/gas_station_configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5393 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/gas_station_configuration/put.py
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/gas_station_configuration/put.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.562917 fireblocks-0.0.1/fireblocks_client/paths/gas_station_configuration_asset_id/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/gas_station_configuration_asset_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/gas_station_configuration_asset_id/put.py
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/gas_station_configuration_asset_id/put.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.562917 fireblocks-0.0.1/fireblocks_client/paths/internal_wallets/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/internal_wallets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/internal_wallets/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     4780 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/internal_wallets/get.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7834 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/internal_wallets/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     7409 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/internal_wallets/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.562917 fireblocks-0.0.1/fireblocks_client/paths/internal_wallets_wallet_id/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/internal_wallets_wallet_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5887 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/internal_wallets_wallet_id/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     5462 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/internal_wallets_wallet_id/delete.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/internal_wallets_wallet_id/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     5722 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/internal_wallets_wallet_id/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.566917 fireblocks-0.0.1/fireblocks_client/paths/internal_wallets_wallet_id_asset_id/
--rw-r--r--   0 runner    (1001) docker     (127)      363 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/internal_wallets_wallet_id_asset_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6263 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/internal_wallets_wallet_id_asset_id/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     5838 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/internal_wallets_wallet_id_asset_id/delete.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6462 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/internal_wallets_wallet_id_asset_id/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     6037 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/internal_wallets_wallet_id_asset_id/get.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9539 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/internal_wallets_wallet_id_asset_id/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     9114 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/internal_wallets_wallet_id_asset_id/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.566917 fireblocks-0.0.1/fireblocks_client/paths/internal_wallets_wallet_id_set_customer_ref_id/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/internal_wallets_wallet_id_set_customer_ref_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8646 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/internal_wallets_wallet_id_set_customer_ref_id/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     8221 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/internal_wallets_wallet_id_set_customer_ref_id/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.566917 fireblocks-0.0.1/fireblocks_client/paths/management_ota/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/management_ota/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5136 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/management_ota/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     5025 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/management_ota/get.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6299 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/management_ota/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/management_ota/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.566917 fireblocks-0.0.1/fireblocks_client/paths/network_connections/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/network_connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5294 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/network_connections/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     4869 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/network_connections/get.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5599 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/network_connections/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/network_connections/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.566917 fireblocks-0.0.1/fireblocks_client/paths/network_connections_connection_id/
--rw-r--r--   0 runner    (1001) docker     (127)      359 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/network_connections_connection_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7984 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/network_connections_connection_id/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     7559 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/network_connections_connection_id/delete.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6219 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/network_connections_connection_id/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/network_connections_connection_id/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.566917 fireblocks-0.0.1/fireblocks_client/paths/network_connections_connection_id_is_third_party_routing_asset_type/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/network_connections_connection_id_is_third_party_routing_asset_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9819 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/network_connections_connection_id_is_third_party_routing_asset_type/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     9163 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/network_connections_connection_id_is_third_party_routing_asset_type/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.566917 fireblocks-0.0.1/fireblocks_client/paths/network_connections_connection_id_set_routing_policy/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/network_connections_connection_id_set_routing_policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10957 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/network_connections_connection_id_set_routing_policy/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)    10532 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/network_connections_connection_id_set_routing_policy/patch.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.570917 fireblocks-0.0.1/fireblocks_client/paths/network_ids/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/network_ids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7030 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/network_ids/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     6605 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/network_ids/get.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8010 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/network_ids/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     7585 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/network_ids/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.570917 fireblocks-0.0.1/fireblocks_client/paths/network_ids_network_id/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/network_ids_network_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7542 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/network_ids_network_id/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     7270 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/network_ids_network_id/delete.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6135 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/network_ids_network_id/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     5710 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/network_ids_network_id/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.570917 fireblocks-0.0.1/fireblocks_client/paths/network_ids_network_id_set_discoverability/
--rw-r--r--   0 runner    (1001) docker     (127)      377 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/network_ids_network_id_set_discoverability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10735 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/network_ids_network_id_set_discoverability/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)    10310 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/network_ids_network_id_set_discoverability/patch.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.570917 fireblocks-0.0.1/fireblocks_client/paths/network_ids_network_id_set_name/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/network_ids_network_id_set_name/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10488 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/network_ids_network_id_set_name/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)    10063 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/network_ids_network_id_set_name/patch.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.570917 fireblocks-0.0.1/fireblocks_client/paths/network_ids_network_id_set_routing_policy/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/network_ids_network_id_set_routing_policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10821 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/network_ids_network_id_set_routing_policy/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)    10396 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/network_ids_network_id_set_routing_policy/patch.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.570917 fireblocks-0.0.1/fireblocks_client/paths/nfts_ownership_collections/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/nfts_ownership_collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11285 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/nfts_ownership_collections/get.py
--rw-r--r--   0 runner    (1001) docker     (127)    10707 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/nfts_ownership_collections/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.570917 fireblocks-0.0.1/fireblocks_client/paths/nfts_ownership_tokens/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/nfts_ownership_tokens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14995 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/nfts_ownership_tokens/get.py
--rw-r--r--   0 runner    (1001) docker     (127)    13863 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/nfts_ownership_tokens/get.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5801 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/nfts_ownership_tokens/put.py
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/nfts_ownership_tokens/put.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.570917 fireblocks-0.0.1/fireblocks_client/paths/nfts_ownership_tokens_id_status/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/nfts_ownership_tokens_id_status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/nfts_ownership_tokens_id_status/put.py
--rw-r--r--   0 runner    (1001) docker     (127)     5313 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/nfts_ownership_tokens_id_status/put.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.574917 fireblocks-0.0.1/fireblocks_client/paths/nfts_tokens/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/nfts_tokens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11456 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/nfts_tokens/get.py
--rw-r--r--   0 runner    (1001) docker     (127)    10764 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/nfts_tokens/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.574917 fireblocks-0.0.1/fireblocks_client/paths/nfts_tokens_id/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/nfts_tokens_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4869 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/nfts_tokens_id/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/nfts_tokens_id/get.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/nfts_tokens_id/put.py
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/nfts_tokens_id/put.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.574917 fireblocks-0.0.1/fireblocks_client/paths/off_exchange_add/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/off_exchange_add/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/off_exchange_add/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     4933 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/off_exchange_add/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.574917 fireblocks-0.0.1/fireblocks_client/paths/off_exchange_collateral_accounts_main_exchange_account_id/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/off_exchange_collateral_accounts_main_exchange_account_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6325 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/off_exchange_collateral_accounts_main_exchange_account_id/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     5900 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/off_exchange_collateral_accounts_main_exchange_account_id/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.574917 fireblocks-0.0.1/fireblocks_client/paths/off_exchange_remove/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/off_exchange_remove/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/off_exchange_remove/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/off_exchange_remove/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.574917 fireblocks-0.0.1/fireblocks_client/paths/off_exchange_settlements_trader/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/off_exchange_settlements_trader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/off_exchange_settlements_trader/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     4958 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/off_exchange_settlements_trader/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.574917 fireblocks-0.0.1/fireblocks_client/paths/off_exchange_settlements_transactions/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/off_exchange_settlements_transactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6095 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/off_exchange_settlements_transactions/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     5823 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/off_exchange_settlements_transactions/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.574917 fireblocks-0.0.1/fireblocks_client/paths/payments_payout/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/payments_payout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5661 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/payments_payout/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/payments_payout/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.574917 fireblocks-0.0.1/fireblocks_client/paths/payments_payout_payout_id/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/payments_payout_payout_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6255 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/payments_payout_payout_id/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     6084 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/payments_payout_payout_id/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.574917 fireblocks-0.0.1/fireblocks_client/paths/payments_payout_payout_id_actions_execute/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/payments_payout_payout_id_actions_execute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6299 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/payments_payout_payout_id_actions_execute/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/payments_payout_payout_id_actions_execute/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.578917 fireblocks-0.0.1/fireblocks_client/paths/payments_xb_settlements_configs/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/payments_xb_settlements_configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/payments_xb_settlements_configs/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/payments_xb_settlements_configs/get.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5876 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/payments_xb_settlements_configs/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     5705 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/payments_xb_settlements_configs/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.578917 fireblocks-0.0.1/fireblocks_client/paths/payments_xb_settlements_configs_config_id/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/payments_xb_settlements_configs_config_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6352 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/payments_xb_settlements_configs_config_id/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     6181 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/payments_xb_settlements_configs_config_id/delete.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6362 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/payments_xb_settlements_configs_config_id/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     6191 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/payments_xb_settlements_configs_config_id/get.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7780 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/payments_xb_settlements_configs_config_id/put.py
--rw-r--r--   0 runner    (1001) docker     (127)     7579 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/payments_xb_settlements_configs_config_id/put.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.578917 fireblocks-0.0.1/fireblocks_client/paths/payments_xb_settlements_flows/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/payments_xb_settlements_flows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5853 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/payments_xb_settlements_flows/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     5682 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/payments_xb_settlements_flows/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.578917 fireblocks-0.0.1/fireblocks_client/paths/payments_xb_settlements_flows_flow_id/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/payments_xb_settlements_flows_flow_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6346 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/payments_xb_settlements_flows_flow_id/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     6175 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/payments_xb_settlements_flows_flow_id/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.578917 fireblocks-0.0.1/fireblocks_client/paths/payments_xb_settlements_flows_flow_id_actions_execute/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/payments_xb_settlements_flows_flow_id_actions_execute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7825 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/payments_xb_settlements_flows_flow_id_actions_execute/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     7624 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/payments_xb_settlements_flows_flow_id_actions_execute/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.578917 fireblocks-0.0.1/fireblocks_client/paths/screeening_travel_rule_vasp_update/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/screeening_travel_rule_vasp_update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/screeening_travel_rule_vasp_update/put.py
--rw-r--r--   0 runner    (1001) docker     (127)     4604 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/screeening_travel_rule_vasp_update/put.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.578917 fireblocks-0.0.1/fireblocks_client/paths/screening_travel_rule_transaction_validate/
--rw-r--r--   0 runner    (1001) docker     (127)      377 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/screening_travel_rule_transaction_validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4893 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/screening_travel_rule_transaction_validate/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/screening_travel_rule_transaction_validate/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.582918 fireblocks-0.0.1/fireblocks_client/paths/screening_travel_rule_transaction_validate_full/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/screening_travel_rule_transaction_validate_full/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4945 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/screening_travel_rule_transaction_validate_full/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/screening_travel_rule_transaction_validate_full/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.582918 fireblocks-0.0.1/fireblocks_client/paths/screening_travel_rule_vasp/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/screening_travel_rule_vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5817 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/screening_travel_rule_vasp/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     5736 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/screening_travel_rule_vasp/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.582918 fireblocks-0.0.1/fireblocks_client/paths/screening_travel_rule_vasp_did/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/screening_travel_rule_vasp_did/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6582 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/screening_travel_rule_vasp_did/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/screening_travel_rule_vasp_did/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.582918 fireblocks-0.0.1/fireblocks_client/paths/supported_assets/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/supported_assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5243 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/supported_assets/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/supported_assets/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.582918 fireblocks-0.0.1/fireblocks_client/paths/tap_active_policy/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/tap_active_policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4640 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/tap_active_policy/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/tap_active_policy/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.582918 fireblocks-0.0.1/fireblocks_client/paths/tap_draft/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/tap_draft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/tap_draft/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/tap_draft/get.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7264 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/tap_draft/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     6839 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/tap_draft/post.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8215 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/tap_draft/put.py
--rw-r--r--   0 runner    (1001) docker     (127)     7790 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/tap_draft/put.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.582918 fireblocks-0.0.1/fireblocks_client/paths/tap_publish/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/tap_publish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8203 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/tap_publish/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     7778 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/tap_publish/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.586917 fireblocks-0.0.1/fireblocks_client/paths/transactions/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/transactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16113 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/transactions/get.py
--rw-r--r--   0 runner    (1001) docker     (127)    14071 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/transactions/get.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6018 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/transactions/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     5593 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/transactions/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.586917 fireblocks-0.0.1/fireblocks_client/paths/transactions_estimate_fee/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/transactions_estimate_fee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5610 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/transactions_estimate_fee/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     5185 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/transactions_estimate_fee/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.586917 fireblocks-0.0.1/fireblocks_client/paths/transactions_external_tx_id_external_tx_id_/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/transactions_external_tx_id_external_tx_id_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6243 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/transactions_external_tx_id_external_tx_id_/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     5818 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/transactions_external_tx_id_external_tx_id_/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.586917 fireblocks-0.0.1/fireblocks_client/paths/transactions_tx_id/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/transactions_tx_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7023 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/transactions_tx_id/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/transactions_tx_id/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.586917 fireblocks-0.0.1/fireblocks_client/paths/transactions_tx_id_cancel/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/transactions_tx_id_cancel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6107 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/transactions_tx_id_cancel/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     5682 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/transactions_tx_id_cancel/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.586917 fireblocks-0.0.1/fireblocks_client/paths/transactions_tx_id_drop/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/transactions_tx_id_drop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6947 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/transactions_tx_id_drop/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     6522 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/transactions_tx_id_drop/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.586917 fireblocks-0.0.1/fireblocks_client/paths/transactions_tx_id_freeze/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/transactions_tx_id_freeze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/transactions_tx_id_freeze/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     4677 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/transactions_tx_id_freeze/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.586917 fireblocks-0.0.1/fireblocks_client/paths/transactions_tx_id_set_confirmation_threshold/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/transactions_tx_id_set_confirmation_threshold/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7176 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/transactions_tx_id_set_confirmation_threshold/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     6751 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/transactions_tx_id_set_confirmation_threshold/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.590918 fireblocks-0.0.1/fireblocks_client/paths/transactions_tx_id_unfreeze/
--rw-r--r--   0 runner    (1001) docker     (127)      347 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/transactions_tx_id_unfreeze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4929 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/transactions_tx_id_unfreeze/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/transactions_tx_id_unfreeze/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.590918 fireblocks-0.0.1/fireblocks_client/paths/transactions_validate_address_asset_id_address/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/transactions_validate_address_asset_id_address/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6437 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/transactions_validate_address_asset_id_address/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     6012 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/transactions_validate_address_asset_id_address/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.590918 fireblocks-0.0.1/fireblocks_client/paths/tx_hash_tx_hash_set_confirmation_threshold/
--rw-r--r--   0 runner    (1001) docker     (127)      377 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/tx_hash_tx_hash_set_confirmation_threshold/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7232 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/tx_hash_tx_hash_set_confirmation_threshold/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     6807 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/tx_hash_tx_hash_set_confirmation_threshold/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.590918 fireblocks-0.0.1/fireblocks_client/paths/users/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4537 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/users/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/users/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.590918 fireblocks-0.0.1/fireblocks_client/paths/users_groups/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/users_groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/users_groups/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     4157 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/users_groups/get.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5593 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/users_groups/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     5168 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/users_groups/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.590918 fireblocks-0.0.1/fireblocks_client/paths/users_groups_group_id/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/users_groups_group_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5847 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/users_groups_group_id/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     5422 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/users_groups_group_id/delete.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6081 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/users_groups_group_id/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     5656 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/users_groups_group_id/get.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6987 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/users_groups_group_id/put.py
--rw-r--r--   0 runner    (1001) docker     (127)     6562 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/users_groups_group_id/put.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.594918 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8125 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     7700 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts/get.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8927 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     8502 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.594918 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_paged/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_paged/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8357 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_paged/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     7931 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_paged/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.594918 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6175 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id/get.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8449 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id/put.py
--rw-r--r--   0 runner    (1001) docker     (127)     8024 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id/put.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.594918 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6133 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     5861 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id/get.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9189 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     8764 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.594918 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_activate/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_activate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6591 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_activate/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     6166 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_activate/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.598918 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_addresses/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_addresses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7176 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_addresses/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     6751 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_addresses/get.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9788 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_addresses/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     9363 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_addresses/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.598918 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_addresses_address_id/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_addresses_address_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9249 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_addresses_address_id/put.py
--rw-r--r--   0 runner    (1001) docker     (127)     8824 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_addresses_address_id/put.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.598918 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_addresses_address_id_create_legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      443 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_addresses_address_id_create_legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6985 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_addresses_address_id_create_legacy/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     6560 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_addresses_address_id_create_legacy/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.598918 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_addresses_address_id_set_customer_ref_id/
--rw-r--r--   0 runner    (1001) docker     (127)      455 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_addresses_address_id_set_customer_ref_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9384 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_addresses_address_id_set_customer_ref_id/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     8959 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_addresses_address_id_set_customer_ref_id/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.598918 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_balance/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_balance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7181 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_balance/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     6756 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_balance/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.598918 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_change_address_index_public_key_info/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_change_address_index_public_key_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8784 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_change_address_index_public_key_info/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     8359 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_change_address_index_public_key_info/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.602918 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_max_spendable_amount/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_max_spendable_amount/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7825 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_max_spendable_amount/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     7400 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_max_spendable_amount/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.602918 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_unspent_inputs/
--rw-r--r--   0 runner    (1001) docker     (127)      403 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_unspent_inputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7237 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_unspent_inputs/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     6812 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_asset_id_unspent_inputs/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.602918 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_hide/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_hide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_hide/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     5497 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_hide/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.602918 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_set_auto_fuel/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_set_auto_fuel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8562 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_set_auto_fuel/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     8137 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_set_auto_fuel/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.602918 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_set_customer_ref_id/
--rw-r--r--   0 runner    (1001) docker     (127)      395 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_set_customer_ref_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8684 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_set_customer_ref_id/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     8259 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_set_customer_ref_id/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.602918 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_unhide/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_unhide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5934 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_unhide/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_accounts_vault_account_id_unhide/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.602918 fireblocks-0.0.1/fireblocks_client/paths/vault_asset_wallets/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_asset_wallets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6819 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_asset_wallets/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     6509 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_asset_wallets/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.602918 fireblocks-0.0.1/fireblocks_client/paths/vault_assets/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7339 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_assets/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     6914 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_assets/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.606918 fireblocks-0.0.1/fireblocks_client/paths/vault_assets_asset_id/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_assets_asset_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6100 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_assets_asset_id/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     5675 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_assets_asset_id/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.606918 fireblocks-0.0.1/fireblocks_client/paths/vault_public_key_info_/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_public_key_info_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_public_key_info_/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     6700 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/vault_public_key_info_/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.606918 fireblocks-0.0.1/fireblocks_client/paths/webhooks_resend/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/webhooks_resend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/webhooks_resend/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/webhooks_resend/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.606918 fireblocks-0.0.1/fireblocks_client/paths/webhooks_resend_tx_id/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/webhooks_resend_tx_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9242 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/webhooks_resend_tx_id/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     8817 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/paths/webhooks_resend_tx_id/post.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9409 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)   103287 2023-12-01 21:50:09.000000 fireblocks-0.0.1/fireblocks_client/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-12-01 21:50:22.678919 fireblocks-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2023-12-01 21:50:09.000000 fireblocks-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.454916 fireblocks-0.0.1/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.638918 fireblocks-0.0.1/test/test_models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_add_collateral_request_body.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_aml_screening_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_amount_aggregation_time_period_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_amount_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_asset_type_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_asset_wallet.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_authorization_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_authorization_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_block_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_cancel_transaction_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_collection_ownership_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_config_change_request_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_create_address_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_create_connection_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_create_connection_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_create_internal_transfer_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_create_payout_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_create_transaction_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_create_users_group_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_create_vault_asset_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_custom_crypto_routing_dest.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_custom_fiat_routing_dest.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_default_network_routing_dest.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_destination_transfer_peer_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_destination_transfer_peer_path_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_dispatch_payout_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_draft_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_draft_review_and_validation_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_drop_transaction_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_drop_transaction_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_estimated_network_fee_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_estimated_transaction_fee_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_exchange_account.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_exchange_asset.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_exchange_trading_account.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_exchange_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_external_wallet_asset.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_fee_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_fiat_account.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_fiat_account_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_fiat_asset.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_freeze_transaction_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_gas_station_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_gas_station_properties_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_get_connections_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_get_settlement_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_get_transaction_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_get_users_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_instruction_amount.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_media_entity_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_ncw.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_network_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_network_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_network_connection_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_network_connection_routing_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_network_fee.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_network_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_network_id_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_network_id_routing_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_network_record.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_none_network_routing_dest.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_one_time_address.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_paginated_asset_wallet_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_paging.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_payee_account.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_payee_account_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_payee_account_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_payment_account.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_payment_account_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_payment_account_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_payout_init_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_payout_instruction.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_payout_instruction_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_payout_instruction_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_payout_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_payout_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_payout_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_policy_and_validation_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_policy_check_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_policy_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_policy_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_policy_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_policy_rule_check_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_policy_rule_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_policy_src_or_dest_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_policy_src_or_dest_sub_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_policy_src_or_dest_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_policy_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_policy_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_public_key_information.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_publish_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_remove_collateral_request_body.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_request_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_resend_webhooks_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_respond_to_connection_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_reward_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_rewards_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_session_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_session_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_set_confirmations_threshold_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_set_confirmations_threshold_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_settlement_request_body.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_settlement_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_signed_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_source_transfer_peer_path_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_system_message_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_term.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_to_collateral_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_to_exchange_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_token_collection_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_token_ownership_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_trading_account_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_transaction_fee.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_transaction_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_transaction_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_transaction_request_destination.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_transaction_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_transaction_response_destination.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_transfer_peer_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_travel_rule_address.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_travel_rule_get_all_vasps_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_travel_rule_issuer.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_travel_rule_issuers.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_travel_rule_ownership_proof.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_travel_rule_pii_ivms.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_travel_rule_transaction_blockchain_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_travel_rule_update_vasp_details.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_travel_rule_validate_full_transaction_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_travel_rule_validate_transaction_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_travel_rule_validate_transaction_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_travel_rule_vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_unfreeze_transaction_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_unmanaged_wallet.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_unsigned_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_unspent_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_unspent_inputs_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_update_token_ownership_status_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_user_group_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_user_group_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_user_group_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_user_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_users_group_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_users_groups_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_validate_address_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_vault_account.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_vault_accounts_paged_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_vault_asset.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_vault_wallet_address.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_wallet_asset.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_wallet_asset_additional_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_xb_settlement_asset.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_xb_settlement_asset_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_xb_settlement_config_creation_request_body.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_xb_settlement_config_creation_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_xb_settlement_config_deletion_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_xb_settlement_config_edit_request_body.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_xb_settlement_config_edit_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_xb_settlement_config_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_xb_settlement_config_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_xb_settlement_config_step.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_xb_settlement_config_steps_record.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_xb_settlement_conversion_slippage_basis_points.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_xb_settlement_corridor_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_xb_settlement_create_flow_request_body.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_xb_settlement_create_flow_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_xb_settlement_crypto_asset.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_xb_settlement_fiat_asset.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_xb_settlement_flow_execution_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_xb_settlement_flow_execution_request_body.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_xb_settlement_flow_execution_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_xb_settlement_flow_execution_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_xb_settlement_flow_execution_step.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_xb_settlement_flow_execution_step_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_xb_settlement_flow_preview_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_xb_settlement_flow_selected_conversion_slippage_reason.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_xb_settlement_flow_setup_step.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_xb_settlement_flow_steps_execution_record.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_xb_settlement_flow_steps_record.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_xb_settlement_get_all_configs_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_xb_settlement_get_config_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_xb_settlement_get_flow_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_models/test_xb_settlement_step_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.638918 fireblocks-0.0.1/test/test_paths/
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.638918 fireblocks-0.0.1/test/test_paths/test_audits/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_audits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_audits/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.638918 fireblocks-0.0.1/test/test_paths/test_connections/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_connections/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.638918 fireblocks-0.0.1/test/test_paths/test_connections_wc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_connections_wc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_connections_wc/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.638918 fireblocks-0.0.1/test/test_paths/test_connections_wc_id/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_connections_wc_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_connections_wc_id/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_connections_wc_id/test_put.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.638918 fireblocks-0.0.1/test/test_paths/test_contracts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_contracts/test_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_contracts/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.642918 fireblocks-0.0.1/test/test_paths/test_contracts_contract_id/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_contracts_contract_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_contracts_contract_id/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_contracts_contract_id/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.642918 fireblocks-0.0.1/test/test_paths/test_contracts_contract_id_asset_id/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_contracts_contract_id_asset_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_contracts_contract_id_asset_id/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_contracts_contract_id_asset_id/test_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_contracts_contract_id_asset_id/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.642918 fireblocks-0.0.1/test/test_paths/test_estimate_network_fee/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_estimate_network_fee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_estimate_network_fee/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.642918 fireblocks-0.0.1/test/test_paths/test_exchange_accounts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_exchange_accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_exchange_accounts/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.642918 fireblocks-0.0.1/test/test_paths/test_exchange_accounts_exchange_account_id/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_exchange_accounts_exchange_account_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_exchange_accounts_exchange_account_id/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.642918 fireblocks-0.0.1/test/test_paths/test_exchange_accounts_exchange_account_id_asset_id/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_exchange_accounts_exchange_account_id_asset_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_exchange_accounts_exchange_account_id_asset_id/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.642918 fireblocks-0.0.1/test/test_paths/test_exchange_accounts_exchange_account_id_convert/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_exchange_accounts_exchange_account_id_convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_exchange_accounts_exchange_account_id_convert/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.642918 fireblocks-0.0.1/test/test_paths/test_exchange_accounts_exchange_account_id_internal_transfer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_exchange_accounts_exchange_account_id_internal_transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_exchange_accounts_exchange_account_id_internal_transfer/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.642918 fireblocks-0.0.1/test/test_paths/test_external_wallets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_external_wallets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_external_wallets/test_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_external_wallets/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.642918 fireblocks-0.0.1/test/test_paths/test_external_wallets_wallet_id/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_external_wallets_wallet_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_external_wallets_wallet_id/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_external_wallets_wallet_id/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.646918 fireblocks-0.0.1/test/test_paths/test_external_wallets_wallet_id_asset_id/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_external_wallets_wallet_id_asset_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_external_wallets_wallet_id_asset_id/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_external_wallets_wallet_id_asset_id/test_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_external_wallets_wallet_id_asset_id/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.646918 fireblocks-0.0.1/test/test_paths/test_external_wallets_wallet_id_set_customer_ref_id/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_external_wallets_wallet_id_set_customer_ref_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_external_wallets_wallet_id_set_customer_ref_id/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.646918 fireblocks-0.0.1/test/test_paths/test_fiat_accounts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_fiat_accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_fiat_accounts/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.646918 fireblocks-0.0.1/test/test_paths/test_fiat_accounts_account_id/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_fiat_accounts_account_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_fiat_accounts_account_id/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.646918 fireblocks-0.0.1/test/test_paths/test_fiat_accounts_account_id_deposit_from_linked_dda/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_fiat_accounts_account_id_deposit_from_linked_dda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_fiat_accounts_account_id_deposit_from_linked_dda/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.646918 fireblocks-0.0.1/test/test_paths/test_fiat_accounts_account_id_redeem_to_linked_dda/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_fiat_accounts_account_id_redeem_to_linked_dda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_fiat_accounts_account_id_redeem_to_linked_dda/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.646918 fireblocks-0.0.1/test/test_paths/test_gas_station/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_gas_station/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_gas_station/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.646918 fireblocks-0.0.1/test/test_paths/test_gas_station_asset_id/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_gas_station_asset_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_gas_station_asset_id/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.646918 fireblocks-0.0.1/test/test_paths/test_gas_station_configuration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_gas_station_configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_gas_station_configuration/test_put.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.646918 fireblocks-0.0.1/test/test_paths/test_gas_station_configuration_asset_id/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_gas_station_configuration_asset_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_gas_station_configuration_asset_id/test_put.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.646918 fireblocks-0.0.1/test/test_paths/test_internal_wallets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_internal_wallets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_internal_wallets/test_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_internal_wallets/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.650918 fireblocks-0.0.1/test/test_paths/test_internal_wallets_wallet_id/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_internal_wallets_wallet_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_internal_wallets_wallet_id/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_internal_wallets_wallet_id/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.650918 fireblocks-0.0.1/test/test_paths/test_internal_wallets_wallet_id_asset_id/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_internal_wallets_wallet_id_asset_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_internal_wallets_wallet_id_asset_id/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_internal_wallets_wallet_id_asset_id/test_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_internal_wallets_wallet_id_asset_id/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.650918 fireblocks-0.0.1/test/test_paths/test_internal_wallets_wallet_id_set_customer_ref_id/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_internal_wallets_wallet_id_set_customer_ref_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_internal_wallets_wallet_id_set_customer_ref_id/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.650918 fireblocks-0.0.1/test/test_paths/test_management_ota/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_management_ota/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_management_ota/test_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_management_ota/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.650918 fireblocks-0.0.1/test/test_paths/test_network_connections/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_network_connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_network_connections/test_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_network_connections/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.650918 fireblocks-0.0.1/test/test_paths/test_network_connections_connection_id/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_network_connections_connection_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_network_connections_connection_id/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_network_connections_connection_id/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.650918 fireblocks-0.0.1/test/test_paths/test_network_connections_connection_id_is_third_party_routing_asset_type/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_network_connections_connection_id_is_third_party_routing_asset_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_network_connections_connection_id_is_third_party_routing_asset_type/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.650918 fireblocks-0.0.1/test/test_paths/test_network_connections_connection_id_set_routing_policy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_network_connections_connection_id_set_routing_policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_network_connections_connection_id_set_routing_policy/test_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.650918 fireblocks-0.0.1/test/test_paths/test_network_ids/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_network_ids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_network_ids/test_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_network_ids/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.654918 fireblocks-0.0.1/test/test_paths/test_network_ids_network_id/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_network_ids_network_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_network_ids_network_id/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_network_ids_network_id/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.654918 fireblocks-0.0.1/test/test_paths/test_network_ids_network_id_set_discoverability/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_network_ids_network_id_set_discoverability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_network_ids_network_id_set_discoverability/test_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.654918 fireblocks-0.0.1/test/test_paths/test_network_ids_network_id_set_name/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_network_ids_network_id_set_name/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_network_ids_network_id_set_name/test_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.654918 fireblocks-0.0.1/test/test_paths/test_network_ids_network_id_set_routing_policy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_network_ids_network_id_set_routing_policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_network_ids_network_id_set_routing_policy/test_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.654918 fireblocks-0.0.1/test/test_paths/test_nfts_ownership_collections/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_nfts_ownership_collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_nfts_ownership_collections/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.654918 fireblocks-0.0.1/test/test_paths/test_nfts_ownership_tokens/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_nfts_ownership_tokens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_nfts_ownership_tokens/test_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_nfts_ownership_tokens/test_put.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.654918 fireblocks-0.0.1/test/test_paths/test_nfts_ownership_tokens_id_status/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_nfts_ownership_tokens_id_status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_nfts_ownership_tokens_id_status/test_put.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.654918 fireblocks-0.0.1/test/test_paths/test_nfts_tokens/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_nfts_tokens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_nfts_tokens/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.654918 fireblocks-0.0.1/test/test_paths/test_nfts_tokens_id/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_nfts_tokens_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_nfts_tokens_id/test_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_nfts_tokens_id/test_put.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.654918 fireblocks-0.0.1/test/test_paths/test_off_exchange_add/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_off_exchange_add/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_off_exchange_add/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.654918 fireblocks-0.0.1/test/test_paths/test_off_exchange_collateral_accounts_main_exchange_account_id/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_off_exchange_collateral_accounts_main_exchange_account_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_off_exchange_collateral_accounts_main_exchange_account_id/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.658918 fireblocks-0.0.1/test/test_paths/test_off_exchange_remove/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_off_exchange_remove/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_off_exchange_remove/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.658918 fireblocks-0.0.1/test/test_paths/test_off_exchange_settlements_trader/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_off_exchange_settlements_trader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_off_exchange_settlements_trader/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.658918 fireblocks-0.0.1/test/test_paths/test_off_exchange_settlements_transactions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_off_exchange_settlements_transactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_off_exchange_settlements_transactions/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.658918 fireblocks-0.0.1/test/test_paths/test_payments_payout/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_payments_payout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_payments_payout/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.658918 fireblocks-0.0.1/test/test_paths/test_payments_payout_payout_id/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_payments_payout_payout_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_payments_payout_payout_id/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.658918 fireblocks-0.0.1/test/test_paths/test_payments_payout_payout_id_actions_execute/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_payments_payout_payout_id_actions_execute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_payments_payout_payout_id_actions_execute/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.658918 fireblocks-0.0.1/test/test_paths/test_payments_xb_settlements_configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_payments_xb_settlements_configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_payments_xb_settlements_configs/test_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_payments_xb_settlements_configs/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.658918 fireblocks-0.0.1/test/test_paths/test_payments_xb_settlements_configs_config_id/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_payments_xb_settlements_configs_config_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_payments_xb_settlements_configs_config_id/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_payments_xb_settlements_configs_config_id/test_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_payments_xb_settlements_configs_config_id/test_put.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.658918 fireblocks-0.0.1/test/test_paths/test_payments_xb_settlements_flows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_payments_xb_settlements_flows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_payments_xb_settlements_flows/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.658918 fireblocks-0.0.1/test/test_paths/test_payments_xb_settlements_flows_flow_id/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_payments_xb_settlements_flows_flow_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_payments_xb_settlements_flows_flow_id/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.658918 fireblocks-0.0.1/test/test_paths/test_payments_xb_settlements_flows_flow_id_actions_execute/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_payments_xb_settlements_flows_flow_id_actions_execute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_payments_xb_settlements_flows_flow_id_actions_execute/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.662918 fireblocks-0.0.1/test/test_paths/test_screeening_travel_rule_vasp_update/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_screeening_travel_rule_vasp_update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_screeening_travel_rule_vasp_update/test_put.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.662918 fireblocks-0.0.1/test/test_paths/test_screening_travel_rule_transaction_validate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_screening_travel_rule_transaction_validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_screening_travel_rule_transaction_validate/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.662918 fireblocks-0.0.1/test/test_paths/test_screening_travel_rule_transaction_validate_full/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_screening_travel_rule_transaction_validate_full/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_screening_travel_rule_transaction_validate_full/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.662918 fireblocks-0.0.1/test/test_paths/test_screening_travel_rule_vasp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_screening_travel_rule_vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_screening_travel_rule_vasp/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.662918 fireblocks-0.0.1/test/test_paths/test_screening_travel_rule_vasp_did/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_screening_travel_rule_vasp_did/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_screening_travel_rule_vasp_did/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.662918 fireblocks-0.0.1/test/test_paths/test_supported_assets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_supported_assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_supported_assets/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.662918 fireblocks-0.0.1/test/test_paths/test_tap_active_policy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_tap_active_policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_tap_active_policy/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.662918 fireblocks-0.0.1/test/test_paths/test_tap_draft/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_tap_draft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_tap_draft/test_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_tap_draft/test_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_tap_draft/test_put.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.662918 fireblocks-0.0.1/test/test_paths/test_tap_publish/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_tap_publish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_tap_publish/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.662918 fireblocks-0.0.1/test/test_paths/test_transactions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_transactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_transactions/test_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_transactions/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.662918 fireblocks-0.0.1/test/test_paths/test_transactions_estimate_fee/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_transactions_estimate_fee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_transactions_estimate_fee/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.666919 fireblocks-0.0.1/test/test_paths/test_transactions_external_tx_id_external_tx_id_/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_transactions_external_tx_id_external_tx_id_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_transactions_external_tx_id_external_tx_id_/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.666919 fireblocks-0.0.1/test/test_paths/test_transactions_tx_id/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_transactions_tx_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_transactions_tx_id/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.666919 fireblocks-0.0.1/test/test_paths/test_transactions_tx_id_cancel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_transactions_tx_id_cancel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_transactions_tx_id_cancel/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.666919 fireblocks-0.0.1/test/test_paths/test_transactions_tx_id_drop/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_transactions_tx_id_drop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_transactions_tx_id_drop/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.666919 fireblocks-0.0.1/test/test_paths/test_transactions_tx_id_freeze/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_transactions_tx_id_freeze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_transactions_tx_id_freeze/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.666919 fireblocks-0.0.1/test/test_paths/test_transactions_tx_id_set_confirmation_threshold/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_transactions_tx_id_set_confirmation_threshold/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_transactions_tx_id_set_confirmation_threshold/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.666919 fireblocks-0.0.1/test/test_paths/test_transactions_tx_id_unfreeze/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_transactions_tx_id_unfreeze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_transactions_tx_id_unfreeze/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.666919 fireblocks-0.0.1/test/test_paths/test_transactions_validate_address_asset_id_address/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_transactions_validate_address_asset_id_address/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_transactions_validate_address_asset_id_address/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.666919 fireblocks-0.0.1/test/test_paths/test_tx_hash_tx_hash_set_confirmation_threshold/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_tx_hash_tx_hash_set_confirmation_threshold/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_tx_hash_tx_hash_set_confirmation_threshold/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.666919 fireblocks-0.0.1/test/test_paths/test_users/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_users/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.666919 fireblocks-0.0.1/test/test_paths/test_users_groups/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_users_groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_users_groups/test_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_users_groups/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.670919 fireblocks-0.0.1/test/test_paths/test_users_groups_group_id/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_users_groups_group_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_users_groups_group_id/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_users_groups_group_id/test_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_users_groups_group_id/test_put.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.670919 fireblocks-0.0.1/test/test_paths/test_vault_accounts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts/test_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.670919 fireblocks-0.0.1/test/test_paths/test_vault_accounts_paged/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts_paged/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts_paged/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.670919 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id/test_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id/test_put.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.670919 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_asset_id/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_asset_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_asset_id/test_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_asset_id/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.670919 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_asset_id_activate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_asset_id_activate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_asset_id_activate/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.670919 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_asset_id_addresses/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_asset_id_addresses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_asset_id_addresses/test_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_asset_id_addresses/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.670919 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_asset_id_addresses_address_id/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_asset_id_addresses_address_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_asset_id_addresses_address_id/test_put.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.670919 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_asset_id_addresses_address_id_create_legacy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_asset_id_addresses_address_id_create_legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_asset_id_addresses_address_id_create_legacy/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.670919 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_asset_id_addresses_address_id_set_customer_ref_id/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_asset_id_addresses_address_id_set_customer_ref_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_asset_id_addresses_address_id_set_customer_ref_id/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.674919 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_asset_id_balance/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_asset_id_balance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_asset_id_balance/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.674919 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_asset_id_change_address_index_public_key_info/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_asset_id_change_address_index_public_key_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_asset_id_change_address_index_public_key_info/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.674919 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_asset_id_max_spendable_amount/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_asset_id_max_spendable_amount/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_asset_id_max_spendable_amount/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.674919 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_asset_id_unspent_inputs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_asset_id_unspent_inputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_asset_id_unspent_inputs/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.674919 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_hide/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_hide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_hide/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.674919 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_set_auto_fuel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_set_auto_fuel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_set_auto_fuel/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.674919 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_set_customer_ref_id/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_set_customer_ref_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_set_customer_ref_id/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.674919 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_unhide/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_unhide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_unhide/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.674919 fireblocks-0.0.1/test/test_paths/test_vault_asset_wallets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_asset_wallets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_asset_wallets/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.674919 fireblocks-0.0.1/test/test_paths/test_vault_assets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_assets/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.674919 fireblocks-0.0.1/test/test_paths/test_vault_assets_asset_id/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_assets_asset_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_assets_asset_id/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.674919 fireblocks-0.0.1/test/test_paths/test_vault_public_key_info_/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_public_key_info_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_vault_public_key_info_/test_get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.674919 fireblocks-0.0.1/test/test_paths/test_webhooks_resend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_webhooks_resend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_webhooks_resend/test_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:22.678919 fireblocks-0.0.1/test/test_paths/test_webhooks_resend_tx_id/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_webhooks_resend_tx_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2023-12-01 21:50:09.000000 fireblocks-0.0.1/test/test_paths/test_webhooks_resend_tx_id/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:02.927155 fireblocks-0.0.2b0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    70992 2024-05-30 14:05:02.927155 fireblocks-0.0.2b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    70231 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:02.771155 fireblocks-0.0.2b0/fireblocks/
+-rw-r--r--   0 runner    (1001) docker     (127)    38788 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/additional_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:02.779155 fireblocks-0.0.2b0/fireblocks/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11065 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/api_user_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/assets_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10507 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/audit_logs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11429 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/blockchains_assets_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32476 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/compliance_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/compliance_screening_configuration_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11166 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/console_user_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20081 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/contract_interactions_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39491 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/contract_templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35409 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/contracts_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26880 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/cosigners_beta_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16623 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/deployed_contracts_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28798 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/exchange_accounts_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41930 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/external_wallets_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21616 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/fiat_accounts_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21776 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/gas_stations_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42202 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/internal_wallets_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29874 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/job_management_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81855 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/network_connections_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64979 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/nfts_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28149 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/off_exchanges_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11062 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/ota_beta_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19060 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/payments_payout_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27654 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/policy_editor_beta_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/reset_device_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    94751 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/smart_transfer_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43041 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/staking_beta_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27427 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/tokenization_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78558 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/transactions_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31643 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/travel_rule_beta_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26750 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/user_groups_beta_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/users_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   146635 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/vaults_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23278 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/web3_connections_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12426 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/webhooks_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/whitelist_ip_addresses_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api/workspace_status_beta_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26508 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/base_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/bearer_token_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12483 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/client_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15930 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:02.851155 fireblocks-0.0.2b0/fireblocks/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    34746 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/abi_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/account_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/add_asset_to_external_wallet_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/add_asset_to_external_wallet_request_one_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/add_asset_to_external_wallet_request_one_of1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8609 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/add_asset_to_external_wallet_request_one_of1_additional_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/add_asset_to_external_wallet_request_one_of1_additional_info_one_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/add_asset_to_external_wallet_request_one_of1_additional_info_one_of1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/add_asset_to_external_wallet_request_one_of1_additional_info_one_of2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/add_collateral_request_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/add_contract_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/additional_info_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/aml_registration_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/aml_screening_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/amount_aggregation_time_period_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/amount_and_chain_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/amount_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/api_keys_paginated_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/api_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/asset_already_exist_http_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/asset_amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/asset_bad_request_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/asset_conflict_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/asset_does_not_exist_http_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/asset_forbidden_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/asset_internal_server_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/asset_metadata_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/asset_not_found_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/asset_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/asset_response_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/asset_response_onchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/asset_type_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/asset_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/audit_log_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/auditor_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/authorization_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/authorization_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/block_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/cancel_transaction_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/chain_info_response_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/collection_metadata_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/collection_ownership_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/compliance_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/compliance_screening_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/config_change_request_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/config_conversion_operation_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/config_disbursement_operation_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6679 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/config_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7154 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/config_operation_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/config_operation_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/config_transfer_operation_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/console_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/contract_abi_response_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/contract_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/contract_deploy_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/contract_deploy_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/contract_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/contract_metadata_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7409 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/contract_template_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/contract_upload_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/conversion_config_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/conversion_operation_config_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/conversion_operation_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/conversion_operation_execution_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/conversion_operation_execution_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/conversion_operation_execution_params_execution_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/conversion_operation_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/conversion_operation_preview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/conversion_operation_preview_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/conversion_operation_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/conversion_validation_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/convert_assets_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/convert_assets_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/cosigner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/cosigners_paginated_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/create_address_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/create_address_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/create_api_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/create_assets_bulk_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/create_assets_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7452 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/create_config_operation_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/create_connection_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/create_connection_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/create_console_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/create_contract_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/create_conversion_config_operation_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/create_disbursement_config_operation_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/create_internal_transfer_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/create_internal_wallet_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/create_multiple_accounts_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/create_ncw_connection_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/create_network_id_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/create_payout_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/create_token_request_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/create_token_request_dto_create_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/create_transaction_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/create_transfer_config_operation_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/create_user_group_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/create_vault_account_connection_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/create_vault_account_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/create_vault_asset_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/create_wallet_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/create_workflow_execution_request_params_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/custom_routing_dest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/default_network_routing_dest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/delegation_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/delegation_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/delete_network_connection_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/delete_network_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/deployed_contract_response_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/deployed_contracts_paginated_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/deposit_funds_from_linked_dda_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/destination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/destination_transfer_peer_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/destination_transfer_peer_path_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/disbursement_amount_instruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/disbursement_config_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/disbursement_instruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/disbursement_instruction_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/disbursement_operation_config_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/disbursement_operation_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/disbursement_operation_execution_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/disbursement_operation_execution_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/disbursement_operation_execution_params_execution_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/disbursement_operation_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/disbursement_operation_preview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/disbursement_operation_preview_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/disbursement_operation_preview_output_instruction_set_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/disbursement_operation_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/disbursement_percentage_instruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/disbursement_validation_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/dispatch_payout_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/draft_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/draft_review_and_validation_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/drop_transaction_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/drop_transaction_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/edit_gas_station_configuration_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/error_response_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/error_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/estimated_network_fee_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/estimated_transaction_fee_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/evm_token_create_params_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/exchange_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/exchange_accounts_paged.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/exchange_accounts_paged_paging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/exchange_asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3886 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/exchange_settlement_transactions_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/exchange_trading_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/exchange_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/execute_action_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6124 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/execute_action_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/execution_conversion_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/execution_disbursement_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/execution_operation_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/execution_screening_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/execution_transfer_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/external_wallet_asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/fee_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/fiat_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/fiat_account_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/fiat_asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/freeze_transaction_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/function_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/funds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/gas_station_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/gas_station_configuration_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/gas_station_properties_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/get_api_users_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/get_audit_logs_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/get_audit_logs_response_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/get_connections_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/get_console_users_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/get_filter_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/get_max_spendable_amount_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/get_nfts_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/get_ota_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/get_ownership_tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/get_transaction_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/get_whitelist_ip_addresses_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/get_workspace_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/http_contract_does_not_exist_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/instruction_amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/internal_transfer_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/job_created.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/lean_abi_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/lean_contract_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/lean_deployed_contract_response_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/list_owned_collections_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/list_owned_tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/media_entity_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/network_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/network_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/network_connection_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/network_connection_routing_policy_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/network_connection_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/network_fee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/network_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/network_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/network_id_routing_policy_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/network_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/none_network_routing_dest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/one_time_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/one_time_address_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/operation_execution_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/paginated_address_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/paginated_address_response_paging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/paginated_asset_wallet_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/paginated_asset_wallet_response_paging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/paging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/parameter_with_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/payee_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/payee_account_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/payee_account_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/payment_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/payment_account_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/payment_account_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/payout_init_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/payout_instruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/payout_instruction_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/payout_instruction_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/payout_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/payout_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/payout_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/policy_and_validation_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/policy_check_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/policy_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/policy_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15577 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/policy_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/policy_rule_amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/policy_rule_amount_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/policy_rule_authorization_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/policy_rule_authorization_groups_groups_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/policy_rule_check_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/policy_rule_designated_signers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/policy_rule_dst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/policy_rule_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/policy_rule_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/policy_rule_raw_message_signing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/policy_rule_raw_message_signing_derivation_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/policy_rule_src.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/policy_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/policy_src_or_dest_sub_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/policy_src_or_dest_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/policy_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/policy_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/pre_screening.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/provider_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/public_key_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/publish_draft_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/publish_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/read_abi_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/read_call_function_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/redeem_funds_to_linked_dda_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/register_new_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/related_transaction_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/remove_collateral_request_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/rename_cosigner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/rename_vault_account_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/resend_transaction_webhooks_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/resend_webhooks_by_transaction_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/resend_webhooks_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/respond_to_connection_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/reward_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/rewards_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/screening_configurations_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/screening_operation_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/screening_operation_execution_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/screening_operation_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/screening_operation_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/screening_policy_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/screening_provider_rules_configuration_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/screening_update_configurations_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/screening_validation_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/screening_verdict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/screening_verdict_matched_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/session_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/session_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/set_admin_quorum_threshold_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/set_admin_quorum_threshold_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/set_auto_fuel_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/set_confirmations_threshold_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/set_confirmations_threshold_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/set_customer_ref_id_for_address_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/set_customer_ref_id_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/set_network_id_discoverability_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/set_network_id_name_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/set_network_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/set_network_id_routing_policy_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/set_ota_status_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/set_ota_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/set_ota_status_response_one_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/set_routing_policy_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/set_routing_policy_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/settlement_request_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/settlement_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/signed_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/signed_message_signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/smart_transfer_bad_request_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/smart_transfer_create_ticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/smart_transfer_create_ticket_term.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/smart_transfer_forbidden_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/smart_transfer_fund_term.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/smart_transfer_manually_fund_term.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/smart_transfer_not_found_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/smart_transfer_set_ticket_expiration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/smart_transfer_set_ticket_external_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/smart_transfer_set_user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/smart_transfer_submit_ticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/smart_transfer_ticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/smart_transfer_ticket_filtered_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/smart_transfer_ticket_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/smart_transfer_ticket_term.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/smart_transfer_ticket_term_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/smart_transfer_update_ticket_term.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/smart_transfer_user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/smart_transfer_user_groups_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/solana_blockchain_data_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/source_transfer_peer_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/source_transfer_peer_path_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/spam_ownership_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/spam_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/src_or_dest_attributes_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/stake_request_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/stake_response_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/stellar_ripple_create_params_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/system_message_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/templates_paginated_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/third_party_routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/to_collateral_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/to_exchange_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/token_collection_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/token_link_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/token_link_dto_token_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/token_link_exists_http_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/token_link_request_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/token_ownership_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/token_ownership_spam_update_payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/token_ownership_status_update_payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/tokens_paginated_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/trading_account_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/transaction_fee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/transaction_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14627 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/transaction_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/transaction_request_amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/transaction_request_destination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/transaction_request_fee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/transaction_request_gas_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/transaction_request_gas_price.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/transaction_request_network_fee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/transaction_request_network_staking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/transaction_request_priority_fee.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22863 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/transaction_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/transaction_response_contract_call_decoded_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/transaction_response_destination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/transfer_config_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/transfer_operation_config_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/transfer_operation_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/transfer_operation_execution_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/transfer_operation_execution_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/transfer_operation_execution_params_execution_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/transfer_operation_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/transfer_operation_failure_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/transfer_operation_preview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/transfer_operation_preview_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/transfer_operation_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/transfer_peer_path_sub_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/transfer_peer_path_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/transfer_validation_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/travel_rule_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/travel_rule_create_transaction_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/travel_rule_get_all_vasps_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/travel_rule_issuer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/travel_rule_issuers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/travel_rule_ownership_proof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/travel_rule_pii_ivms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/travel_rule_policy_rule_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/travel_rule_transaction_blockchain_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/travel_rule_update_vasp_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/travel_rule_validate_full_transaction_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/travel_rule_validate_transaction_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/travel_rule_validate_transaction_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8209 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/travel_rule_vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/unfreeze_transaction_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/unmanaged_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/unspent_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/unspent_inputs_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/unstake_request_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/update_token_ownership_status_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/update_vault_account_asset_address_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/update_vault_account_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/user_group_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/user_group_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/user_group_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/user_group_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/user_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/user_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/user_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/user_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/validate_address_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/validator_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/vault_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/vault_accounts_paged_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/vault_accounts_paged_response_paging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/vault_action_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/vault_asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/vault_wallet_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/vendor_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/wallet_asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/wallet_asset_additional_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/withdraw_request_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/workflow_config_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/workflow_configuration_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7899 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/workflow_execution_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/write_abi_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/write_call_function_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/models/write_call_function_response_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9280 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/threaded_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/unknown_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/fireblocks/user_agent_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:02.927155 fireblocks-0.0.2b0/fireblocks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    70992 2024-05-30 14:05:02.000000 fireblocks-0.0.2b0/fireblocks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    40677 2024-05-30 14:05:02.000000 fireblocks-0.0.2b0/fireblocks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 14:05:02.000000 fireblocks-0.0.2b0/fireblocks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-30 14:05:02.000000 fireblocks-0.0.2b0/fireblocks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-30 14:05:02.000000 fireblocks-0.0.2b0/fireblocks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-30 14:05:02.927155 fireblocks-0.0.2b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:02.923155 fireblocks-0.0.2b0/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:05:02.927155 fireblocks-0.0.2b0/test/fireblocks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/fireblocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/fireblocks/test_additional_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/fireblocks/test_bearer_token_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8141 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/fireblocks/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/fireblocks/test_client_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/fireblocks/test_threaded_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/fireblocks/test_unknown_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/fireblocks/test_user_agent_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_abi_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_account_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_add_asset_to_external_wallet_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_add_asset_to_external_wallet_request_one_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_add_asset_to_external_wallet_request_one_of1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_add_asset_to_external_wallet_request_one_of1_additional_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_add_asset_to_external_wallet_request_one_of1_additional_info_one_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_add_asset_to_external_wallet_request_one_of1_additional_info_one_of1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_add_asset_to_external_wallet_request_one_of1_additional_info_one_of2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_add_collateral_request_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_add_contract_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_additional_info_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_aml_registration_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_aml_screening_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_amount_aggregation_time_period_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_amount_and_chain_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_amount_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_api_keys_paginated_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_api_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_api_user_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_asset_already_exist_http_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_asset_amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_asset_bad_request_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_asset_conflict_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_asset_does_not_exist_http_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_asset_forbidden_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_asset_internal_server_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_asset_metadata_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_asset_not_found_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_asset_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_asset_response_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_asset_response_onchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_asset_type_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_asset_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_assets_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_audit_log_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_audit_logs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_auditor_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_authorization_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_authorization_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_block_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_blockchains_assets_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_cancel_transaction_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_chain_info_response_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_collection_metadata_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_collection_ownership_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_compliance_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_compliance_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_compliance_screening_configuration_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_compliance_screening_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_config_change_request_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_config_conversion_operation_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_config_disbursement_operation_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_config_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_config_operation_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_config_operation_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_config_transfer_operation_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_console_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_console_user_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_contract_abi_response_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_contract_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_contract_deploy_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_contract_deploy_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_contract_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_contract_interactions_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_contract_metadata_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_contract_template_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_contract_templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_contract_upload_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_contracts_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_conversion_config_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_conversion_operation_config_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_conversion_operation_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_conversion_operation_execution_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_conversion_operation_execution_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_conversion_operation_execution_params_execution_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_conversion_operation_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_conversion_operation_preview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_conversion_operation_preview_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_conversion_operation_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_conversion_validation_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_convert_assets_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_convert_assets_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_cosigner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_cosigners_beta_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_cosigners_paginated_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_create_address_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_create_address_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_create_api_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_create_assets_bulk_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_create_assets_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_create_config_operation_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_create_connection_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_create_connection_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_create_console_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_create_contract_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_create_conversion_config_operation_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_create_disbursement_config_operation_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_create_internal_transfer_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_create_internal_wallet_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_create_multiple_accounts_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_create_ncw_connection_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_create_network_id_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_create_payout_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_create_token_request_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_create_token_request_dto_create_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_create_transaction_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_create_transfer_config_operation_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_create_user_group_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_create_vault_account_connection_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_create_vault_account_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_create_vault_asset_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_create_wallet_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_create_workflow_execution_request_params_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_custom_routing_dest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_default_network_routing_dest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_delegation_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_delegation_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_delete_network_connection_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_delete_network_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_deployed_contract_response_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_deployed_contracts_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_deployed_contracts_paginated_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_deposit_funds_from_linked_dda_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_destination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_destination_transfer_peer_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_destination_transfer_peer_path_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_disbursement_amount_instruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_disbursement_config_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_disbursement_instruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_disbursement_instruction_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_disbursement_operation_config_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_disbursement_operation_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_disbursement_operation_execution_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_disbursement_operation_execution_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_disbursement_operation_execution_params_execution_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_disbursement_operation_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_disbursement_operation_preview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_disbursement_operation_preview_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_disbursement_operation_preview_output_instruction_set_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_disbursement_operation_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_disbursement_percentage_instruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_disbursement_validation_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_dispatch_payout_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8738 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_draft_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11580 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_draft_review_and_validation_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_drop_transaction_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_drop_transaction_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_edit_gas_station_configuration_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_error_response_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_error_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_estimated_network_fee_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_estimated_transaction_fee_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_evm_token_create_params_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_exchange_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_exchange_accounts_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_exchange_accounts_paged.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_exchange_accounts_paged_paging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_exchange_asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_exchange_settlement_transactions_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_exchange_trading_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_exchange_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_execute_action_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_execute_action_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_execution_conversion_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_execution_disbursement_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_execution_operation_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_execution_screening_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_execution_transfer_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_external_wallet_asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_external_wallets_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_fee_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_fiat_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_fiat_account_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_fiat_accounts_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_fiat_asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_freeze_transaction_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_function_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_funds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_gas_station_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_gas_station_configuration_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_gas_station_properties_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_gas_stations_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_get_api_users_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_get_audit_logs_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_get_audit_logs_response_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_get_connections_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_get_console_users_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_get_filter_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_get_max_spendable_amount_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_get_nfts_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_get_ota_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_get_ownership_tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_get_transaction_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_get_whitelist_ip_addresses_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_get_workspace_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_http_contract_does_not_exist_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_instruction_amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_internal_transfer_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_internal_wallets_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_job_created.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_job_management_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_lean_abi_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_lean_contract_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_lean_deployed_contract_response_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_list_owned_collections_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_list_owned_tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_media_entity_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_network_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_network_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_network_connection_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_network_connection_routing_policy_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_network_connection_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_network_connections_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_network_fee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_network_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_network_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_network_id_routing_policy_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_network_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_nfts_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_none_network_routing_dest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_off_exchanges_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_one_time_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_one_time_address_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_operation_execution_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_ota_beta_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_paginated_address_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_paginated_address_response_paging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_paginated_asset_wallet_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_paginated_asset_wallet_response_paging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_paging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_parameter_with_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_payee_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_payee_account_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_payee_account_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_payment_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_payment_account_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_payment_account_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_payments_payout_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_payout_init_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_payout_instruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_payout_instruction_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_payout_instruction_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_payout_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_payout_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_payout_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_policy_and_validation_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_policy_check_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_policy_editor_beta_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_policy_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8630 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_policy_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_policy_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_policy_rule_amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_policy_rule_amount_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_policy_rule_authorization_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_policy_rule_authorization_groups_groups_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_policy_rule_check_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_policy_rule_designated_signers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_policy_rule_dst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_policy_rule_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_policy_rule_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_policy_rule_raw_message_signing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_policy_rule_raw_message_signing_derivation_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_policy_rule_src.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_policy_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_policy_src_or_dest_sub_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_policy_src_or_dest_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_policy_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_policy_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_pre_screening.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_provider_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_public_key_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_publish_draft_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10214 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_publish_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_read_abi_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_read_call_function_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_redeem_funds_to_linked_dda_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_register_new_asset_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_related_transaction_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_remove_collateral_request_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_rename_cosigner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_rename_vault_account_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_resend_transaction_webhooks_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_resend_webhooks_by_transaction_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_resend_webhooks_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_reset_device_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_respond_to_connection_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_reward_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_rewards_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_screening_configurations_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_screening_operation_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_screening_operation_execution_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_screening_operation_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_screening_operation_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_screening_policy_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_screening_provider_rules_configuration_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_screening_update_configurations_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_screening_validation_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_screening_verdict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_screening_verdict_matched_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_session_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_session_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_set_admin_quorum_threshold_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_set_admin_quorum_threshold_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_set_auto_fuel_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_set_confirmations_threshold_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_set_confirmations_threshold_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_set_customer_ref_id_for_address_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_set_customer_ref_id_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_set_network_id_discoverability_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_set_network_id_name_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_set_network_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_set_network_id_routing_policy_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_set_ota_status_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_set_ota_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_set_ota_status_response_one_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_set_routing_policy_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_set_routing_policy_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_settlement_request_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_settlement_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_signed_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_signed_message_signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_smart_transfer_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_smart_transfer_bad_request_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_smart_transfer_create_ticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_smart_transfer_create_ticket_term.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_smart_transfer_forbidden_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_smart_transfer_fund_term.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_smart_transfer_manually_fund_term.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_smart_transfer_not_found_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_smart_transfer_set_ticket_expiration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_smart_transfer_set_ticket_external_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_smart_transfer_set_user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_smart_transfer_submit_ticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_smart_transfer_ticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_smart_transfer_ticket_filtered_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_smart_transfer_ticket_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_smart_transfer_ticket_term.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_smart_transfer_ticket_term_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_smart_transfer_update_ticket_term.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_smart_transfer_user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_smart_transfer_user_groups_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_solana_blockchain_data_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_source_transfer_peer_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_source_transfer_peer_path_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_spam_ownership_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_spam_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_src_or_dest_attributes_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_stake_request_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_stake_response_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_staking_beta_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_stellar_ripple_create_params_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_system_message_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_templates_paginated_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_third_party_routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_to_collateral_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_to_exchange_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_token_collection_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_token_link_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_token_link_dto_token_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_token_link_exists_http_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_token_link_request_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_token_ownership_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_token_ownership_spam_update_payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_token_ownership_status_update_payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_tokenization_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_tokens_paginated_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_trading_account_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_transaction_fee.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_transaction_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_transaction_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_transaction_request_amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_transaction_request_destination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_transaction_request_fee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_transaction_request_gas_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_transaction_request_gas_price.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_transaction_request_network_fee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_transaction_request_network_staking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_transaction_request_priority_fee.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10274 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_transaction_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_transaction_response_contract_call_decoded_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_transaction_response_destination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_transactions_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_transfer_config_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_transfer_operation_config_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_transfer_operation_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_transfer_operation_execution_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_transfer_operation_execution_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_transfer_operation_execution_params_execution_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_transfer_operation_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_transfer_operation_failure_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_transfer_operation_preview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_transfer_operation_preview_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_transfer_operation_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_transfer_peer_path_sub_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_transfer_peer_path_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_transfer_validation_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_travel_rule_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_travel_rule_beta_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_travel_rule_create_transaction_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7703 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_travel_rule_get_all_vasps_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_travel_rule_issuer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_travel_rule_issuers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_travel_rule_ownership_proof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_travel_rule_pii_ivms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_travel_rule_policy_rule_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_travel_rule_transaction_blockchain_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_travel_rule_update_vasp_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_travel_rule_validate_full_transaction_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_travel_rule_validate_transaction_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_travel_rule_validate_transaction_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_travel_rule_vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_unfreeze_transaction_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_unmanaged_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_unspent_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_unspent_inputs_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_unstake_request_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_update_token_ownership_status_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_update_vault_account_asset_address_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_update_vault_account_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_user_group_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_user_group_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_user_group_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_user_group_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_user_groups_beta_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_user_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_user_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_user_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_users_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_validate_address_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_validator_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_vault_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_vault_accounts_paged_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_vault_accounts_paged_response_paging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_vault_action_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_vault_asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_vault_wallet_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_vaults_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_vendor_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_wallet_asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_wallet_asset_additional_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_web3_connections_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_webhooks_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_whitelist_ip_addresses_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_withdraw_request_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_workflow_config_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_workflow_configuration_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_workflow_execution_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_workspace_status_beta_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_write_abi_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_write_call_function_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-30 14:04:58.000000 fireblocks-0.0.2b0/test/test_write_call_function_response_dto.py
```

### Comparing `fireblocks-0.0.1/fireblocks_client/apis/tags/audit_logs_api.py` & `fireblocks-0.0.2b0/test/test_account_type.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,36 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-from fireblocks_client.paths.audits.get import GetAudits
+    Do not edit the class manually.
+"""  # noqa: E501
 
 
-class AuditLogsApi(
-    GetAudits,
-):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
+import unittest
 
-    Do not edit the class manually.
-    """
-    pass
+from fireblocks.models.account_type import AccountType
+
+
+class TestAccountType(unittest.TestCase):
+    """AccountType unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testAccountType(self):
+        """Test AccountType"""
+        # inst = AccountType()
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `fireblocks-0.0.1/fireblocks_client/apis/tags/blockchains_assets_api.py` & `fireblocks-0.0.2b0/fireblocks/models/payout_init_method.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,38 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-from fireblocks_client.paths.supported_assets.get import GetSupportedAssets
+    Do not edit the class manually.
+"""  # noqa: E501
 
 
-class BlockchainsAssetsApi(
-    GetSupportedAssets,
-):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
+from __future__ import annotations
+import json
+from enum import Enum
+from typing_extensions import Self
 
-    Do not edit the class manually.
+
+class PayoutInitMethod(str, Enum):
+    """
+    PayoutInitMethod
     """
-    pass
+
+    """
+    allowed enum values
+    """
+    FILE = 'FILE'
+    API = 'API'
+
+    @classmethod
+    def from_json(cls, json_str: str) -> Self:
+        """Create an instance of PayoutInitMethod from a JSON string"""
+        return cls(json.loads(json_str))
+
+
```

### Comparing `fireblocks-0.0.1/fireblocks_client/apis/tags/external_wallets_api.py` & `fireblocks-0.0.2b0/test/test_external_wallets_api.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,88 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from fireblocks_client.paths.external_wallets_wallet_id_asset_id.post import AddAssetToExternalWallet
-from fireblocks_client.paths.external_wallets.post import CreateExternalWallet
-from fireblocks_client.paths.external_wallets_wallet_id.delete import DeleteExternalWallet
-from fireblocks_client.paths.external_wallets_wallet_id_asset_id.get import GetAssetInExternalWallet
-from fireblocks_client.paths.external_wallets_wallet_id.get import GetExternalWalletById
-from fireblocks_client.paths.external_wallets.get import GetExternalWallets
-from fireblocks_client.paths.external_wallets_wallet_id_asset_id.delete import RemoveAssetFromExternalWallet
-from fireblocks_client.paths.external_wallets_wallet_id_set_customer_ref_id.post import SetCustomerRefIdForExternalWallet
-
-
-class ExternalWalletsApi(
-    AddAssetToExternalWallet,
-    CreateExternalWallet,
-    DeleteExternalWallet,
-    GetAssetInExternalWallet,
-    GetExternalWalletById,
-    GetExternalWallets,
-    RemoveAssetFromExternalWallet,
-    SetCustomerRefIdForExternalWallet,
-):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-    """
-    pass
+"""  # noqa: E501
+
+
+import unittest
+
+from fireblocks.api.external_wallets_api import ExternalWalletsApi
+
+
+class TestExternalWalletsApi(unittest.TestCase):
+    """ExternalWalletsApi unit test stubs"""
+
+    def setUp(self) -> None:
+        self.api = ExternalWalletsApi()
+
+    def tearDown(self) -> None:
+        pass
+
+    def test_add_asset_to_external_wallet(self) -> None:
+        """Test case for add_asset_to_external_wallet
+
+        Add an asset to an external wallet.
+        """
+        pass
+
+    def test_create_external_wallet(self) -> None:
+        """Test case for create_external_wallet
+
+        Create an external wallet
+        """
+        pass
+
+    def test_delete_external_wallet(self) -> None:
+        """Test case for delete_external_wallet
+
+        Delete an external wallet
+        """
+        pass
+
+    def test_get_external_wallet(self) -> None:
+        """Test case for get_external_wallet
+
+        Find an external wallet
+        """
+        pass
+
+    def test_get_external_wallet_asset(self) -> None:
+        """Test case for get_external_wallet_asset
+
+        Get an asset from an external wallet
+        """
+        pass
+
+    def test_get_external_wallets(self) -> None:
+        """Test case for get_external_wallets
+
+        List external wallets
+        """
+        pass
+
+    def test_remove_asset_from_external_wallet(self) -> None:
+        """Test case for remove_asset_from_external_wallet
+
+        Delete an asset from an external wallet
+        """
+        pass
+
+    def test_set_external_wallet_customer_ref_id(self) -> None:
+        """Test case for set_external_wallet_customer_ref_id
+
+        Set an AML customer reference ID for an external wallet
+        """
+        pass
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `fireblocks-0.0.1/fireblocks_client/apis/tags/off_exchanges_api.py` & `fireblocks-0.0.2b0/test/test_off_exchanges_api.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,67 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from fireblocks_client.paths.off_exchange_add.post import AddOffExchange
-from fireblocks_client.paths.off_exchange_collateral_accounts_main_exchange_account_id.get import GetOffExchangeCollateralAccounts
-from fireblocks_client.paths.off_exchange_settlements_transactions.get import GetOffExchangeSettlementTransactions
-from fireblocks_client.paths.off_exchange_remove.post import RemoveOffExchange
-from fireblocks_client.paths.off_exchange_settlements_trader.post import SettleOffExchangeTrades
-
-
-class OffExchangesApi(
-    AddOffExchange,
-    GetOffExchangeCollateralAccounts,
-    GetOffExchangeSettlementTransactions,
-    RemoveOffExchange,
-    SettleOffExchangeTrades,
-):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-    """
-    pass
+"""  # noqa: E501
+
+
+import unittest
+
+from fireblocks.api.off_exchanges_api import OffExchangesApi
+
+
+class TestOffExchangesApi(unittest.TestCase):
+    """OffExchangesApi unit test stubs"""
+
+    def setUp(self) -> None:
+        self.api = OffExchangesApi()
+
+    def tearDown(self) -> None:
+        pass
+
+    def test_add_off_exchange(self) -> None:
+        """Test case for add_off_exchange
+
+        add collateral
+        """
+        pass
+
+    def test_get_off_exchange_collateral_accounts(self) -> None:
+        """Test case for get_off_exchange_collateral_accounts
+
+        Find a specific collateral exchange account
+        """
+        pass
+
+    def test_get_off_exchange_settlement_transactions(self) -> None:
+        """Test case for get_off_exchange_settlement_transactions
+
+        get settlements transactions from exchange
+        """
+        pass
+
+    def test_remove_off_exchange(self) -> None:
+        """Test case for remove_off_exchange
+
+        remove collateral
+        """
+        pass
+
+    def test_settle_off_exchange_trades(self) -> None:
+        """Test case for settle_off_exchange_trades
+
+        create settlement for a trader
+        """
+        pass
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `fireblocks-0.0.1/fireblocks_client/apis/tags/ota_beta_api.py` & `fireblocks-0.0.2b0/test/test_network_connection_status.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-from fireblocks_client.paths.management_ota.get import GetOtaStatus
-from fireblocks_client.paths.management_ota.post import SetOtaStatus
+    Do not edit the class manually.
+"""  # noqa: E501
 
 
-class OTABetaApi(
-    GetOtaStatus,
-    SetOtaStatus,
-):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
+import unittest
 
-    Do not edit the class manually.
-    """
-    pass
+from fireblocks.models.network_connection_status import NetworkConnectionStatus
+
+
+class TestNetworkConnectionStatus(unittest.TestCase):
+    """NetworkConnectionStatus unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testNetworkConnectionStatus(self):
+        """Test NetworkConnectionStatus"""
+        # inst = NetworkConnectionStatus()
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `fireblocks-0.0.1/fireblocks_client/apis/tags/payments_payout_api.py` & `fireblocks-0.0.2b0/test/test_payout_instruction_state.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-from fireblocks_client.paths.payments_payout.post import CreatePayout
-from fireblocks_client.paths.payments_payout_payout_id_actions_execute.post import ExecutePayoutAction
-from fireblocks_client.paths.payments_payout_payout_id.get import GetPayoutById
+    Do not edit the class manually.
+"""  # noqa: E501
 
 
-class PaymentsPayoutApi(
-    CreatePayout,
-    ExecutePayoutAction,
-    GetPayoutById,
-):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
+import unittest
 
-    Do not edit the class manually.
-    """
-    pass
+from fireblocks.models.payout_instruction_state import PayoutInstructionState
+
+
+class TestPayoutInstructionState(unittest.TestCase):
+    """PayoutInstructionState unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testPayoutInstructionState(self):
+        """Test PayoutInstructionState"""
+        # inst = PayoutInstructionState()
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `fireblocks-0.0.1/fireblocks_client/apis/tags/users_api.py` & `fireblocks-0.0.2b0/test/test_user_role.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,36 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-from fireblocks_client.paths.users.get import GetUsers
+    Do not edit the class manually.
+"""  # noqa: E501
 
 
-class UsersApi(
-    GetUsers,
-):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
+import unittest
 
-    Do not edit the class manually.
-    """
-    pass
+from fireblocks.models.user_role import UserRole
+
+
+class TestUserRole(unittest.TestCase):
+    """UserRole unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testUserRole(self):
+        """Test UserRole"""
+        # inst = UserRole()
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `fireblocks-0.0.1/fireblocks_client/apis/tags/web3_connections_api.py` & `fireblocks-0.0.2b0/test/test_policy_src_or_dest_sub_type.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-from fireblocks_client.paths.connections_wc.post import Create
-from fireblocks_client.paths.connections.get import Get
-from fireblocks_client.paths.connections_wc_id.delete import Remove
-from fireblocks_client.paths.connections_wc_id.put import Submit
+    Do not edit the class manually.
+"""  # noqa: E501
 
 
-class Web3ConnectionsApi(
-    Create,
-    Get,
-    Remove,
-    Submit,
-):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
+import unittest
 
-    Do not edit the class manually.
-    """
-    pass
+from fireblocks.models.policy_src_or_dest_sub_type import PolicySrcOrDestSubType
+
+
+class TestPolicySrcOrDestSubType(unittest.TestCase):
+    """PolicySrcOrDestSubType unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testPolicySrcOrDestSubType(self):
+        """Test PolicySrcOrDestSubType"""
+        # inst = PolicySrcOrDestSubType()
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `fireblocks-0.0.1/fireblocks_client/apis/tags/webhooks_api.py` & `fireblocks-0.0.2b0/test/test_user_type.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-from fireblocks_client.paths.webhooks_resend.post import ResendWebhooks
-from fireblocks_client.paths.webhooks_resend_tx_id.post import ResendWebhooksForTransaction
+    Do not edit the class manually.
+"""  # noqa: E501
 
 
-class WebhooksApi(
-    ResendWebhooks,
-    ResendWebhooksForTransaction,
-):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
+import unittest
 
-    Do not edit the class manually.
-    """
-    pass
+from fireblocks.models.user_type import UserType
+
+
+class TestUserType(unittest.TestCase):
+    """UserType unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testUserType(self):
+        """Test UserType"""
+        # inst = UserType()
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `fireblocks-0.0.1/fireblocks_client/configuration.py` & `fireblocks-0.0.2b0/fireblocks/configuration.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,257 +1,226 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import copy
 import logging
-import math
+from logging import FileHandler
 import multiprocessing
-import secrets
 import sys
-import time
-from typing import Optional, Dict, Any
-import jwt
-import json
-import mimetypes
-from hashlib import sha256
+from typing import Optional
 import urllib3
-import os
-from http import client as http_client
-from fireblocks_client.exceptions import ApiValueError
 
+import http.client as httplib
 
 JSON_SCHEMA_VALIDATION_KEYWORDS = {
     "multipleOf",
     "maximum",
     "exclusiveMaximum",
     "minimum",
     "exclusiveMinimum",
     "maxLength",
     "minLength",
     "pattern",
     "maxItems",
     "minItems",
-    "uniqueItems",
-    "maxProperties",
-    "minProperties",
 }
 
 
-class SDKOptions:
-    def __init__(
-        self,
-        timeout_in_ms: Optional[int] = None,
-        proxy: Optional[Dict[str, Any]] = None,
-        anonymous_platform: Optional[bool] = None,
-        user_agent: Optional[str] = None,
-    ):
-        self.timeout_in_ms = timeout_in_ms
-        self.proxy = proxy
-        self.anonymous_platform = anonymous_platform
-        self.user_agent = user_agent
-        self.retries = None
-        self.connection_pool_maxsize = 3
-
-    @staticmethod
-    def get_default():
-        options = SDKOptions()
-        options.timeout_in_ms = 10000
-        options.proxy = None
-        options.anonymous_platform = None
-        options.user_agent = None
-        options.retries = None
-        options.connection_pool_maxsize = 3
-        return options
-
-
-class Configuration(object):
-    """NOTE: This class is auto generated by OpenAPI Generator
-
-        Ref: https://openapi-generator.tech
-        Do not edit the class manually.
+class Configuration:
+    """This class contains various settings of the API client.
 
-        :param host: Base url
+        :param host: Base url.
         :param api_key: Dict to store API key(s).
           Each entry in the dict specifies an API key.
           The dict key is the name of the security scheme in the OAS specification.
           The dict value is the API key secret.
-        :param api_key_prefix: Dict to store API prefix (e.g. Bearer)
+        :param api_key_prefix: Dict to store API prefix (e.g. Bearer).
           The dict key is the name of the security scheme in the OAS specification.
           The dict value is an API key prefix when generating the auth data.
-        :param username: Username for HTTP basic authentication
-        :param password: Password for HTTP basic authentication
-        :param discard_unknown_keys: Boolean value indicating whether to discard
-          unknown properties. A server may send a response that includes additional
-          properties that are not known by the client in the following scenarios:
-          1. The OpenAPI document is incomplete, i.e. it does not match the server
-             implementation.
-          2. The client was generated using an older version of the OpenAPI document
-             and the server has been upgraded since then.
-          If a schema in the OpenAPI document defines the additionalProperties attribute,
-          then all undeclared properties received by the server are injected into the
-          additional properties map. In that case, there are undeclared properties, and
-          nothing to discard.
-        :param disabled_client_side_validations (string): Comma-separated list of
-          JSON schema validation keywords to disable JSON schema structural validation
-          rules. The following keywords may be specified: multipleOf, maximum,
-          exclusiveMaximum, minimum, exclusiveMinimum, maxLength, minLength, pattern,
-          maxItems, minItems.
-          By default, the validation is performed for data generated locally by the client
-          and data received from the server, independent of any validation performed by
-          the server side. If the input data does not satisfy the JSON schema validation
-          rules specified in the OpenAPI document, an exception is raised.
-          If disabled_client_side_validations is set, structural validation is
-          disabled. This can be useful to troubleshoot data validation problem, such as
-          when the OpenAPI document validation rules do not match the actual API data
-          received by the server.
+        :param username: Username for HTTP basic authentication.
+        :param password: Password for HTTP basic authentication.
+        :param access_token: Access token.
         :param server_index: Index to servers configuration.
         :param server_variables: Mapping with string values to replace variables in
           templated server configuration. The validation of enums is performed for
           variables with defined enum values before.
         :param server_operation_index: Mapping from operation ID to an index to server
           configuration.
         :param server_operation_variables: Mapping from operation ID to a mapping with
           string values to replace variables in templated server configuration.
-          The validation of enums is performed for variables with defined enum values before.
+          The validation of enums is performed for variables with defined enum
+          values before.
+        :param ssl_ca_cert: str - the path to a file of concatenated CA certificates
+          in PEM format.
 
         :Example:
 
         API Key Authentication Example.
         Given the following security scheme in the OpenAPI specification:
           components:
             securitySchemes:
               cookieAuth:         # name for the security scheme
                 type: apiKey
                 in: cookie
                 name: JSESSIONID  # cookie name
 
         You can programmatically set the cookie:
 
-    conf = fireblocks_client.Configuration(
+    conf = fireblocks.Configuration(
         api_key={'cookieAuth': 'abc123'}
         api_key_prefix={'cookieAuth': 'JSESSIONID'}
     )
 
         The following cookie will be added to the HTTP request:
            Cookie: JSESSIONID abc123
     """
 
     _default = None
 
     def __init__(
         self,
-        base_path: str = None,
-        api_key: str = None,
-        secret_key: str = None,
-        connection_pool_maxsize: int = None,
-        options: SDKOptions = None,
-    ):
+        host=None,
+        api_key=None,
+        api_key_prefix=None,
+        username=None,
+        password=None,
+        access_token=None,
+        server_index=None,
+        server_variables=None,
+        server_operation_index=None,
+        server_operation_variables=None,
+        ssl_ca_cert=None,
+    ) -> None:
         """Constructor"""
-        self._base_path = base_path or "https://api.fireblocks.io/v1"
-        if base_path is not None:
-            self._base_path = base_path
-        elif os.environ.get("FIREBLOCKS_BASE_PATH", None) is not None:
-            self._base_path = os.environ["FIREBLOCKS_BASE_PATH"]
-
-        self._api_key = api_key
-        if (
-            os.environ.get("FIREBLOCKS_API_KEY", None) is not None
-            and self._api_key is None
-        ):
-            self._api_key = os.environ["FIREBLOCKS_API_KEY"]
-        if self._api_key is None:
-            raise ValueError("api_key is missing please provide it and try again")
-
-        self._secret_key = secret_key
-        if (
-            os.environ.get("FIREBLOCKS_SECRET_KEY", None) is not None
-            and self._secret_key is None
-        ):
-            self._secret_key = os.environ["FIREBLOCKS_SECRET_KEY"]
-        if self._secret_key is None:
-            raise ValueError("secret_key is missing please provide it and try again")
-
-        self._sdk_options = options
-        if self._sdk_options is None:
-            self._sdk_options = SDKOptions.get_default()
+        self._base_path = "https://api.fireblocks.io/v1" if host is None else host
+        """Default Base url
+        """
+        self.server_index = 0 if server_index is None and host is None else server_index
+        self.server_operation_index = server_operation_index or {}
+        """Default server index
+        """
+        self.server_variables = server_variables or {}
+        self.server_operation_variables = server_operation_variables or {}
+        """Default server variables
+        """
+        self.temp_folder_path = None
+        """Temp file folder for downloading files
+        """
+        # Authentication Settings
+        self.api_key = {}
+        if api_key:
+            self.api_key = api_key
+        """dict to store API key(s)
+        """
+        self.api_key_prefix = {}
+        if api_key_prefix:
+            self.api_key_prefix = api_key_prefix
+        """dict to store API prefix (e.g. Bearer)
+        """
+        self.refresh_api_key_hook = None
+        """function hook to refresh API key if expired
+        """
+        self.username = username
+        """Username for HTTP basic authentication
+        """
+        self.password = password
+        """Password for HTTP basic authentication
+        """
+        self.access_token = access_token
+        """Access token
+        """
         self.logger = {}
         """Logging Settings
         """
-        self.logger["package_logger"] = logging.getLogger("fireblocks_client")
+        self.logger["package_logger"] = logging.getLogger("fireblocks")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = "%(asctime)s %(levelname)s %(message)s"
         """Log format
         """
         self.logger_stream_handler = None
         """Log stream handler
         """
-        self.logger_file_handler = None
+        self.logger_file_handler: Optional[FileHandler] = None
         """Log file handler
         """
         self.logger_file = None
         """Debug file location
         """
         self.debug = False
         """Debug switch
         """
 
+        self.verify_ssl = True
+        """SSL/TLS verification
+           Set this to false to skip verifying SSL certificate when calling API
+           from https server.
+        """
+        self.ssl_ca_cert = ssl_ca_cert
+        """Set this to customize the certificate file to verify the peer.
+        """
+        self.cert_file = None
+        """client certificate file
+        """
+        self.key_file = None
+        """client key file
+        """
+        self.assert_hostname = None
+        """Set this to True/False to enable/disable SSL hostname verification.
+        """
+        self.tls_server_name = None
+        """SSL/TLS Server Name Indication (SNI)
+           Set this to the SNI value expected by the server.
+        """
+
         self.connection_pool_maxsize = multiprocessing.cpu_count() * 5
         """urllib3 connection pool's maximum number of connections saved
            per pool. urllib3 uses 1 connection as default value, but this is
            not the best value when you are making a lot of possibly parallel
            requests to the same host, which is often the case here.
            cpu_count * 5 is used as default value to increase performance.
         """
 
-        self.proxy = None
+        self.proxy: Optional[str] = None
         """Proxy URL
         """
         self.proxy_headers = None
         """Proxy headers
         """
         self.safe_chars_for_path_param = ""
         """Safe chars for path_param
         """
         self.retries = None
         """Adding retries to override urllib3 default value 3
         """
         # Enable client side validation
         self.client_side_validation = True
 
-        # Options to pass down to the underlying urllib3 socket
         self.socket_options = None
+        """Options to pass down to the underlying urllib3 socket
+        """
 
-    @property
-    def options(self):
-        return self._sdk_options
-
-    @property
-    def base_path(self):
-        return self._base_path
-
-    @property
-    def api_key(self):
-        return self._api_key
-
-    @property
-    def secret_key(self):
-        return self._secret_key
+        self.datetime_format = "%Y-%m-%dT%H:%M:%S.%f%z"
+        """datetime format
+        """
 
-    @options.setter
-    def options(self, options):
-        self.options = options
+        self.date_format = "%Y-%m-%d"
+        """date format
+        """
 
     def __deepcopy__(self, memo):
         cls = self.__class__
         result = cls.__new__(cls)
         memo[id(self)] = result
         for k, v in self.__dict__.items():
             if k not in ("logger", "logger_file_handler"):
@@ -261,45 +230,49 @@
         # use setters to configure loggers
         result.logger_file = self.logger_file
         result.debug = self.debug
         return result
 
     def __setattr__(self, name, value):
         object.__setattr__(self, name, value)
-        if name == "disabled_client_side_validations":
-            s = set(filter(None, value.split(",")))
-            for v in s:
-                if v not in JSON_SCHEMA_VALIDATION_KEYWORDS:
-                    raise ApiValueError("Invalid keyword: '{0}''".format(v))
-            self._disabled_client_side_validations = s
 
     @classmethod
     def set_default(cls, default):
         """Set default instance of configuration.
 
         It stores default configuration, which can be
         returned by get_default_copy method.
 
         :param default: object of Configuration
         """
-        cls._default = copy.deepcopy(default)
+        cls._default = default
 
     @classmethod
     def get_default_copy(cls):
-        """Return new instance of configuration.
+        """Deprecated. Please use `get_default` instead.
+
+        Deprecated. Please use `get_default` instead.
+
+        :return: The configuration object.
+        """
+        return cls.get_default()
+
+    @classmethod
+    def get_default(cls):
+        """Return the default configuration.
 
         This method returns newly created, based on default constructor,
         object of Configuration class or returns a copy of default
-        configuration passed by the set_default method.
+        configuration.
 
         :return: The configuration object.
         """
-        if cls._default is not None:
-            return copy.deepcopy(cls._default)
-        return Configuration()
+        if cls._default is None:
+            cls._default = Configuration()
+        return cls._default
 
     @property
     def logger_file(self):
         """The logger file.
 
         If the logger_file is None, then add stream handler and remove file
         handler. Otherwise, add file handler and remove stream handler.
@@ -345,23 +318,23 @@
         :type: bool
         """
         self.__debug = value
         if self.__debug:
             # if debug status is True, turn on debug logging
             for _, logger in self.logger.items():
                 logger.setLevel(logging.DEBUG)
-            # turn on http_client debug
-            http_client.HTTPConnection.debuglevel = 1
+            # turn on httplib debug
+            httplib.HTTPConnection.debuglevel = 1
         else:
             # if debug status is False, turn off debug logging,
             # setting log level to default `logging.WARNING`
             for _, logger in self.logger.items():
                 logger.setLevel(logging.WARNING)
-            # turn off http_client debug
-            http_client.HTTPConnection.debuglevel = 0
+            # turn off httplib debug
+            httplib.HTTPConnection.debuglevel = 0
 
     @property
     def logger_format(self):
         """The logger format.
 
         The logger_formatter will be updated when sets logger_format.
 
@@ -378,25 +351,86 @@
 
         :param value: The format string.
         :type: str
         """
         self.__logger_format = value
         self.logger_formatter = logging.Formatter(self.__logger_format)
 
+    def get_api_key_with_prefix(self, identifier, alias=None):
+        """Gets API key (with prefix if set).
+
+        :param identifier: The identifier of apiKey.
+        :param alias: The alternative identifier of apiKey.
+        :return: The token for api key authentication.
+        """
+        if self.refresh_api_key_hook is not None:
+            self.refresh_api_key_hook(self)
+        key = self.api_key.get(
+            identifier, self.api_key.get(alias) if alias is not None else None
+        )
+        if key:
+            prefix = self.api_key_prefix.get(identifier)
+            if prefix:
+                return "%s %s" % (prefix, key)
+            else:
+                return key
+
+    def get_basic_auth_token(self):
+        """Gets HTTP basic authentication header (string).
+
+        :return: The token for basic HTTP authentication.
+        """
+        username = ""
+        if self.username is not None:
+            username = self.username
+        password = ""
+        if self.password is not None:
+            password = self.password
+        return urllib3.util.make_headers(basic_auth=username + ":" + password).get(
+            "authorization"
+        )
+
+    def auth_settings(self):
+        """Gets Auth Settings dict for api client.
+
+        :return: The Auth Settings information dict.
+        """
+        auth = {}
+        if self.access_token is not None:
+            auth["bearerTokenAuth"] = {
+                "type": "bearer",
+                "in": "header",
+                "format": "JWT",
+                "key": "Authorization",
+                "value": "Bearer " + self.access_token,
+            }
+        if "ApiKeyAuth" in self.api_key:
+            auth["ApiKeyAuth"] = {
+                "type": "api_key",
+                "in": "header",
+                "key": "X-API-Key",
+                "value": self.get_api_key_with_prefix(
+                    "ApiKeyAuth",
+                ),
+            }
+        return auth
+
     def to_debug_report(self):
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return (
             "Python SDK Debug Report:\n"
             "OS: {env}\n"
             "Python Version: {pyversion}\n"
             "Version of the API: 1.6.2\n"
-            "SDK Package Version: 1.0.0".format(env=sys.platform, pyversion=sys.version)
+            "SDK Package Version: 0.0.2-beta".format(
+                env=sys.platform, pyversion=sys.version
+            )
         )
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `fireblocks-0.0.1/fireblocks_client/exceptions.py` & `fireblocks-0.0.2b0/fireblocks/exceptions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
-import dataclasses
-import typing
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
 
-from urllib3._collections import HTTPHeaderDict
+from typing import Any, Optional
+from typing_extensions import Self
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
 
 
 class ApiTypeError(OpenApiException, TypeError):
-    def __init__(self, msg, path_to_item=None, valid_classes=None, key_type=None):
+    def __init__(
+        self, msg, path_to_item=None, valid_classes=None, key_type=None
+    ) -> None:
         """Raises an exception for TypeErrors
 
         Args:
             msg (str): the exception message
 
         Keyword Args:
             path_to_item (list): a list of keys an indices to get to the
@@ -44,15 +47,15 @@
         full_msg = msg
         if path_to_item:
             full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
         super(ApiTypeError, self).__init__(full_msg)
 
 
 class ApiValueError(OpenApiException, ValueError):
-    def __init__(self, msg, path_to_item=None):
+    def __init__(self, msg, path_to_item=None) -> None:
         """
         Args:
             msg (str): the exception message
 
         Keyword Args:
             path_to_item (list) the path to the exception in the
                 received_data dict. None if unset
@@ -62,15 +65,15 @@
         full_msg = msg
         if path_to_item:
             full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
         super(ApiValueError, self).__init__(full_msg)
 
 
 class ApiAttributeError(OpenApiException, AttributeError):
-    def __init__(self, msg, path_to_item=None):
+    def __init__(self, msg, path_to_item=None) -> None:
         """
         Raised when an attribute reference or assignment fails.
 
         Args:
             msg (str): the exception message
 
         Keyword Args:
@@ -81,15 +84,15 @@
         full_msg = msg
         if path_to_item:
             full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
         super(ApiAttributeError, self).__init__(full_msg)
 
 
 class ApiKeyError(OpenApiException, KeyError):
-    def __init__(self, msg, path_to_item=None):
+    def __init__(self, msg, path_to_item=None) -> None:
         """
         Args:
             msg (str): the exception message
 
         Keyword Args:
             path_to_item (None/list) the path to the exception in the
                 received_data dict
@@ -97,47 +100,99 @@
         self.path_to_item = path_to_item
         full_msg = msg
         if path_to_item:
             full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
         super(ApiKeyError, self).__init__(full_msg)
 
 
-T = typing.TypeVar("T")
+class ApiException(OpenApiException):
 
-
-@dataclasses.dataclass
-class ApiException(OpenApiException, typing.Generic[T]):
-    status: int
-    reason: str
-    api_response: typing.Optional[T] = None
-
-    @property
-    def body(self) -> typing.Union[str, bytes, None]:
-        if not self.api_response:
-            return None
-        return self.api_response.response.data
-
-    @property
-    def headers(self) -> typing.Optional[HTTPHeaderDict]:
-        if not self.api_response:
-            return None
-        return self.api_response.response.getheaders()
+    def __init__(
+        self,
+        status=None,
+        reason=None,
+        http_resp=None,
+        *,
+        body: Optional[str] = None,
+        data: Optional[Any] = None,
+    ) -> None:
+        self.status = status
+        self.reason = reason
+        self.body = body
+        self.data = data
+        self.headers = None
+
+        if http_resp:
+            if self.status is None:
+                self.status = http_resp.status
+            if self.reason is None:
+                self.reason = http_resp.reason
+            if self.body is None:
+                try:
+                    self.body = http_resp.data.decode("utf-8")
+                except Exception:
+                    pass
+            self.headers = http_resp.getheaders()
+
+    @classmethod
+    def from_response(
+        cls,
+        *,
+        http_resp,
+        body: Optional[str],
+        data: Optional[Any],
+    ) -> Self:
+        if http_resp.status == 400:
+            raise BadRequestException(http_resp=http_resp, body=body, data=data)
+
+        if http_resp.status == 401:
+            raise UnauthorizedException(http_resp=http_resp, body=body, data=data)
+
+        if http_resp.status == 403:
+            raise ForbiddenException(http_resp=http_resp, body=body, data=data)
+
+        if http_resp.status == 404:
+            raise NotFoundException(http_resp=http_resp, body=body, data=data)
+
+        if 500 <= http_resp.status <= 599:
+            raise ServiceException(http_resp=http_resp, body=body, data=data)
+        raise ApiException(http_resp=http_resp, body=body, data=data)
 
     def __str__(self):
         """Custom error messages for exception"""
         error_message = "({0})\n" "Reason: {1}\n".format(self.status, self.reason)
         if self.headers:
             error_message += "HTTP response headers: {0}\n".format(self.headers)
 
-        if self.body:
-            error_message += "HTTP response body: {0}\n".format(self.body)
+        if self.data or self.body:
+            error_message += "HTTP response body: {0}\n".format(self.data or self.body)
 
         return error_message
 
 
+class BadRequestException(ApiException):
+    pass
+
+
+class NotFoundException(ApiException):
+    pass
+
+
+class UnauthorizedException(ApiException):
+    pass
+
+
+class ForbiddenException(ApiException):
+    pass
+
+
+class ServiceException(ApiException):
+    pass
+
+
 def render_path(path_to_item):
     """Returns a string representation of a path"""
     result = ""
     for pth in path_to_item:
         if isinstance(pth, int):
             result += "[{0}]".format(pth)
         else:
```

### Comparing `fireblocks-0.0.1/fireblocks_client/model/create_payout_request.py` & `fireblocks-0.0.2b0/fireblocks/models/payout_instruction_response.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,127 +1,113 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import frozendict  # noqa: F401
+    Do not edit the class manually.
+"""  # noqa: E501
 
-from fireblocks_client import schemas  # noqa: F401
 
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
-class CreatePayoutRequest(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
+from fireblocks.models.instruction_amount import InstructionAmount
+from fireblocks.models.payee_account_response import PayeeAccountResponse
+from fireblocks.models.payout_instruction_state import PayoutInstructionState
+from fireblocks.models.transaction import Transaction
+from typing import Optional, Set
+from typing_extensions import Self
 
-    Do not edit the class manually.
+class PayoutInstructionResponse(BaseModel):
     """
-
-
-    class MetaOapg:
-        required = {
-            "instructionSet",
-            "paymentAccount",
-        }
-        
-        class properties:
-        
-            @staticmethod
-            def paymentAccount() -> typing.Type['PaymentAccount']:
-                return PaymentAccount
-            
-            
-            class instructionSet(
-                schemas.ListSchema
-            ):
-            
-            
-                class MetaOapg:
-                    
-                    @staticmethod
-                    def items() -> typing.Type['PayoutInstruction']:
-                        return PayoutInstruction
-            
-                def __new__(
-                    cls,
-                    _arg: typing.Union[typing.Tuple['PayoutInstruction'], typing.List['PayoutInstruction']],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'instructionSet':
-                    return super().__new__(
-                        cls,
-                        _arg,
-                        _configuration=_configuration,
-                    )
-            
-                def __getitem__(self, i: int) -> 'PayoutInstruction':
-                    return super().__getitem__(i)
-            __annotations__ = {
-                "paymentAccount": paymentAccount,
-                "instructionSet": instructionSet,
-            }
-    
-    instructionSet: MetaOapg.properties.instructionSet
-    paymentAccount: 'PaymentAccount'
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["paymentAccount"]) -> 'PaymentAccount': ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["instructionSet"]) -> MetaOapg.properties.instructionSet: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["paymentAccount", "instructionSet", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["paymentAccount"]) -> 'PaymentAccount': ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["instructionSet"]) -> MetaOapg.properties.instructionSet: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["paymentAccount", "instructionSet", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        instructionSet: typing.Union[MetaOapg.properties.instructionSet, list, tuple, ],
-        paymentAccount: 'PaymentAccount',
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'CreatePayoutRequest':
-        return super().__new__(
-            cls,
-            *_args,
-            instructionSet=instructionSet,
-            paymentAccount=paymentAccount,
-            _configuration=_configuration,
-            **kwargs,
+    PayoutInstructionResponse
+    """ # noqa: E501
+    id: Optional[StrictStr] = None
+    payee_account: PayeeAccountResponse = Field(alias="payeeAccount")
+    amount: InstructionAmount
+    state: PayoutInstructionState
+    transactions: List[Transaction]
+    __properties: ClassVar[List[str]] = ["id", "payeeAccount", "amount", "state", "transactions"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
+
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.model_dump(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of PayoutInstructionResponse from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        excluded_fields: Set[str] = set([
+        ])
+
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude=excluded_fields,
+            exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of payee_account
+        if self.payee_account:
+            _dict['payeeAccount'] = self.payee_account.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of amount
+        if self.amount:
+            _dict['amount'] = self.amount.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in transactions (list)
+        _items = []
+        if self.transactions:
+            for _item in self.transactions:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['transactions'] = _items
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of PayoutInstructionResponse from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return cls.model_validate(obj)
+
+        _obj = cls.model_validate({
+            "id": obj.get("id"),
+            "payeeAccount": PayeeAccountResponse.from_dict(obj["payeeAccount"]) if obj.get("payeeAccount") is not None else None,
+            "amount": InstructionAmount.from_dict(obj["amount"]) if obj.get("amount") is not None else None,
+            "state": obj.get("state"),
+            "transactions": [Transaction.from_dict(_item) for _item in obj["transactions"]] if obj.get("transactions") is not None else None
+        })
+        return _obj
+
 
-from fireblocks_client.model.payment_account import PaymentAccount
-from fireblocks_client.model.payout_instruction import PayoutInstruction
```

### Comparing `fireblocks-0.0.1/fireblocks_client/model/draft_review_and_validation_response.py` & `fireblocks-0.0.2b0/fireblocks/models/draft_review_and_validation_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,107 +1,98 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import frozendict  # noqa: F401
-
-from fireblocks_client import schemas  # noqa: F401
+    Do not edit the class manually.
+"""  # noqa: E501
 
 
-class DraftReviewAndValidationResponse(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
-    Do not edit the class manually.
+from pydantic import BaseModel, ConfigDict, Field
+from typing import Any, ClassVar, Dict, List
+from fireblocks.models.draft_response import DraftResponse
+from fireblocks.models.policy_validation import PolicyValidation
+from typing import Optional, Set
+from typing_extensions import Self
 
-    Draft validation
+class DraftReviewAndValidationResponse(BaseModel):
     """
-
-
-    class MetaOapg:
-        required = {
-            "draftResponse",
-            "validation",
-        }
-        
-        class properties:
-        
-            @staticmethod
-            def draftResponse() -> typing.Type['DraftResponse']:
-                return DraftResponse
-        
-            @staticmethod
-            def validation() -> typing.Type['PolicyValidation']:
-                return PolicyValidation
-            __annotations__ = {
-                "draftResponse": draftResponse,
-                "validation": validation,
-            }
-    
-    draftResponse: 'DraftResponse'
-    validation: 'PolicyValidation'
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["draftResponse"]) -> 'DraftResponse': ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["validation"]) -> 'PolicyValidation': ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["draftResponse", "validation", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["draftResponse"]) -> 'DraftResponse': ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["validation"]) -> 'PolicyValidation': ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["draftResponse", "validation", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        draftResponse: 'DraftResponse',
-        validation: 'PolicyValidation',
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'DraftReviewAndValidationResponse':
-        return super().__new__(
-            cls,
-            *_args,
-            draftResponse=draftResponse,
-            validation=validation,
-            _configuration=_configuration,
-            **kwargs,
+    Draft validation
+    """ # noqa: E501
+    draft_response: DraftResponse = Field(alias="draftResponse")
+    validation: PolicyValidation
+    __properties: ClassVar[List[str]] = ["draftResponse", "validation"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
+
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.model_dump(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of DraftReviewAndValidationResponse from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        excluded_fields: Set[str] = set([
+        ])
+
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude=excluded_fields,
+            exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of draft_response
+        if self.draft_response:
+            _dict['draftResponse'] = self.draft_response.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of validation
+        if self.validation:
+            _dict['validation'] = self.validation.to_dict()
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of DraftReviewAndValidationResponse from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return cls.model_validate(obj)
+
+        _obj = cls.model_validate({
+            "draftResponse": DraftResponse.from_dict(obj["draftResponse"]) if obj.get("draftResponse") is not None else None,
+            "validation": PolicyValidation.from_dict(obj["validation"]) if obj.get("validation") is not None else None
+        })
+        return _obj
+
 
-from fireblocks_client.model.draft_response import DraftResponse
-from fireblocks_client.model.policy_validation import PolicyValidation
```

### Comparing `fireblocks-0.0.1/fireblocks_client/model/draft_review_and_validation_response.pyi` & `fireblocks-0.0.2b0/fireblocks/models/policy_and_validation_response.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,107 +1,98 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import frozendict  # noqa: F401
-
-from fireblocks_client import schemas  # noqa: F401
+    Do not edit the class manually.
+"""  # noqa: E501
 
 
-class DraftReviewAndValidationResponse(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
-    Do not edit the class manually.
+from pydantic import BaseModel, ConfigDict
+from typing import Any, ClassVar, Dict, List
+from fireblocks.models.policy_response import PolicyResponse
+from fireblocks.models.policy_validation import PolicyValidation
+from typing import Optional, Set
+from typing_extensions import Self
 
-    Draft validation
+class PolicyAndValidationResponse(BaseModel):
     """
-
-
-    class MetaOapg:
-        required = {
-            "draftResponse",
-            "validation",
-        }
-        
-        class properties:
-        
-            @staticmethod
-            def draftResponse() -> typing.Type['DraftResponse']:
-                return DraftResponse
-        
-            @staticmethod
-            def validation() -> typing.Type['PolicyValidation']:
-                return PolicyValidation
-            __annotations__ = {
-                "draftResponse": draftResponse,
-                "validation": validation,
-            }
-    
-    draftResponse: 'DraftResponse'
-    validation: 'PolicyValidation'
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["draftResponse"]) -> 'DraftResponse': ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["validation"]) -> 'PolicyValidation': ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["draftResponse", "validation", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["draftResponse"]) -> 'DraftResponse': ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["validation"]) -> 'PolicyValidation': ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["draftResponse", "validation", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        draftResponse: 'DraftResponse',
-        validation: 'PolicyValidation',
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'DraftReviewAndValidationResponse':
-        return super().__new__(
-            cls,
-            *_args,
-            draftResponse=draftResponse,
-            validation=validation,
-            _configuration=_configuration,
-            **kwargs,
+    Policy validation
+    """ # noqa: E501
+    policy: PolicyResponse
+    validation: PolicyValidation
+    __properties: ClassVar[List[str]] = ["policy", "validation"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
+
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.model_dump(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of PolicyAndValidationResponse from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        excluded_fields: Set[str] = set([
+        ])
+
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude=excluded_fields,
+            exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of policy
+        if self.policy:
+            _dict['policy'] = self.policy.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of validation
+        if self.validation:
+            _dict['validation'] = self.validation.to_dict()
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of PolicyAndValidationResponse from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return cls.model_validate(obj)
+
+        _obj = cls.model_validate({
+            "policy": PolicyResponse.from_dict(obj["policy"]) if obj.get("policy") is not None else None,
+            "validation": PolicyValidation.from_dict(obj["validation"]) if obj.get("validation") is not None else None
+        })
+        return _obj
+
 
-from fireblocks_client.model.draft_response import DraftResponse
-from fireblocks_client.model.policy_validation import PolicyValidation
```

### Comparing `fireblocks-0.0.1/fireblocks_client/model/fiat_account_type.py` & `fireblocks-0.0.2b0/fireblocks/models/conversion_operation_type.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,37 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
-
-import frozendict  # noqa: F401
-
-from fireblocks_client import schemas  # noqa: F401
-
-
-class FiatAccountType(
-    schemas.EnumBase,
-    schemas.StrSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
+"""  # noqa: E501
+
+
+from __future__ import annotations
+import json
+from enum import Enum
+from typing_extensions import Self
+
+
+class ConversionOperationType(str, Enum):
     """
+    ConversionOperationType
+    """
+
+    """
+    allowed enum values
+    """
+    CONVERSION = 'CONVERSION'
+
+    @classmethod
+    def from_json(cls, json_str: str) -> Self:
+        """Create an instance of ConversionOperationType from a JSON string"""
+        return cls(json.loads(json_str))
 
 
-    class MetaOapg:
-        enum_value_to_name = {
-            "BLINC": "BLINC",
-        }
-    
-    @schemas.classproperty
-    def BLINC(cls):
-        return cls("BLINC")
```

### Comparing `fireblocks-0.0.1/fireblocks_client/model/fiat_account_type.pyi` & `fireblocks-0.0.2b0/test/test_transfer_operation_type.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
-
-import frozendict  # noqa: F401
-
-from fireblocks_client import schemas  # noqa: F401
-
-
-class FiatAccountType(
-    schemas.EnumBase,
-    schemas.StrSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-    """
-    
-    @schemas.classproperty
-    def BLINC(cls):
-        return cls("BLINC")
+"""  # noqa: E501
+
+
+import unittest
+
+from fireblocks.models.transfer_operation_type import TransferOperationType
+
+
+class TestTransferOperationType(unittest.TestCase):
+    """TransferOperationType unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testTransferOperationType(self):
+        """Test TransferOperationType"""
+        # inst = TransferOperationType()
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `fireblocks-0.0.1/fireblocks_client/model/payout_init_method.py` & `fireblocks-0.0.2b0/fireblocks/unknown_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,33 @@
-# coding: utf-8
-
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
-
-import frozendict  # noqa: F401
-
-from fireblocks_client import schemas  # noqa: F401
-
-
-class PayoutInitMethod(
-    schemas.EnumBase,
-    schemas.StrSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-    """
+"""  # noqa: E501
+
+from pydantic import BaseModel, create_model
+import json
+import pprint
+
+
+class UnknownBaseModel(BaseModel):
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.model_dump(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    def to_dict(self):
+        return self.dict()
 
 
-    class MetaOapg:
-        enum_value_to_name = {
-            "FILE": "FILE",
-            "API": "API",
-        }
-    
-    @schemas.classproperty
-    def FILE(cls):
-        return cls("FILE")
-    
-    @schemas.classproperty
-    def API(cls):
-        return cls("API")
+def create_unknown_model(data):
+    fields = {f: (type(v), ...) for f, v in data.items()}
+    return create_model("UnknownModel", __base__=UnknownBaseModel, **fields)
```

### Comparing `fireblocks-0.0.1/fireblocks_client/model/payout_init_method.pyi` & `fireblocks-0.0.2b0/test/test_payout_init_method.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,36 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
-
-import frozendict  # noqa: F401
-
-from fireblocks_client import schemas  # noqa: F401
-
-
-class PayoutInitMethod(
-    schemas.EnumBase,
-    schemas.StrSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-    """
-    
-    @schemas.classproperty
-    def FILE(cls):
-        return cls("FILE")
-    
-    @schemas.classproperty
-    def API(cls):
-        return cls("API")
+"""  # noqa: E501
+
+
+import unittest
+
+from fireblocks.models.payout_init_method import PayoutInitMethod
+
+
+class TestPayoutInitMethod(unittest.TestCase):
+    """PayoutInitMethod unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testPayoutInitMethod(self):
+        """Test PayoutInitMethod"""
+        # inst = PayoutInitMethod()
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `fireblocks-0.0.1/fireblocks_client/model/policy_src_or_dest_sub_type.pyi` & `fireblocks-0.0.2b0/fireblocks/models/policy_src_or_dest_sub_type.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,62 +1,41 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
-
-import frozendict  # noqa: F401
-
-from fireblocks_client import schemas  # noqa: F401
-
-
-class PolicySrcOrDestSubType(
-    schemas.EnumBase,
-    schemas.StrSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
+"""  # noqa: E501
+
+
+from __future__ import annotations
+import json
+from enum import Enum
+from typing_extensions import Self
+
 
-    * EXTERNAL - A whitelisted wallet assigned as external is typically used for addresses managed by your clients and counterparties
-* INTERNAL - A whitelisted wallet assigned as internal, is typically used for addresses that you control outside of your Fireblocks workspace
-* CONTRACT - A whitelisted wallet assigned as contract is for identifying and managing external smart contracts
-* EXCHANGETEST - Exchanges which operate only on testnet assets
-* "*" - All subtypes
+class PolicySrcOrDestSubType(str, Enum):
+    """
+    * EXTERNAL - A whitelisted wallet assigned as external is typically used for addresses managed by your clients and counterparties * INTERNAL - A whitelisted wallet assigned as internal, is typically used for addresses that you control outside of your Fireblocks workspace * CONTRACT - A whitelisted wallet assigned as contract is for identifying and managing external smart contracts * EXCHANGETEST - Exchanges which operate only on testnet assets * \"*\" - All subtypes 
+    """
 
     """
-    
-    @schemas.classproperty
-    def EXTERNAL(cls):
-        return cls("EXTERNAL")
-    
-    @schemas.classproperty
-    def INTERNAL(cls):
-        return cls("INTERNAL")
-    
-    @schemas.classproperty
-    def CONTRACT(cls):
-        return cls("CONTRACT")
-    
-    @schemas.classproperty
-    def EXCHANGETEST(cls):
-        return cls("EXCHANGETEST")
-    
-    @schemas.classproperty
-    def ASTERISK(cls):
-        return cls("*")
+    allowed enum values
+    """
+    EXTERNAL = 'EXTERNAL'
+    INTERNAL = 'INTERNAL'
+    CONTRACT = 'CONTRACT'
+    EXCHANGETEST = 'EXCHANGETEST'
+    STAR = '*'
+
+    @classmethod
+    def from_json(cls, json_str: str) -> Self:
+        """Create an instance of PolicySrcOrDestSubType from a JSON string"""
+        return cls(json.loads(json_str))
+
+
```

### Comparing `fireblocks-0.0.1/fireblocks_client/model/policy_validation.py` & `fireblocks-0.0.2b0/fireblocks/models/policy_validation.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,103 +1,94 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import frozendict  # noqa: F401
-
-from fireblocks_client import schemas  # noqa: F401
+    Do not edit the class manually.
+"""  # noqa: E501
 
 
-class PolicyValidation(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
-    Do not edit the class manually.
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
+from typing import Any, ClassVar, Dict, List
+from fireblocks.models.policy_check_result import PolicyCheckResult
+from typing import Optional, Set
+from typing_extensions import Self
 
-    Policy validation object
+class PolicyValidation(BaseModel):
     """
-
-
-    class MetaOapg:
-        required = {
-            "checkResult",
-            "status",
-        }
-        
-        class properties:
-            status = schemas.StrSchema
-        
-            @staticmethod
-            def checkResult() -> typing.Type['PolicyCheckResult']:
-                return PolicyCheckResult
-            __annotations__ = {
-                "status": status,
-                "checkResult": checkResult,
-            }
-    
-    checkResult: 'PolicyCheckResult'
-    status: MetaOapg.properties.status
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["status"]) -> MetaOapg.properties.status: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["checkResult"]) -> 'PolicyCheckResult': ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["status", "checkResult", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["status"]) -> MetaOapg.properties.status: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["checkResult"]) -> 'PolicyCheckResult': ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["status", "checkResult", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        checkResult: 'PolicyCheckResult',
-        status: typing.Union[MetaOapg.properties.status, str, ],
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'PolicyValidation':
-        return super().__new__(
-            cls,
-            *_args,
-            checkResult=checkResult,
-            status=status,
-            _configuration=_configuration,
-            **kwargs,
+    Policy validation object
+    """ # noqa: E501
+    status: StrictStr = Field(description="Validation status")
+    check_result: PolicyCheckResult = Field(alias="checkResult")
+    __properties: ClassVar[List[str]] = ["status", "checkResult"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
+
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.model_dump(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of PolicyValidation from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        excluded_fields: Set[str] = set([
+        ])
+
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude=excluded_fields,
+            exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of check_result
+        if self.check_result:
+            _dict['checkResult'] = self.check_result.to_dict()
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of PolicyValidation from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return cls.model_validate(obj)
+
+        _obj = cls.model_validate({
+            "status": obj.get("status"),
+            "checkResult": PolicyCheckResult.from_dict(obj["checkResult"]) if obj.get("checkResult") is not None else None
+        })
+        return _obj
+
 
-from fireblocks_client.model.policy_check_result import PolicyCheckResult
```

### Comparing `fireblocks-0.0.1/fireblocks_client/model/policy_validation.pyi` & `fireblocks-0.0.2b0/fireblocks/models/policy_response.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,103 +1,102 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import frozendict  # noqa: F401
-
-from fireblocks_client import schemas  # noqa: F401
+    Do not edit the class manually.
+"""  # noqa: E501
 
 
-class PolicyValidation(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
-    Do not edit the class manually.
+from pydantic import BaseModel, ConfigDict, Field
+from typing import Any, ClassVar, Dict, List
+from fireblocks.models.policy_metadata import PolicyMetadata
+from fireblocks.models.policy_rule import PolicyRule
+from typing import Optional, Set
+from typing_extensions import Self
 
-    Policy validation object
+class PolicyResponse(BaseModel):
     """
-
-
-    class MetaOapg:
-        required = {
-            "checkResult",
-            "status",
-        }
-        
-        class properties:
-            status = schemas.StrSchema
-        
-            @staticmethod
-            def checkResult() -> typing.Type['PolicyCheckResult']:
-                return PolicyCheckResult
-            __annotations__ = {
-                "status": status,
-                "checkResult": checkResult,
-            }
-    
-    checkResult: 'PolicyCheckResult'
-    status: MetaOapg.properties.status
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["status"]) -> MetaOapg.properties.status: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["checkResult"]) -> 'PolicyCheckResult': ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["status", "checkResult", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["status"]) -> MetaOapg.properties.status: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["checkResult"]) -> 'PolicyCheckResult': ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["status", "checkResult", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        checkResult: 'PolicyCheckResult',
-        status: typing.Union[MetaOapg.properties.status, str, ],
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'PolicyValidation':
-        return super().__new__(
-            cls,
-            *_args,
-            checkResult=checkResult,
-            status=status,
-            _configuration=_configuration,
-            **kwargs,
+    Response object for policy operations
+    """ # noqa: E501
+    rules: List[PolicyRule] = Field(description="A set of policy rules")
+    metadata: PolicyMetadata
+    __properties: ClassVar[List[str]] = ["rules", "metadata"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
+
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.model_dump(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of PolicyResponse from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        excluded_fields: Set[str] = set([
+        ])
+
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude=excluded_fields,
+            exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of each item in rules (list)
+        _items = []
+        if self.rules:
+            for _item in self.rules:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['rules'] = _items
+        # override the default output from pydantic by calling `to_dict()` of metadata
+        if self.metadata:
+            _dict['metadata'] = self.metadata.to_dict()
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of PolicyResponse from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return cls.model_validate(obj)
+
+        _obj = cls.model_validate({
+            "rules": [PolicyRule.from_dict(_item) for _item in obj["rules"]] if obj.get("rules") is not None else None,
+            "metadata": PolicyMetadata.from_dict(obj["metadata"]) if obj.get("metadata") is not None else None
+        })
+        return _obj
+
 
-from fireblocks_client.model.policy_check_result import PolicyCheckResult
```

### Comparing `fireblocks-0.0.1/fireblocks_client/model/set_confirmations_threshold_request.py` & `fireblocks-0.0.2b0/fireblocks/models/gas_station_properties_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,79 +1,94 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import frozendict  # noqa: F401
+    Do not edit the class manually.
+"""  # noqa: E501
 
-from fireblocks_client import schemas  # noqa: F401
 
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
-class SetConfirmationsThresholdRequest(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+from pydantic import BaseModel, ConfigDict
+from typing import Any, ClassVar, Dict, List, Optional
+from fireblocks.models.gas_station_configuration_response import GasStationConfigurationResponse
+from typing import Optional, Set
+from typing_extensions import Self
 
-    Do not edit the class manually.
+class GasStationPropertiesResponse(BaseModel):
     """
+    GasStationPropertiesResponse
+    """ # noqa: E501
+    balance: Optional[Dict[str, Any]] = None
+    configuration: Optional[GasStationConfigurationResponse] = None
+    __properties: ClassVar[List[str]] = ["balance", "configuration"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
+
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.model_dump(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of GasStationPropertiesResponse from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        excluded_fields: Set[str] = set([
+        ])
+
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude=excluded_fields,
+            exclude_none=True,
+        )
+        # override the default output from pydantic by calling `to_dict()` of configuration
+        if self.configuration:
+            _dict['configuration'] = self.configuration.to_dict()
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of GasStationPropertiesResponse from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return cls.model_validate(obj)
+
+        _obj = cls.model_validate({
+            "balance": obj.get("balance"),
+            "configuration": GasStationConfigurationResponse.from_dict(obj["configuration"]) if obj.get("configuration") is not None else None
+        })
+        return _obj
 
 
-    class MetaOapg:
-        
-        class properties:
-            numOfConfirmations = schemas.NumberSchema
-            __annotations__ = {
-                "numOfConfirmations": numOfConfirmations,
-            }
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["numOfConfirmations"]) -> MetaOapg.properties.numOfConfirmations: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["numOfConfirmations", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["numOfConfirmations"]) -> typing.Union[MetaOapg.properties.numOfConfirmations, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["numOfConfirmations", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        numOfConfirmations: typing.Union[MetaOapg.properties.numOfConfirmations, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SetConfirmationsThresholdRequest':
-        return super().__new__(
-            cls,
-            *_args,
-            numOfConfirmations=numOfConfirmations,
-            _configuration=_configuration,
-            **kwargs,
-        )
```

### Comparing `fireblocks-0.0.1/fireblocks_client/model/transaction_operation.py` & `fireblocks-0.0.2b0/fireblocks/models/transaction_operation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,78 +1,42 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
-
-import frozendict  # noqa: F401
-
-from fireblocks_client import schemas  # noqa: F401
-
-
-class TransactionOperation(
-    schemas.EnumBase,
-    schemas.StrSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
+"""  # noqa: E501
+
+
+from __future__ import annotations
+import json
+from enum import Enum
+from typing_extensions import Self
 
-    * `TRANSFER` - The default value for an operation. Transfers funds from one account to another. UTXO blockchains allow multi-input and multi-output transfers. All other blockchains allow transfers with one source address and one destination address.
-* `MINT` - Mints new tokens. Supported for Stellar, Ripple and EVM-based blockchains.
-* `BURN` - Burns tokens. Supported for Stellar, Ripple and EVM-based blockchains.
-* `CONTRACT_CALL` - Calls a smart contract method for web3 operations on any EVM blockchain. The Fireblocks [development libraries](https://developers.fireblocks.com/docs/ethereum-development#convenience-libraries) are recommended for building contract call transactions.
-* `TYPED_MESSAGE` - An off-chain message in either Ethereum Personal Message or EIP712 format. Use it to sign specific readable messages that are not actual transactions. [Learn more about typed messages](https://developers.fireblocks.com/docs/typed-message-signing).
-* `RAW` - An off-chain message with no predefined format. Use it to sign any message with your private key, including protocols such as blockchains and custom transaction types that are not natively supported by Fireblocks. [Learn more about raw signing transactions.](https://developers.fireblocks.com/docs/raw-message-signing)
 
+class TransactionOperation(str, Enum):
+    """
+    * `TRANSFER` - The default value for an operation. Transfers funds from one account to another. UTXO blockchains allow multi-input and multi-output transfers. All other blockchains allow transfers with one source address and one destination address. * `MINT` - Mints new tokens. Supported for Stellar, Ripple and EVM-based blockchains. * `BURN` - Burns tokens. Supported for Stellar, Ripple and EVM-based blockchains. * `CONTRACT_CALL` - Calls a smart contract method for web3 operations on any EVM blockchain. The Fireblocks [development libraries](https://developers.fireblocks.com/docs/ethereum-development#convenience-libraries) are recommended for building contract call transactions. * `TYPED_MESSAGE` - An off-chain message in either Ethereum Personal Message or EIP712 format. Use it to sign specific readable messages that are not actual transactions. [Learn more about typed messages](https://developers.fireblocks.com/docs/typed-message-signing). * `RAW` - An off-chain message with no predefined format. Use it to sign any message with your private key, including protocols such as blockchains and custom transaction types that are not natively supported by Fireblocks. [Learn more about raw signing transactions.](https://developers.fireblocks.com/docs/raw-message-signing) 
+    """
+
+    """
+    allowed enum values
     """
+    TRANSFER = 'TRANSFER'
+    BURN = 'BURN'
+    CONTRACT_CALL = 'CONTRACT_CALL'
+    MINT = 'MINT'
+    RAW = 'RAW'
+    TYPED_MESSAGE = 'TYPED_MESSAGE'
+
+    @classmethod
+    def from_json(cls, json_str: str) -> Self:
+        """Create an instance of TransactionOperation from a JSON string"""
+        return cls(json.loads(json_str))
 
 
-    class MetaOapg:
-        enum_value_to_name = {
-            "TRANSFER": "TRANSFER",
-            "BURN": "BURN",
-            "CONTRACT_CALL": "CONTRACT_CALL",
-            "MINT": "MINT",
-            "RAW": "RAW",
-            "TYPED_MESSAGE": "TYPED_MESSAGE",
-        }
-    
-    @schemas.classproperty
-    def TRANSFER(cls):
-        return cls("TRANSFER")
-    
-    @schemas.classproperty
-    def BURN(cls):
-        return cls("BURN")
-    
-    @schemas.classproperty
-    def CONTRACT_CALL(cls):
-        return cls("CONTRACT_CALL")
-    
-    @schemas.classproperty
-    def MINT(cls):
-        return cls("MINT")
-    
-    @schemas.classproperty
-    def RAW(cls):
-        return cls("RAW")
-    
-    @schemas.classproperty
-    def TYPED_MESSAGE(cls):
-        return cls("TYPED_MESSAGE")
```

### Comparing `fireblocks-0.0.1/fireblocks_client/model/transaction_request_destination.py` & `fireblocks-0.0.2b0/fireblocks/models/transaction_request_destination.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,94 +1,94 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import frozendict  # noqa: F401
+    Do not edit the class manually.
+"""  # noqa: E501
 
-from fireblocks_client import schemas  # noqa: F401
 
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
-class TransactionRequestDestination(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+from pydantic import BaseModel, ConfigDict, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
+from fireblocks.models.destination_transfer_peer_path import DestinationTransferPeerPath
+from typing import Optional, Set
+from typing_extensions import Self
 
-    Do not edit the class manually.
+class TransactionRequestDestination(BaseModel):
     """
-
-
-    class MetaOapg:
-        
-        class properties:
-            amount = schemas.StrSchema
-        
-            @staticmethod
-            def destination() -> typing.Type['DestinationTransferPeerPath']:
-                return DestinationTransferPeerPath
-            __annotations__ = {
-                "amount": amount,
-                "destination": destination,
-            }
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["amount"]) -> MetaOapg.properties.amount: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["destination"]) -> 'DestinationTransferPeerPath': ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["amount", "destination", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["amount"]) -> typing.Union[MetaOapg.properties.amount, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["destination"]) -> typing.Union['DestinationTransferPeerPath', schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["amount", "destination", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        amount: typing.Union[MetaOapg.properties.amount, str, schemas.Unset] = schemas.unset,
-        destination: typing.Union['DestinationTransferPeerPath', schemas.Unset] = schemas.unset,
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'TransactionRequestDestination':
-        return super().__new__(
-            cls,
-            *_args,
-            amount=amount,
-            destination=destination,
-            _configuration=_configuration,
-            **kwargs,
+    TransactionRequestDestination
+    """ # noqa: E501
+    amount: Optional[StrictStr] = None
+    destination: Optional[DestinationTransferPeerPath] = None
+    __properties: ClassVar[List[str]] = ["amount", "destination"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
+
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.model_dump(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of TransactionRequestDestination from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        excluded_fields: Set[str] = set([
+        ])
+
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude=excluded_fields,
+            exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of destination
+        if self.destination:
+            _dict['destination'] = self.destination.to_dict()
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of TransactionRequestDestination from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return cls.model_validate(obj)
+
+        _obj = cls.model_validate({
+            "amount": obj.get("amount"),
+            "destination": DestinationTransferPeerPath.from_dict(obj["destination"]) if obj.get("destination") is not None else None
+        })
+        return _obj
+
 
-from fireblocks_client.model.destination_transfer_peer_path import DestinationTransferPeerPath
```

### Comparing `fireblocks-0.0.1/fireblocks_client/model/update_token_ownership_status_dto.pyi` & `fireblocks-0.0.2b0/fireblocks/models/create_disbursement_config_operation_request.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,97 +1,95 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import frozendict  # noqa: F401
+    Do not edit the class manually.
+"""  # noqa: E501
 
-from fireblocks_client import schemas  # noqa: F401
 
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
-class UpdateTokenOwnershipStatusDto(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+from pydantic import BaseModel, ConfigDict
+from typing import Any, ClassVar, Dict, List
+from fireblocks.models.disbursement_operation_config_params import DisbursementOperationConfigParams
+from fireblocks.models.disbursement_operation_type import DisbursementOperationType
+from typing import Optional, Set
+from typing_extensions import Self
 
-    Do not edit the class manually.
+class CreateDisbursementConfigOperationRequest(BaseModel):
     """
+    CreateDisbursementConfigOperationRequest
+    """ # noqa: E501
+    type: DisbursementOperationType
+    params: DisbursementOperationConfigParams
+    __properties: ClassVar[List[str]] = ["type", "params"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
+
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.model_dump(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of CreateDisbursementConfigOperationRequest from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        excluded_fields: Set[str] = set([
+        ])
+
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude=excluded_fields,
+            exclude_none=True,
+        )
+        # override the default output from pydantic by calling `to_dict()` of params
+        if self.params:
+            _dict['params'] = self.params.to_dict()
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of CreateDisbursementConfigOperationRequest from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return cls.model_validate(obj)
+
+        _obj = cls.model_validate({
+            "type": obj.get("type"),
+            "params": DisbursementOperationConfigParams.from_dict(obj["params"]) if obj.get("params") is not None else None
+        })
+        return _obj
 
 
-    class MetaOapg:
-        required = {
-            "status",
-        }
-        
-        class properties:
-            
-            
-            class status(
-                schemas.EnumBase,
-                schemas.StrSchema
-            ):
-                
-                @schemas.classproperty
-                def LISTED(cls):
-                    return cls("LISTED")
-                
-                @schemas.classproperty
-                def ARCHIVED(cls):
-                    return cls("ARCHIVED")
-            __annotations__ = {
-                "status": status,
-            }
-    
-    status: MetaOapg.properties.status
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["status"]) -> MetaOapg.properties.status: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["status", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["status"]) -> MetaOapg.properties.status: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["status", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        status: typing.Union[MetaOapg.properties.status, str, ],
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'UpdateTokenOwnershipStatusDto':
-        return super().__new__(
-            cls,
-            *_args,
-            status=status,
-            _configuration=_configuration,
-            **kwargs,
-        )
```

### Comparing `fireblocks-0.0.1/fireblocks_client/model/xb_settlement_asset_id.py` & `fireblocks-0.0.2b0/fireblocks/models/create_console_user.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,69 +1,94 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import frozendict  # noqa: F401
+    Do not edit the class manually.
+"""  # noqa: E501
 
-from fireblocks_client import schemas  # noqa: F401
 
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
-class XBSettlementAssetID(
-    schemas.ComposedSchema,
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
+from typing import Any, ClassVar, Dict, List
+from typing import Optional, Set
+from typing_extensions import Self
 
-    Do not edit the class manually.
+class CreateConsoleUser(BaseModel):
     """
+    CreateConsoleUser
+    """ # noqa: E501
+    first_name: StrictStr = Field(description="users firstName", alias="firstName")
+    last_name: StrictStr = Field(description="users lastName", alias="lastName")
+    role: StrictStr = Field(description="users role")
+    email: StrictStr = Field(description="valid email address")
+    __properties: ClassVar[List[str]] = ["firstName", "lastName", "role", "email"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
+
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.model_dump(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of CreateConsoleUser from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        excluded_fields: Set[str] = set([
+        ])
+
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude=excluded_fields,
+            exclude_none=True,
+        )
+        return _dict
 
+    @classmethod
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of CreateConsoleUser from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return cls.model_validate(obj)
+
+        _obj = cls.model_validate({
+            "firstName": obj.get("firstName"),
+            "lastName": obj.get("lastName"),
+            "role": obj.get("role"),
+            "email": obj.get("email")
+        })
+        return _obj
 
-    class MetaOapg:
-        
-        @classmethod
-        @functools.lru_cache()
-        def one_of(cls):
-            # we need this here to make our import statements work
-            # we must store _composed_schemas in here so the code is only run
-            # when we invoke this method. If we kept this at the class
-            # level we would get an error because the class level
-            # code would be run when this module is imported, and these composed
-            # classes don't exist yet because their module has not finished
-            # loading
-            return [
-                XBSettlementFiatAsset,
-                XBSettlementCryptoAsset,
-            ]
-
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'XBSettlementAssetID':
-        return super().__new__(
-            cls,
-            *_args,
-            _configuration=_configuration,
-            **kwargs,
-        )
 
-from fireblocks_client.model.xb_settlement_crypto_asset import XBSettlementCryptoAsset
-from fireblocks_client.model.xb_settlement_fiat_asset import XBSettlementFiatAsset
```

### Comparing `fireblocks-0.0.1/fireblocks_client/model/xb_settlement_conversion_slippage_basis_points.pyi` & `fireblocks-0.0.2b0/test/test_transfer_peer_path_sub_type.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
-
-import frozendict  # noqa: F401
-
-from fireblocks_client import schemas  # noqa: F401
-
-
-class XBSettlementConversionSlippageBasisPoints(
-    schemas.IntSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
+"""  # noqa: E501
+
+
+import unittest
+
+from fireblocks.models.transfer_peer_path_sub_type import TransferPeerPathSubType
+
+
+class TestTransferPeerPathSubType(unittest.TestCase):
+    """TransferPeerPathSubType unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testTransferPeerPathSubType(self):
+        """Test TransferPeerPathSubType"""
+        # inst = TransferPeerPathSubType()
 
-    Slippage configuarion in basis points, the default value is 10%
 
-    """
-    pass
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `fireblocks-0.0.1/fireblocks_client/model/xb_settlement_crypto_asset.pyi` & `fireblocks-0.0.2b0/test/test_transaction_operation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,36 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
-
-import frozendict  # noqa: F401
-
-from fireblocks_client import schemas  # noqa: F401
-
-
-class XBSettlementCryptoAsset(
-    schemas.EnumBase,
-    schemas.StrSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
+"""  # noqa: E501
+
+
+import unittest
+
+from fireblocks.models.transaction_operation import TransactionOperation
+
+
+class TestTransactionOperation(unittest.TestCase):
+    """TransactionOperation unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testTransactionOperation(self):
+        """Test TransactionOperation"""
+        # inst = TransactionOperation()
 
-    - XLM_USDC_5F3T : USDC over Stellar network
 
-    """
-    
-    @schemas.classproperty
-    def XLM_USDC_5F3T(cls):
-        return cls("XLM_USDC_5F3T")
-    
-    @schemas.classproperty
-    def XLM(cls):
-        return cls("XLM")
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `fireblocks-0.0.1/fireblocks_client/model/xb_settlement_flow_execution_status.py` & `fireblocks-0.0.2b0/test/test_api_key.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,57 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
-
-import frozendict  # noqa: F401
-
-from fireblocks_client import schemas  # noqa: F401
-
-
-class XBSettlementFlowExecutionStatus(
-    schemas.EnumBase,
-    schemas.StrSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-    """
+"""  # noqa: E501
+
+
+import unittest
+
+from fireblocks.models.api_key import ApiKey
+
+
+class TestApiKey(unittest.TestCase):
+    """ApiKey unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional) -> ApiKey:
+        """Test ApiKey
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # uncomment below to create an instance of `ApiKey`
+        """
+        model = ApiKey()
+        if include_optional:
+            return ApiKey(
+                id = '44fcead0-7053-4831-a53a-df7fb90d440f',
+                last_seen = '2021-07-01T00:00Z'
+            )
+        else:
+            return ApiKey(
+                id = '44fcead0-7053-4831-a53a-df7fb90d440f',
+                last_seen = '2021-07-01T00:00Z',
+        )
+        """
+
+    def testApiKey(self):
+        """Test ApiKey"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-    class MetaOapg:
-        enum_value_to_name = {
-            "NOT_LAUNCHED": "NOT_LAUNCHED",
-            "PROCESSING": "PROCESSING",
-            "COMPLETED": "COMPLETED",
-            "FAILED": "FAILED",
-        }
-    
-    @schemas.classproperty
-    def NOT_LAUNCHED(cls):
-        return cls("NOT_LAUNCHED")
-    
-    @schemas.classproperty
-    def PROCESSING(cls):
-        return cls("PROCESSING")
-    
-    @schemas.classproperty
-    def COMPLETED(cls):
-        return cls("COMPLETED")
-    
-    @schemas.classproperty
-    def FAILED(cls):
-        return cls("FAILED")
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `fireblocks-0.0.1/fireblocks_client/model/xb_settlement_flow_execution_status.pyi` & `fireblocks-0.0.2b0/test/test_set_routing_policy_request.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,59 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
-
-import frozendict  # noqa: F401
-
-from fireblocks_client import schemas  # noqa: F401
-
-
-class XBSettlementFlowExecutionStatus(
-    schemas.EnumBase,
-    schemas.StrSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-    """
-    
-    @schemas.classproperty
-    def NOT_LAUNCHED(cls):
-        return cls("NOT_LAUNCHED")
-    
-    @schemas.classproperty
-    def PROCESSING(cls):
-        return cls("PROCESSING")
-    
-    @schemas.classproperty
-    def COMPLETED(cls):
-        return cls("COMPLETED")
-    
-    @schemas.classproperty
-    def FAILED(cls):
-        return cls("FAILED")
+"""  # noqa: E501
+
+
+import unittest
+
+from fireblocks.models.set_routing_policy_request import SetRoutingPolicyRequest
+
+
+class TestSetRoutingPolicyRequest(unittest.TestCase):
+    """SetRoutingPolicyRequest unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional) -> SetRoutingPolicyRequest:
+        """Test SetRoutingPolicyRequest
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # uncomment below to create an instance of `SetRoutingPolicyRequest`
+        """
+        model = SetRoutingPolicyRequest()
+        if include_optional:
+            return SetRoutingPolicyRequest(
+                routing_policy = {
+                    'key' : null
+                    }
+            )
+        else:
+            return SetRoutingPolicyRequest(
+                routing_policy = {
+                    'key' : null
+                    },
+        )
+        """
+
+    def testSetRoutingPolicyRequest(self):
+        """Test SetRoutingPolicyRequest"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `fireblocks-0.0.1/fireblocks_client/model/xb_settlement_flow_selected_conversion_slippage_reason.py` & `fireblocks-0.0.2b0/test/test_policy_rule_operators.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,63 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
-
-import frozendict  # noqa: F401
-
-from fireblocks_client import schemas  # noqa: F401
-
-
-class XBSettlementFlowSelectedConversionSlippageReason(
-    schemas.EnumBase,
-    schemas.StrSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-    """
+"""  # noqa: E501
+
+
+import unittest
+
+from fireblocks.models.policy_rule_operators import PolicyRuleOperators
+
+
+class TestPolicyRuleOperators(unittest.TestCase):
+    """PolicyRuleOperators unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional) -> PolicyRuleOperators:
+        """Test PolicyRuleOperators
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # uncomment below to create an instance of `PolicyRuleOperators`
+        """
+        model = PolicyRuleOperators()
+        if include_optional:
+            return PolicyRuleOperators(
+                wildcard = '*',
+                users = [
+                    ''
+                    ],
+                users_groups = [
+                    ''
+                    ],
+                services = [
+                    ''
+                    ]
+            )
+        else:
+            return PolicyRuleOperators(
+        )
+        """
+
+    def testPolicyRuleOperators(self):
+        """Test PolicyRuleOperators"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-    class MetaOapg:
-        enum_value_to_name = {
-            "DEFAULT": "DEFAULT",
-            "CONFIG": "CONFIG",
-            "FLOW": "FLOW",
-        }
-    
-    @schemas.classproperty
-    def DEFAULT(cls):
-        return cls("DEFAULT")
-    
-    @schemas.classproperty
-    def CONFIG(cls):
-        return cls("CONFIG")
-    
-    @schemas.classproperty
-    def FLOW(cls):
-        return cls("FLOW")
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `fireblocks-0.0.1/fireblocks_client/model/xb_settlement_flow_steps_execution_record.py` & `fireblocks-0.0.2b0/fireblocks/models/settlement_request_body.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,87 +1,88 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import frozendict  # noqa: F401
+    Do not edit the class manually.
+"""  # noqa: E501
 
-from fireblocks_client import schemas  # noqa: F401
 
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
-class XBSettlementFlowStepsExecutionRecord(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
+from typing import Optional, Set
+from typing_extensions import Self
 
-    Do not edit the class manually.
+class SettlementRequestBody(BaseModel):
     """
+    SettlementRequestBody
+    """ # noqa: E501
+    main_exchange_account_id: Optional[StrictStr] = Field(default=None, alias="mainExchangeAccountId")
+    __properties: ClassVar[List[str]] = ["mainExchangeAccountId"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
+
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.model_dump(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of SettlementRequestBody from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        excluded_fields: Set[str] = set([
+        ])
+
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude=excluded_fields,
+            exclude_none=True,
+        )
+        return _dict
 
+    @classmethod
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of SettlementRequestBody from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return cls.model_validate(obj)
+
+        _obj = cls.model_validate({
+            "mainExchangeAccountId": obj.get("mainExchangeAccountId")
+        })
+        return _obj
 
-    class MetaOapg:
-        
-        class properties:
-        
-            @staticmethod
-            def stepType() -> typing.Type['XBSettlementStepType']:
-                return XBSettlementStepType
-            __annotations__ = {
-                "stepType": stepType,
-            }
-        
-        @staticmethod
-        def additional_properties() -> typing.Type['XBSettlementFlowExecutionStep']:
-            return XBSettlementFlowExecutionStep
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["stepType"]) -> 'XBSettlementStepType': ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> 'XBSettlementFlowExecutionStep': ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["stepType"], str, ]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["stepType"]) -> typing.Union['XBSettlementStepType', schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union['XBSettlementFlowExecutionStep', schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["stepType"], str, ]):
-        return super().get_item_oapg(name)
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        stepType: typing.Union['XBSettlementStepType', schemas.Unset] = schemas.unset,
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: 'XBSettlementFlowExecutionStep',
-    ) -> 'XBSettlementFlowStepsExecutionRecord':
-        return super().__new__(
-            cls,
-            *_args,
-            stepType=stepType,
-            _configuration=_configuration,
-            **kwargs,
-        )
 
-from fireblocks_client.model.xb_settlement_flow_execution_step import XBSettlementFlowExecutionStep
-from fireblocks_client.model.xb_settlement_step_type import XBSettlementStepType
```

### Comparing `fireblocks-0.0.1/fireblocks_client/model/xb_settlement_flow_steps_execution_record.pyi` & `fireblocks-0.0.2b0/fireblocks/models/config_conversion_operation_snapshot.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,87 +1,97 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import frozendict  # noqa: F401
+    Do not edit the class manually.
+"""  # noqa: E501
 
-from fireblocks_client import schemas  # noqa: F401
 
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
-class XBSettlementFlowStepsExecutionRecord(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
+from typing import Any, ClassVar, Dict, List
+from fireblocks.models.conversion_operation_config_params import ConversionOperationConfigParams
+from fireblocks.models.conversion_operation_type import ConversionOperationType
+from typing import Optional, Set
+from typing_extensions import Self
 
-    Do not edit the class manually.
+class ConfigConversionOperationSnapshot(BaseModel):
     """
-
-
-    class MetaOapg:
-        
-        class properties:
-        
-            @staticmethod
-            def stepType() -> typing.Type['XBSettlementStepType']:
-                return XBSettlementStepType
-            __annotations__ = {
-                "stepType": stepType,
-            }
-        
-        @staticmethod
-        def additional_properties() -> typing.Type['XBSettlementFlowExecutionStep']:
-            return XBSettlementFlowExecutionStep
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["stepType"]) -> 'XBSettlementStepType': ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> 'XBSettlementFlowExecutionStep': ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["stepType"], str, ]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["stepType"]) -> typing.Union['XBSettlementStepType', schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union['XBSettlementFlowExecutionStep', schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["stepType"], str, ]):
-        return super().get_item_oapg(name)
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        stepType: typing.Union['XBSettlementStepType', schemas.Unset] = schemas.unset,
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: 'XBSettlementFlowExecutionStep',
-    ) -> 'XBSettlementFlowStepsExecutionRecord':
-        return super().__new__(
-            cls,
-            *_args,
-            stepType=stepType,
-            _configuration=_configuration,
-            **kwargs,
+    ConfigConversionOperationSnapshot
+    """ # noqa: E501
+    operation_id: StrictStr = Field(alias="operationId")
+    type: ConversionOperationType
+    params: ConversionOperationConfigParams
+    __properties: ClassVar[List[str]] = ["operationId", "type", "params"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
+
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.model_dump(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of ConfigConversionOperationSnapshot from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        excluded_fields: Set[str] = set([
+        ])
+
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude=excluded_fields,
+            exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of params
+        if self.params:
+            _dict['params'] = self.params.to_dict()
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of ConfigConversionOperationSnapshot from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return cls.model_validate(obj)
+
+        _obj = cls.model_validate({
+            "operationId": obj.get("operationId"),
+            "type": obj.get("type"),
+            "params": ConversionOperationConfigParams.from_dict(obj["params"]) if obj.get("params") is not None else None
+        })
+        return _obj
+
 
-from fireblocks_client.model.xb_settlement_flow_execution_step import XBSettlementFlowExecutionStep
-from fireblocks_client.model.xb_settlement_step_type import XBSettlementStepType
```

### Comparing `fireblocks-0.0.1/fireblocks_client/paths/contracts/post.py` & `fireblocks-0.0.2b0/fireblocks/api/reset_device_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,230 +1,174 @@
 # coding: utf-8
-from dataclasses import dataclass
-import typing_extensions
-from fireblocks_client.model.request_options import RequestOptions
-import urllib3
-from urllib3._collections import HTTPHeaderDict
-
-from fireblocks_client import api_client, exceptions
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
-
-import frozendict  # noqa: F401
-
-from fireblocks_client import schemas  # noqa: F401
-
-from fireblocks_client.model.unmanaged_wallet import UnmanagedWallet
-from fireblocks_client.model.error import Error
-
-from . import path
-
-# body param
-
-
-class SchemaForRequestBodyApplicationJson(
-    schemas.AnyTypeSchema,
-):
-
-
-    class MetaOapg:
-        
-        class properties:
-            name = schemas.StrSchema
-            __annotations__ = {
-                "name": name,
-            }
-
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> typing.Union[MetaOapg.properties.name, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
-        name: typing.Union[MetaOapg.properties.name, str, schemas.Unset] = schemas.unset,
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SchemaForRequestBodyApplicationJson':
-        return super().__new__(
-            cls,
-            *_args,
-            name=name,
-            _configuration=_configuration,
-            **kwargs,
-        )
 
+"""
+    Fireblocks API
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-request_body_any_type = api_client.RequestBody(
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaForRequestBodyApplicationJson),
-    },
-)
-XRequestIDSchema = schemas.StrSchema
-x_request_id_parameter = api_client.HeaderParameter(
-    name="X-Request-ID",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=XRequestIDSchema,
-)
-SchemaFor200ResponseBody = UnmanagedWallet
-ResponseHeadersFor200 = typing_extensions.TypedDict(
-    'ResponseHeadersFor200',
-    {
-        'X-Request-ID': XRequestIDSchema,
-    }
-)
-
-
-@dataclass
-class ApiResponseFor200(api_client.ApiResponse):
-    response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor200ResponseBody,
-    ]
-    headers: ResponseHeadersFor200
-
-
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
-    content={
-        '*/*': api_client.MediaType(
-            schema=SchemaFor200ResponseBody),
-    },
-    headers=[
-        x_request_id_parameter,
-    ]
-)
-XRequestIDSchema = schemas.StrSchema
-x_request_id_parameter = api_client.HeaderParameter(
-    name="X-Request-ID",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=XRequestIDSchema,
-)
-SchemaFor0ResponseBodyApplicationJson = Error
-ResponseHeadersFor0 = typing_extensions.TypedDict(
-    'ResponseHeadersFor0',
-    {
-        'X-Request-ID': XRequestIDSchema,
-    }
-)
-
-
-@dataclass
-class ApiResponseForDefault(api_client.ApiResponse):
-    response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor0ResponseBodyApplicationJson,
-    ]
-    headers: ResponseHeadersFor0
-
-
-_response_for_default = api_client.OpenApiResponse(
-    response_cls=ApiResponseForDefault,
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor0ResponseBodyApplicationJson),
-    },
-    headers=[
-        x_request_id_parameter,
-    ]
-)
-_status_code_to_response = {
-    '200': _response_for_200,
-    'default': _response_for_default,
-}
-_all_accept_content_types = (
-    '*/*',
-    'application/json',
-)
-
-
-class BaseApi(api_client.Api):
-
-    def _create_contract_oapg(self, params: typing.Union[SchemaForRequestBodyApplicationJson,] = None, request_options: RequestOptions = None):
-        """
-        Create a contract
-        """
-        used_path = path.value
-        _headers = HTTPHeaderDict()
-        _fields = None
-        _body = None
-        serialized_data = request_body_any_type.serialize(params, "application/json")
-        _headers.add('Content-Type', "application/json")
-        if 'fields' in serialized_data:
-            _fields = serialized_data['fields']
-
-        elif 'body' in serialized_data:
-                _body = serialized_data['body']
-
-        if request_options and request_options.get("idempotency_key"):
-            idempotency_key = request_options.get("idempotency_key")
-            if idempotency_key:
-                _headers.add("Idempotency-Key", idempotency_key)
-
-        response = self.api_client.call_api(
-            resource_path=used_path,
-            method='post'.upper(),
-            headers=_headers,
-            fields=_fields,
-            body=_body,
-            timeout=10000,
+    The version of the OpenAPI document: 1.6.2
+    Contact: support@fireblocks.com
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
+import warnings
+from concurrent.futures import Future
+from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
+from typing import Any, Dict, List, Optional, Tuple, Union
+from typing_extensions import Annotated
+
+from pydantic import Field, StrictStr
+from typing import Optional
+from typing_extensions import Annotated
+
+from fireblocks.api_client import ApiClient, RequestSerialized
+from fireblocks.api_response import ApiResponse
+from fireblocks.rest import RESTResponseType
+
+
+class ResetDeviceApi:
+    """NOTE: This class is auto generated by OpenAPI Generator
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+    """
+
+    def __init__(self, api_client=None) -> None:
+        if api_client is None:
+            api_client = ApiClient.get_default()
+        self.api_client = api_client
+
+
+    @validate_call
+    def reset_device(
+        self,
+        id: Annotated[StrictStr, Field(description="The ID of the console user")],
+        idempotency_key: Annotated[Optional[StrictStr], Field(description="A unique identifier for the request. If the request is sent multiple times with the same idempotency key, the server will return the same response as the first request. The idempotency key is valid for 24 hours.")] = None,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> Future[ApiResponse[None]]:
+        """Resets device
+
+        Resets mobile device for given console user, that user will need to do mobile onboarding again.
+
+        :param id: The ID of the console user (required)
+        :type id: str
+        :param idempotency_key: A unique identifier for the request. If the request is sent multiple times with the same idempotency key, the server will return the same response as the first request. The idempotency key is valid for 24 hours.
+        :type idempotency_key: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._reset_device_serialize(
+            id=id,
+            idempotency_key=idempotency_key,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
         )
 
-        response_for_status = _status_code_to_response.get(str(response.status))
-        if response_for_status:
-            api_response = response_for_status.deserialize(response, self.api_client.configuration)
-        else:
-            default_response = _status_code_to_response.get('default')
-            if default_response:
-                api_response = default_response.deserialize(response, self.api_client.configuration)
-            else:
-                api_response = api_client.ApiResponseWithoutDeserialization(response=response)
-
-        if not 200 <= response.status <= 299:
-            raise exceptions.ApiException(
-                status=response.status,
-                reason=response.reason,
-                api_response=api_response
-            )
-
-        return api_response.body
-
-
-class CreateContract(BaseApi):
-    # this class is used by api classes that refer to endpoints with operationId fn names
-
-    def create_contract(self , params: typing.Union[SchemaForRequestBodyApplicationJson,] = None, request_options: RequestOptions = None):
-        return self._create_contract_oapg(params, request_options)
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': None,
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
+            '5XX': "ErrorResponse",
+            'default': "ErrorSchema",
+        }
+
+        return self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout,
+            _response_types_map=_response_types_map,
+        )
 
+    def _reset_device_serialize(
+        self,
+        id,
+        idempotency_key,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, Union[str, bytes]] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        if id is not None:
+            _path_params['id'] = id
+        # process the query parameters
+        # process the header parameters
+        if idempotency_key is not None:
+            _header_params['Idempotency-Key'] = idempotency_key
+        # process the form parameters
+        # process the body parameter
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
 
-class ApiForpost(BaseApi):
-    # this class is used by api classes that refer to endpoints by path and http method names
 
-    def post(self , params: typing.Union[SchemaForRequestBodyApplicationJson,] = None, request_options: RequestOptions = None):
-        return self._create_contract_oapg(params, request_options)
+        # authentication setting
+        _auth_settings: List[str] = [
+        ]
+
+        return self.api_client.param_serialize(
+            method='POST',
+            resource_path='/management/users/{id}/reset_device',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
```

### Comparing `fireblocks-0.0.1/fireblocks_client/paths/contracts_contract_id/delete.pyi` & `fireblocks-0.0.2b0/fireblocks/api/users_api.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,182 +1,156 @@
 # coding: utf-8
-from dataclasses import dataclass
-import typing_extensions
-from fireblocks_client.model.request_options import RequestOptions
-import urllib3
-from urllib3._collections import HTTPHeaderDict
-
-from fireblocks_client import api_client, exceptions
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
-
-import frozendict  # noqa: F401
-
-from fireblocks_client import schemas  # noqa: F401
-
-from fireblocks_client.model.error import Error
-
-# Path params
-ContractIdSchema = schemas.StrSchema
-RequestRequiredPathParams = typing_extensions.TypedDict(
-    'RequestRequiredPathParams',
-    {
-        'contractId': typing.Union[ContractIdSchema, str, ],
-    }
-)
-RequestOptionalPathParams = typing_extensions.TypedDict(
-    'RequestOptionalPathParams',
-    {
-    },
-    total=False
-)
-
-
-class RequestPathParams(RequestRequiredPathParams, RequestOptionalPathParams):
-    pass
-
-
-request_path_contract_id = api_client.PathParameter(
-    name="contractId",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=ContractIdSchema,
-    required=True,
-)
-XRequestIDSchema = schemas.StrSchema
-ResponseHeadersFor201 = typing_extensions.TypedDict(
-    'ResponseHeadersFor201',
-    {
-        'X-Request-ID': XRequestIDSchema,
-    }
-)
-
-
-@dataclass
-class ApiResponseFor201(api_client.ApiResponse):
-    response: urllib3.HTTPResponse
-    headers: ResponseHeadersFor201
-    body: schemas.Unset = schemas.unset
-
-
-_response_for_201 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor201,
-    headers=[
-        x_request_id_parameter,
-    ]
-)
-XRequestIDSchema = schemas.StrSchema
-SchemaFor0ResponseBodyApplicationJson = Error
-ResponseHeadersFor0 = typing_extensions.TypedDict(
-    'ResponseHeadersFor0',
-    {
-        'X-Request-ID': XRequestIDSchema,
-    }
-)
-
-
-@dataclass
-class ApiResponseForDefault(api_client.ApiResponse):
-    response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor0ResponseBodyApplicationJson,
-    ]
-    headers: ResponseHeadersFor0
-
-
-_response_for_default = api_client.OpenApiResponse(
-    response_cls=ApiResponseForDefault,
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor0ResponseBodyApplicationJson),
-    },
-    headers=[
-        x_request_id_parameter,
-    ]
-)
-_all_accept_content_types = (
-    'application/json',
-)
-
-
-class BaseApi(api_client.Api):
-
-    def _delete_contract_oapg(self, params: typing.Union[ RequestPathParams] = None, request_options: RequestOptions = None):
-        """
-        Delete a contract
-        """
-        path_params = {}
-        for parameter in (
-            request_path_contract_id,
-        ):
-            if params and params.get(parameter.name):
-                path_params[parameter.name] = params.get(parameter.name)
-        self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
-        used_path = path.value
-
-        _path_params = {}
-        for parameter in (
-            request_path_contract_id,
-        ):
-            parameter_data = path_params.get(parameter.name, schemas.unset)
-            if parameter_data is schemas.unset:
-                continue
-            serialized_data = parameter.serialize(parameter_data)
-            _path_params.update(serialized_data)
-
-        for k, v in _path_params.items():
-            used_path = used_path.replace('{%s}' % k, v)
-        _headers = HTTPHeaderDict()
-        _fields = None
-        _body = None
-
-        if request_options and request_options.get("idempotency_key"):
-            idempotency_key = request_options.get("idempotency_key")
-            if idempotency_key:
-                _headers.add("Idempotency-Key", idempotency_key)
-
-        response = self.api_client.call_api(
-            resource_path=used_path,
-            method='delete'.upper(),
-            headers=_headers,
-            timeout=10000,
+
+"""
+    Fireblocks API
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
+
+    The version of the OpenAPI document: 1.6.2
+    Contact: support@fireblocks.com
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
+import warnings
+from concurrent.futures import Future
+from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
+from typing import Any, Dict, List, Optional, Tuple, Union
+from typing_extensions import Annotated
+
+from typing import List
+from fireblocks.models.user_response import UserResponse
+
+from fireblocks.api_client import ApiClient, RequestSerialized
+from fireblocks.api_response import ApiResponse
+from fireblocks.rest import RESTResponseType
+
+
+class UsersApi:
+    """NOTE: This class is auto generated by OpenAPI Generator
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+    """
+
+    def __init__(self, api_client=None) -> None:
+        if api_client is None:
+            api_client = ApiClient.get_default()
+        self.api_client = api_client
+
+
+    @validate_call
+    def get_users(
+        self,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> Future[ApiResponse[List[UserResponse]]]:
+        """List users
+
+        List all users for the workspace.  Please note that this endpoint is available only for API keys with Admin permissions. 
+
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._get_users_serialize(
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
         )
 
-        response_for_status = _status_code_to_response.get(str(response.status))
-        if response_for_status:
-            api_response = response_for_status.deserialize(response, self.api_client.configuration)
-        else:
-            default_response = _status_code_to_response.get('default')
-            if default_response:
-                api_response = default_response.deserialize(response, self.api_client.configuration)
-            else:
-                api_response = api_client.ApiResponseWithoutDeserialization(response=response)
-
-        if not 200 <= response.status <= 299:
-            raise exceptions.ApiException(
-                status=response.status,
-                reason=response.reason,
-                api_response=api_response
-            )
-
-        return api_response.body
-
-
-class DeleteContract(BaseApi):
-    # this class is used by api classes that refer to endpoints with operationId fn names
-
-    def delete_contract(self , params: typing.Union[ RequestPathParams] = None, request_options: RequestOptions = None):
-        return self._delete_contract_oapg(params, request_options)
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "List[UserResponse]",
+            'default': "ErrorSchema",
+        }
+
+        return self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout,
+            _response_types_map=_response_types_map,
+        )
 
+    def _get_users_serialize(
+        self,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, Union[str, bytes]] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
 
-class ApiFordelete(BaseApi):
-    # this class is used by api classes that refer to endpoints by path and http method names
 
-    def delete(self , params: typing.Union[ RequestPathParams] = None, request_options: RequestOptions = None):
-        return self._delete_contract_oapg(params, request_options)
+        # authentication setting
+        _auth_settings: List[str] = [
+        ]
+
+        return self.api_client.param_serialize(
+            method='GET',
+            resource_path='/users',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
```

### Comparing `fireblocks-0.0.1/fireblocks_client/paths/external_wallets/post.py` & `fireblocks-0.0.2b0/fireblocks/api/assets_api.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,240 +1,186 @@
 # coding: utf-8
-from dataclasses import dataclass
-import typing_extensions
-from fireblocks_client.model.request_options import RequestOptions
-import urllib3
-from urllib3._collections import HTTPHeaderDict
-
-from fireblocks_client import api_client, exceptions
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
-
-import frozendict  # noqa: F401
-
-from fireblocks_client import schemas  # noqa: F401
-
-from fireblocks_client.model.unmanaged_wallet import UnmanagedWallet
-from fireblocks_client.model.error import Error
-
-from . import path
-
-# body param
-
-
-class SchemaForRequestBodyApplicationJson(
-    schemas.AnyTypeSchema,
-):
-
-
-    class MetaOapg:
-        
-        class properties:
-            name = schemas.StrSchema
-            customerRefId = schemas.StrSchema
-            __annotations__ = {
-                "name": name,
-                "customerRefId": customerRefId,
-            }
-
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["customerRefId"]) -> MetaOapg.properties.customerRefId: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", "customerRefId", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> typing.Union[MetaOapg.properties.name, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["customerRefId"]) -> typing.Union[MetaOapg.properties.customerRefId, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", "customerRefId", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
-        name: typing.Union[MetaOapg.properties.name, str, schemas.Unset] = schemas.unset,
-        customerRefId: typing.Union[MetaOapg.properties.customerRefId, str, schemas.Unset] = schemas.unset,
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SchemaForRequestBodyApplicationJson':
-        return super().__new__(
-            cls,
-            *_args,
-            name=name,
-            customerRefId=customerRefId,
-            _configuration=_configuration,
-            **kwargs,
+
+"""
+    Fireblocks API
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
+
+    The version of the OpenAPI document: 1.6.2
+    Contact: support@fireblocks.com
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
+import warnings
+from concurrent.futures import Future
+from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
+from typing import Any, Dict, List, Optional, Tuple, Union
+from typing_extensions import Annotated
+
+from pydantic import Field, StrictStr
+from typing import Optional
+from typing_extensions import Annotated
+from fireblocks.models.create_assets_bulk_request import CreateAssetsBulkRequest
+from fireblocks.models.job_created import JobCreated
+
+from fireblocks.api_client import ApiClient, RequestSerialized
+from fireblocks.api_response import ApiResponse
+from fireblocks.rest import RESTResponseType
+
+
+class AssetsApi:
+    """NOTE: This class is auto generated by OpenAPI Generator
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+    """
+
+    def __init__(self, api_client=None) -> None:
+        if api_client is None:
+            api_client = ApiClient.get_default()
+        self.api_client = api_client
+
+
+    @validate_call
+    def create_assets_bulk(
+        self,
+        create_assets_bulk_request: CreateAssetsBulkRequest,
+        idempotency_key: Annotated[Optional[StrictStr], Field(description="A unique identifier for the request. If the request is sent multiple times with the same idempotency key, the server will return the same response as the first request. The idempotency key is valid for 24 hours.")] = None,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> Future[ApiResponse[JobCreated]]:
+        """Bulk creation of wallets
+
+        Create multiple wallets for a given vault account by running an async job. </br> **Note**: - These endpoints are currently in beta and might be subject to changes. - We limit accounts to 10k per operation and 200k per customer during beta testing. - Currently, we are only supporting EVM wallets. 
+
+        :param create_assets_bulk_request: (required)
+        :type create_assets_bulk_request: CreateAssetsBulkRequest
+        :param idempotency_key: A unique identifier for the request. If the request is sent multiple times with the same idempotency key, the server will return the same response as the first request. The idempotency key is valid for 24 hours.
+        :type idempotency_key: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._create_assets_bulk_serialize(
+            create_assets_bulk_request=create_assets_bulk_request,
+            idempotency_key=idempotency_key,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
         )
 
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "JobCreated",
+            'default': "ErrorSchema",
+        }
+
+        return self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout,
+            _response_types_map=_response_types_map,
+        )
 
-request_body_any_type = api_client.RequestBody(
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaForRequestBodyApplicationJson),
-    },
-)
-XRequestIDSchema = schemas.StrSchema
-x_request_id_parameter = api_client.HeaderParameter(
-    name="X-Request-ID",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=XRequestIDSchema,
-)
-SchemaFor200ResponseBody = UnmanagedWallet
-ResponseHeadersFor200 = typing_extensions.TypedDict(
-    'ResponseHeadersFor200',
-    {
-        'X-Request-ID': XRequestIDSchema,
-    }
-)
-
-
-@dataclass
-class ApiResponseFor200(api_client.ApiResponse):
-    response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor200ResponseBody,
-    ]
-    headers: ResponseHeadersFor200
-
-
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
-    content={
-        '*/*': api_client.MediaType(
-            schema=SchemaFor200ResponseBody),
-    },
-    headers=[
-        x_request_id_parameter,
-    ]
-)
-XRequestIDSchema = schemas.StrSchema
-x_request_id_parameter = api_client.HeaderParameter(
-    name="X-Request-ID",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=XRequestIDSchema,
-)
-SchemaFor0ResponseBodyApplicationJson = Error
-ResponseHeadersFor0 = typing_extensions.TypedDict(
-    'ResponseHeadersFor0',
-    {
-        'X-Request-ID': XRequestIDSchema,
-    }
-)
-
-
-@dataclass
-class ApiResponseForDefault(api_client.ApiResponse):
-    response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor0ResponseBodyApplicationJson,
-    ]
-    headers: ResponseHeadersFor0
-
-
-_response_for_default = api_client.OpenApiResponse(
-    response_cls=ApiResponseForDefault,
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor0ResponseBodyApplicationJson),
-    },
-    headers=[
-        x_request_id_parameter,
-    ]
-)
-_status_code_to_response = {
-    '200': _response_for_200,
-    'default': _response_for_default,
-}
-_all_accept_content_types = (
-    '*/*',
-    'application/json',
-)
-
-
-class BaseApi(api_client.Api):
-
-    def _create_external_wallet_oapg(self, params: typing.Union[SchemaForRequestBodyApplicationJson,] = None, request_options: RequestOptions = None):
-        """
-        Create an external wallet
-        """
-        used_path = path.value
-        _headers = HTTPHeaderDict()
-        _fields = None
-        _body = None
-        serialized_data = request_body_any_type.serialize(params, "application/json")
-        _headers.add('Content-Type', "application/json")
-        if 'fields' in serialized_data:
-            _fields = serialized_data['fields']
-
-        elif 'body' in serialized_data:
-                _body = serialized_data['body']
-
-        if request_options and request_options.get("idempotency_key"):
-            idempotency_key = request_options.get("idempotency_key")
-            if idempotency_key:
-                _headers.add("Idempotency-Key", idempotency_key)
-
-        response = self.api_client.call_api(
-            resource_path=used_path,
-            method='post'.upper(),
-            headers=_headers,
-            fields=_fields,
-            body=_body,
-            timeout=10000,
+    def _create_assets_bulk_serialize(
+        self,
+        create_assets_bulk_request,
+        idempotency_key,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, Union[str, bytes]] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        # process the query parameters
+        # process the header parameters
+        if idempotency_key is not None:
+            _header_params['Idempotency-Key'] = idempotency_key
+        # process the form parameters
+        # process the body parameter
+        if create_assets_bulk_request is not None:
+            _body_params = create_assets_bulk_request
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
         )
 
-        response_for_status = _status_code_to_response.get(str(response.status))
-        if response_for_status:
-            api_response = response_for_status.deserialize(response, self.api_client.configuration)
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
         else:
-            default_response = _status_code_to_response.get('default')
-            if default_response:
-                api_response = default_response.deserialize(response, self.api_client.configuration)
-            else:
-                api_response = api_client.ApiResponseWithoutDeserialization(response=response)
-
-        if not 200 <= response.status <= 299:
-            raise exceptions.ApiException(
-                status=response.status,
-                reason=response.reason,
-                api_response=api_response
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json'
+                    ]
+                )
             )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
 
-        return api_response.body
-
-
-class CreateExternalWallet(BaseApi):
-    # this class is used by api classes that refer to endpoints with operationId fn names
-
-    def create_external_wallet(self , params: typing.Union[SchemaForRequestBodyApplicationJson,] = None, request_options: RequestOptions = None):
-        return self._create_external_wallet_oapg(params, request_options)
-
-
-class ApiForpost(BaseApi):
-    # this class is used by api classes that refer to endpoints by path and http method names
-
-    def post(self , params: typing.Union[SchemaForRequestBodyApplicationJson,] = None, request_options: RequestOptions = None):
-        return self._create_external_wallet_oapg(params, request_options)
+        # authentication setting
+        _auth_settings: List[str] = [
+        ]
+
+        return self.api_client.param_serialize(
+            method='POST',
+            resource_path='/vault/assets/bulk',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
```

### Comparing `fireblocks-0.0.1/fireblocks_client/paths/network_ids_network_id_set_routing_policy/patch.pyi` & `fireblocks-0.0.2b0/fireblocks/api/console_user_api.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,323 +1,310 @@
 # coding: utf-8
-from dataclasses import dataclass
-import typing_extensions
-from fireblocks_client.model.request_options import RequestOptions
-import urllib3
-from urllib3._collections import HTTPHeaderDict
-
-from fireblocks_client import api_client, exceptions
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
-
-import frozendict  # noqa: F401
-
-from fireblocks_client import schemas  # noqa: F401
-
-from fireblocks_client.model.network_id_routing_policy import NetworkIdRoutingPolicy
-from fireblocks_client.model.error import Error
-
-# Path params
-NetworkIdSchema = schemas.StrSchema
-RequestRequiredPathParams = typing_extensions.TypedDict(
-    'RequestRequiredPathParams',
-    {
-        'networkId': typing.Union[NetworkIdSchema, str, ],
-    }
-)
-RequestOptionalPathParams = typing_extensions.TypedDict(
-    'RequestOptionalPathParams',
-    {
-    },
-    total=False
-)
-
-
-class RequestPathParams(RequestRequiredPathParams, RequestOptionalPathParams):
-    pass
-
-
-request_path_network_id = api_client.PathParameter(
-    name="networkId",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=NetworkIdSchema,
-    required=True,
-)
-# body param
-
-
-class SchemaForRequestBodyApplicationJson(
-    schemas.AnyTypeSchema,
-):
-
-
-    class MetaOapg:
-        required = {
-            "routingPolicy",
+
+"""
+    Fireblocks API
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
+
+    The version of the OpenAPI document: 1.6.2
+    Contact: support@fireblocks.com
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
+import warnings
+from concurrent.futures import Future
+from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
+from typing import Any, Dict, List, Optional, Tuple, Union
+from typing_extensions import Annotated
+
+from pydantic import Field, StrictStr
+from typing import Optional
+from typing_extensions import Annotated
+from fireblocks.models.create_console_user import CreateConsoleUser
+from fireblocks.models.get_console_users_response import GetConsoleUsersResponse
+
+from fireblocks.api_client import ApiClient, RequestSerialized
+from fireblocks.api_response import ApiResponse
+from fireblocks.rest import RESTResponseType
+
+
+class ConsoleUserApi:
+    """NOTE: This class is auto generated by OpenAPI Generator
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+    """
+
+    def __init__(self, api_client=None) -> None:
+        if api_client is None:
+            api_client = ApiClient.get_default()
+        self.api_client = api_client
+
+
+    @validate_call
+    def create_console_user(
+        self,
+        idempotency_key: Annotated[Optional[StrictStr], Field(description="A unique identifier for the request. If the request is sent multiple times with the same idempotency key, the server will return the same response as the first request. The idempotency key is valid for 24 hours.")] = None,
+        create_console_user: Optional[CreateConsoleUser] = None,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> Future[ApiResponse[None]]:
+        """Create console user
+
+        Creates console user in your tenant
+
+        :param idempotency_key: A unique identifier for the request. If the request is sent multiple times with the same idempotency key, the server will return the same response as the first request. The idempotency key is valid for 24 hours.
+        :type idempotency_key: str
+        :param create_console_user:
+        :type create_console_user: CreateConsoleUser
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._create_console_user_serialize(
+            idempotency_key=idempotency_key,
+            create_console_user=create_console_user,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': None,
+            '400': None,
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
+            '5XX': "ErrorResponse",
+            'default': "ErrorSchema",
         }
-        
-        class properties:
-        
-            @staticmethod
-            def routingPolicy() -> typing.Type['NetworkIdRoutingPolicy']:
-                return NetworkIdRoutingPolicy
-            __annotations__ = {
-                "routingPolicy": routingPolicy,
-            }
-
-    
-    routingPolicy: 'NetworkIdRoutingPolicy'
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["routingPolicy"]) -> 'NetworkIdRoutingPolicy': ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["routingPolicy", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["routingPolicy"]) -> 'NetworkIdRoutingPolicy': ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["routingPolicy", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
-        routingPolicy: 'NetworkIdRoutingPolicy',
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SchemaForRequestBodyApplicationJson':
-        return super().__new__(
-            cls,
-            *_args,
-            routingPolicy=routingPolicy,
-            _configuration=_configuration,
-            **kwargs,
+
+        return self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout,
+            _response_types_map=_response_types_map,
         )
 
+    def _create_console_user_serialize(
+        self,
+        idempotency_key,
+        create_console_user,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
 
-request_body_any_type = api_client.RequestBody(
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaForRequestBodyApplicationJson),
-    },
-)
-XRequestIDSchema = schemas.StrSchema
-
-
-class SchemaFor200ResponseBody(
-    schemas.AnyTypeSchema,
-):
-
-
-    class MetaOapg:
-        required = {
-            "success",
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
         }
-        
-        class properties:
-            success = schemas.BoolSchema
-            __annotations__ = {
-                "success": success,
-            }
-
-    
-    success: MetaOapg.properties.success
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["success"]) -> MetaOapg.properties.success: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["success", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["success"]) -> MetaOapg.properties.success: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["success", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
-        success: typing.Union[MetaOapg.properties.success, bool, ],
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SchemaFor200ResponseBody':
-        return super().__new__(
-            cls,
-            *_args,
-            success=success,
-            _configuration=_configuration,
-            **kwargs,
-        )
-ResponseHeadersFor200 = typing_extensions.TypedDict(
-    'ResponseHeadersFor200',
-    {
-        'X-Request-ID': XRequestIDSchema,
-    }
-)
-
-
-@dataclass
-class ApiResponseFor200(api_client.ApiResponse):
-    response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor200ResponseBody,
-    ]
-    headers: ResponseHeadersFor200
-
-
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
-    content={
-        '*/*': api_client.MediaType(
-            schema=SchemaFor200ResponseBody),
-    },
-    headers=[
-        x_request_id_parameter,
-    ]
-)
-XRequestIDSchema = schemas.StrSchema
-SchemaFor0ResponseBodyApplicationJson = Error
-ResponseHeadersFor0 = typing_extensions.TypedDict(
-    'ResponseHeadersFor0',
-    {
-        'X-Request-ID': XRequestIDSchema,
-    }
-)
-
-
-@dataclass
-class ApiResponseForDefault(api_client.ApiResponse):
-    response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor0ResponseBodyApplicationJson,
-    ]
-    headers: ResponseHeadersFor0
-
-
-_response_for_default = api_client.OpenApiResponse(
-    response_cls=ApiResponseForDefault,
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor0ResponseBodyApplicationJson),
-    },
-    headers=[
-        x_request_id_parameter,
-    ]
-)
-_all_accept_content_types = (
-    '*/*',
-    'application/json',
-)
-
-
-class BaseApi(api_client.Api):
-
-    def _set_routing_policy_for_network_id_oapg(self, params: typing.Union[SchemaForRequestBodyApplicationJson, RequestPathParams] = None, request_options: RequestOptions = None):
-        """
-        Update network id routing policy.
-        """
-        path_params = {}
-        for parameter in (
-            request_path_network_id,
-        ):
-            if params and params.get(parameter.name):
-                path_params[parameter.name] = params.get(parameter.name)
-        self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
-        used_path = path.value
-
-        _path_params = {}
-        for parameter in (
-            request_path_network_id,
-        ):
-            parameter_data = path_params.get(parameter.name, schemas.unset)
-            if parameter_data is schemas.unset:
-                continue
-            serialized_data = parameter.serialize(parameter_data)
-            _path_params.update(serialized_data)
-
-        for k, v in _path_params.items():
-            used_path = used_path.replace('{%s}' % k, v)
-        _headers = HTTPHeaderDict()
-        _fields = None
-        _body = None
-        serialized_data = request_body_any_type.serialize(params, "application/json")
-        _headers.add('Content-Type', "application/json")
-        if 'fields' in serialized_data:
-            _fields = serialized_data['fields']
-
-        elif 'body' in serialized_data:
-                _body = serialized_data['body']
-
-        if request_options and request_options.get("idempotency_key"):
-            idempotency_key = request_options.get("idempotency_key")
-            if idempotency_key:
-                _headers.add("Idempotency-Key", idempotency_key)
-
-        response = self.api_client.call_api(
-            resource_path=used_path,
-            method='patch'.upper(),
-            headers=_headers,
-            fields=_fields,
-            body=_body,
-            timeout=10000,
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, Union[str, bytes]] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        # process the query parameters
+        # process the header parameters
+        if idempotency_key is not None:
+            _header_params['Idempotency-Key'] = idempotency_key
+        # process the form parameters
+        # process the body parameter
+        if create_console_user is not None:
+            _body_params = create_console_user
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
         )
 
-        response_for_status = _status_code_to_response.get(str(response.status))
-        if response_for_status:
-            api_response = response_for_status.deserialize(response, self.api_client.configuration)
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
         else:
-            default_response = _status_code_to_response.get('default')
-            if default_response:
-                api_response = default_response.deserialize(response, self.api_client.configuration)
-            else:
-                api_response = api_client.ApiResponseWithoutDeserialization(response=response)
-
-        if not 200 <= response.status <= 299:
-            raise exceptions.ApiException(
-                status=response.status,
-                reason=response.reason,
-                api_response=api_response
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json'
+                    ]
+                )
             )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
+
+        # authentication setting
+        _auth_settings: List[str] = [
+        ]
+
+        return self.api_client.param_serialize(
+            method='POST',
+            resource_path='/management/users',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
 
-        return api_response.body
 
 
-class SetRoutingPolicyForNetworkId(BaseApi):
-    # this class is used by api classes that refer to endpoints with operationId fn names
 
-    def set_routing_policy_for_network_id(self , params: typing.Union[SchemaForRequestBodyApplicationJson, RequestPathParams] = None, request_options: RequestOptions = None):
-        return self._set_routing_policy_for_network_id_oapg(params, request_options)
+    @validate_call
+    def get_console_users(
+        self,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> Future[ApiResponse[GetConsoleUsersResponse]]:
+        """Get console users
+
+        Get console users for your tenant
+
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._get_console_users_serialize(
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "GetConsoleUsersResponse",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
+            '5XX': "ErrorResponse",
+            'default': "ErrorSchema",
+        }
 
+        return self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout,
+            _response_types_map=_response_types_map,
+        )
+
+    def _get_console_users_serialize(
+        self,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
 
-class ApiForpatch(BaseApi):
-    # this class is used by api classes that refer to endpoints by path and http method names
+        _host = None
 
-    def patch(self , params: typing.Union[SchemaForRequestBodyApplicationJson, RequestPathParams] = None, request_options: RequestOptions = None):
-        return self._set_routing_policy_for_network_id_oapg(params, request_options)
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, Union[str, bytes]] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+
+        # authentication setting
+        _auth_settings: List[str] = [
+        ]
+
+        return self.api_client.param_serialize(
+            method='GET',
+            resource_path='/management/users',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
```

### Comparing `fireblocks-0.0.1/fireblocks_client/paths/nfts_ownership_collections/get.py` & `fireblocks-0.0.2b0/fireblocks/api/webhooks_api.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,369 +1,318 @@
 # coding: utf-8
-from dataclasses import dataclass
-import typing_extensions
-from fireblocks_client.model.request_options import RequestOptions
-import urllib3
-from urllib3._collections import HTTPHeaderDict
-
-from fireblocks_client import api_client, exceptions
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
-
-import frozendict  # noqa: F401
-
-from fireblocks_client import schemas  # noqa: F401
-
-from fireblocks_client.model.paging import Paging
-from fireblocks_client.model.collection_ownership_response import CollectionOwnershipResponse
-
-from . import path
-
-# Query params
-
-
-class SearchSchema(
-    schemas.StrSchema
-):
-
-
-    class MetaOapg:
-PageCursorSchema = schemas.StrSchema
-
-
-class PageSizeSchema(
-    schemas.NumberSchema
-):
-
-
-    class MetaOapg:
-        inclusive_maximum = 100
-        inclusive_minimum = 1
-
-
-class SortSchema(
-    schemas.ListSchema
-):
-
-
-    class MetaOapg:
-        
-        
-        class items(
-            schemas.EnumBase,
-            schemas.StrSchema
-        ):
-        
-        
-            class MetaOapg:
-                enum_value_to_name = {
-                    "name": "NAME",
-                }
-            
-            @schemas.classproperty
-            def NAME(cls):
-                return cls("name")
-
-    def __new__(
-        cls,
-        _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
-        _configuration: typing.Optional[schemas.Configuration] = None,
-    ) -> 'SortSchema':
-        return super().__new__(
-            cls,
-            _arg,
-            _configuration=_configuration,
+
+"""
+    Fireblocks API
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
+
+    The version of the OpenAPI document: 1.6.2
+    Contact: support@fireblocks.com
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
+import warnings
+from concurrent.futures import Future
+from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
+from typing import Any, Dict, List, Optional, Tuple, Union
+from typing_extensions import Annotated
+
+from pydantic import Field, StrictStr
+from typing import Optional
+from typing_extensions import Annotated
+from fireblocks.models.resend_transaction_webhooks_request import ResendTransactionWebhooksRequest
+from fireblocks.models.resend_webhooks_by_transaction_id_response import ResendWebhooksByTransactionIdResponse
+from fireblocks.models.resend_webhooks_response import ResendWebhooksResponse
+
+from fireblocks.api_client import ApiClient, RequestSerialized
+from fireblocks.api_response import ApiResponse
+from fireblocks.rest import RESTResponseType
+
+
+class WebhooksApi:
+    """NOTE: This class is auto generated by OpenAPI Generator
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+    """
+
+    def __init__(self, api_client=None) -> None:
+        if api_client is None:
+            api_client = ApiClient.get_default()
+        self.api_client = api_client
+
+
+    @validate_call
+    def resend_transaction_webhooks(
+        self,
+        tx_id: Annotated[StrictStr, Field(description="The ID of the transaction for webhooks")],
+        resend_transaction_webhooks_request: ResendTransactionWebhooksRequest,
+        idempotency_key: Annotated[Optional[StrictStr], Field(description="A unique identifier for the request. If the request is sent multiple times with the same idempotency key, the server will return the same response as the first request. The idempotency key is valid for 24 hours.")] = None,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> Future[ApiResponse[ResendWebhooksByTransactionIdResponse]]:
+        """Resend failed webhooks for a transaction by ID
+
+        Resends failed webhook notifications for a transaction by ID.
+
+        :param tx_id: The ID of the transaction for webhooks (required)
+        :type tx_id: str
+        :param resend_transaction_webhooks_request: (required)
+        :type resend_transaction_webhooks_request: ResendTransactionWebhooksRequest
+        :param idempotency_key: A unique identifier for the request. If the request is sent multiple times with the same idempotency key, the server will return the same response as the first request. The idempotency key is valid for 24 hours.
+        :type idempotency_key: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._resend_transaction_webhooks_serialize(
+            tx_id=tx_id,
+            resend_transaction_webhooks_request=resend_transaction_webhooks_request,
+            idempotency_key=idempotency_key,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
         )
 
-    def __getitem__(self, i: int) -> MetaOapg.items:
-        return super().__getitem__(i)
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "ResendWebhooksByTransactionIdResponse",
+            'default': "ErrorSchema",
+        }
 
+        return self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout,
+            _response_types_map=_response_types_map,
+        )
 
-class OrderSchema(
-    schemas.EnumBase,
-    schemas.StrSchema
-):
+    def _resend_transaction_webhooks_serialize(
+        self,
+        tx_id,
+        resend_transaction_webhooks_request,
+        idempotency_key,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
 
+        _host = None
 
-    class MetaOapg:
-        enum_value_to_name = {
-            "DESC": "DESC",
-            "ASC": "ASC",
+        _collection_formats: Dict[str, str] = {
         }
-    
-    @schemas.classproperty
-    def DESC(cls):
-        return cls("DESC")
-    
-    @schemas.classproperty
-    def ASC(cls):
-        return cls("ASC")
-RequestRequiredQueryParams = typing_extensions.TypedDict(
-    'RequestRequiredQueryParams',
-    {
-    }
-)
-RequestOptionalQueryParams = typing_extensions.TypedDict(
-    'RequestOptionalQueryParams',
-    {
-        'search': typing.Union[SearchSchema, str, ],
-        'pageCursor': typing.Union[PageCursorSchema, str, ],
-        'pageSize': typing.Union[PageSizeSchema, decimal.Decimal, int, float, ],
-        'sort': typing.Union[SortSchema, list, tuple, ],
-        'order': typing.Union[OrderSchema, str, ],
-    },
-    total=False
-)
-
-
-class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
-    pass
-
-
-request_query_search = api_client.QueryParameter(
-    name="search",
-    style=api_client.ParameterStyle.FORM,
-    schema=SearchSchema,
-    explode=True,
-)
-request_query_page_cursor = api_client.QueryParameter(
-    name="pageCursor",
-    style=api_client.ParameterStyle.FORM,
-    schema=PageCursorSchema,
-    explode=True,
-)
-request_query_page_size = api_client.QueryParameter(
-    name="pageSize",
-    style=api_client.ParameterStyle.FORM,
-    schema=PageSizeSchema,
-    explode=True,
-)
-request_query_sort = api_client.QueryParameter(
-    name="sort",
-    style=api_client.ParameterStyle.FORM,
-    schema=SortSchema,
-    explode=True,
-)
-request_query_order = api_client.QueryParameter(
-    name="order",
-    style=api_client.ParameterStyle.FORM,
-    schema=OrderSchema,
-    explode=True,
-)
-XRequestIDSchema = schemas.StrSchema
-x_request_id_parameter = api_client.HeaderParameter(
-    name="X-Request-ID",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=XRequestIDSchema,
-)
-
-
-class SchemaFor200ResponseBodyApplicationJson(
-    schemas.AnyTypeSchema,
-):
-
-
-    class MetaOapg:
-        
-        class properties:
-        
-            @staticmethod
-            def paging() -> typing.Type['Paging']:
-                return Paging
-            
-            
-            class data(
-                schemas.ListSchema
-            ):
-            
-            
-                class MetaOapg:
-                    
-                    @staticmethod
-                    def items() -> typing.Type['CollectionOwnershipResponse']:
-                        return CollectionOwnershipResponse
-            
-                def __new__(
-                    cls,
-                    _arg: typing.Union[typing.Tuple['CollectionOwnershipResponse'], typing.List['CollectionOwnershipResponse']],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'data':
-                    return super().__new__(
-                        cls,
-                        _arg,
-                        _configuration=_configuration,
-                    )
-            
-                def __getitem__(self, i: int) -> 'CollectionOwnershipResponse':
-                    return super().__getitem__(i)
-            __annotations__ = {
-                "paging": paging,
-                "data": data,
-            }
-
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["paging"]) -> 'Paging': ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["data"]) -> MetaOapg.properties.data: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["paging", "data", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["paging"]) -> typing.Union['Paging', schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["data"]) -> typing.Union[MetaOapg.properties.data, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["paging", "data", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
-        paging: typing.Union['Paging', schemas.Unset] = schemas.unset,
-        data: typing.Union[MetaOapg.properties.data, list, tuple, schemas.Unset] = schemas.unset,
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SchemaFor200ResponseBodyApplicationJson':
-        return super().__new__(
-            cls,
-            *_args,
-            paging=paging,
-            data=data,
-            _configuration=_configuration,
-            **kwargs,
-        )
-ResponseHeadersFor200 = typing_extensions.TypedDict(
-    'ResponseHeadersFor200',
-    {
-        'X-Request-ID': XRequestIDSchema,
-    }
-)
-
-
-@dataclass
-class ApiResponseFor200(api_client.ApiResponse):
-    response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
-    ]
-    headers: ResponseHeadersFor200
-
-
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
-    },
-    headers=[
-        x_request_id_parameter,
-    ]
-)
-_status_code_to_response = {
-    '200': _response_for_200,
-}
-_all_accept_content_types = (
-    'application/json',
-)
-
-
-class BaseApi(api_client.Api):
-
-    def _list_owned_collections_oapg(self, params: typing.Union[ RequestQueryParams,] = None, request_options: RequestOptions = None):
-        """
-        List owned collections (paginated)
-        """
-        query_params = {}
-        if params and params.get("search"):
-            query_params["search"] = params.get("search")
-        if params and params.get("page_cursor"):
-            query_params["page_cursor"] = params.get("page_cursor")
-        if params and params.get("page_size"):
-            query_params["page_size"] = params.get("page_size")
-        if params and params.get("sort"):
-            query_params["sort"] = params.get("sort")
-        if params and params.get("order"):
-            query_params["order"] = params.get("order")
-        self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
-        used_path = path.value
-
-        prefix_separator_iterator = None
-        for parameter in (
-            request_query_search,
-            request_query_page_cursor,
-            request_query_page_size,
-            request_query_sort,
-            request_query_order,
-        ):
-            parameter_data = query_params.get(parameter.name, schemas.unset)
-            if parameter_data is schemas.unset:
-                continue
-            if prefix_separator_iterator is None:
-                prefix_separator_iterator = parameter.get_prefix_separator_iterator()
-            serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
-            for serialized_value in serialized_data.values():
-                used_path += serialized_value
-        _headers = HTTPHeaderDict()
-        _fields = None
-        _body = None
-
-        if request_options and request_options.get("idempotency_key"):
-            idempotency_key = request_options.get("idempotency_key")
-            if idempotency_key:
-                _headers.add("Idempotency-Key", idempotency_key)
-
-        response = self.api_client.call_api(
-            resource_path=used_path,
-            method='get'.upper(),
-            headers=_headers,
-            timeout=10000,
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, Union[str, bytes]] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        if tx_id is not None:
+            _path_params['txId'] = tx_id
+        # process the query parameters
+        # process the header parameters
+        if idempotency_key is not None:
+            _header_params['Idempotency-Key'] = idempotency_key
+        # process the form parameters
+        # process the body parameter
+        if resend_transaction_webhooks_request is not None:
+            _body_params = resend_transaction_webhooks_request
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
         )
 
-        response_for_status = _status_code_to_response.get(str(response.status))
-        if response_for_status:
-            api_response = response_for_status.deserialize(response, self.api_client.configuration)
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
         else:
-            api_response = api_client.ApiResponseWithoutDeserialization(response=response)
-
-        if not 200 <= response.status <= 299:
-            raise exceptions.ApiException(
-                status=response.status,
-                reason=response.reason,
-                api_response=api_response
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json'
+                    ]
+                )
             )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
 
-        return api_response.body
+        # authentication setting
+        _auth_settings: List[str] = [
+        ]
+
+        return self.api_client.param_serialize(
+            method='POST',
+            resource_path='/webhooks/resend/{txId}',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
 
 
-class ListOwnedCollections(BaseApi):
-    # this class is used by api classes that refer to endpoints with operationId fn names
 
-    def list_owned_collections(self , params: typing.Union[ RequestQueryParams,] = None, request_options: RequestOptions = None):
-        return self._list_owned_collections_oapg(params, request_options)
 
+    @validate_call
+    def resend_webhooks(
+        self,
+        idempotency_key: Annotated[Optional[StrictStr], Field(description="A unique identifier for the request. If the request is sent multiple times with the same idempotency key, the server will return the same response as the first request. The idempotency key is valid for 24 hours.")] = None,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> Future[ApiResponse[ResendWebhooksResponse]]:
+        """Resend failed webhooks
+
+        Resends all failed webhook notifications.
+
+        :param idempotency_key: A unique identifier for the request. If the request is sent multiple times with the same idempotency key, the server will return the same response as the first request. The idempotency key is valid for 24 hours.
+        :type idempotency_key: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._resend_webhooks_serialize(
+            idempotency_key=idempotency_key,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
 
-class ApiForget(BaseApi):
-    # this class is used by api classes that refer to endpoints by path and http method names
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "ResendWebhooksResponse",
+            'default': "ErrorSchema",
+        }
 
-    def get(self , params: typing.Union[ RequestQueryParams,] = None, request_options: RequestOptions = None):
-        return self._list_owned_collections_oapg(params, request_options)
+        return self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout,
+            _response_types_map=_response_types_map,
+        )
+
+    def _resend_webhooks_serialize(
+        self,
+        idempotency_key,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, Union[str, bytes]] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        # process the query parameters
+        # process the header parameters
+        if idempotency_key is not None:
+            _header_params['Idempotency-Key'] = idempotency_key
+        # process the form parameters
+        # process the body parameter
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+
+        # authentication setting
+        _auth_settings: List[str] = [
+        ]
+
+        return self.api_client.param_serialize(
+            method='POST',
+            resource_path='/webhooks/resend',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
```

### Comparing `fireblocks-0.0.1/fireblocks_client/paths/tap_draft/get.pyi` & `fireblocks-0.0.2b0/test/test_payout_response.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,145 +1,106 @@
 # coding: utf-8
-from dataclasses import dataclass
-import typing_extensions
-from fireblocks_client.model.request_options import RequestOptions
-import urllib3
-from urllib3._collections import HTTPHeaderDict
-
-from fireblocks_client import api_client, exceptions
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
-
-import frozendict  # noqa: F401
-
-from fireblocks_client import schemas  # noqa: F401
-
-from fireblocks_client.model.draft_review_and_validation_response import DraftReviewAndValidationResponse
-from fireblocks_client.model.error import Error
-
-XRequestIDSchema = schemas.StrSchema
-SchemaFor200ResponseBody = DraftReviewAndValidationResponse
-ResponseHeadersFor200 = typing_extensions.TypedDict(
-    'ResponseHeadersFor200',
-    {
-        'X-Request-ID': XRequestIDSchema,
-    }
-)
-
-
-@dataclass
-class ApiResponseFor200(api_client.ApiResponse):
-    response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor200ResponseBody,
-    ]
-    headers: ResponseHeadersFor200
-
-
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
-    content={
-        '*/*': api_client.MediaType(
-            schema=SchemaFor200ResponseBody),
-    },
-    headers=[
-        x_request_id_parameter,
-    ]
-)
-XRequestIDSchema = schemas.StrSchema
-SchemaFor0ResponseBodyApplicationJson = Error
-ResponseHeadersFor0 = typing_extensions.TypedDict(
-    'ResponseHeadersFor0',
-    {
-        'X-Request-ID': XRequestIDSchema,
-    }
-)
-
-
-@dataclass
-class ApiResponseForDefault(api_client.ApiResponse):
-    response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor0ResponseBodyApplicationJson,
-    ]
-    headers: ResponseHeadersFor0
-
-
-_response_for_default = api_client.OpenApiResponse(
-    response_cls=ApiResponseForDefault,
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor0ResponseBodyApplicationJson),
-    },
-    headers=[
-        x_request_id_parameter,
-    ]
-)
-_all_accept_content_types = (
-    '*/*',
-    'application/json',
-)
 
+"""
+    Fireblocks API
 
-class BaseApi(api_client.Api):
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    def _get_draft_oapg(self, request_options: RequestOptions = None):
-        """
-        Get the active draft
-        """
-        used_path = path.value
-        _headers = HTTPHeaderDict()
-        _fields = None
-        _body = None
-
-        if request_options and request_options.get("idempotency_key"):
-            idempotency_key = request_options.get("idempotency_key")
-            if idempotency_key:
-                _headers.add("Idempotency-Key", idempotency_key)
-
-        response = self.api_client.call_api(
-            resource_path=used_path,
-            method='get'.upper(),
-            headers=_headers,
-            timeout=10000,
-        )
+    The version of the OpenAPI document: 1.6.2
+    Contact: support@fireblocks.com
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
 
-        response_for_status = _status_code_to_response.get(str(response.status))
-        if response_for_status:
-            api_response = response_for_status.deserialize(response, self.api_client.configuration)
-        else:
-            default_response = _status_code_to_response.get('default')
-            if default_response:
-                api_response = default_response.deserialize(response, self.api_client.configuration)
-            else:
-                api_response = api_client.ApiResponseWithoutDeserialization(response=response)
-
-        if not 200 <= response.status <= 299:
-            raise exceptions.ApiException(
-                status=response.status,
-                reason=response.reason,
-                api_response=api_response
-            )
 
-        return api_response.body
+import unittest
 
+from fireblocks.models.payout_response import PayoutResponse
 
-class GetDraft(BaseApi):
-    # this class is used by api classes that refer to endpoints with operationId fn names
 
-    def get_draft(self , request_options: RequestOptions = None):
-        return self._get_draft_oapg(request_options)
+class TestPayoutResponse(unittest.TestCase):
+    """PayoutResponse unit test stubs"""
 
+    def setUp(self):
+        pass
 
-class ApiForget(BaseApi):
-    # this class is used by api classes that refer to endpoints by path and http method names
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional) -> PayoutResponse:
+        """Test PayoutResponse
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # uncomment below to create an instance of `PayoutResponse`
+        """
+        model = PayoutResponse()
+        if include_optional:
+            return PayoutResponse(
+                payout_id = '',
+                payment_account = fireblocks.models.payment_account_response.PaymentAccountResponse(
+                    id = '', 
+                    type = 'VAULT_ACCOUNT', ),
+                created_at = 1.337,
+                state = 'CREATED',
+                status = 'REGISTERED',
+                reason_of_failure = '',
+                init_method = 'FILE',
+                instruction_set = [
+                    fireblocks.models.payout_instruction_response.PayoutInstructionResponse(
+                        id = '', 
+                        payee_account = fireblocks.models.payee_account_response.PayeeAccountResponse(
+                            id = '', 
+                            type = 'VAULT_ACCOUNT', ), 
+                        amount = fireblocks.models.instruction_amount.InstructionAmount(
+                            amount = '', 
+                            asset_id = '', ), 
+                        state = 'NOT_STARTED', 
+                        transactions = [
+                            fireblocks.models.transaction.Transaction(
+                                id = '', 
+                                state = 'SUBMITTED', 
+                                timestamp = 1.337, 
+                                instruction_id = '', )
+                            ], )
+                    ],
+                report_url = ''
+            )
+        else:
+            return PayoutResponse(
+                payout_id = '',
+                payment_account = fireblocks.models.payment_account_response.PaymentAccountResponse(
+                    id = '', 
+                    type = 'VAULT_ACCOUNT', ),
+                created_at = 1.337,
+                state = 'CREATED',
+                status = 'REGISTERED',
+                instruction_set = [
+                    fireblocks.models.payout_instruction_response.PayoutInstructionResponse(
+                        id = '', 
+                        payee_account = fireblocks.models.payee_account_response.PayeeAccountResponse(
+                            id = '', 
+                            type = 'VAULT_ACCOUNT', ), 
+                        amount = fireblocks.models.instruction_amount.InstructionAmount(
+                            amount = '', 
+                            asset_id = '', ), 
+                        state = 'NOT_STARTED', 
+                        transactions = [
+                            fireblocks.models.transaction.Transaction(
+                                id = '', 
+                                state = 'SUBMITTED', 
+                                timestamp = 1.337, 
+                                instruction_id = '', )
+                            ], )
+                    ],
+        )
+        """
 
-    def get(self , request_options: RequestOptions = None):
-        return self._get_draft_oapg(request_options)
+    def testPayoutResponse(self):
+        """Test PayoutResponse"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `fireblocks-0.0.1/fireblocks_client/paths/vault_asset_wallets/get.pyi` & `fireblocks-0.0.2b0/fireblocks/api/whitelist_ip_addresses_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,202 +1,167 @@
 # coding: utf-8
-from dataclasses import dataclass
-import typing_extensions
-from fireblocks_client.model.request_options import RequestOptions
-import urllib3
-from urllib3._collections import HTTPHeaderDict
-
-from fireblocks_client import api_client, exceptions
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
-
-import frozendict  # noqa: F401
-
-from fireblocks_client import schemas  # noqa: F401
-
-from fireblocks_client.model.paginated_asset_wallet_response import PaginatedAssetWalletResponse
-
-# Query params
-TotalAmountLargerThanSchema = schemas.NumberSchema
-AssetIdSchema = schemas.StrSchema
-BeforeSchema = schemas.StrSchema
-AfterSchema = schemas.StrSchema
-
-
-class LimitSchema(
-    schemas.NumberSchema
-):
-    pass
-RequestRequiredQueryParams = typing_extensions.TypedDict(
-    'RequestRequiredQueryParams',
-    {
-    }
-)
-RequestOptionalQueryParams = typing_extensions.TypedDict(
-    'RequestOptionalQueryParams',
-    {
-        'totalAmountLargerThan': typing.Union[TotalAmountLargerThanSchema, decimal.Decimal, int, float, ],
-        'assetId': typing.Union[AssetIdSchema, str, ],
-        'before': typing.Union[BeforeSchema, str, ],
-        'after': typing.Union[AfterSchema, str, ],
-        'limit': typing.Union[LimitSchema, decimal.Decimal, int, float, ],
-    },
-    total=False
-)
-
-
-class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
-    pass
-
-
-request_query_total_amount_larger_than = api_client.QueryParameter(
-    name="totalAmountLargerThan",
-    style=api_client.ParameterStyle.FORM,
-    schema=TotalAmountLargerThanSchema,
-    explode=True,
-)
-request_query_asset_id = api_client.QueryParameter(
-    name="assetId",
-    style=api_client.ParameterStyle.FORM,
-    schema=AssetIdSchema,
-    explode=True,
-)
-request_query_before = api_client.QueryParameter(
-    name="before",
-    style=api_client.ParameterStyle.FORM,
-    schema=BeforeSchema,
-    explode=True,
-)
-request_query_after = api_client.QueryParameter(
-    name="after",
-    style=api_client.ParameterStyle.FORM,
-    schema=AfterSchema,
-    explode=True,
-)
-request_query_limit = api_client.QueryParameter(
-    name="limit",
-    style=api_client.ParameterStyle.FORM,
-    schema=LimitSchema,
-    explode=True,
-)
-XRequestIDSchema = schemas.StrSchema
-SchemaFor200ResponseBody = PaginatedAssetWalletResponse
-ResponseHeadersFor200 = typing_extensions.TypedDict(
-    'ResponseHeadersFor200',
-    {
-        'X-Request-ID': XRequestIDSchema,
-    }
-)
-
-
-@dataclass
-class ApiResponseFor200(api_client.ApiResponse):
-    response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor200ResponseBody,
-    ]
-    headers: ResponseHeadersFor200
-
-
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
-    content={
-        '*/*': api_client.MediaType(
-            schema=SchemaFor200ResponseBody),
-    },
-    headers=[
-        x_request_id_parameter,
-    ]
-)
-_all_accept_content_types = (
-    '*/*',
-)
-
-
-class BaseApi(api_client.Api):
-
-    def _get_asset_wallets_oapg(self, params: typing.Union[ RequestQueryParams,] = None, request_options: RequestOptions = None):
-        """
-        List asset wallets (Paginated)
-        """
-        query_params = {}
-        if params and params.get("total_amount_larger_than"):
-            query_params["total_amount_larger_than"] = params.get("total_amount_larger_than")
-        if params and params.get("asset_id"):
-            query_params["asset_id"] = params.get("asset_id")
-        if params and params.get("before"):
-            query_params["before"] = params.get("before")
-        if params and params.get("after"):
-            query_params["after"] = params.get("after")
-        if params and params.get("limit"):
-            query_params["limit"] = params.get("limit")
-        self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
-        used_path = path.value
-
-        prefix_separator_iterator = None
-        for parameter in (
-            request_query_total_amount_larger_than,
-            request_query_asset_id,
-            request_query_before,
-            request_query_after,
-            request_query_limit,
-        ):
-            parameter_data = query_params.get(parameter.name, schemas.unset)
-            if parameter_data is schemas.unset:
-                continue
-            if prefix_separator_iterator is None:
-                prefix_separator_iterator = parameter.get_prefix_separator_iterator()
-            serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
-            for serialized_value in serialized_data.values():
-                used_path += serialized_value
-        _headers = HTTPHeaderDict()
-        _fields = None
-        _body = None
-
-        if request_options and request_options.get("idempotency_key"):
-            idempotency_key = request_options.get("idempotency_key")
-            if idempotency_key:
-                _headers.add("Idempotency-Key", idempotency_key)
-
-        response = self.api_client.call_api(
-            resource_path=used_path,
-            method='get'.upper(),
-            headers=_headers,
-            timeout=10000,
-        )
-
-        response_for_status = _status_code_to_response.get(str(response.status))
-        if response_for_status:
-            api_response = response_for_status.deserialize(response, self.api_client.configuration)
-        else:
-            api_response = api_client.ApiResponseWithoutDeserialization(response=response)
 
-        if not 200 <= response.status <= 299:
-            raise exceptions.ApiException(
-                status=response.status,
-                reason=response.reason,
-                api_response=api_response
-            )
+"""
+    Fireblocks API
 
-        return api_response.body
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
+    The version of the OpenAPI document: 1.6.2
+    Contact: support@fireblocks.com
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
+import warnings
+from concurrent.futures import Future
+from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
+from typing import Any, Dict, List, Optional, Tuple, Union
+from typing_extensions import Annotated
+
+from pydantic import Field, StrictStr
+from typing_extensions import Annotated
+from fireblocks.models.get_whitelist_ip_addresses_response import GetWhitelistIpAddressesResponse
+
+from fireblocks.api_client import ApiClient, RequestSerialized
+from fireblocks.api_response import ApiResponse
+from fireblocks.rest import RESTResponseType
+
+
+class WhitelistIpAddressesApi:
+    """NOTE: This class is auto generated by OpenAPI Generator
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+    """
+
+    def __init__(self, api_client=None) -> None:
+        if api_client is None:
+            api_client = ApiClient.get_default()
+        self.api_client = api_client
+
+
+    @validate_call
+    def get_whitelist_ip_addresses(
+        self,
+        user_id: Annotated[StrictStr, Field(description="The ID of the api user")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> Future[ApiResponse[GetWhitelistIpAddressesResponse]]:
+        """Gets whitelisted ip addresses
+
+        Gets whitelisted ip addresses for given Api user.
+
+        :param user_id: The ID of the api user (required)
+        :type user_id: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._get_whitelist_ip_addresses_serialize(
+            user_id=user_id,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
 
-class GetAssetWallets(BaseApi):
-    # this class is used by api classes that refer to endpoints with operationId fn names
-
-    def get_asset_wallets(self , params: typing.Union[ RequestQueryParams,] = None, request_options: RequestOptions = None):
-        return self._get_asset_wallets_oapg(params, request_options)
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "GetWhitelistIpAddressesResponse",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
+            '5XX': "ErrorResponse",
+            'default': "ErrorSchema",
+        }
+
+        return self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout,
+            _response_types_map=_response_types_map,
+        )
 
+    def _get_whitelist_ip_addresses_serialize(
+        self,
+        user_id,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, Union[str, bytes]] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        if user_id is not None:
+            _path_params['userId'] = user_id
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
 
-class ApiForget(BaseApi):
-    # this class is used by api classes that refer to endpoints by path and http method names
 
-    def get(self , params: typing.Union[ RequestQueryParams,] = None, request_options: RequestOptions = None):
-        return self._get_asset_wallets_oapg(params, request_options)
+        # authentication setting
+        _auth_settings: List[str] = [
+        ]
+
+        return self.api_client.param_serialize(
+            method='GET',
+            resource_path='/management/api_users/{userId}/whitelist_ip_addresses',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
```

### Comparing `fireblocks-0.0.1/fireblocks_client/rest.py` & `fireblocks-0.0.2b0/fireblocks/rest.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,268 +1,245 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
-import logging
+import io
+import json
+import re
 import ssl
-from urllib.parse import urlencode
-import typing
 
-import certifi
 import urllib3
-from urllib3._collections import HTTPHeaderDict
 
-from fireblocks_client.exceptions import ApiException, ApiValueError
+from fireblocks.exceptions import ApiException, ApiValueError
+
+SUPPORTED_SOCKS_PROXIES = {"socks5", "socks5h", "socks4", "socks4a"}
+RESTResponseType = urllib3.HTTPResponse
+
+
+def is_socks_proxy_url(url):
+    if url is None:
+        return False
+    split_section = url.split("://")
+    if len(split_section) < 2:
+        return False
+    else:
+        return split_section[0].lower() in SUPPORTED_SOCKS_PROXIES
+
+
+class RESTResponse(io.IOBase):
+
+    def __init__(self, resp) -> None:
+        self.response = resp
+        self.status = resp.status
+        self.reason = resp.reason
+        self.data = None
 
-urllib3.disable_warnings()
-logger = logging.getLogger(__name__)
+    def read(self):
+        if self.data is None:
+            self.data = self.response.data
+        return self.data
 
+    def getheaders(self):
+        """Returns a dictionary of the response headers."""
+        return self.response.headers
 
-class RESTClientObject(object):
-    def __init__(self, configuration, pools_size=4, maxsize=None):
-        cert_reqs = ssl.CERT_NONE
-        ca_certs = certifi.where()
+    def getheader(self, name, default=None):
+        """Returns a given response header."""
+        return self.response.headers.get(name, default)
 
-        addition_pool_args = {}
 
-        if configuration.options and configuration.options.retries is not None:
-            addition_pool_args["retries"] = configuration.retries
+class RESTClientObject:
+
+    def __init__(self, configuration) -> None:
+        # urllib3.PoolManager will pass all kw parameters to connectionpool
+        # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/poolmanager.py#L75  # noqa: E501
+        # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/connectionpool.py#L680  # noqa: E501
+        # Custom SSL certificates and client certificates: http://urllib3.readthedocs.io/en/latest/advanced-usage.html  # noqa: E501
+
+        # cert_reqs
+        if configuration.verify_ssl:
+            cert_reqs = ssl.CERT_REQUIRED
+        else:
+            cert_reqs = ssl.CERT_NONE
+
+        pool_args = {
+            "cert_reqs": cert_reqs,
+            "ca_certs": configuration.ssl_ca_cert,
+            "cert_file": configuration.cert_file,
+            "key_file": configuration.key_file,
+        }
+        if configuration.assert_hostname is not None:
+            pool_args["assert_hostname"] = configuration.assert_hostname
+
+        if configuration.retries is not None:
+            pool_args["retries"] = configuration.retries
+
+        if configuration.tls_server_name:
+            pool_args["server_hostname"] = configuration.tls_server_name
 
         if configuration.socket_options is not None:
-            addition_pool_args["socket_options"] = configuration.socket_options
+            pool_args["socket_options"] = configuration.socket_options
 
-        if maxsize is None:
-            if configuration.connection_pool_maxsize is not None:
-                maxsize = configuration.connection_pool_maxsize
-            else:
-                maxsize = 4
+        if configuration.connection_pool_maxsize is not None:
+            pool_args["maxsize"] = configuration.connection_pool_maxsize
 
         # https pool manager
+        self.pool_manager: urllib3.PoolManager
+
         if configuration.proxy:
-            self.pool_manager = urllib3.ProxyManager(
-                num_pools=pools_size,
-                maxsize=maxsize,
-                cert_reqs=cert_reqs,
-                ca_certs=ca_certs,
-                cert_file=None,
-                key_file=None,
-                proxy_url=configuration.proxy,
-                proxy_headers=configuration.proxy_headers,
-                **addition_pool_args
-            )
+            if is_socks_proxy_url(configuration.proxy):
+                from urllib3.contrib.socks import SOCKSProxyManager
+
+                pool_args["proxy_url"] = configuration.proxy
+                pool_args["headers"] = configuration.proxy_headers
+                self.pool_manager = SOCKSProxyManager(**pool_args)
+            else:
+                pool_args["proxy_url"] = configuration.proxy
+                pool_args["proxy_headers"] = configuration.proxy_headers
+                self.pool_manager = urllib3.ProxyManager(**pool_args)
         else:
-            self.pool_manager = urllib3.PoolManager(
-                num_pools=pools_size,
-                maxsize=maxsize,
-                cert_reqs=cert_reqs,
-                ca_certs=ca_certs,
-                cert_file=None,
-                key_file=None,
-                **addition_pool_args
-            )
+            self.pool_manager = urllib3.PoolManager(**pool_args)
 
     def request(
         self,
-        method: str,
-        url: str,
-        headers: typing.Optional[HTTPHeaderDict] = None,
-        fields: typing.Optional[
-            typing.Tuple[typing.Tuple[str, typing.Any], ...]
-        ] = None,
-        body: typing.Optional[typing.Union[str, bytes]] = None,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> urllib3.HTTPResponse:
+        method,
+        url,
+        headers=None,
+        body=None,
+        post_params=None,
+        _request_timeout=None,
+    ):
         """Perform requests.
 
         :param method: http request method
         :param url: http request url
         :param headers: http request headers
-        :param body: request body, for other types
-        :param fields: request parameters for
-                                `application/x-www-form-urlencoded`
-                                or `multipart/form-data`
-        :param stream: if True, the urllib3.HTTPResponse object will
-                                be returned without reading/decoding response
-                                data. Default is False.
-        :param timeout: timeout setting for this request. If one
-                                number provided, it will be total request
-                                timeout. It can also be a pair (tuple) of
-                                (connection, read) timeouts.
+        :param body: request json body, for `application/json`
+        :param post_params: request post parameters,
+                            `application/x-www-form-urlencoded`
+                            and `multipart/form-data`
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
         """
         method = method.upper()
         assert method in ["GET", "HEAD", "DELETE", "POST", "PUT", "PATCH", "OPTIONS"]
 
-        if fields and body:
-            raise ApiValueError("body parameter cannot be used with fields parameter.")
+        if post_params and body:
+            raise ApiValueError(
+                "body parameter cannot be used with post_params parameter."
+            )
 
-        fields = fields or {}
+        post_params = post_params or {}
         headers = headers or {}
 
-        if timeout:
-            if isinstance(timeout, (int, float)):  # noqa: E501,F821
-                timeout = urllib3.Timeout(total=timeout)
-            elif isinstance(timeout, tuple) and len(timeout) == 2:
-                timeout = urllib3.Timeout(connect=timeout[0], read=timeout[1])
+        timeout = None
+        if _request_timeout:
+            if isinstance(_request_timeout, (int, float)):
+                timeout = urllib3.Timeout(total=_request_timeout)
+            elif isinstance(_request_timeout, tuple) and len(_request_timeout) == 2:
+                timeout = urllib3.Timeout(
+                    connect=_request_timeout[0], read=_request_timeout[1]
+                )
 
         try:
             # For `POST`, `PUT`, `PATCH`, `OPTIONS`, `DELETE`
             if method in ["POST", "PUT", "PATCH", "OPTIONS", "DELETE"]:
-                if "Content-Type" not in headers and body is None:
+
+                # no content type provided or payload is json
+                content_type = headers.get("Content-Type")
+                if not content_type or re.search("json", content_type, re.IGNORECASE):
+                    request_body = None
+                    if body is not None:
+                        request_body = json.dumps(body)
                     r = self.pool_manager.request(
                         method,
                         url,
-                        preload_content=not stream,
+                        body=request_body,
                         timeout=timeout,
                         headers=headers,
+                        preload_content=False,
                     )
-                elif (
-                    headers["Content-Type"] == "application/x-www-form-urlencoded"
-                ):  # noqa: E501
+                elif content_type == "application/x-www-form-urlencoded":
                     r = self.pool_manager.request(
                         method,
                         url,
-                        body=body,
-                        fields=fields,
+                        fields=post_params,
                         encode_multipart=False,
-                        preload_content=not stream,
                         timeout=timeout,
                         headers=headers,
+                        preload_content=False,
                     )
-                elif headers["Content-Type"] == "multipart/form-data":
+                elif content_type == "multipart/form-data":
                     # must del headers['Content-Type'], or the correct
                     # Content-Type which generated by urllib3 will be
                     # overwritten.
                     del headers["Content-Type"]
+                    # Ensures that dict objects are serialized
+                    post_params = [
+                        (a, json.dumps(b)) if isinstance(b, dict) else (a, b)
+                        for a, b in post_params
+                    ]
                     r = self.pool_manager.request(
                         method,
                         url,
-                        fields=fields,
+                        fields=post_params,
                         encode_multipart=True,
-                        preload_content=not stream,
                         timeout=timeout,
                         headers=headers,
+                        preload_content=False,
                     )
                 # Pass a `string` parameter directly in the body to support
-                # other content types than Json when `body` argument is
-                # provided in serialized form
+                # other content types than JSON when `body` argument is
+                # provided in serialized form.
                 elif isinstance(body, str) or isinstance(body, bytes):
-                    request_body = body
+                    r = self.pool_manager.request(
+                        method,
+                        url,
+                        body=body,
+                        timeout=timeout,
+                        headers=headers,
+                        preload_content=False,
+                    )
+                elif headers["Content-Type"] == "text/plain" and isinstance(body, bool):
+                    request_body = "true" if body else "false"
                     r = self.pool_manager.request(
                         method,
                         url,
                         body=request_body,
-                        preload_content=not stream,
+                        preload_content=False,
                         timeout=timeout,
                         headers=headers,
                     )
                 else:
                     # Cannot generate the request from given parameters
                     msg = """Cannot prepare a request message for provided
                              arguments. Please check that your arguments match
                              declared content type."""
                     raise ApiException(status=0, reason=msg)
             # For `GET`, `HEAD`
             else:
                 r = self.pool_manager.request(
                     method,
                     url,
-                    preload_content=not stream,
+                    fields={},
                     timeout=timeout,
                     headers=headers,
+                    preload_content=False,
                 )
         except urllib3.exceptions.SSLError as e:
-            msg = "{0}\n{1}".format(type(e).__name__, str(e))
+            msg = "\n".join([type(e).__name__, str(e)])
             raise ApiException(status=0, reason=msg)
 
-        if not stream:
-            # log response body
-            logger.debug("response body: %s", r.data)
-
-        return r
-
-    def GET(
-        self, url, headers=None, stream=False, timeout=None, fields=None
-    ) -> urllib3.HTTPResponse:
-        return self.request(
-            "GET", url, headers=headers, stream=stream, timeout=timeout, fields=fields
-        )
-
-    def HEAD(
-        self, url, headers=None, stream=False, timeout=None, fields=None
-    ) -> urllib3.HTTPResponse:
-        return self.request(
-            "HEAD", url, headers=headers, stream=stream, timeout=timeout, fields=fields
-        )
-
-    def OPTIONS(
-        self, url, headers=None, body=None, stream=False, timeout=None, fields=None
-    ) -> urllib3.HTTPResponse:
-        return self.request(
-            "OPTIONS",
-            url,
-            headers=headers,
-            stream=stream,
-            timeout=timeout,
-            body=body,
-            fields=fields,
-        )
-
-    def DELETE(
-        self, url, headers=None, body=None, stream=False, timeout=None, fields=None
-    ) -> urllib3.HTTPResponse:
-        return self.request(
-            "DELETE",
-            url,
-            headers=headers,
-            stream=stream,
-            timeout=timeout,
-            body=body,
-            fields=fields,
-        )
-
-    def POST(
-        self, url, headers=None, body=None, stream=False, timeout=None, fields=None
-    ) -> urllib3.HTTPResponse:
-        return self.request(
-            "POST",
-            url,
-            headers=headers,
-            stream=stream,
-            timeout=timeout,
-            body=body,
-            fields=fields,
-        )
-
-    def PUT(
-        self, url, headers=None, body=None, stream=False, timeout=None, fields=None
-    ) -> urllib3.HTTPResponse:
-        return self.request(
-            "PUT",
-            url,
-            headers=headers,
-            stream=stream,
-            timeout=timeout,
-            body=body,
-            fields=fields,
-        )
-
-    def PATCH(
-        self, url, headers=None, body=None, stream=False, timeout=None, fields=None
-    ) -> urllib3.HTTPResponse:
-        return self.request(
-            "PATCH",
-            url,
-            headers=headers,
-            stream=stream,
-            timeout=timeout,
-            body=body,
-            fields=fields,
-        )
+        return RESTResponse(r)
```

### Comparing `fireblocks-0.0.1/setup.py` & `fireblocks-0.0.2b0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,62 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 from setuptools import setup, find_packages  # noqa: H301
 
-NAME = "fireblocks"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
-
+NAME = "fireblocks"
+VERSION = "0.0.2-beta"
+PYTHON_REQUIRES = ">=3.8"
 REQUIRES = [
-    "certifi >= 14.5.14",
-    "frozendict ~= 2.3.4",
-    "python-dateutil ~= 2.7.0",
-    "setuptools >= 21.0.0",
-    "typing_extensions ~= 4.3.0",
-    "urllib3 ~= 2.0.0",
-    "aenum >= 3.1.11",
-    "cryptography >= 2.7",
+    "urllib3 >= 1.25.3, < 2.1.0",
+    "python-dateutil",
+    "pydantic >= 2",
+    "typing-extensions >= 4.7.1",
     "PyJWT >= 2.3.0",
-    "requests >= 2.22.0",
-    "typing_extensions ~= 4.3.0",
-    "python-dateutil ~= 2.7.0",
+    "cryptography >=2.7",
 ]
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name=NAME,
-    version="v0.0.1",
-    description="Fireblocks Auto Generated SDK",
+    version=VERSION,
+    description="Fireblocks API",
     author="Fireblocks",
     author_email="support@fireblocks.com",
     url="https://pypi.org/project/fireblocks",
     keywords=["Fireblocks", "SDK", "Fireblocks API"],
-    python_requires=">=3.7",
+    python_requires=PYTHON_REQUIRES,
     install_requires=REQUIRES,
     packages=find_packages(exclude=["test", "tests"]),
     include_package_data=True,
-    license="MIT License (MIT)",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
+    license="MIT License",
+    long_description_content_type='text/markdown',
+    long_description=long_description,  # noqa: E501
+    package_data={"fireblocks": ["py.typed"]},
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Topic :: Software Development',
         'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.7',
-    ],
+        'Programming Language :: Python :: 3.8',
+    ]
 )
```

### Comparing `fireblocks-0.0.1/test/test_models/test_add_collateral_request_body.py` & `fireblocks-0.0.2b0/test/test_screening_operation_type.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import unittest
 
-import fireblocks_client
-from fireblocks_client.model.add_collateral_request_body import AddCollateralRequestBody
-from fireblocks_client import configuration
+from fireblocks.models.screening_operation_type import ScreeningOperationType
+
+
+class TestScreeningOperationType(unittest.TestCase):
+    """ScreeningOperationType unit test stubs"""
+
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
 
-class TestAddCollateralRequestBody(unittest.TestCase):
-    """AddCollateralRequestBody unit test stubs"""
-    _configuration = configuration.Configuration()
+    def testScreeningOperationType(self):
+        """Test ScreeningOperationType"""
+        # inst = ScreeningOperationType()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_models/test_aml_screening_result.py` & `fireblocks-0.0.2b0/test/test_blockchains_assets_api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,46 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import unittest
 
-import fireblocks_client
-from fireblocks_client.model.aml_screening_result import AmlScreeningResult
-from fireblocks_client import configuration
+from fireblocks.api.blockchains_assets_api import BlockchainsAssetsApi
+
+
+class TestBlockchainsAssetsApi(unittest.TestCase):
+    """BlockchainsAssetsApi unit test stubs"""
+
+    def setUp(self) -> None:
+        self.api = BlockchainsAssetsApi()
+
+    def tearDown(self) -> None:
+        pass
+
+    def test_get_supported_assets(self) -> None:
+        """Test case for get_supported_assets
+
+        List all asset types supported by Fireblocks
+        """
+        pass
 
+    def test_register_new_asset(self) -> None:
+        """Test case for register_new_asset
 
-class TestAmlScreeningResult(unittest.TestCase):
-    """AmlScreeningResult unit test stubs"""
-    _configuration = configuration.Configuration()
+        Register an asset
+        """
+        pass
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_models/test_amount_aggregation_time_period_method.py` & `fireblocks-0.0.2b0/test/test_users_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,39 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import unittest
 
-import fireblocks_client
-from fireblocks_client.model.amount_aggregation_time_period_method import AmountAggregationTimePeriodMethod
-from fireblocks_client import configuration
+from fireblocks.api.users_api import UsersApi
+
+
+class TestUsersApi(unittest.TestCase):
+    """UsersApi unit test stubs"""
+
+    def setUp(self) -> None:
+        self.api = UsersApi()
+
+    def tearDown(self) -> None:
+        pass
 
+    def test_get_users(self) -> None:
+        """Test case for get_users
 
-class TestAmountAggregationTimePeriodMethod(unittest.TestCase):
-    """AmountAggregationTimePeriodMethod unit test stubs"""
-    _configuration = configuration.Configuration()
+        List users
+        """
+        pass
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_models/test_amount_info.py` & `fireblocks-0.0.2b0/test/test_conversion_operation_type.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import unittest
 
-import fireblocks_client
-from fireblocks_client.model.amount_info import AmountInfo
-from fireblocks_client import configuration
+from fireblocks.models.conversion_operation_type import ConversionOperationType
+
+
+class TestConversionOperationType(unittest.TestCase):
+    """ConversionOperationType unit test stubs"""
+
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
 
-class TestAmountInfo(unittest.TestCase):
-    """AmountInfo unit test stubs"""
-    _configuration = configuration.Configuration()
+    def testConversionOperationType(self):
+        """Test ConversionOperationType"""
+        # inst = ConversionOperationType()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_models/test_asset_type_response.py` & `fireblocks-0.0.2b0/test/test_transfer_peer_path_type.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import unittest
 
-import fireblocks_client
-from fireblocks_client.model.asset_type_response import AssetTypeResponse
-from fireblocks_client import configuration
+from fireblocks.models.transfer_peer_path_type import TransferPeerPathType
+
+
+class TestTransferPeerPathType(unittest.TestCase):
+    """TransferPeerPathType unit test stubs"""
+
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
 
-class TestAssetTypeResponse(unittest.TestCase):
-    """AssetTypeResponse unit test stubs"""
-    _configuration = configuration.Configuration()
+    def testTransferPeerPathType(self):
+        """Test TransferPeerPathType"""
+        # inst = TransferPeerPathType()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_models/test_asset_wallet.py` & `fireblocks-0.0.2b0/test/test_fiat_account_type.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import unittest
 
-import fireblocks_client
-from fireblocks_client.model.asset_wallet import AssetWallet
-from fireblocks_client import configuration
+from fireblocks.models.fiat_account_type import FiatAccountType
+
+
+class TestFiatAccountType(unittest.TestCase):
+    """FiatAccountType unit test stubs"""
+
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
 
-class TestAssetWallet(unittest.TestCase):
-    """AssetWallet unit test stubs"""
-    _configuration = configuration.Configuration()
+    def testFiatAccountType(self):
+        """Test FiatAccountType"""
+        # inst = FiatAccountType()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_models/test_block_info.py` & `fireblocks-0.0.2b0/test/test_workflow_config_status.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import unittest
 
-import fireblocks_client
-from fireblocks_client.model.block_info import BlockInfo
-from fireblocks_client import configuration
+from fireblocks.models.workflow_config_status import WorkflowConfigStatus
+
+
+class TestWorkflowConfigStatus(unittest.TestCase):
+    """WorkflowConfigStatus unit test stubs"""
+
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
 
-class TestBlockInfo(unittest.TestCase):
-    """BlockInfo unit test stubs"""
-    _configuration = configuration.Configuration()
+    def testWorkflowConfigStatus(self):
+        """Test WorkflowConfigStatus"""
+        # inst = WorkflowConfigStatus()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_models/test_cancel_transaction_response.py` & `fireblocks-0.0.2b0/test/test_assets_api.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,39 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import unittest
 
-import fireblocks_client
-from fireblocks_client.model.cancel_transaction_response import CancelTransactionResponse
-from fireblocks_client import configuration
+from fireblocks.api.assets_api import AssetsApi
+
+
+class TestAssetsApi(unittest.TestCase):
+    """AssetsApi unit test stubs"""
+
+    def setUp(self) -> None:
+        self.api = AssetsApi()
+
+    def tearDown(self) -> None:
+        pass
 
+    def test_create_assets_bulk(self) -> None:
+        """Test case for create_assets_bulk
 
-class TestCancelTransactionResponse(unittest.TestCase):
-    """CancelTransactionResponse unit test stubs"""
-    _configuration = configuration.Configuration()
+        Bulk creation of wallets
+        """
+        pass
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_models/test_collection_ownership_response.py` & `fireblocks-0.0.2b0/test/test_execution_operation_status.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import unittest
 
-import fireblocks_client
-from fireblocks_client.model.collection_ownership_response import CollectionOwnershipResponse
-from fireblocks_client import configuration
+from fireblocks.models.execution_operation_status import ExecutionOperationStatus
+
+
+class TestExecutionOperationStatus(unittest.TestCase):
+    """ExecutionOperationStatus unit test stubs"""
+
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
 
-class TestCollectionOwnershipResponse(unittest.TestCase):
-    """CollectionOwnershipResponse unit test stubs"""
-    _configuration = configuration.Configuration()
+    def testExecutionOperationStatus(self):
+        """Test ExecutionOperationStatus"""
+        # inst = ExecutionOperationStatus()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_models/test_create_connection_request.py` & `fireblocks-0.0.2b0/test/test_user_status.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import unittest
 
-import fireblocks_client
-from fireblocks_client.model.create_connection_request import CreateConnectionRequest
-from fireblocks_client import configuration
+from fireblocks.models.user_status import UserStatus
+
+
+class TestUserStatus(unittest.TestCase):
+    """UserStatus unit test stubs"""
+
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
 
-class TestCreateConnectionRequest(unittest.TestCase):
-    """CreateConnectionRequest unit test stubs"""
-    _configuration = configuration.Configuration()
+    def testUserStatus(self):
+        """Test UserStatus"""
+        # inst = UserStatus()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_models/test_create_internal_transfer_request.py` & `fireblocks-0.0.2b0/test/test_disbursement_operation_type.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import unittest
 
-import fireblocks_client
-from fireblocks_client.model.create_internal_transfer_request import CreateInternalTransferRequest
-from fireblocks_client import configuration
+from fireblocks.models.disbursement_operation_type import DisbursementOperationType
+
+
+class TestDisbursementOperationType(unittest.TestCase):
+    """DisbursementOperationType unit test stubs"""
+
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
 
-class TestCreateInternalTransferRequest(unittest.TestCase):
-    """CreateInternalTransferRequest unit test stubs"""
-    _configuration = configuration.Configuration()
+    def testDisbursementOperationType(self):
+        """Test DisbursementOperationType"""
+        # inst = DisbursementOperationType()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_models/test_create_transaction_response.py` & `fireblocks-0.0.2b0/fireblocks/models/screening_operation_type.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
+
+from __future__ import annotations
+import json
+from enum import Enum
+from typing_extensions import Self
 
-import unittest
 
-import fireblocks_client
-from fireblocks_client.model.create_transaction_response import CreateTransactionResponse
-from fireblocks_client import configuration
+class ScreeningOperationType(str, Enum):
+    """
+    ScreeningOperationType
+    """
 
+    """
+    allowed enum values
+    """
+    SCREENING = 'SCREENING'
 
-class TestCreateTransactionResponse(unittest.TestCase):
-    """CreateTransactionResponse unit test stubs"""
-    _configuration = configuration.Configuration()
+    @classmethod
+    def from_json(cls, json_str: str) -> Self:
+        """Create an instance of ScreeningOperationType from a JSON string"""
+        return cls(json.loads(json_str))
 
 
-if __name__ == '__main__':
-    unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_models/test_create_users_group_response.py` & `fireblocks-0.0.2b0/fireblocks/base_path.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,20 @@
-# coding: utf-8
-
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
-
-import unittest
-
-import fireblocks_client
-from fireblocks_client.model.create_users_group_response import CreateUsersGroupResponse
-from fireblocks_client import configuration
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""  # noqa: E501
 
-class TestCreateUsersGroupResponse(unittest.TestCase):
-    """CreateUsersGroupResponse unit test stubs"""
-    _configuration = configuration.Configuration()
+from enum import Enum
 
 
-if __name__ == '__main__':
-    unittest.main()
+class BasePath(str, Enum):
+    Sandbox = "https://sandbox-api.fireblocks.io/v1"
+    US = "https://api.fireblocks.io/v1"
+    EU = "https://eu-api.fireblocks.io/v1"
+    EU2 = "https://eu2-api.fireblocks.io/v1"
```

### Comparing `fireblocks-0.0.1/test/test_models/test_custom_crypto_routing_dest.py` & `fireblocks-0.0.2b0/test/test_webhooks_api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,46 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import unittest
 
-import fireblocks_client
-from fireblocks_client.model.custom_crypto_routing_dest import CustomCryptoRoutingDest
-from fireblocks_client import configuration
+from fireblocks.api.webhooks_api import WebhooksApi
+
+
+class TestWebhooksApi(unittest.TestCase):
+    """WebhooksApi unit test stubs"""
+
+    def setUp(self) -> None:
+        self.api = WebhooksApi()
+
+    def tearDown(self) -> None:
+        pass
+
+    def test_resend_transaction_webhooks(self) -> None:
+        """Test case for resend_transaction_webhooks
+
+        Resend failed webhooks for a transaction by ID
+        """
+        pass
 
+    def test_resend_webhooks(self) -> None:
+        """Test case for resend_webhooks
 
-class TestCustomCryptoRoutingDest(unittest.TestCase):
-    """CustomCryptoRoutingDest unit test stubs"""
-    _configuration = configuration.Configuration()
+        Resend failed webhooks
+        """
+        pass
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_models/test_custom_fiat_routing_dest.py` & `fireblocks-0.0.2b0/test/test_get_transaction_operation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import unittest
 
-import fireblocks_client
-from fireblocks_client.model.custom_fiat_routing_dest import CustomFiatRoutingDest
-from fireblocks_client import configuration
+from fireblocks.models.get_transaction_operation import GetTransactionOperation
+
+
+class TestGetTransactionOperation(unittest.TestCase):
+    """GetTransactionOperation unit test stubs"""
+
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
 
-class TestCustomFiatRoutingDest(unittest.TestCase):
-    """CustomFiatRoutingDest unit test stubs"""
-    _configuration = configuration.Configuration()
+    def testGetTransactionOperation(self):
+        """Test GetTransactionOperation"""
+        # inst = GetTransactionOperation()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_models/test_default_network_routing_dest.py` & `fireblocks-0.0.2b0/test/test_whitelist_ip_addresses_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,39 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import unittest
 
-import fireblocks_client
-from fireblocks_client.model.default_network_routing_dest import DefaultNetworkRoutingDest
-from fireblocks_client import configuration
+from fireblocks.api.whitelist_ip_addresses_api import WhitelistIpAddressesApi
+
+
+class TestWhitelistIpAddressesApi(unittest.TestCase):
+    """WhitelistIpAddressesApi unit test stubs"""
+
+    def setUp(self) -> None:
+        self.api = WhitelistIpAddressesApi()
+
+    def tearDown(self) -> None:
+        pass
 
+    def test_get_whitelist_ip_addresses(self) -> None:
+        """Test case for get_whitelist_ip_addresses
 
-class TestDefaultNetworkRoutingDest(unittest.TestCase):
-    """DefaultNetworkRoutingDest unit test stubs"""
-    _configuration = configuration.Configuration()
+        Gets whitelisted ip addresses
+        """
+        pass
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_models/test_destination_transfer_peer_path_response.py` & `fireblocks-0.0.2b0/test/test_config_operation_status.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import unittest
 
-import fireblocks_client
-from fireblocks_client.model.destination_transfer_peer_path_response import DestinationTransferPeerPathResponse
-from fireblocks_client import configuration
+from fireblocks.models.config_operation_status import ConfigOperationStatus
+
+
+class TestConfigOperationStatus(unittest.TestCase):
+    """ConfigOperationStatus unit test stubs"""
+
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
 
-class TestDestinationTransferPeerPathResponse(unittest.TestCase):
-    """DestinationTransferPeerPathResponse unit test stubs"""
-    _configuration = configuration.Configuration()
+    def testConfigOperationStatus(self):
+        """Test ConfigOperationStatus"""
+        # inst = ConfigOperationStatus()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_models/test_error_response.py` & `fireblocks-0.0.2b0/test/test_reset_device_api.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,39 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import unittest
 
-import fireblocks_client
-from fireblocks_client.model.error_response import ErrorResponse
-from fireblocks_client import configuration
+from fireblocks.api.reset_device_api import ResetDeviceApi
+
+
+class TestResetDeviceApi(unittest.TestCase):
+    """ResetDeviceApi unit test stubs"""
+
+    def setUp(self) -> None:
+        self.api = ResetDeviceApi()
+
+    def tearDown(self) -> None:
+        pass
 
+    def test_reset_device(self) -> None:
+        """Test case for reset_device
 
-class TestErrorResponse(unittest.TestCase):
-    """ErrorResponse unit test stubs"""
-    _configuration = configuration.Configuration()
+        Resets device
+        """
+        pass
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_models/test_exchange_trading_account.py` & `fireblocks-0.0.2b0/test/test_policy_status.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import unittest
 
-import fireblocks_client
-from fireblocks_client.model.exchange_trading_account import ExchangeTradingAccount
-from fireblocks_client import configuration
+from fireblocks.models.policy_status import PolicyStatus
+
+
+class TestPolicyStatus(unittest.TestCase):
+    """PolicyStatus unit test stubs"""
+
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
 
-class TestExchangeTradingAccount(unittest.TestCase):
-    """ExchangeTradingAccount unit test stubs"""
-    _configuration = configuration.Configuration()
+    def testPolicyStatus(self):
+        """Test PolicyStatus"""
+        # inst = PolicyStatus()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_models/test_exchange_type.py` & `fireblocks-0.0.2b0/test/test_exchange_type.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import unittest
 
-import fireblocks_client
-from fireblocks_client.model.exchange_type import ExchangeType
-from fireblocks_client import configuration
+from fireblocks.models.exchange_type import ExchangeType
 
 
 class TestExchangeType(unittest.TestCase):
     """ExchangeType unit test stubs"""
-    _configuration = configuration.Configuration()
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def testExchangeType(self):
+        """Test ExchangeType"""
+        # inst = ExchangeType()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_models/test_fee_info.py` & `fireblocks-0.0.2b0/test/test_payout_status.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import unittest
 
-import fireblocks_client
-from fireblocks_client.model.fee_info import FeeInfo
-from fireblocks_client import configuration
+from fireblocks.models.payout_status import PayoutStatus
+
+
+class TestPayoutStatus(unittest.TestCase):
+    """PayoutStatus unit test stubs"""
+
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
 
-class TestFeeInfo(unittest.TestCase):
-    """FeeInfo unit test stubs"""
-    _configuration = configuration.Configuration()
+    def testPayoutStatus(self):
+        """Test PayoutStatus"""
+        # inst = PayoutStatus()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_models/test_freeze_transaction_response.py` & `fireblocks-0.0.2b0/fireblocks/models/fiat_account_type.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
+
+from __future__ import annotations
+import json
+from enum import Enum
+from typing_extensions import Self
 
-import unittest
 
-import fireblocks_client
-from fireblocks_client.model.freeze_transaction_response import FreezeTransactionResponse
-from fireblocks_client import configuration
+class FiatAccountType(str, Enum):
+    """
+    FiatAccountType
+    """
 
+    """
+    allowed enum values
+    """
+    BLINC = 'BLINC'
 
-class TestFreezeTransactionResponse(unittest.TestCase):
-    """FreezeTransactionResponse unit test stubs"""
-    _configuration = configuration.Configuration()
+    @classmethod
+    def from_json(cls, json_str: str) -> Self:
+        """Create an instance of FiatAccountType from a JSON string"""
+        return cls(json.loads(json_str))
 
 
-if __name__ == '__main__':
-    unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_models/test_gas_station_configuration.py` & `fireblocks-0.0.2b0/test/test_ota_beta_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,46 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import unittest
 
-import fireblocks_client
-from fireblocks_client.model.gas_station_configuration import GasStationConfiguration
-from fireblocks_client import configuration
+from fireblocks.api.ota_beta_api import OTABetaApi
+
+
+class TestOTABetaApi(unittest.TestCase):
+    """OTABetaApi unit test stubs"""
+
+    def setUp(self) -> None:
+        self.api = OTABetaApi()
+
+    def tearDown(self) -> None:
+        pass
+
+    def test_get_ota_status(self) -> None:
+        """Test case for get_ota_status
+
+        Returns current OTA status
+        """
+        pass
 
+    def test_set_ota_status(self) -> None:
+        """Test case for set_ota_status
 
-class TestGasStationConfiguration(unittest.TestCase):
-    """GasStationConfiguration unit test stubs"""
-    _configuration = configuration.Configuration()
+        Enable or disable transactions to OTA
+        """
+        pass
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_models/test_get_settlement_response.py` & `fireblocks-0.0.2b0/test/test_policy_src_or_dest_type.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import unittest
 
-import fireblocks_client
-from fireblocks_client.model.get_settlement_response import GetSettlementResponse
-from fireblocks_client import configuration
+from fireblocks.models.policy_src_or_dest_type import PolicySrcOrDestType
+
+
+class TestPolicySrcOrDestType(unittest.TestCase):
+    """PolicySrcOrDestType unit test stubs"""
+
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
 
-class TestGetSettlementResponse(unittest.TestCase):
-    """GetSettlementResponse unit test stubs"""
-    _configuration = configuration.Configuration()
+    def testPolicySrcOrDestType(self):
+        """Test PolicySrcOrDestType"""
+        # inst = PolicySrcOrDestType()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_models/test_get_transaction_operation.py` & `fireblocks-0.0.2b0/test/test_config_change_request_status.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import unittest
 
-import fireblocks_client
-from fireblocks_client.model.get_transaction_operation import GetTransactionOperation
-from fireblocks_client import configuration
+from fireblocks.models.config_change_request_status import ConfigChangeRequestStatus
+
+
+class TestConfigChangeRequestStatus(unittest.TestCase):
+    """ConfigChangeRequestStatus unit test stubs"""
+
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
 
-class TestGetTransactionOperation(unittest.TestCase):
-    """GetTransactionOperation unit test stubs"""
-    _configuration = configuration.Configuration()
+    def testConfigChangeRequestStatus(self):
+        """Test ConfigChangeRequestStatus"""
+        # inst = ConfigChangeRequestStatus()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_models/test_instruction_amount.py` & `fireblocks-0.0.2b0/test/test_api_user_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,46 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import unittest
 
-import fireblocks_client
-from fireblocks_client.model.instruction_amount import InstructionAmount
-from fireblocks_client import configuration
+from fireblocks.api.api_user_api import ApiUserApi
+
+
+class TestApiUserApi(unittest.TestCase):
+    """ApiUserApi unit test stubs"""
+
+    def setUp(self) -> None:
+        self.api = ApiUserApi()
+
+    def tearDown(self) -> None:
+        pass
+
+    def test_create_api_user(self) -> None:
+        """Test case for create_api_user
+
+        Create Api user
+        """
+        pass
 
+    def test_get_api_users(self) -> None:
+        """Test case for get_api_users
 
-class TestInstructionAmount(unittest.TestCase):
-    """InstructionAmount unit test stubs"""
-    _configuration = configuration.Configuration()
+        Get Api users
+        """
+        pass
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_models/test_payee_account.py` & `fireblocks-0.0.2b0/test/test_payee_account_type.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import unittest
 
-import fireblocks_client
-from fireblocks_client.model.payee_account import PayeeAccount
-from fireblocks_client import configuration
+from fireblocks.models.payee_account_type import PayeeAccountType
+
+
+class TestPayeeAccountType(unittest.TestCase):
+    """PayeeAccountType unit test stubs"""
+
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
 
-class TestPayeeAccount(unittest.TestCase):
-    """PayeeAccount unit test stubs"""
-    _configuration = configuration.Configuration()
+    def testPayeeAccountType(self):
+        """Test PayeeAccountType"""
+        # inst = PayeeAccountType()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_models/test_payment_account.py` & `fireblocks-0.0.2b0/test/test_payment_account_type.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import unittest
 
-import fireblocks_client
-from fireblocks_client.model.payment_account import PaymentAccount
-from fireblocks_client import configuration
+from fireblocks.models.payment_account_type import PaymentAccountType
+
+
+class TestPaymentAccountType(unittest.TestCase):
+    """PaymentAccountType unit test stubs"""
+
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
 
-class TestPaymentAccount(unittest.TestCase):
-    """PaymentAccount unit test stubs"""
-    _configuration = configuration.Configuration()
+    def testPaymentAccountType(self):
+        """Test PaymentAccountType"""
+        # inst = PaymentAccountType()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_models/test_payment_account_type.py` & `fireblocks-0.0.2b0/test/test_audit_logs_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,46 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import unittest
 
-import fireblocks_client
-from fireblocks_client.model.payment_account_type import PaymentAccountType
-from fireblocks_client import configuration
+from fireblocks.api.audit_logs_api import AuditLogsApi
+
+
+class TestAuditLogsApi(unittest.TestCase):
+    """AuditLogsApi unit test stubs"""
+
+    def setUp(self) -> None:
+        self.api = AuditLogsApi()
+
+    def tearDown(self) -> None:
+        pass
+
+    def test_get_audit_logs(self) -> None:
+        """Test case for get_audit_logs
+
+        Get audit logs
+        """
+        pass
 
+    def test_get_audits(self) -> None:
+        """Test case for get_audits
 
-class TestPaymentAccountType(unittest.TestCase):
-    """PaymentAccountType unit test stubs"""
-    _configuration = configuration.Configuration()
+        Get audit logs
+        """
+        pass
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_models/test_respond_to_connection_request.py` & `fireblocks-0.0.2b0/test/test_payout_state.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import unittest
 
-import fireblocks_client
-from fireblocks_client.model.respond_to_connection_request import RespondToConnectionRequest
-from fireblocks_client import configuration
+from fireblocks.models.payout_state import PayoutState
+
+
+class TestPayoutState(unittest.TestCase):
+    """PayoutState unit test stubs"""
+
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
 
-class TestRespondToConnectionRequest(unittest.TestCase):
-    """RespondToConnectionRequest unit test stubs"""
-    _configuration = configuration.Configuration()
+    def testPayoutState(self):
+        """Test PayoutState"""
+        # inst = PayoutState()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_models/test_source_transfer_peer_path_response.py` & `fireblocks-0.0.2b0/test/test_amount_aggregation_time_period_method.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,38 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import unittest
 
-import fireblocks_client
-from fireblocks_client.model.source_transfer_peer_path_response import SourceTransferPeerPathResponse
-from fireblocks_client import configuration
+from fireblocks.models.amount_aggregation_time_period_method import (
+    AmountAggregationTimePeriodMethod,
+)
+
+
+class TestAmountAggregationTimePeriodMethod(unittest.TestCase):
+    """AmountAggregationTimePeriodMethod unit test stubs"""
+
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
 
-class TestSourceTransferPeerPathResponse(unittest.TestCase):
-    """SourceTransferPeerPathResponse unit test stubs"""
-    _configuration = configuration.Configuration()
+    def testAmountAggregationTimePeriodMethod(self):
+        """Test AmountAggregationTimePeriodMethod"""
+        # inst = AmountAggregationTimePeriodMethod()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_models/test_travel_rule_validate_full_transaction_request.py` & `fireblocks-0.0.2b0/fireblocks/models/payment_account_type.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,39 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
-
-import unittest
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import fireblocks_client
-from fireblocks_client.model.travel_rule_validate_full_transaction_request import TravelRuleValidateFullTransactionRequest
-from fireblocks_client import configuration
+    Do not edit the class manually.
+"""  # noqa: E501
 
 
-class TestTravelRuleValidateFullTransactionRequest(unittest.TestCase):
-    """TravelRuleValidateFullTransactionRequest unit test stubs"""
-    _configuration = configuration.Configuration()
+from __future__ import annotations
+import json
+from enum import Enum
+from typing_extensions import Self
+
+
+class PaymentAccountType(str, Enum):
+    """
+    PaymentAccountType
+    """
+
+    """
+    allowed enum values
+    """
+    VAULT_ACCOUNT = 'VAULT_ACCOUNT'
+    EXCHANGE_ACCOUNT = 'EXCHANGE_ACCOUNT'
+    FIAT_ACCOUNT = 'FIAT_ACCOUNT'
+
+    @classmethod
+    def from_json(cls, json_str: str) -> Self:
+        """Create an instance of PaymentAccountType from a JSON string"""
+        return cls(json.loads(json_str))
 
 
-if __name__ == '__main__':
-    unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_models/test_xb_settlement_crypto_asset.py` & `fireblocks-0.0.2b0/test/test_workspace_status_beta_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,39 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import unittest
 
-import fireblocks_client
-from fireblocks_client.model.xb_settlement_crypto_asset import XBSettlementCryptoAsset
-from fireblocks_client import configuration
+from fireblocks.api.workspace_status_beta_api import WorkspaceStatusBetaApi
+
+
+class TestWorkspaceStatusBetaApi(unittest.TestCase):
+    """WorkspaceStatusBetaApi unit test stubs"""
+
+    def setUp(self) -> None:
+        self.api = WorkspaceStatusBetaApi()
+
+    def tearDown(self) -> None:
+        pass
 
+    def test_get_workspace_status(self) -> None:
+        """Test case for get_workspace_status
 
-class TestXBSettlementCryptoAsset(unittest.TestCase):
-    """XBSettlementCryptoAsset unit test stubs"""
-    _configuration = configuration.Configuration()
+        Returns current workspace status
+        """
+        pass
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_connections/test_get.py` & `fireblocks-0.0.2b0/test/test_error_schema.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,55 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import unittest
-from unittest.mock import patch
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import urllib3
 
-import fireblocks_client
-from fireblocks_client.paths.connections import get  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
+import unittest
 
-from .. import ApiTestMixin
+from fireblocks.models.error_schema import ErrorSchema
 
 
-class TestConnections(ApiTestMixin, unittest.TestCase):
-    """
-    Connections unit test stubs
-        List all open Web3 connections.  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+class TestErrorSchema(unittest.TestCase):
+    """ErrorSchema unit test stubs"""
 
     def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    response_status = 200
-
-
+    def make_instance(self, include_optional) -> ErrorSchema:
+        """Test ErrorSchema
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # uncomment below to create an instance of `ErrorSchema`
+        """
+        model = ErrorSchema()
+        if include_optional:
+            return ErrorSchema(
+                message = '',
+                code = 1.337
+            )
+        else:
+            return ErrorSchema(
+        )
+        """
+
+    def testErrorSchema(self):
+        """Test ErrorSchema"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_connections_wc/test_post.py` & `fireblocks-0.0.2b0/fireblocks/models/disbursement_operation_type.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,37 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
-
-import unittest
-from unittest.mock import patch
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import urllib3
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import fireblocks_client
-from fireblocks_client.paths.connections_wc import post  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
 
-from .. import ApiTestMixin
+from __future__ import annotations
+import json
+from enum import Enum
+from typing_extensions import Self
 
 
-class TestConnectionsWc(ApiTestMixin, unittest.TestCase):
+class DisbursementOperationType(str, Enum):
     """
-    ConnectionsWc unit test stubs
-        Create a new Web3 connection.  # noqa: E501
+    DisbursementOperationType
     """
-    _configuration = configuration.Configuration()
-
-    def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
-
-    def tearDown(self):
-        pass
-
-    response_status = 201
-
-
 
+    """
+    allowed enum values
+    """
+    DISBURSEMENT = 'DISBURSEMENT'
 
+    @classmethod
+    def from_json(cls, json_str: str) -> Self:
+        """Create an instance of DisbursementOperationType from a JSON string"""
+        return cls(json.loads(json_str))
 
 
-if __name__ == '__main__':
-    unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_connections_wc_id/test_delete.py` & `fireblocks-0.0.2b0/test/test_rename_cosigner.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,54 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import unittest
-from unittest.mock import patch
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import urllib3
 
-import fireblocks_client
-from fireblocks_client.paths.connections_wc_id import delete  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
+import unittest
 
-from .. import ApiTestMixin
+from fireblocks.models.rename_cosigner import RenameCosigner
 
 
-class TestConnectionsWcId(ApiTestMixin, unittest.TestCase):
-    """
-    ConnectionsWcId unit test stubs
-        Remove an existing Web3 connection.  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+class TestRenameCosigner(unittest.TestCase):
+    """RenameCosigner unit test stubs"""
 
     def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    response_status = 200
-    response_body = ''
+    def make_instance(self, include_optional) -> RenameCosigner:
+        """Test RenameCosigner
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # uncomment below to create an instance of `RenameCosigner`
+        """
+        model = RenameCosigner()
+        if include_optional:
+            return RenameCosigner(
+                name = 'My Cosigner 1'
+            )
+        else:
+            return RenameCosigner(
+        )
+        """
+
+    def testRenameCosigner(self):
+        """Test RenameCosigner"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_connections_wc_id/test_put.py` & `fireblocks-0.0.2b0/test/test_network_channel.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,55 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import unittest
-from unittest.mock import patch
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import urllib3
 
-import fireblocks_client
-from fireblocks_client.paths.connections_wc_id import put  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
+import unittest
 
-from .. import ApiTestMixin
+from fireblocks.models.network_channel import NetworkChannel
 
 
-class TestConnectionsWcId(ApiTestMixin, unittest.TestCase):
-    """
-    ConnectionsWcId unit test stubs
-        Respond to a pending Web3 connection request.  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+class TestNetworkChannel(unittest.TestCase):
+    """NetworkChannel unit test stubs"""
 
     def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    response_status = 200
-    response_body = ''
-
-
+    def make_instance(self, include_optional) -> NetworkChannel:
+        """Test NetworkChannel
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # uncomment below to create an instance of `NetworkChannel`
+        """
+        model = NetworkChannel()
+        if include_optional:
+            return NetworkChannel(
+                network_id = '',
+                name = ''
+            )
+        else:
+            return NetworkChannel(
+        )
+        """
+
+    def testNetworkChannel(self):
+        """Test NetworkChannel"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_contracts/test_get.py` & `fireblocks-0.0.2b0/test/test_network_id.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,57 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import unittest
-from unittest.mock import patch
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import urllib3
 
-import fireblocks_client
-from fireblocks_client.paths.contracts import get  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
+import unittest
 
-from .. import ApiTestMixin
+from fireblocks.models.network_id import NetworkId
 
 
-class TestContracts(ApiTestMixin, unittest.TestCase):
-    """
-    Contracts unit test stubs
-        List contracts  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+class TestNetworkId(unittest.TestCase):
+    """NetworkId unit test stubs"""
 
     def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    response_status = 200
-
-
+    def make_instance(self, include_optional) -> NetworkId:
+        """Test NetworkId
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # uncomment below to create an instance of `NetworkId`
+        """
+        model = NetworkId()
+        if include_optional:
+            return NetworkId(
+                id = '',
+                name = ''
+            )
+        else:
+            return NetworkId(
+                id = '',
+                name = '',
+        )
+        """
+
+    def testNetworkId(self):
+        """Test NetworkId"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_contracts/test_post.py` & `fireblocks-0.0.2b0/test/test_user_groups_beta_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,67 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import unittest
-from unittest.mock import patch
 
-import urllib3
+from fireblocks.api.user_groups_beta_api import UserGroupsBetaApi
 
-import fireblocks_client
-from fireblocks_client.paths.contracts import post  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
 
-from .. import ApiTestMixin
+class TestUserGroupsBetaApi(unittest.TestCase):
+    """UserGroupsBetaApi unit test stubs"""
 
+    def setUp(self) -> None:
+        self.api = UserGroupsBetaApi()
 
-class TestContracts(ApiTestMixin, unittest.TestCase):
-    """
-    Contracts unit test stubs
-        Create a contract  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+    def tearDown(self) -> None:
+        pass
 
-    def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+    def test_create_user_group(self) -> None:
+        """Test case for create_user_group
 
-    def tearDown(self):
+        Create user group
+        """
         pass
 
-    response_status = 200
+    def test_delete_user_group(self) -> None:
+        """Test case for delete_user_group
 
+        Delete user group
+        """
+        pass
+
+    def test_get_user_group(self) -> None:
+        """Test case for get_user_group
 
+        Get user group
+        """
+        pass
+
+    def test_get_user_groups(self) -> None:
+        """Test case for get_user_groups
+
+        List user groups
+        """
+        pass
+
+    def test_update_user_group(self) -> None:
+        """Test case for update_user_group
+
+        Update user group
+        """
+        pass
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_contracts_contract_id/test_get.py` & `fireblocks-0.0.2b0/test/test_contract_interactions_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,53 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import unittest
-from unittest.mock import patch
 
-import urllib3
+from fireblocks.api.contract_interactions_api import ContractInteractionsApi
 
-import fireblocks_client
-from fireblocks_client.paths.contracts_contract_id import get  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
 
-from .. import ApiTestMixin
+class TestContractInteractionsApi(unittest.TestCase):
+    """ContractInteractionsApi unit test stubs"""
 
+    def setUp(self) -> None:
+        self.api = ContractInteractionsApi()
 
-class TestContractsContractId(ApiTestMixin, unittest.TestCase):
-    """
-    ContractsContractId unit test stubs
-        Find a specific contract  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+    def tearDown(self) -> None:
+        pass
 
-    def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+    def test_get_deployed_contract_abi(self) -> None:
+        """Test case for get_deployed_contract_abi
 
-    def tearDown(self):
+        Return deployed contract's ABI
+        """
         pass
 
-    response_status = 200
+    def test_read_call_function(self) -> None:
+        """Test case for read_call_function
 
+        Call a read function on a deployed contract
+        """
+        pass
+
+    def test_write_call_function(self) -> None:
+        """Test case for write_call_function
 
+        Call a write function on a deployed contract
+        """
+        pass
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_contracts_contract_id_asset_id/test_delete.py` & `fireblocks-0.0.2b0/test/test_deployed_contracts_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,53 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import unittest
-from unittest.mock import patch
 
-import urllib3
+from fireblocks.api.deployed_contracts_api import DeployedContractsApi
 
-import fireblocks_client
-from fireblocks_client.paths.contracts_contract_id_asset_id import delete  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
 
-from .. import ApiTestMixin
+class TestDeployedContractsApi(unittest.TestCase):
+    """DeployedContractsApi unit test stubs"""
 
+    def setUp(self) -> None:
+        self.api = DeployedContractsApi()
 
-class TestContractsContractIdAssetId(ApiTestMixin, unittest.TestCase):
-    """
-    ContractsContractIdAssetId unit test stubs
-        Delete a contract asset  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+    def tearDown(self) -> None:
+        pass
 
-    def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
+    def test_get_deployed_contract_by_address(self) -> None:
+        """Test case for get_deployed_contract_by_address
 
-    def tearDown(self):
+        Return deployed contract data
+        """
         pass
 
-    response_status = 201
-    response_body = ''
+    def test_get_deployed_contract_by_id(self) -> None:
+        """Test case for get_deployed_contract_by_id
+
+        Return deployed contract data by id
+        """
+        pass
+
+    def test_get_deployed_contracts(self) -> None:
+        """Test case for get_deployed_contracts
+
+        List deployed contracts data
+        """
+        pass
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_contracts_contract_id_asset_id/test_post.py` & `fireblocks-0.0.2b0/test/test_console_user_api.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import unittest
-from unittest.mock import patch
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import urllib3
 
-import fireblocks_client
-from fireblocks_client.paths.contracts_contract_id_asset_id import post  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
+import unittest
 
-from .. import ApiTestMixin
+from fireblocks.api.console_user_api import ConsoleUserApi
 
 
-class TestContractsContractIdAssetId(ApiTestMixin, unittest.TestCase):
-    """
-    ContractsContractIdAssetId unit test stubs
-        Add an asset to a contract  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+class TestConsoleUserApi(unittest.TestCase):
+    """ConsoleUserApi unit test stubs"""
 
-    def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+    def setUp(self) -> None:
+        self.api = ConsoleUserApi()
 
-    def tearDown(self):
+    def tearDown(self) -> None:
         pass
 
-    response_status = 200
+    def test_create_console_user(self) -> None:
+        """Test case for create_console_user
 
+        Create console user
+        """
+        pass
+
+    def test_get_console_users(self) -> None:
+        """Test case for get_console_users
 
+        Get console users
+        """
+        pass
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_exchange_accounts_exchange_account_id_asset_id/test_get.py` & `fireblocks-0.0.2b0/test/test_asset_amount.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,57 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import unittest
-from unittest.mock import patch
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import urllib3
 
-import fireblocks_client
-from fireblocks_client.paths.exchange_accounts_exchange_account_id_asset_id import get  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
+import unittest
 
-from .. import ApiTestMixin
+from fireblocks.models.asset_amount import AssetAmount
 
 
-class TestExchangeAccountsExchangeAccountIdAssetId(ApiTestMixin, unittest.TestCase):
-    """
-    ExchangeAccountsExchangeAccountIdAssetId unit test stubs
-        Find an asset for an exchange account  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+class TestAssetAmount(unittest.TestCase):
+    """AssetAmount unit test stubs"""
 
     def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    response_status = 200
-
-
+    def make_instance(self, include_optional) -> AssetAmount:
+        """Test AssetAmount
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # uncomment below to create an instance of `AssetAmount`
+        """
+        model = AssetAmount()
+        if include_optional:
+            return AssetAmount(
+                amount = '',
+                asset_id = ''
+            )
+        else:
+            return AssetAmount(
+                amount = '',
+                asset_id = '',
+        )
+        """
+
+    def testAssetAmount(self):
+        """Test AssetAmount"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_exchange_accounts_exchange_account_id_convert/test_post.py` & `fireblocks-0.0.2b0/test/test_signed_message.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,64 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import unittest
-from unittest.mock import patch
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import urllib3
 
-import fireblocks_client
-from fireblocks_client.paths.exchange_accounts_exchange_account_id_convert import post  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
+import unittest
 
-from .. import ApiTestMixin
+from fireblocks.models.signed_message import SignedMessage
 
 
-class TestExchangeAccountsExchangeAccountIdConvert(ApiTestMixin, unittest.TestCase):
-    """
-    ExchangeAccountsExchangeAccountIdConvert unit test stubs
-        Convert exchange account funds from the source asset to the destination asset. Coinbase (USD to USDC, USDC to USD) and Bitso (MXN to USD) are supported conversions.  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+class TestSignedMessage(unittest.TestCase):
+    """SignedMessage unit test stubs"""
 
     def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    response_status = 200
-    response_body = ''
+    def make_instance(self, include_optional) -> SignedMessage:
+        """Test SignedMessage
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # uncomment below to create an instance of `SignedMessage`
+        """
+        model = SignedMessage()
+        if include_optional:
+            return SignedMessage(
+                content = '',
+                algorithm = 'MPC_ECDSA_SECP256K1',
+                derivation_path = [
+                    1.337
+                    ],
+                signature = fireblocks.models.signed_message_signature.SignedMessage_signature(
+                    full_sig = '', 
+                    r = '', 
+                    s = '', 
+                    v = 1.337, ),
+                public_key = ''
+            )
+        else:
+            return SignedMessage(
+        )
+        """
+
+    def testSignedMessage(self):
+        """Test SignedMessage"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_external_wallets_wallet_id/test_delete.py` & `fireblocks-0.0.2b0/test/test_aml_registration_result.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,56 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import unittest
-from unittest.mock import patch
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import urllib3
 
-import fireblocks_client
-from fireblocks_client.paths.external_wallets_wallet_id import delete  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
+import unittest
 
-from .. import ApiTestMixin
+from fireblocks.models.aml_registration_result import AmlRegistrationResult
 
 
-class TestExternalWalletsWalletId(ApiTestMixin, unittest.TestCase):
-    """
-    ExternalWalletsWalletId unit test stubs
-        Delete an external wallet  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+class TestAmlRegistrationResult(unittest.TestCase):
+    """AmlRegistrationResult unit test stubs"""
 
     def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    response_status = 201
-    response_body = ''
+    def make_instance(self, include_optional) -> AmlRegistrationResult:
+        """Test AmlRegistrationResult
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # uncomment below to create an instance of `AmlRegistrationResult`
+        """
+        model = AmlRegistrationResult()
+        if include_optional:
+            return AmlRegistrationResult(
+                provider = '',
+                success = True,
+                timestamp = 1.337
+            )
+        else:
+            return AmlRegistrationResult(
+        )
+        """
+
+    def testAmlRegistrationResult(self):
+        """Test AmlRegistrationResult"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_external_wallets_wallet_id_asset_id/test_post.py` & `fireblocks-0.0.2b0/test/test_pre_screening.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,55 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import unittest
-from unittest.mock import patch
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import urllib3
 
-import fireblocks_client
-from fireblocks_client.paths.external_wallets_wallet_id_asset_id import post  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
+import unittest
 
-from .. import ApiTestMixin
+from fireblocks.models.pre_screening import PreScreening
 
 
-class TestExternalWalletsWalletIdAssetId(ApiTestMixin, unittest.TestCase):
-    """
-    ExternalWalletsWalletIdAssetId unit test stubs
-        Add an asset to an external wallet.  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+class TestPreScreening(unittest.TestCase):
+    """PreScreening unit test stubs"""
 
     def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    response_status = 200
-
-
+    def make_instance(self, include_optional) -> PreScreening:
+        """Test PreScreening
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # uncomment below to create an instance of `PreScreening`
+        """
+        model = PreScreening()
+        if include_optional:
+            return PreScreening(
+                enabled = True
+            )
+        else:
+            return PreScreening(
+                enabled = True,
+        )
+        """
+
+    def testPreScreening(self):
+        """Test PreScreening"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_gas_station_asset_id/test_get.py` & `fireblocks-0.0.2b0/test/test_paging.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,55 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import unittest
-from unittest.mock import patch
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import urllib3
 
-import fireblocks_client
-from fireblocks_client.paths.gas_station_asset_id import get  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
+import unittest
 
-from .. import ApiTestMixin
+from fireblocks.models.paging import Paging
 
 
-class TestGasStationAssetId(ApiTestMixin, unittest.TestCase):
-    """
-    GasStationAssetId unit test stubs
-        Get gas station settings by asset  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+class TestPaging(unittest.TestCase):
+    """Paging unit test stubs"""
 
     def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    response_status = 200
-
-
+    def make_instance(self, include_optional) -> Paging:
+        """Test Paging
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # uncomment below to create an instance of `Paging`
+        """
+        model = Paging()
+        if include_optional:
+            return Paging(
+                next = ''
+            )
+        else:
+            return Paging(
+                next = '',
+        )
+        """
+
+    def testPaging(self):
+        """Test Paging"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_gas_station_configuration_asset_id/test_put.py` & `fireblocks-0.0.2b0/test/test_screening_update_configurations_request.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,57 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import unittest
-from unittest.mock import patch
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import urllib3
 
-import fireblocks_client
-from fireblocks_client.paths.gas_station_configuration_asset_id import put  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
+import unittest
 
-from .. import ApiTestMixin
+from fireblocks.models.screening_update_configurations_request import (
+    ScreeningUpdateConfigurationsRequest,
+)
 
 
-class TestGasStationConfigurationAssetId(ApiTestMixin, unittest.TestCase):
-    """
-    GasStationConfigurationAssetId unit test stubs
-        Edit gas station settings for an asset  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+class TestScreeningUpdateConfigurationsRequest(unittest.TestCase):
+    """ScreeningUpdateConfigurationsRequest unit test stubs"""
 
     def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    response_status = 201
-    response_body = ''
-
-
+    def make_instance(self, include_optional) -> ScreeningUpdateConfigurationsRequest:
+        """Test ScreeningUpdateConfigurationsRequest
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # uncomment below to create an instance of `ScreeningUpdateConfigurationsRequest`
+        """
+        model = ScreeningUpdateConfigurationsRequest()
+        if include_optional:
+            return ScreeningUpdateConfigurationsRequest(
+                disable_bypass = True,
+                disable_unfreeze = True
+            )
+        else:
+            return ScreeningUpdateConfigurationsRequest(
+        )
+        """
+
+    def testScreeningUpdateConfigurationsRequest(self):
+        """Test ScreeningUpdateConfigurationsRequest"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_internal_wallets_wallet_id/test_delete.py` & `fireblocks-0.0.2b0/test/test_conversion_operation_config_params.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,61 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import unittest
-from unittest.mock import patch
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import urllib3
 
-import fireblocks_client
-from fireblocks_client.paths.internal_wallets_wallet_id import delete  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
+import unittest
 
-from .. import ApiTestMixin
+from fireblocks.models.conversion_operation_config_params import (
+    ConversionOperationConfigParams,
+)
 
 
-class TestInternalWalletsWalletId(ApiTestMixin, unittest.TestCase):
-    """
-    InternalWalletsWalletId unit test stubs
-        Delete an internal wallet  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+class TestConversionOperationConfigParams(unittest.TestCase):
+    """ConversionOperationConfigParams unit test stubs"""
 
     def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    response_status = 201
-    response_body = ''
+    def make_instance(self, include_optional) -> ConversionOperationConfigParams:
+        """Test ConversionOperationConfigParams
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # uncomment below to create an instance of `ConversionOperationConfigParams`
+        """
+        model = ConversionOperationConfigParams()
+        if include_optional:
+            return ConversionOperationConfigParams(
+                amount = '',
+                account_id = '',
+                src_asset_id = '',
+                dest_asset_id = '',
+                slippage_basis_points = 0
+            )
+        else:
+            return ConversionOperationConfigParams(
+                dest_asset_id = '',
+        )
+        """
+
+    def testConversionOperationConfigParams(self):
+        """Test ConversionOperationConfigParams"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_internal_wallets_wallet_id_asset_id/test_get.py` & `fireblocks-0.0.2b0/test/test_none_network_routing_dest.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,55 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import unittest
-from unittest.mock import patch
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import urllib3
 
-import fireblocks_client
-from fireblocks_client.paths.internal_wallets_wallet_id_asset_id import get  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
+import unittest
 
-from .. import ApiTestMixin
+from fireblocks.models.none_network_routing_dest import NoneNetworkRoutingDest
 
 
-class TestInternalWalletsWalletIdAssetId(ApiTestMixin, unittest.TestCase):
-    """
-    InternalWalletsWalletIdAssetId unit test stubs
-        Get an asset from an internal wallet  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+class TestNoneNetworkRoutingDest(unittest.TestCase):
+    """NoneNetworkRoutingDest unit test stubs"""
 
     def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    response_status = 200
-
-
+    def make_instance(self, include_optional) -> NoneNetworkRoutingDest:
+        """Test NoneNetworkRoutingDest
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # uncomment below to create an instance of `NoneNetworkRoutingDest`
+        """
+        model = NoneNetworkRoutingDest()
+        if include_optional:
+            return NoneNetworkRoutingDest(
+                scheme = 'NONE'
+            )
+        else:
+            return NoneNetworkRoutingDest(
+                scheme = 'NONE',
+        )
+        """
+
+    def testNoneNetworkRoutingDest(self):
+        """Test NoneNetworkRoutingDest"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_internal_wallets_wallet_id_asset_id/test_post.py` & `fireblocks-0.0.2b0/test/test_one_time_address_account.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,56 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import unittest
-from unittest.mock import patch
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import urllib3
 
-import fireblocks_client
-from fireblocks_client.paths.internal_wallets_wallet_id_asset_id import post  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
+import unittest
 
-from .. import ApiTestMixin
+from fireblocks.models.one_time_address_account import OneTimeAddressAccount
 
 
-class TestInternalWalletsWalletIdAssetId(ApiTestMixin, unittest.TestCase):
-    """
-    InternalWalletsWalletIdAssetId unit test stubs
-        Add an asset to an internal wallet  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+class TestOneTimeAddressAccount(unittest.TestCase):
+    """OneTimeAddressAccount unit test stubs"""
 
     def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    response_status = 200
-
-
+    def make_instance(self, include_optional) -> OneTimeAddressAccount:
+        """Test OneTimeAddressAccount
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # uncomment below to create an instance of `OneTimeAddressAccount`
+        """
+        model = OneTimeAddressAccount()
+        if include_optional:
+            return OneTimeAddressAccount(
+                one_time_address = '',
+                tag = ''
+            )
+        else:
+            return OneTimeAddressAccount(
+                one_time_address = '',
+        )
+        """
+
+    def testOneTimeAddressAccount(self):
+        """Test OneTimeAddressAccount"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_network_connections_connection_id_is_third_party_routing_asset_type/test_get.py` & `fireblocks-0.0.2b0/test/test_transaction.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,59 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import unittest
-from unittest.mock import patch
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import urllib3
 
-import fireblocks_client
-from fireblocks_client.paths.network_connections_connection_id_is_third_party_routing_asset_type import get  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
+import unittest
 
-from .. import ApiTestMixin
+from fireblocks.models.transaction import Transaction
 
 
-class TestNetworkConnectionsConnectionIdIsThirdPartyRoutingAssetType(ApiTestMixin, unittest.TestCase):
-    """
-    NetworkConnectionsConnectionIdIsThirdPartyRoutingAssetType unit test stubs
-        Retrieve third-party network routing validation by asset type.  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+class TestTransaction(unittest.TestCase):
+    """Transaction unit test stubs"""
 
     def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    response_status = 200
-
-
+    def make_instance(self, include_optional) -> Transaction:
+        """Test Transaction
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # uncomment below to create an instance of `Transaction`
+        """
+        model = Transaction()
+        if include_optional:
+            return Transaction(
+                id = '',
+                state = 'SUBMITTED',
+                timestamp = 1.337,
+                instruction_id = ''
+            )
+        else:
+            return Transaction(
+                id = '',
+                state = 'SUBMITTED',
+        )
+        """
+
+    def testTransaction(self):
+        """Test Transaction"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_network_ids_network_id/test_get.py` & `fireblocks-0.0.2b0/test/test_web3_connections_api.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,60 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import unittest
-from unittest.mock import patch
 
-import urllib3
+from fireblocks.api.web3_connections_api import Web3ConnectionsApi
+
+
+class TestWeb3ConnectionsApi(unittest.TestCase):
+    """Web3ConnectionsApi unit test stubs"""
 
-import fireblocks_client
-from fireblocks_client.paths.network_ids_network_id import get  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
+    def setUp(self) -> None:
+        self.api = Web3ConnectionsApi()
 
-from .. import ApiTestMixin
+    def tearDown(self) -> None:
+        pass
 
+    def test_create(self) -> None:
+        """Test case for create
 
-class TestNetworkIdsNetworkId(ApiTestMixin, unittest.TestCase):
-    """
-    NetworkIdsNetworkId unit test stubs
-        Returns specific network ID.  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+        Create a new Web3 connection.
+        """
+        pass
 
-    def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+    def test_get(self) -> None:
+        """Test case for get
 
-    def tearDown(self):
+        List all open Web3 connections.
+        """
         pass
 
-    response_status = 200
+    def test_remove(self) -> None:
+        """Test case for remove
 
+        Remove an existing Web3 connection.
+        """
+        pass
 
+    def test_submit(self) -> None:
+        """Test case for submit
+
+        Respond to a pending Web3 connection request.
+        """
+        pass
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_network_ids_network_id_set_routing_policy/test_patch.py` & `fireblocks-0.0.2b0/fireblocks/additional_options.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,34 @@
-# coding: utf-8
-
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
-
-import unittest
-from unittest.mock import patch
-
-import urllib3
-
-import fireblocks_client
-from fireblocks_client.paths.network_ids_network_id_set_routing_policy import patch  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
-
-from .. import ApiTestMixin
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""  # noqa: E501
 
-class TestNetworkIdsNetworkIdSetRoutingPolicy(ApiTestMixin, unittest.TestCase):
-    """
-    NetworkIdsNetworkIdSetRoutingPolicy unit test stubs
-        Update network id routing policy.  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
-
-    def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = patch.ApiForpatch(api_client=used_api_client)  # noqa: E501
-
-    def tearDown(self):
-        pass
-
-    response_status = 200
-
+from pydantic import Field, BaseModel
+from typing import Optional
 
+"""This class contains additional options for the Fireblocks API client.
+:param is_anonymous_platform: If set to true, the platform will be anonymous.
+:param user_agent: The user agent to use for the client.
+:param thread_pool_size: The number of threads to use for the client.
+"""
 
 
-if __name__ == '__main__':
-    unittest.main()
+class AdditionalOptions(BaseModel):
+    is_anonymous_platform: Optional[bool] = Field(
+        False, description="If set to true, the platform will be anonymous"
+    )
+    user_agent: Optional[str] = Field(
+        None,
+        description="The custom User-Agent string to be included in the header of every API call made by the client",
+    )
+    thread_pool_size: Optional[int] = Field(
+        None,
+        description="The number of threads to use in the thread pool for the client",
+    )
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_nfts_ownership_collections/test_get.py` & `fireblocks-0.0.2b0/fireblocks/models/user_type.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,38 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
-
-import unittest
-from unittest.mock import patch
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import urllib3
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import fireblocks_client
-from fireblocks_client.paths.nfts_ownership_collections import get  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
 
-from .. import ApiTestMixin
+from __future__ import annotations
+import json
+from enum import Enum
+from typing_extensions import Self
 
 
-class TestNftsOwnershipCollections(ApiTestMixin, unittest.TestCase):
+class UserType(str, Enum):
     """
-    NftsOwnershipCollections unit test stubs
-        List owned collections (paginated)  # noqa: E501
+    The type of the user
     """
-    _configuration = configuration.Configuration()
-
-    def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
-
-    def tearDown(self):
-        pass
-
-    response_status = 200
 
+    """
+    allowed enum values
+    """
+    API = 'API'
+    CONSOLE = 'CONSOLE'
 
+    @classmethod
+    def from_json(cls, json_str: str) -> Self:
+        """Create an instance of UserType from a JSON string"""
+        return cls(json.loads(json_str))
 
 
-if __name__ == '__main__':
-    unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_nfts_ownership_tokens/test_get.py` & `fireblocks-0.0.2b0/test/test_fee_info.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,56 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import unittest
-from unittest.mock import patch
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import urllib3
 
-import fireblocks_client
-from fireblocks_client.paths.nfts_ownership_tokens import get  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
+import unittest
 
-from .. import ApiTestMixin
+from fireblocks.models.fee_info import FeeInfo
 
 
-class TestNftsOwnershipTokens(ApiTestMixin, unittest.TestCase):
-    """
-    NftsOwnershipTokens unit test stubs
-        List all owned tokens (paginated)  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+class TestFeeInfo(unittest.TestCase):
+    """FeeInfo unit test stubs"""
 
     def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    response_status = 200
-
-
+    def make_instance(self, include_optional) -> FeeInfo:
+        """Test FeeInfo
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # uncomment below to create an instance of `FeeInfo`
+        """
+        model = FeeInfo()
+        if include_optional:
+            return FeeInfo(
+                network_fee = '',
+                service_fee = '',
+                gas_price = ''
+            )
+        else:
+            return FeeInfo(
+        )
+        """
+
+    def testFeeInfo(self):
+        """Test FeeInfo"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_nfts_ownership_tokens/test_put.py` & `fireblocks-0.0.2b0/test/test_unspent_input.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,55 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import unittest
-from unittest.mock import patch
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import urllib3
 
-import fireblocks_client
-from fireblocks_client.paths.nfts_ownership_tokens import put  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
+import unittest
 
-from .. import ApiTestMixin
+from fireblocks.models.unspent_input import UnspentInput
 
 
-class TestNftsOwnershipTokens(ApiTestMixin, unittest.TestCase):
-    """
-    NftsOwnershipTokens unit test stubs
-        Refresh vault account tokens  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+class TestUnspentInput(unittest.TestCase):
+    """UnspentInput unit test stubs"""
 
     def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    response_status = 202
-    response_body = ''
+    def make_instance(self, include_optional) -> UnspentInput:
+        """Test UnspentInput
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # uncomment below to create an instance of `UnspentInput`
+        """
+        model = UnspentInput()
+        if include_optional:
+            return UnspentInput(
+                tx_hash = '',
+                index = 1.337
+            )
+        else:
+            return UnspentInput(
+        )
+        """
+
+    def testUnspentInput(self):
+        """Test UnspentInput"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_nfts_ownership_tokens_id_status/test_put.py` & `fireblocks-0.0.2b0/test/test_user_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,59 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import unittest
-from unittest.mock import patch
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import urllib3
 
-import fireblocks_client
-from fireblocks_client.paths.nfts_ownership_tokens_id_status import put  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
+import unittest
 
-from .. import ApiTestMixin
+from fireblocks.models.user_response import UserResponse
 
 
-class TestNftsOwnershipTokensIdStatus(ApiTestMixin, unittest.TestCase):
-    """
-    NftsOwnershipTokensIdStatus unit test stubs
-        Update token ownership status  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+class TestUserResponse(unittest.TestCase):
+    """UserResponse unit test stubs"""
 
     def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    response_status = 200
-    response_body = ''
-
-
+    def make_instance(self, include_optional) -> UserResponse:
+        """Test UserResponse
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # uncomment below to create an instance of `UserResponse`
+        """
+        model = UserResponse()
+        if include_optional:
+            return UserResponse(
+                id = '',
+                first_name = '',
+                last_name = '',
+                role = '',
+                email = '',
+                enabled = True
+            )
+        else:
+            return UserResponse(
+        )
+        """
+
+    def testUserResponse(self):
+        """Test UserResponse"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_nfts_tokens_id/test_put.py` & `fireblocks-0.0.2b0/test/test_rewards_info.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,54 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import unittest
-from unittest.mock import patch
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import urllib3
 
-import fireblocks_client
-from fireblocks_client.paths.nfts_tokens_id import put  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
+import unittest
 
-from .. import ApiTestMixin
+from fireblocks.models.rewards_info import RewardsInfo
 
 
-class TestNftsTokensId(ApiTestMixin, unittest.TestCase):
-    """
-    NftsTokensId unit test stubs
-        Refresh token metadata  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+class TestRewardsInfo(unittest.TestCase):
+    """RewardsInfo unit test stubs"""
 
     def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    response_status = 202
-    response_body = ''
+    def make_instance(self, include_optional) -> RewardsInfo:
+        """Test RewardsInfo
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # uncomment below to create an instance of `RewardsInfo`
+        """
+        model = RewardsInfo()
+        if include_optional:
+            return RewardsInfo(
+                pending_rewards = ''
+            )
+        else:
+            return RewardsInfo(
+        )
+        """
+
+    def testRewardsInfo(self):
+        """Test RewardsInfo"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_off_exchange_settlements_trader/test_post.py` & `fireblocks-0.0.2b0/fireblocks/models/config_change_request_status.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,41 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
-
-import unittest
-from unittest.mock import patch
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import urllib3
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import fireblocks_client
-from fireblocks_client.paths.off_exchange_settlements_trader import post  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
 
-from .. import ApiTestMixin
+from __future__ import annotations
+import json
+from enum import Enum
+from typing_extensions import Self
 
 
-class TestOffExchangeSettlementsTrader(ApiTestMixin, unittest.TestCase):
+class ConfigChangeRequestStatus(str, Enum):
     """
-    OffExchangeSettlementsTrader unit test stubs
-        create settlement for a trader  # noqa: E501
+    ConfigChangeRequestStatus
     """
-    _configuration = configuration.Configuration()
-
-    def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
-
-    def tearDown(self):
-        pass
-
-    response_status = 201
-
 
+    """
+    allowed enum values
+    """
+    WAITING_FOR_APPROVAL = 'WAITING_FOR_APPROVAL'
+    APPROVED = 'APPROVED'
+    CANCELLED = 'CANCELLED'
+    REJECTED = 'REJECTED'
+    FAILED = 'FAILED'
+
+    @classmethod
+    def from_json(cls, json_str: str) -> Self:
+        """Create an instance of ConfigChangeRequestStatus from a JSON string"""
+        return cls(json.loads(json_str))
 
 
-if __name__ == '__main__':
-    unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_off_exchange_settlements_transactions/test_get.py` & `fireblocks-0.0.2b0/fireblocks/models/account_type.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,41 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
-
-import unittest
-from unittest.mock import patch
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import urllib3
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import fireblocks_client
-from fireblocks_client.paths.off_exchange_settlements_transactions import get  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
 
-from .. import ApiTestMixin
+from __future__ import annotations
+import json
+from enum import Enum
+from typing_extensions import Self
 
 
-class TestOffExchangeSettlementsTransactions(ApiTestMixin, unittest.TestCase):
+class AccountType(str, Enum):
     """
-    OffExchangeSettlementsTransactions unit test stubs
-        get settlements transactions from exchange  # noqa: E501
+    AccountType
     """
-    _configuration = configuration.Configuration()
-
-    def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
-
-    def tearDown(self):
-        pass
-
-    response_status = 200
-
 
+    """
+    allowed enum values
+    """
+    EXCHANGE_ACCOUNT = 'EXCHANGE_ACCOUNT'
+    UNMANAGED_WALLET = 'UNMANAGED_WALLET'
+    VAULT_ACCOUNT = 'VAULT_ACCOUNT'
+    NETWORK_CONNECTION = 'NETWORK_CONNECTION'
+    FIAT_ACCOUNT = 'FIAT_ACCOUNT'
+
+    @classmethod
+    def from_json(cls, json_str: str) -> Self:
+        """Create an instance of AccountType from a JSON string"""
+        return cls(json.loads(json_str))
 
 
-if __name__ == '__main__':
-    unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_payments_payout_payout_id_actions_execute/test_post.py` & `fireblocks-0.0.2b0/test/test_payment_account_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,55 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import unittest
-from unittest.mock import patch
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import urllib3
 
-import fireblocks_client
-from fireblocks_client.paths.payments_payout_payout_id_actions_execute import post  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
+import unittest
 
-from .. import ApiTestMixin
+from fireblocks.models.payment_account_response import PaymentAccountResponse
 
 
-class TestPaymentsPayoutPayoutIdActionsExecute(ApiTestMixin, unittest.TestCase):
-    """
-    PaymentsPayoutPayoutIdActionsExecute unit test stubs
-        Execute a payout instruction set  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+class TestPaymentAccountResponse(unittest.TestCase):
+    """PaymentAccountResponse unit test stubs"""
 
     def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    response_status = 200
-
-
+    def make_instance(self, include_optional) -> PaymentAccountResponse:
+        """Test PaymentAccountResponse
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # uncomment below to create an instance of `PaymentAccountResponse`
+        """
+        model = PaymentAccountResponse()
+        if include_optional:
+            return PaymentAccountResponse(
+                id = '',
+                type = 'VAULT_ACCOUNT'
+            )
+        else:
+            return PaymentAccountResponse(
+        )
+        """
+
+    def testPaymentAccountResponse(self):
+        """Test PaymentAccountResponse"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_payments_xb_settlements_configs_config_id/test_get.py` & `fireblocks-0.0.2b0/test/test_payments_payout_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,53 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import unittest
-from unittest.mock import patch
 
-import urllib3
+from fireblocks.api.payments_payout_api import PaymentsPayoutApi
 
-import fireblocks_client
-from fireblocks_client.paths.payments_xb_settlements_configs_config_id import get  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
 
-from .. import ApiTestMixin
+class TestPaymentsPayoutApi(unittest.TestCase):
+    """PaymentsPayoutApi unit test stubs"""
 
+    def setUp(self) -> None:
+        self.api = PaymentsPayoutApi()
 
-class TestPaymentsXbSettlementsConfigsConfigId(ApiTestMixin, unittest.TestCase):
-    """
-    PaymentsXbSettlementsConfigsConfigId unit test stubs
-        Get a specific cross-border settlement configuration  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+    def tearDown(self) -> None:
+        pass
 
-    def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+    def test_create_payout(self) -> None:
+        """Test case for create_payout
 
-    def tearDown(self):
+        Create a payout instruction set
+        """
         pass
 
-    response_status = 200
+    def test_execute_payout_action(self) -> None:
+        """Test case for execute_payout_action
 
+        Execute a payout instruction set
+        """
+        pass
+
+    def test_get_payout(self) -> None:
+        """Test case for get_payout
 
+        Get the status of a payout instruction set
+        """
+        pass
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_payments_xb_settlements_flows/test_post.py` & `fireblocks-0.0.2b0/test/test_wallet_asset.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,60 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import unittest
-from unittest.mock import patch
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import urllib3
 
-import fireblocks_client
-from fireblocks_client.paths.payments_xb_settlements_flows import post  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
+import unittest
 
-from .. import ApiTestMixin
+from fireblocks.models.wallet_asset import WalletAsset
 
 
-class TestPaymentsXbSettlementsFlows(ApiTestMixin, unittest.TestCase):
-    """
-    PaymentsXbSettlementsFlows unit test stubs
-        Create a new cross-border settlement flow  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+class TestWalletAsset(unittest.TestCase):
+    """WalletAsset unit test stubs"""
 
     def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    response_status = 200
-
-
+    def make_instance(self, include_optional) -> WalletAsset:
+        """Test WalletAsset
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # uncomment below to create an instance of `WalletAsset`
+        """
+        model = WalletAsset()
+        if include_optional:
+            return WalletAsset(
+                id = '',
+                balance = '',
+                locked_amount = '',
+                status = 'WAITING_FOR_APPROVAL',
+                address = '',
+                tag = '',
+                activation_time = ''
+            )
+        else:
+            return WalletAsset(
+        )
+        """
+
+    def testWalletAsset(self):
+        """Test WalletAsset"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_payments_xb_settlements_flows_flow_id/test_get.py` & `fireblocks-0.0.2b0/test/test_tokenization_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,67 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import unittest
-from unittest.mock import patch
 
-import urllib3
+from fireblocks.api.tokenization_api import TokenizationApi
 
-import fireblocks_client
-from fireblocks_client.paths.payments_xb_settlements_flows_flow_id import get  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
 
-from .. import ApiTestMixin
+class TestTokenizationApi(unittest.TestCase):
+    """TokenizationApi unit test stubs"""
 
+    def setUp(self) -> None:
+        self.api = TokenizationApi()
 
-class TestPaymentsXbSettlementsFlowsFlowId(ApiTestMixin, unittest.TestCase):
-    """
-    PaymentsXbSettlementsFlowsFlowId unit test stubs
-        Get specific cross-border settlement flow details  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+    def tearDown(self) -> None:
+        pass
 
-    def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+    def test_get_linked_token(self) -> None:
+        """Test case for get_linked_token
 
-    def tearDown(self):
+        Return a linked token
+        """
         pass
 
-    response_status = 200
+    def test_get_linked_tokens(self) -> None:
+        """Test case for get_linked_tokens
 
+        List all linked tokens
+        """
+        pass
+
+    def test_issue_new_token(self) -> None:
+        """Test case for issue_new_token
 
+        Issue a new token
+        """
+        pass
+
+    def test_link(self) -> None:
+        """Test case for link
+
+        Link a token
+        """
+        pass
+
+    def test_unlink(self) -> None:
+        """Test case for unlink
+
+        Unlink a token
+        """
+        pass
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_payments_xb_settlements_flows_flow_id_actions_execute/test_post.py` & `fireblocks-0.0.2b0/test/test_payment_account.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,57 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import unittest
-from unittest.mock import patch
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import urllib3
 
-import fireblocks_client
-from fireblocks_client.paths.payments_xb_settlements_flows_flow_id_actions_execute import post  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
+import unittest
 
-from .. import ApiTestMixin
+from fireblocks.models.payment_account import PaymentAccount
 
 
-class TestPaymentsXbSettlementsFlowsFlowIdActionsExecute(ApiTestMixin, unittest.TestCase):
-    """
-    PaymentsXbSettlementsFlowsFlowIdActionsExecute unit test stubs
-        Execute cross-border settlement flow  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+class TestPaymentAccount(unittest.TestCase):
+    """PaymentAccount unit test stubs"""
 
     def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    response_status = 200
-
-
+    def make_instance(self, include_optional) -> PaymentAccount:
+        """Test PaymentAccount
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # uncomment below to create an instance of `PaymentAccount`
+        """
+        model = PaymentAccount()
+        if include_optional:
+            return PaymentAccount(
+                id = '',
+                type = 'VAULT_ACCOUNT'
+            )
+        else:
+            return PaymentAccount(
+                id = '',
+                type = 'VAULT_ACCOUNT',
+        )
+        """
+
+    def testPaymentAccount(self):
+        """Test PaymentAccount"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_screening_travel_rule_transaction_validate/test_post.py` & `fireblocks-0.0.2b0/test/test_task.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,60 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import unittest
-from unittest.mock import patch
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import urllib3
 
-import fireblocks_client
-from fireblocks_client.paths.screening_travel_rule_transaction_validate import post  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
+import unittest
 
-from .. import ApiTestMixin
+from fireblocks.models.task import Task
 
 
-class TestScreeningTravelRuleTransactionValidate(ApiTestMixin, unittest.TestCase):
-    """
-    ScreeningTravelRuleTransactionValidate unit test stubs
-        Validate Travel Rule Transaction  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+class TestTask(unittest.TestCase):
+    """Task unit test stubs"""
 
     def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    response_status = 200
-
-
-
-
+    def make_instance(self, include_optional) -> Task:
+        """Test Task
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # uncomment below to create an instance of `Task`
+        """
+        model = Task()
+        if include_optional:
+            return Task(
+                id = '',
+                job_id = '',
+                type = '',
+                tenant_id = '',
+                created = 1.337,
+                updated = 1.337,
+                state = ''
+            )
+        else:
+            return Task(
+        )
+        """
+
+    def testTask(self):
+        """Test Task"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_screening_travel_rule_transaction_validate_full/test_post.py` & `fireblocks-0.0.2b0/test/test_create_transaction_response.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,58 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import unittest
-from unittest.mock import patch
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import urllib3
 
-import fireblocks_client
-from fireblocks_client.paths.screening_travel_rule_transaction_validate_full import post  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
+import unittest
 
-from .. import ApiTestMixin
+from fireblocks.models.create_transaction_response import CreateTransactionResponse
 
 
-class TestScreeningTravelRuleTransactionValidateFull(ApiTestMixin, unittest.TestCase):
-    """
-    ScreeningTravelRuleTransactionValidateFull unit test stubs
-        Validate Full Travel Rule Transaction  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+class TestCreateTransactionResponse(unittest.TestCase):
+    """CreateTransactionResponse unit test stubs"""
 
     def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    response_status = 200
-
-
-
-
+    def make_instance(self, include_optional) -> CreateTransactionResponse:
+        """Test CreateTransactionResponse
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # uncomment below to create an instance of `CreateTransactionResponse`
+        """
+        model = CreateTransactionResponse()
+        if include_optional:
+            return CreateTransactionResponse(
+                id = '',
+                status = '',
+                system_messages = fireblocks.models.system_message_info.SystemMessageInfo(
+                    type = 'WARN', 
+                    message = 'Slow transaction processing. Outgoing transactions might be stuck.', )
+            )
+        else:
+            return CreateTransactionResponse(
+        )
+        """
+
+    def testCreateTransactionResponse(self):
+        """Test CreateTransactionResponse"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_screening_travel_rule_vasp_did/test_get.py` & `fireblocks-0.0.2b0/test/test_fiat_asset.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,55 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import unittest
-from unittest.mock import patch
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import urllib3
 
-import fireblocks_client
-from fireblocks_client.paths.screening_travel_rule_vasp_did import get  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
+import unittest
 
-from .. import ApiTestMixin
+from fireblocks.models.fiat_asset import FiatAsset
 
 
-class TestScreeningTravelRuleVaspDid(ApiTestMixin, unittest.TestCase):
-    """
-    ScreeningTravelRuleVaspDid unit test stubs
-        Get VASP details  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+class TestFiatAsset(unittest.TestCase):
+    """FiatAsset unit test stubs"""
 
     def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    response_status = 200
-
-
+    def make_instance(self, include_optional) -> FiatAsset:
+        """Test FiatAsset
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # uncomment below to create an instance of `FiatAsset`
+        """
+        model = FiatAsset()
+        if include_optional:
+            return FiatAsset(
+                id = '',
+                balance = ''
+            )
+        else:
+            return FiatAsset(
+        )
+        """
+
+    def testFiatAsset(self):
+        """Test FiatAsset"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_tap_draft/test_get.py` & `fireblocks-0.0.2b0/fireblocks/models/user_role.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
-
-import unittest
-from unittest.mock import patch
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import urllib3
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import fireblocks_client
-from fireblocks_client.paths.tap_draft import get  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
 
-from .. import ApiTestMixin
+from __future__ import annotations
+import json
+from enum import Enum
+from typing_extensions import Self
 
 
-class TestTapDraft(ApiTestMixin, unittest.TestCase):
+class UserRole(str, Enum):
     """
-    TapDraft unit test stubs
-        Get the active draft  # noqa: E501
+    The role of the user
     """
-    _configuration = configuration.Configuration()
-
-    def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
-
-    def tearDown(self):
-        pass
-
-    response_status = 200
-
 
+    """
+    allowed enum values
+    """
+    OWNER = 'OWNER'
+    ADMIN = 'ADMIN'
+    SIGNER = 'SIGNER'
+    COLLATERALS_SIGNER = 'COLLATERALS_SIGNER'
+    EDITOR = 'EDITOR'
+    APPROVER = 'APPROVER'
+    VIEWER = 'VIEWER'
+    NON_SIGNING_ADMIN = 'NON_SIGNING_ADMIN'
+    AUDITOR = 'AUDITOR'
+    NCW_ADMIN = 'NCW_ADMIN'
+    NCW_SIGNER = 'NCW_SIGNER'
+
+    @classmethod
+    def from_json(cls, json_str: str) -> Self:
+        """Create an instance of UserRole from a JSON string"""
+        return cls(json.loads(json_str))
 
 
-if __name__ == '__main__':
-    unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_tap_draft/test_put.py` & `fireblocks-0.0.2b0/test/test_job_created.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,54 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import unittest
-from unittest.mock import patch
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import urllib3
 
-import fireblocks_client
-from fireblocks_client.paths.tap_draft import put  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
+import unittest
 
-from .. import ApiTestMixin
+from fireblocks.models.job_created import JobCreated
 
 
-class TestTapDraft(ApiTestMixin, unittest.TestCase):
-    """
-    TapDraft unit test stubs
-        Update the draft with a new set of rules  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+class TestJobCreated(unittest.TestCase):
+    """JobCreated unit test stubs"""
 
     def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    response_status = 200
-
-
-
-
+    def make_instance(self, include_optional) -> JobCreated:
+        """Test JobCreated
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # uncomment below to create an instance of `JobCreated`
+        """
+        model = JobCreated()
+        if include_optional:
+            return JobCreated(
+                job_id = ''
+            )
+        else:
+            return JobCreated(
+        )
+        """
+
+    def testJobCreated(self):
+        """Test JobCreated"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_transactions_external_tx_id_external_tx_id_/test_get.py` & `fireblocks-0.0.2b0/test/test_drop_transaction_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,56 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import unittest
-from unittest.mock import patch
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import urllib3
 
-import fireblocks_client
-from fireblocks_client.paths.transactions_external_tx_id_external_tx_id_ import get  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
+import unittest
 
-from .. import ApiTestMixin
+from fireblocks.models.drop_transaction_response import DropTransactionResponse
 
 
-class TestTransactionsExternalTxIdExternalTxId(ApiTestMixin, unittest.TestCase):
-    """
-    TransactionsExternalTxIdExternalTxId unit test stubs
-        Find a specific transaction by external transaction ID  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+class TestDropTransactionResponse(unittest.TestCase):
+    """DropTransactionResponse unit test stubs"""
 
     def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    response_status = 200
-
-
+    def make_instance(self, include_optional) -> DropTransactionResponse:
+        """Test DropTransactionResponse
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # uncomment below to create an instance of `DropTransactionResponse`
+        """
+        model = DropTransactionResponse()
+        if include_optional:
+            return DropTransactionResponse(
+                tx_status = '',
+                tx_id = '',
+                replaced_tx_hash = ''
+            )
+        else:
+            return DropTransactionResponse(
+        )
+        """
+
+    def testDropTransactionResponse(self):
+        """Test DropTransactionResponse"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_transactions_tx_id_unfreeze/test_post.py` & `fireblocks-0.0.2b0/test/test_fiat_accounts_api.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,60 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
 
 import unittest
-from unittest.mock import patch
 
-import urllib3
+from fireblocks.api.fiat_accounts_api import FiatAccountsApi
+
+
+class TestFiatAccountsApi(unittest.TestCase):
+    """FiatAccountsApi unit test stubs"""
 
-import fireblocks_client
-from fireblocks_client.paths.transactions_tx_id_unfreeze import post  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
+    def setUp(self) -> None:
+        self.api = FiatAccountsApi()
 
-from .. import ApiTestMixin
+    def tearDown(self) -> None:
+        pass
 
+    def test_deposit_funds_from_linked_dda(self) -> None:
+        """Test case for deposit_funds_from_linked_dda
 
-class TestTransactionsTxIdUnfreeze(ApiTestMixin, unittest.TestCase):
-    """
-    TransactionsTxIdUnfreeze unit test stubs
-        Unfreeze a transaction  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+        Deposit funds from DDA
+        """
+        pass
 
-    def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+    def test_get_fiat_account(self) -> None:
+        """Test case for get_fiat_account
 
-    def tearDown(self):
+        Find a specific fiat account
+        """
         pass
 
-    response_status = 200
+    def test_get_fiat_accounts(self) -> None:
+        """Test case for get_fiat_accounts
 
+        List fiat accounts
+        """
+        pass
 
+    def test_redeem_funds_to_linked_dda(self) -> None:
+        """Test case for redeem_funds_to_linked_dda
+
+        Redeem funds to DDA
+        """
+        pass
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_transactions_validate_address_asset_id_address/test_get.py` & `fireblocks-0.0.2b0/test/test_account.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,57 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import unittest
-from unittest.mock import patch
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import urllib3
 
-import fireblocks_client
-from fireblocks_client.paths.transactions_validate_address_asset_id_address import get  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
+import unittest
 
-from .. import ApiTestMixin
+from fireblocks.models.account import Account
 
 
-class TestTransactionsValidateAddressAssetIdAddress(ApiTestMixin, unittest.TestCase):
-    """
-    TransactionsValidateAddressAssetIdAddress unit test stubs
-        Validate destination address  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+class TestAccount(unittest.TestCase):
+    """Account unit test stubs"""
 
     def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    response_status = 200
-
-
+    def make_instance(self, include_optional) -> Account:
+        """Test Account
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # uncomment below to create an instance of `Account`
+        """
+        model = Account()
+        if include_optional:
+            return Account(
+                account_id = '',
+                account_type = 'EXCHANGE_ACCOUNT'
+            )
+        else:
+            return Account(
+                account_id = '',
+                account_type = 'EXCHANGE_ACCOUNT',
+        )
+        """
+
+    def testAccount(self):
+        """Test Account"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_asset_id/test_post.py` & `fireblocks-0.0.2b0/test/test_default_network_routing_dest.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,55 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import unittest
-from unittest.mock import patch
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import urllib3
 
-import fireblocks_client
-from fireblocks_client.paths.vault_accounts_vault_account_id_asset_id import post  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
+import unittest
 
-from .. import ApiTestMixin
+from fireblocks.models.default_network_routing_dest import DefaultNetworkRoutingDest
 
 
-class TestVaultAccountsVaultAccountIdAssetId(ApiTestMixin, unittest.TestCase):
-    """
-    VaultAccountsVaultAccountIdAssetId unit test stubs
-        Create a new wallet  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+class TestDefaultNetworkRoutingDest(unittest.TestCase):
+    """DefaultNetworkRoutingDest unit test stubs"""
 
     def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    response_status = 200
-
-
+    def make_instance(self, include_optional) -> DefaultNetworkRoutingDest:
+        """Test DefaultNetworkRoutingDest
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # uncomment below to create an instance of `DefaultNetworkRoutingDest`
+        """
+        model = DefaultNetworkRoutingDest()
+        if include_optional:
+            return DefaultNetworkRoutingDest(
+                scheme = 'DEFAULT'
+            )
+        else:
+            return DefaultNetworkRoutingDest(
+                scheme = 'DEFAULT',
+        )
+        """
+
+    def testDefaultNetworkRoutingDest(self):
+        """Test DefaultNetworkRoutingDest"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_asset_id_addresses/test_get.py` & `fireblocks-0.0.2b0/test/test_cosigner.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,58 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import unittest
-from unittest.mock import patch
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import urllib3
 
-import fireblocks_client
-from fireblocks_client.paths.vault_accounts_vault_account_id_asset_id_addresses import get  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
+import unittest
 
-from .. import ApiTestMixin
+from fireblocks.models.cosigner import Cosigner
 
 
-class TestVaultAccountsVaultAccountIdAssetIdAddresses(ApiTestMixin, unittest.TestCase):
-    """
-    VaultAccountsVaultAccountIdAssetIdAddresses unit test stubs
-        Get asset addresses  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+class TestCosigner(unittest.TestCase):
+    """Cosigner unit test stubs"""
 
     def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    response_status = 200
-
-
+    def make_instance(self, include_optional) -> Cosigner:
+        """Test Cosigner
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # uncomment below to create an instance of `Cosigner`
+        """
+        model = Cosigner()
+        if include_optional:
+            return Cosigner(
+                archived = False,
+                id = '44fcead0-7053-4831-a53a-df7fb90d440f',
+                name = 'My Cosigner 1'
+            )
+        else:
+            return Cosigner(
+                archived = False,
+                id = '44fcead0-7053-4831-a53a-df7fb90d440f',
+        )
+        """
+
+    def testCosigner(self):
+        """Test Cosigner"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_asset_id_addresses/test_post.py` & `fireblocks-0.0.2b0/test/test_transfer_operation_config_params.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,62 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import unittest
-from unittest.mock import patch
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import urllib3
 
-import fireblocks_client
-from fireblocks_client.paths.vault_accounts_vault_account_id_asset_id_addresses import post  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
+import unittest
 
-from .. import ApiTestMixin
+from fireblocks.models.transfer_operation_config_params import (
+    TransferOperationConfigParams,
+)
 
 
-class TestVaultAccountsVaultAccountIdAssetIdAddresses(ApiTestMixin, unittest.TestCase):
-    """
-    VaultAccountsVaultAccountIdAssetIdAddresses unit test stubs
-        Create new asset deposit address  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+class TestTransferOperationConfigParams(unittest.TestCase):
+    """TransferOperationConfigParams unit test stubs"""
 
     def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    response_status = 200
-
-
+    def make_instance(self, include_optional) -> TransferOperationConfigParams:
+        """Test TransferOperationConfigParams
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # uncomment below to create an instance of `TransferOperationConfigParams`
+        """
+        model = TransferOperationConfigParams()
+        if include_optional:
+            return TransferOperationConfigParams(
+                amount = '',
+                asset_id = '',
+                source = fireblocks.models.account.Account(
+                    account_id = '', 
+                    account_type = 'EXCHANGE_ACCOUNT', ),
+                destination = None
+            )
+        else:
+            return TransferOperationConfigParams(
+                destination = None,
+        )
+        """
+
+    def testTransferOperationConfigParams(self):
+        """Test TransferOperationConfigParams"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_asset_id_addresses_address_id/test_put.py` & `fireblocks-0.0.2b0/test/test_transaction_request_amount.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,53 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import unittest
-from unittest.mock import patch
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import urllib3
 
-import fireblocks_client
-from fireblocks_client.paths.vault_accounts_vault_account_id_asset_id_addresses_address_id import put  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
+import unittest
 
-from .. import ApiTestMixin
+from fireblocks.models.transaction_request_amount import TransactionRequestAmount
 
 
-class TestVaultAccountsVaultAccountIdAssetIdAddressesAddressId(ApiTestMixin, unittest.TestCase):
-    """
-    VaultAccountsVaultAccountIdAssetIdAddressesAddressId unit test stubs
-        Update address description  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+class TestTransactionRequestAmount(unittest.TestCase):
+    """TransactionRequestAmount unit test stubs"""
 
     def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    response_status = 201
-    response_body = ''
+    def make_instance(self, include_optional) -> TransactionRequestAmount:
+        """Test TransactionRequestAmount
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # uncomment below to create an instance of `TransactionRequestAmount`
+        """
+        model = TransactionRequestAmount()
+        if include_optional:
+            return TransactionRequestAmount(
+            )
+        else:
+            return TransactionRequestAmount(
+        )
+        """
+
+    def testTransactionRequestAmount(self):
+        """Test TransactionRequestAmount"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fireblocks-0.0.1/test/test_paths/test_vault_accounts_vault_account_id_hide/test_post.py` & `fireblocks-0.0.2b0/test/test_unstake_request_dto.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,58 @@
 # coding: utf-8
 
 """
     Fireblocks API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 
+    The version of the OpenAPI document: 1.6.2
     Contact: support@fireblocks.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import unittest
-from unittest.mock import patch
+    Do not edit the class manually.
+"""  # noqa: E501
 
-import urllib3
 
-import fireblocks_client
-from fireblocks_client.paths.vault_accounts_vault_account_id_hide import post  # noqa: E501
-from fireblocks_client import configuration, schemas, api_client
+import unittest
 
-from .. import ApiTestMixin
+from fireblocks.models.unstake_request_dto import UnstakeRequestDto
 
 
-class TestVaultAccountsVaultAccountIdHide(ApiTestMixin, unittest.TestCase):
-    """
-    VaultAccountsVaultAccountIdHide unit test stubs
-        Hide a vault account in the console  # noqa: E501
-    """
-    _configuration = configuration.Configuration()
+class TestUnstakeRequestDto(unittest.TestCase):
+    """UnstakeRequestDto unit test stubs"""
 
     def setUp(self):
-        used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    response_status = 201
-    response_body = ''
+    def make_instance(self, include_optional) -> UnstakeRequestDto:
+        """Test UnstakeRequestDto
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # uncomment below to create an instance of `UnstakeRequestDto`
+        """
+        model = UnstakeRequestDto()
+        if include_optional:
+            return UnstakeRequestDto(
+                id = 'b70701f4-d7b1-4795-a8ee-b09cdb5b850e',
+                fee = '7',
+                fee_level = 'MEDIUM',
+                tx_note = 'unstake request id b70701f4-d7b1-4795-a8ee-b09cdb5b850d #ETH'
+            )
+        else:
+            return UnstakeRequestDto(
+                id = 'b70701f4-d7b1-4795-a8ee-b09cdb5b850e',
+        )
+        """
+
+    def testUnstakeRequestDto(self):
+        """Test UnstakeRequestDto"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

