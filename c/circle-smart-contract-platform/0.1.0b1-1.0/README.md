# Comparing `tmp/circle_smart_contract_platform-0.1.0b1.tar.gz` & `tmp/circle_smart_contract_platform-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circle_smart_contract_platform-0.1.0b1.tar", last modified: Fri May 24 20:24:56 2024, max compression
+gzip compressed data, was "circle_smart_contract_platform-1.0.tar", last modified: Thu May 30 18:21:20 2024, max compression
```

## Comparing `circle_smart_contract_platform-0.1.0b1.tar` & `circle_smart_contract_platform-1.0.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-24 20:24:56.416221 circle_smart_contract_platform-0.1.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2024-05-24 20:24:56.416221 circle_smart_contract_platform-0.1.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2024-05-24 20:23:22.000000 circle_smart_contract_platform-0.1.0b1/README.md
-drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-24 20:24:56.312221 circle_smart_contract_platform-0.1.0b1/circle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2024-05-24 20:23:22.000000 circle_smart_contract_platform-0.1.0b1/circle/__init__.py
-drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-24 20:24:56.312221 circle_smart_contract_platform-0.1.0b1/circle/web3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2024-05-24 20:23:22.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/__init__.py
-drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-24 20:24:56.316221 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2024-05-24 20:23:22.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/__init__.py
-drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-24 20:24:56.316221 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/api/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2024-05-24 20:23:22.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23270 2024-05-24 20:23:22.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/api/deploy_import_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16133 2024-05-24 20:23:22.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/api/interact_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17405 2024-05-24 20:23:22.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/api/templates_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    31801 2024-05-24 20:23:22.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/api/view_update_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    31579 2024-05-24 20:23:22.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2024-05-24 20:23:23.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/api_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    15107 2024-05-24 20:23:22.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2024-05-24 20:23:22.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/exceptions.py
-drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-24 20:24:56.404221 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2024-05-24 20:23:22.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6093 2024-05-24 20:23:19.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/abi_parameters_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2024-05-24 20:23:20.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/blockchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     8963 2024-05-24 20:23:20.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2024-05-24 20:23:20.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/contract_deployment_estimate_fee_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2024-05-24 20:23:20.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/contract_deployment_estimate_fee_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7146 2024-05-24 20:23:20.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/contract_deployment_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2024-05-24 20:23:20.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/contract_deployment_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2024-05-24 20:23:20.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/contract_input_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2024-05-24 20:23:20.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/contract_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2024-05-24 20:23:20.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/contract_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2024-05-24 20:23:20.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/contracts_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2024-05-24 20:23:20.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/deploy_contract200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2024-05-24 20:23:20.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/deploy_contract_template200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2024-05-24 20:23:20.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/estimate_contract_deploy200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/estimate_contract_template_deploy200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/estimate_deploy_contract_by_template_fee_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/estimate_deploy_contract_by_template_fee_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/estimated_transaction_fee.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/event.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/fee_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/function.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/import_contract200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/import_contract_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/list_contracts200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/patch_contract_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/query_contract200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/read_contract_state_by_id_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/read_contract_state_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/read_contract_state_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/sol_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/template_contract_deployment_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/template_contract_deployment_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/verification_status.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2024-05-24 20:23:22.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12809 2024-05-24 20:23:23.000000 circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/rest.py
-drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-24 20:24:56.416221 circle_smart_contract_platform-0.1.0b1/circle_smart_contract_platform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2024-05-24 20:24:56.000000 circle_smart_contract_platform-0.1.0b1/circle_smart_contract_platform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2024-05-24 20:24:56.000000 circle_smart_contract_platform-0.1.0b1/circle_smart_contract_platform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2024-05-24 20:24:56.000000 circle_smart_contract_platform-0.1.0b1/circle_smart_contract_platform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2024-05-24 20:24:56.000000 circle_smart_contract_platform-0.1.0b1/circle_smart_contract_platform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2024-05-24 20:24:56.000000 circle_smart_contract_platform-0.1.0b1/circle_smart_contract_platform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      794 2024-05-24 20:23:22.000000 circle_smart_contract_platform-0.1.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2024-05-24 20:24:56.416221 circle_smart_contract_platform-0.1.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2024-05-24 20:23:22.000000 circle_smart_contract_platform-0.1.0b1/setup.py
-drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-24 20:24:56.416221 circle_smart_contract_platform-0.1.0b1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2024-05-24 20:23:20.000000 circle_smart_contract_platform-0.1.0b1/test/test_abi_parameters_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2024-05-24 20:23:20.000000 circle_smart_contract_platform-0.1.0b1/test/test_blockchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2024-05-24 20:23:20.000000 circle_smart_contract_platform-0.1.0b1/test/test_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2024-05-24 20:23:20.000000 circle_smart_contract_platform-0.1.0b1/test/test_contract_deployment_estimate_fee_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2024-05-24 20:23:20.000000 circle_smart_contract_platform-0.1.0b1/test/test_contract_deployment_estimate_fee_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2024-05-24 20:23:20.000000 circle_smart_contract_platform-0.1.0b1/test/test_contract_deployment_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2024-05-24 20:23:20.000000 circle_smart_contract_platform-0.1.0b1/test/test_contract_deployment_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2024-05-24 20:23:20.000000 circle_smart_contract_platform-0.1.0b1/test/test_contract_input_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4844 2024-05-24 20:23:20.000000 circle_smart_contract_platform-0.1.0b1/test/test_contract_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2024-05-24 20:23:20.000000 circle_smart_contract_platform-0.1.0b1/test/test_contract_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2024-05-24 20:23:20.000000 circle_smart_contract_platform-0.1.0b1/test/test_contracts_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2024-05-24 20:23:20.000000 circle_smart_contract_platform-0.1.0b1/test/test_deploy_contract200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2024-05-24 20:23:20.000000 circle_smart_contract_platform-0.1.0b1/test/test_deploy_contract_template200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2024-05-24 20:23:22.000000 circle_smart_contract_platform-0.1.0b1/test/test_deploy_import_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2024-05-24 20:23:20.000000 circle_smart_contract_platform-0.1.0b1/test/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/test/test_estimate_contract_deploy200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/test/test_estimate_contract_template_deploy200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/test/test_estimate_deploy_contract_by_template_fee_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/test/test_estimate_deploy_contract_by_template_fee_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/test/test_estimated_transaction_fee.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/test/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/test/test_fee_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/test/test_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     5482 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/test/test_import_contract200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/test/test_import_contract_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2024-05-24 20:23:22.000000 circle_smart_contract_platform-0.1.0b1/test/test_interact_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/test/test_list_contracts200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/test/test_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/test/test_patch_contract_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/test/test_query_contract200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/test/test_read_contract_state_by_id_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/test/test_read_contract_state_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/test/test_read_contract_state_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/test/test_sol_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/test/test_template_contract_deployment_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/test/test_template_contract_deployment_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2024-05-24 20:23:22.000000 circle_smart_contract_platform-0.1.0b1/test/test_templates_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2024-05-24 20:23:21.000000 circle_smart_contract_platform-0.1.0b1/test/test_verification_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2024-05-24 20:23:22.000000 circle_smart_contract_platform-0.1.0b1/test/test_view_update_api.py
+drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-30 18:21:20.077049 circle_smart_contract_platform-1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2024-05-30 18:21:20.077049 circle_smart_contract_platform-1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2024-05-30 18:19:45.000000 circle_smart_contract_platform-1.0/README.md
+drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-30 18:21:19.913049 circle_smart_contract_platform-1.0/circle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2024-05-30 18:19:45.000000 circle_smart_contract_platform-1.0/circle/__init__.py
+drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-30 18:21:19.913049 circle_smart_contract_platform-1.0/circle/web3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2024-05-30 18:19:45.000000 circle_smart_contract_platform-1.0/circle/web3/__init__.py
+drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-30 18:21:19.913049 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2024-05-30 18:19:45.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/__init__.py
+drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-30 18:21:19.913049 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2024-05-30 18:19:45.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23270 2024-05-30 18:19:45.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/api/deploy_import_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16133 2024-05-30 18:19:45.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/api/interact_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17405 2024-05-30 18:19:45.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/api/templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31801 2024-05-30 18:19:45.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/api/view_update_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31575 2024-05-30 18:19:46.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2024-05-30 18:19:46.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15103 2024-05-30 18:19:45.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2024-05-30 18:19:46.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/exceptions.py
+drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-30 18:21:19.981049 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2024-05-30 18:19:45.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6093 2024-05-30 18:19:43.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/abi_parameters_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2024-05-30 18:19:43.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/blockchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8963 2024-05-30 18:19:43.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2024-05-30 18:19:43.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/contract_deployment_estimate_fee_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2024-05-30 18:19:43.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/contract_deployment_estimate_fee_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7146 2024-05-30 18:19:43.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/contract_deployment_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2024-05-30 18:19:43.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/contract_deployment_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2024-05-30 18:19:43.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/contract_input_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2024-05-30 18:19:43.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/contract_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2024-05-30 18:19:43.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/contract_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2024-05-30 18:19:43.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/contracts_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2024-05-30 18:19:43.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/deploy_contract200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2024-05-30 18:19:43.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/deploy_contract_template200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2024-05-30 18:19:43.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2024-05-30 18:19:43.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/estimate_contract_deploy200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2024-05-30 18:19:43.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/estimate_contract_template_deploy200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/estimate_deploy_contract_by_template_fee_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/estimate_deploy_contract_by_template_fee_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/estimated_transaction_fee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/fee_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/import_contract200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/import_contract_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/list_contracts200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/patch_contract_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/query_contract200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/read_contract_state_by_id_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/read_contract_state_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/read_contract_state_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/sol_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/template_contract_deployment_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/template_contract_deployment_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/verification_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2024-05-30 18:19:45.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12809 2024-05-30 18:19:46.000000 circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/rest.py
+drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-30 18:21:20.077049 circle_smart_contract_platform-1.0/circle_smart_contract_platform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2024-05-30 18:21:19.000000 circle_smart_contract_platform-1.0/circle_smart_contract_platform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2024-05-30 18:21:19.000000 circle_smart_contract_platform-1.0/circle_smart_contract_platform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2024-05-30 18:21:19.000000 circle_smart_contract_platform-1.0/circle_smart_contract_platform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2024-05-30 18:21:19.000000 circle_smart_contract_platform-1.0/circle_smart_contract_platform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2024-05-30 18:21:19.000000 circle_smart_contract_platform-1.0/circle_smart_contract_platform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2024-05-30 18:19:45.000000 circle_smart_contract_platform-1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2024-05-30 18:21:20.081049 circle_smart_contract_platform-1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2024-05-30 18:19:45.000000 circle_smart_contract_platform-1.0/setup.py
+drwxr-sr-x   0 runner    (1001) docker     (123)        0 2024-05-30 18:21:20.077049 circle_smart_contract_platform-1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2024-05-30 18:19:43.000000 circle_smart_contract_platform-1.0/test/test_abi_parameters_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2024-05-30 18:19:43.000000 circle_smart_contract_platform-1.0/test/test_blockchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2024-05-30 18:19:43.000000 circle_smart_contract_platform-1.0/test/test_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2024-05-30 18:19:43.000000 circle_smart_contract_platform-1.0/test/test_contract_deployment_estimate_fee_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2024-05-30 18:19:43.000000 circle_smart_contract_platform-1.0/test/test_contract_deployment_estimate_fee_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2024-05-30 18:19:43.000000 circle_smart_contract_platform-1.0/test/test_contract_deployment_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2024-05-30 18:19:43.000000 circle_smart_contract_platform-1.0/test/test_contract_deployment_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2024-05-30 18:19:43.000000 circle_smart_contract_platform-1.0/test/test_contract_input_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2024-05-30 18:19:43.000000 circle_smart_contract_platform-1.0/test/test_contract_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2024-05-30 18:19:43.000000 circle_smart_contract_platform-1.0/test/test_contract_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2024-05-30 18:19:43.000000 circle_smart_contract_platform-1.0/test/test_contracts_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2024-05-30 18:19:43.000000 circle_smart_contract_platform-1.0/test/test_deploy_contract200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2024-05-30 18:19:43.000000 circle_smart_contract_platform-1.0/test/test_deploy_contract_template200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2024-05-30 18:19:45.000000 circle_smart_contract_platform-1.0/test/test_deploy_import_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2024-05-30 18:19:43.000000 circle_smart_contract_platform-1.0/test/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2024-05-30 18:19:43.000000 circle_smart_contract_platform-1.0/test/test_estimate_contract_deploy200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/test/test_estimate_contract_template_deploy200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/test/test_estimate_deploy_contract_by_template_fee_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/test/test_estimate_deploy_contract_by_template_fee_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/test/test_estimated_transaction_fee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/test/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/test/test_fee_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/test/test_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/test/test_import_contract200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/test/test_import_contract_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2024-05-30 18:19:45.000000 circle_smart_contract_platform-1.0/test/test_interact_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/test/test_list_contracts200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/test/test_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/test/test_patch_contract_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/test/test_query_contract200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/test/test_read_contract_state_by_id_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/test/test_read_contract_state_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/test/test_read_contract_state_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/test/test_sol_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/test/test_template_contract_deployment_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/test/test_template_contract_deployment_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2024-05-30 18:19:45.000000 circle_smart_contract_platform-1.0/test/test_templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2024-05-30 18:19:44.000000 circle_smart_contract_platform-1.0/test/test_verification_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2024-05-30 18:19:45.000000 circle_smart_contract_platform-1.0/test/test_view_update_api.py
```

### Comparing `circle_smart_contract_platform-0.1.0b1/PKG-INFO` & `circle_smart_contract_platform-1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: circle-smart-contract-platform
-Version: 0.1.0b1
+Version: 1.0
 Summary: Smart Contract Platform
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: team@openapitools.org
 Keywords: OpenAPI,OpenAPI-Generator,Smart Contract Platform
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
 
 # circle-smart-contract-platform
 This is the Smart Contract Platform API documentation.
 
 - API version: 1.0
-- Package version: 0.1.0b1
+- Package version: 1.0
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation
 ### pip install
```

### Comparing `circle_smart_contract_platform-0.1.0b1/README.md` & `circle_smart_contract_platform-1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # circle-smart-contract-platform
 This is the Smart Contract Platform API documentation.
 
 - API version: 1.0
-- Package version: 0.1.0b1
+- Package version: 1.0
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation
 ### pip install
```

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/__init__.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/__init__.py`

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
 from circle.web3.smart_contract_platform.api.deploy_import_api import DeployImportApi
 from circle.web3.smart_contract_platform.api.interact_api import InteractApi
 from circle.web3.smart_contract_platform.api.templates_api import TemplatesApi
 from circle.web3.smart_contract_platform.api.view_update_api import ViewUpdateApi
```

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/api/deploy_import_api.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/api/deploy_import_api.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/api/interact_api.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/api/interact_api.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/api/templates_api.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/api/templates_api.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/api/view_update_api.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/api/view_update_api.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/api_client.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = (user_agent + ' / ' if user_agent else '') + 'CircleWeb3PythonSDK / SmartContractPlatform / 0.1.0b1'
+        self.user_agent = (user_agent + ' / ' if user_agent else '') + 'CircleWeb3PythonSDK / SmartContractPlatform / 1.0'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/api_response.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/api_response.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/configuration.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/configuration.py`

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

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/exceptions.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/exceptions.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/__init__.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/__init__.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/abi_parameters_inner.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/abi_parameters_inner.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/blockchain.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/blockchain.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/contract.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/contract.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/contract_deployment_estimate_fee_request.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/contract_deployment_estimate_fee_request.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/contract_deployment_estimate_fee_response.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/contract_deployment_estimate_fee_response.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/contract_deployment_request.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/contract_deployment_request.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/contract_deployment_response.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/contract_deployment_response.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/contract_input_type.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/contract_input_type.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/contract_response.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/contract_response.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/contract_status.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/contract_status.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/contracts_response.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/contracts_response.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/deploy_contract200_response.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/deploy_contract200_response.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/deploy_contract_template200_response.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/deploy_contract_template200_response.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/error.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/error.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/estimate_contract_deploy200_response.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/estimate_contract_deploy200_response.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/estimate_contract_template_deploy200_response.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/estimate_contract_template_deploy200_response.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/estimate_deploy_contract_by_template_fee_request.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/estimate_deploy_contract_by_template_fee_request.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/estimate_deploy_contract_by_template_fee_response.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/estimate_deploy_contract_by_template_fee_response.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/estimated_transaction_fee.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/estimated_transaction_fee.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/event.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/event.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/fee_level.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/fee_level.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/function.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/function.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/import_contract200_response.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/import_contract200_response.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/import_contract_request.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/import_contract_request.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/list_contracts200_response.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/list_contracts200_response.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/param_type.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/param_type.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/patch_contract_request.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/patch_contract_request.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/query_contract200_response.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/query_contract200_response.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/read_contract_state_by_id_request.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/read_contract_state_by_id_request.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/read_contract_state_request.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/read_contract_state_request.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/read_contract_state_response.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/read_contract_state_response.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/sol_file.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/sol_file.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/template_contract_deployment_request.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/template_contract_deployment_request.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/template_contract_deployment_response.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/template_contract_deployment_response.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/models/verification_status.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/models/verification_status.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle/web3/smart_contract_platform/rest.py` & `circle_smart_contract_platform-1.0/circle/web3/smart_contract_platform/rest.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/circle_smart_contract_platform.egg-info/PKG-INFO` & `circle_smart_contract_platform-1.0/circle_smart_contract_platform.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: circle-smart-contract-platform
-Version: 0.1.0b1
+Version: 1.0
 Summary: Smart Contract Platform
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: team@openapitools.org
 Keywords: OpenAPI,OpenAPI-Generator,Smart Contract Platform
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
 
 # circle-smart-contract-platform
 This is the Smart Contract Platform API documentation.
 
 - API version: 1.0
-- Package version: 0.1.0b1
+- Package version: 1.0
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation
 ### pip install
```

### Comparing `circle_smart_contract_platform-0.1.0b1/circle_smart_contract_platform.egg-info/SOURCES.txt` & `circle_smart_contract_platform-1.0/circle_smart_contract_platform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/pyproject.toml` & `circle_smart_contract_platform-1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "circle.web3.smart_contract_platform"
-version = "0.1.0b1"
+version = "1.0"
 description = "Smart Contract Platform"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Smart Contract Platform"]
 include = ["circle.web3.smart_contract_platform/py.typed"]
```

### Comparing `circle_smart_contract_platform-0.1.0b1/setup.py` & `circle_smart_contract_platform-1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "circle-smart-contract-platform"
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

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_abi_parameters_inner.py` & `circle_smart_contract_platform-1.0/test/test_abi_parameters_inner.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_blockchain.py` & `circle_smart_contract_platform-1.0/test/test_blockchain.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_contract.py` & `circle_smart_contract_platform-1.0/test/test_contract.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_contract_deployment_estimate_fee_request.py` & `circle_smart_contract_platform-1.0/test/test_contract_deployment_estimate_fee_request.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_contract_deployment_estimate_fee_response.py` & `circle_smart_contract_platform-1.0/test/test_contract_deployment_estimate_fee_response.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_contract_deployment_request.py` & `circle_smart_contract_platform-1.0/test/test_contract_deployment_request.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_contract_deployment_response.py` & `circle_smart_contract_platform-1.0/test/test_contract_deployment_response.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_contract_input_type.py` & `circle_smart_contract_platform-1.0/test/test_contract_input_type.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_contract_response.py` & `circle_smart_contract_platform-1.0/test/test_contract_response.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_contract_status.py` & `circle_smart_contract_platform-1.0/test/test_contract_status.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_contracts_response.py` & `circle_smart_contract_platform-1.0/test/test_contracts_response.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_deploy_contract200_response.py` & `circle_smart_contract_platform-1.0/test/test_deploy_contract200_response.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_deploy_contract_template200_response.py` & `circle_smart_contract_platform-1.0/test/test_deploy_contract_template200_response.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_deploy_import_api.py` & `circle_smart_contract_platform-1.0/test/test_deploy_import_api.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_error.py` & `circle_smart_contract_platform-1.0/test/test_error.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_estimate_contract_deploy200_response.py` & `circle_smart_contract_platform-1.0/test/test_estimate_contract_deploy200_response.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_estimate_contract_template_deploy200_response.py` & `circle_smart_contract_platform-1.0/test/test_estimate_contract_template_deploy200_response.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_estimate_deploy_contract_by_template_fee_request.py` & `circle_smart_contract_platform-1.0/test/test_estimate_deploy_contract_by_template_fee_request.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_estimate_deploy_contract_by_template_fee_response.py` & `circle_smart_contract_platform-1.0/test/test_estimate_deploy_contract_by_template_fee_response.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_estimated_transaction_fee.py` & `circle_smart_contract_platform-1.0/test/test_estimated_transaction_fee.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_event.py` & `circle_smart_contract_platform-1.0/test/test_event.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_fee_level.py` & `circle_smart_contract_platform-1.0/test/test_fee_level.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_function.py` & `circle_smart_contract_platform-1.0/test/test_function.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_import_contract200_response.py` & `circle_smart_contract_platform-1.0/test/test_import_contract200_response.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_import_contract_request.py` & `circle_smart_contract_platform-1.0/test/test_import_contract_request.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_interact_api.py` & `circle_smart_contract_platform-1.0/test/test_interact_api.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_list_contracts200_response.py` & `circle_smart_contract_platform-1.0/test/test_list_contracts200_response.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_param_type.py` & `circle_smart_contract_platform-1.0/test/test_param_type.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_patch_contract_request.py` & `circle_smart_contract_platform-1.0/test/test_patch_contract_request.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_query_contract200_response.py` & `circle_smart_contract_platform-1.0/test/test_query_contract200_response.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_read_contract_state_by_id_request.py` & `circle_smart_contract_platform-1.0/test/test_read_contract_state_by_id_request.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_read_contract_state_request.py` & `circle_smart_contract_platform-1.0/test/test_read_contract_state_request.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_read_contract_state_response.py` & `circle_smart_contract_platform-1.0/test/test_read_contract_state_response.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_sol_file.py` & `circle_smart_contract_platform-1.0/test/test_sol_file.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_template_contract_deployment_request.py` & `circle_smart_contract_platform-1.0/test/test_template_contract_deployment_request.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_template_contract_deployment_response.py` & `circle_smart_contract_platform-1.0/test/test_template_contract_deployment_response.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_templates_api.py` & `circle_smart_contract_platform-1.0/test/test_templates_api.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_verification_status.py` & `circle_smart_contract_platform-1.0/test/test_verification_status.py`

 * *Files identical despite different names*

### Comparing `circle_smart_contract_platform-0.1.0b1/test/test_view_update_api.py` & `circle_smart_contract_platform-1.0/test/test_view_update_api.py`

 * *Files identical despite different names*

