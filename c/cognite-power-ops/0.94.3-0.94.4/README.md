# Comparing `tmp/cognite_power_ops-0.94.3.tar.gz` & `tmp/cognite_power_ops-0.94.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_power_ops-0.94.3.tar", max compression
+gzip compressed data, was "cognite_power_ops-0.94.4.tar", max compression
```

## Comparing `cognite_power_ops-0.94.3.tar` & `cognite_power_ops-0.94.4.tar`

### file list

```diff
@@ -1,675 +1,678 @@
--rw-r--r--   0        0        0    10758 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/LICENSE
--rw-r--r--   0        0        0     3322 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/README.md
--rw-r--r--   0        0        0      213 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/__init__.py
--rw-r--r--   0        0        0       23 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/_version.py
--rw-r--r--   0        0        0     5273 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/cdf_labels.py
--rw-r--r--   0        0        0     8997 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/cli.py
--rw-r--r--   0        0        0       74 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/__init__.py
--rw-r--r--   0        0        0      105 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/__init__.py
--rw-r--r--   0        0        0    32135 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/_core.py
--rw-r--r--   0        0        0    26235 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/alert.py
--rw-r--r--   0        0        0     1492 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/alert_query.py
--rw-r--r--   0        0        0    27110 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/bid_document.py
--rw-r--r--   0        0        0     2041 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/bid_document_alerts.py
--rw-r--r--   0        0        0     2039 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/bid_document_bids.py
--rw-r--r--   0        0        0    11759 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/bid_document_query.py
--rw-r--r--   0        0        0    16844 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/bid_method.py
--rw-r--r--   0        0        0     1513 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/bid_method_query.py
--rw-r--r--   0        0        0    27874 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/bid_row.py
--rw-r--r--   0        0        0     1971 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/bid_row_alerts.py
--rw-r--r--   0        0        0     8302 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/bid_row_query.py
--rw-r--r--   0        0        0    16131 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/price_area.py
--rw-r--r--   0        0        0    25401 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/price_area_activation_price_down.py
--rw-r--r--   0        0        0    25313 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/price_area_activation_price_up.py
--rw-r--r--   0        0        0    25313 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/price_area_capacity_price_down.py
--rw-r--r--   0        0        0    25195 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/price_area_capacity_price_up.py
--rw-r--r--   0        0        0    25692 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/price_area_own_capacity_allocation_down.py
--rw-r--r--   0        0        0    25604 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/price_area_own_capacity_allocation_up.py
--rw-r--r--   0        0        0     1513 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/price_area_query.py
--rw-r--r--   0        0        0    25330 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/price_area_relative_activation.py
--rw-r--r--   0        0        0    25780 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/price_area_total_capacity_allocation_down.py
--rw-r--r--   0        0        0    25692 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/price_area_total_capacity_allocation_up.py
--rw-r--r--   0        0        0     9211 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api_client.py
--rw-r--r--   0        0        0     2654 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/data_classes/__init__.py
--rw-r--r--   0        0        0    16231 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/data_classes/_alert.py
--rw-r--r--   0        0        0    19483 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/data_classes/_bid_document.py
--rw-r--r--   0        0        0     8200 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/data_classes/_bid_method.py
--rw-r--r--   0        0        0    23816 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/data_classes/_bid_row.py
--rw-r--r--   0        0        0    22916 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/data_classes/_core.py
--rw-r--r--   0        0        0     9041 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/data_classes/_price_area.py
--rw-r--r--   0        0        0      109 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/__init__.py
--rw-r--r--   0        0        0    32350 2024-05-13 10:44:35.772060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/_core.py
--rw-r--r--   0        0        0    16860 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/bid_method.py
--rw-r--r--   0        0        0     1511 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/bid_method_query.py
--rw-r--r--   0        0        0    26226 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/generator.py
--rw-r--r--   0        0        0    15705 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/generator_efficiency_curve.py
--rw-r--r--   0        0        0     1625 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/generator_efficiency_curve_query.py
--rw-r--r--   0        0        0    28005 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/generator_is_available_time_series.py
--rw-r--r--   0        0        0     5828 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/generator_query.py
--rw-r--r--   0        0        0    27596 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/generator_start_stop_cost.py
--rw-r--r--   0        0        0     2197 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/generator_turbine_curves.py
--rw-r--r--   0        0        0    32967 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/plant.py
--rw-r--r--   0        0        0    30394 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/plant_feeding_fee_time_series.py
--rw-r--r--   0        0        0     1998 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/plant_generators.py
--rw-r--r--   0        0        0    30394 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/plant_head_direct_time_series.py
--rw-r--r--   0        0        0    30394 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/plant_inlet_level_time_series.py
--rw-r--r--   0        0        0    30438 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/plant_outlet_level_time_series.py
--rw-r--r--   0        0        0    30100 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/plant_p_max_time_series.py
--rw-r--r--   0        0        0    30100 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/plant_p_min_time_series.py
--rw-r--r--   0        0        0     8084 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/plant_query.py
--rw-r--r--   0        0        0    30394 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/plant_water_value_time_series.py
--rw-r--r--   0        0        0    27060 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/price_area.py
--rw-r--r--   0        0        0    27668 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/price_area_activation_price_down.py
--rw-r--r--   0        0        0    27580 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/price_area_activation_price_up.py
--rw-r--r--   0        0        0    27580 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/price_area_capacity_price_down.py
--rw-r--r--   0        0        0    27462 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/price_area_capacity_price_up.py
--rw-r--r--   0        0        0    27374 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/price_area_day_ahead_price.py
--rw-r--r--   0        0        0    27739 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/price_area_main_scenario_day_ahead.py
--rw-r--r--   0        0        0    27959 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/price_area_own_capacity_allocation_down.py
--rw-r--r--   0        0        0    27871 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/price_area_own_capacity_allocation_up.py
--rw-r--r--   0        0        0     2011 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/price_area_plants.py
--rw-r--r--   0        0        0    11709 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/price_area_query.py
--rw-r--r--   0        0        0    27597 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/price_area_relative_activation.py
--rw-r--r--   0        0        0    28047 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/price_area_total_capacity_allocation_down.py
--rw-r--r--   0        0        0    27959 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/price_area_total_capacity_allocation_up.py
--rw-r--r--   0        0        0     2095 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/price_area_watercourses.py
--rw-r--r--   0        0        0    20054 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/reservoir.py
--rw-r--r--   0        0        0     1510 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/reservoir_query.py
--rw-r--r--   0        0        0    15561 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/turbine_efficiency_curve.py
--rw-r--r--   0        0        0     1615 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/turbine_efficiency_curve_query.py
--rw-r--r--   0        0        0    22125 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/watercourse.py
--rw-r--r--   0        0        0     2026 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/watercourse_plants.py
--rw-r--r--   0        0        0    26508 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/watercourse_production_obligation.py
--rw-r--r--   0        0        0     6635 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/watercourse_query.py
--rw-r--r--   0        0        0    10150 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api_client.py
--rw-r--r--   0        0        0     4810 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/data_classes/__init__.py
--rw-r--r--   0        0        0     8080 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/data_classes/_bid_method.py
--rw-r--r--   0        0        0    22916 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/data_classes/_core.py
--rw-r--r--   0        0        0    19940 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/data_classes/_generator.py
--rw-r--r--   0        0        0     9827 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/data_classes/_generator_efficiency_curve.py
--rw-r--r--   0        0        0    32140 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/data_classes/_plant.py
--rw-r--r--   0        0        0    33483 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/data_classes/_price_area.py
--rw-r--r--   0        0        0    10168 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/data_classes/_reservoir.py
--rw-r--r--   0        0        0     9697 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/data_classes/_turbine_efficiency_curve.py
--rw-r--r--   0        0        0    13872 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/data_classes/_watercourse.py
--rw-r--r--   0        0        0      113 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 10:44:35.776060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/_api/__init__.py
--rw-r--r--   0        0        0     8201 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/_api/_core.py
--rw-r--r--   0        0        0    14521 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/_api/case.py
--rw-r--r--   0        0        0     7486 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/_api/commands_config.py
--rw-r--r--   0        0        0     9780 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/_api/file_ref.py
--rw-r--r--   0        0        0    15960 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/_api/mapping.py
--rw-r--r--   0        0        0    17869 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/_api/model_template.py
--rw-r--r--   0        0        0    11367 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/_api/processing_log.py
--rw-r--r--   0        0        0    19744 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/_api/scenario.py
--rw-r--r--   0        0        0    10871 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/_api/transformation.py
--rw-r--r--   0        0        0     3003 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/_api_client.py
--rw-r--r--   0        0        0     2524 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/data_classes/__init__.py
--rw-r--r--   0        0        0     4596 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/data_classes/_case.py
--rw-r--r--   0        0        0     2226 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/data_classes/_commands_config.py
--rw-r--r--   0        0        0     5824 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/data_classes/_core.py
--rw-r--r--   0        0        0     2393 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/data_classes/_file_ref.py
--rw-r--r--   0        0        0     4586 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/data_classes/_mapping.py
--rw-r--r--   0        0        0     5174 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/data_classes/_model_template.py
--rw-r--r--   0        0        0     2819 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/data_classes/_processing_log.py
--rw-r--r--   0        0        0     6951 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/data_classes/_scenario.py
--rw-r--r--   0        0        0     2621 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/data_classes/_transformation.py
--rw-r--r--   0        0        0      118 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/__init__.py
--rw-r--r--   0        0        0    32598 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/_core.py
--rw-r--r--   0        0        0    26333 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/alert.py
--rw-r--r--   0        0        0     1497 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/alert_query.py
--rw-r--r--   0        0        0    23471 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/basic_bid_matrix.py
--rw-r--r--   0        0        0     2115 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/basic_bid_matrix_alerts.py
--rw-r--r--   0        0        0     7177 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/basic_bid_matrix_query.py
--rw-r--r--   0        0        0    29138 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document.py
--rw-r--r--   0        0        0     2059 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document_alerts.py
--rw-r--r--   0        0        0     2106 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document_partials.py
--rw-r--r--   0        0        0    13622 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document_query.py
--rw-r--r--   0        0        0    22831 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_matrix.py
--rw-r--r--   0        0        0     2032 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_matrix_alerts.py
--rw-r--r--   0        0        0     7128 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_matrix_query.py
--rw-r--r--   0        0        0    16942 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_method.py
--rw-r--r--   0        0        0     1518 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_method_query.py
--rw-r--r--   0        0        0    24946 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix.py
--rw-r--r--   0        0        0     2185 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix_alerts.py
--rw-r--r--   0        0        0    10308 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix_query.py
--rw-r--r--   0        0        0     2410 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix_scenario_results.py
--rw-r--r--   0        0        0    19843 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area.py
--rw-r--r--   0        0        0    25798 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area_main_scenario.py
--rw-r--r--   0        0        0    25883 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area_price_scenarios.py
--rw-r--r--   0        0        0     2613 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area_query.py
--rw-r--r--   0        0        0    20327 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_multi_scenario_method.py
--rw-r--r--   0        0        0     2415 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_multi_scenario_method_price_scenarios.py
--rw-r--r--   0        0        0     4483 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_multi_scenario_method_query.py
--rw-r--r--   0        0        0    18030 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario.py
--rw-r--r--   0        0        0    24799 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_price.py
--rw-r--r--   0        0        0     1559 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_query.py
--rw-r--r--   0        0        0    15855 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result.py
--rw-r--r--   0        0        0    24935 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result_price.py
--rw-r--r--   0        0        0    25177 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result_production.py
--rw-r--r--   0        0        0     2777 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result_query.py
--rw-r--r--   0        0        0    18424 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/water_value_based_method.py
--rw-r--r--   0        0        0     1618 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/water_value_based_method_query.py
--rw-r--r--   0        0        0    11242 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api_client.py
--rw-r--r--   0        0        0     7397 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/data_classes/__init__.py
--rw-r--r--   0        0        0    16231 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_alert.py
--rw-r--r--   0        0        0    14798 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_basic_bid_matrix.py
--rw-r--r--   0        0        0    24120 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_bid_document.py
--rw-r--r--   0        0        0    15156 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_bid_matrix.py
--rw-r--r--   0        0        0     8094 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_bid_method.py
--rw-r--r--   0        0        0    22916 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_core.py
--rw-r--r--   0        0        0    17204 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_multi_scenario_matrix.py
--rw-r--r--   0        0        0    14748 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_price_area.py
--rw-r--r--   0        0        0    11974 2024-05-13 10:44:35.780060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_shop_multi_scenario_method.py
--rw-r--r--   0        0        0     9405 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_shop_price_scenario.py
--rw-r--r--   0        0        0    13294 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_shop_price_scenario_result.py
--rw-r--r--   0        0        0     8961 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_water_value_based_method.py
--rw-r--r--   0        0        0      123 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/__init__.py
--rw-r--r--   0        0        0    41803 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/_core.py
--rw-r--r--   0        0        0    28392 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/alert.py
--rw-r--r--   0        0        0     1486 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/alert_query.py
--rw-r--r--   0        0        0    24852 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_configuration_day_ahead.py
--rw-r--r--   0        0        0     2445 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_configuration_day_ahead_partials.py
--rw-r--r--   0        0        0     7859 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_configuration_day_ahead_query.py
--rw-r--r--   0        0        0    27557 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_document.py
--rw-r--r--   0        0        0    29838 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_document_afrr.py
--rw-r--r--   0        0        0     2125 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_document_afrr_alerts.py
--rw-r--r--   0        0        0     2123 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_document_afrr_bids.py
--rw-r--r--   0        0        0    11654 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_document_afrr_query.py
--rw-r--r--   0        0        0     2056 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_document_alerts.py
--rw-r--r--   0        0        0    31537 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead.py
--rw-r--r--   0        0        0     2194 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead_alerts.py
--rw-r--r--   0        0        0     2399 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead_partials.py
--rw-r--r--   0        0        0    13156 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead_query.py
--rw-r--r--   0        0        0     6256 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_document_query.py
--rw-r--r--   0        0        0    16995 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_matrix.py
--rw-r--r--   0        0        0    20707 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_matrix_information.py
--rw-r--r--   0        0        0     2194 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_matrix_information_alerts.py
--rw-r--r--   0        0        0     2352 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_matrix_information_intermediate_bid_matrices.py
--rw-r--r--   0        0        0     9120 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_matrix_information_query.py
--rw-r--r--   0        0        0     1507 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_matrix_query.py
--rw-r--r--   0        0        0    24990 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_row.py
--rw-r--r--   0        0        0     1986 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_row_alerts.py
--rw-r--r--   0        0        0     8727 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_row_query.py
--rw-r--r--   0        0        0    23488 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/function_input.py
--rw-r--r--   0        0        0     1527 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/function_input_query.py
--rw-r--r--   0        0        0    26010 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/function_output.py
--rw-r--r--   0        0        0     2098 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/function_output_alerts.py
--rw-r--r--   0        0        0     7530 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/function_output_query.py
--rw-r--r--   0        0        0    30503 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/generator.py
--rw-r--r--   0        0        0    29640 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/generator_availability_time_series.py
--rw-r--r--   0        0        0    14623 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/generator_efficiency_curve.py
--rw-r--r--   0        0        0     1621 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/generator_efficiency_curve_query.py
--rw-r--r--   0        0        0     5996 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/generator_query.py
--rw-r--r--   0        0        0    29214 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/generator_start_stop_cost.py
--rw-r--r--   0        0        0     2275 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/generator_turbine_efficiency_curves.py
--rw-r--r--   0        0        0    30967 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/market_configuration.py
--rw-r--r--   0        0        0     1557 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/market_configuration_query.py
--rw-r--r--   0        0        0    21738 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/partial_bid_configuration.py
--rw-r--r--   0        0        0     2719 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/partial_bid_configuration_query.py
--rw-r--r--   0        0        0    30364 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_input.py
--rw-r--r--   0        0        0     4187 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_input_query.py
--rw-r--r--   0        0        0    31040 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_output.py
--rw-r--r--   0        0        0     2403 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_output_alerts.py
--rw-r--r--   0        0        0    10702 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_output_query.py
--rw-r--r--   0        0        0    26004 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information.py
--rw-r--r--   0        0        0     2305 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_alerts.py
--rw-r--r--   0        0        0     2463 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_intermediate_bid_matrices.py
--rw-r--r--   0        0        0    12658 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_query.py
--rw-r--r--   0        0        0    29102 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios.py
--rw-r--r--   0        0        0     2502 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_alerts.py
--rw-r--r--   0        0        0     2660 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_intermediate_bid_matrices.py
--rw-r--r--   0        0        0     2676 2024-05-13 10:44:35.784060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_multi_scenario_input.py
--rw-r--r--   0        0        0    16509 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_query.py
--rw-r--r--   0        0        0    21267 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant.py
--rw-r--r--   0        0        0    34870 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_information.py
--rw-r--r--   0        0        0    31031 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_information_feeding_fee_time_series.py
--rw-r--r--   0        0        0     2177 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_information_generators.py
--rw-r--r--   0        0        0    31031 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_information_head_direct_time_series.py
--rw-r--r--   0        0        0    31031 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_information_inlet_level_time_series.py
--rw-r--r--   0        0        0    31075 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_information_outlet_level_time_series.py
--rw-r--r--   0        0        0    31163 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_information_production_max_time_series.py
--rw-r--r--   0        0        0    31163 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_information_production_min_time_series.py
--rw-r--r--   0        0        0     6307 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_information_query.py
--rw-r--r--   0        0        0    31031 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_information_water_value_time_series.py
--rw-r--r--   0        0        0     1486 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_query.py
--rw-r--r--   0        0        0    35566 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_water_value_based.py
--rw-r--r--   0        0        0    31218 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_feeding_fee_time_series.py
--rw-r--r--   0        0        0     2260 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_generators.py
--rw-r--r--   0        0        0    31218 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_head_direct_time_series.py
--rw-r--r--   0        0        0    31218 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_inlet_level_time_series.py
--rw-r--r--   0        0        0    31262 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_outlet_level_time_series.py
--rw-r--r--   0        0        0    31350 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_production_max_time_series.py
--rw-r--r--   0        0        0    31350 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_production_min_time_series.py
--rw-r--r--   0        0        0     6373 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_query.py
--rw-r--r--   0        0        0    31218 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_water_value_time_series.py
--rw-r--r--   0        0        0    21879 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/power_asset.py
--rw-r--r--   0        0        0     1512 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/power_asset_query.py
--rw-r--r--   0        0        0    21768 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area.py
--rw-r--r--   0        0        0    23928 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_afrr.py
--rw-r--r--   0        0        0    27423 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_afrr_activation_price_down.py
--rw-r--r--   0        0        0    27335 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_afrr_activation_price_up.py
--rw-r--r--   0        0        0    27335 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_afrr_capacity_price_down.py
--rw-r--r--   0        0        0    27217 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_afrr_capacity_price_up.py
--rw-r--r--   0        0        0    27714 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_afrr_own_capacity_allocation_down.py
--rw-r--r--   0        0        0    27626 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_afrr_own_capacity_allocation_up.py
--rw-r--r--   0        0        0     1528 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_afrr_query.py
--rw-r--r--   0        0        0    27352 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_afrr_relative_activation.py
--rw-r--r--   0        0        0    27802 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_afrr_total_capacity_allocation_down.py
--rw-r--r--   0        0        0    27714 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_afrr_total_capacity_allocation_up.py
--rw-r--r--   0        0        0    24500 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead.py
--rw-r--r--   0        0        0    27713 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead_main_price_scenario.py
--rw-r--r--   0        0        0    27521 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead_price_scenarios.py
--rw-r--r--   0        0        0     2794 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead_query.py
--rw-r--r--   0        0        0    26627 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_information.py
--rw-r--r--   0        0        0    28169 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_information_activation_price_down.py
--rw-r--r--   0        0        0    28081 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_information_activation_price_up.py
--rw-r--r--   0        0        0    28081 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_information_capacity_price_down.py
--rw-r--r--   0        0        0    27963 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_information_capacity_price_up.py
--rw-r--r--   0        0        0    28081 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_information_main_price_scenario.py
--rw-r--r--   0        0        0    28460 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_information_own_capacity_allocation_down.py
--rw-r--r--   0        0        0    28372 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_information_own_capacity_allocation_up.py
--rw-r--r--   0        0        0    27889 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_information_price_scenarios.py
--rw-r--r--   0        0        0     2851 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_information_query.py
--rw-r--r--   0        0        0    28098 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_information_relative_activation.py
--rw-r--r--   0        0        0    28548 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_information_total_capacity_allocation_down.py
--rw-r--r--   0        0        0    28460 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_information_total_capacity_allocation_up.py
--rw-r--r--   0        0        0     1507 2024-05-13 10:44:35.788060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_query.py
--rw-r--r--   0        0        0    18930 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_production.py
--rw-r--r--   0        0        0    25079 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_production_price.py
--rw-r--r--   0        0        0    25321 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_production_production.py
--rw-r--r--   0        0        0     2623 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_production_query.py
--rw-r--r--   0        0        0    25220 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_attribute_mapping.py
--rw-r--r--   0        0        0     1601 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_attribute_mapping_query.py
--rw-r--r--   0        0        0    27660 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_attribute_mapping_time_series.py
--rw-r--r--   0        0        0    24151 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_based_partial_bid_configuration.py
--rw-r--r--   0        0        0     3878 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_based_partial_bid_configuration_query.py
--rw-r--r--   0        0        0    18438 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_case.py
--rw-r--r--   0        0        0     6064 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_case_query.py
--rw-r--r--   0        0        0     2071 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_case_shop_files.py
--rw-r--r--   0        0        0    17214 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_commands.py
--rw-r--r--   0        0        0     1521 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_commands_query.py
--rw-r--r--   0        0        0    20249 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_file.py
--rw-r--r--   0        0        0     1502 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_file_query.py
--rw-r--r--   0        0        0    23570 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_model.py
--rw-r--r--   0        0        0     2279 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_model_base_attribute_mappings.py
--rw-r--r--   0        0        0     5631 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_model_query.py
--rw-r--r--   0        0        0    32763 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_partial_bid_matrix_calculation_input.py
--rw-r--r--   0        0        0     2608 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_partial_bid_matrix_calculation_input_price_production.py
--rw-r--r--   0        0        0     7877 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_partial_bid_matrix_calculation_input_query.py
--rw-r--r--   0        0        0    29852 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_penalty_report.py
--rw-r--r--   0        0        0     1548 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_penalty_report_query.py
--rw-r--r--   0        0        0    29105 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_input.py
--rw-r--r--   0        0        0     2688 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_input_query.py
--rw-r--r--   0        0        0    27944 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_output.py
--rw-r--r--   0        0        0     2223 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_output_alerts.py
--rw-r--r--   0        0        0     8858 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_output_query.py
--rw-r--r--   0        0        0    16377 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_result.py
--rw-r--r--   0        0        0     2042 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_result_alerts.py
--rw-r--r--   0        0        0     2214 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_result_output_time_series.py
--rw-r--r--   0        0        0    11103 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_result_query.py
--rw-r--r--   0        0        0    22289 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_scenario.py
--rw-r--r--   0        0        0     2338 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_scenario_attribute_mappings_override.py
--rw-r--r--   0        0        0     8104 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_scenario_query.py
--rw-r--r--   0        0        0    23085 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_scenario_set.py
--rw-r--r--   0        0        0     4851 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_scenario_set_query.py
--rw-r--r--   0        0        0     2216 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_scenario_set_scenarios.py
--rw-r--r--   0        0        0    21375 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_time_series.py
--rw-r--r--   0        0        0     1533 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_time_series_query.py
--rw-r--r--   0        0        0    26338 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_time_series_time_series.py
--rw-r--r--   0        0        0    27685 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_trigger_input.py
--rw-r--r--   0        0        0     3695 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_trigger_input_query.py
--rw-r--r--   0        0        0    27490 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_trigger_output.py
--rw-r--r--   0        0        0     2153 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_trigger_output_alerts.py
--rw-r--r--   0        0        0     8841 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_trigger_output_query.py
--rw-r--r--   0        0        0    27145 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/task_dispatcher_input.py
--rw-r--r--   0        0        0     2743 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/task_dispatcher_input_query.py
--rw-r--r--   0        0        0    27652 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output.py
--rw-r--r--   0        0        0     2195 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output_alerts.py
--rw-r--r--   0        0        0     2330 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output_process_sub_tasks.py
--rw-r--r--   0        0        0    11719 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output_query.py
--rw-r--r--   0        0        0    30353 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_input.py
--rw-r--r--   0        0        0     2477 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_input_partial_bid_matrices.py
--rw-r--r--   0        0        0     5956 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_input_query.py
--rw-r--r--   0        0        0    29442 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_output.py
--rw-r--r--   0        0        0     2375 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_output_alerts.py
--rw-r--r--   0        0        0     9141 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_output_query.py
--rw-r--r--   0        0        0    15615 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/turbine_efficiency_curve.py
--rw-r--r--   0        0        0     1611 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/turbine_efficiency_curve_query.py
--rw-r--r--   0        0        0    24038 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_configuration.py
--rw-r--r--   0        0        0     2906 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_configuration_query.py
--rw-r--r--   0        0        0    32573 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_matrix_calculation_input.py
--rw-r--r--   0        0        0     4476 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_matrix_calculation_input_query.py
--rw-r--r--   0        0        0    21933 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/watercourse.py
--rw-r--r--   0        0        0     1516 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/watercourse_query.py
--rw-r--r--   0        0        0    44629 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api_client.py
--rw-r--r--   0        0        0    37530 2024-05-13 10:44:35.792060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/__init__.py
--rw-r--r--   0        0        0    17776 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_alert.py
--rw-r--r--   0        0        0    19097 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_bid_configuration_day_ahead.py
--rw-r--r--   0        0        0    17055 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_bid_document.py
--rw-r--r--   0        0        0    20377 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_bid_document_afrr.py
--rw-r--r--   0        0        0    24090 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_bid_document_day_ahead.py
--rw-r--r--   0        0        0     8899 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_bid_matrix.py
--rw-r--r--   0        0        0    13521 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_bid_matrix_information.py
--rw-r--r--   0        0        0    21991 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_bid_row.py
--rw-r--r--   0        0        0    22919 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_core.py
--rw-r--r--   0        0        0    12488 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_function_input.py
--rw-r--r--   0        0        0    16546 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_function_output.py
--rw-r--r--   0        0        0    23123 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_generator.py
--rw-r--r--   0        0        0     9234 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_generator_efficiency_curve.py
--rw-r--r--   0        0        0    16741 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_market_configuration.py
--rw-r--r--   0        0        0    13579 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_configuration.py
--rw-r--r--   0        0        0    21950 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_calculation_input.py
--rw-r--r--   0        0        0    23555 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_calculation_output.py
--rw-r--r--   0        0        0    21084 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_information.py
--rw-r--r--   0        0        0    23573 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_information_with_scenarios.py
--rw-r--r--   0        0        0    10552 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_plant.py
--rw-r--r--   0        0        0    26558 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_plant_information.py
--rw-r--r--   0        0        0    29359 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_plant_water_value_based.py
--rw-r--r--   0        0        0    11245 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_power_asset.py
--rw-r--r--   0        0        0    10801 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_price_area.py
--rw-r--r--   0        0        0    23345 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_price_area_afrr.py
--rw-r--r--   0        0        0    17926 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_price_area_day_ahead.py
--rw-r--r--   0        0        0    28027 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_price_area_information.py
--rw-r--r--   0        0        0    13204 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_price_production.py
--rw-r--r--   0        0        0    15412 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_shop_attribute_mapping.py
--rw-r--r--   0        0        0    16843 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_shop_based_partial_bid_configuration.py
--rw-r--r--   0        0        0    14508 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_shop_case.py
--rw-r--r--   0        0        0     8933 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_shop_commands.py
--rw-r--r--   0        0        0    11434 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_shop_file.py
--rw-r--r--   0        0        0    16868 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_shop_model.py
--rw-r--r--   0        0        0    24050 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_shop_partial_bid_matrix_calculation_input.py
--rw-r--r--   0        0        0    18171 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_shop_penalty_report.py
--rw-r--r--   0        0        0    17791 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_shop_preprocessor_input.py
--rw-r--r--   0        0        0    18602 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_shop_preprocessor_output.py
--rw-r--r--   0        0        0    17342 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_shop_result.py
--rw-r--r--   0        0        0    17049 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_shop_scenario.py
--rw-r--r--   0        0        0    13264 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_shop_scenario_set.py
--rw-r--r--   0        0        0    12545 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_shop_time_series.py
--rw-r--r--   0        0        0    19594 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_shop_trigger_input.py
--rw-r--r--   0        0        0    18692 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_shop_trigger_output.py
--rw-r--r--   0        0        0    17272 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_task_dispatcher_input.py
--rw-r--r--   0        0        0    18343 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_task_dispatcher_output.py
--rw-r--r--   0        0        0    20134 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_total_bid_matrix_calculation_input.py
--rw-r--r--   0        0        0    19932 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_total_bid_matrix_calculation_output.py
--rw-r--r--   0        0        0     9709 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_turbine_efficiency_curve.py
--rw-r--r--   0        0        0    14472 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_water_value_based_partial_bid_configuration.py
--rw-r--r--   0        0        0    22567 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_water_value_based_partial_bid_matrix_calculation_input.py
--rw-r--r--   0        0        0    10900 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_watercourse.py
--rw-r--r--   0        0        0     1301 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/_logger.py
--rw-r--r--   0        0        0      139 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/data_classes.py
--rw-r--r--   0        0        0     1322 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/data_set_api.py
--rw-r--r--   0        0        0     6750 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/powerops_client.py
--rw-r--r--   0        0        0       62 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/shop/__init__.py
--rw-r--r--   0        0        0      885 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/shop/_api_client.py
--rw-r--r--   0        0        0        0 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/shop/api/__init__.py
--rw-r--r--   0        0        0     8367 2024-05-13 10:44:35.796060 cognite_power_ops-0.94.3/cognite/powerops/client/shop/api/dayahead_trigger_api.py
--rw-r--r--   0        0        0     4797 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/client/shop/api/shop_result_files_api.py
--rw-r--r--   0        0        0     4432 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/client/shop/api/shop_results_api.py
--rw-r--r--   0        0        0     9593 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/client/shop/api/shop_run_api.py
--rw-r--r--   0        0        0      600 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/client/shop/data_classes/__init__.py
--rw-r--r--   0        0        0     4114 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/client/shop/data_classes/case.py
--rw-r--r--   0        0        0     9057 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/client/shop/data_classes/dayahead_trigger.py
--rw-r--r--   0        0        0     2720 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/client/shop/data_classes/helpers.py
--rw-r--r--   0        0        0      603 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/client/shop/data_classes/plotting.py
--rw-r--r--   0        0        0     6164 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/client/shop/data_classes/shop_result_files.py
--rw-r--r--   0        0        0     6607 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/client/shop/data_classes/shop_results.py
--rw-r--r--   0        0        0    10210 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/client/shop/data_classes/shop_results_compare.py
--rw-r--r--   0        0        0     3021 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/client/shop/data_classes/shop_run.py
--rw-r--r--   0        0        0     3743 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/client/shop/data_classes/shop_run_event.py
--rw-r--r--   0        0        0     4374 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/client/shop/shop_case.py
--rw-r--r--   0        0        0     1101 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/client/shop/shop_file_reference.py
--rw-r--r--   0        0        0    13466 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/client/shop/shop_run.py
--rw-r--r--   0        0        0    15419 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/client/shop/shop_run_api.py
--rw-r--r--   0        0        0     3885 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/client/shop/shop_run_filter.py
--rw-r--r--   0        0        0      563 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/client/shop/utils.py
--rw-r--r--   0        0        0      947 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/cognite_modules/_system.yaml
--rw-r--r--   0        0        0     1941 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/config.dev.yaml
--rw-r--r--   0        0        0      729 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/AFRRBid.datamodel.yaml
--rw-r--r--   0        0        0     1095 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/Asset.datamodel.yaml
--rw-r--r--   0        0        0     1680 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/DayAheadBid.datamodel.yaml
--rw-r--r--   0        0        0      100 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/affr_space.space.yaml
--rw-r--r--   0        0        0       92 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/asset.space.yaml
--rw-r--r--   0        0        0      367 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/containers/AFRRBid-BidMethod.container.yaml
--rw-r--r--   0        0        0     2102 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/containers/AFRRBid-BidRow.container.yaml
--rw-r--r--   0        0        0      750 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/containers/asset-EfficiencyCurve.container.yaml
--rw-r--r--   0        0        0     1380 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Alert.container.yaml
--rw-r--r--   0        0        0      857 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Asset.container.yaml
--rw-r--r--   0        0        0     1038 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-BidDocument.container.yaml
--rw-r--r--   0        0        0      502 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-BidMethod.container.yaml
--rw-r--r--   0        0        0     1408 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Generator.container.yaml
--rw-r--r--   0        0        0     2281 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Plant.container.yaml
--rw-r--r--   0        0        0     2375 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-PriceArea.container.yaml
--rw-r--r--   0        0        0      556 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Watercourse.container.yaml
--rw-r--r--   0        0        0      466 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-BidDocument.container.yaml
--rw-r--r--   0        0        0      767 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-BidMatrix.container.yaml
--rw-r--r--   0        0        0      371 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-BidMethod.container.yaml
--rw-r--r--   0        0        0      532 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-MultiScenarioMatrix.container.yaml
--rw-r--r--   0        0        0      618 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-SHOPMultiScenario.container.yaml
--rw-r--r--   0        0        0      416 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-SHOPPriceScenario.container.yaml
--rw-r--r--   0        0        0      490 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-SHOPPriceScenarioResults.container.yaml
--rw-r--r--   0        0        0      113 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/dayahead_space.space.yaml
--rw-r--r--   0        0        0      118 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/instance.space.yaml
--rw-r--r--   0        0        0     1515 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/node_types/power-ops-types.powerops_nodes.yaml
--rw-r--r--   0        0        0      116 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/shared.space.yaml
--rw-r--r--   0        0        0       81 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/types.space.yaml
--rw-r--r--   0        0        0     1379 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-BidDocument.view.yaml
--rw-r--r--   0        0        0      606 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-BidMethod.view.yaml
--rw-r--r--   0        0        0     3917 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-BidRow.view.yaml
--rw-r--r--   0        0        0     2786 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-PriceArea.view.yaml
--rw-r--r--   0        0        0     2618 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Generator.view.yaml
--rw-r--r--   0        0        0     1138 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-GeneratorEfficiency.view.yaml
--rw-r--r--   0        0        0     5199 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Plant.view.yaml
--rw-r--r--   0        0        0     5204 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-PriceArea.view.yaml
--rw-r--r--   0        0        0     1060 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Reservoir.view.yaml
--rw-r--r--   0        0        0     1121 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-TurbineEfficiency.view.yaml
--rw-r--r--   0        0        0     1887 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Watercourse.view.yaml
--rw-r--r--   0        0        0     2558 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/baseBids-Alert.view.yaml
--rw-r--r--   0        0        0     2374 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/baseBids-BidDocument.view.yaml
--rw-r--r--   0        0        0      858 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/baseBids-BidMethod.view.yaml
--rw-r--r--   0        0        0      579 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BasicBidMatrix.view.yaml
--rw-r--r--   0        0        0     1945 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BidDocument.view.yaml
--rw-r--r--   0        0        0     1845 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BidMatrix.view.yaml
--rw-r--r--   0        0        0      723 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BidMethod.view.yaml
--rw-r--r--   0        0        0      700 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-CustomBidMatrix.view.yaml
--rw-r--r--   0        0        0      711 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-CustomBidMethod.view.yaml
--rw-r--r--   0        0        0     1015 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-MultiScenarioMatrix.view.yaml
--rw-r--r--   0        0        0     1479 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-PriceArea.view.yaml
--rw-r--r--   0        0        0     1312 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-SHOPMultiScenarioMethod.view.yaml
--rw-r--r--   0        0        0      666 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-SHOPPriceScenario.view.yaml
--rw-r--r--   0        0        0     1230 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-SHOPPriceScenarioResult.view.yaml
--rw-r--r--   0        0        0      605 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-WaterValueBasedMethod.view.yaml
--rw-r--r--   0        0        0     4964 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/all_DayAhead.datamodel.yaml
--rw-r--r--   0        0        0     6519 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/all_PowerOps.datamodel.yaml
--rw-r--r--   0        0        0     2052 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/compute_DayAheadBenchmarking.datamodel.yaml
--rw-r--r--   0        0        0     3499 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/compute_SHOPBasedDayAhead.datamodel.yaml
--rw-r--r--   0        0        0     2918 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/compute_TotalBidMatrixCalculation.datamodel.yaml
--rw-r--r--   0        0        0     2575 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/compute_WaterValueBasedDayAhead.datamodel.yaml
--rw-r--r--   0        0        0     2276 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/config_DayAheadConfiguration.datamodel.yaml
--rw-r--r--   0        0        0     2163 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/config_Resync.datamodel.yaml
--rw-r--r--   0        0        0     1748 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/Alert.container.yaml
--rw-r--r--   0        0        0      814 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidConfiguration.container.yaml
--rw-r--r--   0        0        0     1292 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidDocument.container.yaml
--rw-r--r--   0        0        0      496 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidDocumentDayAhead.container.yaml
--rw-r--r--   0        0        0      771 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidMatrix.container.yaml
--rw-r--r--   0        0        0     1659 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidRow.container.yaml
--rw-r--r--   0        0        0      755 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/EfficiencyCurve.container.yaml
--rw-r--r--   0        0        0     3521 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/FunctionData.container.yaml
--rw-r--r--   0        0        0     1038 2024-05-13 10:44:35.800060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/Generator.container.yaml
--rw-r--r--   0        0        0     2082 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/MarketConfiguration.container.yaml
--rw-r--r--   0        0        0      756 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PartialBidConfiguration.container.yaml
--rw-r--r--   0        0        0     2425 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PlantWaterValueBased.container.yaml
--rw-r--r--   0        0        0     1076 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PowerAsset.container.yaml
--rw-r--r--   0        0        0     1628 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PriceAreaAFRR.container.yaml
--rw-r--r--   0        0        0      689 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PriceAreaDayAhead.container.yaml
--rw-r--r--   0        0        0      710 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PriceProduction.container.yaml
--rw-r--r--   0        0        0      504 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/SHOPObjectiveValue.container.yaml
--rw-r--r--   0        0        0     1074 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/SHOPResult.container.yaml
--rw-r--r--   0        0        0     1106 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/SHOPTimeSeries.container.yaml
--rw-r--r--   0        0        0     1462 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopAttributeMapping.container.yaml
--rw-r--r--   0        0        0      634 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopCase.container.yaml
--rw-r--r--   0        0        0      464 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopCommands.container.yaml
--rw-r--r--   0        0        0     1128 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopFile.container.yaml
--rw-r--r--   0        0        0     1446 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopModel.container.yaml
--rw-r--r--   0        0        0      280 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopPartialBidConfiguration.container.yaml
--rw-r--r--   0        0        0      978 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopScenario.container.yaml
--rw-r--r--   0        0        0      690 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopScenarioSet.container.yaml
--rw-r--r--   0        0        0      869 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/frontend_AFRRBid.datamodel.yaml
--rw-r--r--   0        0        0     1789 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/frontend_Asset.datamodel.yaml
--rw-r--r--   0        0        0     2661 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/frontend_DayAheadBid.datamodel.yaml
--rw-r--r--   0        0        0      118 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/instance.space.yaml
--rw-r--r--   0        0        0      104 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/models.space.yaml
--rw-r--r--   0        0        0     5275 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/node_types/power-ops-types.powerops_nodes.yaml
--rw-r--r--   0        0        0      854 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/product_CogShop.datamodel.yaml
--rw-r--r--   0        0        0       91 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/type.space.yaml
--rw-r--r--   0        0        0     3704 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/BidRow.view.yaml
--rw-r--r--   0        0        0     2834 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/MarketConfiguration.view.yaml
--rw-r--r--   0        0        0     2983 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/alerts/1-interface.Alert.view.yaml
--rw-r--r--   0        0        0      871 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/alerts/ShopPenaltyReport.view.yaml
--rw-r--r--   0        0        0     1283 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/1-interface.PowerAsset.view.yaml
--rw-r--r--   0        0        0     2330 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/generator/Generator.view.yaml
--rw-r--r--   0        0        0     1073 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/generator/GeneratorEfficiencyCurve.view.yaml
--rw-r--r--   0        0        0     1260 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/generator/TurbineEfficiencyCurve.view.yaml
--rw-r--r--   0        0        0      535 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/plant/1-interface.Plant.view.yaml
--rw-r--r--   0        0        0      599 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/plant/PlantInformation.view.yaml
--rw-r--r--   0        0        0     4498 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/plant/PlantWaterValueBased.view.yaml
--rw-r--r--   0        0        0      512 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/1-interface.PriceArea.view.yaml
--rw-r--r--   0        0        0     2932 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/PriceAreaAFRR.view.yaml
--rw-r--r--   0        0        0     1659 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/PriceAreaDayAhead.view.yaml
--rw-r--r--   0        0        0      596 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/PriceAreaInformation.view.yaml
--rw-r--r--   0        0        0      543 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/watercourse/1-interface.Watercourse.view.yaml
--rw-r--r--   0        0        0     1476 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/1-interface.PartialBidConfiguration.view.yaml
--rw-r--r--   0        0        0     2264 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/BidConfigurationDayAhead.view.yaml
--rw-r--r--   0        0        0     1059 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/ShopBasedPartialBidConfiguration.view.yaml
--rw-r--r--   0        0        0     1184 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/WaterValueBasedPartialBidConfiguration.view.yaml
--rw-r--r--   0        0        0     2520 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/1-interface.BidDocument.view.yaml
--rw-r--r--   0        0        0     1450 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/BidDocumentAFRR.view.yaml
--rw-r--r--   0        0        0     1726 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/BidDocumentDayAhead.view.yaml
--rw-r--r--   0        0        0     1564 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/BidDocumentDayAheadSimple.view.yaml
--rw-r--r--   0        0        0      701 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/1-interface.BidMatrix.view.yaml
--rw-r--r--   0        0        0     1225 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/1-interface.BidMatrixInformation.view.yaml
--rw-r--r--   0        0        0     1349 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/1-interface.PartialBidMatrixInformation.view.yaml
--rw-r--r--   0        0        0      890 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/PartialBidMatrixInformationWithScenarios.view.yaml
--rw-r--r--   0        0        0     2331 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopAttributeMapping.view.yaml
--rw-r--r--   0        0        0     1840 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopCase.view.yaml
--rw-r--r--   0        0        0     1027 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopCommands.view.yaml
--rw-r--r--   0        0        0     1705 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopFile.view.yaml
--rw-r--r--   0        0        0     2573 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopModel.view.yaml
--rw-r--r--   0        0        0     1965 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopScenario.view.yaml
--rw-r--r--   0        0        0     1535 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopScenarioSet.view.yaml
--rw-r--r--   0        0        0     1399 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/1-interface.FunctionInput.view.yaml
--rw-r--r--   0        0        0     1797 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/1-interface.PartialBidMatrixCalculationInput.view.yaml
--rw-r--r--   0        0        0     1053 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/BenchmarkingCollectorInput.view.yaml
--rw-r--r--   0        0        0     1750 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/ShopPartialBidMatrixCalculationInput.view.yaml
--rw-r--r--   0        0        0     1522 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/ShopPreprocessorInput.view.yaml
--rw-r--r--   0        0        0     1660 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/ShopTriggerInput.view.yaml
--rw-r--r--   0        0        0     1069 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/TaskDispatcherBenchmarkingInput.view.yaml
--rw-r--r--   0        0        0     1249 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/TaskDispatcherInput.view.yaml
--rw-r--r--   0        0        0     1680 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/TotalBidMatrixCalculationInput.view.yaml
--rw-r--r--   0        0        0     1336 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/WaterPartialBidMatrixCalculationInput.view.yaml
--rw-r--r--   0        0        0     2119 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/1-interface.FunctionOutput.view.yaml
--rw-r--r--   0        0        0      981 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/BenchmarkingCollectorOutput.view.yaml
--rw-r--r--   0        0        0     1757 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/PartialBidMatrixCalculationOutput.view.yaml
--rw-r--r--   0        0        0     1355 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/SHOPTriggerOutput.view.yaml
--rw-r--r--   0        0        0     1426 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/ShopPreprocessorOutput.view.yaml
--rw-r--r--   0        0        0     1010 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/TaskDispatcherBenchmarkingOutput.view.yaml
--rw-r--r--   0        0        0     1378 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/TaskDispatcherOutput.view.yaml
--rw-r--r--   0        0        0     1434 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/TotalBidMatrixCalculationOutput.view.yaml
--rw-r--r--   0        0        0     1392 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/PriceProduction.view.yaml
--rw-r--r--   0        0        0     2707 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/SHOPResult.view.yaml
--rw-r--r--   0        0        0     1587 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/SHOPTimeSeries.view.yaml
--rw-r--r--   0        0        0     1114 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/ShopObjectiveValue.view.yaml
--rw-r--r--   0        0        0        0 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/prerun_transformations/__init__.py
--rw-r--r--   0        0        0    34098 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/prerun_transformations/transformations.py
--rw-r--r--   0        0        0      394 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/resync/__init__.py
--rw-r--r--   0        0        0     1792 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/resync/config/__init__.py
--rw-r--r--   0        0        0    12764 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/resync/config/_main.py
--rw-r--r--   0        0        0      595 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/resync/config/_settings.py
--rw-r--r--   0        0        0    12408 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/resync/config/_shared.py
--rw-r--r--   0        0        0       75 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/resync/config/cogshop/__init__.py
--rw-r--r--   0        0        0      720 2024-05-13 10:44:35.804060 cognite_power_ops-0.94.3/cognite/powerops/resync/config/cogshop/shop_file_config.py
--rw-r--r--   0        0        0      815 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/config/market/__init__.py
--rw-r--r--   0        0        0     5486 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/config/market/_core.py
--rw-r--r--   0        0        0     2106 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/config/market/benchmarking.py
--rw-r--r--   0        0        0     2105 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/config/market/dayahead.py
--rw-r--r--   0        0        0      961 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/config/market/market.py
--rw-r--r--   0        0        0    10827 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/config/market/rkom.py
--rw-r--r--   0        0        0      417 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/config/production/__init__.py
--rw-r--r--   0        0        0      830 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/config/production/connections.py
--rw-r--r--   0        0        0     1414 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/config/production/generator.py
--rw-r--r--   0        0        0     5675 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/config/production/plant.py
--rw-r--r--   0        0        0     2868 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/config/production/watercourse.py
--rw-r--r--   0        0        0      244 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/core/__init__.py
--rw-r--r--   0        0        0     9185 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/core/cdf.py
--rw-r--r--   0        0        0      442 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/core/echo.py
--rw-r--r--   0        0        0    27692 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/core/main.py
--rw-r--r--   0        0        0     2563 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/core/transform.py
--rw-r--r--   0        0        0     2161 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/core/validation.py
--rw-r--r--   0        0        0      474 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/diff/__init__.py
--rw-r--r--   0        0        0     6774 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/diff/core.py
--rw-r--r--   0        0        0    12631 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/diff/data_classes.py
--rw-r--r--   0        0        0      424 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/models/__init__.py
--rw-r--r--   0        0        0       82 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/models/_shared_v1_v2/__init__.py
--rw-r--r--   0        0        0      811 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/models/_shared_v1_v2/_to_instances.py
--rw-r--r--   0        0        0    10495 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/models/_shared_v1_v2/cogshop_model.py
--rw-r--r--   0        0        0     1143 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/models/_shared_v1_v2/market_model.py
--rw-r--r--   0        0        0     8337 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/models/_shared_v1_v2/production_model.py
--rw-r--r--   0        0        0      788 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/models/base/__init__.py
--rw-r--r--   0        0        0    11195 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/models/base/asset_model.py
--rw-r--r--   0        0        0     9602 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/models/base/asset_type.py
--rw-r--r--   0        0        0     5251 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/models/base/cdf_resources.py
--rw-r--r--   0        0        0    11641 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/models/base/data_model.py
--rw-r--r--   0        0        0     1896 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/models/base/dms_models.py
--rw-r--r--   0        0        0      592 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/models/base/graph_ql.py
--rw-r--r--   0        0        0      148 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/models/base/helpers.py
--rw-r--r--   0        0        0     6668 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/models/base/model.py
--rw-r--r--   0        0        0     1705 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/models/base/resource_type.py
--rw-r--r--   0        0        0     1302 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/models/v1/__init__.py
--rw-r--r--   0        0        0     8141 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/models/v1/cogshop.py
--rw-r--r--   0        0        0      243 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/models/v1/config_to_model/__init__.py
--rw-r--r--   0        0        0     8940 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/models/v1/config_to_model/to_cogshop_model.py
--rw-r--r--   0        0        0    15631 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/models/v1/config_to_model/to_market_model.py
--rw-r--r--   0        0        0     9726 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/models/v1/config_to_model/to_production_model.py
--rw-r--r--   0        0        0      491 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/models/v1/graphql_schemas/__init__.py
--rw-r--r--   0        0        0      832 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/models/v1/graphql_schemas/cogshop1.graphql
--rw-r--r--   0        0        0     3499 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/models/v1/market/__init__.py
--rw-r--r--   0        0        0     1291 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/models/v1/market/base.py
--rw-r--r--   0        0        0     3184 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/models/v1/market/benchmark.py
--rw-r--r--   0        0        0     2405 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/models/v1/market/dayahead.py
--rw-r--r--   0        0        0     2797 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/models/v1/market/rkom.py
--rw-r--r--   0        0        0     7801 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/models/v1/production.py
--rw-r--r--   0        0        0      395 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/models/v2/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/models/v2/config_to_model/__init__.py
--rw-r--r--   0        0        0     8873 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/models/v2/config_to_model/to_powerasset_model.py
--rw-r--r--   0        0        0    27181 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/models/v2/powerops_models.py
--rw-r--r--   0        0        0     7631 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/models/v2/production_dm.py
--rw-r--r--   0        0        0      150 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/time_series_mapping/__init__.py
--rw-r--r--   0        0        0     2149 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/time_series_mapping/mapping.py
--rw-r--r--   0        0        0     2456 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/time_series_mapping/static_mapping.py
--rw-r--r--   0        0        0     6585 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/v1/README.md
--rw-r--r--   0        0        0       59 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/v1/__init__.py
--rw-r--r--   0        0        0    29458 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/v1/config_to_fdm.py
--rw-r--r--   0        0        0    14948 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/v1/data_classes.py
--rw-r--r--   0        0        0     2931 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/v1/main.py
--rw-r--r--   0        0        0    12112 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/v1/utils.py
--rw-r--r--   0        0        0     4524 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/resync/validation.py
--rw-r--r--   0        0        0        0 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/utils/__init__.py
--rw-r--r--   0        0        0      160 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/utils/cdf/__init__.py
--rw-r--r--   0        0        0     1389 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/utils/cdf/_cdf_auth.py
--rw-r--r--   0        0        0     3169 2024-05-13 10:44:35.808060 cognite_power_ops-0.94.3/cognite/powerops/utils/cdf/_settings.py
--rw-r--r--   0        0        0     7517 2024-05-13 10:44:35.812060 cognite_power_ops-0.94.3/cognite/powerops/utils/cdf/calls.py
--rw-r--r--   0        0        0    10874 2024-05-13 10:44:35.812060 cognite_power_ops-0.94.3/cognite/powerops/utils/cdf/extraction_pipelines.py
--rw-r--r--   0        0        0      970 2024-05-13 10:44:35.812060 cognite_power_ops-0.94.3/cognite/powerops/utils/cdf/resource_creation.py
--rw-r--r--   0        0        0     2540 2024-05-13 10:44:35.812060 cognite_power_ops-0.94.3/cognite/powerops/utils/lookup.py
--rw-r--r--   0        0        0     1097 2024-05-13 10:44:35.812060 cognite_power_ops-0.94.3/cognite/powerops/utils/navigation.py
--rw-r--r--   0        0        0      514 2024-05-13 10:44:35.812060 cognite_power_ops-0.94.3/cognite/powerops/utils/require.py
--rw-r--r--   0        0        0      227 2024-05-13 10:44:35.812060 cognite_power_ops-0.94.3/cognite/powerops/utils/retry/__init__.py
--rw-r--r--   0        0        0     5619 2024-05-13 10:44:35.812060 cognite_power_ops-0.94.3/cognite/powerops/utils/retry/api.py
--rw-r--r--   0        0        0     7828 2024-05-13 10:44:35.812060 cognite_power_ops-0.94.3/cognite/powerops/utils/serialization.py
--rw-r--r--   0        0        0     3667 2024-05-13 10:44:35.812060 cognite_power_ops-0.94.3/cognite/powerops/utils/time.py
--rw-r--r--   0        0        0     3732 2024-05-13 10:44:35.812060 cognite_power_ops-0.94.3/pyproject.toml
--rw-r--r--   0        0        0     5525 1970-01-01 00:00:00.000000 cognite_power_ops-0.94.3/PKG-INFO
+-rw-r--r--   0        0        0    10758 2024-05-30 13:24:25.494284 cognite_power_ops-0.94.4/LICENSE
+-rw-r--r--   0        0        0     3322 2024-05-30 13:24:25.494284 cognite_power_ops-0.94.4/README.md
+-rw-r--r--   0        0        0      213 2024-05-30 13:24:25.494284 cognite_power_ops-0.94.4/cognite/powerops/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-30 13:24:25.494284 cognite_power_ops-0.94.4/cognite/powerops/_version.py
+-rw-r--r--   0        0        0     5273 2024-05-30 13:24:25.494284 cognite_power_ops-0.94.4/cognite/powerops/cdf_labels.py
+-rw-r--r--   0        0        0     8997 2024-05-30 13:24:25.494284 cognite_power_ops-0.94.4/cognite/powerops/cli.py
+-rw-r--r--   0        0        0       74 2024-05-30 13:24:25.494284 cognite_power_ops-0.94.4/cognite/powerops/client/__init__.py
+-rw-r--r--   0        0        0      105 2024-05-30 13:24:25.494284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 13:24:25.494284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/__init__.py
+-rw-r--r--   0        0        0    32135 2024-05-30 13:24:25.494284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/_core.py
+-rw-r--r--   0        0        0    26235 2024-05-30 13:24:25.494284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/alert.py
+-rw-r--r--   0        0        0     1492 2024-05-30 13:24:25.494284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/alert_query.py
+-rw-r--r--   0        0        0    27110 2024-05-30 13:24:25.494284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/bid_document.py
+-rw-r--r--   0        0        0     2041 2024-05-30 13:24:25.494284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/bid_document_alerts.py
+-rw-r--r--   0        0        0     2039 2024-05-30 13:24:25.494284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/bid_document_bids.py
+-rw-r--r--   0        0        0    11759 2024-05-30 13:24:25.494284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/bid_document_query.py
+-rw-r--r--   0        0        0    16844 2024-05-30 13:24:25.494284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/bid_method.py
+-rw-r--r--   0        0        0     1513 2024-05-30 13:24:25.494284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/bid_method_query.py
+-rw-r--r--   0        0        0    27874 2024-05-30 13:24:25.494284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/bid_row.py
+-rw-r--r--   0        0        0     1971 2024-05-30 13:24:25.494284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/bid_row_alerts.py
+-rw-r--r--   0        0        0     8302 2024-05-30 13:24:25.494284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/bid_row_query.py
+-rw-r--r--   0        0        0    16131 2024-05-30 13:24:25.494284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/price_area.py
+-rw-r--r--   0        0        0    25401 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/price_area_activation_price_down.py
+-rw-r--r--   0        0        0    25313 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/price_area_activation_price_up.py
+-rw-r--r--   0        0        0    25313 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/price_area_capacity_price_down.py
+-rw-r--r--   0        0        0    25195 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/price_area_capacity_price_up.py
+-rw-r--r--   0        0        0    25692 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/price_area_own_capacity_allocation_down.py
+-rw-r--r--   0        0        0    25604 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/price_area_own_capacity_allocation_up.py
+-rw-r--r--   0        0        0     1513 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/price_area_query.py
+-rw-r--r--   0        0        0    25330 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/price_area_relative_activation.py
+-rw-r--r--   0        0        0    25780 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/price_area_total_capacity_allocation_down.py
+-rw-r--r--   0        0        0    25692 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/price_area_total_capacity_allocation_up.py
+-rw-r--r--   0        0        0     9211 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api_client.py
+-rw-r--r--   0        0        0     2654 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/data_classes/__init__.py
+-rw-r--r--   0        0        0    16231 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/data_classes/_alert.py
+-rw-r--r--   0        0        0    19483 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/data_classes/_bid_document.py
+-rw-r--r--   0        0        0     8200 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/data_classes/_bid_method.py
+-rw-r--r--   0        0        0    23816 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/data_classes/_bid_row.py
+-rw-r--r--   0        0        0    22916 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/data_classes/_core.py
+-rw-r--r--   0        0        0     9041 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/data_classes/_price_area.py
+-rw-r--r--   0        0        0      109 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/__init__.py
+-rw-r--r--   0        0        0    32350 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/_core.py
+-rw-r--r--   0        0        0    16860 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/bid_method.py
+-rw-r--r--   0        0        0     1511 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/bid_method_query.py
+-rw-r--r--   0        0        0    26226 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/generator.py
+-rw-r--r--   0        0        0    15705 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/generator_efficiency_curve.py
+-rw-r--r--   0        0        0     1625 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/generator_efficiency_curve_query.py
+-rw-r--r--   0        0        0    28005 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/generator_is_available_time_series.py
+-rw-r--r--   0        0        0     5828 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/generator_query.py
+-rw-r--r--   0        0        0    27596 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/generator_start_stop_cost.py
+-rw-r--r--   0        0        0     2197 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/generator_turbine_curves.py
+-rw-r--r--   0        0        0    32967 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/plant.py
+-rw-r--r--   0        0        0    30394 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/plant_feeding_fee_time_series.py
+-rw-r--r--   0        0        0     1998 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/plant_generators.py
+-rw-r--r--   0        0        0    30394 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/plant_head_direct_time_series.py
+-rw-r--r--   0        0        0    30394 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/plant_inlet_level_time_series.py
+-rw-r--r--   0        0        0    30438 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/plant_outlet_level_time_series.py
+-rw-r--r--   0        0        0    30100 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/plant_p_max_time_series.py
+-rw-r--r--   0        0        0    30100 2024-05-30 13:24:25.498284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/plant_p_min_time_series.py
+-rw-r--r--   0        0        0     8084 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/plant_query.py
+-rw-r--r--   0        0        0    30394 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/plant_water_value_time_series.py
+-rw-r--r--   0        0        0    27060 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/price_area.py
+-rw-r--r--   0        0        0    27668 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/price_area_activation_price_down.py
+-rw-r--r--   0        0        0    27580 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/price_area_activation_price_up.py
+-rw-r--r--   0        0        0    27580 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/price_area_capacity_price_down.py
+-rw-r--r--   0        0        0    27462 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/price_area_capacity_price_up.py
+-rw-r--r--   0        0        0    27374 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/price_area_day_ahead_price.py
+-rw-r--r--   0        0        0    27739 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/price_area_main_scenario_day_ahead.py
+-rw-r--r--   0        0        0    27959 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/price_area_own_capacity_allocation_down.py
+-rw-r--r--   0        0        0    27871 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/price_area_own_capacity_allocation_up.py
+-rw-r--r--   0        0        0     2011 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/price_area_plants.py
+-rw-r--r--   0        0        0    11709 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/price_area_query.py
+-rw-r--r--   0        0        0    27597 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/price_area_relative_activation.py
+-rw-r--r--   0        0        0    28047 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/price_area_total_capacity_allocation_down.py
+-rw-r--r--   0        0        0    27959 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/price_area_total_capacity_allocation_up.py
+-rw-r--r--   0        0        0     2095 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/price_area_watercourses.py
+-rw-r--r--   0        0        0    20054 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/reservoir.py
+-rw-r--r--   0        0        0     1510 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/reservoir_query.py
+-rw-r--r--   0        0        0    15561 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/turbine_efficiency_curve.py
+-rw-r--r--   0        0        0     1615 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/turbine_efficiency_curve_query.py
+-rw-r--r--   0        0        0    22125 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/watercourse.py
+-rw-r--r--   0        0        0     2026 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/watercourse_plants.py
+-rw-r--r--   0        0        0    26508 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/watercourse_production_obligation.py
+-rw-r--r--   0        0        0     6635 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/watercourse_query.py
+-rw-r--r--   0        0        0    10150 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api_client.py
+-rw-r--r--   0        0        0     4810 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/data_classes/__init__.py
+-rw-r--r--   0        0        0     8080 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/data_classes/_bid_method.py
+-rw-r--r--   0        0        0    22916 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/data_classes/_core.py
+-rw-r--r--   0        0        0    19940 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/data_classes/_generator.py
+-rw-r--r--   0        0        0     9827 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/data_classes/_generator_efficiency_curve.py
+-rw-r--r--   0        0        0    32140 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/data_classes/_plant.py
+-rw-r--r--   0        0        0    33483 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/data_classes/_price_area.py
+-rw-r--r--   0        0        0    10168 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/data_classes/_reservoir.py
+-rw-r--r--   0        0        0     9697 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/data_classes/_turbine_efficiency_curve.py
+-rw-r--r--   0        0        0    13872 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/data_classes/_watercourse.py
+-rw-r--r--   0        0        0      113 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/_api/__init__.py
+-rw-r--r--   0        0        0     8201 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/_api/_core.py
+-rw-r--r--   0        0        0    14521 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/_api/case.py
+-rw-r--r--   0        0        0     7486 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/_api/commands_config.py
+-rw-r--r--   0        0        0     9780 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/_api/file_ref.py
+-rw-r--r--   0        0        0    15960 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/_api/mapping.py
+-rw-r--r--   0        0        0    17869 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/_api/model_template.py
+-rw-r--r--   0        0        0    11367 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/_api/processing_log.py
+-rw-r--r--   0        0        0    19744 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/_api/scenario.py
+-rw-r--r--   0        0        0    10871 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/_api/transformation.py
+-rw-r--r--   0        0        0     3003 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/_api_client.py
+-rw-r--r--   0        0        0     2524 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/data_classes/__init__.py
+-rw-r--r--   0        0        0     4596 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/data_classes/_case.py
+-rw-r--r--   0        0        0     2226 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/data_classes/_commands_config.py
+-rw-r--r--   0        0        0     5824 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/data_classes/_core.py
+-rw-r--r--   0        0        0     2393 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/data_classes/_file_ref.py
+-rw-r--r--   0        0        0     4586 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/data_classes/_mapping.py
+-rw-r--r--   0        0        0     5174 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/data_classes/_model_template.py
+-rw-r--r--   0        0        0     2819 2024-05-30 13:24:25.502284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/data_classes/_processing_log.py
+-rw-r--r--   0        0        0     6951 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/data_classes/_scenario.py
+-rw-r--r--   0        0        0     2621 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/data_classes/_transformation.py
+-rw-r--r--   0        0        0      118 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/__init__.py
+-rw-r--r--   0        0        0    32598 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/_core.py
+-rw-r--r--   0        0        0    26333 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/alert.py
+-rw-r--r--   0        0        0     1497 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/alert_query.py
+-rw-r--r--   0        0        0    23471 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/basic_bid_matrix.py
+-rw-r--r--   0        0        0     2115 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/basic_bid_matrix_alerts.py
+-rw-r--r--   0        0        0     7177 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/basic_bid_matrix_query.py
+-rw-r--r--   0        0        0    29138 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document.py
+-rw-r--r--   0        0        0     2059 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document_alerts.py
+-rw-r--r--   0        0        0     2106 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document_partials.py
+-rw-r--r--   0        0        0    13622 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document_query.py
+-rw-r--r--   0        0        0    22831 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_matrix.py
+-rw-r--r--   0        0        0     2032 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_matrix_alerts.py
+-rw-r--r--   0        0        0     7128 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_matrix_query.py
+-rw-r--r--   0        0        0    16942 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_method.py
+-rw-r--r--   0        0        0     1518 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_method_query.py
+-rw-r--r--   0        0        0    24946 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix.py
+-rw-r--r--   0        0        0     2185 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix_alerts.py
+-rw-r--r--   0        0        0    10308 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix_query.py
+-rw-r--r--   0        0        0     2410 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix_scenario_results.py
+-rw-r--r--   0        0        0    19843 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area.py
+-rw-r--r--   0        0        0    25798 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area_main_scenario.py
+-rw-r--r--   0        0        0    25883 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area_price_scenarios.py
+-rw-r--r--   0        0        0     2613 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area_query.py
+-rw-r--r--   0        0        0    20327 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_multi_scenario_method.py
+-rw-r--r--   0        0        0     2415 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_multi_scenario_method_price_scenarios.py
+-rw-r--r--   0        0        0     4483 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_multi_scenario_method_query.py
+-rw-r--r--   0        0        0    18030 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario.py
+-rw-r--r--   0        0        0    24799 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_price.py
+-rw-r--r--   0        0        0     1559 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_query.py
+-rw-r--r--   0        0        0    15855 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result.py
+-rw-r--r--   0        0        0    24935 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result_price.py
+-rw-r--r--   0        0        0    25177 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result_production.py
+-rw-r--r--   0        0        0     2777 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result_query.py
+-rw-r--r--   0        0        0    18424 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/water_value_based_method.py
+-rw-r--r--   0        0        0     1618 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/water_value_based_method_query.py
+-rw-r--r--   0        0        0    11242 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api_client.py
+-rw-r--r--   0        0        0     7397 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/data_classes/__init__.py
+-rw-r--r--   0        0        0    16231 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_alert.py
+-rw-r--r--   0        0        0    14798 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_basic_bid_matrix.py
+-rw-r--r--   0        0        0    24120 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_bid_document.py
+-rw-r--r--   0        0        0    15156 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_bid_matrix.py
+-rw-r--r--   0        0        0     8094 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_bid_method.py
+-rw-r--r--   0        0        0    22916 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_core.py
+-rw-r--r--   0        0        0    17204 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_multi_scenario_matrix.py
+-rw-r--r--   0        0        0    14748 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_price_area.py
+-rw-r--r--   0        0        0    11974 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_shop_multi_scenario_method.py
+-rw-r--r--   0        0        0     9405 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_shop_price_scenario.py
+-rw-r--r--   0        0        0    13294 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_shop_price_scenario_result.py
+-rw-r--r--   0        0        0     8961 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_water_value_based_method.py
+-rw-r--r--   0        0        0      123 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/__init__.py
+-rw-r--r--   0        0        0    41803 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/_core.py
+-rw-r--r--   0        0        0    28392 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/alert.py
+-rw-r--r--   0        0        0     1486 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/alert_query.py
+-rw-r--r--   0        0        0    24852 2024-05-30 13:24:25.506284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_configuration_day_ahead.py
+-rw-r--r--   0        0        0     2445 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_configuration_day_ahead_partials.py
+-rw-r--r--   0        0        0     7859 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_configuration_day_ahead_query.py
+-rw-r--r--   0        0        0    27557 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_document.py
+-rw-r--r--   0        0        0    29838 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_document_afrr.py
+-rw-r--r--   0        0        0     2125 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_document_afrr_alerts.py
+-rw-r--r--   0        0        0     2123 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_document_afrr_bids.py
+-rw-r--r--   0        0        0    11654 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_document_afrr_query.py
+-rw-r--r--   0        0        0     2056 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_document_alerts.py
+-rw-r--r--   0        0        0    31537 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead.py
+-rw-r--r--   0        0        0     2194 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead_alerts.py
+-rw-r--r--   0        0        0     2399 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead_partials.py
+-rw-r--r--   0        0        0    13156 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead_query.py
+-rw-r--r--   0        0        0     6256 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_document_query.py
+-rw-r--r--   0        0        0    16995 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_matrix.py
+-rw-r--r--   0        0        0    20707 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_matrix_information.py
+-rw-r--r--   0        0        0     2194 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_matrix_information_alerts.py
+-rw-r--r--   0        0        0     2352 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_matrix_information_intermediate_bid_matrices.py
+-rw-r--r--   0        0        0     9120 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_matrix_information_query.py
+-rw-r--r--   0        0        0     1507 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_matrix_query.py
+-rw-r--r--   0        0        0    24990 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_row.py
+-rw-r--r--   0        0        0     1986 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_row_alerts.py
+-rw-r--r--   0        0        0     8727 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_row_query.py
+-rw-r--r--   0        0        0    23488 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/function_input.py
+-rw-r--r--   0        0        0     1527 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/function_input_query.py
+-rw-r--r--   0        0        0    26010 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/function_output.py
+-rw-r--r--   0        0        0     2098 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/function_output_alerts.py
+-rw-r--r--   0        0        0     7530 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/function_output_query.py
+-rw-r--r--   0        0        0    30503 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/generator.py
+-rw-r--r--   0        0        0    29640 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/generator_availability_time_series.py
+-rw-r--r--   0        0        0    14623 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/generator_efficiency_curve.py
+-rw-r--r--   0        0        0     1621 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/generator_efficiency_curve_query.py
+-rw-r--r--   0        0        0     5996 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/generator_query.py
+-rw-r--r--   0        0        0    29214 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/generator_start_stop_cost.py
+-rw-r--r--   0        0        0     2275 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/generator_turbine_efficiency_curves.py
+-rw-r--r--   0        0        0    30967 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/market_configuration.py
+-rw-r--r--   0        0        0     1557 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/market_configuration_query.py
+-rw-r--r--   0        0        0    21738 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/partial_bid_configuration.py
+-rw-r--r--   0        0        0     2719 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/partial_bid_configuration_query.py
+-rw-r--r--   0        0        0    30364 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_input.py
+-rw-r--r--   0        0        0     4187 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_input_query.py
+-rw-r--r--   0        0        0    31040 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_output.py
+-rw-r--r--   0        0        0     2403 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_output_alerts.py
+-rw-r--r--   0        0        0    10702 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_output_query.py
+-rw-r--r--   0        0        0    26004 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information.py
+-rw-r--r--   0        0        0     2305 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_alerts.py
+-rw-r--r--   0        0        0     2463 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_intermediate_bid_matrices.py
+-rw-r--r--   0        0        0    12658 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_query.py
+-rw-r--r--   0        0        0    29102 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios.py
+-rw-r--r--   0        0        0     2502 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_alerts.py
+-rw-r--r--   0        0        0     2660 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_intermediate_bid_matrices.py
+-rw-r--r--   0        0        0     2676 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_multi_scenario_input.py
+-rw-r--r--   0        0        0    16509 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_query.py
+-rw-r--r--   0        0        0    21267 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant.py
+-rw-r--r--   0        0        0    34870 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_information.py
+-rw-r--r--   0        0        0    31031 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_information_feeding_fee_time_series.py
+-rw-r--r--   0        0        0     2177 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_information_generators.py
+-rw-r--r--   0        0        0    31031 2024-05-30 13:24:25.510284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_information_head_direct_time_series.py
+-rw-r--r--   0        0        0    31031 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_information_inlet_level_time_series.py
+-rw-r--r--   0        0        0    31075 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_information_outlet_level_time_series.py
+-rw-r--r--   0        0        0    31163 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_information_production_max_time_series.py
+-rw-r--r--   0        0        0    31163 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_information_production_min_time_series.py
+-rw-r--r--   0        0        0     6307 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_information_query.py
+-rw-r--r--   0        0        0    31031 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_information_water_value_time_series.py
+-rw-r--r--   0        0        0     1486 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_query.py
+-rw-r--r--   0        0        0    35566 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_water_value_based.py
+-rw-r--r--   0        0        0    31218 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_feeding_fee_time_series.py
+-rw-r--r--   0        0        0     2260 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_generators.py
+-rw-r--r--   0        0        0    31218 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_head_direct_time_series.py
+-rw-r--r--   0        0        0    31218 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_inlet_level_time_series.py
+-rw-r--r--   0        0        0    31262 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_outlet_level_time_series.py
+-rw-r--r--   0        0        0    31350 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_production_max_time_series.py
+-rw-r--r--   0        0        0    31350 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_production_min_time_series.py
+-rw-r--r--   0        0        0     6373 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_query.py
+-rw-r--r--   0        0        0    31218 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_water_value_time_series.py
+-rw-r--r--   0        0        0    21879 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/power_asset.py
+-rw-r--r--   0        0        0     1512 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/power_asset_query.py
+-rw-r--r--   0        0        0    21768 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area.py
+-rw-r--r--   0        0        0    23928 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_afrr.py
+-rw-r--r--   0        0        0    27423 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_afrr_activation_price_down.py
+-rw-r--r--   0        0        0    27335 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_afrr_activation_price_up.py
+-rw-r--r--   0        0        0    27335 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_afrr_capacity_price_down.py
+-rw-r--r--   0        0        0    27217 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_afrr_capacity_price_up.py
+-rw-r--r--   0        0        0    27714 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_afrr_own_capacity_allocation_down.py
+-rw-r--r--   0        0        0    27626 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_afrr_own_capacity_allocation_up.py
+-rw-r--r--   0        0        0     1528 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_afrr_query.py
+-rw-r--r--   0        0        0    27352 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_afrr_relative_activation.py
+-rw-r--r--   0        0        0    27802 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_afrr_total_capacity_allocation_down.py
+-rw-r--r--   0        0        0    27714 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_afrr_total_capacity_allocation_up.py
+-rw-r--r--   0        0        0    24500 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead.py
+-rw-r--r--   0        0        0    27713 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead_main_price_scenario.py
+-rw-r--r--   0        0        0    27521 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead_price_scenarios.py
+-rw-r--r--   0        0        0     2794 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead_query.py
+-rw-r--r--   0        0        0    26627 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_information.py
+-rw-r--r--   0        0        0    28169 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_information_activation_price_down.py
+-rw-r--r--   0        0        0    28081 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_information_activation_price_up.py
+-rw-r--r--   0        0        0    28081 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_information_capacity_price_down.py
+-rw-r--r--   0        0        0    27963 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_information_capacity_price_up.py
+-rw-r--r--   0        0        0    28081 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_information_main_price_scenario.py
+-rw-r--r--   0        0        0    28460 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_information_own_capacity_allocation_down.py
+-rw-r--r--   0        0        0    28372 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_information_own_capacity_allocation_up.py
+-rw-r--r--   0        0        0    27889 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_information_price_scenarios.py
+-rw-r--r--   0        0        0     2851 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_information_query.py
+-rw-r--r--   0        0        0    28098 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_information_relative_activation.py
+-rw-r--r--   0        0        0    28548 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_information_total_capacity_allocation_down.py
+-rw-r--r--   0        0        0    28460 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_information_total_capacity_allocation_up.py
+-rw-r--r--   0        0        0     1507 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_query.py
+-rw-r--r--   0        0        0    18930 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_production.py
+-rw-r--r--   0        0        0    25079 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_production_price.py
+-rw-r--r--   0        0        0    25321 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_production_production.py
+-rw-r--r--   0        0        0     2623 2024-05-30 13:24:25.514284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_production_query.py
+-rw-r--r--   0        0        0    25220 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_attribute_mapping.py
+-rw-r--r--   0        0        0     1601 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_attribute_mapping_query.py
+-rw-r--r--   0        0        0    27660 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_attribute_mapping_time_series.py
+-rw-r--r--   0        0        0    24151 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_based_partial_bid_configuration.py
+-rw-r--r--   0        0        0     3878 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_based_partial_bid_configuration_query.py
+-rw-r--r--   0        0        0    18438 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_case.py
+-rw-r--r--   0        0        0     6064 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_case_query.py
+-rw-r--r--   0        0        0     2071 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_case_shop_files.py
+-rw-r--r--   0        0        0    17214 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_commands.py
+-rw-r--r--   0        0        0     1521 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_commands_query.py
+-rw-r--r--   0        0        0    20249 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_file.py
+-rw-r--r--   0        0        0     1502 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_file_query.py
+-rw-r--r--   0        0        0    23570 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_model.py
+-rw-r--r--   0        0        0     2279 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_model_base_attribute_mappings.py
+-rw-r--r--   0        0        0     5631 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_model_query.py
+-rw-r--r--   0        0        0    32763 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_partial_bid_matrix_calculation_input.py
+-rw-r--r--   0        0        0     2608 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_partial_bid_matrix_calculation_input_price_production.py
+-rw-r--r--   0        0        0     7877 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_partial_bid_matrix_calculation_input_query.py
+-rw-r--r--   0        0        0    29852 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_penalty_report.py
+-rw-r--r--   0        0        0     1548 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_penalty_report_query.py
+-rw-r--r--   0        0        0    29105 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_input.py
+-rw-r--r--   0        0        0     2688 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_input_query.py
+-rw-r--r--   0        0        0    27944 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_output.py
+-rw-r--r--   0        0        0     2223 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_output_alerts.py
+-rw-r--r--   0        0        0     8858 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_output_query.py
+-rw-r--r--   0        0        0    16377 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_result.py
+-rw-r--r--   0        0        0     2042 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_result_alerts.py
+-rw-r--r--   0        0        0     2214 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_result_output_time_series.py
+-rw-r--r--   0        0        0    11103 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_result_query.py
+-rw-r--r--   0        0        0    22289 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_scenario.py
+-rw-r--r--   0        0        0     2338 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_scenario_attribute_mappings_override.py
+-rw-r--r--   0        0        0     8104 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_scenario_query.py
+-rw-r--r--   0        0        0    23085 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_scenario_set.py
+-rw-r--r--   0        0        0     4851 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_scenario_set_query.py
+-rw-r--r--   0        0        0     2216 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_scenario_set_scenarios.py
+-rw-r--r--   0        0        0    21375 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_time_series.py
+-rw-r--r--   0        0        0     1533 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_time_series_query.py
+-rw-r--r--   0        0        0    26338 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_time_series_time_series.py
+-rw-r--r--   0        0        0    27685 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_trigger_input.py
+-rw-r--r--   0        0        0     3695 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_trigger_input_query.py
+-rw-r--r--   0        0        0    27490 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_trigger_output.py
+-rw-r--r--   0        0        0     2153 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_trigger_output_alerts.py
+-rw-r--r--   0        0        0     8841 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_trigger_output_query.py
+-rw-r--r--   0        0        0    27145 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/task_dispatcher_input.py
+-rw-r--r--   0        0        0     2743 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/task_dispatcher_input_query.py
+-rw-r--r--   0        0        0    27652 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output.py
+-rw-r--r--   0        0        0     2195 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output_alerts.py
+-rw-r--r--   0        0        0     2330 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output_process_sub_tasks.py
+-rw-r--r--   0        0        0    11719 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output_query.py
+-rw-r--r--   0        0        0    30353 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_input.py
+-rw-r--r--   0        0        0     2477 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_input_partial_bid_matrices.py
+-rw-r--r--   0        0        0     5956 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_input_query.py
+-rw-r--r--   0        0        0    29442 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_output.py
+-rw-r--r--   0        0        0     2375 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_output_alerts.py
+-rw-r--r--   0        0        0     9141 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_output_query.py
+-rw-r--r--   0        0        0    15615 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/turbine_efficiency_curve.py
+-rw-r--r--   0        0        0     1611 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/turbine_efficiency_curve_query.py
+-rw-r--r--   0        0        0    24038 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_configuration.py
+-rw-r--r--   0        0        0     2906 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_configuration_query.py
+-rw-r--r--   0        0        0    32573 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_matrix_calculation_input.py
+-rw-r--r--   0        0        0     4476 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_matrix_calculation_input_query.py
+-rw-r--r--   0        0        0    21933 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/watercourse.py
+-rw-r--r--   0        0        0     1516 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/watercourse_query.py
+-rw-r--r--   0        0        0    44629 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api_client.py
+-rw-r--r--   0        0        0    37530 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/__init__.py
+-rw-r--r--   0        0        0    17776 2024-05-30 13:24:25.518284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_alert.py
+-rw-r--r--   0        0        0    19097 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_bid_configuration_day_ahead.py
+-rw-r--r--   0        0        0    17055 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_bid_document.py
+-rw-r--r--   0        0        0    20377 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_bid_document_afrr.py
+-rw-r--r--   0        0        0    24090 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_bid_document_day_ahead.py
+-rw-r--r--   0        0        0     8899 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_bid_matrix.py
+-rw-r--r--   0        0        0    13521 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_bid_matrix_information.py
+-rw-r--r--   0        0        0    21991 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_bid_row.py
+-rw-r--r--   0        0        0    22919 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_core.py
+-rw-r--r--   0        0        0    12488 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_function_input.py
+-rw-r--r--   0        0        0    16546 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_function_output.py
+-rw-r--r--   0        0        0    23123 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_generator.py
+-rw-r--r--   0        0        0     9234 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_generator_efficiency_curve.py
+-rw-r--r--   0        0        0    16741 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_market_configuration.py
+-rw-r--r--   0        0        0    13579 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_configuration.py
+-rw-r--r--   0        0        0    21950 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_calculation_input.py
+-rw-r--r--   0        0        0    23555 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_calculation_output.py
+-rw-r--r--   0        0        0    21084 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_information.py
+-rw-r--r--   0        0        0    23573 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_information_with_scenarios.py
+-rw-r--r--   0        0        0    10552 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_plant.py
+-rw-r--r--   0        0        0    26558 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_plant_information.py
+-rw-r--r--   0        0        0    29359 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_plant_water_value_based.py
+-rw-r--r--   0        0        0    11245 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_power_asset.py
+-rw-r--r--   0        0        0    10801 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_price_area.py
+-rw-r--r--   0        0        0    23345 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_price_area_afrr.py
+-rw-r--r--   0        0        0    17926 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_price_area_day_ahead.py
+-rw-r--r--   0        0        0    28027 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_price_area_information.py
+-rw-r--r--   0        0        0    13204 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_price_production.py
+-rw-r--r--   0        0        0    15412 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_shop_attribute_mapping.py
+-rw-r--r--   0        0        0    16843 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_shop_based_partial_bid_configuration.py
+-rw-r--r--   0        0        0    14508 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_shop_case.py
+-rw-r--r--   0        0        0     8933 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_shop_commands.py
+-rw-r--r--   0        0        0    11434 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_shop_file.py
+-rw-r--r--   0        0        0    16868 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_shop_model.py
+-rw-r--r--   0        0        0    24050 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_shop_partial_bid_matrix_calculation_input.py
+-rw-r--r--   0        0        0    18171 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_shop_penalty_report.py
+-rw-r--r--   0        0        0    17791 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_shop_preprocessor_input.py
+-rw-r--r--   0        0        0    18602 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_shop_preprocessor_output.py
+-rw-r--r--   0        0        0    17342 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_shop_result.py
+-rw-r--r--   0        0        0    17049 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_shop_scenario.py
+-rw-r--r--   0        0        0    13264 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_shop_scenario_set.py
+-rw-r--r--   0        0        0    12545 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_shop_time_series.py
+-rw-r--r--   0        0        0    19594 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_shop_trigger_input.py
+-rw-r--r--   0        0        0    18692 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_shop_trigger_output.py
+-rw-r--r--   0        0        0    17272 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_task_dispatcher_input.py
+-rw-r--r--   0        0        0    18343 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_task_dispatcher_output.py
+-rw-r--r--   0        0        0    20134 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_total_bid_matrix_calculation_input.py
+-rw-r--r--   0        0        0    19932 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_total_bid_matrix_calculation_output.py
+-rw-r--r--   0        0        0     9709 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_turbine_efficiency_curve.py
+-rw-r--r--   0        0        0    14472 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_water_value_based_partial_bid_configuration.py
+-rw-r--r--   0        0        0    22567 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_water_value_based_partial_bid_matrix_calculation_input.py
+-rw-r--r--   0        0        0    10900 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_watercourse.py
+-rw-r--r--   0        0        0     1301 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/_logger.py
+-rw-r--r--   0        0        0      139 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/data_classes.py
+-rw-r--r--   0        0        0     1322 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/data_set_api.py
+-rw-r--r--   0        0        0     6750 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/powerops_client.py
+-rw-r--r--   0        0        0       62 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/shop/__init__.py
+-rw-r--r--   0        0        0      885 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/shop/_api_client.py
+-rw-r--r--   0        0        0        0 2024-05-30 13:24:25.522284 cognite_power_ops-0.94.4/cognite/powerops/client/shop/api/__init__.py
+-rw-r--r--   0        0        0     8367 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/client/shop/api/dayahead_trigger_api.py
+-rw-r--r--   0        0        0     4797 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/client/shop/api/shop_result_files_api.py
+-rw-r--r--   0        0        0     4432 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/client/shop/api/shop_results_api.py
+-rw-r--r--   0        0        0     9593 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/client/shop/api/shop_run_api.py
+-rw-r--r--   0        0        0      600 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/client/shop/data_classes/__init__.py
+-rw-r--r--   0        0        0     4114 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/client/shop/data_classes/case.py
+-rw-r--r--   0        0        0     9057 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/client/shop/data_classes/dayahead_trigger.py
+-rw-r--r--   0        0        0     2720 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/client/shop/data_classes/helpers.py
+-rw-r--r--   0        0        0      603 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/client/shop/data_classes/plotting.py
+-rw-r--r--   0        0        0     6164 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/client/shop/data_classes/shop_result_files.py
+-rw-r--r--   0        0        0     6607 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/client/shop/data_classes/shop_results.py
+-rw-r--r--   0        0        0    10210 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/client/shop/data_classes/shop_results_compare.py
+-rw-r--r--   0        0        0     3021 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/client/shop/data_classes/shop_run.py
+-rw-r--r--   0        0        0     3743 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/client/shop/data_classes/shop_run_event.py
+-rw-r--r--   0        0        0     4374 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/client/shop/shop_case.py
+-rw-r--r--   0        0        0     1101 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/client/shop/shop_file_reference.py
+-rw-r--r--   0        0        0    13466 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/client/shop/shop_run.py
+-rw-r--r--   0        0        0    15419 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/client/shop/shop_run_api.py
+-rw-r--r--   0        0        0     3885 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/client/shop/shop_run_filter.py
+-rw-r--r--   0        0        0      563 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/client/shop/utils.py
+-rw-r--r--   0        0        0      947 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/cognite_modules/_system.yaml
+-rw-r--r--   0        0        0     1895 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/config.dev.yaml
+-rw-r--r--   0        0        0     1895 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/config.heco-dev.yaml
+-rw-r--r--   0        0        0     1895 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/config.lyse-dev.yaml
+-rw-r--r--   0        0        0     1899 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/config.staging.yaml
+-rw-r--r--   0        0        0      729 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/AFRRBid.datamodel.yaml
+-rw-r--r--   0        0        0     1095 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/Asset.datamodel.yaml
+-rw-r--r--   0        0        0     1680 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/DayAheadBid.datamodel.yaml
+-rw-r--r--   0        0        0      100 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/affr_space.space.yaml
+-rw-r--r--   0        0        0       92 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/asset.space.yaml
+-rw-r--r--   0        0        0      367 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/containers/AFRRBid-BidMethod.container.yaml
+-rw-r--r--   0        0        0     2102 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/containers/AFRRBid-BidRow.container.yaml
+-rw-r--r--   0        0        0      750 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/containers/asset-EfficiencyCurve.container.yaml
+-rw-r--r--   0        0        0     1380 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Alert.container.yaml
+-rw-r--r--   0        0        0      857 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Asset.container.yaml
+-rw-r--r--   0        0        0     1038 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-BidDocument.container.yaml
+-rw-r--r--   0        0        0      502 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-BidMethod.container.yaml
+-rw-r--r--   0        0        0     1408 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Generator.container.yaml
+-rw-r--r--   0        0        0     2281 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Plant.container.yaml
+-rw-r--r--   0        0        0     2375 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-PriceArea.container.yaml
+-rw-r--r--   0        0        0      556 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Watercourse.container.yaml
+-rw-r--r--   0        0        0      466 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-BidDocument.container.yaml
+-rw-r--r--   0        0        0      767 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-BidMatrix.container.yaml
+-rw-r--r--   0        0        0      371 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-BidMethod.container.yaml
+-rw-r--r--   0        0        0      532 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-MultiScenarioMatrix.container.yaml
+-rw-r--r--   0        0        0      618 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-SHOPMultiScenario.container.yaml
+-rw-r--r--   0        0        0      416 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-SHOPPriceScenario.container.yaml
+-rw-r--r--   0        0        0      490 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-SHOPPriceScenarioResults.container.yaml
+-rw-r--r--   0        0        0      113 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/dayahead_space.space.yaml
+-rw-r--r--   0        0        0      118 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/instance.space.yaml
+-rw-r--r--   0        0        0     1515 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/node_types/power-ops-types.powerops_nodes.yaml
+-rw-r--r--   0        0        0      116 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/shared.space.yaml
+-rw-r--r--   0        0        0       81 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/types.space.yaml
+-rw-r--r--   0        0        0     1379 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-BidDocument.view.yaml
+-rw-r--r--   0        0        0      606 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-BidMethod.view.yaml
+-rw-r--r--   0        0        0     3917 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-BidRow.view.yaml
+-rw-r--r--   0        0        0     2786 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-PriceArea.view.yaml
+-rw-r--r--   0        0        0     2618 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Generator.view.yaml
+-rw-r--r--   0        0        0     1138 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-GeneratorEfficiency.view.yaml
+-rw-r--r--   0        0        0     5199 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Plant.view.yaml
+-rw-r--r--   0        0        0     5204 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-PriceArea.view.yaml
+-rw-r--r--   0        0        0     1060 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Reservoir.view.yaml
+-rw-r--r--   0        0        0     1121 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-TurbineEfficiency.view.yaml
+-rw-r--r--   0        0        0     1887 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Watercourse.view.yaml
+-rw-r--r--   0        0        0     2558 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/baseBids-Alert.view.yaml
+-rw-r--r--   0        0        0     2374 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/baseBids-BidDocument.view.yaml
+-rw-r--r--   0        0        0      858 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/baseBids-BidMethod.view.yaml
+-rw-r--r--   0        0        0      579 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BasicBidMatrix.view.yaml
+-rw-r--r--   0        0        0     1945 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BidDocument.view.yaml
+-rw-r--r--   0        0        0     1845 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BidMatrix.view.yaml
+-rw-r--r--   0        0        0      723 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BidMethod.view.yaml
+-rw-r--r--   0        0        0      700 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-CustomBidMatrix.view.yaml
+-rw-r--r--   0        0        0      711 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-CustomBidMethod.view.yaml
+-rw-r--r--   0        0        0     1015 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-MultiScenarioMatrix.view.yaml
+-rw-r--r--   0        0        0     1479 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-PriceArea.view.yaml
+-rw-r--r--   0        0        0     1312 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-SHOPMultiScenarioMethod.view.yaml
+-rw-r--r--   0        0        0      666 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-SHOPPriceScenario.view.yaml
+-rw-r--r--   0        0        0     1230 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-SHOPPriceScenarioResult.view.yaml
+-rw-r--r--   0        0        0      605 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-WaterValueBasedMethod.view.yaml
+-rw-r--r--   0        0        0     4964 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/all_DayAhead.datamodel.yaml
+-rw-r--r--   0        0        0     6519 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/all_PowerOps.datamodel.yaml
+-rw-r--r--   0        0        0     2052 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/compute_DayAheadBenchmarking.datamodel.yaml
+-rw-r--r--   0        0        0     3499 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/compute_SHOPBasedDayAhead.datamodel.yaml
+-rw-r--r--   0        0        0     2918 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/compute_TotalBidMatrixCalculation.datamodel.yaml
+-rw-r--r--   0        0        0     2575 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/compute_WaterValueBasedDayAhead.datamodel.yaml
+-rw-r--r--   0        0        0     2276 2024-05-30 13:24:25.526284 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/config_DayAheadConfiguration.datamodel.yaml
+-rw-r--r--   0        0        0     2163 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/config_Resync.datamodel.yaml
+-rw-r--r--   0        0        0     1748 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/Alert.container.yaml
+-rw-r--r--   0        0        0      814 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidConfiguration.container.yaml
+-rw-r--r--   0        0        0     1292 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidDocument.container.yaml
+-rw-r--r--   0        0        0      496 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidDocumentDayAhead.container.yaml
+-rw-r--r--   0        0        0      771 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidMatrix.container.yaml
+-rw-r--r--   0        0        0     1659 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidRow.container.yaml
+-rw-r--r--   0        0        0      755 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/EfficiencyCurve.container.yaml
+-rw-r--r--   0        0        0     3539 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/FunctionData.container.yaml
+-rw-r--r--   0        0        0     1038 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/Generator.container.yaml
+-rw-r--r--   0        0        0     2082 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/MarketConfiguration.container.yaml
+-rw-r--r--   0        0        0      756 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PartialBidConfiguration.container.yaml
+-rw-r--r--   0        0        0     2425 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PlantWaterValueBased.container.yaml
+-rw-r--r--   0        0        0     1076 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PowerAsset.container.yaml
+-rw-r--r--   0        0        0     1628 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PriceAreaAFRR.container.yaml
+-rw-r--r--   0        0        0      689 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PriceAreaDayAhead.container.yaml
+-rw-r--r--   0        0        0      710 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PriceProduction.container.yaml
+-rw-r--r--   0        0        0      504 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/SHOPObjectiveValue.container.yaml
+-rw-r--r--   0        0        0     1074 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/SHOPResult.container.yaml
+-rw-r--r--   0        0        0     1106 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/SHOPTimeSeries.container.yaml
+-rw-r--r--   0        0        0     1462 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopAttributeMapping.container.yaml
+-rw-r--r--   0        0        0      634 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopCase.container.yaml
+-rw-r--r--   0        0        0      464 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopCommands.container.yaml
+-rw-r--r--   0        0        0     1128 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopFile.container.yaml
+-rw-r--r--   0        0        0     1446 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopModel.container.yaml
+-rw-r--r--   0        0        0      280 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopPartialBidConfiguration.container.yaml
+-rw-r--r--   0        0        0      978 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopScenario.container.yaml
+-rw-r--r--   0        0        0      690 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopScenarioSet.container.yaml
+-rw-r--r--   0        0        0      869 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/frontend_AFRRBid.datamodel.yaml
+-rw-r--r--   0        0        0     1789 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/frontend_Asset.datamodel.yaml
+-rw-r--r--   0        0        0     2661 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/frontend_DayAheadBid.datamodel.yaml
+-rw-r--r--   0        0        0      118 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/instance.space.yaml
+-rw-r--r--   0        0        0      104 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/models.space.yaml
+-rw-r--r--   0        0        0     5275 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/node_types/power-ops-types.powerops_nodes.yaml
+-rw-r--r--   0        0        0      854 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/product_CogShop.datamodel.yaml
+-rw-r--r--   0        0        0       91 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/type.space.yaml
+-rw-r--r--   0        0        0     3704 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/BidRow.view.yaml
+-rw-r--r--   0        0        0     2834 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/MarketConfiguration.view.yaml
+-rw-r--r--   0        0        0     2983 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/alerts/1-interface.Alert.view.yaml
+-rw-r--r--   0        0        0      871 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/alerts/ShopPenaltyReport.view.yaml
+-rw-r--r--   0        0        0     1283 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/1-interface.PowerAsset.view.yaml
+-rw-r--r--   0        0        0     2330 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/generator/Generator.view.yaml
+-rw-r--r--   0        0        0     1073 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/generator/GeneratorEfficiencyCurve.view.yaml
+-rw-r--r--   0        0        0     1260 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/generator/TurbineEfficiencyCurve.view.yaml
+-rw-r--r--   0        0        0      535 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/plant/1-interface.Plant.view.yaml
+-rw-r--r--   0        0        0      599 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/plant/PlantInformation.view.yaml
+-rw-r--r--   0        0        0     4498 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/plant/PlantWaterValueBased.view.yaml
+-rw-r--r--   0        0        0      512 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/1-interface.PriceArea.view.yaml
+-rw-r--r--   0        0        0     2932 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/PriceAreaAFRR.view.yaml
+-rw-r--r--   0        0        0     1659 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/PriceAreaDayAhead.view.yaml
+-rw-r--r--   0        0        0      596 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/PriceAreaInformation.view.yaml
+-rw-r--r--   0        0        0      543 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/watercourse/1-interface.Watercourse.view.yaml
+-rw-r--r--   0        0        0     1476 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/1-interface.PartialBidConfiguration.view.yaml
+-rw-r--r--   0        0        0     2264 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/BidConfigurationDayAhead.view.yaml
+-rw-r--r--   0        0        0     1059 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/ShopBasedPartialBidConfiguration.view.yaml
+-rw-r--r--   0        0        0     1184 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/WaterValueBasedPartialBidConfiguration.view.yaml
+-rw-r--r--   0        0        0     2520 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/1-interface.BidDocument.view.yaml
+-rw-r--r--   0        0        0     1450 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/BidDocumentAFRR.view.yaml
+-rw-r--r--   0        0        0     1726 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/BidDocumentDayAhead.view.yaml
+-rw-r--r--   0        0        0     1564 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/BidDocumentDayAheadSimple.view.yaml
+-rw-r--r--   0        0        0      701 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/1-interface.BidMatrix.view.yaml
+-rw-r--r--   0        0        0     1225 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/1-interface.BidMatrixInformation.view.yaml
+-rw-r--r--   0        0        0     1349 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/1-interface.PartialBidMatrixInformation.view.yaml
+-rw-r--r--   0        0        0      890 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/PartialBidMatrixInformationWithScenarios.view.yaml
+-rw-r--r--   0        0        0     2331 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopAttributeMapping.view.yaml
+-rw-r--r--   0        0        0     1840 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopCase.view.yaml
+-rw-r--r--   0        0        0     1027 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopCommands.view.yaml
+-rw-r--r--   0        0        0     1705 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopFile.view.yaml
+-rw-r--r--   0        0        0     2573 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopModel.view.yaml
+-rw-r--r--   0        0        0     1965 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopScenario.view.yaml
+-rw-r--r--   0        0        0     1535 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopScenarioSet.view.yaml
+-rw-r--r--   0        0        0     1399 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/1-interface.FunctionInput.view.yaml
+-rw-r--r--   0        0        0     1797 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/1-interface.PartialBidMatrixCalculationInput.view.yaml
+-rw-r--r--   0        0        0     1053 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/BenchmarkingCollectorInput.view.yaml
+-rw-r--r--   0        0        0     1750 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/ShopPartialBidMatrixCalculationInput.view.yaml
+-rw-r--r--   0        0        0     1522 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/ShopPreprocessorInput.view.yaml
+-rw-r--r--   0        0        0     1660 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/ShopTriggerInput.view.yaml
+-rw-r--r--   0        0        0     1069 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/TaskDispatcherBenchmarkingInput.view.yaml
+-rw-r--r--   0        0        0     1249 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/TaskDispatcherInput.view.yaml
+-rw-r--r--   0        0        0     1680 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/TotalBidMatrixCalculationInput.view.yaml
+-rw-r--r--   0        0        0     1336 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/WaterPartialBidMatrixCalculationInput.view.yaml
+-rw-r--r--   0        0        0     2119 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/1-interface.FunctionOutput.view.yaml
+-rw-r--r--   0        0        0      981 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/BenchmarkingCollectorOutput.view.yaml
+-rw-r--r--   0        0        0     1757 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/PartialBidMatrixCalculationOutput.view.yaml
+-rw-r--r--   0        0        0     1355 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/SHOPTriggerOutput.view.yaml
+-rw-r--r--   0        0        0     1426 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/ShopPreprocessorOutput.view.yaml
+-rw-r--r--   0        0        0     1010 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/TaskDispatcherBenchmarkingOutput.view.yaml
+-rw-r--r--   0        0        0     1378 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/TaskDispatcherOutput.view.yaml
+-rw-r--r--   0        0        0     1434 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/TotalBidMatrixCalculationOutput.view.yaml
+-rw-r--r--   0        0        0     1392 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/PriceProduction.view.yaml
+-rw-r--r--   0        0        0     2707 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/SHOPResult.view.yaml
+-rw-r--r--   0        0        0     1587 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/SHOPTimeSeries.view.yaml
+-rw-r--r--   0        0        0     1114 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/ShopObjectiveValue.view.yaml
+-rw-r--r--   0        0        0        0 2024-05-30 13:24:25.530285 cognite_power_ops-0.94.4/cognite/powerops/prerun_transformations/__init__.py
+-rw-r--r--   0        0        0    34098 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/prerun_transformations/transformations.py
+-rw-r--r--   0        0        0      394 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/__init__.py
+-rw-r--r--   0        0        0     1792 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/config/__init__.py
+-rw-r--r--   0        0        0    12764 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/config/_main.py
+-rw-r--r--   0        0        0      595 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/config/_settings.py
+-rw-r--r--   0        0        0    12408 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/config/_shared.py
+-rw-r--r--   0        0        0       75 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/config/cogshop/__init__.py
+-rw-r--r--   0        0        0      720 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/config/cogshop/shop_file_config.py
+-rw-r--r--   0        0        0      815 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/config/market/__init__.py
+-rw-r--r--   0        0        0     5486 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/config/market/_core.py
+-rw-r--r--   0        0        0     2106 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/config/market/benchmarking.py
+-rw-r--r--   0        0        0     2105 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/config/market/dayahead.py
+-rw-r--r--   0        0        0      961 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/config/market/market.py
+-rw-r--r--   0        0        0    10827 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/config/market/rkom.py
+-rw-r--r--   0        0        0      417 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/config/production/__init__.py
+-rw-r--r--   0        0        0      830 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/config/production/connections.py
+-rw-r--r--   0        0        0     1414 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/config/production/generator.py
+-rw-r--r--   0        0        0     5675 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/config/production/plant.py
+-rw-r--r--   0        0        0     2868 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/config/production/watercourse.py
+-rw-r--r--   0        0        0      244 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/core/__init__.py
+-rw-r--r--   0        0        0     9185 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/core/cdf.py
+-rw-r--r--   0        0        0      442 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/core/echo.py
+-rw-r--r--   0        0        0    27692 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/core/main.py
+-rw-r--r--   0        0        0     2563 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/core/transform.py
+-rw-r--r--   0        0        0     2161 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/core/validation.py
+-rw-r--r--   0        0        0      474 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/diff/__init__.py
+-rw-r--r--   0        0        0     6774 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/diff/core.py
+-rw-r--r--   0        0        0    12631 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/diff/data_classes.py
+-rw-r--r--   0        0        0      424 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/models/__init__.py
+-rw-r--r--   0        0        0       82 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/models/_shared_v1_v2/__init__.py
+-rw-r--r--   0        0        0      811 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/models/_shared_v1_v2/_to_instances.py
+-rw-r--r--   0        0        0    10495 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/models/_shared_v1_v2/cogshop_model.py
+-rw-r--r--   0        0        0     1143 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/models/_shared_v1_v2/market_model.py
+-rw-r--r--   0        0        0     8337 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/models/_shared_v1_v2/production_model.py
+-rw-r--r--   0        0        0      788 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/models/base/__init__.py
+-rw-r--r--   0        0        0    11195 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/models/base/asset_model.py
+-rw-r--r--   0        0        0     9602 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/models/base/asset_type.py
+-rw-r--r--   0        0        0     5251 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/models/base/cdf_resources.py
+-rw-r--r--   0        0        0    11641 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/models/base/data_model.py
+-rw-r--r--   0        0        0     1896 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/models/base/dms_models.py
+-rw-r--r--   0        0        0      592 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/models/base/graph_ql.py
+-rw-r--r--   0        0        0      148 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/models/base/helpers.py
+-rw-r--r--   0        0        0     6668 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/models/base/model.py
+-rw-r--r--   0        0        0     1705 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/models/base/resource_type.py
+-rw-r--r--   0        0        0     1302 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/models/v1/__init__.py
+-rw-r--r--   0        0        0     8141 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/models/v1/cogshop.py
+-rw-r--r--   0        0        0      243 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/models/v1/config_to_model/__init__.py
+-rw-r--r--   0        0        0     8940 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/models/v1/config_to_model/to_cogshop_model.py
+-rw-r--r--   0        0        0    15631 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/models/v1/config_to_model/to_market_model.py
+-rw-r--r--   0        0        0     9726 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/models/v1/config_to_model/to_production_model.py
+-rw-r--r--   0        0        0      491 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/models/v1/graphql_schemas/__init__.py
+-rw-r--r--   0        0        0      832 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/models/v1/graphql_schemas/cogshop1.graphql
+-rw-r--r--   0        0        0     3499 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/models/v1/market/__init__.py
+-rw-r--r--   0        0        0     1291 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/models/v1/market/base.py
+-rw-r--r--   0        0        0     3184 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/models/v1/market/benchmark.py
+-rw-r--r--   0        0        0     2405 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/models/v1/market/dayahead.py
+-rw-r--r--   0        0        0     2797 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/models/v1/market/rkom.py
+-rw-r--r--   0        0        0     7801 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/models/v1/production.py
+-rw-r--r--   0        0        0      395 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/models/v2/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/models/v2/config_to_model/__init__.py
+-rw-r--r--   0        0        0     8873 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/models/v2/config_to_model/to_powerasset_model.py
+-rw-r--r--   0        0        0    27181 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/models/v2/powerops_models.py
+-rw-r--r--   0        0        0     7631 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/models/v2/production_dm.py
+-rw-r--r--   0        0        0      150 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/time_series_mapping/__init__.py
+-rw-r--r--   0        0        0     2149 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/time_series_mapping/mapping.py
+-rw-r--r--   0        0        0     2456 2024-05-30 13:24:25.534284 cognite_power_ops-0.94.4/cognite/powerops/resync/time_series_mapping/static_mapping.py
+-rw-r--r--   0        0        0     6585 2024-05-30 13:24:25.538284 cognite_power_ops-0.94.4/cognite/powerops/resync/v1/README.md
+-rw-r--r--   0        0        0       59 2024-05-30 13:24:25.538284 cognite_power_ops-0.94.4/cognite/powerops/resync/v1/__init__.py
+-rw-r--r--   0        0        0    30081 2024-05-30 13:24:25.538284 cognite_power_ops-0.94.4/cognite/powerops/resync/v1/config_to_fdm.py
+-rw-r--r--   0        0        0    14948 2024-05-30 13:24:25.538284 cognite_power_ops-0.94.4/cognite/powerops/resync/v1/data_classes.py
+-rw-r--r--   0        0        0     2909 2024-05-30 13:24:25.538284 cognite_power_ops-0.94.4/cognite/powerops/resync/v1/main.py
+-rw-r--r--   0        0        0    12112 2024-05-30 13:24:25.538284 cognite_power_ops-0.94.4/cognite/powerops/resync/v1/utils.py
+-rw-r--r--   0        0        0     4524 2024-05-30 13:24:25.538284 cognite_power_ops-0.94.4/cognite/powerops/resync/validation.py
+-rw-r--r--   0        0        0        0 2024-05-30 13:24:25.538284 cognite_power_ops-0.94.4/cognite/powerops/utils/__init__.py
+-rw-r--r--   0        0        0      160 2024-05-30 13:24:25.538284 cognite_power_ops-0.94.4/cognite/powerops/utils/cdf/__init__.py
+-rw-r--r--   0        0        0     1389 2024-05-30 13:24:25.538284 cognite_power_ops-0.94.4/cognite/powerops/utils/cdf/_cdf_auth.py
+-rw-r--r--   0        0        0     3169 2024-05-30 13:24:25.538284 cognite_power_ops-0.94.4/cognite/powerops/utils/cdf/_settings.py
+-rw-r--r--   0        0        0     7517 2024-05-30 13:24:25.538284 cognite_power_ops-0.94.4/cognite/powerops/utils/cdf/calls.py
+-rw-r--r--   0        0        0    10874 2024-05-30 13:24:25.538284 cognite_power_ops-0.94.4/cognite/powerops/utils/cdf/extraction_pipelines.py
+-rw-r--r--   0        0        0      970 2024-05-30 13:24:25.538284 cognite_power_ops-0.94.4/cognite/powerops/utils/cdf/resource_creation.py
+-rw-r--r--   0        0        0     2540 2024-05-30 13:24:25.538284 cognite_power_ops-0.94.4/cognite/powerops/utils/lookup.py
+-rw-r--r--   0        0        0     1097 2024-05-30 13:24:25.538284 cognite_power_ops-0.94.4/cognite/powerops/utils/navigation.py
+-rw-r--r--   0        0        0      514 2024-05-30 13:24:25.538284 cognite_power_ops-0.94.4/cognite/powerops/utils/require.py
+-rw-r--r--   0        0        0      227 2024-05-30 13:24:25.538284 cognite_power_ops-0.94.4/cognite/powerops/utils/retry/__init__.py
+-rw-r--r--   0        0        0     5619 2024-05-30 13:24:25.538284 cognite_power_ops-0.94.4/cognite/powerops/utils/retry/api.py
+-rw-r--r--   0        0        0     8228 2024-05-30 13:24:25.538284 cognite_power_ops-0.94.4/cognite/powerops/utils/serialization.py
+-rw-r--r--   0        0        0     3667 2024-05-30 13:24:25.538284 cognite_power_ops-0.94.4/cognite/powerops/utils/time.py
+-rw-r--r--   0        0        0     3732 2024-05-30 13:24:25.542284 cognite_power_ops-0.94.4/pyproject.toml
+-rw-r--r--   0        0        0     5525 1970-01-01 00:00:00.000000 cognite_power_ops-0.94.4/PKG-INFO
```

### Comparing `cognite_power_ops-0.94.3/LICENSE` & `cognite_power_ops-0.94.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/README.md` & `cognite_power_ops-0.94.4/README.md`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/cdf_labels.py` & `cognite_power_ops-0.94.4/cognite/powerops/cdf_labels.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/cli.py` & `cognite_power_ops-0.94.4/cognite/powerops/cli.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/_core.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/alert.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/alert.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/alert_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/alert_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/bid_document.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/bid_document.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/bid_document_alerts.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/bid_document_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/bid_document_bids.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/bid_document_bids.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/bid_document_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/bid_document_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/bid_method.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/bid_method.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/bid_method_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/bid_method_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/bid_row.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/bid_row.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/bid_row_alerts.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/bid_row_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/bid_row_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/bid_row_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/price_area.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/price_area.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/price_area_activation_price_down.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/price_area_activation_price_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/price_area_activation_price_up.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/price_area_activation_price_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/price_area_capacity_price_down.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/price_area_capacity_price_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/price_area_capacity_price_up.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/price_area_capacity_price_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/price_area_own_capacity_allocation_down.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/price_area_own_capacity_allocation_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/price_area_own_capacity_allocation_up.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/price_area_own_capacity_allocation_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/price_area_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/price_area_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/price_area_relative_activation.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/price_area_relative_activation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/price_area_total_capacity_allocation_down.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/price_area_total_capacity_allocation_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api/price_area_total_capacity_allocation_up.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api/price_area_total_capacity_allocation_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/_api_client.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/_api_client.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/data_classes/__init__.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/data_classes/_alert.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/data_classes/_alert.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/data_classes/_bid_document.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/data_classes/_bid_document.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/data_classes/_bid_method.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/data_classes/_bid_method.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/data_classes/_bid_row.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/data_classes/_bid_row.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/data_classes/_core.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/data_classes/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/afrr_bid/data_classes/_price_area.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/afrr_bid/data_classes/_price_area.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/_core.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/bid_method.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/bid_method.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/bid_method_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/bid_method_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/generator.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/generator.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/generator_efficiency_curve.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/generator_efficiency_curve.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/generator_efficiency_curve_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/generator_efficiency_curve_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/generator_is_available_time_series.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/generator_is_available_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/generator_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/generator_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/generator_start_stop_cost.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/generator_start_stop_cost.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/generator_turbine_curves.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/generator_turbine_curves.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/plant.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/plant.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/plant_feeding_fee_time_series.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/plant_feeding_fee_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/plant_generators.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/plant_generators.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/plant_head_direct_time_series.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/plant_head_direct_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/plant_inlet_level_time_series.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/plant_inlet_level_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/plant_outlet_level_time_series.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/plant_outlet_level_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/plant_p_max_time_series.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/plant_p_max_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/plant_p_min_time_series.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/plant_p_min_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/plant_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/plant_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/plant_water_value_time_series.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/plant_water_value_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/price_area.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/price_area.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/price_area_activation_price_down.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/price_area_activation_price_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/price_area_activation_price_up.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/price_area_activation_price_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/price_area_capacity_price_down.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/price_area_capacity_price_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/price_area_capacity_price_up.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/price_area_capacity_price_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/price_area_day_ahead_price.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/price_area_day_ahead_price.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/price_area_main_scenario_day_ahead.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/price_area_main_scenario_day_ahead.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/price_area_own_capacity_allocation_down.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/price_area_own_capacity_allocation_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/price_area_own_capacity_allocation_up.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/price_area_own_capacity_allocation_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/price_area_plants.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/price_area_plants.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/price_area_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/price_area_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/price_area_relative_activation.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/price_area_relative_activation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/price_area_total_capacity_allocation_down.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/price_area_total_capacity_allocation_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/price_area_total_capacity_allocation_up.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/price_area_total_capacity_allocation_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/price_area_watercourses.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/price_area_watercourses.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/reservoir.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/reservoir.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/reservoir_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/reservoir_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/turbine_efficiency_curve.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/turbine_efficiency_curve.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/turbine_efficiency_curve_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/turbine_efficiency_curve_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/watercourse.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/watercourse.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/watercourse_plants.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/watercourse_plants.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/watercourse_production_obligation.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/watercourse_production_obligation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api/watercourse_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api/watercourse_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/_api_client.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/_api_client.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/data_classes/__init__.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/data_classes/_bid_method.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/data_classes/_bid_method.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/data_classes/_core.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/data_classes/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/data_classes/_generator.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/data_classes/_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/data_classes/_generator_efficiency_curve.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/data_classes/_generator_efficiency_curve.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/data_classes/_plant.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/data_classes/_plant.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/data_classes/_price_area.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/data_classes/_price_area.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/data_classes/_reservoir.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/data_classes/_reservoir.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/data_classes/_turbine_efficiency_curve.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/data_classes/_turbine_efficiency_curve.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/assets/data_classes/_watercourse.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/assets/data_classes/_watercourse.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/_api/_core.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/_api/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/_api/case.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/_api/case.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/_api/commands_config.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/_api/commands_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/_api/file_ref.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/_api/file_ref.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/_api/mapping.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/_api/mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/_api/model_template.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/_api/model_template.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/_api/processing_log.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/_api/processing_log.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/_api/scenario.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/_api/scenario.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/_api/transformation.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/_api/transformation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/_api_client.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/_api_client.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/data_classes/__init__.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/data_classes/_case.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/data_classes/_case.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/data_classes/_commands_config.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/data_classes/_commands_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/data_classes/_core.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/data_classes/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/data_classes/_file_ref.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/data_classes/_file_ref.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/data_classes/_mapping.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/data_classes/_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/data_classes/_model_template.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/data_classes/_model_template.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/data_classes/_processing_log.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/data_classes/_processing_log.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/data_classes/_scenario.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/data_classes/_scenario.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/cogshop1/data_classes/_transformation.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/cogshop1/data_classes/_transformation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/_core.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/alert.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/alert.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/alert_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/alert_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/basic_bid_matrix.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/basic_bid_matrix.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/basic_bid_matrix_alerts.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/basic_bid_matrix_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/basic_bid_matrix_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/basic_bid_matrix_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document_alerts.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document_partials.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document_partials.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_matrix.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_matrix.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_matrix_alerts.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_matrix_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_matrix_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_matrix_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_method.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_method.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_method_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_method_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix_alerts.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix_scenario_results.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix_scenario_results.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area_main_scenario.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area_main_scenario.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area_price_scenarios.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area_price_scenarios.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_multi_scenario_method.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_multi_scenario_method.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_multi_scenario_method_price_scenarios.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_multi_scenario_method_price_scenarios.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_multi_scenario_method_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_multi_scenario_method_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_price.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_price.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result_price.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result_price.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result_production.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result_production.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/water_value_based_method.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/water_value_based_method.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api/water_value_based_method_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api/water_value_based_method_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/_api_client.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/_api_client.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/data_classes/__init__.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_alert.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_alert.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_basic_bid_matrix.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_basic_bid_matrix.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_bid_document.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_bid_document.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_bid_matrix.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_bid_matrix.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_bid_method.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_bid_method.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_core.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_multi_scenario_matrix.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_multi_scenario_matrix.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_price_area.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_price_area.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_shop_multi_scenario_method.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_shop_multi_scenario_method.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_shop_price_scenario.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_shop_price_scenario.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_shop_price_scenario_result.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_shop_price_scenario_result.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_water_value_based_method.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_water_value_based_method.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/_core.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/alert.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/alert.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/alert_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/alert_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_configuration_day_ahead.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_configuration_day_ahead.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_configuration_day_ahead_partials.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_configuration_day_ahead_partials.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_configuration_day_ahead_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_configuration_day_ahead_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_document.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_document.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_document_afrr.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_document_afrr.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_document_afrr_alerts.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_document_afrr_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_document_afrr_bids.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_document_afrr_bids.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_document_afrr_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_document_afrr_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_document_alerts.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_document_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead_alerts.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead_partials.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead_partials.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_document_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_document_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_matrix.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_matrix.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_matrix_information.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_matrix_information.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_matrix_information_alerts.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_matrix_information_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_matrix_information_intermediate_bid_matrices.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_matrix_information_intermediate_bid_matrices.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_matrix_information_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_matrix_information_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_matrix_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_matrix_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_row.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_row.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_row_alerts.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_row_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/bid_row_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/bid_row_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/function_input.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/function_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/function_input_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/function_input_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/function_output.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/function_output.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/function_output_alerts.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/function_output_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/function_output_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/function_output_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/generator.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/generator.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/generator_availability_time_series.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/generator_availability_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/generator_efficiency_curve.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/generator_efficiency_curve.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/generator_efficiency_curve_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/generator_efficiency_curve_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/generator_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/generator_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/generator_start_stop_cost.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/generator_start_stop_cost.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/generator_turbine_efficiency_curves.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/generator_turbine_efficiency_curves.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/market_configuration.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/market_configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/market_configuration_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/market_configuration_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/partial_bid_configuration.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/partial_bid_configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/partial_bid_configuration_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/partial_bid_configuration_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_input.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_input_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_input_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_output.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_output.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_output_alerts.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_output_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_output_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_output_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_alerts.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_intermediate_bid_matrices.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_intermediate_bid_matrices.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_alerts.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_intermediate_bid_matrices.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_intermediate_bid_matrices.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_multi_scenario_input.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_multi_scenario_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_information.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_information.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_information_feeding_fee_time_series.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_information_feeding_fee_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_information_generators.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_information_generators.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_information_head_direct_time_series.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_information_head_direct_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_information_inlet_level_time_series.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_information_inlet_level_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_information_outlet_level_time_series.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_information_outlet_level_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_information_production_max_time_series.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_information_production_max_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_information_production_min_time_series.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_information_production_min_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_information_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_information_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_information_water_value_time_series.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_information_water_value_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_water_value_based.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_water_value_based.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_feeding_fee_time_series.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_feeding_fee_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_generators.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_generators.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_head_direct_time_series.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_head_direct_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_inlet_level_time_series.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_inlet_level_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_outlet_level_time_series.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_outlet_level_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_production_max_time_series.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_production_max_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_production_min_time_series.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_production_min_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_water_value_time_series.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_water_value_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/power_asset.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/power_asset.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/power_asset_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/power_asset_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_afrr.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_afrr.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_afrr_activation_price_down.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_afrr_activation_price_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_afrr_activation_price_up.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_afrr_activation_price_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_afrr_capacity_price_down.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_afrr_capacity_price_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_afrr_capacity_price_up.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_afrr_capacity_price_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_afrr_own_capacity_allocation_down.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_afrr_own_capacity_allocation_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_afrr_own_capacity_allocation_up.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_afrr_own_capacity_allocation_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_afrr_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_afrr_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_afrr_relative_activation.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_afrr_relative_activation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_afrr_total_capacity_allocation_down.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_afrr_total_capacity_allocation_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_afrr_total_capacity_allocation_up.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_afrr_total_capacity_allocation_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead_main_price_scenario.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead_main_price_scenario.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead_price_scenarios.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead_price_scenarios.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_information.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_information.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_information_activation_price_down.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_information_activation_price_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_information_activation_price_up.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_information_activation_price_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_information_capacity_price_down.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_information_capacity_price_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_information_capacity_price_up.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_information_capacity_price_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_information_main_price_scenario.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_information_main_price_scenario.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_information_own_capacity_allocation_down.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_information_own_capacity_allocation_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_information_own_capacity_allocation_up.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_information_own_capacity_allocation_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_information_price_scenarios.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_information_price_scenarios.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_information_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_information_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_information_relative_activation.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_information_relative_activation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_information_total_capacity_allocation_down.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_information_total_capacity_allocation_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_information_total_capacity_allocation_up.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_information_total_capacity_allocation_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_area_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_area_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_production.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_production.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_production_price.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_production_price.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_production_production.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_production_production.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/price_production_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/price_production_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_attribute_mapping.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_attribute_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_attribute_mapping_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_attribute_mapping_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_attribute_mapping_time_series.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_attribute_mapping_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_based_partial_bid_configuration.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_based_partial_bid_configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_based_partial_bid_configuration_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_based_partial_bid_configuration_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_case.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_case.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_case_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_case_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_case_shop_files.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_case_shop_files.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_commands.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_commands.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_commands_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_commands_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_file.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_file.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_file_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_file_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_model.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_model.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_model_base_attribute_mappings.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_model_base_attribute_mappings.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_model_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_model_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_partial_bid_matrix_calculation_input.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_partial_bid_matrix_calculation_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_partial_bid_matrix_calculation_input_price_production.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_partial_bid_matrix_calculation_input_price_production.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_partial_bid_matrix_calculation_input_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_partial_bid_matrix_calculation_input_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_penalty_report.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_penalty_report.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_penalty_report_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_penalty_report_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_input.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_input_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_input_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_output.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_output.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_output_alerts.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_output_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_output_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_output_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_result.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_result.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_result_alerts.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_result_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_result_output_time_series.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_result_output_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_result_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_result_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_scenario.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_scenario.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_scenario_attribute_mappings_override.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_scenario_attribute_mappings_override.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_scenario_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_scenario_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_scenario_set.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_scenario_set.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_scenario_set_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_scenario_set_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_scenario_set_scenarios.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_scenario_set_scenarios.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_time_series.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_time_series_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_time_series_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_time_series_time_series.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_time_series_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_trigger_input.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_trigger_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_trigger_input_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_trigger_input_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_trigger_output.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_trigger_output.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_trigger_output_alerts.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_trigger_output_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/shop_trigger_output_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/shop_trigger_output_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/task_dispatcher_input.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/task_dispatcher_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/task_dispatcher_input_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/task_dispatcher_input_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output_alerts.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output_process_sub_tasks.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output_process_sub_tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_input.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_input_partial_bid_matrices.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_input_partial_bid_matrices.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_input_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_input_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_output.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_output.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_output_alerts.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_output_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_output_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_output_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/turbine_efficiency_curve.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/turbine_efficiency_curve.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/turbine_efficiency_curve_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/turbine_efficiency_curve_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_configuration.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_configuration_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_configuration_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_matrix_calculation_input.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_matrix_calculation_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_matrix_calculation_input_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_matrix_calculation_input_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/watercourse.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/watercourse.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api/watercourse_query.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api/watercourse_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/_api_client.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/_api_client.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/__init__.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_alert.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_alert.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_bid_configuration_day_ahead.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_bid_configuration_day_ahead.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_bid_document.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_bid_document.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_bid_document_afrr.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_bid_document_afrr.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_bid_document_day_ahead.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_bid_document_day_ahead.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_bid_matrix.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_bid_matrix.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_bid_matrix_information.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_bid_matrix_information.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_bid_row.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_bid_row.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_core.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_function_input.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_function_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_function_output.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_function_output.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_generator.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_generator_efficiency_curve.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_generator_efficiency_curve.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_market_configuration.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_market_configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_configuration.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_calculation_input.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_calculation_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_calculation_output.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_calculation_output.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_information.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_information.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_information_with_scenarios.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_information_with_scenarios.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_plant.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_plant.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_plant_information.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_plant_information.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_plant_water_value_based.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_plant_water_value_based.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_power_asset.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_power_asset.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_price_area.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_price_area.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_price_area_afrr.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_price_area_afrr.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_price_area_day_ahead.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_price_area_day_ahead.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_price_area_information.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_price_area_information.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_price_production.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_price_production.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_shop_attribute_mapping.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_shop_attribute_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_shop_based_partial_bid_configuration.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_shop_based_partial_bid_configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_shop_case.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_shop_case.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_shop_commands.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_shop_commands.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_shop_file.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_shop_file.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_shop_model.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_shop_model.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_shop_partial_bid_matrix_calculation_input.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_shop_partial_bid_matrix_calculation_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_shop_penalty_report.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_shop_penalty_report.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_shop_preprocessor_input.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_shop_preprocessor_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_shop_preprocessor_output.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_shop_preprocessor_output.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_shop_result.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_shop_result.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_shop_scenario.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_shop_scenario.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_shop_scenario_set.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_shop_scenario_set.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_shop_time_series.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_shop_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_shop_trigger_input.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_shop_trigger_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_shop_trigger_output.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_shop_trigger_output.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_task_dispatcher_input.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_task_dispatcher_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_task_dispatcher_output.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_task_dispatcher_output.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_total_bid_matrix_calculation_input.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_total_bid_matrix_calculation_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_total_bid_matrix_calculation_output.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_total_bid_matrix_calculation_output.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_turbine_efficiency_curve.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_turbine_efficiency_curve.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_water_value_based_partial_bid_configuration.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_water_value_based_partial_bid_configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_water_value_based_partial_bid_matrix_calculation_input.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_water_value_based_partial_bid_matrix_calculation_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_generated/v1/data_classes/_watercourse.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_generated/v1/data_classes/_watercourse.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/_logger.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/_logger.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/data_set_api.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/data_set_api.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/powerops_client.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/powerops_client.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/shop/_api_client.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/shop/_api_client.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/shop/api/dayahead_trigger_api.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/shop/api/dayahead_trigger_api.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/shop/api/shop_result_files_api.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/shop/api/shop_result_files_api.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/shop/api/shop_results_api.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/shop/api/shop_results_api.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/shop/api/shop_run_api.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/shop/api/shop_run_api.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/shop/data_classes/__init__.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/shop/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/shop/data_classes/case.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/shop/data_classes/case.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/shop/data_classes/dayahead_trigger.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/shop/data_classes/dayahead_trigger.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/shop/data_classes/helpers.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/shop/data_classes/helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/shop/data_classes/plotting.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/shop/data_classes/plotting.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/shop/data_classes/shop_result_files.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/shop/data_classes/shop_result_files.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/shop/data_classes/shop_results.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/shop/data_classes/shop_results.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/shop/data_classes/shop_results_compare.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/shop/data_classes/shop_results_compare.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/shop/data_classes/shop_run.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/shop/data_classes/shop_run.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/shop/data_classes/shop_run_event.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/shop/data_classes/shop_run_event.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/shop/shop_case.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/shop/shop_case.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/shop/shop_file_reference.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/shop/shop_file_reference.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/shop/shop_run.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/shop/shop_run.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/shop/shop_run_api.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/shop/shop_run_api.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/shop/shop_run_filter.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/shop/shop_run_filter.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/client/shop/utils.py` & `cognite_power_ops-0.94.4/cognite/powerops/client/shop/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/cognite_modules/_system.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/cognite_modules/_system.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -21,8 +21,8 @@
     - cdf_infield_location
   example_pump:
     - example_pump_asset_hierarchy
     - cdf_asset_source_model
     - example_pump_data_model
 
 # This part is used by cdf-toolkit to keep track of the version and help you upgrade.
-cdf_toolkit_version: 0.1.1
+cdf_toolkit_version: 0.1.4
```

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/config.dev.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/config.heco-dev.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 environment:
-  name: dev
-  project: power-ops-staging
+  name: heco-dev
+  project: heco-dev
   type: dev
   selected_modules_and_packages:
     - power_model_v1
 
 modules:
   custom_modules:
     power_model_v1:
-      # TODO: update space to not be temp
       power_ops_type_space: "sp_power_ops_types"
       power_ops_instance_space: "sp_power_ops_instance"
       power_ops_models: "sp_power_ops_models"
       version: "1"
     power_model_v0:
       # variables used for substitution in other files in this directory
       afrr_model_space: "power-ops-afrr-bid"
```

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/AFRRBid.datamodel.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/AFRRBid.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/Asset.datamodel.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/Asset.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/DayAheadBid.datamodel.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/DayAheadBid.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/containers/AFRRBid-BidRow.container.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/containers/AFRRBid-BidRow.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/containers/asset-EfficiencyCurve.container.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/containers/asset-EfficiencyCurve.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Alert.container.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Alert.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Asset.container.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Asset.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-BidDocument.container.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-BidDocument.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Generator.container.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Generator.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Plant.container.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Plant.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-PriceArea.container.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-PriceArea.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Watercourse.container.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Watercourse.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-BidMatrix.container.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-BidMatrix.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-MultiScenarioMatrix.container.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-MultiScenarioMatrix.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-SHOPMultiScenario.container.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-SHOPMultiScenario.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/node_types/power-ops-types.powerops_nodes.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/node_types/power-ops-types.powerops_nodes.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-BidDocument.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-BidDocument.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-BidMethod.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-BidMethod.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-BidRow.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-BidRow.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-PriceArea.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-PriceArea.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Generator.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Generator.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-GeneratorEfficiency.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-GeneratorEfficiency.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Plant.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Plant.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-PriceArea.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-PriceArea.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Reservoir.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Reservoir.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-TurbineEfficiency.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-TurbineEfficiency.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Watercourse.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Watercourse.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/baseBids-Alert.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/baseBids-Alert.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/baseBids-BidDocument.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/baseBids-BidDocument.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/baseBids-BidMethod.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/baseBids-BidMethod.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BasicBidMatrix.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BasicBidMatrix.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BidDocument.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BidDocument.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BidMatrix.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BidMatrix.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BidMethod.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BidMethod.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-CustomBidMatrix.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-CustomBidMatrix.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-CustomBidMethod.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-CustomBidMethod.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-MultiScenarioMatrix.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-MultiScenarioMatrix.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-PriceArea.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-PriceArea.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-SHOPMultiScenarioMethod.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-SHOPMultiScenarioMethod.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-SHOPPriceScenario.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-SHOPPriceScenario.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-SHOPPriceScenarioResult.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-SHOPPriceScenarioResult.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-WaterValueBasedMethod.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-WaterValueBasedMethod.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/all_DayAhead.datamodel.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/all_DayAhead.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/all_PowerOps.datamodel.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/all_PowerOps.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/compute_DayAheadBenchmarking.datamodel.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/compute_DayAheadBenchmarking.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/compute_SHOPBasedDayAhead.datamodel.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/compute_SHOPBasedDayAhead.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/compute_TotalBidMatrixCalculation.datamodel.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/compute_TotalBidMatrixCalculation.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/compute_WaterValueBasedDayAhead.datamodel.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/compute_WaterValueBasedDayAhead.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/config_DayAheadConfiguration.datamodel.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/config_DayAheadConfiguration.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/config_Resync.datamodel.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/config_Resync.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/Alert.container.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/Alert.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidConfiguration.container.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidConfiguration.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidDocument.container.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidDocument.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidMatrix.container.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidMatrix.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidRow.container.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidRow.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/EfficiencyCurve.container.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/EfficiencyCurve.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/FunctionData.container.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/FunctionData.container.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -163,14 +163,15 @@
       list: false
       type: sequence
     nullable: true
     autoIncrement: false
     name: sequence
   flag:
     type:
+      list: false
       type: boolean
     nullable: true
     autoIncrement: false
     name: flag
 indexes:
   functionNameIndex:
     properties:
```

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/Generator.container.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/Generator.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/MarketConfiguration.container.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/MarketConfiguration.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PartialBidConfiguration.container.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PartialBidConfiguration.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PlantWaterValueBased.container.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PlantWaterValueBased.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PowerAsset.container.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PowerAsset.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PriceAreaAFRR.container.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PriceAreaAFRR.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PriceAreaDayAhead.container.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PriceAreaDayAhead.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PriceProduction.container.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PriceProduction.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/SHOPResult.container.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/SHOPResult.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/SHOPTimeSeries.container.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/SHOPTimeSeries.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopAttributeMapping.container.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopAttributeMapping.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopCase.container.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopCase.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopFile.container.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopFile.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopModel.container.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopModel.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopScenario.container.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopScenario.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopScenarioSet.container.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopScenarioSet.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/frontend_AFRRBid.datamodel.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/frontend_AFRRBid.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/frontend_Asset.datamodel.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/frontend_Asset.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/frontend_DayAheadBid.datamodel.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/frontend_DayAheadBid.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/node_types/power-ops-types.powerops_nodes.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/node_types/power-ops-types.powerops_nodes.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/product_CogShop.datamodel.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/product_CogShop.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/BidRow.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/BidRow.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/MarketConfiguration.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/MarketConfiguration.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/alerts/1-interface.Alert.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/alerts/1-interface.Alert.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/alerts/ShopPenaltyReport.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/alerts/ShopPenaltyReport.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/1-interface.PowerAsset.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/1-interface.PowerAsset.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/generator/Generator.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/generator/Generator.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/generator/GeneratorEfficiencyCurve.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/generator/GeneratorEfficiencyCurve.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/generator/TurbineEfficiencyCurve.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/generator/TurbineEfficiencyCurve.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/plant/1-interface.Plant.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/plant/1-interface.Plant.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/plant/PlantInformation.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/plant/PlantInformation.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/plant/PlantWaterValueBased.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/plant/PlantWaterValueBased.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/1-interface.PriceArea.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/1-interface.PriceArea.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/PriceAreaAFRR.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/PriceAreaAFRR.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/PriceAreaDayAhead.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/PriceAreaDayAhead.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/PriceAreaInformation.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/PriceAreaInformation.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/watercourse/1-interface.Watercourse.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/watercourse/1-interface.Watercourse.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/1-interface.PartialBidConfiguration.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/1-interface.PartialBidConfiguration.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/BidConfigurationDayAhead.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/BidConfigurationDayAhead.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/ShopBasedPartialBidConfiguration.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/ShopBasedPartialBidConfiguration.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/WaterValueBasedPartialBidConfiguration.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/WaterValueBasedPartialBidConfiguration.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/1-interface.BidDocument.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/1-interface.BidDocument.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/BidDocumentAFRR.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/BidDocumentAFRR.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/BidDocumentDayAhead.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/BidDocumentDayAhead.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/BidDocumentDayAheadSimple.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/BidDocumentDayAheadSimple.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/1-interface.BidMatrix.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/1-interface.BidMatrix.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/1-interface.BidMatrixInformation.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/1-interface.BidMatrixInformation.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/1-interface.PartialBidMatrixInformation.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/1-interface.PartialBidMatrixInformation.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/PartialBidMatrixInformationWithScenarios.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/PartialBidMatrixInformationWithScenarios.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopAttributeMapping.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopAttributeMapping.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopCase.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopCase.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopCommands.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopCommands.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopFile.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopFile.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopModel.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopModel.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopScenario.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopScenario.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopScenarioSet.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopScenarioSet.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/1-interface.FunctionInput.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/1-interface.FunctionInput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/1-interface.PartialBidMatrixCalculationInput.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/1-interface.PartialBidMatrixCalculationInput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/BenchmarkingCollectorInput.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/BenchmarkingCollectorInput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/ShopPartialBidMatrixCalculationInput.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/ShopPartialBidMatrixCalculationInput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/ShopPreprocessorInput.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/ShopPreprocessorInput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/ShopTriggerInput.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/ShopTriggerInput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/TaskDispatcherBenchmarkingInput.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/TaskDispatcherBenchmarkingInput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/TaskDispatcherInput.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/TaskDispatcherInput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/TotalBidMatrixCalculationInput.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/TotalBidMatrixCalculationInput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/WaterPartialBidMatrixCalculationInput.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/WaterPartialBidMatrixCalculationInput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/1-interface.FunctionOutput.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/1-interface.FunctionOutput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/BenchmarkingCollectorOutput.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/BenchmarkingCollectorOutput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/PartialBidMatrixCalculationOutput.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/PartialBidMatrixCalculationOutput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/SHOPTriggerOutput.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/SHOPTriggerOutput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/ShopPreprocessorOutput.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/ShopPreprocessorOutput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/TaskDispatcherBenchmarkingOutput.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/TaskDispatcherBenchmarkingOutput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/TaskDispatcherOutput.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/TaskDispatcherOutput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/TotalBidMatrixCalculationOutput.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/TotalBidMatrixCalculationOutput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/PriceProduction.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/PriceProduction.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/SHOPResult.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/SHOPResult.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/SHOPTimeSeries.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/SHOPTimeSeries.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/ShopObjectiveValue.view.yaml` & `cognite_power_ops-0.94.4/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/ShopObjectiveValue.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/prerun_transformations/transformations.py` & `cognite_power_ops-0.94.4/cognite/powerops/prerun_transformations/transformations.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/config/__init__.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/config/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/config/_main.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/config/_main.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/config/_settings.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/config/_settings.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/config/_shared.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/config/_shared.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/config/cogshop/shop_file_config.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/config/cogshop/shop_file_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/config/market/__init__.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/config/market/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/config/market/_core.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/config/market/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/config/market/benchmarking.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/config/market/benchmarking.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/config/market/dayahead.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/config/market/dayahead.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/config/market/market.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/config/market/market.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/config/market/rkom.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/config/market/rkom.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/config/production/connections.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/config/production/connections.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/config/production/generator.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/config/production/generator.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/config/production/plant.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/config/production/plant.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/config/production/watercourse.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/config/production/watercourse.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/core/cdf.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/core/cdf.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/core/main.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/core/main.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/core/transform.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/core/transform.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/core/validation.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/core/validation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/diff/core.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/diff/core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/diff/data_classes.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/diff/data_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/models/_shared_v1_v2/_to_instances.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/models/_shared_v1_v2/_to_instances.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/models/_shared_v1_v2/cogshop_model.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/models/_shared_v1_v2/cogshop_model.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/models/_shared_v1_v2/market_model.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/models/_shared_v1_v2/market_model.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/models/_shared_v1_v2/production_model.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/models/_shared_v1_v2/production_model.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/models/base/__init__.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/models/base/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/models/base/asset_model.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/models/base/asset_model.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/models/base/asset_type.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/models/base/asset_type.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/models/base/cdf_resources.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/models/base/cdf_resources.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/models/base/data_model.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/models/base/data_model.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/models/base/dms_models.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/models/base/dms_models.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/models/base/graph_ql.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/models/base/graph_ql.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/models/base/model.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/models/base/model.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/models/base/resource_type.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/models/base/resource_type.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/models/v1/__init__.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/models/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/models/v1/cogshop.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/models/v1/cogshop.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/models/v1/config_to_model/to_cogshop_model.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/models/v1/config_to_model/to_cogshop_model.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/models/v1/config_to_model/to_market_model.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/models/v1/config_to_model/to_market_model.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/models/v1/config_to_model/to_production_model.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/models/v1/config_to_model/to_production_model.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/models/v1/graphql_schemas/cogshop1.graphql` & `cognite_power_ops-0.94.4/cognite/powerops/resync/models/v1/graphql_schemas/cogshop1.graphql`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/models/v1/market/__init__.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/models/v1/market/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/models/v1/market/base.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/models/v1/market/base.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/models/v1/market/benchmark.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/models/v1/market/benchmark.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/models/v1/market/dayahead.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/models/v1/market/dayahead.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/models/v1/market/rkom.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/models/v1/market/rkom.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/models/v1/production.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/models/v1/production.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/models/v2/config_to_model/to_powerasset_model.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/models/v2/config_to_model/to_powerasset_model.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/models/v2/powerops_models.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/models/v2/powerops_models.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/models/v2/production_dm.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/models/v2/production_dm.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/time_series_mapping/mapping.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/time_series_mapping/mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/time_series_mapping/static_mapping.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/time_series_mapping/static_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/v1/README.md` & `cognite_power_ops-0.94.4/cognite/powerops/resync/v1/README.md`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/v1/config_to_fdm.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/v1/config_to_fdm.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,19 +202,20 @@
 
         # join all dictionaries together in priority order
         parsed_data = self._join_data_by_parsing_method(immutable_data, parsed_properties, parsed_reference_data)
 
         # TODO: handle these special cases in a better way
         if type_configuration.type_ is v1_data_classes.PlantWaterValueBasedWrite:
             # TODO: remove when model is updated to a list instead of json
-            raw_penstock_head_loss_factor = parsed_data["penstock_head_loss_factors"]
-            parsed_data["penstock_head_loss_factors"] = {
-                str(index): float(loss_factor)
-                for index, loss_factor in enumerate(raw_penstock_head_loss_factor, start=1)
-            }
+            raw_penstock_head_loss_factors = parsed_data["penstock_head_loss_factors"]
+            if raw_penstock_head_loss_factors:
+                parsed_data["penstock_head_loss_factors"] = {
+                    str(index): float(loss_factor)
+                    for index, loss_factor in enumerate(raw_penstock_head_loss_factors, start=1)
+                }
 
             parsed_data["generators"] = (
                 self._get_all_connections(parsed_data, "plant", "generator")
                 if "generators" not in parsed_data
                 else parsed_data["generators"]
             )
             parsed_data["connection_losses"] = (
@@ -379,23 +380,31 @@
             power_asset_type_a: A string of the first power asset type to filter the connections.
             power_asset_type_b: A string of the second power asset type to filter the connections.
 
         Returns:
             connections: A list of all connections external ids based on the provided data and asset types.
         """
 
-        all_connections = self._get_property_value_from_source(
-            PropertyConfiguration(
-                property="connections",
-                source_file=Path("files/model.yaml"),
-                extraction_path="connections",
-                cast_type=None,
-            ),
-            data,
-        )
+        all_connections = []
+        source_files = set()
+        for dm_config in self.data_model_configuration.values():
+            for property_config in dm_config.property_configurations:
+                if property_config.source_file:
+                    source_files.add(property_config.source_file)
+
+        for source_file in source_files:
+            all_connections += self._get_property_value_from_source(
+                PropertyConfiguration(
+                    property="connections",
+                    source_file=source_file,
+                    extraction_path="connections",
+                    cast_type=None,
+                ),
+                data,
+            )
         connections = []
 
         name = data["name"]
 
         for connection in all_connections:
             if (
                 connection["from"] == name
@@ -464,15 +473,17 @@
         if instance_data is None:
             instance_data = {}
         if not source_data:
             if property_configuration.source_file:
                 path = self.working_directory / Path(property_configuration.source_file)
                 source_data = load_yaml(path, "dict")
             else:
-                raise ValueError("No source data provided for property configuration")
+                if property_configuration.default_value:
+                    return property_configuration.default_value
+                raise ValueError("No source data or default value provided for property configuration")
 
         try:
             for key in property_configuration.extraction_path or []:
                 match = re.match(r"\[(\w+)\]", key)
                 if key == "value":
                     # TODO: handle value and key to not use next(iter)??
                     if isinstance(source_data, dict):
@@ -575,15 +586,16 @@
             ValueError: Type is not supported, add import to type
             ValueError: Property configuration requires a cast_type
         """
 
         if instance_data is None:
             instance_data = {}
         list_data = self._get_property_value_from_source(property_configuration, instance_data)
-
+        if not list_data:
+            return []
         if property_configuration.cast_type not in self.data_model_configuration:
             raise ValueError(f"Type {property_configuration.cast_type} is not supported, add import to type")
         subtype_data_model_configuration = self.data_model_configuration[property_configuration.cast_type]
 
         parsed_list_data = []
         for source_data in list_data:
             subtype_data = {}
```

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/v1/data_classes.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/v1/data_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/v1/main.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/v1/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     data_model_classes = get_data_model_write_classes(client.v1)
 
     resync_importer = ResyncImporter.from_yaml(configuration, data_model_classes, client.cdf)
     resync_data_model_objects, external_ids = resync_importer.to_data_model()
 
     logger.info(resync_data_model_objects)
-    logger.info(f"Generated {len(resync_data_model_objects)} bid configurations")
+    logger.info(f"Generated {len(resync_data_model_objects)} objects")
     logger.info(f"External IDs: {external_ids}")
 
 
 def apply(configuration: Path, client: PowerOpsClient | None = None) -> None:
     """Generates data model objects from a resync configuration and upserts them to CDF.
 
     Initializes a ResyncImporter given the input configuration path. The importer is then used to generate data model
@@ -57,8 +57,8 @@
 
     # TODO: check all linked sources exist
     check_all_linked_sources_exist(resync_data_model_objects, file_external_ids, [], external_ids)
 
     logger.info(resync_data_model_objects)
     client.v1.upsert(resync_data_model_objects, replace=resync_importer.overwrite_data)
 
-    logger.info(f"Upserted {len(resync_data_model_objects)} bid configurations")
+    logger.info(f"Upserted {len(resync_data_model_objects)} objects")
```

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/v1/utils.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/v1/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/resync/validation.py` & `cognite_power_ops-0.94.4/cognite/powerops/resync/validation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/utils/cdf/_cdf_auth.py` & `cognite_power_ops-0.94.4/cognite/powerops/utils/cdf/_cdf_auth.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/utils/cdf/_settings.py` & `cognite_power_ops-0.94.4/cognite/powerops/utils/cdf/_settings.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/utils/cdf/calls.py` & `cognite_power_ops-0.94.4/cognite/powerops/utils/cdf/calls.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/utils/cdf/extraction_pipelines.py` & `cognite_power_ops-0.94.4/cognite/powerops/utils/cdf/extraction_pipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/utils/cdf/resource_creation.py` & `cognite_power_ops-0.94.4/cognite/powerops/utils/cdf/resource_creation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/utils/lookup.py` & `cognite_power_ops-0.94.4/cognite/powerops/utils/lookup.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/utils/navigation.py` & `cognite_power_ops-0.94.4/cognite/powerops/utils/navigation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/utils/require.py` & `cognite_power_ops-0.94.4/cognite/powerops/utils/require.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/utils/retry/api.py` & `cognite_power_ops-0.94.4/cognite/powerops/utils/retry/api.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/utils/serialization.py` & `cognite_power_ops-0.94.4/cognite/powerops/utils/serialization.py`

 * *Files 6% similar despite different names*

```diff
@@ -203,16 +203,28 @@
         data = re.sub(rf"[{'|'.join(invalid_characters)}]", UNRECOGNIZABLE_CHARACTER, data)
         warnings.warn(
             f"File {yaml_path.parent}/{yaml_path.name} contains invalid characters: {', '.join(invalid_characters)}",
             stacklevel=2,
         )
     output = CSafeLoader(data).get_data()
     if expected_return_type == "dict" and not isinstance(output, dict):
+        if not output:
+            warnings.warn(
+                f"File {yaml_path.parent}/{yaml_path.name} contains no data",
+                stacklevel=2,
+            )
+            return {}
         raise ValueError(f"Expected a dictionary, got {type(output)}")
     if expected_return_type == "list" and not isinstance(output, list):
+        if not output:
+            warnings.warn(
+                f"File {yaml_path.parent}/{yaml_path.name} contains no data",
+                stacklevel=2,
+            )
+            return []
         raise ValueError(f"Expected a list, got {type(output)}")
     return output
 
 
 def dump_yaml(yaml_path: Path, data: dict, encoding="utf-8") -> None:
     """
     Dump a dictionary to a yaml file.
```

### Comparing `cognite_power_ops-0.94.3/cognite/powerops/utils/time.py` & `cognite_power_ops-0.94.4/cognite/powerops/utils/time.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.3/pyproject.toml` & `cognite_power_ops-0.94.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-power-ops"
-version = "0.94.3"
+version = "0.94.4"
 description = "SDK for power markets operations on Cognite Data Fusion"
 readme = "README.md"
 authors = ["Cognite <support@cognite.com>"]
 license = "Apache 2.0"
 documentation = "https://cognite-power-ops-sdk.readthedocs-hosted.com/en/latest/"
 homepage = "https://cognite-power-ops-sdk.readthedocs-hosted.com/en/latest/"
 repository = "https://github.com/cognitedata/power-ops-sdk"
```

### Comparing `cognite_power_ops-0.94.3/PKG-INFO` & `cognite_power_ops-0.94.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-power-ops
-Version: 0.94.3
+Version: 0.94.4
 Summary: SDK for power markets operations on Cognite Data Fusion
 Home-page: https://cognite-power-ops-sdk.readthedocs-hosted.com/en/latest/
 License: Apache 2.0
 Author: Cognite
 Author-email: support@cognite.com
 Requires-Python: >=3.9,<3.13
 Classifier: License :: Other/Proprietary License
```

