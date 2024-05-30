# Comparing `tmp/airbyte-source-tplcentral-0.1.1.tar.gz` & `tmp/airbyte_source_tplcentral-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-tplcentral-0.1.1.tar", last modified: Thu Feb  1 08:02:59 2024, max compression
+gzip compressed data, was "airbyte_source_tplcentral-0.1.2.tar", max compression
```

## Comparing `airbyte-source-tplcentral-0.1.1.tar` & `airbyte_source_tplcentral-0.1.2.tar`

### file list

```diff
@@ -1,143 +1,103 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 08:02:59.154112 airbyte-source-tplcentral-0.1.1/
--rw-r--r--   0 root         (0) root         (0)     5469 2024-02-01 08:02:59.154112 airbyte-source-tplcentral-0.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5429 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 08:02:59.154112 airbyte-source-tplcentral-0.1.1/airbyte_source_tplcentral.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5469 2024-02-01 08:02:59.000000 airbyte-source-tplcentral-0.1.1/airbyte_source_tplcentral.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7633 2024-02-01 08:02:59.000000 airbyte-source-tplcentral-0.1.1/airbyte_source_tplcentral.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-01 08:02:59.000000 airbyte-source-tplcentral-0.1.1/airbyte_source_tplcentral.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-02-01 08:02:59.000000 airbyte-source-tplcentral-0.1.1/airbyte_source_tplcentral.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       86 2024-02-01 08:02:59.000000 airbyte-source-tplcentral-0.1.1/airbyte_source_tplcentral.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       47 2024-02-01 08:02:59.000000 airbyte-source-tplcentral-0.1.1/airbyte_source_tplcentral.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 08:02:59.134112 airbyte-source-tplcentral-0.1.1/integration_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      260 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      314 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)     1392 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/integration_tests/catalog.json
--rw-r--r--   0 root         (0) root         (0)       43 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/integration_tests/config_http_url.json
--rw-r--r--   0 root         (0) root         (0)    30643 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/integration_tests/configured_catalog_customers.json
--rw-r--r--   0 root         (0) root         (0)     9551 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/integration_tests/configured_catalog_inventory.json
--rw-r--r--   0 root         (0) root         (0)    20081 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/integration_tests/configured_catalog_items.json
--rw-r--r--   0 root         (0) root         (0)    54038 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/integration_tests/configured_catalog_orders.json
--rw-r--r--   0 root         (0) root         (0)     7536 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/integration_tests/configured_catalog_stock_details.json
--rw-r--r--   0 root         (0) root         (0)     1498 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/integration_tests/configured_catalog_stock_summaries.json
--rw-r--r--   0 root         (0) root         (0)      233 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)      233 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)      260 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/integration_tests/sample_state.json
--rw-r--r--   0 root         (0) root         (0)     5335 2024-02-01 08:02:59.158112 airbyte-source-tplcentral-0.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      948 2024-02-01 08:02:57.000000 airbyte-source-tplcentral-0.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 08:02:59.134112 airbyte-source-tplcentral-0.1.1/source_tplcentral/
--rw-r--r--   0 root         (0) root         (0)     1177 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/__init__.py
--rw-r--r--   0 root         (0) root         (0)      242 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 08:02:59.134112 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/
--rw-r--r--   0 root         (0) root         (0)     1952 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/customers.json
--rw-r--r--   0 root         (0) root         (0)     3376 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/inventory.json
--rw-r--r--   0 root         (0) root         (0)     1483 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/items.json
--rw-r--r--   0 root         (0) root         (0)     3196 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/orders.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 08:02:59.130112 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 08:02:59.126112 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/common/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 08:02:59.138112 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/common/enum/
--rw-r--r--   0 root         (0) root         (0)      168 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/common/enum/address_status_type.json
--rw-r--r--   0 root         (0) root         (0)      156 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/common/enum/contact_type.json
--rw-r--r--   0 root         (0) root         (0)      162 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/common/enum/fulfillment_invoicing.json
--rw-r--r--   0 root         (0) root         (0)      196 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/common/enum/outbound_mobile_serialization_behavior.json
--rw-r--r--   0 root         (0) root         (0)      145 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/common/enum/parcel_label_type.json
--rw-r--r--   0 root         (0) root         (0)      176 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/common/enum/prepopulate_carrier_info.json
--rw-r--r--   0 root         (0) root         (0)      406 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/common/enum/price_calc_field_type.json
--rw-r--r--   0 root         (0) root         (0)      155 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/common/enum/receive_against_asns.json
--rw-r--r--   0 root         (0) root         (0)      197 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/common/enum/serial_number_usage_level.json
--rw-r--r--   0 root         (0) root         (0)      173 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/common/enum/transaction_confirm_invoice_create_default.json
--rw-r--r--   0 root         (0) root         (0)      218 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/common/enum/transaction_entry_type.json
--rw-r--r--   0 root         (0) root         (0)      155 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/common/enum/usage_level.json
--rw-r--r--   0 root         (0) root         (0)      223 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/common/enum/warehouse_transaction_api_status.json
--rw-r--r--   0 root         (0) root         (0)      284 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/common/enum/warehouse_transaction_source_type.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 08:02:59.126112 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 08:02:59.146112 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/
--rw-r--r--   0 root         (0) root         (0)      692 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/alerts.json
--rw-r--r--   0 root         (0) root         (0)     1078 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/asn_pre_check.json
--rw-r--r--   0 root         (0) root         (0)      753 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/asn_pre_check_options.json
--rw-r--r--   0 root         (0) root         (0)      370 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/component.json
--rw-r--r--   0 root         (0) root         (0)      328 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/customer_read_only.json
--rw-r--r--   0 root         (0) root         (0)      416 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/dimension_net.json
--rw-r--r--   0 root         (0) root         (0)      683 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/directed_put_away.json
--rw-r--r--   0 root         (0) root         (0)      432 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/edi.json
--rw-r--r--   0 root         (0) root         (0)      523 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/haz_mat.json
--rw-r--r--   0 root         (0) root         (0)      554 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/inventory_unit.json
--rw-r--r--   0 root         (0) root         (0)      686 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/item_options.json
--rw-r--r--   0 root         (0) root         (0)      183 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/item_qualifier.json
--rw-r--r--   0 root         (0) root         (0)      716 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/item_read_only.json
--rw-r--r--   0 root         (0) root         (0)      295 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/kit.json
--rw-r--r--   0 root         (0) root         (0)      924 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/options.json
--rw-r--r--   0 root         (0) root         (0)      339 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/other_system_behaviors.json
--rw-r--r--   0 root         (0) root         (0)      456 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/package_unit.json
--rw-r--r--   0 root         (0) root         (0)     1474 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/packaging.json
--rw-r--r--   0 root         (0) root         (0)      585 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/pallets.json
--rw-r--r--   0 root         (0) root         (0)      230 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/qualifier_renamer.json
--rw-r--r--   0 root         (0) root         (0)     1108 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/receiving.json
--rw-r--r--   0 root         (0) root         (0)      448 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/saved_element_def.json
--rw-r--r--   0 root         (0) root         (0)      273 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/saved_element_defs.json
--rw-r--r--   0 root         (0) root         (0)      558 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/saved_element_trans_def.json
--rw-r--r--   0 root         (0) root         (0)      392 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/secondary_unit.json
--rw-r--r--   0 root         (0) root         (0)     1774 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/shipping.json
--rw-r--r--   0 root         (0) root         (0)      443 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/storage.json
--rw-r--r--   0 root         (0) root         (0)      883 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/track_bys.json
--rw-r--r--   0 root         (0) root         (0)      722 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/user_interface.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 08:02:59.126112 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 08:02:59.150112 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/
--rw-r--r--   0 root         (0) root         (0)      237 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/batch_identifier.json
--rw-r--r--   0 root         (0) root         (0)      254 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/batch_name_key.json
--rw-r--r--   0 root         (0) root         (0)      323 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/billing.json
--rw-r--r--   0 root         (0) root         (0)      423 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/billing_charge.json
--rw-r--r--   0 root         (0) root         (0)      712 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/billing_charge_detail.json
--rw-r--r--   0 root         (0) root         (0)      221 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/capacity_type_identifier.json
--rw-r--r--   0 root         (0) root         (0)      221 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/channel_identifier.json
--rw-r--r--   0 root         (0) root         (0)      221 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/contact_identifier.json
--rw-r--r--   0 root         (0) root         (0)     1177 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/contact_info.json
--rw-r--r--   0 root         (0) root         (0)      271 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/customer_identifier.json
--rw-r--r--   0 root         (0) root         (0)      357 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/dimension.json
--rw-r--r--   0 root         (0) root         (0)      221 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/facility_identifier.json
--rw-r--r--   0 root         (0) root         (0)      221 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/item_classification_identifier.json
--rw-r--r--   0 root         (0) root         (0)      220 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/item_identifier.json
--rw-r--r--   0 root         (0) root         (0)      507 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/item_traits.json
--rw-r--r--   0 root         (0) root         (0)      240 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/location_identifier.json
--rw-r--r--   0 root         (0) root         (0)      254 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/location_name_key.json
--rw-r--r--   0 root         (0) root         (0)     1836 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/order_contact_info.json
--rw-r--r--   0 root         (0) root         (0)     1907 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/order_ship_to_info.json
--rw-r--r--   0 root         (0) root         (0)     1129 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/other_contact_info.json
--rw-r--r--   0 root         (0) root         (0)      193 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/other_customer_contact_type.json
--rw-r--r--   0 root         (0) root         (0)      221 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/package_def_identifier.json
--rw-r--r--   0 root         (0) root         (0)      238 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/pallet_identifier.json
--rw-r--r--   0 root         (0) root         (0)      254 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/pallet_name_key.json
--rw-r--r--   0 root         (0) root         (0)      221 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/pallet_type_identifier.json
--rw-r--r--   0 root         (0) root         (0)      272 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/proposed_allocation.json
--rw-r--r--   0 root         (0) root         (0)      240 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/retailer_info.json
--rw-r--r--   0 root         (0) root         (0)      300 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/retailer_name_key.json
--rw-r--r--   0 root         (0) root         (0)      223 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/saved_element.json
--rw-r--r--   0 root         (0) root         (0)      221 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/unit_of_measure_identifier.json
--rw-r--r--   0 root         (0) root         (0)      221 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/user_identifier.json
--rw-r--r--   0 root         (0) root         (0)      501 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/web_hook_parameters_for_events.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 08:02:59.130112 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/order/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 08:02:59.154112 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/order/models/
--rw-r--r--   0 root         (0) root         (0)      569 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/order/models/allocation.json
--rw-r--r--   0 root         (0) root         (0)      532 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/order/models/allocation_detail.json
--rw-r--r--   0 root         (0) root         (0)      473 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/order/models/fulfill_inv_info.json
--rw-r--r--   0 root         (0) root         (0)      168 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/order/models/load_out_state.json
--rw-r--r--   0 root         (0) root         (0)     2613 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/order/models/order_item.json
--rw-r--r--   0 root         (0) root         (0)      686 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/order/models/order_item_in_package.json
--rw-r--r--   0 root         (0) root         (0)     1686 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/order/models/order_item_read_only.json
--rw-r--r--   0 root         (0) root         (0)     4120 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/order/models/order_read_only.json
--rw-r--r--   0 root         (0) root         (0)      375 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/order/models/outbound_serial_numbers.json
--rw-r--r--   0 root         (0) root         (0)      841 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/order/models/package_content_info.json
--rw-r--r--   0 root         (0) root         (0)     1256 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/order/models/package_info.json
--rw-r--r--   0 root         (0) root         (0)      711 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/order/models/parcel_option.json
--rw-r--r--   0 root         (0) root         (0)     1097 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/order/models/routing_info.json
--rw-r--r--   0 root         (0) root         (0)     2622 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/stock_details.json
--rw-r--r--   0 root         (0) root         (0)      620 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/stock_summaries.json
--rw-r--r--   0 root         (0) root         (0)     3290 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/source.py
--rw-r--r--   0 root         (0) root         (0)     1552 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/spec.json
--rw-r--r--   0 root         (0) root         (0)     9610 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/streams.py
--rw-r--r--   0 root         (0) root         (0)      965 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/source_tplcentral/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 08:02:59.154112 airbyte-source-tplcentral-0.1.1/unit_tests/
--rw-r--r--   0 root         (0) root         (0)     1106 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/unit_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2957 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/unit_tests/test_incremental_streams.py
--rw-r--r--   0 root         (0) root         (0)     1156 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/unit_tests/test_source.py
--rw-r--r--   0 root         (0) root         (0)     5901 2024-02-01 07:53:30.000000 airbyte-source-tplcentral-0.1.1/unit_tests/test_streams.py
+-rw-r--r--   0        0        0     4568 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/README.md
+-rw-r--r--   0        0        0      785 2024-05-30 02:38:58.680969 airbyte_source_tplcentral-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1177 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/__init__.py
+-rw-r--r--   0        0        0      242 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/run.py
+-rw-r--r--   0        0        0     1952 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/customers.json
+-rw-r--r--   0        0        0     3376 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/inventory.json
+-rw-r--r--   0        0        0     1483 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/items.json
+-rw-r--r--   0        0        0     3196 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/orders.json
+-rw-r--r--   0        0        0      168 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/common/enum/address_status_type.json
+-rw-r--r--   0        0        0      156 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/common/enum/contact_type.json
+-rw-r--r--   0        0        0      162 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/common/enum/fulfillment_invoicing.json
+-rw-r--r--   0        0        0      196 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/common/enum/outbound_mobile_serialization_behavior.json
+-rw-r--r--   0        0        0      145 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/common/enum/parcel_label_type.json
+-rw-r--r--   0        0        0      176 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/common/enum/prepopulate_carrier_info.json
+-rw-r--r--   0        0        0      406 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/common/enum/price_calc_field_type.json
+-rw-r--r--   0        0        0      155 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/common/enum/receive_against_asns.json
+-rw-r--r--   0        0        0      197 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/common/enum/serial_number_usage_level.json
+-rw-r--r--   0        0        0      173 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/common/enum/transaction_confirm_invoice_create_default.json
+-rw-r--r--   0        0        0      218 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/common/enum/transaction_entry_type.json
+-rw-r--r--   0        0        0      155 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/common/enum/usage_level.json
+-rw-r--r--   0        0        0      223 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/common/enum/warehouse_transaction_api_status.json
+-rw-r--r--   0        0        0      284 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/common/enum/warehouse_transaction_source_type.json
+-rw-r--r--   0        0        0      692 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/alerts.json
+-rw-r--r--   0        0        0     1078 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/asn_pre_check.json
+-rw-r--r--   0        0        0      753 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/asn_pre_check_options.json
+-rw-r--r--   0        0        0      370 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/component.json
+-rw-r--r--   0        0        0      328 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/customer_read_only.json
+-rw-r--r--   0        0        0      416 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/dimension_net.json
+-rw-r--r--   0        0        0      683 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/directed_put_away.json
+-rw-r--r--   0        0        0      432 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/edi.json
+-rw-r--r--   0        0        0      523 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/haz_mat.json
+-rw-r--r--   0        0        0      554 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/inventory_unit.json
+-rw-r--r--   0        0        0      686 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/item_options.json
+-rw-r--r--   0        0        0      183 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/item_qualifier.json
+-rw-r--r--   0        0        0      716 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/item_read_only.json
+-rw-r--r--   0        0        0      295 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/kit.json
+-rw-r--r--   0        0        0      924 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/options.json
+-rw-r--r--   0        0        0      339 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/other_system_behaviors.json
+-rw-r--r--   0        0        0      456 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/package_unit.json
+-rw-r--r--   0        0        0     1474 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/packaging.json
+-rw-r--r--   0        0        0      585 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/pallets.json
+-rw-r--r--   0        0        0      230 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/qualifier_renamer.json
+-rw-r--r--   0        0        0     1108 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/receiving.json
+-rw-r--r--   0        0        0      448 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/saved_element_def.json
+-rw-r--r--   0        0        0      273 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/saved_element_defs.json
+-rw-r--r--   0        0        0      558 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/saved_element_trans_def.json
+-rw-r--r--   0        0        0      392 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/secondary_unit.json
+-rw-r--r--   0        0        0     1774 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/shipping.json
+-rw-r--r--   0        0        0      443 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/storage.json
+-rw-r--r--   0        0        0      883 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/track_bys.json
+-rw-r--r--   0        0        0      722 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/user_interface.json
+-rw-r--r--   0        0        0      237 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/batch_identifier.json
+-rw-r--r--   0        0        0      254 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/batch_name_key.json
+-rw-r--r--   0        0        0      323 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/billing.json
+-rw-r--r--   0        0        0      423 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/billing_charge.json
+-rw-r--r--   0        0        0      712 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/billing_charge_detail.json
+-rw-r--r--   0        0        0      221 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/capacity_type_identifier.json
+-rw-r--r--   0        0        0      221 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/channel_identifier.json
+-rw-r--r--   0        0        0      221 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/contact_identifier.json
+-rw-r--r--   0        0        0     1177 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/contact_info.json
+-rw-r--r--   0        0        0      271 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/customer_identifier.json
+-rw-r--r--   0        0        0      357 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/dimension.json
+-rw-r--r--   0        0        0      221 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/facility_identifier.json
+-rw-r--r--   0        0        0      221 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/item_classification_identifier.json
+-rw-r--r--   0        0        0      220 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/item_identifier.json
+-rw-r--r--   0        0        0      507 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/item_traits.json
+-rw-r--r--   0        0        0      240 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/location_identifier.json
+-rw-r--r--   0        0        0      254 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/location_name_key.json
+-rw-r--r--   0        0        0     1836 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/order_contact_info.json
+-rw-r--r--   0        0        0     1907 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/order_ship_to_info.json
+-rw-r--r--   0        0        0     1129 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/other_contact_info.json
+-rw-r--r--   0        0        0      193 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/other_customer_contact_type.json
+-rw-r--r--   0        0        0      221 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/package_def_identifier.json
+-rw-r--r--   0        0        0      238 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/pallet_identifier.json
+-rw-r--r--   0        0        0      254 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/pallet_name_key.json
+-rw-r--r--   0        0        0      221 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/pallet_type_identifier.json
+-rw-r--r--   0        0        0      272 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/proposed_allocation.json
+-rw-r--r--   0        0        0      240 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/retailer_info.json
+-rw-r--r--   0        0        0      300 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/retailer_name_key.json
+-rw-r--r--   0        0        0      223 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/saved_element.json
+-rw-r--r--   0        0        0      221 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/unit_of_measure_identifier.json
+-rw-r--r--   0        0        0      221 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/user_identifier.json
+-rw-r--r--   0        0        0      501 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/web_hook_parameters_for_events.json
+-rw-r--r--   0        0        0      569 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/order/models/allocation.json
+-rw-r--r--   0        0        0      532 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/order/models/allocation_detail.json
+-rw-r--r--   0        0        0      473 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/order/models/fulfill_inv_info.json
+-rw-r--r--   0        0        0      168 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/order/models/load_out_state.json
+-rw-r--r--   0        0        0     2613 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/order/models/order_item.json
+-rw-r--r--   0        0        0      686 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/order/models/order_item_in_package.json
+-rw-r--r--   0        0        0     1686 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/order/models/order_item_read_only.json
+-rw-r--r--   0        0        0     4120 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/order/models/order_read_only.json
+-rw-r--r--   0        0        0      375 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/order/models/outbound_serial_numbers.json
+-rw-r--r--   0        0        0      841 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/order/models/package_content_info.json
+-rw-r--r--   0        0        0     1256 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/order/models/package_info.json
+-rw-r--r--   0        0        0      711 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/order/models/parcel_option.json
+-rw-r--r--   0        0        0     1097 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/order/models/routing_info.json
+-rw-r--r--   0        0        0     2622 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/stock_details.json
+-rw-r--r--   0        0        0      620 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/stock_summaries.json
+-rw-r--r--   0        0        0     3290 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/source.py
+-rw-r--r--   0        0        0     1552 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/spec.json
+-rw-r--r--   0        0        0     9610 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/streams.py
+-rw-r--r--   0        0        0      965 2024-05-30 02:26:09.000000 airbyte_source_tplcentral-0.1.2/source_tplcentral/util.py
+-rw-r--r--   0        0        0     5315 1970-01-01 00:00:00.000000 airbyte_source_tplcentral-0.1.2/PKG-INFO
```

### Comparing `airbyte-source-tplcentral-0.1.1/README.md` & `airbyte_source_tplcentral-0.1.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,100 +1,111 @@
-# 3PL Central Source
+Metadata-Version: 2.1
+Name: airbyte-source-tplcentral
+Version: 0.1.2
+Summary: Source implementation for Tplcentral.
+Home-page: https://airbyte.com
+License: MIT
+Author: Airbyte
+Author-email: contact@airbyte.io
+Requires-Python: >=3.9,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: airbyte-cdk (==0.80.0)
+Requires-Dist: arrow (==1.2.1)
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/tplcentral
+Project-URL: Repository, https://github.com/airbytehq/airbyte
+Description-Content-Type: text/markdown
 
-This is the repository for the 3PL Central source connector, written in Python.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/tplcentral).
+# Tplcentral source connector
+
+
+This is the repository for the Tplcentral source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/tplcentral).
 
 ## Local development
 
 ### Prerequisites
-**To iterate on this connector, make sure to complete this prerequisites section.**
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
-#### Minimum Python version required `= 3.7.0`
-
-#### Build & Activate Virtual Environment and install dependencies
-From this connector directory, create a virtual environment:
-```
-python -m venv .venv
-```
 
-This will generate a virtualenv for this module in `.venv/`. Make sure this venv is active in your
-development environment of choice. To activate it from the terminal, run:
-```
-source .venv/bin/activate
-pip install -r requirements.txt
-pip install '.[tests]'
+### Installing the connector
+From this connector directory, run:
+```bash
+poetry install --with dev
 ```
-If you are in an IDE, follow your IDE's instructions to activate the virtualenv.
 
-Note that while we are installing dependencies from `requirements.txt`, you should only edit `setup.py` for your dependencies. `requirements.txt` is
-used for editable installs (`pip install -e`) to pull in Python dependencies from the monorepo and will call `setup.py`.
-If this is mumbo jumbo to you, don't worry about it, just put your deps in `setup.py` but install using `pip install -r requirements.txt` and everything
-should work as you expect.
 
-#### Create credentials
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/tplcentral)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_tplcentral/spec.json` file.
+### Create credentials
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/tplcentral)
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_tplcentral/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source tplcentral test creds`
-and place them into `secrets/config.json`.
 
 ### Locally running the connector
 ```
-python main.py spec
-python main.py check --config secrets/config.json
-python main.py discover --config secrets/config.json
-python main.py read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+poetry run source-tplcentral spec
+poetry run source-tplcentral check --config secrets/config.json
+poetry run source-tplcentral discover --config secrets/config.json
+poetry run source-tplcentral read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
-### Locally running the connector docker image
-
+### Running unit tests
+To run unit tests locally, from the connector directory run:
+```
+poetry run pytest unit_tests
+```
 
-#### Build
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
+### Building the docker image
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
 airbyte-ci connectors --name=source-tplcentral build
 ```
 
-An image will be built with the tag `airbyte/source-tplcentral:dev`.
+An image will be available on your host with the tag `airbyte/source-tplcentral:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-tplcentral:dev .
-```
 
-#### Run
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-tplcentral:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-tplcentral:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-tplcentral:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-tplcentral:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
-## Testing
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-tplcentral test
 ```
 
 ### Customizing acceptance Tests
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-## Dependency Management
-All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
+### Dependency Management
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
 
-### Publishing a new version of the connector
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
+
+## Publishing a new version of the connector
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-tplcentral test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/tplcentral.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/tplcentral.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-tplcentral-0.1.1/integration_tests/configured_catalog_stock_summaries.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/order/models/package_info.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('$schema', 'http://json-schema.org/draft-07/schema#'), ('type', "*

 * *            "'object'), ('additionalProperties', False), ('properties', OrderedDict([('PackageId', "*

 * *            "OrderedDict([('type', 'integer')])), ('PackageTypeId', OrderedDict([('type', "*

 * *            "'integer')])), ('PackageDefIdentifier', OrderedDict([('$ref', "*

 * *            "'../../generic/models/package_def_identifier.json')])), ('Length', "*

 * *            "OrderedDict([('type', ['null', 'number'])])), ('Width' […]*

```diff
@@ -1,66 +1,92 @@
 {
-    "streams": [
-        {
-            "destination_sync_mode": "append",
-            "stream": {
-                "json_schema": {
-                    "$schema": "http://json-schema.org/draft-07/schema#",
-                    "additionalProperties": false,
-                    "properties": {
-                        "Allocated": {
-                            "type": "number"
-                        },
-                        "Available": {
-                            "type": "number"
-                        },
-                        "FacilityId": {
-                            "type": "integer"
-                        },
-                        "ItemIdentifier": {
-                            "$schema": "http://json-schema.org/draft-07/schema#",
-                            "additionalProperties": false,
-                            "properties": {
-                                "Id": {
-                                    "type": "integer"
-                                },
-                                "Sku": {
-                                    "type": "string"
-                                }
-                            },
-                            "type": "object"
-                        },
-                        "OnHand": {
-                            "type": "number"
-                        },
-                        "OnHold": {
-                            "type": "number"
-                        },
-                        "Qualifier": {
-                            "type": "string"
-                        },
-                        "TotalReceived": {
-                            "type": "number"
-                        },
-                        "_item_identifier_id": {
-                            "type": "integer"
-                        }
-                    },
-                    "type": "object"
-                },
-                "name": "stock_summaries",
-                "source_defined_primary_key": [
-                    [
-                        "FacilityId"
-                    ],
-                    [
-                        "_item_identifier_id"
-                    ]
-                ],
-                "supported_sync_modes": [
-                    "full_refresh"
-                ]
+    "$schema": "http://json-schema.org/draft-07/schema#",
+    "additionalProperties": false,
+    "properties": {
+        "CartonId": {
+            "type": "string"
+        },
+        "Cod": {
+            "type": [
+                "null",
+                "boolean"
+            ]
+        },
+        "CodAmount": {
+            "type": [
+                "null",
+                "number"
+            ]
+        },
+        "CreateDate": {
+            "format": "date-time",
+            "type": "string"
+        },
+        "Description": {
+            "type": "string"
+        },
+        "Height": {
+            "type": [
+                "null",
+                "number"
+            ]
+        },
+        "InsuredAmount": {
+            "type": [
+                "null",
+                "number"
+            ]
+        },
+        "Label": {
+            "type": "string"
+        },
+        "Length": {
+            "type": [
+                "null",
+                "number"
+            ]
+        },
+        "Oversize": {
+            "type": [
+                "null",
+                "boolean"
+            ]
+        },
+        "PackageContents": {
+            "items": {
+                "$ref": "package_content_info.json"
             },
-            "sync_mode": "full_refresh"
+            "type": "array"
+        },
+        "PackageDefIdentifier": {
+            "$ref": "../../generic/models/package_def_identifier.json"
+        },
+        "PackageId": {
+            "type": "integer"
+        },
+        "PackageTypeId": {
+            "type": "integer"
+        },
+        "TrackingNumber": {
+            "type": "string"
+        },
+        "Ucc128": {
+            "type": [
+                "null",
+                "integer"
+            ]
+        },
+        "Weight": {
+            "type": [
+                "null",
+                "number"
+            ]
+        },
+        "Width": {
+            "type": [
+                "null",
+                "number"
+            ]
         }
-    ]
+    },
+    "type": "object"
 }
```

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/__init__.py` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/customers.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/customers.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/inventory.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/inventory.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/items.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/items.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/orders.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/orders.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/alerts.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/alerts.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/asn_pre_check.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/asn_pre_check.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/asn_pre_check_options.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/asn_pre_check_options.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/directed_put_away.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/directed_put_away.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/haz_mat.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/haz_mat.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/inventory_unit.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/inventory_unit.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/item_options.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/item_options.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/item_read_only.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/item_read_only.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/options.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/options.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/packaging.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/packaging.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/pallets.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/pallets.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/receiving.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/receiving.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/saved_element_trans_def.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/saved_element_trans_def.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/shipping.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/shipping.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/track_bys.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/track_bys.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/customer/models/user_interface.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/customer/models/user_interface.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/billing_charge_detail.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/billing_charge_detail.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/contact_info.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/contact_info.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/order_contact_info.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/order_contact_info.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/order_ship_to_info.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/order_ship_to_info.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/generic/models/other_contact_info.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/generic/models/other_contact_info.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/order/models/allocation.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/order/models/allocation.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/order/models/allocation_detail.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/order/models/allocation_detail.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/order/models/order_item.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/order/models/order_item.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/order/models/order_item_in_package.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/order/models/order_item_in_package.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/order/models/order_item_read_only.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/order/models/order_item_read_only.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/order/models/order_read_only.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/order/models/order_read_only.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/order/models/package_content_info.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/order/models/package_content_info.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/order/models/package_info.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/order/models/routing_info.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8786764705882353%*

 * *Differences: {"'properties'": "{'IsCod': OrderedDict([('type', 'boolean')]), 'IsInsurance': "*

 * *                 "OrderedDict([('type', 'boolean')]), 'RequiresDeliveryConf': "*

 * *                 "OrderedDict([('type', 'boolean')]), 'RequiresReturnReceipt': "*

 * *                 "OrderedDict([('type', 'boolean')]), 'ScacCode': OrderedDict([('type', "*

 * *                 "'string')]), 'Carrier': OrderedDict([('type', 'string')]), 'Mode': "*

 * *                 "OrderedDict([('type', 'string')]), 'Account': OrderedDict([('type', 'string […]*

```diff
@@ -1,92 +1,62 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "additionalProperties": false,
     "properties": {
-        "CartonId": {
+        "Account": {
             "type": "string"
         },
-        "Cod": {
-            "type": [
-                "null",
-                "boolean"
-            ]
+        "BillOfLading": {
+            "type": "string"
         },
-        "CodAmount": {
-            "type": [
-                "null",
-                "number"
-            ]
+        "CapacityTypeIdentifier": {
+            "$ref": "../../generic/models/capacity_type_identifier.json"
         },
-        "CreateDate": {
-            "format": "date-time",
+        "Carrier": {
             "type": "string"
         },
-        "Description": {
+        "DoorNumber": {
             "type": "string"
         },
-        "Height": {
-            "type": [
-                "null",
-                "number"
-            ]
+        "IsCod": {
+            "type": "boolean"
         },
-        "InsuredAmount": {
-            "type": [
-                "null",
-                "number"
-            ]
+        "IsInsurance": {
+            "type": "boolean"
         },
-        "Label": {
+        "LoadNumber": {
             "type": "string"
         },
-        "Length": {
-            "type": [
-                "null",
-                "number"
-            ]
+        "Mode": {
+            "type": "string"
         },
-        "Oversize": {
+        "PickupDate": {
+            "format": "date-time",
             "type": [
                 "null",
-                "boolean"
+                "string"
             ]
         },
-        "PackageContents": {
-            "items": {
-                "$ref": "package_content_info.json"
-            },
-            "type": "array"
-        },
-        "PackageDefIdentifier": {
-            "$ref": "../../generic/models/package_def_identifier.json"
+        "RequiresDeliveryConf": {
+            "type": "boolean"
         },
-        "PackageId": {
-            "type": "integer"
+        "RequiresReturnReceipt": {
+            "type": "boolean"
         },
-        "PackageTypeId": {
-            "type": "integer"
+        "ScacCode": {
+            "type": "string"
         },
-        "TrackingNumber": {
+        "SealNumber": {
             "type": "string"
         },
-        "Ucc128": {
-            "type": [
-                "null",
-                "integer"
-            ]
+        "ShipPointZip": {
+            "type": "string"
         },
-        "Weight": {
-            "type": [
-                "null",
-                "number"
-            ]
+        "TrackingNumber": {
+            "type": "string"
         },
-        "Width": {
-            "type": [
-                "null",
-                "number"
-            ]
+        "TrailerNumber": {
+            "type": "string"
         }
     },
     "type": "object"
 }
```

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/shared/order/models/parcel_option.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/shared/order/models/parcel_option.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/stock_details.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/stock_details.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/schemas/stock_summaries.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/schemas/stock_summaries.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/source.py` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/source.py`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/spec.json` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/streams.py` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte-source-tplcentral-0.1.1/source_tplcentral/util.py` & `airbyte_source_tplcentral-0.1.2/source_tplcentral/util.py`

 * *Files identical despite different names*

