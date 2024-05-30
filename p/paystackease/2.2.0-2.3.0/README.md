# Comparing `tmp/paystackease-2.2.0.tar.gz` & `tmp/paystackease-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paystackease-2.2.0.tar", max compression
+gzip compressed data, was "paystackease-2.3.0.tar", max compression
```

## Comparing `paystackease-2.2.0.tar` & `paystackease-2.3.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0     1069 2024-05-28 02:58:06.877679 paystackease-2.2.0/LICENSE
--rw-r--r--   0        0        0     4802 2024-05-28 02:58:06.877679 paystackease-2.2.0/README.md
--rw-r--r--   0        0        0     1767 2024-05-28 02:58:06.881679 paystackease-2.2.0/paystackease/__init__.py
--rw-r--r--   0        0        0     4841 2024-05-28 02:58:06.881679 paystackease-2.2.0/paystackease/apaystack.py
--rw-r--r--   0        0        0      988 2024-05-28 02:58:06.881679 paystackease-2.2.0/paystackease/apis/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 02:58:06.881679 paystackease-2.2.0/paystackease/apis/async_apis/__init__.py
--rw-r--r--   0        0        0     2137 2024-05-28 02:58:06.881679 paystackease-2.2.0/paystackease/apis/async_apis/aapple_pay.py
--rw-r--r--   0        0        0     4355 2024-05-28 02:58:06.881679 paystackease-2.2.0/paystackease/apis/async_apis/abulk_charges.py
--rw-r--r--   0        0        0     5820 2024-05-28 02:58:06.881679 paystackease-2.2.0/paystackease/apis/async_apis/acharges.py
--rw-r--r--   0        0        0     6762 2024-05-28 02:58:06.881679 paystackease-2.2.0/paystackease/apis/async_apis/acustomers.py
--rw-r--r--   0        0        0     9269 2024-05-28 02:58:06.881679 paystackease-2.2.0/paystackease/apis/async_apis/adedicated_virtual_accounts.py
--rw-r--r--   0        0        0     7980 2024-05-28 02:58:06.881679 paystackease-2.2.0/paystackease/apis/async_apis/adisputes.py
--rw-r--r--   0        0        0     1146 2024-05-28 02:58:06.881679 paystackease-2.2.0/paystackease/apis/async_apis/aintegration.py
--rw-r--r--   0        0        0     4327 2024-05-28 02:58:06.881679 paystackease-2.2.0/paystackease/apis/async_apis/amiscellaneous.py
--rw-r--r--   0        0        0     5644 2024-05-28 02:58:06.881679 paystackease-2.2.0/paystackease/apis/async_apis/apayment_pages.py
--rw-r--r--   0        0        0     9834 2024-05-28 02:58:06.881679 paystackease-2.2.0/paystackease/apis/async_apis/apayment_requests.py
--rw-r--r--   0        0        0     4547 2024-05-28 02:58:06.881679 paystackease-2.2.0/paystackease/apis/async_apis/aplans.py
--rw-r--r--   0        0        0     4253 2024-05-28 02:58:06.881679 paystackease-2.2.0/paystackease/apis/async_apis/aproducts.py
--rw-r--r--   0        0        0     3233 2024-05-28 02:58:06.881679 paystackease-2.2.0/paystackease/apis/async_apis/arefund.py
--rw-r--r--   0        0        0     3250 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/async_apis/asettlements.py
--rw-r--r--   0        0        0     6232 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/async_apis/asubaccounts.py
--rw-r--r--   0        0        0     4396 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/async_apis/asubscriptions.py
--rw-r--r--   0        0        0     5399 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/async_apis/aterminal.py
--rw-r--r--   0        0        0     5844 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/async_apis/atransaction_splits.py
--rw-r--r--   0        0        0    12559 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/async_apis/atransactions.py
--rw-r--r--   0        0        0     5281 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/async_apis/atransfer_recipients.py
--rw-r--r--   0        0        0     4822 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/async_apis/atransfers.py
--rw-r--r--   0        0        0     2717 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/async_apis/atransfers_control.py
--rw-r--r--   0        0        0     2802 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/async_apis/averification.py
--rw-r--r--   0        0        0        0 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/__init__.py
--rw-r--r--   0        0        0     2084 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/apple_pay.py
--rw-r--r--   0        0        0     4263 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/bulk_charges.py
--rw-r--r--   0        0        0     5724 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/charges.py
--rw-r--r--   0        0        0     6663 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/customers.py
--rw-r--r--   0        0        0     9141 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/dedicated_virtual_accounts.py
--rw-r--r--   0        0        0     7864 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/disputes.py
--rw-r--r--   0        0        0     1110 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/integration.py
--rw-r--r--   0        0        0     4283 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/miscellaneous.py
--rw-r--r--   0        0        0     5560 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/payment_pages.py
--rw-r--r--   0        0        0     9706 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/payment_requests.py
--rw-r--r--   0        0        0     4479 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/plans.py
--rw-r--r--   0        0        0     4185 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/products.py
--rw-r--r--   0        0        0     3177 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/refund.py
--rw-r--r--   0        0        0     3214 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/settlements.py
--rw-r--r--   0        0        0     6158 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/subaccounts.py
--rw-r--r--   0        0        0     4305 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/subscriptions.py
--rw-r--r--   0        0        0     5285 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/terminal.py
--rw-r--r--   0        0        0     5747 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/transaction_splits.py
--rw-r--r--   0        0        0    12421 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/transactions.py
--rw-r--r--   0        0        0     5189 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/transfer_recipients.py
--rw-r--r--   0        0        0     4730 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/transfers.py
--rw-r--r--   0        0        0     2625 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/transfers_control.py
--rw-r--r--   0        0        0     2746 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/apis/sync_apis/verification.py
--rw-r--r--   0        0        0      730 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/core/__init__.py
--rw-r--r--   0        0        0     3101 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/core/_api_base.py
--rw-r--r--   0        0        0     6808 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/core/_api_base_client.py
--rw-r--r--   0        0        0     4680 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/core/_api_client_requests.py
--rw-r--r--   0        0        0      660 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/core/_api_client_response.py
--rw-r--r--   0        0        0      873 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/core/_api_env.py
--rw-r--r--   0        0        0     5007 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/core/_api_errors.py
--rw-r--r--   0        0        0     1968 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/core/_events.py
--rw-r--r--   0        0        0     1547 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/core/_webhook.py
--rw-r--r--   0        0        0      552 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/helpers/__init__.py
--rw-r--r--   0        0        0      742 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/helpers/convert.py
--rw-r--r--   0        0        0     3566 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/helpers/tool_kit.py
--rw-r--r--   0        0        0        0 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/metadata/__init__.py
--rw-r--r--   0        0        0       98 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/metadata/__version__.py
--rw-r--r--   0        0        0     2334 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/paystack.py
--rw-r--r--   0        0        0        0 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/utils/__init__.py
--rw-r--r--   0        0        0      193 2024-05-28 02:58:06.885679 paystackease-2.2.0/paystackease/utils/_compact.py
--rw-r--r--   0        0        0     2259 2024-05-28 02:58:08.457671 paystackease-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     6151 1970-01-01 00:00:00.000000 paystackease-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-30 14:19:43.034883 paystackease-2.3.0/LICENSE
+-rw-r--r--   0        0        0     4802 2024-05-30 14:19:43.034883 paystackease-2.3.0/README.md
+-rw-r--r--   0        0        0     1767 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/__init__.py
+-rw-r--r--   0        0        0     4841 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apaystack.py
+-rw-r--r--   0        0        0      988 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apis/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apis/async_apis/__init__.py
+-rw-r--r--   0        0        0     2137 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apis/async_apis/aapple_pay.py
+-rw-r--r--   0        0        0     4355 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apis/async_apis/abulk_charges.py
+-rw-r--r--   0        0        0     5820 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apis/async_apis/acharges.py
+-rw-r--r--   0        0        0     6762 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apis/async_apis/acustomers.py
+-rw-r--r--   0        0        0     9269 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apis/async_apis/adedicated_virtual_accounts.py
+-rw-r--r--   0        0        0     7980 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apis/async_apis/adisputes.py
+-rw-r--r--   0        0        0     1146 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apis/async_apis/aintegration.py
+-rw-r--r--   0        0        0     4332 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apis/async_apis/amiscellaneous.py
+-rw-r--r--   0        0        0     5644 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apis/async_apis/apayment_pages.py
+-rw-r--r--   0        0        0     9461 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apis/async_apis/apayment_requests.py
+-rw-r--r--   0        0        0     4259 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apis/async_apis/aplans.py
+-rw-r--r--   0        0        0     4075 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apis/async_apis/aproducts.py
+-rw-r--r--   0        0        0     3233 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apis/async_apis/arefund.py
+-rw-r--r--   0        0        0     3250 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apis/async_apis/asettlements.py
+-rw-r--r--   0        0        0     6232 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apis/async_apis/asubaccounts.py
+-rw-r--r--   0        0        0     4396 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apis/async_apis/asubscriptions.py
+-rw-r--r--   0        0        0     5399 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apis/async_apis/aterminal.py
+-rw-r--r--   0        0        0     5844 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apis/async_apis/atransaction_splits.py
+-rw-r--r--   0        0        0    12559 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apis/async_apis/atransactions.py
+-rw-r--r--   0        0        0     5281 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apis/async_apis/atransfer_recipients.py
+-rw-r--r--   0        0        0     4822 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apis/async_apis/atransfers.py
+-rw-r--r--   0        0        0     2717 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apis/async_apis/atransfers_control.py
+-rw-r--r--   0        0        0     2802 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apis/async_apis/averification.py
+-rw-r--r--   0        0        0        0 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apis/sync_apis/__init__.py
+-rw-r--r--   0        0        0     2084 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apis/sync_apis/apple_pay.py
+-rw-r--r--   0        0        0     4263 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apis/sync_apis/bulk_charges.py
+-rw-r--r--   0        0        0     5724 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apis/sync_apis/charges.py
+-rw-r--r--   0        0        0     6663 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apis/sync_apis/customers.py
+-rw-r--r--   0        0        0     9141 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apis/sync_apis/dedicated_virtual_accounts.py
+-rw-r--r--   0        0        0     7864 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apis/sync_apis/disputes.py
+-rw-r--r--   0        0        0     1110 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apis/sync_apis/integration.py
+-rw-r--r--   0        0        0     4288 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apis/sync_apis/miscellaneous.py
+-rw-r--r--   0        0        0     5560 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apis/sync_apis/payment_pages.py
+-rw-r--r--   0        0        0     9333 2024-05-30 14:19:43.038883 paystackease-2.3.0/paystackease/apis/sync_apis/payment_requests.py
+-rw-r--r--   0        0        0     4191 2024-05-30 14:19:43.042883 paystackease-2.3.0/paystackease/apis/sync_apis/plans.py
+-rw-r--r--   0        0        0     4007 2024-05-30 14:19:43.042883 paystackease-2.3.0/paystackease/apis/sync_apis/products.py
+-rw-r--r--   0        0        0     3177 2024-05-30 14:19:43.042883 paystackease-2.3.0/paystackease/apis/sync_apis/refund.py
+-rw-r--r--   0        0        0     3214 2024-05-30 14:19:43.042883 paystackease-2.3.0/paystackease/apis/sync_apis/settlements.py
+-rw-r--r--   0        0        0     6158 2024-05-30 14:19:43.042883 paystackease-2.3.0/paystackease/apis/sync_apis/subaccounts.py
+-rw-r--r--   0        0        0     4305 2024-05-30 14:19:43.042883 paystackease-2.3.0/paystackease/apis/sync_apis/subscriptions.py
+-rw-r--r--   0        0        0     5285 2024-05-30 14:19:43.042883 paystackease-2.3.0/paystackease/apis/sync_apis/terminal.py
+-rw-r--r--   0        0        0     5747 2024-05-30 14:19:43.042883 paystackease-2.3.0/paystackease/apis/sync_apis/transaction_splits.py
+-rw-r--r--   0        0        0    12421 2024-05-30 14:19:43.042883 paystackease-2.3.0/paystackease/apis/sync_apis/transactions.py
+-rw-r--r--   0        0        0     5189 2024-05-30 14:19:43.042883 paystackease-2.3.0/paystackease/apis/sync_apis/transfer_recipients.py
+-rw-r--r--   0        0        0     4730 2024-05-30 14:19:43.042883 paystackease-2.3.0/paystackease/apis/sync_apis/transfers.py
+-rw-r--r--   0        0        0     2625 2024-05-30 14:19:43.042883 paystackease-2.3.0/paystackease/apis/sync_apis/transfers_control.py
+-rw-r--r--   0        0        0     2746 2024-05-30 14:19:43.042883 paystackease-2.3.0/paystackease/apis/sync_apis/verification.py
+-rw-r--r--   0        0        0      730 2024-05-30 14:19:43.042883 paystackease-2.3.0/paystackease/core/__init__.py
+-rw-r--r--   0        0        0     3109 2024-05-30 14:19:43.042883 paystackease-2.3.0/paystackease/core/_api_base.py
+-rw-r--r--   0        0        0     6842 2024-05-30 14:19:43.042883 paystackease-2.3.0/paystackease/core/_api_base_client.py
+-rw-r--r--   0        0        0     4680 2024-05-30 14:19:43.042883 paystackease-2.3.0/paystackease/core/_api_client_requests.py
+-rw-r--r--   0        0        0      929 2024-05-30 14:19:43.042883 paystackease-2.3.0/paystackease/core/_api_client_response.py
+-rw-r--r--   0        0        0      873 2024-05-30 14:19:43.042883 paystackease-2.3.0/paystackease/core/_api_env.py
+-rw-r--r--   0        0        0     5007 2024-05-30 14:19:43.042883 paystackease-2.3.0/paystackease/core/_api_errors.py
+-rw-r--r--   0        0        0     1968 2024-05-30 14:19:43.042883 paystackease-2.3.0/paystackease/core/_events.py
+-rw-r--r--   0        0        0     1547 2024-05-30 14:19:43.042883 paystackease-2.3.0/paystackease/core/_webhook.py
+-rw-r--r--   0        0        0      552 2024-05-30 14:19:43.042883 paystackease-2.3.0/paystackease/helpers/__init__.py
+-rw-r--r--   0        0        0      742 2024-05-30 14:19:43.042883 paystackease-2.3.0/paystackease/helpers/convert.py
+-rw-r--r--   0        0        0     3566 2024-05-30 14:19:43.042883 paystackease-2.3.0/paystackease/helpers/tool_kit.py
+-rw-r--r--   0        0        0        0 2024-05-30 14:19:43.042883 paystackease-2.3.0/paystackease/metadata/__init__.py
+-rw-r--r--   0        0        0       98 2024-05-30 14:19:43.042883 paystackease-2.3.0/paystackease/metadata/__version__.py
+-rw-r--r--   0        0        0     2334 2024-05-30 14:19:43.042883 paystackease-2.3.0/paystackease/paystack.py
+-rw-r--r--   0        0        0        0 2024-05-30 14:19:43.042883 paystackease-2.3.0/paystackease/utils/__init__.py
+-rw-r--r--   0        0        0      193 2024-05-30 14:19:43.042883 paystackease-2.3.0/paystackease/utils/_compact.py
+-rw-r--r--   0        0        0     2259 2024-05-30 14:19:44.802893 paystackease-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6151 1970-01-01 00:00:00.000000 paystackease-2.3.0/PKG-INFO
```

### Comparing `paystackease-2.2.0/LICENSE` & `paystackease-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/README.md` & `paystackease-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/__init__.py` & `paystackease-2.3.0/paystackease/__init__.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apaystack.py` & `paystackease-2.3.0/paystackease/apaystack.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/__init__.py` & `paystackease-2.3.0/paystackease/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/async_apis/aapple_pay.py` & `paystackease-2.3.0/paystackease/apis/async_apis/aapple_pay.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/async_apis/abulk_charges.py` & `paystackease-2.3.0/paystackease/apis/async_apis/abulk_charges.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/async_apis/acharges.py` & `paystackease-2.3.0/paystackease/apis/async_apis/acharges.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/async_apis/acustomers.py` & `paystackease-2.3.0/paystackease/apis/async_apis/acustomers.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/async_apis/adedicated_virtual_accounts.py` & `paystackease-2.3.0/paystackease/apis/async_apis/adedicated_virtual_accounts.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/async_apis/adisputes.py` & `paystackease-2.3.0/paystackease/apis/async_apis/adisputes.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/async_apis/aintegration.py` & `paystackease-2.3.0/paystackease/apis/async_apis/aintegration.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/async_apis/amiscellaneous.py` & `paystackease-2.3.0/paystackease/apis/async_apis/amiscellaneous.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         pay_with_bank = self._convert_to_string(pay_with_bank)
         enabled_for_verification = self._convert_to_string(enabled_for_verification)
 
         params = {
             "country": country,
             "use_cursor": use_cursor,
             "perPage": per_page,
-            "supports_transfer": pay_with_bank_transfer,
+            "pay_with_bank_transfer": pay_with_bank_transfer,
             "pay_with_bank": pay_with_bank,
             "enabled_for_verification": enabled_for_verification,
             "next": next_cursor,
             "previous": previous_cursor,
             "gateway": gateway,
             "type": channel_type,
             "currency": currency,
```

### Comparing `paystackease-2.2.0/paystackease/apis/async_apis/apayment_pages.py` & `paystackease-2.3.0/paystackease/apis/async_apis/apayment_pages.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/async_apis/apayment_requests.py` & `paystackease-2.3.0/paystackease/apis/async_apis/apayment_requests.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,17 +17,17 @@
     Reference: https://paystack.com/docs/api/payment-request/
     """
 
     async def create_payment_request(
             self,
             customer: str,
             amount: int,
-            draft: bool,
-            has_invoice: bool,
-            send_notification: bool,
+            draft: bool = False,
+            has_invoice: bool = True,
+            send_notification: bool = True,
             due_date: Optional[Union[date, None]] = None,
             description: Optional[Union[str, Any]] = None,
             line_items: Optional[Union[List[Dict[str, Any]], None]] = None,
             tax: Optional[Union[List[Dict[str, Any]], None]] = None,
             currency: Optional[Union[Currency, Any]] = None,
             invoice_number: Optional[Union[int, Any]] = None,
             split_code: Optional[Union[str, Any]] = None,
@@ -49,17 +49,14 @@
         :param: split_code: split code of the transaction split
 
         :return: The PayStackResponse from the API
         :rtype: PayStackResponse object
         """
         # convert date and bool to string
         due_date = self._convert_to_string(due_date)
-        draft = self._convert_to_string(draft)
-        has_invoice = self._convert_to_string(has_invoice)
-        send_notification = self._convert_to_string(send_notification)
 
         data = {
             "customer": customer,
             "amount": amount,
             "due_date": due_date,
             "description": description,
             "line_items": line_items,
@@ -165,16 +162,14 @@
 
         :param: code: Payment request code
         :param: send_notification: Set true if you want to send a notification to the customer email
 
         :return: The PayStackResponse from the API
         :rtype: PayStackResponse object
         """
-        # convert to strings
-        send_notification = self._convert_to_string(send_notification)
 
         data = {"send_notification": send_notification}
         return await self._post_request(f"/paymentrequest/finalize/{code}", data=data)
 
     async def update_payment_request(
             self,
             id_or_code: str,
@@ -208,16 +203,14 @@
 
         :return: The PayStackResponse from the API
         :rtype: PayStackResponse object
         """
 
         # convert date and bool to string
         due_date = self._convert_to_string(due_date)
-        draft = self._convert_to_string(draft)
-        send_notification = self._convert_to_string(send_notification)
 
         data = {
             "customer": customer,
             "amount": amount,
             "due_date": due_date,
             "description": description,
             "line_items": line_items,
```

### Comparing `paystackease-2.2.0/paystackease/apis/async_apis/aplans.py` & `paystackease-2.3.0/paystackease/apis/async_apis/aplans.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,18 +38,14 @@
         :param: send_sms: Send SMS to customer
         :param: currency: Currency of the plan
         :param: invoice_limit: Invoice limit of the plan
 
         :return: The PayStackResponse from the API
         :rtype: PayStackResponse object
         """
-        # convert to strings
-        send_invoices = self._convert_to_string(send_invoices)
-        send_sms = self._convert_to_string(send_sms)
-
         data = {
             "name": name,
             "amount": amount,
             "interval": interval,
             "description": description,
             "send_invoices": send_invoices,
             "send_sms": send_sms,
@@ -58,15 +54,15 @@
         }
         return await self._post_request("/plan", data=data)
 
     async def list_plans(
             self,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
-            status: Optional[Union[str, None]] = None,
+            status: Optional[Union[str, None]] = 'active',
             interval: Optional[Union[Interval, None]] = None,
             amount: Optional[Union[int, None]] = None,
     ) -> PayStackResponse:
         """
         List all the plans
 
         :param: per_page: Number of records to return
@@ -122,18 +118,14 @@
         :param: send_sms:
         :param: currency:
         :param: invoice_limit:
 
         :return: The PayStackResponse from the API
         :rtype: PayStackResponse object
         """
-        # convert to strings
-        send_invoices = self._convert_to_string(send_invoices)
-        send_sms = self._convert_to_string(send_sms)
-
         data = {
             "name": name,
             "amount": amount,
             "interval": interval,
             "description": description,
             "send_invoices": send_invoices,
             "send_sms": send_sms,
```

### Comparing `paystackease-2.2.0/paystackease/apis/async_apis/aproducts.py` & `paystackease-2.3.0/paystackease/apis/async_apis/aproducts.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,17 +35,14 @@
         :param: unlimited: Set true if the product has unlimited stock,
         :param: quantity: Quantity of the product in stock Use if unlimited is false
 
         :return: The PayStackResponse from the API
         :rtype: PayStackResponse object
         """
 
-        # convert bool to string
-        unlimited = self._convert_to_string(unlimited)
-
         data = {
             "name": name,
             "description": description,
             "price": amount,
             "currency": currency,
             "unlimited": unlimited,
             "quantity": quantity,
@@ -110,17 +107,14 @@
         :param: unlimited: Set true if the product has unlimited stock,
         :param: quantity: Quantity of the product in stock Use if unlimited is false
 
         :return: The PayStackResponse from the API
         :rtype: PayStackResponse object
         """
 
-        # convert bool to string
-        unlimited = self._convert_to_string(unlimited)
-
         data = {
             "name": name,
             "description": description,
             "price": amount,
             "currency": currency,
             "unlimited": unlimited,
             "quantity": quantity,
```

### Comparing `paystackease-2.2.0/paystackease/apis/async_apis/arefund.py` & `paystackease-2.3.0/paystackease/apis/async_apis/arefund.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/async_apis/asettlements.py` & `paystackease-2.3.0/paystackease/apis/async_apis/asettlements.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/async_apis/asubaccounts.py` & `paystackease-2.3.0/paystackease/apis/async_apis/asubaccounts.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/async_apis/asubscriptions.py` & `paystackease-2.3.0/paystackease/apis/async_apis/asubscriptions.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/async_apis/aterminal.py` & `paystackease-2.3.0/paystackease/apis/async_apis/aterminal.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/async_apis/atransaction_splits.py` & `paystackease-2.3.0/paystackease/apis/async_apis/atransaction_splits.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/async_apis/atransactions.py` & `paystackease-2.3.0/paystackease/apis/async_apis/atransactions.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/async_apis/atransfer_recipients.py` & `paystackease-2.3.0/paystackease/apis/async_apis/atransfer_recipients.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/async_apis/atransfers.py` & `paystackease-2.3.0/paystackease/apis/async_apis/atransfers.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/async_apis/atransfers_control.py` & `paystackease-2.3.0/paystackease/apis/async_apis/atransfers_control.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/async_apis/averification.py` & `paystackease-2.3.0/paystackease/apis/async_apis/averification.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/sync_apis/apple_pay.py` & `paystackease-2.3.0/paystackease/apis/sync_apis/apple_pay.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/sync_apis/bulk_charges.py` & `paystackease-2.3.0/paystackease/apis/sync_apis/bulk_charges.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/sync_apis/charges.py` & `paystackease-2.3.0/paystackease/apis/sync_apis/charges.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/sync_apis/customers.py` & `paystackease-2.3.0/paystackease/apis/sync_apis/customers.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/sync_apis/dedicated_virtual_accounts.py` & `paystackease-2.3.0/paystackease/apis/sync_apis/dedicated_virtual_accounts.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/sync_apis/disputes.py` & `paystackease-2.3.0/paystackease/apis/sync_apis/disputes.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/sync_apis/integration.py` & `paystackease-2.3.0/paystackease/apis/sync_apis/integration.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/sync_apis/miscellaneous.py` & `paystackease-2.3.0/paystackease/apis/sync_apis/miscellaneous.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         pay_with_bank = self._convert_to_string(pay_with_bank)
         enabled_for_verification = self._convert_to_string(enabled_for_verification)
 
         params = {
             "country": country,
             "use_cursor": use_cursor,
             "perPage": per_page,
-            "supports_transfer": pay_with_bank_transfer,
+            "pay_with_bank_transfer": pay_with_bank_transfer,
             "pay_with_bank": pay_with_bank,
             "enabled_for_verification": enabled_for_verification,
             "next": next_cursor,
             "previous": previous_cursor,
             "gateway": gateway,
             "type": channel_type,
             "currency": currency,
```

### Comparing `paystackease-2.2.0/paystackease/apis/sync_apis/payment_pages.py` & `paystackease-2.3.0/paystackease/apis/sync_apis/payment_pages.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/sync_apis/payment_requests.py` & `paystackease-2.3.0/paystackease/apis/sync_apis/payment_requests.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,17 +17,17 @@
     Reference: https://paystack.com/docs/api/payment-request/
     """
 
     def create_payment_request(
             self,
             customer: str,
             amount: int,
-            draft: bool,
-            has_invoice: bool,
-            send_notification: bool,
+            draft: bool = False,
+            has_invoice: bool = True,
+            send_notification: bool = True,
             due_date: Optional[Union[date, None]] = None,
             description: Optional[Union[str, Any]] = None,
             line_items: Optional[Union[List[Dict[str, Any]], None]] = None,
             tax: Optional[Union[List[Dict[str, Any]], None]] = None,
             currency: Optional[Union[Currency, Any]] = None,
             invoice_number: Optional[Union[int, Any]] = None,
             split_code: Optional[Union[str, Any]] = None,
@@ -49,17 +49,14 @@
         :param: split_code: split code of the transaction split
 
         :return: The PayStackResponse from the API
         :rtype: PayStackResponse object
         """
         # convert date and bool to string
         due_date = self._convert_to_string(due_date)
-        draft = self._convert_to_string(draft)
-        has_invoice = self._convert_to_string(has_invoice)
-        send_notification = self._convert_to_string(send_notification)
 
         data = {
             "customer": customer,
             "amount": amount,
             "due_date": due_date,
             "description": description,
             "line_items": line_items,
@@ -165,16 +162,14 @@
 
         :param: code: Payment request code
         :param: send_notification: Set true if you want to send a notification to the customer email
 
         :return: The PayStackResponse from the API
         :rtype: PayStackResponse object
         """
-        # convert to strings
-        send_notification = self._convert_to_string(send_notification)
 
         data = {"send_notification": send_notification}
         return self._post_request(f"/paymentrequest/finalize/{code}", data=data)
 
     def update_payment_request(
             self,
             id_or_code: str,
@@ -208,16 +203,14 @@
 
         :return: The PayStackResponse from the API
         :rtype: PayStackResponse object
         """
 
         # convert date and bool to string
         due_date = self._convert_to_string(due_date)
-        draft = self._convert_to_string(draft)
-        send_notification = self._convert_to_string(send_notification)
 
         data = {
             "customer": customer,
             "amount": amount,
             "due_date": due_date,
             "description": description,
             "line_items": line_items,
```

### Comparing `paystackease-2.2.0/paystackease/apis/sync_apis/plans.py` & `paystackease-2.3.0/paystackease/apis/sync_apis/plans.py`

 * *Files 20% similar despite different names*

```diff
@@ -38,18 +38,14 @@
         :param: send_sms: Send SMS to customer
         :param: currency: Currency of the plan
         :param: invoice_limit: Invoice limit of the plan
 
         :return: The PayStackResponse from the API
         :rtype: PayStackResponse object
         """
-        # convert to strings
-        send_invoices = self._convert_to_string(send_invoices)
-        send_sms = self._convert_to_string(send_sms)
-
         data = {
             "name": name,
             "amount": amount,
             "interval": interval,
             "description": description,
             "send_invoices": send_invoices,
             "send_sms": send_sms,
@@ -58,15 +54,15 @@
         }
         return self._post_request("/plan", data=data)
 
     def list_plans(
             self,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
-            status: Optional[Union[str, None]] = None,
+            status: Optional[Union[str, None]] = 'active',
             interval: Optional[Union[Interval, None]] = None,
             amount: Optional[Union[int, None]] = None,
     ) -> PayStackResponse:
         """
         List all the plans
 
         :param: per_page: Number of records to return
@@ -122,18 +118,14 @@
         :param: send_sms:
         :param: currency:
         :param: invoice_limit:
 
         :return: The PayStackResponse from the API
         :rtype: PayStackResponse object
         """
-        # convert to strings
-        send_invoices = self._convert_to_string(send_invoices)
-        send_sms = self._convert_to_string(send_sms)
-
         data = {
             "name": name,
             "amount": amount,
             "interval": interval,
             "description": description,
             "send_invoices": send_invoices,
             "send_sms": send_sms,
```

### Comparing `paystackease-2.2.0/paystackease/apis/sync_apis/products.py` & `paystackease-2.3.0/paystackease/apis/sync_apis/products.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,17 +35,14 @@
         :param: unlimited: Set true if the product has unlimited stock,
         :param: quantity: Quantity of the product in stock Use if unlimited is false
 
         :return: The PayStackResponse from the API
         :rtype: PayStackResponse object
         """
 
-        # convert bool to string
-        unlimited = self._convert_to_string(unlimited)
-
         data = {
             "name": name,
             "description": description,
             "price": amount,
             "currency": currency,
             "unlimited": unlimited,
             "quantity": quantity,
@@ -110,17 +107,14 @@
         :param: unlimited: Set true if the product has unlimited stock,
         :param: quantity: Quantity of the product in stock Use if unlimited is false
 
         :return: The PayStackResponse from the API
         :rtype: PayStackResponse object
         """
 
-        # convert bool to string
-        unlimited = self._convert_to_string(unlimited)
-
         data = {
             "name": name,
             "description": description,
             "price": amount,
             "currency": currency,
             "unlimited": unlimited,
             "quantity": quantity,
```

### Comparing `paystackease-2.2.0/paystackease/apis/sync_apis/refund.py` & `paystackease-2.3.0/paystackease/apis/sync_apis/refund.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/sync_apis/settlements.py` & `paystackease-2.3.0/paystackease/apis/sync_apis/settlements.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/sync_apis/subaccounts.py` & `paystackease-2.3.0/paystackease/apis/sync_apis/subaccounts.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/sync_apis/subscriptions.py` & `paystackease-2.3.0/paystackease/apis/sync_apis/subscriptions.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/sync_apis/terminal.py` & `paystackease-2.3.0/paystackease/apis/sync_apis/terminal.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/sync_apis/transaction_splits.py` & `paystackease-2.3.0/paystackease/apis/sync_apis/transaction_splits.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/sync_apis/transactions.py` & `paystackease-2.3.0/paystackease/apis/sync_apis/transactions.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/sync_apis/transfer_recipients.py` & `paystackease-2.3.0/paystackease/apis/sync_apis/transfer_recipients.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/sync_apis/transfers.py` & `paystackease-2.3.0/paystackease/apis/sync_apis/transfers.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/sync_apis/transfers_control.py` & `paystackease-2.3.0/paystackease/apis/sync_apis/transfers_control.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/apis/sync_apis/verification.py` & `paystackease-2.3.0/paystackease/apis/sync_apis/verification.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/core/__init__.py` & `paystackease-2.3.0/paystackease/core/__init__.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/core/_api_base.py` & `paystackease-2.3.0/paystackease/core/_api_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         :raise TypeError: if the value is not a supported type
 
         :return: The value as a string
         :rtype: str
         """
         # each supported type is mapped to its corresponding conversion function
         conversion_functions = {
-            bool: lambda val: str(val),
+            bool: lambda val: str(val).lower(),
             date: lambda val: val.strftime("%Y-%m-%d"),
             datetime: lambda val: val.strftime("%Y-%m-%d %H:%M:%S"),  # Added a datetime
         }
 
         if value is None:
             return None
         if type(value) in conversion_functions:
```

### Comparing `paystackease-2.2.0/paystackease/core/_api_base_client.py` & `paystackease-2.3.0/paystackease/core/_api_base_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,17 +79,17 @@
                 if 500 <= response.status_code <= 600:
                     error_message = f"Server error occurred: {response.status_code}"
                     logger.error(error_message)
                     raise PayStackServerError(message=error_message, status_code=response.status_code)
 
                 return PayStackResponse(
                     status_code=response.status_code,
-                    status=response_data.get('status'),
-                    message=response_data.get('message'),
-                    data=response_data.get('data'),
+                    status=response_data.get('status', False),
+                    message=response_data.get('message', ''),
+                    data=response_data.get('data', None),
                 )
         except (RequestException, ConnectionError) as error:
             # Extract status code if available from the exception
             error_message = str(error)
             status_code = getattr(error, "response", None) and getattr(
                 error.response, "status_code", None
             )
@@ -165,17 +165,17 @@
                 if 500 <= response.status <= 600:
                     error_message = f"Server error occurred: {response.status}"
                     logger.error(error_message)
                     raise PayStackServerError(message=error_message, status_code=response.status)
 
                 return PayStackResponse(
                     status_code=response.status,
-                    status=response_data.get('status'),
-                    message=response_data.get('message'),
-                    data=response_data.get('data'),
+                    status=response_data.get('status', False),
+                    message=response_data.get('message', ''),
+                    data=response_data.get('data', None),
                 )
         except (ClientError, ClientConnectionError) as error:
             # Extract status code if available from the exception
             error_message = str(error)
             status_code = getattr(error, "response", None) and getattr(
                 error.args[0], "status_code", None
             )
```

### Comparing `paystackease-2.2.0/paystackease/core/_api_client_requests.py` & `paystackease-2.3.0/paystackease/core/_api_client_requests.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/core/_api_client_response.py` & `paystackease-2.3.0/paystackease/core/_api_client_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,23 @@
 
     status_code: int
     status: bool
     message: str
     data: Optional[Union[Dict[str, Any], None]]
 
     @property
-    def url(self) -> Optional[Union[str, None]]:
+    def checkout_url(self) -> Optional[Union[str, None]]:
         """
         URL of the request
         """
         if self.status_code == 200 and self.data and isinstance(self.data, dict):
             return self.data["authorization_url"]
         return None
+
+    @property
+    def charge_url(self) -> Optional[Union[str, None]]:
+        """
+        URL of the request
+        """
+        if self.status_code == 200 and self.data and isinstance(self.data, dict):
+            return self.data["url"]
+        return None
```

### Comparing `paystackease-2.2.0/paystackease/core/_api_env.py` & `paystackease-2.3.0/paystackease/core/_api_env.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/core/_api_errors.py` & `paystackease-2.3.0/paystackease/core/_api_errors.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/core/_events.py` & `paystackease-2.3.0/paystackease/core/_events.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/core/_webhook.py` & `paystackease-2.3.0/paystackease/core/_webhook.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/helpers/__init__.py` & `paystackease-2.3.0/paystackease/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/helpers/convert.py` & `paystackease-2.3.0/paystackease/helpers/convert.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/helpers/tool_kit.py` & `paystackease-2.3.0/paystackease/helpers/tool_kit.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/paystackease/paystack.py` & `paystackease-2.3.0/paystackease/paystack.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.2.0/pyproject.toml` & `paystackease-2.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "paystackease"
-version = "2.2.0"
+version = "2.3.0"
 description = "This is a simple api wrapper that implements both asynchronous and synchronous http requests to interact with Paystack APIs."
 authors = ["Peter Mbachu <doublep098@gmail.com>"]
 maintainers = []
 license = "MIT"
 readme = "README.md"
 keywords = ["paystack", "paystackease", "python", "api", "payment integration"]
 classifiers = [
```

### Comparing `paystackease-2.2.0/PKG-INFO` & `paystackease-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paystackease
-Version: 2.2.0
+Version: 2.3.0
 Summary: This is a simple api wrapper that implements both asynchronous and synchronous http requests to interact with Paystack APIs.
 License: MIT
 Keywords: paystack,paystackease,python,api,payment integration
 Author: Peter Mbachu
 Author-email: doublep098@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

